# Comparing `tmp/django_sql_explorer-4.2.tar.gz` & `tmp/django_sql_explorer-4.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sql_explorer-4.2.tar", last modified: Fri Apr 26 14:15:38 2024, max compression
+gzip compressed data, was "django_sql_explorer-4.2b1.tar", last modified: Thu Apr 25 21:16:35 2024, max compression
```

## Comparing `django_sql_explorer-4.2.tar` & `django_sql_explorer-4.2b1.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.664281 django_sql_explorer-4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-26 14:15:38.664281 django_sql_explorer-4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.664281 django_sql_explorer-4.2/django_sql_explorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-26 14:15:38.000000 django_sql_explorer-4.2/django_sql_explorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-26 14:15:38.000000 django_sql_explorer-4.2/django_sql_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:15:38.000000 django_sql_explorer-4.2/django_sql_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:15:38.000000 django_sql_explorer-4.2/django_sql_explorer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-26 14:15:38.000000 django_sql_explorer-4.2/django_sql_explorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 14:15:38.000000 django_sql_explorer-4.2/django_sql_explorer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.644281 django_sql_explorer-4.2/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.644281 django_sql_explorer-4.2/explorer/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/assistant/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/assistant/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/assistant/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/assistant/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/assistant/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.636281 django_sql_explorer-4.2/explorer/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.636281 django_sql_explorer-4.2/explorer/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.644281 django_sql_explorer-4.2/explorer/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10091 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.636281 django_sql_explorer-4.2/explorer/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.644281 django_sql_explorer-4.2/explorer/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.648281 django_sql_explorer-4.2/explorer/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0002_auto_20150501_1515.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0003_query_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0004_querylog_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0005_auto_20160105_2052.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0006_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0007_querylog_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0008_auto_20190308_1642.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0009_auto_20201009_0547.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0010_sql_required.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0011_query_favorites.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0013_querylog_error_querylog_success.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0014_promptlog.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/0015_explorervalue.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.636281 django_sql_explorer-4.2/explorer/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.648281 django_sql_explorer-4.2/explorer/src/js/
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/js/assistant.js
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/js/codemirror-config.js
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/js/csrf.js
--rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/js/explorer.js
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/js/favorites.js
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/js/pivot-setup.js
--rw-r--r--   0 runner    (1001) docker     (127)    77235 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/js/pivot.js
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/js/query-list.js
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/js/schema.js
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/js/table-to-csv.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.652281 django_sql_explorer-4.2/explorer/src/scss/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/scss/assistant.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/scss/explorer.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/scss/pivot.css
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/scss/styles.scss
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/src/scss/variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.636281 django_sql_explorer-4.2/explorer/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.652281 django_sql_explorer-4.2/explorer/static/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)   176088 2024-04-26 14:15:35.000000 django_sql_explorer-4.2/explorer/static/explorer/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   130648 2024-04-26 14:15:35.000000 django_sql_explorer-4.2/explorer/static/explorer/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   546031 2024-04-26 14:15:35.000000 django_sql_explorer-4.2/explorer/static/explorer/explorer.js
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-26 14:15:35.000000 django_sql_explorer-4.2/explorer/static/explorer/favorites.js
--rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-26 14:15:35.000000 django_sql_explorer-4.2/explorer/static/explorer/index.js
--rw-r--r--   0 runner    (1001) docker     (127)    84338 2024-04-26 14:15:35.000000 django_sql_explorer-4.2/explorer/static/explorer/main.js
--rw-r--r--   0 runner    (1001) docker     (127)    66999 2024-04-26 14:15:35.000000 django_sql_explorer-4.2/explorer/static/explorer/pivot-setup.js
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-26 14:15:35.000000 django_sql_explorer-4.2/explorer/static/explorer/query-list.js
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-26 14:15:35.000000 django_sql_explorer-4.2/explorer/static/explorer/schema.js
--rw-r--r--   0 runner    (1001) docker     (127)   308829 2024-04-26 14:15:35.000000 django_sql_explorer-4.2/explorer/static/explorer/styles.css
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.636281 django_sql_explorer-4.2/explorer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.656281 django_sql_explorer-4.2/explorer/templates/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/assistant.html
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/export_buttons.html
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/fullscreen.html
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/params.html
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/pdf_template.html
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/play.html
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/preview_pane.html
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/query.html
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/query_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/query_favorite_button.html
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/query_favorites.html
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/query_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/querylog_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/schema.html
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templates/explorer/schema_building.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.656281 django_sql_explorer-4.2/explorer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templatetags/explorer_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/templatetags/vite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.660281 django_sql_explorer-4.2/explorer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tests/test_csrf_cookie_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tests/test_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    32205 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.664281 django_sql_explorer-4.2/explorer/views/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/export.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/format_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/query_favorite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/explorer/views/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.664281 django_sql_explorer-4.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/requirements/dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:15:38.664281 django_sql_explorer-4.2/requirements/extra/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/requirements/extra/assistant.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/requirements/extra/charts.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/requirements/extra/snapshots.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/requirements/extra/xls.txt
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-26 14:15:38.668281 django_sql_explorer-4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-26 14:15:23.000000 django_sql_explorer-4.2/vite.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.202532 django_sql_explorer-4.2b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-25 21:16:35.202532 django_sql_explorer-4.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.202532 django_sql_explorer-4.2b1/django_sql_explorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-25 21:16:35.000000 django_sql_explorer-4.2b1/django_sql_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-25 21:16:35.000000 django_sql_explorer-4.2b1/django_sql_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:16:35.000000 django_sql_explorer-4.2b1/django_sql_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:16:34.000000 django_sql_explorer-4.2b1/django_sql_explorer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-25 21:16:35.000000 django_sql_explorer-4.2b1/django_sql_explorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 21:16:35.000000 django_sql_explorer-4.2b1/django_sql_explorer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.178532 django_sql_explorer-4.2b1/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.182532 django_sql_explorer-4.2b1/explorer/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/assistant/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/assistant/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/assistant/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/assistant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/assistant/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.170532 django_sql_explorer-4.2b1/explorer/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.170532 django_sql_explorer-4.2b1/explorer/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.182532 django_sql_explorer-4.2b1/explorer/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10091 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.170532 django_sql_explorer-4.2b1/explorer/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.182532 django_sql_explorer-4.2b1/explorer/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.186532 django_sql_explorer-4.2b1/explorer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0002_auto_20150501_1515.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0003_query_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0004_querylog_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0005_auto_20160105_2052.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0006_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0007_querylog_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0008_auto_20190308_1642.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0009_auto_20201009_0547.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0010_sql_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0011_query_favorites.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0013_querylog_error_querylog_success.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0014_promptlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/0015_explorervalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.174532 django_sql_explorer-4.2b1/explorer/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.186532 django_sql_explorer-4.2b1/explorer/src/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/assistant.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/codemirror-config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/csrf.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/explorer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/favorites.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/pivot-setup.js
+-rw-r--r--   0 runner    (1001) docker     (127)    77235 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/pivot.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/query-list.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/schema.js
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/js/table-to-csv.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.186532 django_sql_explorer-4.2b1/explorer/src/scss/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/scss/assistant.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/scss/explorer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/scss/pivot.css
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/scss/styles.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/src/scss/variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.174532 django_sql_explorer-4.2b1/explorer/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.190532 django_sql_explorer-4.2b1/explorer/static/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)   176088 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   130648 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   546527 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/explorer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/favorites.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    84338 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    66999 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/pivot-setup.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/query-list.js
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/schema.js
+-rw-r--r--   0 runner    (1001) docker     (127)   308829 2024-04-25 21:16:31.000000 django_sql_explorer-4.2b1/explorer/static/explorer/styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.174532 django_sql_explorer-4.2b1/explorer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.194532 django_sql_explorer-4.2b1/explorer/templates/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/assistant.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/export_buttons.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/fullscreen.html
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/params.html
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/pdf_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/play.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/preview_pane.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/query.html
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/query_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/query_favorite_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/query_favorites.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/query_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/querylog_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/schema.html
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templates/explorer/schema_building.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.194532 django_sql_explorer-4.2b1/explorer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templatetags/explorer_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/templatetags/vite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.198532 django_sql_explorer-4.2b1/explorer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_csrf_cookie_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32205 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.202532 django_sql_explorer-4.2b1/explorer/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/format_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/query_favorite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/explorer/views/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.202532 django_sql_explorer-4.2b1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/requirements/dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:16:35.202532 django_sql_explorer-4.2b1/requirements/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/requirements/extra/assistant.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/requirements/extra/charts.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/requirements/extra/snapshots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/requirements/extra/xls.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-25 21:16:35.206532 django_sql_explorer-4.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-25 21:16:18.000000 django_sql_explorer-4.2b1/vite.config.js
```

### Comparing `django_sql_explorer-4.2/AUTHORS` & `django_sql_explorer-4.2b1/AUTHORS`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/LICENSE` & `django_sql_explorer-4.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/PKG-INFO` & `django_sql_explorer-4.2b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sql-explorer
-Version: 4.2
+Version: 4.2b1
 Summary: A pluggable app that allows users (admins) to execute SQL, view, and export the results.
 Home-page: https://www.sqlexplorer.io
 Author: Chris Clark
 Author-email: chris@untrod.com
 Maintainer: Mark Walker
 Maintainer-email: theshow@gmail.com
 License: MIT
```

### Comparing `django_sql_explorer-4.2/README.rst` & `django_sql_explorer-4.2b1/README.rst`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/django_sql_explorer.egg-info/PKG-INFO` & `django_sql_explorer-4.2b1/django_sql_explorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sql-explorer
-Version: 4.2
+Version: 4.2b1
 Summary: A pluggable app that allows users (admins) to execute SQL, view, and export the results.
 Home-page: https://www.sqlexplorer.io
 Author: Chris Clark
 Author-email: chris@untrod.com
 Maintainer: Mark Walker
 Maintainer-email: theshow@gmail.com
 License: MIT
```

### Comparing `django_sql_explorer-4.2/django_sql_explorer.egg-info/SOURCES.txt` & `django_sql_explorer-4.2b1/django_sql_explorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/__init__.py` & `django_sql_explorer-4.2b1/explorer/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __version_info__ = {
     "major": 4,
     "minor": 2,
     "patch": 0,
-    "releaselevel": "final",
-    "serial": 0
+    "releaselevel": "beta",
+    "serial": 1
 }
 
 
 def get_version(short=False):
     assert __version_info__["releaselevel"] in ("alpha", "beta", "final")
     vers = ["%(major)i.%(minor)i" % __version_info__, ]
     if __version_info__["patch"]:
```

### Comparing `django_sql_explorer-4.2/explorer/actions.py` & `django_sql_explorer-4.2b1/explorer/actions.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/app_settings.py` & `django_sql_explorer-4.2b1/explorer/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/apps.py` & `django_sql_explorer-4.2b1/explorer/apps.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/assistant/models.py` & `django_sql_explorer-4.2b1/explorer/assistant/models.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/assistant/prompts.py` & `django_sql_explorer-4.2b1/explorer/assistant/prompts.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/assistant/tests.py` & `django_sql_explorer-4.2b1/explorer/assistant/tests.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/assistant/utils.py` & `django_sql_explorer-4.2b1/explorer/assistant/utils.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/assistant/views.py` & `django_sql_explorer-4.2b1/explorer/assistant/views.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/charts.py` & `django_sql_explorer-4.2b1/explorer/charts.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/connections.py` & `django_sql_explorer-4.2b1/explorer/connections.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/exporters.py` & `django_sql_explorer-4.2b1/explorer/exporters.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/forms.py` & `django_sql_explorer-4.2b1/explorer/forms.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/locale/ru/LC_MESSAGES/django.mo` & `django_sql_explorer-4.2b1/explorer/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/locale/ru/LC_MESSAGES/django.po` & `django_sql_explorer-4.2b1/explorer/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_sql_explorer-4.2b1/explorer/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/locale/zh_Hans/LC_MESSAGES/django.po` & `django_sql_explorer-4.2b1/explorer/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/migrations/0001_initial.py` & `django_sql_explorer-4.2b1/explorer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/migrations/0009_auto_20201009_0547.py` & `django_sql_explorer-4.2b1/explorer/migrations/0009_auto_20201009_0547.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/migrations/0011_query_favorites.py` & `django_sql_explorer-4.2b1/explorer/migrations/0011_query_favorites.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py` & `django_sql_explorer-4.2b1/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/migrations/0013_querylog_error_querylog_success.py` & `django_sql_explorer-4.2b1/explorer/migrations/0013_querylog_error_querylog_success.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/migrations/0014_promptlog.py` & `django_sql_explorer-4.2b1/explorer/migrations/0014_promptlog.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/migrations/0015_explorervalue.py` & `django_sql_explorer-4.2b1/explorer/migrations/0015_explorervalue.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/models.py` & `django_sql_explorer-4.2b1/explorer/models.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/permissions.py` & `django_sql_explorer-4.2b1/explorer/permissions.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/schema.py` & `django_sql_explorer-4.2b1/explorer/schema.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/src/js/assistant.js` & `django_sql_explorer-4.2b1/explorer/src/js/assistant.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -10,14 +10,18 @@
 import List from "list.js";
 
 function getErrorMessage() {
     const errorElement = document.querySelector('.alert-danger.db-error');
     return errorElement ? errorElement.textContent.trim() : null;
 }
 
+function assistantSearchFocus() {
+    document.getElementById("search_assistant_tables").focus();
+}
+
 export function setUpAssistant(expand = false) {
 
     const error = getErrorMessage();
 
     if (expand || error) {
         const myCollapseElement = document.getElementById('assistant_collapse');
         const bsCollapse = new bootstrap.Collapse(myCollapseElement, {
@@ -67,14 +71,35 @@
 
             new List('additional_table_container', options);
         })
         .catch(error => {
             console.error('Error retrieving JSON schema:', error);
         });
 
+    const checkbox = document.getElementById('include_other_tables');
+    const additionalTableContainer = document.getElementById('additional_table_container');
+    const assistantInputWrapper = document.getElementById('assistant_input_wrapper');
+
+    function showHideExtraTables(checked) {
+        if (checked) {
+            additionalTableContainer.classList.remove('d-none');
+            assistantInputWrapper.classList.remove('col-12');
+            assistantInputWrapper.classList.add('col-9');
+            assistantSearchFocus();
+        } else {
+            additionalTableContainer.classList.add('d-none');
+            assistantInputWrapper.classList.remove('col-9');
+            assistantInputWrapper.classList.add('col-12');
+        }
+    }
+    checkbox.addEventListener('change', function() {
+        showHideExtraTables(this.checked);
+    });
+    showHideExtraTables(checkbox.checked);
+
     document.getElementById('id_assistant_input').addEventListener('keydown', function(event) {
         if ((event.ctrlKey || event.metaKey) && (event.key === 'Enter')) {
             event.preventDefault();
             submitAssistantAsk();
         }
     });
```

### Comparing `django_sql_explorer-4.2/explorer/src/js/codemirror-config.js` & `django_sql_explorer-4.2b1/explorer/src/js/codemirror-config.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/src/js/explorer.js` & `django_sql_explorer-4.2b1/explorer/src/js/explorer.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/src/js/favorites.js` & `django_sql_explorer-4.2b1/explorer/src/js/favorites.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/src/js/main.js` & `django_sql_explorer-4.2b1/explorer/src/js/main.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/src/js/pivot-setup.js` & `django_sql_explorer-4.2b1/explorer/src/js/pivot-setup.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/src/js/pivot.js` & `django_sql_explorer-4.2b1/explorer/src/js/pivot.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/src/js/query-list.js` & `django_sql_explorer-4.2b1/explorer/src/js/query-list.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/src/js/schema.js` & `django_sql_explorer-4.2b1/explorer/src/js/schema.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/src/js/table-to-csv.js` & `django_sql_explorer-4.2b1/explorer/src/js/table-to-csv.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/src/scss/assistant.scss` & `django_sql_explorer-4.2b1/explorer/src/scss/assistant.scss`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     top: 5px;
     right: 5px;
     cursor: pointer;
 }
 
 #additional_table_container {
     overflow-y: auto;
-    max-height: 10rem;
+    max-height: 120px;
 }
 
 #assistant_input_parent {
     max-height: 120px;
     overflow: hidden;
 }
```

### Comparing `django_sql_explorer-4.2/explorer/src/scss/explorer.scss` & `django_sql_explorer-4.2b1/explorer/src/scss/explorer.scss`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/src/scss/pivot.css` & `django_sql_explorer-4.2b1/explorer/src/scss/pivot.css`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/static/explorer/bootstrap-icons.woff` & `django_sql_explorer-4.2b1/explorer/static/explorer/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/static/explorer/bootstrap-icons.woff2` & `django_sql_explorer-4.2b1/explorer/static/explorer/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/static/explorer/explorer.js` & `django_sql_explorer-4.2b1/explorer/static/explorer/explorer.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -69,16 +69,16 @@
             } : function(a) {
                 return i.concat.apply([], a)
             },
             l = i.push,
             h = i.indexOf,
             f = {},
             u = f.toString,
-            g = f.hasOwnProperty,
-            y = g.toString,
+            m = f.hasOwnProperty,
+            y = m.toString,
             k = y.call(Object),
             v = {},
             A = function(c) {
                 return typeof c == "function" && typeof c.nodeType != "number" && typeof c.item != "function"
             },
             O = function(c) {
                 return c != null && c === c.window
@@ -89,17 +89,17 @@
                 src: !0,
                 nonce: !0,
                 noModule: !0
             };
 
         function $(a, c, d) {
             d = d || D;
-            var m, b, x = d.createElement("script");
+            var g, b, x = d.createElement("script");
             if (x.text = a, c)
-                for (m in F) b = c[m] || c.getAttribute && c.getAttribute(m), b && x.setAttribute(m, b);
+                for (g in F) b = c[g] || c.getAttribute && c.getAttribute(g), b && x.setAttribute(g, b);
             d.head.appendChild(x).parentNode.removeChild(x)
         }
 
         function j(a) {
             return a == null ? a + "" : typeof a == "object" || typeof a == "function" ? f[u.call(a)] || "object" : typeof a
         }
         var z = "3.7.1",
@@ -156,58 +156,58 @@
             end: function() {
                 return this.prevObject || this.constructor()
             },
             push: l,
             sort: i.sort,
             splice: i.splice
         }, p.extend = p.fn.extend = function() {
-            var a, c, d, m, b, x, w = arguments[0] || {},
+            var a, c, d, g, b, x, w = arguments[0] || {},
                 T = 1,
                 C = arguments.length,
                 E = !1;
             for (typeof w == "boolean" && (E = w, w = arguments[T] || {}, T++), typeof w != "object" && !A(w) && (w = {}), T === C && (w = this, T--); T < C; T++)
                 if ((a = arguments[T]) != null)
-                    for (c in a) m = a[c], !(c === "__proto__" || w === m) && (E && m && (p.isPlainObject(m) || (b = Array.isArray(m))) ? (d = w[c], b && !Array.isArray(d) ? x = [] : !b && !p.isPlainObject(d) ? x = {} : x = d, b = !1, w[c] = p.extend(E, x, m)) : m !== void 0 && (w[c] = m));
+                    for (c in a) g = a[c], !(c === "__proto__" || w === g) && (E && g && (p.isPlainObject(g) || (b = Array.isArray(g))) ? (d = w[c], b && !Array.isArray(d) ? x = [] : !b && !p.isPlainObject(d) ? x = {} : x = d, b = !1, w[c] = p.extend(E, x, g)) : g !== void 0 && (w[c] = g));
             return w
         }, p.extend({
             expando: "jQuery" + (z + Math.random()).replace(/\D/g, ""),
             isReady: !0,
             error: function(a) {
                 throw new Error(a)
             },
             noop: function() {},
             isPlainObject: function(a) {
                 var c, d;
-                return !a || u.call(a) !== "[object Object]" ? !1 : (c = r(a), c ? (d = g.call(c, "constructor") && c.constructor, typeof d == "function" && y.call(d) === k) : !0)
+                return !a || u.call(a) !== "[object Object]" ? !1 : (c = r(a), c ? (d = m.call(c, "constructor") && c.constructor, typeof d == "function" && y.call(d) === k) : !0)
             },
             isEmptyObject: function(a) {
                 var c;
                 for (c in a) return !1;
                 return !0
             },
             globalEval: function(a, c, d) {
                 $(a, {
                     nonce: c && c.nonce
                 }, d)
             },
             each: function(a, c) {
-                var d, m = 0;
+                var d, g = 0;
                 if (he(a))
-                    for (d = a.length; m < d && c.call(a[m], m, a[m]) !== !1; m++);
+                    for (d = a.length; g < d && c.call(a[g], g, a[g]) !== !1; g++);
                 else
-                    for (m in a)
-                        if (c.call(a[m], m, a[m]) === !1) break;
+                    for (g in a)
+                        if (c.call(a[g], g, a[g]) === !1) break;
                 return a
             },
             text: function(a) {
                 var c, d = "",
-                    m = 0,
+                    g = 0,
                     b = a.nodeType;
                 if (!b)
-                    for (; c = a[m++];) d += p.text(c);
+                    for (; c = a[g++];) d += p.text(c);
                 return b === 1 || b === 11 ? a.textContent : b === 9 ? a.documentElement.textContent : b === 3 || b === 4 ? a.nodeValue : d
             },
             makeArray: function(a, c) {
                 var d = c || [];
                 return a != null && (he(Object(a)) ? p.merge(d, typeof a == "string" ? [a] : a) : l.call(d, a)), d
             },
             inArray: function(a, c, d) {
@@ -215,26 +215,26 @@
             },
             isXMLDoc: function(a) {
                 var c = a && a.namespaceURI,
                     d = a && (a.ownerDocument || a).documentElement;
                 return !G.test(c || d && d.nodeName || "HTML")
             },
             merge: function(a, c) {
-                for (var d = +c.length, m = 0, b = a.length; m < d; m++) a[b++] = c[m];
+                for (var d = +c.length, g = 0, b = a.length; g < d; g++) a[b++] = c[g];
                 return a.length = b, a
             },
             grep: function(a, c, d) {
-                for (var m, b = [], x = 0, w = a.length, T = !d; x < w; x++) m = !c(a[x], x), m !== T && b.push(a[x]);
+                for (var g, b = [], x = 0, w = a.length, T = !d; x < w; x++) g = !c(a[x], x), g !== T && b.push(a[x]);
                 return b
             },
             map: function(a, c, d) {
-                var m, b, x = 0,
+                var g, b, x = 0,
                     w = [];
                 if (he(a))
-                    for (m = a.length; x < m; x++) b = c(a[x], x, d), b != null && w.push(b);
+                    for (g = a.length; x < g; x++) b = c(a[x], x, d), b != null && w.push(b);
                 else
                     for (x in a) b = c(a[x], x, d), b != null && w.push(b);
                 return o(w)
             },
             guid: 1,
             support: v
         }), typeof Symbol == "function" && (p.fn[Symbol.iterator] = i[Symbol.iterator]), p.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "), function(a, c) {
@@ -266,15 +266,15 @@
         }
         p.escapeSelector = function(a) {
             return (a + "").replace(Be, st)
         };
         var _e = D,
             Ye = l;
         (function() {
-            var a, c, d, m, b, x = Ye,
+            var a, c, d, g, b, x = Ye,
                 w, T, C, E, I, _ = p.expando,
                 P = 0,
                 W = 0,
                 ce = Gs(),
                 Ae = Gs(),
                 ge = Gs(),
                 ut = Gs(),
@@ -470,15 +470,15 @@
                     if (typeof B.getElementsByClassName != "undefined" && C) return B.getElementsByClassName(N)
                 }, E = [], sr(function(N) {
                     var B;
                     T.appendChild(N).innerHTML = "<a id='" + _ + "' href='' disabled='disabled'></a><select id='" + _ + "-\r\\' disabled='disabled'><option selected=''></option></select>", N.querySelectorAll("[selected]").length || E.push("\\[" + ie + "*(?:value|" + wi + ")"), N.querySelectorAll("[id~=" + _ + "-]").length || E.push("~="), N.querySelectorAll("a#" + _ + "+*").length || E.push(".#.+[+~]"), N.querySelectorAll(":checked").length || E.push(":checked"), B = w.createElement("input"), B.setAttribute("type", "hidden"), N.appendChild(B).setAttribute("name", "D"), T.appendChild(N).disabled = !0, N.querySelectorAll(":disabled").length !== 2 && E.push(":enabled", ":disabled"), B = w.createElement("input"), B.setAttribute("name", ""), N.appendChild(B), N.querySelectorAll("[name='']").length || E.push("\\[" + ie + "*name" + ie + "*=" + ie + `*(?:''|"")`)
                 }), v.cssHas || E.push(":has"), E = E.length && new RegExp(E.join("|")), et = function(N, B) {
                     if (N === B) return b = !0, 0;
                     var U = !N.compareDocumentPosition - !B.compareDocumentPosition;
-                    return U || (U = (N.ownerDocument || N) == (B.ownerDocument || B) ? N.compareDocumentPosition(B) : 1, U & 1 || !v.sortDetached && B.compareDocumentPosition(N) === U ? N === w || N.ownerDocument == _e && Le.contains(_e, N) ? -1 : B === w || B.ownerDocument == _e && Le.contains(_e, B) ? 1 : m ? h.call(m, N) - h.call(m, B) : 0 : U & 4 ? -1 : 1)
+                    return U || (U = (N.ownerDocument || N) == (B.ownerDocument || B) ? N.compareDocumentPosition(B) : 1, U & 1 || !v.sortDetached && B.compareDocumentPosition(N) === U ? N === w || N.ownerDocument == _e && Le.contains(_e, N) ? -1 : B === w || B.ownerDocument == _e && Le.contains(_e, B) ? 1 : g ? h.call(g, N) - h.call(g, B) : 0 : U & 4 ? -1 : 1)
                 }), w
             }
             Le.matches = function(S, M) {
                 return Le(S, null, null, M)
             }, Le.matchesSelector = function(S, M) {
                 if (an(S), C && !ut[M + " "] && (!E || !E.test(M))) try {
                     var L = I.call(S, M);
@@ -488,27 +488,27 @@
                 }
                 return Le(M, w, null, [S]).length > 0
             }, Le.contains = function(S, M) {
                 return (S.ownerDocument || S) != w && an(S), p.contains(S, M)
             }, Le.attr = function(S, M) {
                 (S.ownerDocument || S) != w && an(S);
                 var L = c.attrHandle[M.toLowerCase()],
-                    N = L && g.call(c.attrHandle, M.toLowerCase()) ? L(S, M, !C) : void 0;
+                    N = L && m.call(c.attrHandle, M.toLowerCase()) ? L(S, M, !C) : void 0;
                 return N !== void 0 ? N : S.getAttribute(M)
             }, Le.error = function(S) {
                 throw new Error("Syntax error, unrecognized expression: " + S)
             }, p.uniqueSort = function(S) {
                 var M, L = [],
                     N = 0,
                     B = 0;
-                if (b = !v.sortStable, m = !v.sortStable && s.call(S, 0), pe.call(S, et), b) {
+                if (b = !v.sortStable, g = !v.sortStable && s.call(S, 0), pe.call(S, et), b) {
                     for (; M = S[B++];) M === S[B] && (N = L.push(B));
                     for (; N--;) fe.call(S, L[N], 1)
                 }
-                return m = null, S
+                return g = null, S
             }, p.fn.uniqueSort = function() {
                 return this.pushStack(p.uniqueSort(s.apply(this)))
             }, c = p.expr = {
                 cacheLength: 50,
                 createPseudo: fi,
                 match: Ci,
                 attrHandle: {},
@@ -892,74 +892,74 @@
                 return (xe || Kl(S, le))(N, M, !C, L, !M || jl.test(S) && Vl(M.parentNode) || M), L
             }
             v.sortStable = _.split("").sort(et).join("") === _, an(), v.sortDetached = sr(function(S) {
                 return S.compareDocumentPosition(w.createElement("fieldset")) & 1
             }), p.find = Le, p.expr[":"] = p.expr.pseudos, p.unique = p.uniqueSort, Le.compile = Kl, Le.select = Nc, Le.setDocument = an, Le.tokenize = $r, Le.escape = p.escapeSelector, Le.getText = p.text, Le.isXML = p.isXMLDoc, Le.selectors = p.expr, Le.support = p.support, Le.uniqueSort = p.uniqueSort
         })();
         var be = function(a, c, d) {
-                for (var m = [], b = d !== void 0;
+                for (var g = [], b = d !== void 0;
                     (a = a[c]) && a.nodeType !== 9;)
                     if (a.nodeType === 1) {
                         if (b && p(a).is(d)) break;
-                        m.push(a)
-                    } return m
+                        g.push(a)
+                    } return g
             },
             We = function(a, c) {
                 for (var d = []; a; a = a.nextSibling) a.nodeType === 1 && a !== c && d.push(a);
                 return d
             },
             Ce = p.expr.match.needsContext,
             bt = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
 
         function Oe(a, c, d) {
-            return A(c) ? p.grep(a, function(m, b) {
-                return !!c.call(m, b, m) !== d
-            }) : c.nodeType ? p.grep(a, function(m) {
-                return m === c !== d
-            }) : typeof c != "string" ? p.grep(a, function(m) {
-                return h.call(c, m) > -1 !== d
+            return A(c) ? p.grep(a, function(g, b) {
+                return !!c.call(g, b, g) !== d
+            }) : c.nodeType ? p.grep(a, function(g) {
+                return g === c !== d
+            }) : typeof c != "string" ? p.grep(a, function(g) {
+                return h.call(c, g) > -1 !== d
             }) : p.filter(c, a, d)
         }
         p.filter = function(a, c, d) {
-            var m = c[0];
-            return d && (a = ":not(" + a + ")"), c.length === 1 && m.nodeType === 1 ? p.find.matchesSelector(m, a) ? [m] : [] : p.find.matches(a, p.grep(c, function(b) {
+            var g = c[0];
+            return d && (a = ":not(" + a + ")"), c.length === 1 && g.nodeType === 1 ? p.find.matchesSelector(g, a) ? [g] : [] : p.find.matches(a, p.grep(c, function(b) {
                 return b.nodeType === 1
             }))
         }, p.fn.extend({
             find: function(a) {
-                var c, d, m = this.length,
+                var c, d, g = this.length,
                     b = this;
                 if (typeof a != "string") return this.pushStack(p(a).filter(function() {
-                    for (c = 0; c < m; c++)
+                    for (c = 0; c < g; c++)
                         if (p.contains(b[c], this)) return !0
                 }));
-                for (d = this.pushStack([]), c = 0; c < m; c++) p.find(a, b[c], d);
-                return m > 1 ? p.uniqueSort(d) : d
+                for (d = this.pushStack([]), c = 0; c < g; c++) p.find(a, b[c], d);
+                return g > 1 ? p.uniqueSort(d) : d
             },
             filter: function(a) {
                 return this.pushStack(Oe(this, a || [], !1))
             },
             not: function(a) {
                 return this.pushStack(Oe(this, a || [], !0))
             },
             is: function(a) {
                 return !!Oe(this, typeof a == "string" && Ce.test(a) ? p(a) : a || [], !1).length
             }
         });
         var Tt, yi = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/,
             On = p.fn.init = function(a, c, d) {
-                var m, b;
+                var g, b;
                 if (!a) return this;
                 if (d = d || Tt, typeof a == "string")
-                    if (a[0] === "<" && a[a.length - 1] === ">" && a.length >= 3 ? m = [null, a, null] : m = yi.exec(a), m && (m[1] || !c))
-                        if (m[1]) {
-                            if (c = c instanceof p ? c[0] : c, p.merge(this, p.parseHTML(m[1], c && c.nodeType ? c.ownerDocument || c : D, !0)), bt.test(m[1]) && p.isPlainObject(c))
-                                for (m in c) A(this[m]) ? this[m](c[m]) : this.attr(m, c[m]);
+                    if (a[0] === "<" && a[a.length - 1] === ">" && a.length >= 3 ? g = [null, a, null] : g = yi.exec(a), g && (g[1] || !c))
+                        if (g[1]) {
+                            if (c = c instanceof p ? c[0] : c, p.merge(this, p.parseHTML(g[1], c && c.nodeType ? c.ownerDocument || c : D, !0)), bt.test(g[1]) && p.isPlainObject(c))
+                                for (g in c) A(this[g]) ? this[g](c[g]) : this.attr(g, c[g]);
                             return this
-                        } else return b = D.getElementById(m[2]), b && (this[0] = b, this.length = 1), this;
+                        } else return b = D.getElementById(g[2]), b && (this[0] = b, this.length = 1), this;
                 else return !c || c.jquery ? (c || d).find(a) : this.constructor(c).find(a);
                 else {
                     if (a.nodeType) return this[0] = a, this.length = 1, this;
                     if (A(a)) return d.ready !== void 0 ? d.ready(a) : a(p)
                 }
                 return p.makeArray(a, this)
             };
@@ -972,26 +972,26 @@
                 prev: !0
             };
         p.fn.extend({
             has: function(a) {
                 var c = p(a, this),
                     d = c.length;
                 return this.filter(function() {
-                    for (var m = 0; m < d; m++)
-                        if (p.contains(this, c[m])) return !0
+                    for (var g = 0; g < d; g++)
+                        if (p.contains(this, c[g])) return !0
                 })
             },
             closest: function(a, c) {
-                var d, m = 0,
+                var d, g = 0,
                     b = this.length,
                     x = [],
                     w = typeof a != "string" && p(a);
                 if (!Ce.test(a)) {
-                    for (; m < b; m++)
-                        for (d = this[m]; d && d !== c; d = d.parentNode)
+                    for (; g < b; g++)
+                        for (d = this[g]; d && d !== c; d = d.parentNode)
                             if (d.nodeType < 11 && (w ? w.index(d) > -1 : d.nodeType === 1 && p.find.matchesSelector(d, a))) {
                                 x.push(d);
                                 break
                             }
                 }
                 return this.pushStack(x.length > 1 ? p.uniqueSort(x) : x)
             },
@@ -1046,34 +1046,34 @@
             children: function(a) {
                 return We(a.firstChild)
             },
             contents: function(a) {
                 return a.contentDocument != null && r(a.contentDocument) ? a.contentDocument : (J(a, "template") && (a = a.content || a), p.merge([], a.childNodes))
             }
         }, function(a, c) {
-            p.fn[a] = function(d, m) {
+            p.fn[a] = function(d, g) {
                 var b = p.map(this, c, d);
-                return a.slice(-5) !== "Until" && (m = d), m && typeof m == "string" && (b = p.filter(m, b)), this.length > 1 && (Bs[a] || p.uniqueSort(b), Mr.test(a) && b.reverse()), this.pushStack(b)
+                return a.slice(-5) !== "Until" && (g = d), g && typeof g == "string" && (b = p.filter(g, b)), this.length > 1 && (Bs[a] || p.uniqueSort(b), Mr.test(a) && b.reverse()), this.pushStack(b)
             }
         });
         var at = /[^\x20\t\r\n\f]+/g;
 
         function zi(a) {
             var c = {};
-            return p.each(a.match(at) || [], function(d, m) {
-                c[m] = !0
+            return p.each(a.match(at) || [], function(d, g) {
+                c[g] = !0
             }), c
         }
         p.Callbacks = function(a) {
             a = typeof a == "string" ? zi(a) : p.extend({}, a);
-            var c, d, m, b, x = [],
+            var c, d, g, b, x = [],
                 w = [],
                 T = -1,
                 C = function() {
-                    for (b = b || a.once, m = c = !0; w.length; T = -1)
+                    for (b = b || a.once, g = c = !0; w.length; T = -1)
                         for (d = w.shift(); ++T < x.length;) x[T].apply(d[0], d[1]) === !1 && a.stopOnFalse && (T = x.length, d = !1);
                     a.memory || (d = !1), c = !1, b && (d ? x = [] : x = "")
                 },
                 E = {
                     add: function() {
                         return x && (d && !c && (T = x.length - 1, w.push(d)), function I(_) {
                             p.each(_, function(P, W) {
@@ -1108,53 +1108,53 @@
                     fireWith: function(I, _) {
                         return b || (_ = _ || [], _ = [I, _.slice ? _.slice() : _], w.push(_), c || C()), this
                     },
                     fire: function() {
                         return E.fireWith(this, arguments), this
                     },
                     fired: function() {
-                        return !!m
+                        return !!g
                     }
                 };
             return E
         };
 
         function bi(a) {
             return a
         }
 
         function Yi(a) {
             throw a
         }
 
-        function $i(a, c, d, m) {
+        function $i(a, c, d, g) {
             var b;
             try {
-                a && A(b = a.promise) ? b.call(a).done(c).fail(d) : a && A(b = a.then) ? b.call(a, c, d) : c.apply(void 0, [a].slice(m))
+                a && A(b = a.promise) ? b.call(a).done(c).fail(d) : a && A(b = a.then) ? b.call(a, c, d) : c.apply(void 0, [a].slice(g))
             } catch (x) {
                 d.apply(void 0, [x])
             }
         }
         p.extend({
             Deferred: function(a) {
                 var c = [
                         ["notify", "progress", p.Callbacks("memory"), p.Callbacks("memory"), 2],
                         ["resolve", "done", p.Callbacks("once memory"), p.Callbacks("once memory"), 0, "resolved"],
                         ["reject", "fail", p.Callbacks("once memory"), p.Callbacks("once memory"), 1, "rejected"]
                     ],
                     d = "pending",
-                    m = {
+                    g = {
                         state: function() {
                             return d
                         },
                         always: function() {
                             return b.done(arguments).fail(arguments), this
                         },
                         catch: function(x) {
-                            return m.then(null, x)
+                            return g.then(null, x)
                         },
                         pipe: function() {
                             var x = arguments;
                             return p.Deferred(function(w) {
                                 p.each(c, function(T, C) {
                                     var E = A(x[C[4]]) && x[C[4]];
                                     b[C[1]](function() {
@@ -1189,37 +1189,37 @@
                                 }
                             }
                             return p.Deferred(function(I) {
                                 c[0][3].add(E(0, I, A(T) ? T : bi, I.notifyWith)), c[1][3].add(E(0, I, A(x) ? x : bi)), c[2][3].add(E(0, I, A(w) ? w : Yi))
                             }).promise()
                         },
                         promise: function(x) {
-                            return x != null ? p.extend(x, m) : m
+                            return x != null ? p.extend(x, g) : g
                         }
                     },
                     b = {};
                 return p.each(c, function(x, w) {
                     var T = w[2],
                         C = w[5];
-                    m[w[1]] = T.add, C && T.add(function() {
+                    g[w[1]] = T.add, C && T.add(function() {
                         d = C
                     }, c[3 - x][2].disable, c[3 - x][3].disable, c[0][2].lock, c[0][3].lock), T.add(w[3].fire), b[w[0]] = function() {
                         return b[w[0] + "With"](this === b ? void 0 : this, arguments), this
                     }, b[w[0] + "With"] = T.fireWith
-                }), m.promise(b), a && a.call(b, b), b
+                }), g.promise(b), a && a.call(b, b), b
             },
             when: function(a) {
                 var c = arguments.length,
                     d = c,
-                    m = Array(d),
+                    g = Array(d),
                     b = s.call(arguments),
                     x = p.Deferred(),
                     w = function(T) {
                         return function(C) {
-                            m[T] = this, b[T] = arguments.length > 1 ? s.call(arguments) : C, --c || x.resolveWith(m, b)
+                            g[T] = this, b[T] = arguments.length > 1 ? s.call(arguments) : C, --c || x.resolveWith(g, b)
                         }
                     };
                 if (c <= 1 && ($i(a, x.done(w(d)).resolve, x.reject, !c), x.state() === "pending" || A(b[d] && b[d].then))) return x.then();
                 for (; d--;) $i(b[d], w(d), x.reject);
                 return x.promise()
             }
         });
@@ -1244,25 +1244,25 @@
             }
         }), p.ready.then = Ji.then;
 
         function Mn() {
             D.removeEventListener("DOMContentLoaded", Mn), e.removeEventListener("load", Mn), p.ready()
         }
         D.readyState === "complete" || D.readyState !== "loading" && !D.documentElement.doScroll ? e.setTimeout(p.ready) : (D.addEventListener("DOMContentLoaded", Mn), e.addEventListener("load", Mn));
-        var Kt = function(a, c, d, m, b, x, w) {
+        var Kt = function(a, c, d, g, b, x, w) {
                 var T = 0,
                     C = a.length,
                     E = d == null;
                 if (j(d) === "object") {
                     b = !0;
                     for (T in d) Kt(a, c, T, d[T], !0, x, w)
-                } else if (m !== void 0 && (b = !0, A(m) || (w = !0), E && (w ? (c.call(a, m), c = null) : (E = c, c = function(I, _, P) {
+                } else if (g !== void 0 && (b = !0, A(g) || (w = !0), E && (w ? (c.call(a, g), c = null) : (E = c, c = function(I, _, P) {
                         return E.call(p(I), P)
                     })), c))
-                    for (; T < C; T++) c(a[T], d, w ? m : m.call(a[T], T, c(a[T], d)));
+                    for (; T < C; T++) c(a[T], d, w ? g : g.call(a[T], T, c(a[T], d)));
                 return b ? a : E ? c.call(a) : C ? c(a[0], d) : x
             },
             Ll = /^-ms-/,
             Dr = /-([a-z])/g;
 
         function En(a, c) {
             return c.toUpperCase()
@@ -1283,32 +1283,32 @@
                 var c = a[this.expando];
                 return c || (c = {}, Xt(a) && (a.nodeType ? a[this.expando] = c : Object.defineProperty(a, this.expando, {
                     value: c,
                     configurable: !0
                 }))), c
             },
             set: function(a, c, d) {
-                var m, b = this.cache(a);
+                var g, b = this.cache(a);
                 if (typeof c == "string") b[ht(c)] = d;
                 else
-                    for (m in c) b[ht(m)] = c[m];
+                    for (g in c) b[ht(g)] = c[g];
                 return b
             },
             get: function(a, c) {
                 return c === void 0 ? this.cache(a) : a[this.expando] && a[this.expando][ht(c)]
             },
             access: function(a, c, d) {
                 return c === void 0 || c && typeof c == "string" && d === void 0 ? this.get(a, c) : (this.set(a, c, d), d !== void 0 ? d : c)
             },
             remove: function(a, c) {
-                var d, m = a[this.expando];
-                if (m !== void 0) {
+                var d, g = a[this.expando];
+                if (g !== void 0) {
                     if (c !== void 0)
-                        for (Array.isArray(c) ? c = c.map(ht) : (c = ht(c), c = c in m ? [c] : c.match(at) || []), d = c.length; d--;) delete m[c[d]];
-                    (c === void 0 || p.isEmptyObject(m)) && (a.nodeType ? a[this.expando] = void 0 : delete a[this.expando])
+                        for (Array.isArray(c) ? c = c.map(ht) : (c = ht(c), c = c in g ? [c] : c.match(at) || []), d = c.length; d--;) delete g[c[d]];
+                    (c === void 0 || p.isEmptyObject(g)) && (a.nodeType ? a[this.expando] = void 0 : delete a[this.expando])
                 }
             },
             hasData: function(a) {
                 var c = a[this.expando];
                 return c !== void 0 && !p.isEmptyObject(c)
             }
         };
@@ -1318,17 +1318,17 @@
             _s = /[A-Z]/g;
 
         function Jn(a) {
             return a === "true" ? !0 : a === "false" ? !1 : a === "null" ? null : a === +a + "" ? +a : Rr.test(a) ? JSON.parse(a) : a
         }
 
         function Dn(a, c, d) {
-            var m;
+            var g;
             if (d === void 0 && a.nodeType === 1)
-                if (m = "data-" + c.replace(_s, "-$&").toLowerCase(), d = a.getAttribute(m), typeof d == "string") {
+                if (g = "data-" + c.replace(_s, "-$&").toLowerCase(), d = a.getAttribute(g), typeof d == "string") {
                     try {
                         d = Jn(d)
                     } catch (b) {}
                     ct.set(a, c, d)
                 } else d = void 0;
             return d
         }
@@ -1346,19 +1346,19 @@
                 return ne.access(a, c, d)
             },
             _removeData: function(a, c) {
                 ne.remove(a, c)
             }
         }), p.fn.extend({
             data: function(a, c) {
-                var d, m, b, x = this[0],
+                var d, g, b, x = this[0],
                     w = x && x.attributes;
                 if (a === void 0) {
                     if (this.length && (b = ct.get(x), x.nodeType === 1 && !ne.get(x, "hasDataAttrs"))) {
-                        for (d = w.length; d--;) w[d] && (m = w[d].name, m.indexOf("data-") === 0 && (m = ht(m.slice(5)), Dn(x, m, b[m])));
+                        for (d = w.length; d--;) w[d] && (g = w[d].name, g.indexOf("data-") === 0 && (g = ht(g.slice(5)), Dn(x, g, b[g])));
                         ne.set(x, "hasDataAttrs", !0)
                     }
                     return b
                 }
                 return typeof a == "object" ? this.each(function() {
                     ct.set(this, a)
                 }) : Kt(this, function(T) {
@@ -1372,61 +1372,61 @@
             removeData: function(a) {
                 return this.each(function() {
                     ct.remove(this, a)
                 })
             }
         }), p.extend({
             queue: function(a, c, d) {
-                var m;
-                if (a) return c = (c || "fx") + "queue", m = ne.get(a, c), d && (!m || Array.isArray(d) ? m = ne.access(a, c, p.makeArray(d)) : m.push(d)), m || []
+                var g;
+                if (a) return c = (c || "fx") + "queue", g = ne.get(a, c), d && (!g || Array.isArray(d) ? g = ne.access(a, c, p.makeArray(d)) : g.push(d)), g || []
             },
             dequeue: function(a, c) {
                 c = c || "fx";
                 var d = p.queue(a, c),
-                    m = d.length,
+                    g = d.length,
                     b = d.shift(),
                     x = p._queueHooks(a, c),
                     w = function() {
                         p.dequeue(a, c)
                     };
-                b === "inprogress" && (b = d.shift(), m--), b && (c === "fx" && d.unshift("inprogress"), delete x.stop, b.call(a, w, x)), !m && x && x.empty.fire()
+                b === "inprogress" && (b = d.shift(), g--), b && (c === "fx" && d.unshift("inprogress"), delete x.stop, b.call(a, w, x)), !g && x && x.empty.fire()
             },
             _queueHooks: function(a, c) {
                 var d = c + "queueHooks";
                 return ne.get(a, d) || ne.access(a, d, {
                     empty: p.Callbacks("once memory").add(function() {
                         ne.remove(a, [c + "queue", d])
                     })
                 })
             }
         }), p.fn.extend({
             queue: function(a, c) {
                 var d = 2;
                 return typeof a != "string" && (c = a, a = "fx", d--), arguments.length < d ? p.queue(this[0], a) : c === void 0 ? this : this.each(function() {
-                    var m = p.queue(this, a, c);
-                    p._queueHooks(this, a), a === "fx" && m[0] !== "inprogress" && p.dequeue(this, a)
+                    var g = p.queue(this, a, c);
+                    p._queueHooks(this, a), a === "fx" && g[0] !== "inprogress" && p.dequeue(this, a)
                 })
             },
             dequeue: function(a) {
                 return this.each(function() {
                     p.dequeue(this, a)
                 })
             },
             clearQueue: function(a) {
                 return this.queue(a || "fx", [])
             },
             promise: function(a, c) {
-                var d, m = 1,
+                var d, g = 1,
                     b = p.Deferred(),
                     x = this,
                     w = this.length,
                     T = function() {
-                        --m || b.resolveWith(x, [x])
+                        --g || b.resolveWith(x, [x])
                     };
-                for (typeof a != "string" && (c = a, a = void 0), a = a || "fx"; w--;) d = ne.get(x[w], a + "queueHooks"), d && d.empty && (m++, d.empty.add(T));
+                for (typeof a != "string" && (c = a, a = void 0), a = a || "fx"; w--;) d = ne.get(x[w], a + "queueHooks"), d && d.empty && (g++, d.empty.add(T));
                 return T(), b.promise(c)
             }
         });
         var Yt = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
             Jt = new RegExp("^(?:([+-])=|)(" + Yt + ")([a-z%]*)$", "i"),
             Ft = ["Top", "Right", "Bottom", "Left"],
             ai = D.documentElement,
@@ -1439,41 +1439,41 @@
         ai.getRootNode && (en = function(a) {
             return p.contains(a.ownerDocument, a) || a.getRootNode(Rn) === a.ownerDocument
         });
         var Zn = function(a, c) {
             return a = c || a, a.style.display === "none" || a.style.display === "" && en(a) && p.css(a, "display") === "none"
         };
 
-        function Hs(a, c, d, m) {
+        function Hs(a, c, d, g) {
             var b, x, w = 20,
-                T = m ? function() {
-                    return m.cur()
+                T = g ? function() {
+                    return g.cur()
                 } : function() {
                     return p.css(a, c, "")
                 },
                 C = T(),
                 E = d && d[3] || (p.cssNumber[c] ? "" : "px"),
                 I = a.nodeType && (p.cssNumber[c] || E !== "px" && +C) && Jt.exec(p.css(a, c));
             if (I && I[3] !== E) {
                 for (C = C / 2, E = E || I[3], I = +C || 1; w--;) p.style(a, c, I + E), (1 - x) * (1 - (x = T() / C || .5)) <= 0 && (w = 0), I = I / x;
                 I = I * 2, p.style(a, c, I + E), d = d || []
             }
-            return d && (I = +I || +C || 0, b = d[1] ? I + (d[1] + 1) * d[2] : +d[2], m && (m.unit = E, m.start = I, m.end = b)), b
+            return d && (I = +I || +C || 0, b = d[1] ? I + (d[1] + 1) * d[2] : +d[2], g && (g.unit = E, g.start = I, g.end = b)), b
         }
         var Ge = {};
 
         function tn(a) {
             var c, d = a.ownerDocument,
-                m = a.nodeName,
-                b = Ge[m];
-            return b || (c = d.body.appendChild(d.createElement(m)), b = p.css(c, "display"), c.parentNode.removeChild(c), b === "none" && (b = "block"), Ge[m] = b, b)
+                g = a.nodeName,
+                b = Ge[g];
+            return b || (c = d.body.appendChild(d.createElement(g)), b = p.css(c, "display"), c.parentNode.removeChild(c), b === "none" && (b = "block"), Ge[g] = b, b)
         }
 
         function nn(a, c) {
-            for (var d, m, b = [], x = 0, w = a.length; x < w; x++) m = a[x], m.style && (d = m.style.display, c ? (d === "none" && (b[x] = ne.get(m, "display") || null, b[x] || (m.style.display = "")), m.style.display === "" && Zn(m) && (b[x] = tn(m))) : d !== "none" && (b[x] = "none", ne.set(m, "display", d)));
+            for (var d, g, b = [], x = 0, w = a.length; x < w; x++) g = a[x], g.style && (d = g.style.display, c ? (d === "none" && (b[x] = ne.get(g, "display") || null, b[x] || (g.style.display = "")), g.style.display === "" && Zn(g) && (b[x] = tn(g))) : d !== "none" && (b[x] = "none", ne.set(g, "display", d)));
             for (x = 0; x < w; x++) b[x] != null && (a[x].style.display = b[x]);
             return a
         }
         p.fn.extend({
             show: function() {
                 return nn(this, !0)
             },
@@ -1506,29 +1506,29 @@
 
         function xt(a, c) {
             var d;
             return typeof a.getElementsByTagName != "undefined" ? d = a.getElementsByTagName(c || "*") : typeof a.querySelectorAll != "undefined" ? d = a.querySelectorAll(c || "*") : d = [], c === void 0 || c && J(a, c) ? p.merge([a], d) : d
         }
 
         function tr(a, c) {
-            for (var d = 0, m = a.length; d < m; d++) ne.set(a[d], "globalEval", !c || ne.get(c[d], "globalEval"))
+            for (var d = 0, g = a.length; d < g; d++) ne.set(a[d], "globalEval", !c || ne.get(c[d], "globalEval"))
         }
         var Fs = /<|&#?\w+;/;
 
-        function zs(a, c, d, m, b) {
+        function zs(a, c, d, g, b) {
             for (var x, w, T, C, E, I, _ = c.createDocumentFragment(), P = [], W = 0, ce = a.length; W < ce; W++)
                 if (x = a[W], x || x === 0)
                     if (j(x) === "object") p.merge(P, x.nodeType ? [x] : x);
                     else if (!Fs.test(x)) P.push(c.createTextNode(x));
             else {
                 for (w = w || _.appendChild(c.createElement("div")), T = (er.exec(x) || ["", ""])[1].toLowerCase(), C = Ot[T] || Ot._default, w.innerHTML = C[1] + p.htmlPrefilter(x) + C[2], I = C[0]; I--;) w = w.lastChild;
                 p.merge(P, w.childNodes), w = _.firstChild, w.textContent = ""
             }
             for (_.textContent = "", W = 0; x = P[W++];) {
-                if (m && p.inArray(x, m) > -1) {
+                if (g && p.inArray(x, g) > -1) {
                     b && b.push(x);
                     continue
                 }
                 if (E = en(x), w = xt(_.appendChild(x), "script"), E && tr(w), d)
                     for (I = 0; x = w[I++];) Lr.test(x.type || "") && d.push(x)
             }
             return _
@@ -1539,83 +1539,83 @@
             return !0
         }
 
         function Wi() {
             return !1
         }
 
-        function ir(a, c, d, m, b, x) {
+        function ir(a, c, d, g, b, x) {
             var w, T;
             if (typeof c == "object") {
-                typeof d != "string" && (m = m || d, d = void 0);
-                for (T in c) ir(a, T, d, m, c[T], x);
+                typeof d != "string" && (g = g || d, d = void 0);
+                for (T in c) ir(a, T, d, g, c[T], x);
                 return a
             }
-            if (m == null && b == null ? (b = d, m = d = void 0) : b == null && (typeof d == "string" ? (b = m, m = void 0) : (b = m, m = d, d = void 0)), b === !1) b = Wi;
+            if (g == null && b == null ? (b = d, g = d = void 0) : b == null && (typeof d == "string" ? (b = g, g = void 0) : (b = g, g = d, d = void 0)), b === !1) b = Wi;
             else if (!b) return a;
             return x === 1 && (w = b, b = function(C) {
                 return p().off(C), w.apply(this, arguments)
             }, b.guid = w.guid || (w.guid = p.guid++)), a.each(function() {
-                p.event.add(this, c, b, m, d)
+                p.event.add(this, c, b, g, d)
             })
         }
         p.event = {
             global: {},
-            add: function(a, c, d, m, b) {
+            add: function(a, c, d, g, b) {
                 var x, w, T, C, E, I, _, P, W, ce, Ae, ge = ne.get(a);
                 if (Xt(a))
                     for (d.handler && (x = d, d = x.handler, b = x.selector), b && p.find.matchesSelector(ai, b), d.guid || (d.guid = p.guid++), (C = ge.events) || (C = ge.events = Object.create(null)), (w = ge.handle) || (w = ge.handle = function(ut) {
                             return typeof p != "undefined" && p.event.triggered !== ut.type ? p.event.dispatch.apply(a, arguments) : void 0
                         }), c = (c || "").match(at) || [""], E = c.length; E--;) T = xi.exec(c[E]) || [], W = Ae = T[1], ce = (T[2] || "").split(".").sort(), W && (_ = p.event.special[W] || {}, W = (b ? _.delegateType : _.bindType) || W, _ = p.event.special[W] || {}, I = p.extend({
                         type: W,
                         origType: Ae,
-                        data: m,
+                        data: g,
                         handler: d,
                         guid: d.guid,
                         selector: b,
                         needsContext: b && p.expr.match.needsContext.test(b),
                         namespace: ce.join(".")
-                    }, x), (P = C[W]) || (P = C[W] = [], P.delegateCount = 0, (!_.setup || _.setup.call(a, m, ce, w) === !1) && a.addEventListener && a.addEventListener(W, w)), _.add && (_.add.call(a, I), I.handler.guid || (I.handler.guid = d.guid)), b ? P.splice(P.delegateCount++, 0, I) : P.push(I), p.event.global[W] = !0)
+                    }, x), (P = C[W]) || (P = C[W] = [], P.delegateCount = 0, (!_.setup || _.setup.call(a, g, ce, w) === !1) && a.addEventListener && a.addEventListener(W, w)), _.add && (_.add.call(a, I), I.handler.guid || (I.handler.guid = d.guid)), b ? P.splice(P.delegateCount++, 0, I) : P.push(I), p.event.global[W] = !0)
             },
-            remove: function(a, c, d, m, b) {
+            remove: function(a, c, d, g, b) {
                 var x, w, T, C, E, I, _, P, W, ce, Ae, ge = ne.hasData(a) && ne.get(a);
                 if (!(!ge || !(C = ge.events))) {
                     for (c = (c || "").match(at) || [""], E = c.length; E--;) {
                         if (T = xi.exec(c[E]) || [], W = Ae = T[1], ce = (T[2] || "").split(".").sort(), !W) {
-                            for (W in C) p.event.remove(a, W + c[E], d, m, !0);
+                            for (W in C) p.event.remove(a, W + c[E], d, g, !0);
                             continue
                         }
-                        for (_ = p.event.special[W] || {}, W = (m ? _.delegateType : _.bindType) || W, P = C[W] || [], T = T[2] && new RegExp("(^|\\.)" + ce.join("\\.(?:.*\\.|)") + "(\\.|$)"), w = x = P.length; x--;) I = P[x], (b || Ae === I.origType) && (!d || d.guid === I.guid) && (!T || T.test(I.namespace)) && (!m || m === I.selector || m === "**" && I.selector) && (P.splice(x, 1), I.selector && P.delegateCount--, _.remove && _.remove.call(a, I));
+                        for (_ = p.event.special[W] || {}, W = (g ? _.delegateType : _.bindType) || W, P = C[W] || [], T = T[2] && new RegExp("(^|\\.)" + ce.join("\\.(?:.*\\.|)") + "(\\.|$)"), w = x = P.length; x--;) I = P[x], (b || Ae === I.origType) && (!d || d.guid === I.guid) && (!T || T.test(I.namespace)) && (!g || g === I.selector || g === "**" && I.selector) && (P.splice(x, 1), I.selector && P.delegateCount--, _.remove && _.remove.call(a, I));
                         w && !P.length && ((!_.teardown || _.teardown.call(a, ce, ge.handle) === !1) && p.removeEvent(a, W, ge.handle), delete C[W])
                     }
                     p.isEmptyObject(C) && ne.remove(a, "handle events")
                 }
             },
             dispatch: function(a) {
-                var c, d, m, b, x, w, T = new Array(arguments.length),
+                var c, d, g, b, x, w, T = new Array(arguments.length),
                     C = p.event.fix(a),
                     E = (ne.get(this, "events") || Object.create(null))[C.type] || [],
                     I = p.event.special[C.type] || {};
                 for (T[0] = C, c = 1; c < arguments.length; c++) T[c] = arguments[c];
                 if (C.delegateTarget = this, !(I.preDispatch && I.preDispatch.call(this, C) === !1)) {
                     for (w = p.event.handlers.call(this, C, E), c = 0;
                         (b = w[c++]) && !C.isPropagationStopped();)
                         for (C.currentTarget = b.elem, d = 0;
-                            (x = b.handlers[d++]) && !C.isImmediatePropagationStopped();)(!C.rnamespace || x.namespace === !1 || C.rnamespace.test(x.namespace)) && (C.handleObj = x, C.data = x.data, m = ((p.event.special[x.origType] || {}).handle || x.handler).apply(b.elem, T), m !== void 0 && (C.result = m) === !1 && (C.preventDefault(), C.stopPropagation()));
+                            (x = b.handlers[d++]) && !C.isImmediatePropagationStopped();)(!C.rnamespace || x.namespace === !1 || C.rnamespace.test(x.namespace)) && (C.handleObj = x, C.data = x.data, g = ((p.event.special[x.origType] || {}).handle || x.handler).apply(b.elem, T), g !== void 0 && (C.result = g) === !1 && (C.preventDefault(), C.stopPropagation()));
                     return I.postDispatch && I.postDispatch.call(this, C), C.result
                 }
             },
             handlers: function(a, c) {
-                var d, m, b, x, w, T = [],
+                var d, g, b, x, w, T = [],
                     C = c.delegateCount,
                     E = a.target;
                 if (C && E.nodeType && !(a.type === "click" && a.button >= 1)) {
                     for (; E !== this; E = E.parentNode || this)
                         if (E.nodeType === 1 && !(a.type === "click" && E.disabled === !0)) {
-                            for (x = [], w = {}, d = 0; d < C; d++) m = c[d], b = m.selector + " ", w[b] === void 0 && (w[b] = m.needsContext ? p(b, this).index(E) > -1 : p.find(b, this, null, [E]).length), w[b] && x.push(m);
+                            for (x = [], w = {}, d = 0; d < C; d++) g = c[d], b = g.selector + " ", w[b] === void 0 && (w[b] = g.needsContext ? p(b, this).index(E) > -1 : p.find(b, this, null, [E]).length), w[b] && x.push(g);
                             x.length && T.push({
                                 elem: E,
                                 handlers: x
                             })
                         }
                 }
                 return E = this, C < c.length && T.push({
@@ -1674,20 +1674,20 @@
         function nr(a, c, d) {
             if (!d) {
                 ne.get(a, c) === void 0 && p.event.add(a, c, ki);
                 return
             }
             ne.set(a, c, !1), p.event.add(a, c, {
                 namespace: !1,
-                handler: function(m) {
+                handler: function(g) {
                     var b, x = ne.get(this, c);
-                    if (m.isTrigger & 1 && this[c]) {
-                        if (x)(p.event.special[c] || {}).delegateType && m.stopPropagation();
-                        else if (x = s.call(arguments), ne.set(this, c, x), this[c](), b = ne.get(this, c), ne.set(this, c, !1), x !== b) return m.stopImmediatePropagation(), m.preventDefault(), b
-                    } else x && (ne.set(this, c, p.event.trigger(x[0], x.slice(1), this)), m.stopPropagation(), m.isImmediatePropagationStopped = ki)
+                    if (g.isTrigger & 1 && this[c]) {
+                        if (x)(p.event.special[c] || {}).delegateType && g.stopPropagation();
+                        else if (x = s.call(arguments), ne.set(this, c, x), this[c](), b = ne.get(this, c), ne.set(this, c, !1), x !== b) return g.stopImmediatePropagation(), g.preventDefault(), b
+                    } else x && (ne.set(this, c, p.event.trigger(x[0], x.slice(1), this)), g.stopPropagation(), g.isImmediatePropagationStopped = ki)
                 }
             })
         }
         p.removeEvent = function(a, c, d) {
             a.removeEventListener && a.removeEventListener(c, d)
         }, p.Event = function(a, c) {
             if (!(this instanceof p.Event)) return new p.Event(a, c);
@@ -1742,79 +1742,79 @@
             toElement: !0,
             touches: !0,
             which: !0
         }, p.event.addProp), p.each({
             focus: "focusin",
             blur: "focusout"
         }, function(a, c) {
-            function d(m) {
+            function d(g) {
                 if (D.documentMode) {
                     var b = ne.get(this, "handle"),
-                        x = p.event.fix(m);
-                    x.type = m.type === "focusin" ? "focus" : "blur", x.isSimulated = !0, b(m), x.target === x.currentTarget && b(x)
-                } else p.event.simulate(c, m.target, p.event.fix(m))
+                        x = p.event.fix(g);
+                    x.type = g.type === "focusin" ? "focus" : "blur", x.isSimulated = !0, b(g), x.target === x.currentTarget && b(x)
+                } else p.event.simulate(c, g.target, p.event.fix(g))
             }
             p.event.special[a] = {
                 setup: function() {
-                    var m;
-                    if (nr(this, a, !0), D.documentMode) m = ne.get(this, c), m || this.addEventListener(c, d), ne.set(this, c, (m || 0) + 1);
+                    var g;
+                    if (nr(this, a, !0), D.documentMode) g = ne.get(this, c), g || this.addEventListener(c, d), ne.set(this, c, (g || 0) + 1);
                     else return !1
                 },
                 trigger: function() {
                     return nr(this, a), !0
                 },
                 teardown: function() {
-                    var m;
-                    if (D.documentMode) m = ne.get(this, c) - 1, m ? ne.set(this, c, m) : (this.removeEventListener(c, d), ne.remove(this, c));
+                    var g;
+                    if (D.documentMode) g = ne.get(this, c) - 1, g ? ne.set(this, c, g) : (this.removeEventListener(c, d), ne.remove(this, c));
                     else return !1
                 },
-                _default: function(m) {
-                    return ne.get(m.target, a)
+                _default: function(g) {
+                    return ne.get(g.target, a)
                 },
                 delegateType: c
             }, p.event.special[c] = {
                 setup: function() {
-                    var m = this.ownerDocument || this.document || this,
-                        b = D.documentMode ? this : m,
+                    var g = this.ownerDocument || this.document || this,
+                        b = D.documentMode ? this : g,
                         x = ne.get(b, c);
-                    x || (D.documentMode ? this.addEventListener(c, d) : m.addEventListener(a, d, !0)), ne.set(b, c, (x || 0) + 1)
+                    x || (D.documentMode ? this.addEventListener(c, d) : g.addEventListener(a, d, !0)), ne.set(b, c, (x || 0) + 1)
                 },
                 teardown: function() {
-                    var m = this.ownerDocument || this.document || this,
-                        b = D.documentMode ? this : m,
+                    var g = this.ownerDocument || this.document || this,
+                        b = D.documentMode ? this : g,
                         x = ne.get(b, c) - 1;
-                    x ? ne.set(b, c, x) : (D.documentMode ? this.removeEventListener(c, d) : m.removeEventListener(a, d, !0), ne.remove(b, c))
+                    x ? ne.set(b, c, x) : (D.documentMode ? this.removeEventListener(c, d) : g.removeEventListener(a, d, !0), ne.remove(b, c))
                 }
             }
         }), p.each({
             mouseenter: "mouseover",
             mouseleave: "mouseout",
             pointerenter: "pointerover",
             pointerleave: "pointerout"
         }, function(a, c) {
             p.event.special[a] = {
                 delegateType: c,
                 bindType: c,
                 handle: function(d) {
-                    var m, b = this,
+                    var g, b = this,
                         x = d.relatedTarget,
                         w = d.handleObj;
-                    return (!x || x !== b && !p.contains(b, x)) && (d.type = w.origType, m = w.handler.apply(this, arguments), d.type = c), m
+                    return (!x || x !== b && !p.contains(b, x)) && (d.type = w.origType, g = w.handler.apply(this, arguments), d.type = c), g
                 }
             }
         }), p.fn.extend({
-            on: function(a, c, d, m) {
-                return ir(this, a, c, d, m)
+            on: function(a, c, d, g) {
+                return ir(this, a, c, d, g)
             },
-            one: function(a, c, d, m) {
-                return ir(this, a, c, d, m, 1)
+            one: function(a, c, d, g) {
+                return ir(this, a, c, d, g, 1)
             },
             off: function(a, c, d) {
-                var m, b;
-                if (a && a.preventDefault && a.handleObj) return m = a.handleObj, p(a.delegateTarget).off(m.namespace ? m.origType + "." + m.namespace : m.origType, m.selector, m.handler), this;
+                var g, b;
+                if (a && a.preventDefault && a.handleObj) return g = a.handleObj, p(a.delegateTarget).off(g.namespace ? g.origType + "." + g.namespace : g.origType, g.selector, g.handler), this;
                 if (typeof a == "object") {
                     for (b in a) this.off(b, c, a[b]);
                     return this
                 }
                 return (c === !1 || typeof c == "function") && (d = c, c = void 0), d === !1 && (d = Wi), this.each(function() {
                     p.event.remove(this, a, d, c)
                 })
@@ -1833,78 +1833,78 @@
         }
 
         function js(a) {
             return (a.type || "").slice(0, 5) === "true/" ? a.type = a.type.slice(5) : a.removeAttribute("type"), a
         }
 
         function Vs(a, c) {
-            var d, m, b, x, w, T, C;
+            var d, g, b, x, w, T, C;
             if (c.nodeType === 1) {
                 if (ne.hasData(a) && (x = ne.get(a), C = x.events, C)) {
                     ne.remove(c, "handle events");
                     for (b in C)
-                        for (d = 0, m = C[b].length; d < m; d++) p.event.add(c, b, C[b][d])
+                        for (d = 0, g = C[b].length; d < g; d++) p.event.add(c, b, C[b][d])
                 }
                 ct.hasData(a) && (w = ct.access(a), T = p.extend({}, w), ct.set(c, T))
             }
         }
 
         function se(a, c) {
             var d = c.nodeName.toLowerCase();
             d === "input" && rn.test(a.type) ? c.checked = a.checked : (d === "input" || d === "textarea") && (c.defaultValue = a.defaultValue)
         }
 
-        function R(a, c, d, m) {
+        function R(a, c, d, g) {
             c = o(c);
             var b, x, w, T, C, E, I = 0,
                 _ = a.length,
                 P = _ - 1,
                 W = c[0],
                 ce = A(W);
             if (ce || _ > 1 && typeof W == "string" && !v.checkClone && hi.test(W)) return a.each(function(Ae) {
                 var ge = a.eq(Ae);
-                ce && (c[0] = W.call(this, Ae, ge.html())), R(ge, c, d, m)
+                ce && (c[0] = W.call(this, Ae, ge.html())), R(ge, c, d, g)
             });
-            if (_ && (b = zs(c, a[0].ownerDocument, !1, a, m), x = b.firstChild, b.childNodes.length === 1 && (b = x), x || m)) {
+            if (_ && (b = zs(c, a[0].ownerDocument, !1, a, g), x = b.firstChild, b.childNodes.length === 1 && (b = x), x || g)) {
                 for (w = p.map(xt(b, "script"), qs), T = w.length; I < _; I++) C = b, I !== P && (C = p.clone(C, !0, !0), T && p.merge(w, xt(C, "script"))), d.call(a[I], C, I);
                 if (T)
                     for (E = w[w.length - 1].ownerDocument, p.map(w, js), I = 0; I < T; I++) C = w[I], Lr.test(C.type || "") && !ne.access(C, "globalEval") && p.contains(E, C) && (C.src && (C.type || "").toLowerCase() !== "module" ? p._evalUrl && !C.noModule && p._evalUrl(C.src, {
                         nonce: C.nonce || C.getAttribute("nonce")
                     }, E) : $(C.textContent.replace(Ws, ""), C, E))
             }
             return a
         }
 
         function V(a, c, d) {
-            for (var m, b = c ? p.filter(c, a) : a, x = 0;
-                (m = b[x]) != null; x++) !d && m.nodeType === 1 && p.cleanData(xt(m)), m.parentNode && (d && en(m) && tr(xt(m, "script")), m.parentNode.removeChild(m));
+            for (var g, b = c ? p.filter(c, a) : a, x = 0;
+                (g = b[x]) != null; x++) !d && g.nodeType === 1 && p.cleanData(xt(g)), g.parentNode && (d && en(g) && tr(xt(g, "script")), g.parentNode.removeChild(g));
             return a
         }
         p.extend({
             htmlPrefilter: function(a) {
                 return a
             },
             clone: function(a, c, d) {
-                var m, b, x, w, T = a.cloneNode(!0),
+                var g, b, x, w, T = a.cloneNode(!0),
                     C = en(a);
                 if (!v.noCloneChecked && (a.nodeType === 1 || a.nodeType === 11) && !p.isXMLDoc(a))
-                    for (w = xt(T), x = xt(a), m = 0, b = x.length; m < b; m++) se(x[m], w[m]);
+                    for (w = xt(T), x = xt(a), g = 0, b = x.length; g < b; g++) se(x[g], w[g]);
                 if (c)
                     if (d)
-                        for (x = x || xt(a), w = w || xt(T), m = 0, b = x.length; m < b; m++) Vs(x[m], w[m]);
+                        for (x = x || xt(a), w = w || xt(T), g = 0, b = x.length; g < b; g++) Vs(x[g], w[g]);
                     else Vs(a, T);
                 return w = xt(T, "script"), w.length > 0 && tr(w, !C && xt(a, "script")), T
             },
             cleanData: function(a) {
-                for (var c, d, m, b = p.event.special, x = 0;
+                for (var c, d, g, b = p.event.special, x = 0;
                     (d = a[x]) !== void 0; x++)
                     if (Xt(d)) {
                         if (c = d[ne.expando]) {
                             if (c.events)
-                                for (m in c.events) b[m] ? p.event.remove(d, m) : p.removeEvent(d, m, c.handle);
+                                for (g in c.events) b[g] ? p.event.remove(d, g) : p.removeEvent(d, g, c.handle);
                             d[ne.expando] = void 0
                         }
                         d[ct.expando] && (d[ct.expando] = void 0)
                     }
             }
         }), p.fn.extend({
             detach: function(a) {
@@ -1955,21 +1955,21 @@
                 return a = a == null ? !1 : a, c = c == null ? a : c, this.map(function() {
                     return p.clone(this, a, c)
                 })
             },
             html: function(a) {
                 return Kt(this, function(c) {
                     var d = this[0] || {},
-                        m = 0,
+                        g = 0,
                         b = this.length;
                     if (c === void 0 && d.nodeType === 1) return d.innerHTML;
                     if (typeof c == "string" && !$s.test(c) && !Ot[(er.exec(c) || ["", ""])[1].toLowerCase()]) {
                         c = p.htmlPrefilter(c);
                         try {
-                            for (; m < b; m++) d = this[m] || {}, d.nodeType === 1 && (p.cleanData(xt(d, !1)), d.innerHTML = c);
+                            for (; g < b; g++) d = this[g] || {}, d.nodeType === 1 && (p.cleanData(xt(d, !1)), d.innerHTML = c);
                             d = 0
                         } catch (x) {}
                     }
                     d && this.empty().append(c)
                 }, null, a, arguments.length)
             },
             replaceWith: function() {
@@ -1983,49 +1983,49 @@
             appendTo: "append",
             prependTo: "prepend",
             insertBefore: "before",
             insertAfter: "after",
             replaceAll: "replaceWith"
         }, function(a, c) {
             p.fn[a] = function(d) {
-                for (var m, b = [], x = p(d), w = x.length - 1, T = 0; T <= w; T++) m = T === w ? this : this.clone(!0), p(x[T])[c](m), l.apply(b, m.get());
+                for (var g, b = [], x = p(d), w = x.length - 1, T = 0; T <= w; T++) g = T === w ? this : this.clone(!0), p(x[T])[c](g), l.apply(b, g.get());
                 return this.pushStack(b)
             }
         });
         var Y = new RegExp("^(" + Yt + ")(?!px)[a-z%]+$", "i"),
             Re = /^--/,
             Ke = function(a) {
                 var c = a.ownerDocument.defaultView;
                 return (!c || !c.opener) && (c = e), c.getComputedStyle(a)
             },
             Ze = function(a, c, d) {
-                var m, b, x = {};
+                var g, b, x = {};
                 for (b in c) x[b] = a.style[b], a.style[b] = c[b];
-                m = d.call(a);
+                g = d.call(a);
                 for (b in c) a.style[b] = x[b];
-                return m
+                return g
             },
             kt = new RegExp(Ft.join("|"), "i");
         (function() {
             function a() {
                 if (E) {
                     C.style.cssText = "position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0", E.style.cssText = "position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%", ai.appendChild(C).appendChild(E);
                     var I = e.getComputedStyle(E);
-                    d = I.top !== "1%", T = c(I.marginLeft) === 12, E.style.right = "60%", x = c(I.right) === 36, m = c(I.width) === 36, E.style.position = "absolute", b = c(E.offsetWidth / 3) === 12, ai.removeChild(C), E = null
+                    d = I.top !== "1%", T = c(I.marginLeft) === 12, E.style.right = "60%", x = c(I.right) === 36, g = c(I.width) === 36, E.style.position = "absolute", b = c(E.offsetWidth / 3) === 12, ai.removeChild(C), E = null
                 }
             }
 
             function c(I) {
                 return Math.round(parseFloat(I))
             }
-            var d, m, b, x, w, T, C = D.createElement("div"),
+            var d, g, b, x, w, T, C = D.createElement("div"),
                 E = D.createElement("div");
             E.style && (E.style.backgroundClip = "content-box", E.cloneNode(!0).style.backgroundClip = "", v.clearCloneStyle = E.style.backgroundClip === "content-box", p.extend(v, {
                 boxSizingReliable: function() {
-                    return a(), m
+                    return a(), g
                 },
                 pixelBoxStyles: function() {
                     return a(), x
                 },
                 pixelPosition: function() {
                     return a(), d
                 },
@@ -2039,17 +2039,17 @@
                     var I, _, P, W;
                     return w == null && (I = D.createElement("table"), _ = D.createElement("tr"), P = D.createElement("div"), I.style.cssText = "position:absolute;left:-11111px;border-collapse:separate", _.style.cssText = "box-sizing:content-box;border:1px solid", _.style.height = "1px", P.style.height = "9px", P.style.display = "block", ai.appendChild(I).appendChild(_).appendChild(P), W = e.getComputedStyle(_), w = parseInt(W.height, 10) + parseInt(W.borderTopWidth, 10) + parseInt(W.borderBottomWidth, 10) === _.offsetHeight, ai.removeChild(I)), w
                 }
             }))
         })();
 
         function zt(a, c, d) {
-            var m, b, x, w, T = Re.test(c),
+            var g, b, x, w, T = Re.test(c),
                 C = a.style;
-            return d = d || Ke(a), d && (w = d.getPropertyValue(c) || d[c], T && w && (w = w.replace(ye, "$1") || void 0), w === "" && !en(a) && (w = p.style(a, c)), !v.pixelBoxStyles() && Y.test(w) && kt.test(c) && (m = C.width, b = C.minWidth, x = C.maxWidth, C.minWidth = C.maxWidth = C.width = w, w = d.width, C.width = m, C.minWidth = b, C.maxWidth = x)), w !== void 0 ? w + "" : w
+            return d = d || Ke(a), d && (w = d.getPropertyValue(c) || d[c], T && w && (w = w.replace(ye, "$1") || void 0), w === "" && !en(a) && (w = p.style(a, c)), !v.pixelBoxStyles() && Y.test(w) && kt.test(c) && (g = C.width, b = C.minWidth, x = C.maxWidth, C.minWidth = C.maxWidth = C.width = w, w = d.width, C.width = g, C.minWidth = b, C.maxWidth = x)), w !== void 0 ? w + "" : w
         }
 
         function sn(a, c) {
             return {
                 get: function() {
                     if (a()) {
                         delete this.get;
@@ -2080,40 +2080,40 @@
             },
             yc = {
                 letterSpacing: "0",
                 fontWeight: "400"
             };
 
         function bc(a, c, d) {
-            var m = Jt.exec(c);
-            return m ? Math.max(0, m[2] - (d || 0)) + (m[3] || "px") : c
+            var g = Jt.exec(c);
+            return g ? Math.max(0, g[2] - (d || 0)) + (g[3] || "px") : c
         }
 
-        function Nl(a, c, d, m, b, x) {
+        function Nl(a, c, d, g, b, x) {
             var w = c === "width" ? 1 : 0,
                 T = 0,
                 C = 0,
                 E = 0;
-            if (d === (m ? "border" : "content")) return 0;
-            for (; w < 4; w += 2) d === "margin" && (E += p.css(a, d + Ft[w], !0, b)), m ? (d === "content" && (C -= p.css(a, "padding" + Ft[w], !0, b)), d !== "margin" && (C -= p.css(a, "border" + Ft[w] + "Width", !0, b))) : (C += p.css(a, "padding" + Ft[w], !0, b), d !== "padding" ? C += p.css(a, "border" + Ft[w] + "Width", !0, b) : T += p.css(a, "border" + Ft[w] + "Width", !0, b));
-            return !m && x >= 0 && (C += Math.max(0, Math.ceil(a["offset" + c[0].toUpperCase() + c.slice(1)] - x - C - T - .5)) || 0), C + E
+            if (d === (g ? "border" : "content")) return 0;
+            for (; w < 4; w += 2) d === "margin" && (E += p.css(a, d + Ft[w], !0, b)), g ? (d === "content" && (C -= p.css(a, "padding" + Ft[w], !0, b)), d !== "margin" && (C -= p.css(a, "border" + Ft[w] + "Width", !0, b))) : (C += p.css(a, "padding" + Ft[w], !0, b), d !== "padding" ? C += p.css(a, "border" + Ft[w] + "Width", !0, b) : T += p.css(a, "border" + Ft[w] + "Width", !0, b));
+            return !g && x >= 0 && (C += Math.max(0, Math.ceil(a["offset" + c[0].toUpperCase() + c.slice(1)] - x - C - T - .5)) || 0), C + E
         }
 
         function xc(a, c, d) {
-            var m = Ke(a),
+            var g = Ke(a),
                 b = !v.boxSizingReliable() || d,
-                x = b && p.css(a, "boxSizing", !1, m) === "border-box",
+                x = b && p.css(a, "boxSizing", !1, g) === "border-box",
                 w = x,
-                T = zt(a, c, m),
+                T = zt(a, c, g),
                 C = "offset" + c[0].toUpperCase() + c.slice(1);
             if (Y.test(T)) {
                 if (!d) return T;
                 T = "auto"
             }
-            return (!v.boxSizingReliable() && x || !v.reliableTrDimensions() && J(a, "tr") || T === "auto" || !parseFloat(T) && p.css(a, "display", !1, m) === "inline") && a.getClientRects().length && (x = p.css(a, "boxSizing", !1, m) === "border-box", w = C in a, w && (T = a[C])), T = parseFloat(T) || 0, T + Nl(a, c, d || (x ? "border" : "content"), w, m, T) + "px"
+            return (!v.boxSizingReliable() && x || !v.reliableTrDimensions() && J(a, "tr") || T === "auto" || !parseFloat(T) && p.css(a, "display", !1, g) === "inline") && a.getClientRects().length && (x = p.css(a, "boxSizing", !1, g) === "border-box", w = C in a, w && (T = a[C])), T = parseFloat(T) || 0, T + Nl(a, c, d || (x ? "border" : "content"), w, g, T) + "px"
         }
         p.extend({
             cssHooks: {
                 opacity: {
                     get: function(a, c) {
                         if (c) {
                             var d = zt(a, "opacity");
@@ -2148,44 +2148,44 @@
                 fillOpacity: !0,
                 floodOpacity: !0,
                 stopOpacity: !0,
                 strokeMiterlimit: !0,
                 strokeOpacity: !0
             },
             cssProps: {},
-            style: function(a, c, d, m) {
+            style: function(a, c, d, g) {
                 if (!(!a || a.nodeType === 3 || a.nodeType === 8 || !a.style)) {
                     var b, x, w, T = ht(c),
                         C = Re.test(c),
                         E = a.style;
                     if (C || (c = Pl(T)), w = p.cssHooks[c] || p.cssHooks[T], d !== void 0) {
                         if (x = typeof d, x === "string" && (b = Jt.exec(d)) && b[1] && (d = Hs(a, c, b), x = "number"), d == null || d !== d) return;
-                        x === "number" && !C && (d += b && b[3] || (p.cssNumber[T] ? "" : "px")), !v.clearCloneStyle && d === "" && c.indexOf("background") === 0 && (E[c] = "inherit"), (!w || !("set" in w) || (d = w.set(a, d, m)) !== void 0) && (C ? E.setProperty(c, d) : E[c] = d)
-                    } else return w && "get" in w && (b = w.get(a, !1, m)) !== void 0 ? b : E[c]
+                        x === "number" && !C && (d += b && b[3] || (p.cssNumber[T] ? "" : "px")), !v.clearCloneStyle && d === "" && c.indexOf("background") === 0 && (E[c] = "inherit"), (!w || !("set" in w) || (d = w.set(a, d, g)) !== void 0) && (C ? E.setProperty(c, d) : E[c] = d)
+                    } else return w && "get" in w && (b = w.get(a, !1, g)) !== void 0 ? b : E[c]
                 }
             },
-            css: function(a, c, d, m) {
+            css: function(a, c, d, g) {
                 var b, x, w, T = ht(c),
                     C = Re.test(c);
-                return C || (c = Pl(T)), w = p.cssHooks[c] || p.cssHooks[T], w && "get" in w && (b = w.get(a, !0, d)), b === void 0 && (b = zt(a, c, m)), b === "normal" && c in yc && (b = yc[c]), d === "" || d ? (x = parseFloat(b), d === !0 || isFinite(x) ? x || 0 : b) : b
+                return C || (c = Pl(T)), w = p.cssHooks[c] || p.cssHooks[T], w && "get" in w && (b = w.get(a, !0, d)), b === void 0 && (b = zt(a, c, g)), b === "normal" && c in yc && (b = yc[c]), d === "" || d ? (x = parseFloat(b), d === !0 || isFinite(x) ? x || 0 : b) : b
             }
         }), p.each(["height", "width"], function(a, c) {
             p.cssHooks[c] = {
-                get: function(d, m, b) {
-                    if (m) return gm.test(p.css(d, "display")) && (!d.getClientRects().length || !d.getBoundingClientRect().width) ? Ze(d, mm, function() {
+                get: function(d, g, b) {
+                    if (g) return gm.test(p.css(d, "display")) && (!d.getClientRects().length || !d.getBoundingClientRect().width) ? Ze(d, mm, function() {
                         return xc(d, c, b)
                     }) : xc(d, c, b)
                 },
-                set: function(d, m, b) {
+                set: function(d, g, b) {
                     var x, w = Ke(d),
                         T = !v.scrollboxSize() && w.position === "absolute",
                         C = T || b,
                         E = C && p.css(d, "boxSizing", !1, w) === "border-box",
                         I = b ? Nl(d, c, b, E, w) : 0;
-                    return E && T && (I -= Math.ceil(d["offset" + c[0].toUpperCase() + c.slice(1)] - parseFloat(w[c]) - Nl(d, c, "border", !1, w) - .5)), I && (x = Jt.exec(m)) && (x[3] || "px") !== "px" && (d.style[c] = m, m = p.css(d, c)), bc(d, m, I)
+                    return E && T && (I -= Math.ceil(d["offset" + c[0].toUpperCase() + c.slice(1)] - parseFloat(w[c]) - Nl(d, c, "border", !1, w) - .5)), I && (x = Jt.exec(g)) && (x[3] || "px") !== "px" && (d.style[c] = g, g = p.css(d, c)), bc(d, g, I)
                 }
             }
         }), p.cssHooks.marginLeft = sn(v.reliableMarginLeft, function(a, c) {
             if (c) return (parseFloat(zt(a, "marginLeft")) || a.getBoundingClientRect().left - Ze(a, {
                 marginLeft: 0
             }, function() {
                 return a.getBoundingClientRect().left
@@ -2193,39 +2193,39 @@
         }), p.each({
             margin: "",
             padding: "",
             border: "Width"
         }, function(a, c) {
             p.cssHooks[a + c] = {
                 expand: function(d) {
-                    for (var m = 0, b = {}, x = typeof d == "string" ? d.split(" ") : [d]; m < 4; m++) b[a + Ft[m] + c] = x[m] || x[m - 2] || x[0];
+                    for (var g = 0, b = {}, x = typeof d == "string" ? d.split(" ") : [d]; g < 4; g++) b[a + Ft[g] + c] = x[g] || x[g - 2] || x[0];
                     return b
                 }
             }, a !== "margin" && (p.cssHooks[a + c].set = bc)
         }), p.fn.extend({
             css: function(a, c) {
-                return Kt(this, function(d, m, b) {
+                return Kt(this, function(d, g, b) {
                     var x, w, T = {},
                         C = 0;
-                    if (Array.isArray(m)) {
-                        for (x = Ke(d), w = m.length; C < w; C++) T[m[C]] = p.css(d, m[C], !1, x);
+                    if (Array.isArray(g)) {
+                        for (x = Ke(d), w = g.length; C < w; C++) T[g[C]] = p.css(d, g[C], !1, x);
                         return T
                     }
-                    return b !== void 0 ? p.style(d, m, b) : p.css(d, m)
+                    return b !== void 0 ? p.style(d, g, b) : p.css(d, g)
                 }, a, c, arguments.length > 1)
             }
         });
 
-        function Pt(a, c, d, m, b) {
-            return new Pt.prototype.init(a, c, d, m, b)
+        function Pt(a, c, d, g, b) {
+            return new Pt.prototype.init(a, c, d, g, b)
         }
         p.Tween = Pt, Pt.prototype = {
             constructor: Pt,
-            init: function(a, c, d, m, b, x) {
-                this.elem = a, this.prop = d, this.easing = b || p.easing._default, this.options = c, this.start = this.now = this.cur(), this.end = m, this.unit = x || (p.cssNumber[d] ? "" : "px")
+            init: function(a, c, d, g, b, x) {
+                this.elem = a, this.prop = d, this.easing = b || p.easing._default, this.options = c, this.start = this.now = this.cur(), this.end = g, this.unit = x || (p.cssNumber[d] ? "" : "px")
             },
             cur: function() {
                 var a = Pt.propHooks[this.prop];
                 return a && a.get ? a.get(this) : Pt.propHooks._default.get(this)
             },
             run: function(a) {
                 var c, d = Pt.propHooks[this.prop];
@@ -2264,73 +2264,73 @@
         function kc() {
             return e.setTimeout(function() {
                 rr = void 0
             }), rr = Date.now()
         }
 
         function Qs(a, c) {
-            var d, m = 0,
+            var d, g = 0,
                 b = {
                     height: a
                 };
-            for (c = c ? 1 : 0; m < 4; m += 2 - c) d = Ft[m], b["margin" + d] = b["padding" + d] = a;
+            for (c = c ? 1 : 0; g < 4; g += 2 - c) d = Ft[g], b["margin" + d] = b["padding" + d] = a;
             return c && (b.opacity = b.width = a), b
         }
 
         function wc(a, c, d) {
-            for (var m, b = (ci.tweeners[c] || []).concat(ci.tweeners["*"]), x = 0, w = b.length; x < w; x++)
-                if (m = b[x].call(d, c, a)) return m
+            for (var g, b = (ci.tweeners[c] || []).concat(ci.tweeners["*"]), x = 0, w = b.length; x < w; x++)
+                if (g = b[x].call(d, c, a)) return g
         }
 
         function xm(a, c, d) {
-            var m, b, x, w, T, C, E, I, _ = "width" in c || "height" in c,
+            var g, b, x, w, T, C, E, I, _ = "width" in c || "height" in c,
                 P = this,
                 W = {},
                 ce = a.style,
                 Ae = a.nodeType && Zn(a),
                 ge = ne.get(a, "fxshow");
             d.queue || (w = p._queueHooks(a, "fx"), w.unqueued == null && (w.unqueued = 0, T = w.empty.fire, w.empty.fire = function() {
                 w.unqueued || T()
             }), w.unqueued++, P.always(function() {
                 P.always(function() {
                     w.unqueued--, p.queue(a, "fx").length || w.empty.fire()
                 })
             }));
-            for (m in c)
-                if (b = c[m], ym.test(b)) {
-                    if (delete c[m], x = x || b === "toggle", b === (Ae ? "hide" : "show"))
-                        if (b === "show" && ge && ge[m] !== void 0) Ae = !0;
+            for (g in c)
+                if (b = c[g], ym.test(b)) {
+                    if (delete c[g], x = x || b === "toggle", b === (Ae ? "hide" : "show"))
+                        if (b === "show" && ge && ge[g] !== void 0) Ae = !0;
                         else continue;
-                    W[m] = ge && ge[m] || p.style(a, m)
+                    W[g] = ge && ge[g] || p.style(a, g)
                 } if (C = !p.isEmptyObject(c), !(!C && p.isEmptyObject(W))) {
                 _ && a.nodeType === 1 && (d.overflow = [ce.overflow, ce.overflowX, ce.overflowY], E = ge && ge.display, E == null && (E = ne.get(a, "display")), I = p.css(a, "display"), I === "none" && (E ? I = E : (nn([a], !0), E = a.style.display || E, I = p.css(a, "display"), nn([a]))), (I === "inline" || I === "inline-block" && E != null) && p.css(a, "float") === "none" && (C || (P.done(function() {
                     ce.display = E
                 }), E == null && (I = ce.display, E = I === "none" ? "" : I)), ce.display = "inline-block")), d.overflow && (ce.overflow = "hidden", P.always(function() {
                     ce.overflow = d.overflow[0], ce.overflowX = d.overflow[1], ce.overflowY = d.overflow[2]
                 })), C = !1;
-                for (m in W) C || (ge ? "hidden" in ge && (Ae = ge.hidden) : ge = ne.access(a, "fxshow", {
+                for (g in W) C || (ge ? "hidden" in ge && (Ae = ge.hidden) : ge = ne.access(a, "fxshow", {
                     display: E
                 }), x && (ge.hidden = !Ae), Ae && nn([a], !0), P.done(function() {
                     Ae || nn([a]), ne.remove(a, "fxshow");
-                    for (m in W) p.style(a, m, W[m])
-                })), C = wc(Ae ? ge[m] : 0, m, P), m in ge || (ge[m] = C.start, Ae && (C.end = C.start, C.start = 0))
+                    for (g in W) p.style(a, g, W[g])
+                })), C = wc(Ae ? ge[g] : 0, g, P), g in ge || (ge[g] = C.start, Ae && (C.end = C.start, C.start = 0))
             }
         }
 
         function km(a, c) {
-            var d, m, b, x, w;
+            var d, g, b, x, w;
             for (d in a)
-                if (m = ht(d), b = c[m], x = a[d], Array.isArray(x) && (b = x[1], x = a[d] = x[0]), d !== m && (a[m] = x, delete a[d]), w = p.cssHooks[m], w && "expand" in w) {
-                    x = w.expand(x), delete a[m];
+                if (g = ht(d), b = c[g], x = a[d], Array.isArray(x) && (b = x[1], x = a[d] = x[0]), d !== g && (a[g] = x, delete a[d]), w = p.cssHooks[g], w && "expand" in w) {
+                    x = w.expand(x), delete a[g];
                     for (d in x) d in a || (a[d] = x[d], c[d] = b)
-                } else c[m] = b
+                } else c[g] = b
         }
 
         function ci(a, c, d) {
-            var m, b, x = 0,
+            var g, b, x = 0,
                 w = ci.prefilters.length,
                 T = p.Deferred().always(function() {
                     delete C.elem
                 }),
                 C = function() {
                     if (b) return !1;
                     for (var _ = rr || kc(), P = Math.max(0, E.startTime + E.duration - _), W = P / E.duration || 0, ce = 1 - W, Ae = 0, ge = E.tweens.length; Ae < ge; Ae++) E.tweens[Ae].run(ce);
@@ -2358,15 +2358,15 @@
                         if (b) return this;
                         for (b = !0; P < W; P++) E.tweens[P].run(1);
                         return _ ? (T.notifyWith(a, [E, 1, 0]), T.resolveWith(a, [E, _])) : T.rejectWith(a, [E, _]), this
                     }
                 }),
                 I = E.props;
             for (km(I, E.opts.specialEasing); x < w; x++)
-                if (m = ci.prefilters[x].call(E, a, I, E.opts), m) return A(m.stop) && (p._queueHooks(E.elem, E.opts.queue).stop = m.stop.bind(m)), m;
+                if (g = ci.prefilters[x].call(E, a, I, E.opts), g) return A(g.stop) && (p._queueHooks(E.elem, E.opts.queue).stop = g.stop.bind(g)), g;
             return p.map(I, wc, E), A(E.opts.start) && E.opts.start.call(a, E), E.progress(E.opts.progress).done(E.opts.done, E.opts.complete).fail(E.opts.fail).always(E.opts.always), p.fx.timer(p.extend(C, {
                 elem: a,
                 anim: E,
                 queue: E.opts.queue
             })), E
         }
         p.Animation = p.extend(ci, {
@@ -2374,77 +2374,77 @@
                     "*": [function(a, c) {
                         var d = this.createTween(a, c);
                         return Hs(d.elem, a, Jt.exec(c), d), d
                     }]
                 },
                 tweener: function(a, c) {
                     A(a) ? (c = a, a = ["*"]) : a = a.match(at);
-                    for (var d, m = 0, b = a.length; m < b; m++) d = a[m], ci.tweeners[d] = ci.tweeners[d] || [], ci.tweeners[d].unshift(c)
+                    for (var d, g = 0, b = a.length; g < b; g++) d = a[g], ci.tweeners[d] = ci.tweeners[d] || [], ci.tweeners[d].unshift(c)
                 },
                 prefilters: [xm],
                 prefilter: function(a, c) {
                     c ? ci.prefilters.unshift(a) : ci.prefilters.push(a)
                 }
             }), p.speed = function(a, c, d) {
-                var m = a && typeof a == "object" ? p.extend({}, a) : {
+                var g = a && typeof a == "object" ? p.extend({}, a) : {
                     complete: d || !d && c || A(a) && a,
                     duration: a,
                     easing: d && c || c && !A(c) && c
                 };
-                return p.fx.off ? m.duration = 0 : typeof m.duration != "number" && (m.duration in p.fx.speeds ? m.duration = p.fx.speeds[m.duration] : m.duration = p.fx.speeds._default), (m.queue == null || m.queue === !0) && (m.queue = "fx"), m.old = m.complete, m.complete = function() {
-                    A(m.old) && m.old.call(this), m.queue && p.dequeue(this, m.queue)
-                }, m
+                return p.fx.off ? g.duration = 0 : typeof g.duration != "number" && (g.duration in p.fx.speeds ? g.duration = p.fx.speeds[g.duration] : g.duration = p.fx.speeds._default), (g.queue == null || g.queue === !0) && (g.queue = "fx"), g.old = g.complete, g.complete = function() {
+                    A(g.old) && g.old.call(this), g.queue && p.dequeue(this, g.queue)
+                }, g
             }, p.fn.extend({
-                fadeTo: function(a, c, d, m) {
+                fadeTo: function(a, c, d, g) {
                     return this.filter(Zn).css("opacity", 0).show().end().animate({
                         opacity: c
-                    }, a, d, m)
+                    }, a, d, g)
                 },
-                animate: function(a, c, d, m) {
+                animate: function(a, c, d, g) {
                     var b = p.isEmptyObject(a),
-                        x = p.speed(c, d, m),
+                        x = p.speed(c, d, g),
                         w = function() {
                             var T = ci(this, p.extend({}, a), x);
                             (b || ne.get(this, "finish")) && T.stop(!0)
                         };
                     return w.finish = w, b || x.queue === !1 ? this.each(w) : this.queue(x.queue, w)
                 },
                 stop: function(a, c, d) {
-                    var m = function(b) {
+                    var g = function(b) {
                         var x = b.stop;
                         delete b.stop, x(d)
                     };
                     return typeof a != "string" && (d = c, c = a, a = void 0), c && this.queue(a || "fx", []), this.each(function() {
                         var b = !0,
                             x = a != null && a + "queueHooks",
                             w = p.timers,
                             T = ne.get(this);
-                        if (x) T[x] && T[x].stop && m(T[x]);
+                        if (x) T[x] && T[x].stop && g(T[x]);
                         else
-                            for (x in T) T[x] && T[x].stop && bm.test(x) && m(T[x]);
+                            for (x in T) T[x] && T[x].stop && bm.test(x) && g(T[x]);
                         for (x = w.length; x--;) w[x].elem === this && (a == null || w[x].queue === a) && (w[x].anim.stop(d), b = !1, w.splice(x, 1));
                         (b || !d) && p.dequeue(this, a)
                     })
                 },
                 finish: function(a) {
                     return a !== !1 && (a = a || "fx"), this.each(function() {
                         var c, d = ne.get(this),
-                            m = d[a + "queue"],
+                            g = d[a + "queue"],
                             b = d[a + "queueHooks"],
                             x = p.timers,
-                            w = m ? m.length : 0;
+                            w = g ? g.length : 0;
                         for (d.finish = !0, p.queue(this, a, []), b && b.stop && b.stop.call(this, !0), c = x.length; c--;) x[c].elem === this && x[c].queue === a && (x[c].anim.stop(!0), x.splice(c, 1));
-                        for (c = 0; c < w; c++) m[c] && m[c].finish && m[c].finish.call(this);
+                        for (c = 0; c < w; c++) g[c] && g[c].finish && g[c].finish.call(this);
                         delete d.finish
                     })
                 }
             }), p.each(["toggle", "show", "hide"], function(a, c) {
                 var d = p.fn[c];
-                p.fn[c] = function(m, b, x) {
-                    return m == null || typeof m == "boolean" ? d.apply(this, arguments) : this.animate(Qs(c, !0), m, b, x)
+                p.fn[c] = function(g, b, x) {
+                    return g == null || typeof g == "boolean" ? d.apply(this, arguments) : this.animate(Qs(c, !0), g, b, x)
                 }
             }), p.each({
                 slideDown: Qs("show"),
                 slideUp: Qs("hide"),
                 slideToggle: Qs("toggle"),
                 fadeIn: {
                     opacity: "show"
@@ -2452,16 +2452,16 @@
                 fadeOut: {
                     opacity: "hide"
                 },
                 fadeToggle: {
                     opacity: "toggle"
                 }
             }, function(a, c) {
-                p.fn[a] = function(d, m, b) {
-                    return this.animate(c, d, m, b)
+                p.fn[a] = function(d, g, b) {
+                    return this.animate(c, d, g, b)
                 }
             }), p.timers = [], p.fx.tick = function() {
                 var a, c = 0,
                     d = p.timers;
                 for (rr = Date.now(); c < d.length; c++) a = d[c], !a() && d[c] === a && d.splice(c--, 1);
                 d.length || p.fx.stop(), rr = void 0
             }, p.fx.timer = function(a) {
@@ -2471,17 +2471,17 @@
             }, p.fx.stop = function() {
                 Us = null
             }, p.fx.speeds = {
                 slow: 600,
                 fast: 200,
                 _default: 400
             }, p.fn.delay = function(a, c) {
-                return a = p.fx && p.fx.speeds[a] || a, c = c || "fx", this.queue(c, function(d, m) {
+                return a = p.fx && p.fx.speeds[a] || a, c = c || "fx", this.queue(c, function(d, g) {
                     var b = e.setTimeout(d, a);
-                    m.stop = function() {
+                    g.stop = function() {
                         e.clearTimeout(b)
                     }
                 })
             },
             function() {
                 var a = D.createElement("input"),
                     c = D.createElement("select"),
@@ -2496,52 +2496,52 @@
             removeAttr: function(a) {
                 return this.each(function() {
                     p.removeAttr(this, a)
                 })
             }
         }), p.extend({
             attr: function(a, c, d) {
-                var m, b, x = a.nodeType;
+                var g, b, x = a.nodeType;
                 if (!(x === 3 || x === 8 || x === 2)) {
                     if (typeof a.getAttribute == "undefined") return p.prop(a, c, d);
                     if ((x !== 1 || !p.isXMLDoc(a)) && (b = p.attrHooks[c.toLowerCase()] || (p.expr.match.bool.test(c) ? vc : void 0)), d !== void 0) {
                         if (d === null) {
                             p.removeAttr(a, c);
                             return
                         }
-                        return b && "set" in b && (m = b.set(a, d, c)) !== void 0 ? m : (a.setAttribute(c, d + ""), d)
+                        return b && "set" in b && (g = b.set(a, d, c)) !== void 0 ? g : (a.setAttribute(c, d + ""), d)
                     }
-                    return b && "get" in b && (m = b.get(a, c)) !== null ? m : (m = p.find.attr(a, c), m == null ? void 0 : m)
+                    return b && "get" in b && (g = b.get(a, c)) !== null ? g : (g = p.find.attr(a, c), g == null ? void 0 : g)
                 }
             },
             attrHooks: {
                 type: {
                     set: function(a, c) {
                         if (!v.radioValue && c === "radio" && J(a, "input")) {
                             var d = a.value;
                             return a.setAttribute("type", c), d && (a.value = d), c
                         }
                     }
                 }
             },
             removeAttr: function(a, c) {
-                var d, m = 0,
+                var d, g = 0,
                     b = c && c.match(at);
                 if (b && a.nodeType === 1)
-                    for (; d = b[m++];) a.removeAttribute(d)
+                    for (; d = b[g++];) a.removeAttribute(d)
             }
         }), vc = {
             set: function(a, c, d) {
                 return c === !1 ? p.removeAttr(a, d) : a.setAttribute(d, d), d
             }
         }, p.each(p.expr.match.bool.source.match(/\w+/g), function(a, c) {
             var d = Br[c] || p.find.attr;
-            Br[c] = function(m, b, x) {
+            Br[c] = function(g, b, x) {
                 var w, T, C = b.toLowerCase();
-                return x || (T = Br[C], Br[C] = w, w = d(m, b, x) != null ? C : null, Br[C] = T), w
+                return x || (T = Br[C], Br[C] = w, w = d(g, b, x) != null ? C : null, Br[C] = T), w
             }
         });
         var wm = /^(?:input|select|textarea|button)$/i,
             vm = /^(?:a|area)$/i;
         p.fn.extend({
             prop: function(a, c) {
                 return Kt(this, p.prop, a, c, arguments.length > 1)
@@ -2549,16 +2549,16 @@
             removeProp: function(a) {
                 return this.each(function() {
                     delete this[p.propFix[a] || a]
                 })
             }
         }), p.extend({
             prop: function(a, c, d) {
-                var m, b, x = a.nodeType;
-                if (!(x === 3 || x === 8 || x === 2)) return (x !== 1 || !p.isXMLDoc(a)) && (c = p.propFix[c] || c, b = p.propHooks[c]), d !== void 0 ? b && "set" in b && (m = b.set(a, d, c)) !== void 0 ? m : a[c] = d : b && "get" in b && (m = b.get(a, c)) !== null ? m : a[c]
+                var g, b, x = a.nodeType;
+                if (!(x === 3 || x === 8 || x === 2)) return (x !== 1 || !p.isXMLDoc(a)) && (c = p.propFix[c] || c, b = p.propHooks[c]), d !== void 0 ? b && "set" in b && (g = b.set(a, d, c)) !== void 0 ? g : a[c] = d : b && "get" in b && (g = b.get(a, c)) !== null ? g : a[c]
             },
             propHooks: {
                 tabIndex: {
                     get: function(a) {
                         var c = p.find.attr(a, "tabindex");
                         return c ? parseInt(c, 10) : wm.test(a.nodeName) || vm.test(a.nodeName) && a.href ? 0 : -1
                     }
@@ -2591,88 +2591,88 @@
         }
 
         function Bl(a) {
             return Array.isArray(a) ? a : typeof a == "string" ? a.match(at) || [] : []
         }
         p.fn.extend({
             addClass: function(a) {
-                var c, d, m, b, x, w;
+                var c, d, g, b, x, w;
                 return A(a) ? this.each(function(T) {
                     p(this).addClass(a.call(this, T, Pn(this)))
                 }) : (c = Bl(a), c.length ? this.each(function() {
-                    if (m = Pn(this), d = this.nodeType === 1 && " " + Ln(m) + " ", d) {
+                    if (g = Pn(this), d = this.nodeType === 1 && " " + Ln(g) + " ", d) {
                         for (x = 0; x < c.length; x++) b = c[x], d.indexOf(" " + b + " ") < 0 && (d += b + " ");
-                        w = Ln(d), m !== w && this.setAttribute("class", w)
+                        w = Ln(d), g !== w && this.setAttribute("class", w)
                     }
                 }) : this)
             },
             removeClass: function(a) {
-                var c, d, m, b, x, w;
+                var c, d, g, b, x, w;
                 return A(a) ? this.each(function(T) {
                     p(this).removeClass(a.call(this, T, Pn(this)))
                 }) : arguments.length ? (c = Bl(a), c.length ? this.each(function() {
-                    if (m = Pn(this), d = this.nodeType === 1 && " " + Ln(m) + " ", d) {
+                    if (g = Pn(this), d = this.nodeType === 1 && " " + Ln(g) + " ", d) {
                         for (x = 0; x < c.length; x++)
                             for (b = c[x]; d.indexOf(" " + b + " ") > -1;) d = d.replace(" " + b + " ", " ");
-                        w = Ln(d), m !== w && this.setAttribute("class", w)
+                        w = Ln(d), g !== w && this.setAttribute("class", w)
                     }
                 }) : this) : this.attr("class", "")
             },
             toggleClass: function(a, c) {
-                var d, m, b, x, w = typeof a,
+                var d, g, b, x, w = typeof a,
                     T = w === "string" || Array.isArray(a);
                 return A(a) ? this.each(function(C) {
                     p(this).toggleClass(a.call(this, C, Pn(this), c), c)
                 }) : typeof c == "boolean" && T ? c ? this.addClass(a) : this.removeClass(a) : (d = Bl(a), this.each(function() {
                     if (T)
-                        for (x = p(this), b = 0; b < d.length; b++) m = d[b], x.hasClass(m) ? x.removeClass(m) : x.addClass(m);
-                    else(a === void 0 || w === "boolean") && (m = Pn(this), m && ne.set(this, "__className__", m), this.setAttribute && this.setAttribute("class", m || a === !1 ? "" : ne.get(this, "__className__") || ""))
+                        for (x = p(this), b = 0; b < d.length; b++) g = d[b], x.hasClass(g) ? x.removeClass(g) : x.addClass(g);
+                    else(a === void 0 || w === "boolean") && (g = Pn(this), g && ne.set(this, "__className__", g), this.setAttribute && this.setAttribute("class", g || a === !1 ? "" : ne.get(this, "__className__") || ""))
                 }))
             },
             hasClass: function(a) {
-                var c, d, m = 0;
-                for (c = " " + a + " "; d = this[m++];)
+                var c, d, g = 0;
+                for (c = " " + a + " "; d = this[g++];)
                     if (d.nodeType === 1 && (" " + Ln(Pn(d)) + " ").indexOf(c) > -1) return !0;
                 return !1
             }
         });
         var Sm = /\r/g;
         p.fn.extend({
             val: function(a) {
-                var c, d, m, b = this[0];
-                return arguments.length ? (m = A(a), this.each(function(x) {
+                var c, d, g, b = this[0];
+                return arguments.length ? (g = A(a), this.each(function(x) {
                     var w;
-                    this.nodeType === 1 && (m ? w = a.call(this, x, p(this).val()) : w = a, w == null ? w = "" : typeof w == "number" ? w += "" : Array.isArray(w) && (w = p.map(w, function(T) {
+                    this.nodeType === 1 && (g ? w = a.call(this, x, p(this).val()) : w = a, w == null ? w = "" : typeof w == "number" ? w += "" : Array.isArray(w) && (w = p.map(w, function(T) {
                         return T == null ? "" : T + ""
                     })), c = p.valHooks[this.type] || p.valHooks[this.nodeName.toLowerCase()], (!c || !("set" in c) || c.set(this, w, "value") === void 0) && (this.value = w))
                 })) : b ? (c = p.valHooks[b.type] || p.valHooks[b.nodeName.toLowerCase()], c && "get" in c && (d = c.get(b, "value")) !== void 0 ? d : (d = b.value, typeof d == "string" ? d.replace(Sm, "") : d == null ? "" : d)) : void 0
             }
         }), p.extend({
             valHooks: {
                 option: {
                     get: function(a) {
                         var c = p.find.attr(a, "value");
                         return c != null ? c : Ln(p.text(a))
                     }
                 },
                 select: {
                     get: function(a) {
-                        var c, d, m, b = a.options,
+                        var c, d, g, b = a.options,
                             x = a.selectedIndex,
                             w = a.type === "select-one",
                             T = w ? null : [],
                             C = w ? x + 1 : b.length;
-                        for (x < 0 ? m = C : m = w ? x : 0; m < C; m++)
-                            if (d = b[m], (d.selected || m === x) && !d.disabled && (!d.parentNode.disabled || !J(d.parentNode, "optgroup"))) {
+                        for (x < 0 ? g = C : g = w ? x : 0; g < C; g++)
+                            if (d = b[g], (d.selected || g === x) && !d.disabled && (!d.parentNode.disabled || !J(d.parentNode, "optgroup"))) {
                                 if (c = p(d).val(), w) return c;
                                 T.push(c)
                             } return T
                     },
                     set: function(a, c) {
-                        for (var d, m, b = a.options, x = p.makeArray(c), w = b.length; w--;) m = b[w], (m.selected = p.inArray(p.valHooks.option.get(m), x) > -1) && (d = !0);
+                        for (var d, g, b = a.options, x = p.makeArray(c), w = b.length; w--;) g = b[w], (g.selected = p.inArray(p.valHooks.option.get(g), x) > -1) && (d = !0);
                         return d || (a.selectedIndex = -1), x
                     }
                 }
             }
         }), p.each(["radio", "checkbox"], function() {
             p.valHooks[this] = {
                 set: function(a, c) {
@@ -2688,45 +2688,45 @@
             },
             _l = /\?/;
         p.parseXML = function(a) {
             var c, d;
             if (!a || typeof a != "string") return null;
             try {
                 c = new e.DOMParser().parseFromString(a, "text/xml")
-            } catch (m) {}
-            return d = c && c.getElementsByTagName("parsererror")[0], (!c || d) && p.error("Invalid XML: " + (d ? p.map(d.childNodes, function(m) {
-                return m.textContent
+            } catch (g) {}
+            return d = c && c.getElementsByTagName("parsererror")[0], (!c || d) && p.error("Invalid XML: " + (d ? p.map(d.childNodes, function(g) {
+                return g.textContent
             }).join(`
 `) : a)), c
         };
         var Cc = /^(?:focusinfocus|focusoutblur)$/,
             Ac = function(a) {
                 a.stopPropagation()
             };
         p.extend(p.event, {
-            trigger: function(a, c, d, m) {
+            trigger: function(a, c, d, g) {
                 var b, x, w, T, C, E, I, _, P = [d || D],
-                    W = g.call(a, "type") ? a.type : a,
-                    ce = g.call(a, "namespace") ? a.namespace.split(".") : [];
-                if (x = _ = w = d = d || D, !(d.nodeType === 3 || d.nodeType === 8) && !Cc.test(W + p.event.triggered) && (W.indexOf(".") > -1 && (ce = W.split("."), W = ce.shift(), ce.sort()), C = W.indexOf(":") < 0 && "on" + W, a = a[p.expando] ? a : new p.Event(W, typeof a == "object" && a), a.isTrigger = m ? 2 : 3, a.namespace = ce.join("."), a.rnamespace = a.namespace ? new RegExp("(^|\\.)" + ce.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, a.result = void 0, a.target || (a.target = d), c = c == null ? [a] : p.makeArray(c, [a]), I = p.event.special[W] || {}, !(!m && I.trigger && I.trigger.apply(d, c) === !1))) {
-                    if (!m && !I.noBubble && !O(d)) {
+                    W = m.call(a, "type") ? a.type : a,
+                    ce = m.call(a, "namespace") ? a.namespace.split(".") : [];
+                if (x = _ = w = d = d || D, !(d.nodeType === 3 || d.nodeType === 8) && !Cc.test(W + p.event.triggered) && (W.indexOf(".") > -1 && (ce = W.split("."), W = ce.shift(), ce.sort()), C = W.indexOf(":") < 0 && "on" + W, a = a[p.expando] ? a : new p.Event(W, typeof a == "object" && a), a.isTrigger = g ? 2 : 3, a.namespace = ce.join("."), a.rnamespace = a.namespace ? new RegExp("(^|\\.)" + ce.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, a.result = void 0, a.target || (a.target = d), c = c == null ? [a] : p.makeArray(c, [a]), I = p.event.special[W] || {}, !(!g && I.trigger && I.trigger.apply(d, c) === !1))) {
+                    if (!g && !I.noBubble && !O(d)) {
                         for (T = I.delegateType || W, Cc.test(T + W) || (x = x.parentNode); x; x = x.parentNode) P.push(x), w = x;
                         w === (d.ownerDocument || D) && P.push(w.defaultView || w.parentWindow || e)
                     }
                     for (b = 0;
                         (x = P[b++]) && !a.isPropagationStopped();) _ = x, a.type = b > 1 ? T : I.bindType || W, E = (ne.get(x, "events") || Object.create(null))[a.type] && ne.get(x, "handle"), E && E.apply(x, c), E = C && x[C], E && E.apply && Xt(x) && (a.result = E.apply(x, c), a.result === !1 && a.preventDefault());
-                    return a.type = W, !m && !a.isDefaultPrevented() && (!I._default || I._default.apply(P.pop(), c) === !1) && Xt(d) && C && A(d[W]) && !O(d) && (w = d[C], w && (d[C] = null), p.event.triggered = W, a.isPropagationStopped() && _.addEventListener(W, Ac), d[W](), a.isPropagationStopped() && _.removeEventListener(W, Ac), p.event.triggered = void 0, w && (d[C] = w)), a.result
+                    return a.type = W, !g && !a.isDefaultPrevented() && (!I._default || I._default.apply(P.pop(), c) === !1) && Xt(d) && C && A(d[W]) && !O(d) && (w = d[C], w && (d[C] = null), p.event.triggered = W, a.isPropagationStopped() && _.addEventListener(W, Ac), d[W](), a.isPropagationStopped() && _.removeEventListener(W, Ac), p.event.triggered = void 0, w && (d[C] = w)), a.result
                 }
             },
             simulate: function(a, c, d) {
-                var m = p.extend(new p.Event, d, {
+                var g = p.extend(new p.Event, d, {
                     type: a,
                     isSimulated: !0
                 });
-                p.event.trigger(m, null, c)
+                p.event.trigger(g, null, c)
             }
         }), p.fn.extend({
             trigger: function(a, c) {
                 return this.each(function() {
                     p.event.trigger(a, c, this)
                 })
             },
@@ -2736,53 +2736,53 @@
             }
         });
         var Cm = /\[\]$/,
             Tc = /\r?\n/g,
             Am = /^(?:submit|button|image|reset|file)$/i,
             Tm = /^(?:input|select|textarea|keygen)/i;
 
-        function Hl(a, c, d, m) {
+        function Hl(a, c, d, g) {
             var b;
             if (Array.isArray(c)) p.each(c, function(x, w) {
-                d || Cm.test(a) ? m(a, w) : Hl(a + "[" + (typeof w == "object" && w != null ? x : "") + "]", w, d, m)
+                d || Cm.test(a) ? g(a, w) : Hl(a + "[" + (typeof w == "object" && w != null ? x : "") + "]", w, d, g)
             });
             else if (!d && j(c) === "object")
-                for (b in c) Hl(a + "[" + b + "]", c[b], d, m);
-            else m(a, c)
+                for (b in c) Hl(a + "[" + b + "]", c[b], d, g);
+            else g(a, c)
         }
         p.param = function(a, c) {
-            var d, m = [],
+            var d, g = [],
                 b = function(x, w) {
                     var T = A(w) ? w() : w;
-                    m[m.length] = encodeURIComponent(x) + "=" + encodeURIComponent(T == null ? "" : T)
+                    g[g.length] = encodeURIComponent(x) + "=" + encodeURIComponent(T == null ? "" : T)
                 };
             if (a == null) return "";
             if (Array.isArray(a) || a.jquery && !p.isPlainObject(a)) p.each(a, function() {
                 b(this.name, this.value)
             });
             else
                 for (d in a) Hl(d, a[d], c, b);
-            return m.join("&")
+            return g.join("&")
         }, p.fn.extend({
             serialize: function() {
                 return p.param(this.serializeArray())
             },
             serializeArray: function() {
                 return this.map(function() {
                     var a = p.prop(this, "elements");
                     return a ? p.makeArray(a) : this
                 }).filter(function() {
                     var a = this.type;
                     return this.name && !p(this).is(":disabled") && Tm.test(this.nodeName) && !Am.test(a) && (this.checked || !rn.test(a))
                 }).map(function(a, c) {
                     var d = p(this).val();
-                    return d == null ? null : Array.isArray(d) ? p.map(d, function(m) {
+                    return d == null ? null : Array.isArray(d) ? p.map(d, function(g) {
                         return {
                             name: c.name,
-                            value: m.replace(Tc, `\r
+                            value: g.replace(Tc, `\r
 `)
                         }
                     }) : {
                         name: c.name,
                         value: d.replace(Tc, `\r
 `)
                     }
@@ -2801,47 +2801,47 @@
             Mc = "*/".concat("*"),
             zl = D.createElement("a");
         zl.href = _r.href;
 
         function Ec(a) {
             return function(c, d) {
                 typeof c != "string" && (d = c, c = "*");
-                var m, b = 0,
+                var g, b = 0,
                     x = c.toLowerCase().match(at) || [];
                 if (A(d))
-                    for (; m = x[b++];) m[0] === "+" ? (m = m.slice(1) || "*", (a[m] = a[m] || []).unshift(d)) : (a[m] = a[m] || []).push(d)
+                    for (; g = x[b++];) g[0] === "+" ? (g = g.slice(1) || "*", (a[g] = a[g] || []).unshift(d)) : (a[g] = a[g] || []).push(d)
             }
         }
 
-        function Dc(a, c, d, m) {
+        function Dc(a, c, d, g) {
             var b = {},
                 x = a === Fl;
 
             function w(T) {
                 var C;
                 return b[T] = !0, p.each(a[T] || [], function(E, I) {
-                    var _ = I(c, d, m);
+                    var _ = I(c, d, g);
                     if (typeof _ == "string" && !x && !b[_]) return c.dataTypes.unshift(_), w(_), !1;
                     if (x) return !(C = _)
                 }), C
             }
             return w(c.dataTypes[0]) || !b["*"] && w("*")
         }
 
         function $l(a, c) {
-            var d, m, b = p.ajaxSettings.flatOptions || {};
-            for (d in c) c[d] !== void 0 && ((b[d] ? a : m || (m = {}))[d] = c[d]);
-            return m && p.extend(!0, a, m), a
+            var d, g, b = p.ajaxSettings.flatOptions || {};
+            for (d in c) c[d] !== void 0 && ((b[d] ? a : g || (g = {}))[d] = c[d]);
+            return g && p.extend(!0, a, g), a
         }
 
         function Nm(a, c, d) {
-            for (var m, b, x, w, T = a.contents, C = a.dataTypes; C[0] === "*";) C.shift(), m === void 0 && (m = a.mimeType || c.getResponseHeader("Content-Type"));
-            if (m) {
+            for (var g, b, x, w, T = a.contents, C = a.dataTypes; C[0] === "*";) C.shift(), g === void 0 && (g = a.mimeType || c.getResponseHeader("Content-Type"));
+            if (g) {
                 for (b in T)
-                    if (T[b] && T[b].test(m)) {
+                    if (T[b] && T[b].test(g)) {
                         C.unshift(b);
                         break
                     }
             }
             if (C[0] in d) x = C[0];
             else {
                 for (b in d) {
@@ -2852,21 +2852,21 @@
                     w || (w = b)
                 }
                 x = x || w
             }
             if (x) return x !== C[0] && C.unshift(x), d[x]
         }
 
-        function Im(a, c, d, m) {
+        function Im(a, c, d, g) {
             var b, x, w, T, C, E = {},
                 I = a.dataTypes.slice();
             if (I[1])
                 for (w in a.converters) E[w.toLowerCase()] = a.converters[w];
             for (x = I.shift(); x;)
-                if (a.responseFields[x] && (d[a.responseFields[x]] = c), !C && m && a.dataFilter && (c = a.dataFilter(c, a.dataType)), C = x, x = I.shift(), x) {
+                if (a.responseFields[x] && (d[a.responseFields[x]] = c), !C && g && a.dataFilter && (c = a.dataFilter(c, a.dataType)), C = x, x = I.shift(), x) {
                     if (x === "*") x = C;
                     else if (C !== "*" && C !== x) {
                         if (w = E[C + " " + x] || E["* " + x], !w) {
                             for (b in E)
                                 if (T = b.split(" "), T[1] === x && (w = E[C + " " + T[0]] || E["* " + T[0]], w)) {
                                     w === !0 ? w = E[b] : E[b] !== !0 && (x = T[0], I.unshift(T[1]));
                                     break
@@ -2931,15 +2931,15 @@
             ajaxSetup: function(a, c) {
                 return c ? $l($l(a, p.ajaxSettings), c) : $l(p.ajaxSettings, a)
             },
             ajaxPrefilter: Ec(Oc),
             ajaxTransport: Ec(Fl),
             ajax: function(a, c) {
                 typeof a == "object" && (c = a, a = void 0), c = c || {};
-                var d, m, b, x, w, T, C, E, I, _, P = p.ajaxSetup({}, c),
+                var d, g, b, x, w, T, C, E, I, _, P = p.ajaxSetup({}, c),
                     W = P.context || P,
                     ce = P.context && (W.nodeType || W.jquery) ? p(W) : p.event,
                     Ae = p.Deferred(),
                     ge = p.Callbacks("once memory"),
                     ut = P.statusCode || {},
                     et = {},
                     wi = {},
@@ -2982,15 +2982,15 @@
                     try {
                         T.href = P.url, T.href = T.href, P.crossDomain = zl.protocol + "//" + zl.host != T.protocol + "//" + T.host
                     } catch (Me) {
                         P.crossDomain = !0
                     }
                 }
                 if (P.data && P.processData && typeof P.data != "string" && (P.data = p.param(P.data, P.traditional)), Dc(Oc, P, c, ve), C) return ve;
-                E = p.event && P.global, E && p.active++ === 0 && p.event.trigger("ajaxStart"), P.type = P.type.toUpperCase(), P.hasContent = !Lm.test(P.type), m = P.url.replace(Mm, ""), P.hasContent ? P.data && P.processData && (P.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && (P.data = P.data.replace(Om, "+")) : (_ = P.url.slice(m.length), P.data && (P.processData || typeof P.data == "string") && (m += (_l.test(m) ? "&" : "?") + P.data, delete P.data), P.cache === !1 && (m = m.replace(Em, "$1"), _ = (_l.test(m) ? "&" : "?") + "_=" + Sc.guid++ + _), P.url = m + _), P.ifModified && (p.lastModified[m] && ve.setRequestHeader("If-Modified-Since", p.lastModified[m]), p.etag[m] && ve.setRequestHeader("If-None-Match", p.etag[m])), (P.data && P.hasContent && P.contentType !== !1 || c.contentType) && ve.setRequestHeader("Content-Type", P.contentType), ve.setRequestHeader("Accept", P.dataTypes[0] && P.accepts[P.dataTypes[0]] ? P.accepts[P.dataTypes[0]] + (P.dataTypes[0] !== "*" ? ", " + Mc + "; q=0.01" : "") : P.accepts["*"]);
+                E = p.event && P.global, E && p.active++ === 0 && p.event.trigger("ajaxStart"), P.type = P.type.toUpperCase(), P.hasContent = !Lm.test(P.type), g = P.url.replace(Mm, ""), P.hasContent ? P.data && P.processData && (P.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && (P.data = P.data.replace(Om, "+")) : (_ = P.url.slice(g.length), P.data && (P.processData || typeof P.data == "string") && (g += (_l.test(g) ? "&" : "?") + P.data, delete P.data), P.cache === !1 && (g = g.replace(Em, "$1"), _ = (_l.test(g) ? "&" : "?") + "_=" + Sc.guid++ + _), P.url = g + _), P.ifModified && (p.lastModified[g] && ve.setRequestHeader("If-Modified-Since", p.lastModified[g]), p.etag[g] && ve.setRequestHeader("If-None-Match", p.etag[g])), (P.data && P.hasContent && P.contentType !== !1 || c.contentType) && ve.setRequestHeader("Content-Type", P.contentType), ve.setRequestHeader("Accept", P.dataTypes[0] && P.accepts[P.dataTypes[0]] ? P.accepts[P.dataTypes[0]] + (P.dataTypes[0] !== "*" ? ", " + Mc + "; q=0.01" : "") : P.accepts["*"]);
                 for (I in P.headers) ve.setRequestHeader(I, P.headers[I]);
                 if (P.beforeSend && (P.beforeSend.call(W, ve, P) === !1 || C)) return ve.abort();
                 if (vi = "abort", ge.add(P.complete), ve.done(P.success), ve.fail(P.error), d = Dc(Fl, P, c, ve), !d) Nn(-1, "No Transport");
                 else {
                     if (ve.readyState = 1, E && ce.trigger("ajaxSend", [ve, P]), C) return ve;
                     P.async && P.timeout > 0 && (w = e.setTimeout(function() {
                         ve.abort("timeout")
@@ -3001,31 +3001,31 @@
                         if (C) throw Me;
                         Nn(-1, Me)
                     }
                 }
 
                 function Nn(Me, Qe, Fr, ql) {
                     var Si, zr, Ci, on, ln, Zt = Qe;
-                    C || (C = !0, w && e.clearTimeout(w), d = void 0, b = ql || "", ve.readyState = Me > 0 ? 4 : 0, Si = Me >= 200 && Me < 300 || Me === 304, Fr && (on = Nm(P, ve, Fr)), !Si && p.inArray("script", P.dataTypes) > -1 && p.inArray("json", P.dataTypes) < 0 && (P.converters["text script"] = function() {}), on = Im(P, on, ve, Si), Si ? (P.ifModified && (ln = ve.getResponseHeader("Last-Modified"), ln && (p.lastModified[m] = ln), ln = ve.getResponseHeader("etag"), ln && (p.etag[m] = ln)), Me === 204 || P.type === "HEAD" ? Zt = "nocontent" : Me === 304 ? Zt = "notmodified" : (Zt = on.state, zr = on.data, Ci = on.error, Si = !Ci)) : (Ci = Zt, (Me || !Zt) && (Zt = "error", Me < 0 && (Me = 0))), ve.status = Me, ve.statusText = (Qe || Zt) + "", Si ? Ae.resolveWith(W, [zr, Zt, ve]) : Ae.rejectWith(W, [ve, Zt, Ci]), ve.statusCode(ut), ut = void 0, E && ce.trigger(Si ? "ajaxSuccess" : "ajaxError", [ve, P, Si ? zr : Ci]), ge.fireWith(W, [ve, Zt]), E && (ce.trigger("ajaxComplete", [ve, P]), --p.active || p.event.trigger("ajaxStop")))
+                    C || (C = !0, w && e.clearTimeout(w), d = void 0, b = ql || "", ve.readyState = Me > 0 ? 4 : 0, Si = Me >= 200 && Me < 300 || Me === 304, Fr && (on = Nm(P, ve, Fr)), !Si && p.inArray("script", P.dataTypes) > -1 && p.inArray("json", P.dataTypes) < 0 && (P.converters["text script"] = function() {}), on = Im(P, on, ve, Si), Si ? (P.ifModified && (ln = ve.getResponseHeader("Last-Modified"), ln && (p.lastModified[g] = ln), ln = ve.getResponseHeader("etag"), ln && (p.etag[g] = ln)), Me === 204 || P.type === "HEAD" ? Zt = "nocontent" : Me === 304 ? Zt = "notmodified" : (Zt = on.state, zr = on.data, Ci = on.error, Si = !Ci)) : (Ci = Zt, (Me || !Zt) && (Zt = "error", Me < 0 && (Me = 0))), ve.status = Me, ve.statusText = (Qe || Zt) + "", Si ? Ae.resolveWith(W, [zr, Zt, ve]) : Ae.rejectWith(W, [ve, Zt, Ci]), ve.statusCode(ut), ut = void 0, E && ce.trigger(Si ? "ajaxSuccess" : "ajaxError", [ve, P, Si ? zr : Ci]), ge.fireWith(W, [ve, Zt]), E && (ce.trigger("ajaxComplete", [ve, P]), --p.active || p.event.trigger("ajaxStop")))
                 }
                 return ve
             },
             getJSON: function(a, c, d) {
                 return p.get(a, c, d, "json")
             },
             getScript: function(a, c) {
                 return p.get(a, void 0, c, "script")
             }
         }), p.each(["get", "post"], function(a, c) {
-            p[c] = function(d, m, b, x) {
-                return A(m) && (x = x || b, b = m, m = void 0), p.ajax(p.extend({
+            p[c] = function(d, g, b, x) {
+                return A(g) && (x = x || b, b = g, g = void 0), p.ajax(p.extend({
                     url: d,
                     type: c,
                     dataType: x,
-                    data: m,
+                    data: g,
                     success: b
                 }, p.isPlainObject(d) && d))
             }
         }), p.ajaxPrefilter(function(a) {
             var c;
             for (c in a.headers) c.toLowerCase() === "content-type" && (a.contentType = a.headers[c] || "")
         }), p._evalUrl = function(a, c, d) {
@@ -3035,16 +3035,16 @@
                 dataType: "script",
                 cache: !0,
                 async: !1,
                 global: !1,
                 converters: {
                     "text script": function() {}
                 },
-                dataFilter: function(m) {
-                    p.globalEval(m, c, d)
+                dataFilter: function(g) {
+                    p.globalEval(g, c, d)
                 }
             })
         }, p.fn.extend({
             wrapAll: function(a) {
                 var c;
                 return this[0] && (A(a) && (a = a.call(this[0])), c = p(a, this[0].ownerDocument).eq(0).clone(!0), this[0].parentNode && c.insertBefore(this[0]), c.map(function() {
                     for (var d = this; d.firstElementChild;) d = d.firstElementChild;
@@ -3084,20 +3084,20 @@
                 0: 200,
                 1223: 204
             },
             Hr = p.ajaxSettings.xhr();
         v.cors = !!Hr && "withCredentials" in Hr, v.ajax = Hr = !!Hr, p.ajaxTransport(function(a) {
             var c, d;
             if (v.cors || Hr && !a.crossDomain) return {
-                send: function(m, b) {
+                send: function(g, b) {
                     var x, w = a.xhr();
                     if (w.open(a.type, a.url, a.async, a.username, a.password), a.xhrFields)
                         for (x in a.xhrFields) w[x] = a.xhrFields[x];
-                    a.mimeType && w.overrideMimeType && w.overrideMimeType(a.mimeType), !a.crossDomain && !m["X-Requested-With"] && (m["X-Requested-With"] = "XMLHttpRequest");
-                    for (x in m) w.setRequestHeader(x, m[x]);
+                    a.mimeType && w.overrideMimeType && w.overrideMimeType(a.mimeType), !a.crossDomain && !g["X-Requested-With"] && (g["X-Requested-With"] = "XMLHttpRequest");
+                    for (x in g) w.setRequestHeader(x, g[x]);
                     c = function(T) {
                         return function() {
                             c && (c = d = w.onload = w.onerror = w.onabort = w.ontimeout = w.onreadystatechange = null, T === "abort" ? w.abort() : T === "error" ? typeof w.status != "number" ? b(0, "error") : b(w.status, w.statusText) : b(Bm[w.status] || w.status, w.statusText, (w.responseType || "text") !== "text" || typeof w.responseText != "string" ? {
                                 binary: w.response
                             } : {
                                 text: w.responseText
                             }, w.getAllResponseHeaders()))
@@ -3133,15 +3133,15 @@
             }
         }), p.ajaxPrefilter("script", function(a) {
             a.cache === void 0 && (a.cache = !1), a.crossDomain && (a.type = "GET")
         }), p.ajaxTransport("script", function(a) {
             if (a.crossDomain || a.scriptAttrs) {
                 var c, d;
                 return {
-                    send: function(m, b) {
+                    send: function(g, b) {
                         c = p("<script>").attr(a.scriptAttrs || {}).prop({
                             charset: a.scriptCharset,
                             src: a.url
                         }).on("load error", d = function(x) {
                             c.remove(), d = null, x && b(x.type === "error" ? 404 : 200, x.type)
                         }), D.head.appendChild(c[0])
                     },
@@ -3156,158 +3156,158 @@
         p.ajaxSetup({
             jsonp: "callback",
             jsonpCallback: function() {
                 var a = Rc.pop() || p.expando + "_" + Sc.guid++;
                 return this[a] = !0, a
             }
         }), p.ajaxPrefilter("json jsonp", function(a, c, d) {
-            var m, b, x, w = a.jsonp !== !1 && (Wl.test(a.url) ? "url" : typeof a.data == "string" && (a.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && Wl.test(a.data) && "data");
-            if (w || a.dataTypes[0] === "jsonp") return m = a.jsonpCallback = A(a.jsonpCallback) ? a.jsonpCallback() : a.jsonpCallback, w ? a[w] = a[w].replace(Wl, "$1" + m) : a.jsonp !== !1 && (a.url += (_l.test(a.url) ? "&" : "?") + a.jsonp + "=" + m), a.converters["script json"] = function() {
-                return x || p.error(m + " was not called"), x[0]
-            }, a.dataTypes[0] = "json", b = e[m], e[m] = function() {
+            var g, b, x, w = a.jsonp !== !1 && (Wl.test(a.url) ? "url" : typeof a.data == "string" && (a.contentType || "").indexOf("application/x-www-form-urlencoded") === 0 && Wl.test(a.data) && "data");
+            if (w || a.dataTypes[0] === "jsonp") return g = a.jsonpCallback = A(a.jsonpCallback) ? a.jsonpCallback() : a.jsonpCallback, w ? a[w] = a[w].replace(Wl, "$1" + g) : a.jsonp !== !1 && (a.url += (_l.test(a.url) ? "&" : "?") + a.jsonp + "=" + g), a.converters["script json"] = function() {
+                return x || p.error(g + " was not called"), x[0]
+            }, a.dataTypes[0] = "json", b = e[g], e[g] = function() {
                 x = arguments
             }, d.always(function() {
-                b === void 0 ? p(e).removeProp(m) : e[m] = b, a[m] && (a.jsonpCallback = c.jsonpCallback, Rc.push(m)), x && A(b) && b(x[0]), x = b = void 0
+                b === void 0 ? p(e).removeProp(g) : e[g] = b, a[g] && (a.jsonpCallback = c.jsonpCallback, Rc.push(g)), x && A(b) && b(x[0]), x = b = void 0
             }), "script"
         }), v.createHTMLDocument = function() {
             var a = D.implementation.createHTMLDocument("").body;
             return a.innerHTML = "<form></form><form></form>", a.childNodes.length === 2
         }(), p.parseHTML = function(a, c, d) {
             if (typeof a != "string") return [];
             typeof c == "boolean" && (d = c, c = !1);
-            var m, b, x;
-            return c || (v.createHTMLDocument ? (c = D.implementation.createHTMLDocument(""), m = c.createElement("base"), m.href = D.location.href, c.head.appendChild(m)) : c = D), b = bt.exec(a), x = !d && [], b ? [c.createElement(b[1])] : (b = zs([a], c, x), x && x.length && p(x).remove(), p.merge([], b.childNodes))
+            var g, b, x;
+            return c || (v.createHTMLDocument ? (c = D.implementation.createHTMLDocument(""), g = c.createElement("base"), g.href = D.location.href, c.head.appendChild(g)) : c = D), b = bt.exec(a), x = !d && [], b ? [c.createElement(b[1])] : (b = zs([a], c, x), x && x.length && p(x).remove(), p.merge([], b.childNodes))
         }, p.fn.load = function(a, c, d) {
-            var m, b, x, w = this,
+            var g, b, x, w = this,
                 T = a.indexOf(" ");
-            return T > -1 && (m = Ln(a.slice(T)), a = a.slice(0, T)), A(c) ? (d = c, c = void 0) : c && typeof c == "object" && (b = "POST"), w.length > 0 && p.ajax({
+            return T > -1 && (g = Ln(a.slice(T)), a = a.slice(0, T)), A(c) ? (d = c, c = void 0) : c && typeof c == "object" && (b = "POST"), w.length > 0 && p.ajax({
                 url: a,
                 type: b || "GET",
                 dataType: "html",
                 data: c
             }).done(function(C) {
-                x = arguments, w.html(m ? p("<div>").append(p.parseHTML(C)).find(m) : C)
+                x = arguments, w.html(g ? p("<div>").append(p.parseHTML(C)).find(g) : C)
             }).always(d && function(C, E) {
                 w.each(function() {
                     d.apply(this, x || [C.responseText, E, C])
                 })
             }), this
         }, p.expr.pseudos.animated = function(a) {
             return p.grep(p.timers, function(c) {
                 return a === c.elem
             }).length
         }, p.offset = {
             setOffset: function(a, c, d) {
-                var m, b, x, w, T, C, E, I = p.css(a, "position"),
+                var g, b, x, w, T, C, E, I = p.css(a, "position"),
                     _ = p(a),
                     P = {};
-                I === "static" && (a.style.position = "relative"), T = _.offset(), x = p.css(a, "top"), C = p.css(a, "left"), E = (I === "absolute" || I === "fixed") && (x + C).indexOf("auto") > -1, E ? (m = _.position(), w = m.top, b = m.left) : (w = parseFloat(x) || 0, b = parseFloat(C) || 0), A(c) && (c = c.call(a, d, p.extend({}, T))), c.top != null && (P.top = c.top - T.top + w), c.left != null && (P.left = c.left - T.left + b), "using" in c ? c.using.call(a, P) : _.css(P)
+                I === "static" && (a.style.position = "relative"), T = _.offset(), x = p.css(a, "top"), C = p.css(a, "left"), E = (I === "absolute" || I === "fixed") && (x + C).indexOf("auto") > -1, E ? (g = _.position(), w = g.top, b = g.left) : (w = parseFloat(x) || 0, b = parseFloat(C) || 0), A(c) && (c = c.call(a, d, p.extend({}, T))), c.top != null && (P.top = c.top - T.top + w), c.left != null && (P.left = c.left - T.left + b), "using" in c ? c.using.call(a, P) : _.css(P)
             }
         }, p.fn.extend({
             offset: function(a) {
                 if (arguments.length) return a === void 0 ? this : this.each(function(b) {
                     p.offset.setOffset(this, a, b)
                 });
-                var c, d, m = this[0];
-                if (m) return m.getClientRects().length ? (c = m.getBoundingClientRect(), d = m.ownerDocument.defaultView, {
+                var c, d, g = this[0];
+                if (g) return g.getClientRects().length ? (c = g.getBoundingClientRect(), d = g.ownerDocument.defaultView, {
                     top: c.top + d.pageYOffset,
                     left: c.left + d.pageXOffset
                 }) : {
                     top: 0,
                     left: 0
                 }
             },
             position: function() {
                 if (this[0]) {
-                    var a, c, d, m = this[0],
+                    var a, c, d, g = this[0],
                         b = {
                             top: 0,
                             left: 0
                         };
-                    if (p.css(m, "position") === "fixed") c = m.getBoundingClientRect();
+                    if (p.css(g, "position") === "fixed") c = g.getBoundingClientRect();
                     else {
-                        for (c = this.offset(), d = m.ownerDocument, a = m.offsetParent || d.documentElement; a && (a === d.body || a === d.documentElement) && p.css(a, "position") === "static";) a = a.parentNode;
-                        a && a !== m && a.nodeType === 1 && (b = p(a).offset(), b.top += p.css(a, "borderTopWidth", !0), b.left += p.css(a, "borderLeftWidth", !0))
+                        for (c = this.offset(), d = g.ownerDocument, a = g.offsetParent || d.documentElement; a && (a === d.body || a === d.documentElement) && p.css(a, "position") === "static";) a = a.parentNode;
+                        a && a !== g && a.nodeType === 1 && (b = p(a).offset(), b.top += p.css(a, "borderTopWidth", !0), b.left += p.css(a, "borderLeftWidth", !0))
                     }
                     return {
-                        top: c.top - b.top - p.css(m, "marginTop", !0),
-                        left: c.left - b.left - p.css(m, "marginLeft", !0)
+                        top: c.top - b.top - p.css(g, "marginTop", !0),
+                        left: c.left - b.left - p.css(g, "marginLeft", !0)
                     }
                 }
             },
             offsetParent: function() {
                 return this.map(function() {
                     for (var a = this.offsetParent; a && p.css(a, "position") === "static";) a = a.offsetParent;
                     return a || ai
                 })
             }
         }), p.each({
             scrollLeft: "pageXOffset",
             scrollTop: "pageYOffset"
         }, function(a, c) {
             var d = c === "pageYOffset";
-            p.fn[a] = function(m) {
+            p.fn[a] = function(g) {
                 return Kt(this, function(b, x, w) {
                     var T;
                     if (O(b) ? T = b : b.nodeType === 9 && (T = b.defaultView), w === void 0) return T ? T[c] : b[x];
                     T ? T.scrollTo(d ? T.pageXOffset : w, d ? w : T.pageYOffset) : b[x] = w
-                }, a, m, arguments.length)
+                }, a, g, arguments.length)
             }
         }), p.each(["top", "left"], function(a, c) {
-            p.cssHooks[c] = sn(v.pixelPosition, function(d, m) {
-                if (m) return m = zt(d, c), Y.test(m) ? p(d).position()[c] + "px" : m
+            p.cssHooks[c] = sn(v.pixelPosition, function(d, g) {
+                if (g) return g = zt(d, c), Y.test(g) ? p(d).position()[c] + "px" : g
             })
         }), p.each({
             Height: "height",
             Width: "width"
         }, function(a, c) {
             p.each({
                 padding: "inner" + a,
                 content: c,
                 "": "outer" + a
-            }, function(d, m) {
-                p.fn[m] = function(b, x) {
+            }, function(d, g) {
+                p.fn[g] = function(b, x) {
                     var w = arguments.length && (d || typeof b != "boolean"),
                         T = d || (b === !0 || x === !0 ? "margin" : "border");
                     return Kt(this, function(C, E, I) {
                         var _;
-                        return O(C) ? m.indexOf("outer") === 0 ? C["inner" + a] : C.document.documentElement["client" + a] : C.nodeType === 9 ? (_ = C.documentElement, Math.max(C.body["scroll" + a], _["scroll" + a], C.body["offset" + a], _["offset" + a], _["client" + a])) : I === void 0 ? p.css(C, E, T) : p.style(C, E, I, T)
+                        return O(C) ? g.indexOf("outer") === 0 ? C["inner" + a] : C.document.documentElement["client" + a] : C.nodeType === 9 ? (_ = C.documentElement, Math.max(C.body["scroll" + a], _["scroll" + a], C.body["offset" + a], _["offset" + a], _["client" + a])) : I === void 0 ? p.css(C, E, T) : p.style(C, E, I, T)
                     }, c, w ? b : void 0, w)
                 }
             })
         }), p.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], function(a, c) {
             p.fn[c] = function(d) {
                 return this.on(c, d)
             }
         }), p.fn.extend({
             bind: function(a, c, d) {
                 return this.on(a, null, c, d)
             },
             unbind: function(a, c) {
                 return this.off(a, null, c)
             },
-            delegate: function(a, c, d, m) {
-                return this.on(c, a, d, m)
+            delegate: function(a, c, d, g) {
+                return this.on(c, a, d, g)
             },
             undelegate: function(a, c, d) {
                 return arguments.length === 1 ? this.off(a, "**") : this.off(c, a || "**", d)
             },
             hover: function(a, c) {
                 return this.on("mouseenter", a).on("mouseleave", c || a)
             }
         }), p.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(a, c) {
-            p.fn[c] = function(d, m) {
-                return arguments.length > 0 ? this.on(c, null, d, m) : this.trigger(c)
+            p.fn[c] = function(d, g) {
+                return arguments.length > 0 ? this.on(c, null, d, g) : this.trigger(c)
             }
         });
         var _m = /^[\s\uFEFF\xA0]+|([^\s\uFEFF\xA0])[\s\uFEFF\xA0]+$/g;
         p.proxy = function(a, c) {
-            var d, m, b;
-            if (typeof c == "string" && (d = a[c], c = a, a = d), !!A(a)) return m = s.call(arguments, 2), b = function() {
-                return a.apply(c || this, m.concat(s.call(arguments)))
+            var d, g, b;
+            if (typeof c == "string" && (d = a[c], c = a, a = d), !!A(a)) return g = s.call(arguments, 2), b = function() {
+                return a.apply(c || this, g.concat(s.call(arguments)))
             }, b.guid = a.guid = a.guid || p.guid++, b
         }, p.holdReady = function(a) {
             a ? p.readyWait++ : p.ready(!0)
         }, p.isArray = Array.isArray, p.parseJSON = JSON.parse, p.nodeName = J, p.isFunction = A, p.isWindow = O, p.camelCase = ht, p.type = j, p.now = Date.now, p.isNumeric = function(a) {
             var c = p.type(a);
             return (c === "number" || c === "string") && !isNaN(a - parseFloat(a))
         }, p.trim = function(a) {
@@ -3527,25 +3527,25 @@
             s = r << 1,
             o = r >> 1,
             l = [],
             h = 0,
             f = -1,
             u = [];
 
-        function g(k) {
+        function m(k) {
             let v;
             if (k.lines > s && k instanceof Ri)
-                for (let A of k.children) g(A);
+                for (let A of k.children) m(A);
             else k.lines > o && (h > o || !h) ? (y(), l.push(k)) : k instanceof Xe && h && (v = u[u.length - 1]) instanceof Xe && k.lines + v.lines <= 32 ? (h += k.lines, f += k.length + 1, u[u.length - 1] = new Xe(v.text.concat(k.text), v.length + 1 + k.length)) : (h + k.lines > r && y(), h += k.lines, f += k.length + 1, u.push(k))
         }
 
         function y() {
             h != 0 && (l.push(u.length == 1 ? u[0] : Ri.from(u, f)), f = -1, h = u.length = 0)
         }
-        for (let k of e) g(k);
+        for (let k of e) m(k);
         return y(), l.length == 1 ? l[0] : new Ri(l, t)
     }
 }
 De.empty = new Xe([""], 0);
 
 function o0(n) {
     let e = -1;
@@ -3863,16 +3863,16 @@
             s = new cs(this);
         e: for (let o = 0, l = 0;;) {
             let h = o == e.length ? 1e9 : e[o++];
             for (; l < h || l == h && s.len == 0;) {
                 if (s.done) break e;
                 let u = Math.min(s.len, h - l);
                 vt(r, u, -1);
-                let g = s.ins == -1 ? -1 : s.off == 0 ? s.ins : 0;
-                vt(t, u, g), g > 0 && un(i, t, s.text), s.forward(u), l += u
+                let m = s.ins == -1 ? -1 : s.off == 0 ? s.ins : 0;
+                vt(t, u, m), m > 0 && un(i, t, s.text), s.forward(u), l += u
             }
             let f = e[o++];
             for (; l < f;) {
                 if (s.done) break e;
                 let u = Math.min(s.len, f - l);
                 vt(t, u, -1), vt(r, u, s.ins == -1 ? -1 : s.off == 0 ? s.ins : 0), s.forward(u), l += u
             }
@@ -3896,35 +3896,35 @@
             s = [],
             o = 0,
             l = null;
 
         function h(u = !1) {
             if (!u && !r.length) return;
             o < t && vt(r, t - o, -1);
-            let g = new it(r, s);
-            l = l ? l.compose(g.map(l)) : g, r = [], s = [], o = 0
+            let m = new it(r, s);
+            l = l ? l.compose(m.map(l)) : m, r = [], s = [], o = 0
         }
 
         function f(u) {
             if (Array.isArray(u))
-                for (let g of u) f(g);
+                for (let m of u) f(m);
             else if (u instanceof it) {
                 if (u.length != t) throw new RangeError(`Mismatched change set length (got ${u.length}, expected ${t})`);
                 h(), l = l ? l.compose(u.map(l)) : u
             } else {
                 let {
-                    from: g,
-                    to: y = g,
+                    from: m,
+                    to: y = m,
                     insert: k
                 } = u;
-                if (g > y || g < 0 || y > t) throw new RangeError(`Invalid change range ${g} to ${y} (in doc of length ${t})`);
+                if (m > y || m < 0 || y > t) throw new RangeError(`Invalid change range ${m} to ${y} (in doc of length ${t})`);
                 let v = k ? typeof k == "string" ? De.of(k.split(i || Ra)) : k : De.empty,
                     A = v.length;
-                if (g == y && A == 0) return;
-                g < o && h(), g > o && vt(r, g - o, -1), vt(r, y - g, A), un(s, r, v), o = y
+                if (m == y && A == 0) return;
+                m < o && h(), m > o && vt(r, m - o, -1), vt(r, y - m, A), un(s, r, v), o = y
             }
         }
         return f(e), h(!l), l
     }
     static empty(e) {
         return new it(e ? [e, -1] : [], [])
     }
@@ -3972,17 +3972,17 @@
     for (let r = 0, s = 0, o = 0; o < n.sections.length;) {
         let l = n.sections[o++],
             h = n.sections[o++];
         if (h < 0) r += l, s += l;
         else {
             let f = r,
                 u = s,
-                g = De.empty;
-            for (; f += l, u += h, h && i && (g = g.append(i[o - 2 >> 1])), !(t || o == n.sections.length || n.sections[o + 1] < 0);) l = n.sections[o++], h = n.sections[o++];
-            e(r, f, s, u, g), r = f, s = u
+                m = De.empty;
+            for (; f += l, u += h, h && i && (m = m.append(i[o - 2 >> 1])), !(t || o == n.sections.length || n.sections[o + 1] < 0);) l = n.sections[o++], h = n.sections[o++];
+            e(r, f, s, u, m), r = f, s = u
         }
     }
 }
 
 function Pa(n, e, t, i = !1) {
     let r = [],
         s = i ? [] : null,
@@ -4000,16 +4000,16 @@
         }
         l.next()
     } else if (o.ins >= 0) {
         let f = 0,
             u = o.len;
         for (; u;)
             if (l.ins == -1) {
-                let g = Math.min(u, l.len);
-                f += g, u -= g, l.forward(g)
+                let m = Math.min(u, l.len);
+                f += m, u -= m, l.forward(m)
             } else if (l.ins == 0 && l.len < u) u -= l.len, l.next();
         else break;
         vt(r, f, h < o.i ? o.ins : 0), s && h < o.i && un(s, r, o.text), h = o.i, o.forward(o.len - u)
     } else {
         if (o.done && l.done) return s ? it.createSet(r, s) : _i.create(r);
         throw new Error("Mismatched change set lengths")
     }
@@ -4238,33 +4238,33 @@
             r = this.facet.compareInput,
             s = this.id,
             o = e[s] >> 1,
             l = this.type == 2,
             h = !1,
             f = !1,
             u = [];
-        for (let g of this.dependencies) g == "doc" ? h = !0 : g == "selection" ? f = !0 : ((t = e[g.id]) !== null && t !== void 0 ? t : 1) & 1 || u.push(e[g.id]);
+        for (let m of this.dependencies) m == "doc" ? h = !0 : m == "selection" ? f = !0 : ((t = e[m.id]) !== null && t !== void 0 ? t : 1) & 1 || u.push(e[m.id]);
         return {
-            create(g) {
-                return g.values[o] = i(g), 1
+            create(m) {
+                return m.values[o] = i(m), 1
             },
-            update(g, y) {
-                if (h && y.docChanged || f && (y.docChanged || y.selection) || Na(g, u)) {
-                    let k = i(g);
-                    if (l ? !Fc(k, g.values[o], r) : !r(k, g.values[o])) return g.values[o] = k, 1
+            update(m, y) {
+                if (h && y.docChanged || f && (y.docChanged || y.selection) || Na(m, u)) {
+                    let k = i(m);
+                    if (l ? !Fc(k, m.values[o], r) : !r(k, m.values[o])) return m.values[o] = k, 1
                 }
                 return 0
             },
-            reconfigure: (g, y) => {
+            reconfigure: (m, y) => {
                 let k, v = y.config.address[s];
                 if (v != null) {
                     let A = zo(y, v);
-                    if (this.dependencies.every(O => O instanceof Z ? y.facet(O) === g.facet(O) : O instanceof yt ? y.field(O, !1) == g.field(O, !1) : !0) || (l ? Fc(k = i(g), A, r) : r(k = i(g), A))) return g.values[o] = A, 0
-                } else k = i(g);
-                return g.values[o] = k, 1
+                    if (this.dependencies.every(O => O instanceof Z ? y.facet(O) === m.facet(O) : O instanceof yt ? y.field(O, !1) == m.field(O, !1) : !0) || (l ? Fc(k = i(m), A, r) : r(k = i(m), A))) return m.values[o] = A, 0
+                } else k = i(m);
+                return m.values[o] = k, 1
             }
         }
     }
 }
 
 function Fc(n, e, t) {
     if (n.length != e.length) return !1;
@@ -4284,18 +4284,18 @@
         r = t.map(h => h.type),
         s = i.filter(h => !(h & 1)),
         o = n[e.id] >> 1;
 
     function l(h) {
         let f = [];
         for (let u = 0; u < i.length; u++) {
-            let g = zo(h, i[u]);
+            let m = zo(h, i[u]);
             if (r[u] == 2)
-                for (let y of g) f.push(y);
-            else f.push(g)
+                for (let y of m) f.push(y);
+            else f.push(m)
         }
         return e.combine(f)
     }
     return {
         create(h) {
             for (let f of i) ss(h, f);
             return h.values[o] = l(h), 1
@@ -4303,17 +4303,17 @@
         update(h, f) {
             if (!Na(h, s)) return 0;
             let u = l(h);
             return e.compare(u, h.values[o]) ? 0 : (h.values[o] = u, 1)
         },
         reconfigure(h, f) {
             let u = Na(h, i),
-                g = f.config.facets[e.id],
+                m = f.config.facets[e.id],
                 y = f.facet(e);
-            if (g && !u && Ph(t, g)) return h.values[o] = y, 0;
+            if (m && !u && Ph(t, m)) return h.values[o] = y, 0;
             let k = l(h);
             return e.compare(k, y) ? (h.values[o] = y, 0) : (h.values[o] = k, 1)
         }
     }
 }
 const zc = Z.define({
     static: !0
@@ -4423,16 +4423,16 @@
                     h.push(i && v.compare(O, i.facet(v)) ? i.facet(v) : O)
                 }
             else {
                 for (let O of k) O.type == 0 ? (l[O.id] = h.length << 1 | 1, h.push(O.value)) : (l[O.id] = f.length << 1, f.push(D => O.dynamicSlot(D)));
                 l[v.id] = f.length << 1, f.push(O => c0(O, v, k))
             }
         }
-        let g = f.map(y => y(l));
-        return new Fo(e, o, g, l, h, s)
+        let m = f.map(y => y(l));
+        return new Fo(e, o, m, l, h, s)
     }
 }
 
 function f0(n, e, t) {
     let i = [
             [],
             [],
@@ -4742,16 +4742,16 @@
             s = [i.range],
             o = gr(i.effects);
         for (let l = 1; l < t.ranges.length; l++) {
             let h = e(t.ranges[l]),
                 f = this.changes(h.changes),
                 u = f.map(r);
             for (let y = 0; y < l; y++) s[y] = s[y].map(u);
-            let g = r.mapDesc(f, !0);
-            s.push(h.range.map(g)), r = r.compose(u), o = me.mapEffects(o, u).concat(me.mapEffects(gr(h.effects), g))
+            let m = r.mapDesc(f, !0);
+            s.push(h.range.map(m)), r = r.compose(u), o = me.mapEffects(o, u).concat(me.mapEffects(gr(h.effects), m))
         }
         return {
             changes: r,
             selection: H.create(s, t.mainIndex),
             effects: o
         }
     }
@@ -4934,20 +4934,20 @@
             r = [],
             s = [],
             o = -1,
             l = -1;
         for (let h = 0; h < this.value.length; h++) {
             let f = this.value[h],
                 u = this.from[h] + e,
-                g = this.to[h] + e,
+                m = this.to[h] + e,
                 y, k;
-            if (u == g) {
+            if (u == m) {
                 let v = t.mapPos(u, f.startSide, f.mapMode);
                 if (v == null || (y = k = v, f.startSide != f.endSide && (k = t.mapPos(u, f.endSide), k < y))) continue
-            } else if (y = t.mapPos(u, f.startSide), k = t.mapPos(g, f.endSide), y > k || y == k && f.startSide > 0 && f.endSide <= 0) continue;
+            } else if (y = t.mapPos(u, f.startSide), k = t.mapPos(m, f.endSide), y > k || y == k && f.startSide > 0 && f.endSide <= 0) continue;
             (k - y || f.endSide - f.startSide) < 0 || (o < 0 && (o = y), f.point && (l = Math.max(l, k - y)), i.push(f), r.push(y - o), s.push(k - o))
         }
         return {
             mapped: i.length ? new Nh(r, s, i, l) : null,
             pos: o
         }
     }
@@ -4983,16 +4983,16 @@
         if (i && (t = t.slice().sort(za)), this.isEmpty) return t.length ? Pe.of(t) : this;
         let l = new fd(this, null, -1).goto(0),
             h = 0,
             f = [],
             u = new xn;
         for (; l.value || h < t.length;)
             if (h < t.length && (l.from - t[h].from || l.startSide - t[h].value.startSide) >= 0) {
-                let g = t[h++];
-                u.addInner(g.from, g.to, g.value) || f.push(g)
+                let m = t[h++];
+                u.addInner(m.from, m.to, m.value) || f.push(m)
             } else l.rangeIndex == 1 && l.chunkIndex < this.chunk.length && (h == t.length || this.chunkEnd(l.chunkIndex) < t[h].from) && (!o || r > this.chunkEnd(l.chunkIndex) || s < this.chunkPos[l.chunkIndex]) && u.addChunk(this.chunkPos[l.chunkIndex], this.chunk[l.chunkIndex]) ? l.nextChunk() : ((!o || r > l.to || s < l.from || o(l.from, l.to, l.value)) && (u.addInner(l.from, l.to, l.value) || f.push(Fa.create(l.from, l.to, l.value))), l.next());
         return u.finishInner(this.nextLayer.isEmpty && !f.length ? Pe.empty : this.nextLayer.update({
             add: f,
             filter: o,
             filterFrom: r,
             filterTo: s
         }))
@@ -5006,17 +5006,17 @@
             let l = this.chunkPos[o],
                 h = this.chunk[o],
                 f = e.touchesRange(l, l + h.length);
             if (f === !1) r = Math.max(r, h.maxPoint), t.push(h), i.push(e.mapPos(l));
             else if (f === !0) {
                 let {
                     mapped: u,
-                    pos: g
+                    pos: m
                 } = h.map(l, e);
-                u && (r = Math.max(r, u.maxPoint), t.push(u), i.push(g))
+                u && (r = Math.max(r, u.maxPoint), t.push(u), i.push(m))
             }
         }
         let s = this.nextLayer.map(e);
         return t.length == 0 ? s : new Pe(i, t, s || Pe.empty, r)
     }
     between(e, t, i) {
         if (!this.isEmpty) {
@@ -5034,20 +5034,20 @@
     get isEmpty() {
         return this.nextLayer == this
     }
     static iter(e, t = 0) {
         return fs.from(e).goto(t)
     }
     static compare(e, t, i, r, s = -1) {
-        let o = e.filter(g => g.maxPoint > 0 || !g.isEmpty && g.maxPoint >= s),
-            l = t.filter(g => g.maxPoint > 0 || !g.isEmpty && g.maxPoint >= s),
+        let o = e.filter(m => m.maxPoint > 0 || !m.isEmpty && m.maxPoint >= s),
+            l = t.filter(m => m.maxPoint > 0 || !m.isEmpty && m.maxPoint >= s),
             h = $c(o, l, i),
             f = new qr(o, h, s),
             u = new qr(l, h, s);
-        i.iterGaps((g, y, k) => Wc(f, g, u, y, k, r)), i.empty && i.length == 0 && Wc(f, 0, u, 0, 0, r)
+        i.iterGaps((m, y, k) => Wc(f, m, u, y, k, r)), i.empty && i.length == 0 && Wc(f, 0, u, 0, 0, r)
     }
     static eq(e, t, i = 0, r) {
         r == null && (r = 999999999);
         let s = e.filter(u => !u.isEmpty && t.indexOf(u) < 0),
             o = t.filter(u => !u.isEmpty && e.indexOf(u) < 0);
         if (s.length != o.length) return !1;
         if (!s.length) return !0;
@@ -5064,16 +5064,16 @@
         let o = new qr(e, null, s).goto(t),
             l = t,
             h = o.openStart;
         for (;;) {
             let f = Math.min(o.to, i);
             if (o.point) {
                 let u = o.activeForPoint(o.to),
-                    g = o.pointFrom < t ? u.length + 1 : Math.min(u.length, h);
-                r.point(l, f, o.point, u, g, o.pointRank), h = Math.min(o.openEnd(f), u.length)
+                    m = o.pointFrom < t ? u.length + 1 : Math.min(u.length, h);
+                r.point(l, f, o.point, u, m, o.pointRank), h = Math.min(o.openEnd(f), u.length)
             } else f > l && (r.span(l, f, o.active, h), h = o.openEnd(f));
             if (o.to > i) return h + (o.point && o.to > i ? 1 : 0);
             l = o.to, o.next()
         }
     }
     static of (e, t = !1) {
         let i = new xn;
@@ -5308,16 +5308,16 @@
     n.goto(e), t.goto(i);
     let o = i + r,
         l = i,
         h = i - e;
     for (;;) {
         let f = n.to + h - t.to || n.endSide - t.endSide,
             u = f < 0 ? n.to + h : t.to,
-            g = Math.min(u, o);
-        if (n.point || t.point ? n.point && t.point && (n.point == t.point || n.point.eq(t.point)) && $a(n.activeForPoint(n.to), t.activeForPoint(t.to)) || s.comparePoint(l, g, n.point, t.point) : g > l && !$a(n.active, t.active) && s.compareRange(l, g, n.active, t.active), u > o) break;
+            m = Math.min(u, o);
+        if (n.point || t.point ? n.point && t.point && (n.point == t.point || n.point.eq(t.point)) && $a(n.activeForPoint(n.to), t.activeForPoint(t.to)) || s.comparePoint(l, m, n.point, t.point) : m > l && !$a(n.active, t.active) && s.compareRange(l, m, n.active, t.active), u > o) break;
         l = u, f <= 0 && n.next(), f >= 0 && t.next()
     }
 }
 
 function $a(n, e) {
     if (n.length != e.length) return !1;
     for (let t = 0; t < n.length; t++)
@@ -5369,25 +5369,25 @@
 
         function r(o) {
             return /^@/.test(o) ? [o] : o.split(/,\s*/)
         }
 
         function s(o, l, h, f) {
             let u = [],
-                g = /^@(\w+)\b/.exec(o[0]),
-                y = g && g[1] == "keyframes";
-            if (g && l == null) return h.push(o[0] + ";");
+                m = /^@(\w+)\b/.exec(o[0]),
+                y = m && m[1] == "keyframes";
+            if (m && l == null) return h.push(o[0] + ";");
             for (let k in l) {
                 let v = l[k];
                 if (/&/.test(k)) s(k.split(/,\s*/).map(A => o.map(O => A.replace(/&/, O))).reduce((A, O) => A.concat(O)), v, h);
                 else if (v && typeof v == "object") {
-                    if (!g) throw new RangeError("The value of a property (" + k + ") should be a primitive value.");
+                    if (!m) throw new RangeError("The value of a property (" + k + ") should be a primitive value.");
                     s(r(k), v, u, y)
                 } else v != null && u.push(k.replace(/_.*/, "").replace(/[A-Z]/g, A => "-" + A.toLowerCase()) + ": " + v + ";")
-            }(u.length || y) && h.push((i && !g && !f ? o.map(i) : o).join(", ") + " {" + u.join(" ") + "}")
+            }(u.length || y) && h.push((i && !m && !f ? o.map(i) : o).join(", ") + " {" + u.join(" ") + "}")
         }
         for (let o in e) s(r(o), e[o], this.rules)
     }
     getRules() {
         return this.rules.join(`
 `)
     }
@@ -5619,22 +5619,22 @@
         scaleY: i
     }
 }
 
 function E0(n, e, t, i, r, s, o, l) {
     let h = n.ownerDocument,
         f = h.defaultView || window;
-    for (let u = n, g = !1; u && !g;)
+    for (let u = n, m = !1; u && !m;)
         if (u.nodeType == 1) {
             let y, k = u == h.body,
                 v = 1,
                 A = 1;
             if (k) y = M0(f);
             else {
-                if (/^(fixed|sticky)$/.test(getComputedStyle(u).position) && (g = !0), u.scrollHeight <= u.clientHeight && u.scrollWidth <= u.clientWidth) {
+                if (/^(fixed|sticky)$/.test(getComputedStyle(u).position) && (m = !0), u.scrollHeight <= u.clientHeight && u.scrollWidth <= u.clientWidth) {
                     u = u.assignedSlot || u.parentNode;
                     continue
                 }
                 let F = u.getBoundingClientRect();
                 ({
                     scaleX: v,
                     scaleY: A
@@ -5862,22 +5862,22 @@
     }
     domBoundsAround(e, t, i = 0) {
         let r = -1,
             s = -1,
             o = -1,
             l = -1;
         for (let h = 0, f = i, u = i; h < this.children.length; h++) {
-            let g = this.children[h],
-                y = f + g.length;
-            if (f < e && y > t) return g.domBoundsAround(e, t, f);
-            if (y >= e && r == -1 && (r = h, s = f), f > t && g.dom.parentNode == this.dom) {
+            let m = this.children[h],
+                y = f + m.length;
+            if (f < e && y > t) return m.domBoundsAround(e, t, f);
+            if (y >= e && r == -1 && (r = h, s = f), f > t && m.dom.parentNode == this.dom) {
                 o = h, l = u;
                 break
             }
-            u = y, f = y + g.breakAfter
+            u = y, f = y + m.breakAfter
         }
         return {
             from: s,
             to: l < 0 ? i + this.length : l,
             startDOM: (r ? this.children[r - 1].dom.nextSibling : null) || this.dom.firstChild,
             endDOM: o < this.children.length && o >= 0 ? this.children[o].dom : null
         }
@@ -5976,19 +5976,19 @@
         }
     }
 }
 
 function yd(n, e, t, i, r, s, o, l, h) {
     let {
         children: f
-    } = n, u = f.length ? f[e] : null, g = s.length ? s[s.length - 1] : null, y = g ? g.breakAfter : o;
-    if (!(e == i && u && !o && !y && s.length < 2 && u.merge(t, r, s.length ? g : null, t == 0, l, h))) {
+    } = n, u = f.length ? f[e] : null, m = s.length ? s[s.length - 1] : null, y = m ? m.breakAfter : o;
+    if (!(e == i && u && !o && !y && s.length < 2 && u.merge(t, r, s.length ? m : null, t == 0, l, h))) {
         if (i < f.length) {
             let k = f[i];
-            k && (r < k.length || k.breakAfter && (g != null && g.breakAfter)) ? (e == i && (k = k.split(r), r = 0), !y && g && k.merge(0, r, g, !0, 0, h) ? s[s.length - 1] = k : ((r || k.children.length && !k.children[0].length) && k.merge(0, r, null, !1, 0, h), s.push(k))) : k != null && k.breakAfter && (g ? g.breakAfter = 1 : o = 1), i++
+            k && (r < k.length || k.breakAfter && (m != null && m.breakAfter)) ? (e == i && (k = k.split(r), r = 0), !y && m && k.merge(0, r, m, !0, 0, h) ? s[s.length - 1] = k : ((r || k.children.length && !k.children[0].length) && k.merge(0, r, null, !1, 0, h), s.push(k))) : k != null && k.breakAfter && (m ? m.breakAfter = 1 : o = 1), i++
         }
         for (u && (u.breakAfter = o, t > 0 && (!o && s.length && u.merge(t, u.length, s[0], !1, l, 0) ? u.breakAfter = s.shift().breakAfter : (t < u.length || u.children.length && u.children[u.children.length - 1].length == 0) && u.merge(t, u.length, null, !1, l, 0), e++)); e < i && s.length;)
             if (f[i - 1].become(s[s.length - 1])) i--, s.pop(), h = s.length ? 0 : l;
             else if (f[e].become(s[0])) e++, s.shift(), l = s.length ? 0 : h;
         else break;
         !s.length && e && i < f.length && !f[e - 1].breakAfter && f[i].merge(0, 0, f[e - 1], !1, l, h) && e--, (e < i || s.length) && n.replaceChildren(e, i, s)
     }
@@ -6000,17 +6000,17 @@
             i: l,
             off: h
         } = o.findPos(t, 1),
         {
             i: f,
             off: u
         } = o.findPos(e, -1),
-        g = e - t;
-    for (let y of i) g += y.length;
-    n.length += g, yd(n, f, u, l, h, i, 0, r, s)
+        m = e - t;
+    for (let y of i) m += y.length;
+    n.length += m, yd(n, f, u, l, h, i, 0, r, s)
 }
 let Qt = typeof navigator != "undefined" ? navigator : {
         userAgent: "",
         vendor: "",
         platform: ""
     },
     Va = typeof document != "undefined" ? document : {
@@ -6289,16 +6289,16 @@
 function Sd(n, e, t) {
     let i = null,
         r = -1,
         s = null,
         o = -1;
 
     function l(f, u) {
-        for (let g = 0, y = 0; g < f.children.length && y <= u; g++) {
-            let k = f.children[g],
+        for (let m = 0, y = 0; m < f.children.length && y <= u; m++) {
+            let k = f.children[m],
                 v = y + k.length;
             v >= u && (k.children.length ? l(k, u - y) : (!s || s.isHidden && t > 0) && (v > u || y == v && k.getSide() > 0) ? (s = k, o = u - y) : (y < u || y == v && k.getSide() < 0 && !k.isHidden) && (i = k, r = u - y)), y = v
         }
     }
     l(n, e);
     let h = (t < 0 ? i : s) || i || s;
     return h ? h.coordsAt(Math.max(0, h == i ? r : o), t) : B0(n)
@@ -6701,16 +6701,16 @@
         let l = t - e;
         if (i instanceof vn)
             if (i.block) i.startSide > 0 && !this.posCovered() && this.getLine(), this.addBlockWidget(new mn(i.widget || new ef("div"), l, i));
             else {
                 let h = dn.create(i.widget || new ef("span"), l, l ? 0 : i.startSide),
                     f = this.atCursorPos && !h.isEditable && s <= r.length && (e < t || i.startSide > 0),
                     u = !h.isEditable && (e < t || s > r.length || i.startSide <= 0),
-                    g = this.getLine();
-                this.pendingBuffer == 2 && !f && !h.isEditable && (this.pendingBuffer = 0), this.flushBuffer(r), f && (g.append(to(new vr(1), r), s), s = r.length + Math.max(0, s - r.length)), g.append(to(h, r), s), this.atCursorPos = u, this.pendingBuffer = u ? e < t || s > r.length ? 1 : 2 : 0, this.pendingBuffer && (this.bufferMarks = r.slice())
+                    m = this.getLine();
+                this.pendingBuffer == 2 && !f && !h.isEditable && (this.pendingBuffer = 0), this.flushBuffer(r), f && (m.append(to(new vr(1), r), s), s = r.length + Math.max(0, s - r.length)), m.append(to(h, r), s), this.atCursorPos = u, this.pendingBuffer = u ? e < t || s > r.length ? 1 : 2 : 0, this.pendingBuffer && (this.bufferMarks = r.slice())
             }
         else this.doc.lineAt(this.pos).from == this.pos && this.getLine().addLineDeco(i);
         l && (this.textOff + l <= this.text.length ? this.textOff += l : (this.skip += l - (this.text.length - this.textOff), this.text = "", this.textOff = 0), this.pos = t), this.openStart < 0 && (this.openStart = s)
     }
     static build(e, t, i, r, s) {
         let o = new os(e, t, i, s);
         return o.openEnd = Pe.spans(r, t, i, o), o.openStart < 0 && (o.openStart = o.openEnd), o.finish(o.openEnd), o
@@ -6845,16 +6845,16 @@
     if (!i.length) return i;
     let r = i.map(o => o instanceof Function ? o(n) : o),
         s = [];
     return Pe.spans(r, e, t, {
         point() {},
         span(o, l, h, f) {
             let u = s;
-            for (let g = h.length - 1; g >= 0; g--, f--) {
-                let y = h[g].spec.bidiIsolate,
+            for (let m = h.length - 1; m >= 0; m--, f--) {
+                let y = h[m].spec.bidiIsolate,
                     k;
                 if (y != null)
                     if (f > 0 && u.length && (k = u[u.length - 1]).to == o && k.direction == y) k.to = l, u = k.inner;
                     else {
                         let v = {
                             from: o,
                             to: l,
@@ -6909,17 +6909,17 @@
         if (t.length == 0) return e;
         let i = [];
         for (let r = 0, s = 0, o = 0, l = 0;; r++) {
             let h = r == e.length ? null : e[r],
                 f = o - l,
                 u = h ? h.fromB : 1e9;
             for (; s < t.length && t[s] < u;) {
-                let g = t[s],
+                let m = t[s],
                     y = t[s + 1],
-                    k = Math.max(l, g),
+                    k = Math.max(l, m),
                     v = Math.min(u, y);
                 if (k <= v && new ri(k + f, v + f, k, v).addToSet(i), y > u) break;
                 s += 2
             }
             if (!h) return i;
             new ri(h.fromA, h.toA, h.fromB, h.toB).addToSet(i), o = h.toA, l = h.toB
         }
@@ -7018,53 +7018,53 @@
 const He = [];
 
 function j0(n, e, t, i, r) {
     for (let s = 0; s <= i.length; s++) {
         let o = s ? i[s - 1].to : e,
             l = s < i.length ? i[s].from : t,
             h = s ? 256 : r;
-        for (let f = o, u = h, g = h; f < l; f++) {
+        for (let f = o, u = h, m = h; f < l; f++) {
             let y = W0(n.charCodeAt(f));
-            y == 512 ? y = u : y == 8 && g == 4 && (y = 16), He[f] = y == 4 ? 2 : y, y & 7 && (g = y), u = y
+            y == 512 ? y = u : y == 8 && m == 4 && (y = 16), He[f] = y == 4 ? 2 : y, y & 7 && (m = y), u = y
         }
-        for (let f = o, u = h, g = h; f < l; f++) {
+        for (let f = o, u = h, m = h; f < l; f++) {
             let y = He[f];
             if (y == 128) f < l - 1 && u == He[f + 1] && u & 24 ? y = He[f] = u : He[f] = 256;
             else if (y == 64) {
                 let k = f + 1;
                 for (; k < l && He[k] == 64;) k++;
-                let v = f && u == 8 || k < t && He[k] == 8 ? g == 1 ? 1 : 8 : 256;
+                let v = f && u == 8 || k < t && He[k] == 8 ? m == 1 ? 1 : 8 : 256;
                 for (let A = f; A < k; A++) He[A] = v;
                 f = k - 1
-            } else y == 8 && g == 1 && (He[f] = 1);
-            u = y, y & 7 && (g = y)
+            } else y == 8 && m == 1 && (He[f] = 1);
+            u = y, y & 7 && (m = y)
         }
     }
 }
 
 function V0(n, e, t, i, r) {
     let s = r == 1 ? 2 : 1;
     for (let o = 0, l = 0, h = 0; o <= i.length; o++) {
         let f = o ? i[o - 1].to : e,
             u = o < i.length ? i[o].from : t;
-        for (let g = f, y, k, v; g < u; g++)
-            if (k = Ja[y = n.charCodeAt(g)])
+        for (let m = f, y, k, v; m < u; m++)
+            if (k = Ja[y = n.charCodeAt(m)])
                 if (k < 0) {
                     for (let A = l - 3; A >= 0; A -= 3)
                         if (Ti[A + 1] == -k) {
                             let O = Ti[A + 2],
                                 D = O & 2 ? r : O & 4 ? O & 1 ? s : r : 0;
-                            D && (He[g] = He[Ti[A]] = D), l = A;
+                            D && (He[m] = He[Ti[A]] = D), l = A;
                             break
                         }
                 } else {
                     if (Ti.length == 189) break;
-                    Ti[l++] = g, Ti[l++] = y, Ti[l++] = h
+                    Ti[l++] = m, Ti[l++] = y, Ti[l++] = h
                 }
-        else if ((v = He[g]) == 2 || v == 1) {
+        else if ((v = He[m]) == 2 || v == 1) {
             let A = v == r;
             h = A ? 0 : 1;
             for (let O = l - 3; O >= 0; O -= 3) {
                 let D = Ti[O + 2];
                 if (D & 2) break;
                 if (A) Ti[O + 2] |= 2;
                 else {
@@ -7086,40 +7086,40 @@
                 let u = h + 1;
                 for (;;)
                     if (u == l) {
                         if (r == t.length) break;
                         u = t[r++].to, l = r < t.length ? t[r].from : e
                     } else if (He[u] == 256) u++;
                 else break;
-                let g = s == 1,
+                let m = s == 1,
                     y = (u < e ? He[u] : i) == 1,
-                    k = g == y ? g ? 1 : 2 : i;
+                    k = m == y ? m ? 1 : 2 : i;
                 for (let v = u, A = r, O = A ? t[A - 1].to : n; v > h;) v == O && (v = t[--A].from, O = A ? t[A - 1].to : n), He[--v] = k;
                 h = u
             } else s = f, h++
         }
     }
 }
 
 function Za(n, e, t, i, r, s, o) {
     let l = i % 2 ? 2 : 1;
     if (i % 2 == r % 2)
         for (let h = e, f = 0; h < t;) {
             let u = !0,
-                g = !1;
+                m = !1;
             if (f == s.length || h < s[f].from) {
                 let A = He[h];
-                A != l && (u = !1, g = A == 16)
+                A != l && (u = !1, m = A == 16)
             }
             let y = !u && l == 1 ? [] : null,
                 k = u ? i : i + 1,
                 v = h;
             e: for (;;)
                 if (f < s.length && v == s[f].from) {
-                    if (g) break e;
+                    if (m) break e;
                     let A = s[f];
                     if (!u)
                         for (let O = A.to, D = f + 1;;) {
                             if (O == t) break e;
                             if (D < s.length && s[D].from == O) O = s[D++].to;
                             else {
                                 if (He[O] == l) break e;
@@ -7136,25 +7136,25 @@
                 } else {
                     if (v == t || (u ? He[v] != l : He[v] == l)) break;
                     v++
                 } y ? Za(n, h, v, i + 1, r, y, o) : h < v && o.push(new pn(h, v, k)), h = v
         } else
             for (let h = t, f = s.length; h > e;) {
                 let u = !0,
-                    g = !1;
+                    m = !1;
                 if (!f || h > s[f - 1].to) {
                     let A = He[h - 1];
-                    A != l && (u = !1, g = A == 16)
+                    A != l && (u = !1, m = A == 16)
                 }
                 let y = !u && l == 1 ? [] : null,
                     k = u ? i : i + 1,
                     v = h;
                 e: for (;;)
                     if (f && v == s[f - 1].to) {
-                        if (g) break e;
+                        if (m) break e;
                         let A = s[--f];
                         if (!u)
                             for (let O = A.from, D = f;;) {
                                 if (O == e) break e;
                                 if (D && s[D - 1].to == O) O = s[--D].from;
                                 else {
                                     if (He[O - 1] == l) break e;
@@ -7209,16 +7209,16 @@
     }
     l < 0 && (l = pn.find(e, o, (s = i.bidiLevel) !== null && s !== void 0 ? s : -1, i.assoc));
     let h = e[l];
     o == h.side(r, t) && (h = e[l += r ? 1 : -1], o = h.side(!r, t));
     let f = r == (h.dir == t),
         u = mt(n.text, o, f);
     if ($d = n.text.slice(Math.min(o, u), Math.max(o, u)), u > h.from && u < h.to) return H.cursor(u + n.from, f ? -1 : 1, h.level);
-    let g = l == (r ? e.length - 1 : 0) ? null : e[l + (r ? 1 : -1)];
-    return !g && h.level != t ? H.cursor(r ? n.to : n.from, r ? -1 : 1, t) : g && g.level < h.level ? H.cursor(g.side(!r, t) + n.from, r ? 1 : -1, g.level) : H.cursor(u + n.from, r ? -1 : 1, h.level)
+    let m = l == (r ? e.length - 1 : 0) ? null : e[l + (r ? 1 : -1)];
+    return !m && h.level != t ? H.cursor(r ? n.to : n.from, r ? -1 : 1, t) : m && m.level < h.level ? H.cursor(m.side(!r, t) + n.from, r ? 1 : -1, m.level) : H.cursor(u + n.from, r ? -1 : 1, h.level)
 }
 class nf extends je {
     get length() {
         return this.view.state.doc.length
     }
     constructor(e) {
         super(), this.view = e, this.decorations = [], this.dynamicDecorationMap = [], this.domChanged = null, this.hasComposition = null, this.markedForComposition = new Set, this.minWidth = 0, this.minWidthFrom = 0, this.minWidthTo = 0, this.impreciseAnchor = null, this.impreciseHead = null, this.forceSelection = !1, this.lastUpdate = Date.now(), this.setDOM(e.contentDOM), this.children = [new tt], this.children[0].setParent(this), this.updateDeco(), this.updateInner([new ri(0, 0, 0, e.state.doc.length)], 0, null)
@@ -7274,28 +7274,28 @@
         for (let o = r.length - 1;; o--) {
             let l = o >= 0 ? r[o] : null;
             if (!l) break;
             let {
                 fromA: h,
                 toA: f,
                 fromB: u,
-                toB: g
+                toB: m
             } = l, y, k, v, A;
-            if (i && i.range.fromB < g && i.range.toB > u) {
+            if (i && i.range.fromB < m && i.range.toB > u) {
                 let j = os.build(this.view.state.doc, u, i.range.fromB, this.decorations, this.dynamicDecorationMap),
-                    z = os.build(this.view.state.doc, i.range.toB, g, this.decorations, this.dynamicDecorationMap);
+                    z = os.build(this.view.state.doc, i.range.toB, m, this.decorations, this.dynamicDecorationMap);
                 k = j.breakAtStart, v = j.openStart, A = z.openEnd;
                 let G = this.compositionView(i);
                 z.breakAtStart ? G.breakAfter = 1 : z.content.length && G.merge(G.length, G.length, z.content[0], !1, z.openStart, 0) && (G.breakAfter = z.content[0].breakAfter, z.content.shift()), j.content.length && G.merge(0, 0, j.content[j.content.length - 1], !0, 0, j.openEnd) && j.content.pop(), y = j.content.concat(G).concat(z.content)
             } else({
                 content: y,
                 breakAtStart: k,
                 openStart: v,
                 openEnd: A
-            } = os.build(this.view.state.doc, u, g, this.decorations, this.dynamicDecorationMap));
+            } = os.build(this.view.state.doc, u, m, this.decorations, this.dynamicDecorationMap));
             let {
                 i: O,
                 off: D
             } = s.findPos(f, 1), {
                 i: F,
                 off: $
             } = s.findPos(h, -1);
@@ -7332,41 +7332,41 @@
         if (!(r || t || s)) return;
         let o = this.forceSelection;
         this.forceSelection = !1;
         let l = this.view.state.selection.main,
             h = this.moveToLine(this.domAtPos(l.anchor)),
             f = l.empty ? h : this.moveToLine(this.domAtPos(l.head));
         if (ee.gecko && l.empty && !this.hasComposition && K0(h)) {
-            let g = document.createTextNode("");
-            this.view.observer.ignore(() => h.node.insertBefore(g, h.node.childNodes[h.offset] || null)), h = f = new St(g, 0), o = !0
+            let m = document.createTextNode("");
+            this.view.observer.ignore(() => h.node.insertBefore(m, h.node.childNodes[h.offset] || null)), h = f = new St(m, 0), o = !0
         }
         let u = this.view.observer.selectionRange;
         (o || !u.focusNode || !Wo(h.node, h.offset, u.anchorNode, u.anchorOffset) || !Wo(f.node, f.offset, u.focusNode, u.focusOffset)) && (this.view.observer.ignore(() => {
             ee.android && ee.chrome && this.dom.contains(u.focusNode) && ey(u.focusNode, this.dom) && (this.dom.blur(), this.dom.focus({
                 preventScroll: !0
             }));
-            let g = $o(this.view.root);
-            if (g)
+            let m = $o(this.view.root);
+            if (m)
                 if (l.empty) {
                     if (ee.gecko) {
                         let y = Y0(h.node, h.offset);
                         if (y && y != 3) {
                             let k = qd(h.node, h.offset, y == 1 ? 1 : -1);
                             k && (h = new St(k.node, k.offset))
                         }
                     }
-                    g.collapse(h.node, h.offset), l.bidiLevel != null && g.caretBidiLevel !== void 0 && (g.caretBidiLevel = l.bidiLevel)
-                } else if (g.extend) {
-                g.collapse(h.node, h.offset);
+                    m.collapse(h.node, h.offset), l.bidiLevel != null && m.caretBidiLevel !== void 0 && (m.caretBidiLevel = l.bidiLevel)
+                } else if (m.extend) {
+                m.collapse(h.node, h.offset);
                 try {
-                    g.extend(f.node, f.offset)
+                    m.extend(f.node, f.offset)
                 } catch (y) {}
             } else {
                 let y = document.createRange();
-                l.anchor > l.head && ([h, f] = [f, h]), y.setEnd(f.node, f.offset), y.setStart(h.node, h.offset), g.removeAllRanges(), g.addRange(y)
+                l.anchor > l.head && ([h, f] = [f, h]), y.setEnd(f.node, f.offset), y.setStart(h.node, h.offset), m.removeAllRanges(), m.addRange(y)
             }
             s && this.view.root.activeElement == this.dom && (this.dom.blur(), i && i.focus())
         }), this.view.observer.setSelectionRange(h, f)), this.impreciseAnchor = h.precise ? null : new St(u.anchorNode, u.anchorOffset), this.impreciseHead = f.precise ? null : new St(u.focusNode, u.focusOffset)
     }
     enforceCursorAssoc() {
         if (this.hasComposition) return;
         let {
@@ -7381,16 +7381,16 @@
         let l = o.posAtStart;
         if (t.head == l || t.head == l + o.length) return;
         let h = this.coordsAt(t.head, -1),
             f = this.coordsAt(t.head, 1);
         if (!h || !f || h.bottom > f.top) return;
         let u = this.domAtPos(t.head + t.assoc);
         i.collapse(u.node, u.offset), i.modify("move", t.assoc < 0 ? "forward" : "backward", "lineboundary"), e.observer.readSelectionRange();
-        let g = e.observer.selectionRange;
-        e.docView.posFromDOM(g.anchorNode, g.anchorOffset) != t.from && i.collapse(r, s)
+        let m = e.observer.selectionRange;
+        e.docView.posFromDOM(m.anchorNode, m.anchorOffset) != t.from && i.collapse(r, s)
     }
     moveToLine(e) {
         let t = this.dom,
             i;
         if (e.node != t) return e;
         for (let r = e.offset; !i && r < t.childNodes.length; r++) {
             let s = je.get(t.childNodes[r]);
@@ -7473,30 +7473,30 @@
                 to: r
             } = e,
             s = this.view.contentDOM.clientWidth,
             o = s > Math.max(this.view.scrollDOM.clientWidth, this.minWidth) + 1,
             l = -1,
             h = this.view.textDirection == Ue.LTR;
         for (let f = 0, u = 0; u < this.children.length; u++) {
-            let g = this.children[u],
-                y = f + g.length;
+            let m = this.children[u],
+                y = f + m.length;
             if (y > r) break;
             if (f >= i) {
-                let k = g.dom.getBoundingClientRect();
+                let k = m.dom.getBoundingClientRect();
                 if (t.push(k.height), o) {
-                    let v = g.dom.lastChild,
+                    let v = m.dom.lastChild,
                         A = v ? ds(v) : [];
                     if (A.length) {
                         let O = A[A.length - 1],
                             D = h ? O.right - k.left : k.right - O.left;
                         D > l && (l = D, this.minWidth = s, this.minWidthFrom = f, this.minWidthTo = y)
                     }
                 }
             }
-            f = y + g.breakAfter
+            f = y + m.breakAfter
         }
         return t
     }
     textDirectionAt(e) {
         let {
             i: t
         } = this.childPos(e, 1);
@@ -7621,33 +7621,33 @@
         from: s,
         to: o
     } = i, l = r.nodeValue;
     if (/[\n\r]/.test(l) || n.state.doc.sliceString(i.from, i.to) != l) return null;
     let h = e.invertedDesc,
         f = new ri(h.mapPos(s), h.mapPos(o), s, o),
         u = [];
-    for (let g = r.parentNode;; g = g.parentNode) {
-        let y = je.get(g);
+    for (let m = r.parentNode;; m = m.parentNode) {
+        let y = je.get(m);
         if (y instanceof Gi) u.push({
-            node: g,
+            node: m,
             deco: y.mark
         });
         else {
-            if (y instanceof tt || g.nodeName == "DIV" && g.parentNode == n.contentDOM) return {
+            if (y instanceof tt || m.nodeName == "DIV" && m.parentNode == n.contentDOM) return {
                 range: f,
                 text: r,
                 marks: u,
-                line: g
+                line: m
             };
-            if (g != n.contentDOM) u.push({
-                node: g,
+            if (m != n.contentDOM) u.push({
+                node: m,
                 deco: new Ms({
                     inclusive: !0,
-                    attributes: _0(g),
-                    tagName: g.tagName.toLowerCase()
+                    attributes: _0(m),
+                    tagName: m.tagName.toLowerCase()
                 })
             });
             else return null
         }
     }
 }
 
@@ -7757,32 +7757,32 @@
         right: n.right,
         bottom: e
     } : n
 }
 
 function th(n, e, t) {
     let i, r, s, o, l = !1,
-        h, f, u, g;
+        h, f, u, m;
     for (let v = n.firstChild; v; v = v.nextSibling) {
         let A = ds(v);
         for (let O = 0; O < A.length; O++) {
             let D = A[O];
             r && na(r, D) && (D = sf(of(D, r.bottom), r.top));
             let F = ny(e, D),
                 $ = ry(t, D);
             if (F == 0 && $ == 0) return v.nodeType == 3 ? lf(v, e, t) : th(v, e, t);
             if (!i || o > $ || o == $ && s > F) {
                 i = v, r = D, s = F, o = $;
                 let j = $ ? t < D.top ? -1 : 1 : F ? e < D.left ? -1 : 1 : 0;
                 l = !j || (j > 0 ? O < A.length - 1 : O > 0)
             }
-            F == 0 ? t > D.bottom && (!u || u.bottom < D.bottom) ? (h = v, u = D) : t < D.top && (!g || g.top > D.top) && (f = v, g = D) : u && na(u, D) ? u = of(u, D.bottom) : g && na(g, D) && (g = sf(g, D.top))
+            F == 0 ? t > D.bottom && (!u || u.bottom < D.bottom) ? (h = v, u = D) : t < D.top && (!m || m.top > D.top) && (f = v, m = D) : u && na(u, D) ? u = of(u, D.bottom) : m && na(m, D) && (m = sf(m, D.top))
         }
     }
-    if (u && u.bottom >= t ? (i = h, r = u) : g && g.top <= t && (i = f, r = g), !i) return {
+    if (u && u.bottom >= t ? (i = h, r = u) : m && m.top <= t && (i = f, r = m), !i) return {
         node: n,
         offset: 0
     };
     let y = Math.max(r.left, Math.min(r.right, e));
     if (i.nodeType == 3) return lf(i, y, t);
     if (l && i.contentEditable != "false") return th(i, y, t);
     let k = Array.prototype.indexOf.call(n.childNodes, i) + (e >= (r.left + r.right) / 2 ? 1 : 0);
@@ -7799,23 +7799,23 @@
         o = 0;
     for (let l = 0; l < i; l++) {
         let h = Un(n, l, l + 1).getClientRects();
         for (let f = 0; f < h.length; f++) {
             let u = h[f];
             if (u.top == u.bottom) continue;
             o || (o = e - u.left);
-            let g = (u.top > t ? u.top - t : t - u.bottom) - 1;
-            if (u.left - 1 <= e && u.right + 1 >= e && g < s) {
+            let m = (u.top > t ? u.top - t : t - u.bottom) - 1;
+            if (u.left - 1 <= e && u.right + 1 >= e && m < s) {
                 let y = e >= (u.left + u.right) / 2,
                     k = y;
-                if ((ee.chrome || ee.gecko) && Un(n, l).getBoundingClientRect().left == u.right && (k = !y), g <= 0) return {
+                if ((ee.chrome || ee.gecko) && Un(n, l).getBoundingClientRect().left == u.right && (k = !y), m <= 0) return {
                     node: n,
                     offset: l + (k ? 1 : 0)
                 };
-                r = l + (k ? 1 : 0), s = g
+                r = l + (k ? 1 : 0), s = m
             }
         }
     }
     return {
         node: n,
         offset: r > -1 ? r : o > 0 ? n.nodeValue.length : 0
     }
@@ -7826,55 +7826,55 @@
     let o = n.contentDOM.getBoundingClientRect(),
         l = o.top + n.viewState.paddingTop,
         h, {
             docHeight: f
         } = n.viewState,
         {
             x: u,
-            y: g
+            y: m
         } = e,
-        y = g - l;
+        y = m - l;
     if (y < 0) return 0;
     if (y > f) return n.state.doc.length;
     for (let j = n.viewState.heightOracle.textHeight / 2, z = !1; h = n.elementAtHeight(y), h.type != Dt.Text;)
         for (; y = i > 0 ? h.bottom + j : h.top - j, !(y >= 0 && y <= f);) {
             if (z) return t ? null : 0;
             z = !0, i = -i
         }
-    g = l + y;
+    m = l + y;
     let k = h.from;
-    if (k < n.viewport.from) return n.viewport.from == 0 ? 0 : t ? null : af(n, o, h, u, g);
-    if (k > n.viewport.to) return n.viewport.to == n.state.doc.length ? n.state.doc.length : t ? null : af(n, o, h, u, g);
+    if (k < n.viewport.from) return n.viewport.from == 0 ? 0 : t ? null : af(n, o, h, u, m);
+    if (k > n.viewport.to) return n.viewport.to == n.state.doc.length ? n.state.doc.length : t ? null : af(n, o, h, u, m);
     let v = n.dom.ownerDocument,
         A = n.root.elementFromPoint ? n.root : v,
-        O = A.elementFromPoint(u, g);
-    O && !n.contentDOM.contains(O) && (O = null), O || (u = Math.max(o.left + 1, Math.min(o.right - 1, u)), O = A.elementFromPoint(u, g), O && !n.contentDOM.contains(O) && (O = null));
+        O = A.elementFromPoint(u, m);
+    O && !n.contentDOM.contains(O) && (O = null), O || (u = Math.max(o.left + 1, Math.min(o.right - 1, u)), O = A.elementFromPoint(u, m), O && !n.contentDOM.contains(O) && (O = null));
     let D, F = -1;
     if (O && ((r = n.docView.nearest(O)) === null || r === void 0 ? void 0 : r.isEditable) != !1) {
         if (v.caretPositionFromPoint) {
-            let j = v.caretPositionFromPoint(u, g);
+            let j = v.caretPositionFromPoint(u, m);
             j && ({
                 offsetNode: D,
                 offset: F
             } = j)
         } else if (v.caretRangeFromPoint) {
-            let j = v.caretRangeFromPoint(u, g);
+            let j = v.caretRangeFromPoint(u, m);
             j && ({
                 startContainer: D,
                 startOffset: F
             } = j, (!n.contentDOM.contains(D) || ee.safari && sy(D, F, u) || ee.chrome && oy(D, F, u)) && (D = void 0))
         }
     }
     if (!D || !n.docView.dom.contains(D)) {
         let j = tt.find(n.docView, k);
         if (!j) return y > h.top + h.height / 2 ? h.to : h.from;
         ({
             node: D,
             offset: F
-        } = th(j.dom, u, g))
+        } = th(j.dom, u, m))
     }
     let $ = n.docView.nearest(D);
     if (!$) return null;
     if ($.isWidget && ((s = $.dom) === null || s === void 0 ? void 0 : s.nodeType) == 1) {
         let j = $.dom.getBoundingClientRect();
         return e.y < j.top || e.y <= j.bottom && e.x <= (j.left + j.right) / 2 ? $.posAtStart : $.posAtEnd
     } else return $.localPosFromDOM(D, F) + $.posAtStart
@@ -7975,20 +7975,20 @@
         f = n.coordsAtPos(r, e.assoc || -1),
         u = n.documentTop;
     if (f) o == null && (o = f.left - h.left), l = s < 0 ? f.top : f.bottom;
     else {
         let k = n.viewState.lineBlockAt(r);
         o == null && (o = Math.min(h.right - h.left, n.defaultCharacterWidth * (r - k.from))), l = (s < 0 ? k.top : k.bottom) + u
     }
-    let g = h.left + o,
+    let m = h.left + o,
         y = i != null ? i : n.viewState.heightOracle.textHeight >> 1;
     for (let k = 0;; k += 10) {
         let v = l + (y + k) * s,
             A = jd(n, {
-                x: g,
+                x: m,
                 y: v
             }, !1, s);
         if (v < h.top || v > h.bottom || (s < 0 ? A < r : A > r)) {
             let O = n.docView.coordsForChar(A),
                 D = !O || v < O.top ? -1 : 1;
             return H.cursor(A, D, void 0, o)
         }
@@ -8266,21 +8266,21 @@
         let h = -1;
         i = t.changeByRange(f => {
             let u = t.doc.lineAt(f.from);
             if (u.from == h) return {
                 range: f
             };
             h = u.from;
-            let g = t.toText((o ? s.line(r++).text : e) + t.lineBreak);
+            let m = t.toText((o ? s.line(r++).text : e) + t.lineBreak);
             return {
                 changes: {
                     from: u.from,
-                    insert: g
+                    insert: m
                 },
-                range: H.cursor(f.from + g.length)
+                range: H.cursor(f.from + m.length)
             }
         })
     } else o ? i = t.changeByRange(h => {
         let f = s.line(r++);
         return {
             changes: {
                 from: h.from,
@@ -8375,17 +8375,17 @@
         update(s) {
             s.docChanged && (t.pos = s.changes.mapPos(t.pos), r = r.map(s.changes))
         },
         get(s, o, l) {
             let h = df(n, s),
                 f, u = ff(n, h.pos, h.bias, i);
             if (t.pos != h.pos && !o) {
-                let g = ff(n, t.pos, t.bias, i),
-                    y = Math.min(g.from, u.from),
-                    k = Math.max(g.to, u.to);
+                let m = ff(n, t.pos, t.bias, i),
+                    y = Math.min(m.from, u.from),
+                    k = Math.max(m.to, u.to);
                 u = y < u.from ? H.range(y, k) : H.range(k, y)
             }
             return o ? r.replaceRange(r.main.extend(u.from, u.to)) : l && i == 1 && r.ranges.length > 1 && (f = Sy(r, h.pos)) ? f : l ? r.addRange(u) : H.create([u])
         }
     }
 }
 
@@ -8685,19 +8685,19 @@
         let s = this,
             o = i.doc;
         for (let l = r.length - 1; l >= 0; l--) {
             let {
                 fromA: h,
                 toA: f,
                 fromB: u,
-                toB: g
+                toB: m
             } = r[l], y = s.lineAt(h, qe.ByPosNoHeight, i.setDoc(t), 0, 0), k = y.to >= f ? y : s.lineAt(f, qe.ByPosNoHeight, i, 0, 0);
-            for (g += k.to - f, f = k.to; l > 0 && y.from <= r[l - 1].toA;) h = r[l - 1].fromA, u = r[l - 1].fromB, l--, h < y.from && (y = s.lineAt(h, qe.ByPosNoHeight, i, 0, 0));
+            for (m += k.to - f, f = k.to; l > 0 && y.from <= r[l - 1].toA;) h = r[l - 1].fromA, u = r[l - 1].fromB, l--, h < y.from && (y = s.lineAt(h, qe.ByPosNoHeight, i, 0, 0));
             u += y.from - h, h = y.from;
-            let v = zh.build(i.setDoc(o), e, u, g);
+            let v = zh.build(i.setDoc(o), e, u, m);
             s = s.replace(h, f, v)
         }
         return s.updateHeight(i, 0)
     }
     static empty() {
         return new jt(0, 0)
     }
@@ -8792,24 +8792,24 @@
             lastLine: o,
             perLine: l,
             perChar: h
         } = this.heightMetrics(t, r);
         if (t.lineWrapping) {
             let f = r + Math.round(Math.max(0, Math.min(1, (e - i) / this.height)) * this.length),
                 u = t.doc.lineAt(f),
-                g = l + u.length * h,
-                y = Math.max(i, e - g / 2);
-            return new Li(u.from, u.length, y, g, 0)
+                m = l + u.length * h,
+                y = Math.max(i, e - m / 2);
+            return new Li(u.from, u.length, y, m, 0)
         } else {
             let f = Math.max(0, Math.min(o - s, Math.floor((e - i) / l))),
                 {
                     from: u,
-                    length: g
+                    length: m
                 } = t.doc.line(s + f);
-            return new Li(u, g, i + l * f, l, 0)
+            return new Li(u, m, i + l * f, l, 0)
         }
     }
     lineAt(e, t, i, r, s) {
         if (t == qe.ByHeight) return this.blockAt(e, i, r, s);
         if (t == qe.ByPosNoHeight) {
             let {
                 from: k,
@@ -8817,32 +8817,32 @@
             } = i.doc.lineAt(e);
             return new Li(k, v - k, 0, 0, 0)
         }
         let {
             firstLine: o,
             perLine: l,
             perChar: h
-        } = this.heightMetrics(i, s), f = i.doc.lineAt(e), u = l + f.length * h, g = f.number - o, y = r + l * g + h * (f.from - s - g);
+        } = this.heightMetrics(i, s), f = i.doc.lineAt(e), u = l + f.length * h, m = f.number - o, y = r + l * m + h * (f.from - s - m);
         return new Li(f.from, f.length, Math.max(r, Math.min(y, r + this.height - u)), u, 0)
     }
     forEachLine(e, t, i, r, s, o) {
         e = Math.max(e, s), t = Math.min(t, s + this.length);
         let {
             firstLine: l,
             perLine: h,
             perChar: f
         } = this.heightMetrics(i, s);
-        for (let u = e, g = r; u <= t;) {
+        for (let u = e, m = r; u <= t;) {
             let y = i.doc.lineAt(u);
             if (u == e) {
                 let v = y.number - l;
-                g += h * v + f * (e - s - v)
+                m += h * v + f * (e - s - v)
             }
             let k = h + f * y.length;
-            o(new Li(y.from, y.length, g, k, 0)), g += k, u = y.to + 1
+            o(new Li(y.from, y.length, m, k, 0)), m += k, u = y.to + 1
         }
     }
     replace(e, t, i) {
         let r = this.length - t;
         if (r > 0) {
             let s = i[i.length - 1];
             s instanceof dt ? i[i.length - 1] = new dt(s.length + r) : i.push(null, new dt(r - 1))
@@ -8864,17 +8864,17 @@
         if (r && r.from <= t + this.length && r.more) {
             let o = [],
                 l = Math.max(t, r.from),
                 h = -1;
             for (r.from > t && o.push(new dt(r.from - t - 1).updateHeight(e, t)); l <= s && r.more;) {
                 let u = e.doc.lineAt(l).length;
                 o.length && o.push(null);
-                let g = r.heights[r.index++];
-                h == -1 ? h = g : Math.abs(g - h) >= Lo && (h = -2);
-                let y = new jt(u, g);
+                let m = r.heights[r.index++];
+                h == -1 ? h = m : Math.abs(m - h) >= Lo && (h = -2);
+                let y = new jt(u, m);
                 y.outdated = !1, o.push(y), l += u + 1
             }
             l <= s && o.push(null, new dt(s - l).updateHeight(e, l));
             let f = Rt.of(o);
             return (h < 0 || Math.abs(f.height - this.height) >= Lo || Math.abs(h - this.heightMetrics(e, t).perLine) >= Lo) && (e.heightChanged = !0), f
         } else(i || this.outdated) && (this.setHeight(e, e.heightForGap(t, t + this.length)), this.outdated = !1);
         return this
@@ -9044,20 +9044,20 @@
         s = Math.max(0, t.left),
         o = Math.min(r.innerWidth, t.right),
         l = Math.max(0, t.top),
         h = Math.min(r.innerHeight, t.bottom);
     for (let f = n.parentNode; f && f != i.body;)
         if (f.nodeType == 1) {
             let u = f,
-                g = window.getComputedStyle(u);
-            if ((u.scrollHeight > u.clientHeight || u.scrollWidth > u.clientWidth) && g.overflow != "visible") {
+                m = window.getComputedStyle(u);
+            if ((u.scrollHeight > u.clientHeight || u.scrollWidth > u.clientWidth) && m.overflow != "visible") {
                 let y = u.getBoundingClientRect();
                 s = Math.max(s, y.left), o = Math.min(o, y.right), l = Math.max(l, y.top), h = f == n.parentNode ? y.bottom : Math.min(h, y.bottom)
             }
-            f = g.position == "absolute" || g.position == "fixed" ? u.offsetParent : u.parentNode
+            f = m.position == "absolute" || m.position == "fixed" ? u.offsetParent : u.parentNode
         } else if (f.nodeType == 11) f = f.host;
     else break;
     return {
         left: s - t.left,
         right: Math.max(s, o) - t.left,
         top: l - (t.top + e),
         bottom: Math.max(l, h) - (t.top + e)
@@ -9172,17 +9172,17 @@
         if (l.width && l.height) {
             let {
                 scaleX: j,
                 scaleY: z
             } = ud(t, l);
             (this.scaleX != j || this.scaleY != z) && (this.scaleX = j, this.scaleY = z, f |= 8, o = h = !0)
         }
-        let g = (parseInt(i.paddingTop) || 0) * this.scaleY,
+        let m = (parseInt(i.paddingTop) || 0) * this.scaleY,
             y = (parseInt(i.paddingBottom) || 0) * this.scaleY;
-        (this.paddingTop != g || this.paddingBottom != y) && (this.paddingTop = g, this.paddingBottom = y, f |= 10), this.editorWidth != e.scrollDOM.clientWidth && (r.lineWrapping && (h = !0), this.editorWidth = e.scrollDOM.clientWidth, f |= 8);
+        (this.paddingTop != m || this.paddingBottom != y) && (this.paddingTop = m, this.paddingBottom = y, f |= 10), this.editorWidth != e.scrollDOM.clientWidth && (r.lineWrapping && (h = !0), this.editorWidth = e.scrollDOM.clientWidth, f |= 8);
         let k = e.scrollDOM.scrollTop * this.scaleY;
         this.scrollTop != k && (this.scrollAnchorHeight = -1, this.scrollTop = k), this.scrolledToBottom = gd(e.scrollDOM);
         let v = (this.printing ? Ny : Py)(t, this.paddingTop),
             A = v.top - this.pixelViewport.top,
             O = v.bottom - this.pixelViewport.bottom;
         this.pixelViewport = v;
         let D = this.pixelViewport.bottom > this.pixelViewport.top && this.pixelViewport.right > this.pixelViewport.left;
@@ -9225,17 +9225,17 @@
             h = new so(r.lineAt(o - i * 1e3, qe.ByHeight, s, 0, 0).from, r.lineAt(l + (1 - i) * 1e3, qe.ByHeight, s, 0, 0).to);
         if (t) {
             let {
                 head: f
             } = t.range;
             if (f < h.from || f > h.to) {
                 let u = Math.min(this.editorHeight, this.pixelViewport.bottom - this.pixelViewport.top),
-                    g = r.lineAt(f, qe.ByPos, s, 0, 0),
+                    m = r.lineAt(f, qe.ByPos, s, 0, 0),
                     y;
-                t.y == "center" ? y = (g.top + g.bottom) / 2 - u / 2 : t.y == "start" || t.y == "nearest" && f < h.from ? y = g.top : y = g.bottom - u, h = new so(r.lineAt(y - 1e3 / 2, qe.ByHeight, s, 0, 0).from, r.lineAt(y + u + 1e3 / 2, qe.ByHeight, s, 0, 0).to)
+                t.y == "center" ? y = (m.top + m.bottom) / 2 - u / 2 : t.y == "start" || t.y == "nearest" && f < h.from ? y = m.top : y = m.bottom - u, h = new so(r.lineAt(y - 1e3 / 2, qe.ByHeight, s, 0, 0).from, r.lineAt(y + u + 1e3 / 2, qe.ByHeight, s, 0, 0).to)
             }
         }
         return h
     }
     mapViewport(e, t) {
         let i = t.mapPos(e.from, -1),
             r = t.mapPos(e.to, 1);
@@ -9265,54 +9265,54 @@
     ensureLineGaps(e, t) {
         let i = this.heightOracle.lineWrapping,
             r = i ? 1e4 : 2e3,
             s = r >> 1,
             o = r << 1;
         if (this.defaultTextDirection != Ue.LTR && !i) return [];
         let l = [],
-            h = (f, u, g, y) => {
+            h = (f, u, m, y) => {
                 if (u - f < s) return;
                 let k = this.state.selection.main,
                     v = [k.from];
                 k.empty || v.push(k.to);
                 for (let O of v)
                     if (O > f && O < u) {
-                        h(f, O - 10, g, y), h(O + 10, u, g, y);
+                        h(f, O - 10, m, y), h(O + 10, u, m, y);
                         return
-                    } let A = _y(e, O => O.from >= g.from && O.to <= g.to && Math.abs(O.from - f) < s && Math.abs(O.to - u) < s && !v.some(D => O.from < D && O.to > D));
+                    } let A = _y(e, O => O.from >= m.from && O.to <= m.to && Math.abs(O.from - f) < s && Math.abs(O.to - u) < s && !v.some(D => O.from < D && O.to > D));
                 if (!A) {
-                    if (u < g.to && t && i && t.visibleRanges.some(O => O.from <= u && O.to >= u)) {
+                    if (u < m.to && t && i && t.visibleRanges.some(O => O.from <= u && O.to >= u)) {
                         let O = t.moveToLineBoundary(H.cursor(u), !1, !0).head;
                         O > f && (u = O)
                     }
-                    A = new sa(f, u, this.gapSize(g, f, u, y))
+                    A = new sa(f, u, this.gapSize(m, f, u, y))
                 }
                 l.push(A)
             };
         for (let f of this.viewportLines) {
             if (f.length < o) continue;
             let u = By(f.from, f.to, this.stateDeco);
             if (u.total < o) continue;
-            let g = this.scrollTarget ? this.scrollTarget.range.head : null,
+            let m = this.scrollTarget ? this.scrollTarget.range.head : null,
                 y, k;
             if (i) {
                 let v = r / this.heightOracle.lineLength * this.heightOracle.lineHeight,
                     A, O;
-                if (g != null) {
-                    let D = lo(u, g),
+                if (m != null) {
+                    let D = lo(u, m),
                         F = ((this.visibleBottom - this.visibleTop) / 2 + v) / f.height;
                     A = D - F, O = D + F
                 } else A = (this.visibleTop - f.top - v) / f.height, O = (this.visibleBottom - f.top + v) / f.height;
                 y = oo(u, A), k = oo(u, O)
             } else {
                 let v = u.total * this.heightOracle.charWidth,
                     A = r * this.heightOracle.charWidth,
                     O, D;
-                if (g != null) {
-                    let F = lo(u, g),
+                if (m != null) {
+                    let F = lo(u, m),
                         $ = ((this.pixelViewport.right - this.pixelViewport.left) / 2 + A) / v;
                     O = F - $, D = F + $
                 } else O = (this.pixelViewport.left - A) / v, D = (this.pixelViewport.right + A) / v;
                 y = oo(u, O), k = oo(u, D)
             }
             y > f.from && h(f.from, y, f, u), k < f.to && h(k, f.to, f, u)
         }
@@ -9918,20 +9918,20 @@
             h = s.to > e.to ? r.sliceDoc(e.to, s.to) : "";
         i = r.replaceSelection(n.state.toText(l + e.insert.sliceString(0, void 0, n.state.lineBreak) + h))
     } else {
         let l = r.changes(e),
             h = t && t.main.to <= l.newLength ? t.main : void 0;
         if (r.selection.ranges.length > 1 && n.inputState.composing >= 0 && e.to <= s.to && e.to >= s.to - 10) {
             let f = n.state.sliceDoc(e.from, e.to),
-                u, g = t && Wd(n, t.main.head);
-            if (g) {
+                u, m = t && Wd(n, t.main.head);
+            if (m) {
                 let v = e.insert.length - (e.to - e.from);
                 u = {
-                    from: g.from,
-                    to: g.to - v
+                    from: m.from,
+                    to: m.to - v
                 }
             } else u = n.state.doc.lineAt(s.head);
             let y = s.to - e.to,
                 k = s.to - s.from;
             i = r.changeByRange(v => {
                 if (v.from == s.from && v.to == s.to) return {
                     changes: l,
@@ -10307,31 +10307,31 @@
             l = 0,
             h = null;
         e.some(y => y.annotation(Yd)) ? (this.inputState.notifiedFocused = o, l = 1) : o != this.inputState.notifiedFocused && (this.inputState.notifiedFocused = o, h = Jd(s, o), h || (l = 1));
         let f = this.observer.delayedAndroidKey,
             u = null;
         if (f ? (this.observer.clearDelayedAndroidKey(), u = this.observer.readChange(), (u && !this.state.doc.eq(s.doc) || !this.state.selection.eq(s.selection)) && (u = null)) : this.observer.clear(), s.facet(Ee.phrases) != this.state.facet(Ee.phrases)) return this.setState(s);
         r = qo.create(this, s, e), r.flags |= l;
-        let g = this.viewState.scrollTarget;
+        let m = this.viewState.scrollTarget;
         try {
             this.updateState = 2;
             for (let y of e) {
-                if (g && (g = g.map(y.changes)), y.scrollIntoView) {
+                if (m && (m = m.map(y.changes)), y.scrollIntoView) {
                     let {
                         main: k
                     } = y.state.selection;
-                    g = new yr(k.empty ? k : H.cursor(k.head, k.head > k.anchor ? -1 : 1))
+                    m = new yr(k.empty ? k : H.cursor(k.head, k.head > k.anchor ? -1 : 1))
                 }
-                for (let k of y.effects) k.is(io) && (g = k.value.clip(this.state))
+                for (let k of y.effects) k.is(io) && (m = k.value.clip(this.state))
             }
-            this.viewState.update(r, g), this.bidiCache = jo.update(this.bidiCache, r.changes), r.empty || (this.updatePlugins(r), this.inputState.update(r)), t = this.docView.update(r), this.state.facet(es) != this.styleModules && this.mountStyles(), i = this.updateAttrs(), this.showAnnouncements(e), this.docView.updateSelection(t, e.some(y => y.isUserEvent("select.pointer")))
+            this.viewState.update(r, m), this.bidiCache = jo.update(this.bidiCache, r.changes), r.empty || (this.updatePlugins(r), this.inputState.update(r)), t = this.docView.update(r), this.state.facet(es) != this.styleModules && this.mountStyles(), i = this.updateAttrs(), this.showAnnouncements(e), this.docView.updateSelection(t, e.some(y => y.isUserEvent("select.pointer")))
         } finally {
             this.updateState = 0
         }
-        if (r.startState.facet(ao) != r.state.facet(ao) && (this.viewState.mustMeasureContent = !0), (t || i || g || this.viewState.mustEnforceCursorAssoc || this.viewState.mustMeasureContent) && this.requestMeasure(), !r.empty)
+        if (r.startState.facet(ao) != r.state.facet(ao) && (this.viewState.mustMeasureContent = !0), (t || i || m || this.viewState.mustEnforceCursorAssoc || this.viewState.mustMeasureContent) && this.requestMeasure(), !r.empty)
             for (let y of this.state.facet(Ya)) try {
                 y(r)
             } catch (k) {
                 ni(this.state, k, "update listener")
             }(h || u) && Promise.resolve().then(() => {
                 h && this.state == h.startState && this.dispatch(h), u && !rp(this, u) && f.force && mr(this.contentDOM, f.key, f.keyCode)
             })
@@ -10408,25 +10408,25 @@
                 let u = f.map(k => {
                         try {
                             return k.read(this)
                         } catch (v) {
                             return ni(this.state, v), Tf
                         }
                     }),
-                    g = qo.create(this, this.state, []),
+                    m = qo.create(this, this.state, []),
                     y = !1;
-                g.flags |= h, t ? t.flags |= h : t = g, this.updateState = 2, g.empty || (this.updatePlugins(g), this.inputState.update(g), this.updateAttrs(), y = this.docView.update(g));
+                m.flags |= h, t ? t.flags |= h : t = m, this.updateState = 2, m.empty || (this.updatePlugins(m), this.inputState.update(m), this.updateAttrs(), y = this.docView.update(m));
                 for (let k = 0; k < f.length; k++)
                     if (u[k] != Tf) try {
                         let v = f[k];
                         v.write && v.write(u[k], this)
                     } catch (v) {
                         ni(this.state, v)
                     }
-                if (y && this.docView.updateSelection(!0), !g.viewportChanged && this.measureRequests.length == 0) {
+                if (y && this.docView.updateSelection(!0), !m.viewportChanged && this.measureRequests.length == 0) {
                     if (this.viewState.editorHeight)
                         if (this.viewState.scrollTarget) {
                             this.docView.scrollIntoView(this.viewState.scrollTarget), this.viewState.scrollTarget = null, o = -1;
                             continue
                         } else {
                             let v = (s < 0 ? this.viewState.heightMap.height : this.viewState.lineBlockAt(s).top) - o;
                             if (v > 1 || v < -1) {
@@ -10744,15 +10744,15 @@
         i = Object.create(null),
         r = (o, l) => {
             let h = i[o];
             if (h == null) i[o] = l;
             else if (h != l) throw new Error("Key binding " + o + " is used both as a regular binding and as a multi-stroke prefix")
         },
         s = (o, l, h, f, u) => {
-            var g, y;
+            var m, y;
             let k = t[o] || (t[o] = Object.create(null)),
                 v = l.split(/ (?!$)/).map(D => Jy(D, e));
             for (let D = 1; D < v.length; D++) {
                 let F = v.slice(0, D).join(" ");
                 r(F, !0), k[F] || (k[F] = {
                     preventDefault: !0,
                     stopPropagation: !1,
@@ -10769,29 +10769,29 @@
                 })
             }
             let A = v.join(" ");
             r(A, !1);
             let O = k[A] || (k[A] = {
                 preventDefault: !1,
                 stopPropagation: !1,
-                run: ((y = (g = k._any) === null || g === void 0 ? void 0 : g.run) === null || y === void 0 ? void 0 : y.slice()) || []
+                run: ((y = (m = k._any) === null || m === void 0 ? void 0 : m.run) === null || y === void 0 ? void 0 : y.slice()) || []
             });
             h && O.run.push(h), f && (O.preventDefault = !0), u && (O.stopPropagation = !0)
         };
     for (let o of n) {
         let l = o.scope ? o.scope.split(" ") : ["editor"];
         if (o.any)
             for (let f of l) {
                 let u = t[f] || (t[f] = Object.create(null));
                 u._any || (u._any = {
                     preventDefault: !1,
                     stopPropagation: !1,
                     run: []
                 });
-                for (let g in u) u[g].run.push(o.any)
+                for (let m in u) u[m].run.push(o.any)
             }
         let h = o[e] || o.key;
         if (h)
             for (let f of l) s(f, h, o.run, o.preventDefault, o.stopPropagation), o.shift && s(f, "Shift-" + h, o.shift, o.preventDefault, o.stopPropagation)
     }
     return t
 }
@@ -10801,19 +10801,19 @@
         s = pt(r, 0),
         o = ti(s) == r.length && r != " ",
         l = "",
         h = !1,
         f = !1,
         u = !1;
     fn && fn.view == t && fn.scope == i && (l = fn.prefix + " ", Ud.indexOf(e.keyCode) < 0 && (f = !0, fn = null));
-    let g = new Set,
+    let m = new Set,
         y = O => {
             if (O) {
                 for (let D of O.run)
-                    if (!g.has(D) && (g.add(D), D(t, e))) return O.stopPropagation && (u = !0), !0;
+                    if (!m.has(D) && (m.add(D), D(t, e))) return O.stopPropagation && (u = !0), !0;
                 O.preventDefault && (O.stopPropagation && (u = !0), f = !0)
             }
             return !1
         },
         k = n[i],
         v, A;
     return k && (y(k[l + ho(r, e, !o)]) ? h = !0 : o && (e.altKey || e.metaKey || e.ctrlKey) && !(ee.windows && e.ctrlKey && e.altKey) && (v = wn[e.keyCode]) && v != r ? (y(k[l + ho(v, e, !0)]) || e.shiftKey && (A = us[e.keyCode]) != r && A != v && y(k[l + ho(A, e, !1)])) && (h = !0) : o && e.shiftKey && y(k[l + ho(r, e, !0)]) && (h = !0), !h && y(k._any) && (h = !0)), f && (h = !0), h && u && e.stopPropagation(), h
@@ -10868,26 +10868,26 @@
         r = Math.min(t.to, n.viewport.to),
         s = n.textDirection == Ue.LTR,
         o = n.contentDOM,
         l = o.getBoundingClientRect(),
         h = lp(n),
         f = o.querySelector(".cm-line"),
         u = f && window.getComputedStyle(f),
-        g = l.left + (u ? parseInt(u.paddingLeft) + Math.min(0, parseInt(u.textIndent)) : 0),
+        m = l.left + (u ? parseInt(u.paddingLeft) + Math.min(0, parseInt(u.textIndent)) : 0),
         y = l.right - (u ? parseInt(u.paddingRight) : 0),
         k = ih(n, i),
         v = ih(n, r),
         A = k.type == Dt.Text ? k : null,
         O = v.type == Dt.Text ? v : null;
     if (A && (n.lineWrapping || k.widgetLineBreaks) && (A = Ef(n, i, A)), O && (n.lineWrapping || v.widgetLineBreaks) && (O = Ef(n, r, O)), A && O && A.from == O.from) return F($(t.from, t.to, A));
     {
         let z = A ? $(t.from, null, A) : j(k, !1),
             G = O ? $(null, t.to, O) : j(v, !0),
             p = [];
-        return (A || k).to < (O || v).from - (A && O ? 1 : 0) || k.widgetLineBreaks > 1 && z.bottom + n.defaultLineHeight / 2 < G.top ? p.push(D(g, z.bottom, y, G.top)) : z.bottom < G.top && n.elementAtHeight((z.bottom + G.top) / 2).type == Dt.Text && (z.bottom = G.top = (z.bottom + G.top) / 2), F(z).concat(p).concat(F(G))
+        return (A || k).to < (O || v).from - (A && O ? 1 : 0) || k.widgetLineBreaks > 1 && z.bottom + n.defaultLineHeight / 2 < G.top ? p.push(D(m, z.bottom, y, G.top)) : z.bottom < G.top && n.elementAtHeight((z.bottom + G.top) / 2).type == Dt.Text && (z.bottom = G.top = (z.bottom + G.top) / 2), F(z).concat(p).concat(F(G))
     }
 
     function D(z, G, p, he) {
         return new Ds(e, z - h.left, G - h.top - .01, p - z, he - G + .01)
     }
 
     function F({
@@ -10904,15 +10904,15 @@
         let he = 1e9,
             J = -1e9,
             ae = [];
 
         function pe(ye, Be, st, _e, Ye) {
             let be = n.coordsAtPos(ye, ye == p.to ? -2 : 2),
                 We = n.coordsAtPos(st, st == p.from ? 2 : -2);
-            !be || !We || (he = Math.min(be.top, We.top, he), J = Math.max(be.bottom, We.bottom, J), Ye == Ue.LTR ? ae.push(s && Be ? g : be.left, s && _e ? y : We.right) : ae.push(!s && _e ? g : We.left, !s && Be ? y : be.right))
+            !be || !We || (he = Math.min(be.top, We.top, he), J = Math.max(be.bottom, We.bottom, J), Ye == Ue.LTR ? ae.push(s && Be ? m : be.left, s && _e ? y : We.right) : ae.push(!s && _e ? m : We.left, !s && Be ? y : be.right))
         }
         let fe = z != null ? z : p.from,
             ie = G != null ? G : p.to;
         for (let ye of n.visibleRanges)
             if (ye.to > fe && ye.from < ie)
                 for (let Be = Math.max(ye.from, fe), st = Math.min(ye.to, ie);;) {
                     let _e = n.state.doc.lineAt(Be);
@@ -11172,16 +11172,16 @@
             decorate: r,
             boundary: s,
             maxLength: o = 1e3
         } = e;
         if (!t.global) throw new RangeError("The regular expression given to MatchDecorator should have its 'g' flag set");
         if (this.regexp = t, r) this.addMatch = (l, h, f, u) => r(u, f, f + l[0].length, l, h);
         else if (typeof i == "function") this.addMatch = (l, h, f, u) => {
-            let g = i(l, h, f);
-            g && u(f, f + l[0].length, g)
+            let m = i(l, h, f);
+            m && u(f, f + l[0].length, m)
         };
         else if (i) this.addMatch = (l, h, f, u) => u(f, f + l[0].length, i);
         else throw new RangeError("Either 'decorate' or 'decoration' should be provided to MatchDecorator");
         this.boundary = s, this.maxLength = o
     }
     createDeco(e) {
         let t = new xn,
@@ -11204,36 +11204,36 @@
         for (let s of e.visibleRanges) {
             let o = Math.max(s.from, i),
                 l = Math.min(s.to, r);
             if (l > o) {
                 let h = e.state.doc.lineAt(o),
                     f = h.to < l ? e.state.doc.lineAt(l) : h,
                     u = Math.max(s.from, h.from),
-                    g = Math.min(s.to, f.to);
+                    m = Math.min(s.to, f.to);
                 if (this.boundary) {
                     for (; o > h.from; o--)
                         if (this.boundary.test(h.text[o - 1 - h.from])) {
                             u = o;
                             break
                         } for (; l < f.to; l++)
                         if (this.boundary.test(f.text[l - f.from])) {
-                            g = l;
+                            m = l;
                             break
                         }
                 }
                 let y = [],
                     k, v = (A, O, D) => y.push(D.range(A, O));
                 if (h == f)
                     for (this.regexp.lastIndex = u - h.from;
-                        (k = this.regexp.exec(h.text)) && k.index < g - h.from;) this.addMatch(k, e, k.index + h.from, v);
-                else Rf(e.state.doc, this.regexp, u, g, (A, O) => this.addMatch(O, e, A, v));
+                        (k = this.regexp.exec(h.text)) && k.index < m - h.from;) this.addMatch(k, e, k.index + h.from, v);
+                else Rf(e.state.doc, this.regexp, u, m, (A, O) => this.addMatch(O, e, A, v));
                 t = t.update({
                     filterFrom: u,
-                    filterTo: g,
-                    filter: (A, O) => A < u || O > g,
+                    filterTo: m,
+                    filter: (A, O) => A < u || O > m,
                     add: y
                 })
             }
         }
         return t
     }
 }
@@ -11404,22 +11404,22 @@
         }
         let o = [],
             l = t ? [] : null;
         for (let h = 0; h < s.length; h++) {
             let f = s[h],
                 u = -1;
             if (f) {
-                for (let g = 0; g < this.tooltips.length; g++) {
-                    let y = this.tooltips[g];
-                    y && y.create == f.create && (u = g)
+                for (let m = 0; m < this.tooltips.length; m++) {
+                    let y = this.tooltips[m];
+                    y && y.create == f.create && (u = m)
                 }
                 if (u < 0) o[h] = this.createTooltipView(f), l && (l[h] = !!f.above);
                 else {
-                    let g = o[h] = this.tooltipViews[u];
-                    l && (l[h] = t[u]), g.update && g.update(e)
+                    let m = o[h] = this.tooltipViews[u];
+                    l && (l[h] = t[u]), m.update && m.update(e)
                 }
             }
         }
         for (let h of this.tooltipViews) o.indexOf(h) < 0 && (h.dom.remove(), (i = h.destroy) === null || i === void 0 || i.call(h));
         return t && (l.forEach((h, f) => t[f] = h), t.length = l.length), this.input = r, this.tooltips = s, this.tooltipViews = o, !0
     }
 }
@@ -11559,43 +11559,43 @@
             } = n, o = [];
             for (let l = 0; l < this.manager.tooltips.length; l++) {
                 let h = this.manager.tooltips[l],
                     f = this.manager.tooltipViews[l],
                     {
                         dom: u
                     } = f,
-                    g = n.pos[l],
+                    m = n.pos[l],
                     y = n.size[l];
-                if (!g || g.bottom <= Math.max(t.top, i.top) || g.top >= Math.min(t.bottom, i.bottom) || g.right < Math.max(t.left, i.left) - .1 || g.left > Math.min(t.right, i.right) + .1) {
+                if (!m || m.bottom <= Math.max(t.top, i.top) || m.top >= Math.min(t.bottom, i.bottom) || m.right < Math.max(t.left, i.left) - .1 || m.left > Math.min(t.right, i.right) + .1) {
                     u.style.top = jr;
                     continue
                 }
                 let k = h.arrow ? f.dom.querySelector(".cm-tooltip-arrow") : null,
                     v = k ? 7 : 0,
                     A = y.right - y.left,
                     O = (e = Pf.get(f)) !== null && e !== void 0 ? e : y.bottom - y.top,
                     D = f.offset || Mb,
                     F = this.view.textDirection == Ue.LTR,
-                    $ = y.width > i.right - i.left ? F ? i.left : i.right - y.width : F ? Math.min(g.left - (k ? 14 : 0) + D.x, i.right - A) : Math.max(i.left, g.left - A + (k ? 14 : 0) - D.x),
+                    $ = y.width > i.right - i.left ? F ? i.left : i.right - y.width : F ? Math.min(m.left - (k ? 14 : 0) + D.x, i.right - A) : Math.max(i.left, m.left - A + (k ? 14 : 0) - D.x),
                     j = this.above[l];
-                !h.strictSide && (j ? g.top - (y.bottom - y.top) - D.y < i.top : g.bottom + (y.bottom - y.top) + D.y > i.bottom) && j == i.bottom - g.bottom > g.top - i.top && (j = this.above[l] = !j);
-                let z = (j ? g.top - i.top : i.bottom - g.bottom) - v;
+                !h.strictSide && (j ? m.top - (y.bottom - y.top) - D.y < i.top : m.bottom + (y.bottom - y.top) + D.y > i.bottom) && j == i.bottom - m.bottom > m.top - i.top && (j = this.above[l] = !j);
+                let z = (j ? m.top - i.top : i.bottom - m.bottom) - v;
                 if (z < O && f.resize !== !1) {
                     if (z < this.view.defaultLineHeight) {
                         u.style.top = jr;
                         continue
                     }
                     Pf.set(f, O), u.style.height = (O = z) / s + "px"
                 } else u.style.height && (u.style.height = "");
-                let G = j ? g.top - O - v - D.y : g.bottom + v + D.y,
+                let G = j ? m.top - O - v - D.y : m.bottom + v + D.y,
                     p = $ + A;
                 if (f.overlap !== !0)
                     for (let he of o) he.left < p && he.right > $ && he.top < G + O && he.bottom > G && (G = j ? he.top - O - 2 - v : he.bottom + v + 2);
                 if (this.position == "absolute" ? (u.style.top = (G - n.parent.top) / s + "px", u.style.left = ($ - n.parent.left) / r + "px") : (u.style.top = G / s + "px", u.style.left = $ / r + "px"), k) {
-                    let he = g.left + (F ? D.x : -D.x) - ($ + 14 - 7);
+                    let he = m.left + (F ? D.x : -D.x) - ($ + 14 - 7);
                     k.style.left = he / r + "px"
                 }
                 f.overlap !== !0 && o.push({
                     left: $,
                     top: G,
                     right: p,
                     bottom: G + O
@@ -12190,26 +12190,26 @@
         for (let s = 0, o = 0;;) {
             let l = o,
                 h = s < t.length ? t[s++] : null,
                 f = !1;
             if (h) {
                 let u = h.elementClass;
                 u && (i += " " + u);
-                for (let g = o; g < this.markers.length; g++)
-                    if (this.markers[g].compare(h)) {
-                        l = g, f = !0;
+                for (let m = o; m < this.markers.length; m++)
+                    if (this.markers[m].compare(h)) {
+                        l = m, f = !0;
                         break
                     }
             } else l = this.markers.length;
             for (; o < l;) {
                 let u = this.markers[o++];
                 if (u.toDOM) {
                     u.destroy(r);
-                    let g = r.nextSibling;
-                    r.remove(), r = g
+                    let m = r.nextSibling;
+                    r.remove(), r = m
                 }
             }
             if (!h) break;
             h.toDOM && (f ? r = r.nextSibling : this.dom.insertBefore(h.toDOM(e), r)), f && o++
         }
         this.dom.className = i, this.markers = t
     }
@@ -12660,24 +12660,24 @@
     nextChild(e, t, i, r, s = 0) {
         for (let o = this;;) {
             for (let {
                     children: l,
                     positions: h
                 } = o._tree, f = t > 0 ? l.length : -1; e != f; e += t) {
                 let u = l[e],
-                    g = h[e] + o.from;
-                if (bp(r, i, g, g + u.length)) {
+                    m = h[e] + o.from;
+                if (bp(r, i, m, m + u.length)) {
                     if (u instanceof Sn) {
                         if (s & ot.ExcludeBuffers) continue;
-                        let y = u.findChild(0, u.buffer.length, t, i - g, r);
-                        if (y > -1) return new gn(new Gb(o, u, e, g), null, y)
+                        let y = u.findChild(0, u.buffer.length, t, i - m, r);
+                        if (y > -1) return new gn(new Gb(o, u, e, m), null, y)
                     } else if (s & ot.IncludeAnonymous || !u.type.isAnonymous || Vh(u)) {
                         let y;
-                        if (!(s & ot.IgnoreMounts) && (y = Uo.get(u)) && !y.overlay) return new si(y.tree, g, e, o);
-                        let k = new si(u, g, e, o);
+                        if (!(s & ot.IgnoreMounts) && (y = Uo.get(u)) && !y.overlay) return new si(y.tree, m, e, o);
+                        let k = new si(u, m, e, o);
                         return s & ot.IncludeAnonymous || !k.type.isAnonymous ? k : k.nextChild(t < 0 ? u.children.length - 1 : 0, t, i, r)
                     }
                 }
             }
             if (s & ot.IncludeAnonymous || !o.type.isAnonymous || (o.index >= 0 ? e = o.index + t : e = t < 0 ? -1 : o._parent._tree.children.length, o = o._parent, !o)) return null
         }
     }
@@ -13064,15 +13064,15 @@
         buffer: t,
         nodeSet: i,
         maxBufferLength: r = yp,
         reused: s = [],
         minRepeatType: o = i.types.length
     } = n, l = Array.isArray(t) ? new jh(t, t.length) : t, h = i.types, f = 0, u = 0;
 
-    function g(z, G, p, he, J, ae) {
+    function m(z, G, p, he, J, ae) {
         let {
             id: pe,
             start: fe,
             end: ie,
             size: ye
         } = l, Be = u;
         for (; ye < 0;)
@@ -13099,15 +13099,15 @@
             let We = l.pos - ye;
             l.next();
             let Ce = [],
                 bt = [],
                 Oe = pe >= o ? pe : -1,
                 Tt = 0,
                 yi = ie;
-            for (; l.pos > We;) Oe >= 0 && l.id == Oe && l.size >= 0 ? (l.end <= yi - r && (v(Ce, bt, fe, Tt, l.end, yi, Oe, Be), Tt = Ce.length, yi = l.end), l.next()) : ae > 2500 ? y(fe, We, Ce, bt) : g(fe, We, Ce, bt, Oe, ae + 1);
+            for (; l.pos > We;) Oe >= 0 && l.id == Oe && l.size >= 0 ? (l.end <= yi - r && (v(Ce, bt, fe, Tt, l.end, yi, Oe, Be), Tt = Ce.length, yi = l.end), l.next()) : ae > 2500 ? y(fe, We, Ce, bt) : m(fe, We, Ce, bt, Oe, ae + 1);
             if (Oe >= 0 && Tt > 0 && Tt < Ce.length && v(Ce, bt, fe, Tt, fe, yi, Oe, Be), Ce.reverse(), bt.reverse(), Oe > -1 && Tt > 0) {
                 let On = k(st);
                 _e = Uh(st, Ce, bt, 0, Ce.length, 0, ie - fe, On, On)
             } else _e = A(st, Ce, bt, ie - fe, Be - ie)
         }
         p.push(_e), he.push(be)
     }
@@ -13217,15 +13217,15 @@
             }
             G[--p] = fe, G[--p] = ae - z, G[--p] = J - z, G[--p] = he
         } else pe == -3 ? f = he : pe == -4 && (u = he);
         return p
     }
     let F = [],
         $ = [];
-    for (; l.pos > 0;) g(n.start || 0, n.bufferStart || 0, F, $, -1, 0);
+    for (; l.pos > 0;) m(n.start || 0, n.bufferStart || 0, F, $, -1, 0);
     let j = (e = n.length) !== null && e !== void 0 ? e : F.length ? $[0] + F[0].length : 0;
     return new Je(h[n.topID], F.reverse(), $.reverse(), j)
 }
 const $f = new WeakMap;
 
 function Bo(n, e) {
     if (!n.isAnonymous || e instanceof Sn || e.type != n) return 1;
@@ -13244,15 +13244,15 @@
     return t
 }
 
 function Uh(n, e, t, i, r, s, o, l, h) {
     let f = 0;
     for (let v = i; v < r; v++) f += Bo(n, e[v]);
     let u = Math.ceil(f * 1.5 / 8),
-        g = [],
+        m = [],
         y = [];
 
     function k(v, A, O, D, F) {
         for (let $ = O; $ < D;) {
             let j = $,
                 z = A[$],
                 G = Bo(n, v[$]);
@@ -13263,23 +13263,23 @@
             }
             if ($ == j + 1) {
                 if (G > u) {
                     let p = v[j];
                     k(p.children, p.positions, 0, p.children.length, A[j] + F);
                     continue
                 }
-                g.push(v[j])
+                m.push(v[j])
             } else {
                 let p = A[$ - 1] + v[$ - 1].length - z;
-                g.push(Uh(n, v, A, j, $, z, p, null, h))
+                m.push(Uh(n, v, A, j, $, z, p, null, h))
             }
             y.push(z + F - s)
         }
     }
-    return k(e, t, i, r, 0), (l || h)(g, y, o)
+    return k(e, t, i, r, 0), (l || h)(m, y, o)
 }
 class jn {
     constructor(e, t, i, r, s = !1, o = !1) {
         this.from = e, this.to = t, this.tree = i, this.offset = r, this.open = (s ? 1 : 0) | (o ? 2 : 0)
     }
     get openStart() {
         return (this.open & 1) > 0
@@ -13295,24 +13295,24 @@
     static applyChanges(e, t, i = 128) {
         if (!t.length) return e;
         let r = [],
             s = 1,
             o = e.length ? e[0] : null;
         for (let l = 0, h = 0, f = 0;; l++) {
             let u = l < t.length ? t[l] : null,
-                g = u ? u.fromA : 1e9;
-            if (g - h >= i)
-                for (; o && o.from < g;) {
+                m = u ? u.fromA : 1e9;
+            if (m - h >= i)
+                for (; o && o.from < m;) {
                     let y = o;
-                    if (h >= y.from || g <= y.to || f) {
+                    if (h >= y.from || m <= y.to || f) {
                         let k = Math.max(y.from, h) - f,
-                            v = Math.min(y.to, g) - f;
+                            v = Math.min(y.to, m) - f;
                         y = k >= v ? null : new jn(k, v, y.tree, y.offset + f, l > 0, !!u)
                     }
-                    if (y && r.push(y), o.to > g) break;
+                    if (y && r.push(y), o.to > m) break;
                     o = s < e.length ? e[s++] : null
                 }
             if (!u) break;
             h = u.toA, f = u.toA - u.toB
         }
         return r
     }
@@ -13405,29 +13405,29 @@
         let i = n[t];
         Array.isArray(i) || (i = [i]);
         for (let r of t.split(" "))
             if (r) {
                 let s = [],
                     o = 2,
                     l = r;
-                for (let g = 0;;) {
-                    if (l == "..." && g > 0 && g + 3 == r.length) {
+                for (let m = 0;;) {
+                    if (l == "..." && m > 0 && m + 3 == r.length) {
                         o = 1;
                         break
                     }
                     let y = /^"(?:[^"\\]|\\.)*?"|[^\/!]+/.exec(l);
                     if (!y) throw new RangeError("Invalid path: " + r);
-                    if (s.push(y[0] == "*" ? "" : y[0][0] == '"' ? JSON.parse(y[0]) : y[0]), g += y[0].length, g == r.length) break;
-                    let k = r[g++];
-                    if (g == r.length && k == "!") {
+                    if (s.push(y[0] == "*" ? "" : y[0][0] == '"' ? JSON.parse(y[0]) : y[0]), m += y[0].length, m == r.length) break;
+                    let k = r[m++];
+                    if (m == r.length && k == "!") {
                         o = 0;
                         break
                     }
                     if (k != "/") throw new RangeError("Invalid path: " + r);
-                    l = r.slice(g)
+                    l = r.slice(m)
                 }
                 let h = s.length - 1,
                     f = s[h];
                 if (!f) throw new RangeError("Invalid path: " + r);
                 let u = new Go(i, o, h > 0 ? s.slice(0, h) : null);
                 e[f] = u.sort(e[f])
             }
@@ -13510,16 +13510,16 @@
             from: l,
             to: h
         } = e;
         if (l >= i || h <= t) return;
         o.isTop && (s = this.highlighters.filter(k => !k.scope || k.scope(o)));
         let f = r,
             u = ox(e) || Go.empty,
-            g = nx(s, u.tags);
-        if (g && (f && (f += " "), f += g, u.mode == 1 && (r += (r ? " " : "") + g)), this.startSpan(Math.max(t, l), f), u.opaque) return;
+            m = nx(s, u.tags);
+        if (m && (f && (f += " "), f += m, u.mode == 1 && (r += (r ? " " : "") + m)), this.startSpan(Math.max(t, l), f), u.opaque) return;
         let y = e.tree && e.tree.prop(Se.mounted);
         if (y && y.overlay) {
             let k = e.node.enter(y.overlay[0].from + l, 1),
                 v = this.highlighters.filter(O => !O.scope || O.scope(y.tree.type)),
                 A = e.firstChild();
             for (let O = 0, D = l;; O++) {
                 let F = O < y.overlay.length ? y.overlay[O] : null,
@@ -13757,18 +13757,18 @@
                 return lt(this)
             }
         }), this.parser = t, this.extension = [Cn.of(this), Ee.languageData.of((s, o, l) => {
             let h = jf(s, o, l),
                 f = h.type.prop(ur);
             if (!f) return [];
             let u = s.facet(f),
-                g = h.type.prop(ax);
-            if (g) {
+                m = h.type.prop(ax);
+            if (m) {
                 let y = h.resolve(o - h.from, l);
-                for (let k of g)
+                for (let k of m)
                     if (k.test(y, s)) {
                         let v = s.facet(k.facet);
                         return k.type == "replace" ? v : v.concat(u)
                     }
             }
             return u
         })].concat(i)
@@ -13925,30 +13925,30 @@
             tree: r,
             treeLen: s,
             viewport: o,
             skipped: l
         } = this;
         if (this.takeTree(), !e.empty) {
             let h = [];
-            if (e.iterChangedRanges((f, u, g, y) => h.push({
+            if (e.iterChangedRanges((f, u, m, y) => h.push({
                     fromA: f,
                     toA: u,
-                    fromB: g,
+                    fromB: m,
                     toB: y
                 })), i = jn.applyChanges(i, h), r = Je.empty, s = 0, o = {
                     from: e.mapPos(o.from, -1),
                     to: e.mapPos(o.to, 1)
                 }, this.skipped.length) {
                 l = [];
                 for (let f of this.skipped) {
                     let u = e.mapPos(f.from, 1),
-                        g = e.mapPos(f.to, -1);
-                    u < g && l.push({
+                        m = e.mapPos(f.to, -1);
+                    u < m && l.push({
                         from: u,
-                        to: g
+                        to: m
                     })
                 }
             }
         }
         return new Xo(this.parser, t, i, r, s, o, l, this.scheduleOn)
     }
     updateViewport(e) {
@@ -14343,18 +14343,18 @@
         for (let {
                 head: f
             }
             of o.selection.ranges) {
             let u = o.doc.lineAt(f);
             if (u.from == l) continue;
             l = u.from;
-            let g = Gh(o, u.from);
-            if (g == null) continue;
+            let m = Gh(o, u.from);
+            if (m == null) continue;
             let y = /^\s*/.exec(u.text)[0],
-                k = ws(o, g);
+                k = ws(o, m);
             y != k && h.push({
                 from: u.from,
                 to: u.from + y.length,
                 insert: k
             })
         }
         return h.length ? [n, {
@@ -14917,32 +14917,32 @@
         },
         f = 0,
         u = l == null ? void 0 : l.cursor();
     if (u && (t < 0 ? u.childBefore(i.from) : u.childAfter(i.to)))
         do
             if (t < 0 ? u.to <= i.from : u.from >= i.to) {
                 if (f == 0 && s.indexOf(u.type.name) > -1 && u.from < u.to) {
-                    let g = mh(u);
+                    let m = mh(u);
                     return {
                         start: h,
-                        end: g ? {
-                            from: g.from,
-                            to: g.to
+                        end: m ? {
+                            from: m.from,
+                            to: m.to
                         } : void 0,
                         matched: !0
                     }
                 } else if (gh(u.type, t, o)) f++;
                 else if (gh(u.type, -t, o)) {
                     if (f == 0) {
-                        let g = mh(u);
+                        let m = mh(u);
                         return {
                             start: h,
-                            end: g && g.from < g.to ? {
-                                from: g.from,
-                                to: g.to
+                            end: m && m.from < m.to ? {
+                                from: m.from,
+                                to: m.to
                             } : void 0,
                             matched: !1
                         }
                     }
                     f--
                 }
             } while (t < 0 ? u.prevSibling() : u.nextSibling());
@@ -14957,33 +14957,33 @@
         h = o.indexOf(l);
     if (h < 0 || h % 2 == 0 != t > 0) return null;
     let f = {
             from: t < 0 ? e - 1 : e,
             to: t > 0 ? e + 1 : e
         },
         u = n.doc.iterRange(e, t > 0 ? n.doc.length : 0),
-        g = 0;
+        m = 0;
     for (let y = 0; !u.next().done && y <= s;) {
         let k = u.value;
         t < 0 && (y += k.length);
         let v = e + y * t;
         for (let A = t > 0 ? 0 : k.length - 1, O = t > 0 ? k.length : -1; A != O; A += t) {
             let D = o.indexOf(k[A]);
             if (!(D < 0 || i.resolveInner(v + A, 1).type != r))
-                if (D % 2 == 0 == t > 0) g++;
+                if (D % 2 == 0 == t > 0) m++;
                 else {
-                    if (g == 1) return {
+                    if (m == 1) return {
                         start: f,
                         end: {
                             from: v + A,
                             to: v + A + 1
                         },
                         matched: D >> 1 == h >> 1
                     };
-                    g--
+                    m--
                 }
         }
         t > 0 && (y += k.length)
     }
     return u.done ? {
         start: f,
         matched: !1
@@ -15079,27 +15079,27 @@
             margin: l && 1
         },
         close: {
             pos: r + h,
             margin: h && 1
         }
     };
-    let u, g;
-    r - i <= 2 * Qr ? u = g = n.sliceDoc(i, r) : (u = n.sliceDoc(i, i + Qr), g = n.sliceDoc(r - Qr, r));
+    let u, m;
+    r - i <= 2 * Qr ? u = m = n.sliceDoc(i, r) : (u = n.sliceDoc(i, i + Qr), m = n.sliceDoc(r - Qr, r));
     let y = /^\s*/.exec(u)[0].length,
-        k = /\s*$/.exec(g)[0].length,
-        v = g.length - k - t.length;
-    return u.slice(y, y + e.length) == e && g.slice(v, v + t.length) == t ? {
+        k = /\s*$/.exec(m)[0].length,
+        v = m.length - k - t.length;
+    return u.slice(y, y + e.length) == e && m.slice(v, v + t.length) == t ? {
         open: {
             pos: i + y + e.length,
             margin: /\s/.test(u.charAt(y + e.length)) ? 1 : 0
         },
         close: {
             pos: r - k - t.length,
-            margin: /\s/.test(g.charAt(v - 1)) ? 1 : 0
+            margin: /\s/.test(m.charAt(v - 1)) ? 1 : 0
         }
     } : null
 }
 
 function s1(n) {
     let e = [];
     for (let t of n.selection.ranges) {
@@ -15159,46 +15159,46 @@
         }
         of t) {
         let l = i.length,
             h = 1e9,
             f = Jh(e, s).line;
         if (f) {
             for (let u = s; u <= o;) {
-                let g = e.doc.lineAt(u);
-                if (g.from > r && (s == o || o > g.from)) {
-                    r = g.from;
-                    let y = /^\s*/.exec(g.text)[0].length,
-                        k = y == g.length,
-                        v = g.text.slice(y, y + f.length) == f ? y : -1;
-                    y < g.text.length && y < h && (h = y), i.push({
-                        line: g,
+                let m = e.doc.lineAt(u);
+                if (m.from > r && (s == o || o > m.from)) {
+                    r = m.from;
+                    let y = /^\s*/.exec(m.text)[0].length,
+                        k = y == m.length,
+                        v = m.text.slice(y, y + f.length) == f ? y : -1;
+                    y < m.text.length && y < h && (h = y), i.push({
+                        line: m,
                         comment: v,
                         token: f,
                         indent: y,
                         empty: k,
                         single: !1
                     })
                 }
-                u = g.to + 1
+                u = m.to + 1
             }
             if (h < 1e9)
                 for (let u = l; u < i.length; u++) i[u].indent < i[u].line.text.length && (i[u].indent = h);
             i.length == l + 1 && (i[l].single = !0)
         }
     }
     if (n != 2 && i.some(s => s.comment < 0 && (!s.empty || s.single))) {
         let s = [];
         for (let {
                 line: l,
                 token: h,
                 indent: f,
                 empty: u,
-                single: g
+                single: m
             }
-            of i)(g || !u) && s.push({
+            of i)(m || !u) && s.push({
             from: l.from + f,
             insert: h + " "
         });
         let o = e.changes(s);
         return {
             changes: o,
             selection: e.selection.map(o, 1)
@@ -16010,22 +16010,22 @@
                 }),
                 u = Gh(f, s);
             for (u == null && (u = Os(/^\s*/.exec(e.doc.lineAt(s).text)[0], e.tabSize)); o < l.to && /\s/.test(l.text[o - l.from]);) o++;
             h ? {
                 from: s,
                 to: o
             } = h : s > l.from && s < l.from + 100 && !/\S/.test(l.text.slice(0, s)) && (s = l.from);
-            let g = ["", ws(e, u)];
-            return h && g.push(ws(e, f.lineIndent(l.from, -1))), {
+            let m = ["", ws(e, u)];
+            return h && m.push(ws(e, f.lineIndent(l.from, -1))), {
                 changes: {
                     from: s,
                     to: o,
-                    insert: De.of(g)
+                    insert: De.of(m)
                 },
-                range: H.cursor(s + 1 + g[1].length)
+                range: H.cursor(s + 1 + m[1].length)
             }
         });
         return t(e.update(i, {
             scrollIntoView: !0,
             userEvent: "input"
         })), !0
     }
@@ -16533,16 +16533,16 @@
         }, n.state.phrase("go")));
 
     function r() {
         let s = /^([+-])?(\d+)?(:\d+)?(%)?$/.exec(t.value);
         if (!s) return;
         let {
             state: o
-        } = n, l = o.doc.lineAt(o.selection.main.head), [, h, f, u, g] = s, y = u ? +u.slice(1) : 0, k = f ? +f : l.number;
-        if (f && g) {
+        } = n, l = o.doc.lineAt(o.selection.main.head), [, h, f, u, m] = s, y = u ? +u.slice(1) : 0, k = f ? +f : l.number;
+        if (f && m) {
             let O = k / 100;
             h && (O = O * (h == "-" ? -1 : 1) + l.number / o.doc.lines), k = Math.round(o.doc.lines * O)
         } else f && h && (k = k * (h == "-" ? -1 : 1) + l.number);
         let v = o.doc.line(Math.max(1, Math.min(o.doc.lines, k))),
             A = H.cursor(v.from + Math.max(0, Math.min(y, v.length)));
         n.dispatch({
             effects: [il.of(!1), te.scrollIntoView(A.from, {
@@ -16648,17 +16648,17 @@
             }
             let l = [];
             for (let h of n.visibleRanges) {
                 let f = new Cr(t.doc, s, h.from, h.to);
                 for (; !f.next().done;) {
                     let {
                         from: u,
-                        to: g
+                        to: m
                     } = f.value;
-                    if ((!o || su(o, t, u, g)) && (r.empty && u <= r.from && g >= r.to ? l.push(bk.range(u, g)) : (u >= r.to || g <= r.from) && l.push(yk.range(u, g)), l.length > e.maxMatches)) return de.none
+                    if ((!o || su(o, t, u, m)) && (r.empty && u <= r.from && m >= r.to ? l.push(bk.range(u, m)) : (u >= r.to || m <= r.from) && l.push(yk.range(u, m)), l.length > e.maxMatches)) return de.none
                 }
             }
             return de.set(l)
         }
     }, {
         decorations: n => n.decorations
     }),
@@ -16901,16 +16901,16 @@
             for (let r = 0, s = t.visibleRanges, o = s.length; r < o; r++) {
                 let {
                     from: l,
                     to: h
                 } = s[r];
                 for (; r < o - 1 && h > s[r + 1].from - 2 * 250;) h = s[++r].to;
                 n.highlight(t.state, l, h, (f, u) => {
-                    let g = t.state.selection.ranges.some(y => y.from == f && y.to == u);
-                    i.add(f, u, g ? Dk : Ek)
+                    let m = t.state.selection.ranges.some(y => y.from == f && y.to == u);
+                    i.add(f, u, m ? Dk : Ek)
                 })
             }
             return i.finish()
         }
     }, {
         decorations: n => n.decorations
     });
@@ -17446,28 +17446,28 @@
             for (let F = 0, $ = Math.min(e.length, 200); F < $ && f < h;) {
                 let j = pt(e, F);
                 (j == t[f] || j == i[f]) && (r[f++] = F), F += ti(j)
             }
             if (f < h) return !1
         }
         let u = 0,
-            g = 0,
+            m = 0,
             y = !1,
             k = 0,
             v = -1,
             A = -1,
             O = /[a-z]/.test(e),
             D = !0;
-        for (let F = 0, $ = Math.min(e.length, 200), j = 0; F < $ && g < h;) {
+        for (let F = 0, $ = Math.min(e.length, 200), j = 0; F < $ && m < h;) {
             let z = pt(e, F);
             l < 0 && (u < h && z == t[u] && (s[u++] = F), k < h && (z == t[k] || z == i[k] ? (k == 0 && (v = F), A = F + 1, k++) : k = 0));
             let G, p = z < 255 ? z >= 48 && z <= 57 || z >= 97 && z <= 122 ? 2 : z >= 65 && z <= 90 ? 1 : 0 : (G = Rh(z)) != G.toLowerCase() ? 1 : G != G.toUpperCase() ? 2 : 0;
-            (!F || p == 1 && O || j == 0 && p != 0) && (t[g] == z || i[g] == z && (y = !0) ? o[g++] = F : o.length && (D = !1)), j = p, F += ti(z)
+            (!F || p == 1 && O || j == 0 && p != 0) && (t[m] == z || i[m] == z && (y = !0) ? o[m++] = F : o.length && (D = !1)), j = p, F += ti(z)
         }
-        return g == h && o[0] == 0 && D ? this.result(-100 + (y ? -200 : 0), o, e) : k == h && v == 0 ? this.ret(-200 - e.length + (A == e.length ? 0 : -100), [0, A]) : l > -1 ? this.ret(-700 - e.length, [l, l + this.pattern.length]) : k == h ? this.ret(-900 - e.length, [v, A]) : g == h ? this.result(-100 + (y ? -200 : 0) + -700 + (D ? 0 : -1100), o, e) : t.length == 2 ? !1 : this.result((r[0] ? -700 : 0) + -200 + -1100, r, e)
+        return m == h && o[0] == 0 && D ? this.result(-100 + (y ? -200 : 0), o, e) : k == h && v == 0 ? this.ret(-200 - e.length + (A == e.length ? 0 : -100), [0, A]) : l > -1 ? this.ret(-700 - e.length, [l, l + this.pattern.length]) : k == h ? this.ret(-900 - e.length, [v, A]) : m == h ? this.result(-100 + (y ? -200 : 0) + -700 + (D ? 0 : -1100), o, e) : t.length == 2 ? !1 : this.result((r[0] ? -700 : 0) + -200 + -1100, r, e)
     }
     result(e, t, i) {
         let r = [],
             s = 0;
         for (let o of t) {
             let l = o + (this.astral ? ti(pt(i, o)) : 1);
             s && r[s - 1] == o ? r[s - 1] = l : (r[s++] = o, r[s++] = l)
@@ -17509,28 +17509,28 @@
 }
 
 function Vk(n, e, t, i, r, s) {
     let o = n.textDirection == Ue.RTL,
         l = o,
         h = !1,
         f = "top",
-        u, g, y = e.left - r.left,
+        u, m, y = e.left - r.left,
         k = r.right - e.right,
         v = i.right - i.left,
         A = i.bottom - i.top;
-    if (l && y < Math.min(v, k) ? l = !1 : !l && k < Math.min(v, y) && (l = !0), v <= (l ? y : k)) u = Math.max(r.top, Math.min(t.top, r.bottom - A)) - e.top, g = Math.min(400, l ? y : k);
+    if (l && y < Math.min(v, k) ? l = !1 : !l && k < Math.min(v, y) && (l = !0), v <= (l ? y : k)) u = Math.max(r.top, Math.min(t.top, r.bottom - A)) - e.top, m = Math.min(400, l ? y : k);
     else {
-        h = !0, g = Math.min(400, (o ? e.right : r.right - e.left) - 30);
+        h = !0, m = Math.min(400, (o ? e.right : r.right - e.left) - 30);
         let F = r.bottom - e.bottom;
         F >= A || F > e.top ? u = t.bottom - e.top : (f = "bottom", u = e.bottom - t.top)
     }
     let O = (e.bottom - e.top) / s.offsetHeight,
         D = (e.right - e.left) / s.offsetWidth;
     return {
-        style: `${f}: ${u/O}px; max-width: ${g/D}px`,
+        style: `${f}: ${u/O}px; max-width: ${m/D}px`,
         class: "cm-completionInfo-" + (h ? o ? "left-narrow" : "right-narrow" : l ? "left" : "right")
     }
 }
 
 function Uk(n) {
     let e = n.addToOptions.slice();
     return n.icons && e.push({
@@ -17543,18 +17543,18 @@
         render(t, i, r, s) {
             let o = document.createElement("span");
             o.className = "cm-completionLabel";
             let l = t.displayLabel || t.label,
                 h = 0;
             for (let f = 0; f < s.length;) {
                 let u = s[f++],
-                    g = s[f++];
+                    m = s[f++];
                 u > h && o.appendChild(document.createTextNode(l.slice(h, u)));
                 let y = o.appendChild(document.createElement("span"));
-                y.appendChild(document.createTextNode(l.slice(u, g))), y.className = "cm-completionMatchedText", h = g
+                y.appendChild(document.createTextNode(l.slice(u, m))), y.className = "cm-completionMatchedText", h = m
             }
             return h < l.length && o.appendChild(document.createTextNode(l.slice(h))), o
         },
         position: 50
     }, {
         render(t) {
             if (!t.detail) return null;
@@ -17596,17 +17596,17 @@
                 selected: o
             } = r.open,
             l = e.state.facet(Ct);
         this.optionContent = Uk(l), this.optionClass = l.optionClass, this.tooltipClass = l.tooltipClass, this.range = wa(s.length, o, l.maxRenderedOptions), this.dom = document.createElement("div"), this.dom.className = "cm-tooltip-autocomplete", this.updateTooltipClass(e.state), this.dom.addEventListener("mousedown", h => {
             let {
                 options: f
             } = e.state.field(t).open;
-            for (let u = h.target, g; u && u != this.dom; u = u.parentNode)
-                if (u.nodeName == "LI" && (g = /-(\d+)$/.exec(u.id)) && +g[1] < f.length) {
-                    this.applyCompletion(e, f[+g[1]]), h.preventDefault();
+            for (let u = h.target, m; u && u != this.dom; u = u.parentNode)
+                if (u.nodeName == "LI" && (m = /-(\d+)$/.exec(u.id)) && +m[1] < f.length) {
+                    this.applyCompletion(e, f[+m[1]]), h.preventDefault();
                     return
                 }
         }), this.dom.addEventListener("focusout", h => {
             let f = e.state.field(this.stateField, !1);
             f && f.tooltip && e.state.facet(Ct).closeOnBlur && h.relatedTarget != e.contentDOM && e.dispatch({
                 effects: Ss.of(null)
             })
@@ -17719,16 +17719,16 @@
                     else {
                         let k = r.appendChild(document.createElement("completion-section"));
                         k.textContent = y
                     }
             }
             const u = r.appendChild(document.createElement("li"));
             u.id = t + "-" + o, u.setAttribute("role", "option");
-            let g = this.optionClass(l);
-            g && (u.className = g);
+            let m = this.optionClass(l);
+            m && (u.className = m);
             for (let y of this.optionContent) {
                 let k = y(l, this.view.state, this.view, h);
                 k && u.appendChild(k)
             }
         }
         return i.from && r.classList.add("cm-completionListIncompleteTop"), i.to < e.length && r.classList.add("cm-completionListIncompleteBottom"), r
     }
@@ -17762,45 +17762,45 @@
             t.push(h);
             let {
                 section: f
             } = h.completion;
             if (f) {
                 i || (i = []);
                 let u = typeof f == "string" ? f : f.name;
-                i.some(g => g.name == u) || i.push(typeof f == "string" ? {
+                i.some(m => m.name == u) || i.push(typeof f == "string" ? {
                     name: u
                 } : f)
             }
         };
     for (let h of n)
         if (h.hasResult()) {
             let f = h.result.getMatch;
             if (h.result.filter === !1)
                 for (let u of h.result.options) r(new au(u, h.source, f ? f(u) : [], 1e9 - t.length));
             else {
                 let u = new jk(e.sliceDoc(h.from, h.to));
-                for (let g of h.result.options)
-                    if (u.match(g.label)) {
-                        let y = g.displayLabel ? f ? f(g, u.matched) : [] : u.matched;
-                        r(new au(g, h.source, y, u.score + (g.boost || 0)))
+                for (let m of h.result.options)
+                    if (u.match(m.label)) {
+                        let y = m.displayLabel ? f ? f(m, u.matched) : [] : u.matched;
+                        r(new au(m, h.source, y, u.score + (m.boost || 0)))
                     }
             }
         } if (i) {
         let h = Object.create(null),
             f = 0,
-            u = (g, y) => {
+            u = (m, y) => {
                 var k, v;
-                return ((k = g.rank) !== null && k !== void 0 ? k : 1e9) - ((v = y.rank) !== null && v !== void 0 ? v : 1e9) || (g.name < y.name ? -1 : 1)
+                return ((k = m.rank) !== null && k !== void 0 ? k : 1e9) - ((v = y.rank) !== null && v !== void 0 ? v : 1e9) || (m.name < y.name ? -1 : 1)
             };
-        for (let g of i.sort(u)) f -= 1e5, h[g.name] = f;
-        for (let g of t) {
+        for (let m of i.sort(u)) f -= 1e5, h[m.name] = f;
+        for (let m of t) {
             let {
                 section: y
-            } = g.completion;
-            y && (g.score += h[typeof y == "string" ? y : y.name])
+            } = m.completion;
+            y && (m.score += h[typeof y == "string" ? y : y.name])
         }
     }
     let s = [],
         o = null,
         l = e.facet(Ct).compareCompletions;
     for (let h of t.sort((f, u) => u.score - f.score || l(f.completion, u.completion))) {
         let f = h.completion;
@@ -18734,22 +18734,22 @@
                 let k = Ar(n.state.field(Gt).diagnostics, e);
                 k && s.apply(n, k.from, k.to)
             },
             {
                 name: f
             } = s,
             u = r[o] ? f.indexOf(r[o]) : -1,
-            g = u < 0 ? f : [f.slice(0, u), $e("u", f.slice(u, u + 1)), f.slice(u + 1)];
+            m = u < 0 ? f : [f.slice(0, u), $e("u", f.slice(u, u + 1)), f.slice(u + 1)];
         return $e("button", {
             type: "button",
             class: "cm-diagnosticAction",
             onclick: h,
             onmousedown: h,
             "aria-label": ` Action: ${f}${u<0?"":` (access key "${r[o]})"`}.`
-        }, g)
+        }, m)
     }), e.source && $e("div", {
         class: "cm-diagnosticSource"
     }, e.source))
 }
 class Rw extends An {
     constructor(e) {
         super(), this.diagnostic = e
@@ -18821,17 +18821,17 @@
             selected: t
         } = this.view.state.field(Gt), i = 0, r = !1, s = null;
         for (e.between(0, this.view.state.doc.length, (o, l, {
                 spec: h
             }) => {
                 let f = -1,
                     u;
-                for (let g = i; g < this.items.length; g++)
-                    if (this.items[g].diagnostic == h.diagnostic) {
-                        f = g;
+                for (let m = i; m < this.items.length; m++)
+                    if (this.items[m].diagnostic == h.diagnostic) {
+                        f = m;
                         break
                     } f < 0 ? (u = new mu(this.view, h.diagnostic), this.items.splice(i, 0, u), r = !0) : (u = this.items[f], f > i && (this.items.splice(i, f - i), r = !0)), t && u.diagnostic == t.diagnostic ? u.dom.hasAttribute("aria-selected") || (u.dom.setAttribute("aria-selected", "true"), s = u) : u.dom.hasAttribute("aria-selected") && u.dom.removeAttribute("aria-selected"), i++
             }); i < this.items.length && !(this.items.length == 1 && this.items[0].diagnostic.from < 0);) r = !0, this.items.pop();
         this.items.length == 0 && (this.items.push(new mu(this.view, {
             from: -1,
             to: -1,
             severity: "info",
@@ -19016,16 +19016,16 @@
         } = n.field(Gt);
         return !e || !t || e.from == e.to ? de.none : de.set([Aw.range(e.from, e.to)])
     }), Pb(Tw, {
         hideOn: Sw
     }), Pw];
 var yu = {};
 class al {
-    constructor(e, t, i, r, s, o, l, h, f, u = 0, g) {
-        this.p = e, this.stack = t, this.state = i, this.reducePos = r, this.pos = s, this.score = o, this.buffer = l, this.bufferBase = h, this.curContext = f, this.lookAhead = u, this.parent = g
+    constructor(e, t, i, r, s, o, l, h, f, u = 0, m) {
+        this.p = e, this.stack = t, this.state = i, this.reducePos = r, this.pos = s, this.score = o, this.buffer = l, this.bufferBase = h, this.curContext = f, this.lookAhead = u, this.parent = m
     }
     toString() {
         return `[${this.stack.filter((e,t)=>t%3==0).concat(this.state)}]@${this.pos}${this.score?"!"+this.score:""}`
     }
     static start(e, t, i = 0) {
         let r = e.parser.context;
         return new al(e, [], t, i, i, 0, [], 0, r ? new bu(r, r.start) : null, 0, null)
@@ -19049,18 +19049,18 @@
             return
         }
         let l = this.stack.length - (i - 1) * 3 - (e & 262144 ? 6 : 0),
             h = l ? this.stack[l - 2] : this.p.ranges[0].from,
             f = this.reducePos - h;
         f >= 2e3 && !(!((t = this.p.parser.nodeSet.types[r]) === null || t === void 0) && t.isAnonymous) && (h == this.p.lastBigReductionStart ? (this.p.bigReductionCount++, this.p.lastBigReductionSize = f) : this.p.lastBigReductionSize < f && (this.p.bigReductionCount = 1, this.p.lastBigReductionStart = h, this.p.lastBigReductionSize = f));
         let u = l ? this.stack[l - 1] : 0,
-            g = this.bufferBase + this.buffer.length - u;
+            m = this.bufferBase + this.buffer.length - u;
         if (r < s.minRepeatTerm || e & 131072) {
             let y = s.stateFlag(this.state, 1) ? this.pos : this.reducePos;
-            this.storeNode(r, h, y, g + 4, !0)
+            this.storeNode(r, h, y, m + 4, !0)
         }
         if (e & 262144) this.state = this.stack[l];
         else {
             let y = this.stack[l - 3];
             this.state = s.getGoto(y, r, !0)
         }
         for (; this.stack.length > l;) this.stack.pop();
@@ -19446,27 +19446,27 @@
             if ((n[k + 1] & l) > 0) {
                 let v = n[k];
                 if (h.allows(v) && (e.token.value == -1 || e.token.value == v || Fw(v, e.token.value, r, s))) {
                     e.acceptToken(v);
                     break
                 }
             } let u = e.next,
-            g = 0,
+            m = 0,
             y = n[o + 2];
-        if (e.next < 0 && y > g && n[f + y * 3 - 3] == 65535) {
+        if (e.next < 0 && y > m && n[f + y * 3 - 3] == 65535) {
             o = n[f + y * 3 - 1];
             continue e
         }
-        for (; g < y;) {
-            let k = g + y >> 1,
+        for (; m < y;) {
+            let k = m + y >> 1,
                 v = f + k + (k << 1),
                 A = n[v],
                 O = n[v + 1] || 65536;
             if (u < A) y = k;
-            else if (u >= O) g = k + 1;
+            else if (u >= O) m = k + 1;
             else {
                 o = n[v + 2], e.advance();
                 continue e
             }
         }
         break
     }
@@ -19552,18 +19552,18 @@
             } = r,
             o = r.stateSlot(e.state, 3),
             l = e.curContext ? e.curContext.hash : 0,
             h = 0;
         for (let f = 0; f < s.length; f++) {
             if (!(1 << f & o)) continue;
             let u = s[f],
-                g = this.tokens[f];
-            if (!(i && !u.fallback) && ((u.contextual || g.start != e.pos || g.mask != o || g.context != l) && (this.updateCachedToken(g, u, e), g.mask = o, g.context = l), g.lookAhead > g.end + 25 && (h = Math.max(g.lookAhead, h)), g.value != 0)) {
+                m = this.tokens[f];
+            if (!(i && !u.fallback) && ((u.contextual || m.start != e.pos || m.mask != o || m.context != l) && (this.updateCachedToken(m, u, e), m.mask = o, m.context = l), m.lookAhead > m.end + 25 && (h = Math.max(m.lookAhead, h)), m.value != 0)) {
                 let y = t;
-                if (g.extended > -1 && (t = this.addActions(e, g.extended, g.end, t)), t = this.addActions(e, g.value, g.end, t), !u.extend && (i = g, t > y)) break
+                if (m.extended > -1 && (t = this.addActions(e, m.extended, m.end, t)), t = this.addActions(e, m.value, m.end, t), !u.extend && (i = m, t > y)) break
             }
         }
         for (; this.actions.length > t;) this.actions.pop();
         return h && e.setLookAhead(h), !i && e.pos == this.stream.end && (i = new _o, i.value = e.p.parser.eofTerm, i.start = i.end = e.pos, t = this.addActions(e, i.value, i.end, t)), this.mainToken = i, this.actions
     }
     getMainToken(e) {
         if (this.mainToken) return this.mainToken;
@@ -19695,36 +19695,36 @@
                 parser: s
             } = this,
             o = Wt ? this.stackID(e) + " -> " : "";
         if (this.stoppedAt != null && r > this.stoppedAt) return e.forceReduce() ? e : null;
         if (this.fragments) {
             let f = e.curContext && e.curContext.tracker.strict,
                 u = f ? e.curContext.hash : 0;
-            for (let g = this.fragments.nodeAt(r); g;) {
-                let y = this.parser.nodeSet.types[g.type.id] == g.type ? s.getGoto(e.state, g.type.id) : -1;
-                if (y > -1 && g.length && (!f || (g.prop(Se.contextHash) || 0) == u)) return e.useNode(g, y), Wt && console.log(o + this.stackID(e) + ` (via reuse of ${s.getName(g.type.id)})`), !0;
-                if (!(g instanceof Je) || g.children.length == 0 || g.positions[0] > 0) break;
-                let k = g.children[0];
-                if (k instanceof Je && g.positions[0] == 0) g = k;
+            for (let m = this.fragments.nodeAt(r); m;) {
+                let y = this.parser.nodeSet.types[m.type.id] == m.type ? s.getGoto(e.state, m.type.id) : -1;
+                if (y > -1 && m.length && (!f || (m.prop(Se.contextHash) || 0) == u)) return e.useNode(m, y), Wt && console.log(o + this.stackID(e) + ` (via reuse of ${s.getName(m.type.id)})`), !0;
+                if (!(m instanceof Je) || m.children.length == 0 || m.positions[0] > 0) break;
+                let k = m.children[0];
+                if (k instanceof Je && m.positions[0] == 0) m = k;
                 else break
             }
         }
         let l = s.stateSlot(e.state, 4);
         if (l > 0) return e.reduce(l), Wt && console.log(o + this.stackID(e) + ` (via always-reduce ${s.getName(l&65535)})`), !0;
         if (e.stack.length >= 8400)
             for (; e.stack.length > 6e3 && e.forceReduce(););
         let h = this.tokens.getActions(e);
         for (let f = 0; f < h.length;) {
             let u = h[f++],
-                g = h[f++],
+                m = h[f++],
                 y = h[f++],
                 k = f == h.length || !i,
                 v = k ? e : e.split(),
                 A = this.tokens.mainToken;
-            if (v.apply(u, g, A ? A.start : v.pos, y), Wt && console.log(o + this.stackID(v) + ` (via ${u&65536?`reduce of ${s.getName(u&65535)}`:"shift"} for ${s.getName(g)} @ ${r}${v==e?"":", split"})`), k) return !0;
+            if (v.apply(u, m, A ? A.start : v.pos, y), Wt && console.log(o + this.stackID(v) + ` (via ${u&65536?`reduce of ${s.getName(u&65535)}`:"shift"} for ${s.getName(m)} @ ${r}${v==e?"":", split"})`), k) return !0;
             v.pos > r ? t.push(v) : i.push(v)
         }
         return !1
     }
     advanceFully(e, t) {
         let i = e.pos;
         for (;;) {
@@ -19737,17 +19737,17 @@
             s = !1;
         for (let o = 0; o < e.length; o++) {
             let l = e[o],
                 h = t[o << 1],
                 f = t[(o << 1) + 1],
                 u = Wt ? this.stackID(l) + " -> " : "";
             if (l.deadEnd && (s || (s = !0, l.restart(), Wt && console.log(u + this.stackID(l) + " (restarted)"), this.advanceFully(l, i)))) continue;
-            let g = l.split(),
+            let m = l.split(),
                 y = u;
-            for (let k = 0; g.forceReduce() && k < 10 && (Wt && console.log(y + this.stackID(g) + " (via force-reduce)"), !this.advanceFully(g, i)); k++) Wt && (y = this.stackID(g) + " -> ");
+            for (let k = 0; m.forceReduce() && k < 10 && (Wt && console.log(y + this.stackID(m) + " (via force-reduce)"), !this.advanceFully(m, i)); k++) Wt && (y = this.stackID(m) + " -> ");
             for (let k of l.recoverByInsert(h)) Wt && console.log(u + this.stackID(k) + " (via recover-insert)"), this.advanceFully(k, i);
             this.stream.end > l.pos ? (f == l.pos && (f++, h = 0), l.recoverByDelete(h, f), Wt && console.log(u + this.stackID(l) + ` (via recover-delete ${this.parser.getName(h)})`), vu(l, i)) : (!r || r.score < l.score) && (r = l)
         }
         return r
     }
     stackToTree(e) {
         return e.close(), Je.build({
@@ -19802,16 +19802,16 @@
             for (let l of e.nodeProps) {
                 let h = l[0];
                 typeof h == "string" && (h = Se[h]);
                 for (let f = 1; f < l.length;) {
                     let u = l[f++];
                     if (u >= 0) s(u, h, l[f++]);
                     else {
-                        let g = l[f + -u];
-                        for (let y = -u; y > 0; y--) s(l[f++], h, g);
+                        let m = l[f + -u];
+                        for (let y = -u; y > 0; y--) s(l[f++], h, m);
                         f++
                     }
                 }
             }
         this.nodeSet = new qh(t.map((l, h) => Ht.define({
             name: h >= this.minRepeatTerm ? void 0 : l,
             id: h,
@@ -20308,31 +20308,31 @@
 
 function Cv(n, e, t, i, r, s) {
     var o;
     let l = new lc,
         h = ((o = s == null ? void 0 : s.spec.identifierQuotes) === null || o === void 0 ? void 0 : o[0]) || '"',
         f = l.child(r || "", h);
     for (let u in n) {
-        let g = u.replace(/\\?\./g, k => k == "." ? "\0" : k).split("\0"),
-            y = g.length == 1 ? f : l;
-        for (let k of g) y = y.child(k.replace(/\\\./g, "."), h);
+        let m = u.replace(/\\?\./g, k => k == "." ? "\0" : k).split("\0"),
+            y = m.length == 1 ? f : l;
+        for (let k of m) y = y.child(k.replace(/\\\./g, "."), h);
         for (let k of n[u]) k && y.list.push(typeof k == "string" ? Kg(k, "property", h) : k)
     }
     return e && f.addCompletions(e), t && l.addCompletions(t), l.addCompletions(f.list), i && l.addCompletions(f.child(i, h).list), u => {
         let {
-            parents: g,
+            parents: m,
             from: y,
             quoted: k,
             empty: v,
             aliases: A
         } = bv(u.state, u.pos);
         if (v && !u.explicit) return null;
-        A && g.length == 1 && (g = A[g[0]] || g);
+        A && m.length == 1 && (m = A[m[0]] || m);
         let O = l;
-        for (let $ of g) {
+        for (let $ of m) {
             for (; !O.children || !O.children[$];)
                 if (O == l) O = f;
                 else if (O == f && i) O = O.child(i, h);
             else return null;
             O = O.child($, h)
         }
         let D = k && u.state.sliceDoc(u.pos, u.pos + 1) == k,
@@ -20720,39 +20720,39 @@
             let l = "",
                 h = "",
                 f = !1;
             for (; e;) {
                 let u = !1;
                 if (!(t = o.exec(e)) || this.rules.block.hr.test(e)) break;
                 l = t[0], e = e.substring(l.length);
-                let g = t[2].split(`
+                let m = t[2].split(`
 `, 1)[0].replace(/^\t+/, D => " ".repeat(3 * D.length)),
                     y = e.split(`
 `, 1)[0],
                     k = 0;
-                this.options.pedantic ? (k = 2, h = g.trimStart()) : (k = t[2].search(/[^ ]/), k = k > 4 ? 1 : k, h = g.slice(k), k += t[1].length);
+                this.options.pedantic ? (k = 2, h = m.trimStart()) : (k = t[2].search(/[^ ]/), k = k > 4 ? 1 : k, h = m.slice(k), k += t[1].length);
                 let v = !1;
-                if (!g && /^ *$/.test(y) && (l += y + `
+                if (!m && /^ *$/.test(y) && (l += y + `
 `, e = e.substring(y.length + 1), u = !0), !u) {
                     const D = new RegExp(`^ {0,${Math.min(3,k-1)}}(?:[*+-]|\\d{1,9}[.)])((?:[ 	][^\\n]*)?(?:\\n|$))`),
                         F = new RegExp(`^ {0,${Math.min(3,k-1)}}((?:- *){3,}|(?:_ *){3,}|(?:\\* *){3,})(?:\\n+|$)`),
                         $ = new RegExp(`^ {0,${Math.min(3,k-1)}}(?:\`\`\`|~~~)`),
                         j = new RegExp(`^ {0,${Math.min(3,k-1)}}#`);
                     for (; e;) {
                         const z = e.split(`
 `, 1)[0];
                         if (y = z, this.options.pedantic && (y = y.replace(/^ {1,4}(?=( {4})*[^ ])/g, "  ")), $.test(y) || j.test(y) || D.test(y) || F.test(e)) break;
                         if (y.search(/[^ ]/) >= k || !y.trim()) h += `
 ` + y.slice(k);
                         else {
-                            if (v || g.search(/[^ ]/) >= 4 || $.test(g) || j.test(g) || F.test(g)) break;
+                            if (v || m.search(/[^ ]/) >= 4 || $.test(m) || j.test(m) || F.test(m)) break;
                             h += `
 ` + y
                         }!v && !y.trim() && (v = !0), l += z + `
-`, e = e.substring(z.length + 1), g = y.slice(k)
+`, e = e.substring(z.length + 1), m = y.slice(k)
                     }
                 }
                 s.loose || (f ? s.loose = !0 : /\n *\n *$/.test(l) && (f = !0));
                 let A = null,
                     O;
                 this.options.gfm && (A = /^\[[ xX]\] /.exec(h), A && (O = A[0] !== "[ ] ", h = h.replace(/^\[[ xX]\] +/, ""))), s.items.push({
                     type: "list_item",
@@ -20763,16 +20763,16 @@
                     text: h,
                     tokens: []
                 }), s.raw += l
             }
             s.items[s.items.length - 1].raw = l.trimEnd(), s.items[s.items.length - 1].text = h.trimEnd(), s.raw = s.raw.trimEnd();
             for (let u = 0; u < s.items.length; u++)
                 if (this.lexer.state.top = !1, s.items[u].tokens = this.lexer.blockTokens(s.items[u].text, []), !s.loose) {
-                    const g = s.items[u].tokens.filter(k => k.type === "space"),
-                        y = g.length > 0 && g.some(k => /\n.*\n/.test(k.raw));
+                    const m = s.items[u].tokens.filter(k => k.type === "space"),
+                        y = m.length > 0 && m.some(k => /\n.*\n/.test(k.raw));
                     s.loose = y
                 } if (s.loose)
                 for (let u = 0; u < s.items.length; u++) s.items[u].loose = !0;
             return s
         }
     }
     html(e) {
@@ -20924,17 +20924,17 @@
     emStrong(e, t, i = "") {
         let r = this.rules.inline.emStrongLDelim.exec(e);
         if (!r || r[3] && i.match(/[\p{L}\p{N}]/u)) return;
         if (!(r[1] || r[2] || "") || !i || this.rules.inline.punctuation.exec(i)) {
             const o = [...r[0]].length - 1;
             let l, h, f = o,
                 u = 0;
-            const g = r[0][0] === "*" ? this.rules.inline.emStrongRDelimAst : this.rules.inline.emStrongRDelimUnd;
-            for (g.lastIndex = 0, t = t.slice(-1 * e.length + o);
-                (r = g.exec(t)) != null;) {
+            const m = r[0][0] === "*" ? this.rules.inline.emStrongRDelimAst : this.rules.inline.emStrongRDelimUnd;
+            for (m.lastIndex = 0, t = t.slice(-1 * e.length + o);
+                (r = m.exec(t)) != null;) {
                 if (l = r[1] || r[2] || r[3] || r[4] || r[5] || r[6], !l) continue;
                 if (h = [...l].length, r[3] || r[4]) {
                     f += h;
                     continue
                 } else if ((r[5] || r[6]) && o % 3 && !((o + h) % 3)) {
                     u += h;
                     continue
@@ -21346,20 +21346,20 @@
                 }
                 if (!this.state.inLink && (i = this.tokenizer.url(e))) {
                     e = e.substring(i.raw.length), t.push(i);
                     continue
                 }
                 if (s = e, this.options.extensions && this.options.extensions.startInline) {
                     let u = 1 / 0;
-                    const g = e.slice(1);
+                    const m = e.slice(1);
                     let y;
                     this.options.extensions.startInline.forEach(k => {
                         y = k.call({
                             lexer: this
-                        }, g), typeof y == "number" && y >= 0 && (u = Math.min(u, y))
+                        }, m), typeof y == "number" && y >= 0 && (u = Math.min(u, y))
                     }), u < 1 / 0 && u >= 0 && (s = e.substring(0, u + 1))
                 }
                 if (i = this.tokenizer.inlineText(s)) {
                     e = e.substring(i.raw.length), i.raw.slice(-1) !== "_" && (f = i.raw.slice(-1)), h = !0, r = t[t.length - 1], r && r.type === "text" ? (r.raw += i.raw, r.text += i.text) : t.push(i);
                     continue
                 }
                 if (e) {
@@ -21549,17 +21549,17 @@
                     for (let u = 0; u < o.header.length; u++) h += this.renderer.tablecell(this.parseInline(o.header[u].tokens), {
                         header: !0,
                         align: o.align[u]
                     });
                     l += this.renderer.tablerow(h);
                     let f = "";
                     for (let u = 0; u < o.rows.length; u++) {
-                        const g = o.rows[u];
+                        const m = o.rows[u];
                         h = "";
-                        for (let y = 0; y < g.length; y++) h += this.renderer.tablecell(this.parseInline(g[y].tokens), {
+                        for (let y = 0; y < m.length; y++) h += this.renderer.tablecell(this.parseInline(m[y].tokens), {
                             header: !1,
                             align: o.align[y]
                         });
                         f += this.renderer.tablerow(h)
                     }
                     i += this.renderer.table(l, f);
                     continue
@@ -21572,16 +21572,16 @@
                 }
                 case "list": {
                     const o = s,
                         l = o.ordered,
                         h = o.start,
                         f = o.loose;
                     let u = "";
-                    for (let g = 0; g < o.items.length; g++) {
-                        const y = o.items[g],
+                    for (let m = 0; m < o.items.length; m++) {
+                        const y = o.items[m],
                             k = y.checked,
                             v = y.task;
                         let A = "";
                         if (y.task) {
                             const O = this.renderer.checkbox(!!k);
                             f ? y.tokens.length > 0 && y.tokens[0].type === "paragraph" ? (y.tokens[0].text = O + " " + y.tokens[0].text, y.tokens[0].tokens && y.tokens[0].tokens.length > 0 && y.tokens[0].tokens[0].type === "text" && (y.tokens[0].tokens[0].text = O + " " + y.tokens[0].tokens[0].text)) : y.tokens.unshift({
                                 type: "text",
@@ -21779,50 +21779,50 @@
                 for (const o in i.renderer) {
                     if (!(o in s)) throw new Error(`renderer '${o}' does not exist`);
                     if (o === "options") continue;
                     const l = o,
                         h = i.renderer[l],
                         f = s[l];
                     s[l] = (...u) => {
-                        let g = h.apply(s, u);
-                        return g === !1 && (g = f.apply(s, u)), g || ""
+                        let m = h.apply(s, u);
+                        return m === !1 && (m = f.apply(s, u)), m || ""
                     }
                 }
                 r.renderer = s
             }
             if (i.tokenizer) {
                 const s = this.defaults.tokenizer || new ul(this.defaults);
                 for (const o in i.tokenizer) {
                     if (!(o in s)) throw new Error(`tokenizer '${o}' does not exist`);
                     if (["options", "rules", "lexer"].includes(o)) continue;
                     const l = o,
                         h = i.tokenizer[l],
                         f = s[l];
                     s[l] = (...u) => {
-                        let g = h.apply(s, u);
-                        return g === !1 && (g = f.apply(s, u)), g
+                        let m = h.apply(s, u);
+                        return m === !1 && (m = f.apply(s, u)), m
                     }
                 }
                 r.tokenizer = s
             }
             if (i.hooks) {
                 const s = this.defaults.hooks || new hs;
                 for (const o in i.hooks) {
                     if (!(o in s)) throw new Error(`hook '${o}' does not exist`);
                     if (o === "options") continue;
                     const l = o,
                         h = i.hooks[l],
                         f = s[l];
                     hs.passThroughHooks.has(o) ? s[l] = u => {
                         if (this.defaults.async) return Promise.resolve(h.call(s, u)).then(y => f.call(s, y));
-                        const g = h.call(s, u);
-                        return f.call(s, g)
+                        const m = h.call(s, u);
+                        return f.call(s, m)
                     } : s[l] = (...u) => {
-                        let g = h.apply(s, u);
-                        return g === !1 && (g = f.apply(s, u)), g
+                        let m = h.apply(s, u);
+                        return m === !1 && (m = f.apply(s, u)), m
                     }
                 }
                 r.hooks = s
             }
             if (i.walkTokens) {
                 const s = this.defaults.walkTokens,
                     o = i.walkTokens;
@@ -22068,15 +22068,15 @@
         {
             DocumentFragment: s,
             HTMLTemplateElement: o,
             Node: l,
             Element: h,
             NodeFilter: f,
             NamedNodeMap: u = n.NamedNodeMap || n.MozNamedAttrMap,
-            HTMLFormElement: g,
+            HTMLFormElement: m,
             DOMParser: y,
             trustedTypes: k
         } = n,
         v = h.prototype,
         A = To(v, "cloneNode"),
         O = To(v, "nextSibling"),
         D = To(v, "childNodes"),
@@ -22249,15 +22249,15 @@
             const Ke = V.body || V.documentElement;
             return R && Y && Ke.insertBefore(t.createTextNode(Y), Ke.childNodes[0] || null), Jt === Yt ? he.call(V, zi ? "html" : "body")[0] : zi ? V.documentElement : Ke
         },
         ir = function(R) {
             return G.call(R.ownerDocument || R, R, f.SHOW_ELEMENT | f.SHOW_COMMENT | f.SHOW_TEXT, null)
         },
         nr = function(R) {
-            return R instanceof g && (typeof R.nodeName != "string" || typeof R.textContent != "string" || typeof R.removeChild != "function" || !(R.attributes instanceof u) || typeof R.removeAttribute != "function" || typeof R.setAttribute != "function" || typeof R.namespaceURI != "string" || typeof R.insertBefore != "function" || typeof R.hasChildNodes != "function")
+            return R instanceof m && (typeof R.nodeName != "string" || typeof R.textContent != "string" || typeof R.removeChild != "function" || !(R.attributes instanceof u) || typeof R.removeAttribute != "function" || typeof R.setAttribute != "function" || typeof R.namespaceURI != "string" || typeof R.insertBefore != "function" || typeof R.hasChildNodes != "function")
         },
         $s = function(R) {
             return typeof l == "function" && R instanceof l
         },
         hi = function(R, V, Y) {
             ae[R] && Ao(ae[R], Re => {
                 Re.call(e, V, Y, tn)
@@ -22425,40 +22425,54 @@
 var IS = um();
 
 function dm() {
     const n = document.querySelector(".alert-danger.db-error");
     return n ? n.textContent.trim() : null
 }
 
-function BS(n = !1) {
+function BS() {
+    document.getElementById("search_assistant_tables").focus()
+}
+
+function _S(n = !1) {
     const e = dm();
     if (n || e) {
-        const i = document.getElementById("assistant_collapse");
-        new Zm(i, {
+        const l = document.getElementById("assistant_collapse");
+        new Zm(l, {
             toggle: !1
         }).show(), e && document.getElementById("id_error_help_message").classList.remove("d-none")
-    } [...document.querySelectorAll('[data-bs-toggle="tooltip"]')].map(i => new e0(i)), fetch("../schema.json/" + Te("#id_connection").val()).then(i => i.json()).then(i => {
-        const r = Object.keys(i),
-            s = document.getElementById("table-list");
-        s.innerHTML = "", r.forEach((l, h) => {
-            const f = document.createElement("div");
-            f.className = "form-check";
-            const u = document.createElement("input");
-            u.className = "form-check-input table-checkbox", u.type = "checkbox", u.value = l, u.id = "flexCheckDefault" + h;
-            const g = document.createElement("label");
-            g.className = "form-check-label", g.setAttribute("for", u.id), g.textContent = l, f.appendChild(u), f.appendChild(g), s.appendChild(f)
+    } [...document.querySelectorAll('[data-bs-toggle="tooltip"]')].map(l => new e0(l)), fetch("../schema.json/" + Te("#id_connection").val()).then(l => l.json()).then(l => {
+        const h = Object.keys(l),
+            f = document.getElementById("table-list");
+        f.innerHTML = "", h.forEach((m, y) => {
+            const k = document.createElement("div");
+            k.className = "form-check";
+            const v = document.createElement("input");
+            v.className = "form-check-input table-checkbox", v.type = "checkbox", v.value = m, v.id = "flexCheckDefault" + y;
+            const A = document.createElement("label");
+            A.className = "form-check-label", A.setAttribute("for", v.id), A.textContent = m, k.appendChild(v), k.appendChild(A), f.appendChild(k)
         });
-        let o = {
+        let u = {
             valueNames: ["form-check-label"]
         };
-        new Vu("additional_table_container", o)
-    }).catch(i => {
-        console.error("Error retrieving JSON schema:", i)
-    }), document.getElementById("id_assistant_input").addEventListener("keydown", function(i) {
-        (i.ctrlKey || i.metaKey) && i.key === "Enter" && (i.preventDefault(), ju())
+        new Vu("additional_table_container", u)
+    }).catch(l => {
+        console.error("Error retrieving JSON schema:", l)
+    });
+    const i = document.getElementById("include_other_tables"),
+        r = document.getElementById("additional_table_container"),
+        s = document.getElementById("assistant_input_wrapper");
+
+    function o(l) {
+        l ? (r.classList.remove("d-none"), s.classList.remove("col-12"), s.classList.add("col-9"), BS()) : (r.classList.add("d-none"), s.classList.remove("col-9"), s.classList.add("col-12"))
+    }
+    i.addEventListener("change", function() {
+        o(this.checked)
+    }), o(i.checked), document.getElementById("id_assistant_input").addEventListener("keydown", function(l) {
+        (l.ctrlKey || l.metaKey) && l.key === "Enter" && (l.preventDefault(), ju())
     }), document.getElementById("ask_assistant_btn").addEventListener("click", ju)
 }
 
 function ju() {
     var t, i, r, s, o, l;
     const n = Array.from(document.querySelectorAll(".table-checkbox:checked")).map(h => h.value),
         e = {
@@ -22476,21 +22490,21 @@
         },
         body: JSON.stringify(e)
     }).then(h => {
         if (!h.ok) throw new Error("Network response was not ok");
         return h.json()
     }).then(h => {
         const f = IS.sanitize(Ne.parse(h.message));
-        document.getElementById("assistant_response").innerHTML = f, document.getElementById("assistant_spinner").classList.add("d-none"), _S()
+        document.getElementById("assistant_response").innerHTML = f, document.getElementById("assistant_spinner").classList.add("d-none"), HS()
     }).catch(h => {
         console.error("Error:", h)
     })
 }
 
-function _S() {
+function HS() {
     document.querySelectorAll("#assistant_response pre").forEach(n => {
         const e = document.createElement("i");
         e.classList.add("copy-btn"), e.classList.add("bi-copy");
         const t = document.createElement("span");
         t.textContent = "Copied!", t.style.display = "none", t.style.marginLeft = "8px", e.appendChild(t), n.appendChild(e), e.addEventListener("click", function() {
             const i = this.parentNode.firstElementChild.innerText;
             navigator.clipboard.writeText(i).then(() => {
@@ -22500,34 +22514,34 @@
             }).catch(r => {
                 console.error("Error in copying text: ", r)
             })
         })
     })
 }
 
-function HS(n) {
+function FS(n) {
     let e = new te({
         doc: n.value,
         extensions: [Iv]
     });
     return n.parentNode.insertBefore(e.dom, n), n.style.display = "none", n.form && n.form.addEventListener("submit", () => {
         n.value = e.state.doc.toString()
     }), e
 }
-class VS {
+class US {
     constructor(e) {
         ze(this, "handleBeforeUnload", e => {
             if (clientRoute === "query_detail" && this.docChanged) {
                 const t = "You have unsaved changes to your query.";
                 return e.returnValue = t, t
             }
         });
         const t = document.getElementById("assistant_accordion"),
             i = document.getElementById("nav-preview");
-        t && BS(!i && e === "new"), this.queryId = e, this.$rows = Te("#rows"), this.$form = Te("form"), this.$snapshotField = Te("#id_snapshot"), this.docChanged = !1, this.$submit = Te("#refresh_play_button, #save_button"), this.$submit.length || (this.$submit = Te("#refresh_button")), this.editor = HS(document.getElementById("id_sql")), window.editor = this.editor, document.addEventListener("submitEventFromCM", r => {
+        t && _S(!i && e === "new"), this.queryId = e, this.$rows = Te("#rows"), this.$form = Te("form"), this.$snapshotField = Te("#id_snapshot"), this.docChanged = !1, this.$submit = Te("#refresh_play_button, #save_button"), this.$submit.length || (this.$submit = Te("#refresh_button")), this.editor = FS(document.getElementById("id_sql")), window.editor = this.editor, document.addEventListener("submitEventFromCM", r => {
             this.$submit.click()
         }), document.addEventListener("docChanged", r => {
             this.docChanged = !0
         }), this.bind(), Jl.get("schema_sidebar_open") === "true" && this.showSchema(!0)
     }
     getParams() {
         let e = !1;
@@ -22664,15 +22678,15 @@
             }))
         }), r)).catch(r => {
             console.error("Error retrieving JSON schema:", r)
         })
     }
 }
 export {
-    VS as ExplorerEditor
+    US as ExplorerEditor
 };
 
 function __vite__mapDeps(indexes) {
     if (!__vite__mapDeps.viteFileDeps) {
         __vite__mapDeps.viteFileDeps = ["./pivot-setup.js", "./main.js", "./index.js", "./favorites.js"]
     }
     return indexes.map((i) => __vite__mapDeps.viteFileDeps[i])
```

### Comparing `django_sql_explorer-4.2/explorer/static/explorer/favorites.js` & `django_sql_explorer-4.2b1/explorer/static/explorer/favorites.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/static/explorer/index.js` & `django_sql_explorer-4.2b1/explorer/static/explorer/index.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/static/explorer/main.js` & `django_sql_explorer-4.2b1/explorer/static/explorer/main.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/static/explorer/pivot-setup.js` & `django_sql_explorer-4.2b1/explorer/static/explorer/pivot-setup.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/static/explorer/query-list.js` & `django_sql_explorer-4.2b1/explorer/static/explorer/query-list.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/static/explorer/schema.js` & `django_sql_explorer-4.2b1/explorer/static/explorer/schema.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/static/explorer/styles.css` & `django_sql_explorer-4.2b1/explorer/static/explorer/styles.css`

 * *Files 0% similar despite different names*

```diff
@@ -2,8 +2,8 @@
  * Bootstrap  v5.3.2 (https://getbootstrap.com/)
  * Copyright 2011-2023 The Bootstrap Authors
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE)
  *//*!
  * Bootstrap Icons v1.11.2 (https://icons.getbootstrap.com/)
  * Copyright 2019-2023 The Bootstrap Authors
  * Licensed under MIT (https://github.com/twbs/icons/blob/main/LICENSE)
- */@font-face{font-display:block;font-family:bootstrap-icons;src:url(./bootstrap-icons.woff2?7141511ac37f13e1a387fb9fc6646256) format("woff2"),url(./bootstrap-icons.woff?7141511ac37f13e1a387fb9fc6646256) format("woff")}.bi:before,[class^=bi-]:before,[class*=" bi-"]:before{display:inline-block;font-family:bootstrap-icons!important;font-style:normal;font-weight:400!important;font-variant:normal;text-transform:none;line-height:1;vertical-align:-.125em;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.bi-123:before{content:""}.bi-alarm-fill:before{content:""}.bi-alarm:before{content:""}.bi-align-bottom:before{content:""}.bi-align-center:before{content:""}.bi-align-end:before{content:""}.bi-align-middle:before{content:""}.bi-align-start:before{content:""}.bi-align-top:before{content:""}.bi-alt:before{content:""}.bi-app-indicator:before{content:""}.bi-app:before{content:""}.bi-archive-fill:before{content:""}.bi-archive:before{content:""}.bi-arrow-90deg-down:before{content:""}.bi-arrow-90deg-left:before{content:""}.bi-arrow-90deg-right:before{content:""}.bi-arrow-90deg-up:before{content:""}.bi-arrow-bar-down:before{content:""}.bi-arrow-bar-left:before{content:""}.bi-arrow-bar-right:before{content:""}.bi-arrow-bar-up:before{content:""}.bi-arrow-clockwise:before{content:""}.bi-arrow-counterclockwise:before{content:""}.bi-arrow-down-circle-fill:before{content:""}.bi-arrow-down-circle:before{content:""}.bi-arrow-down-left-circle-fill:before{content:""}.bi-arrow-down-left-circle:before{content:""}.bi-arrow-down-left-square-fill:before{content:""}.bi-arrow-down-left-square:before{content:""}.bi-arrow-down-left:before{content:""}.bi-arrow-down-right-circle-fill:before{content:""}.bi-arrow-down-right-circle:before{content:""}.bi-arrow-down-right-square-fill:before{content:""}.bi-arrow-down-right-square:before{content:""}.bi-arrow-down-right:before{content:""}.bi-arrow-down-short:before{content:""}.bi-arrow-down-square-fill:before{content:""}.bi-arrow-down-square:before{content:""}.bi-arrow-down-up:before{content:""}.bi-arrow-down:before{content:""}.bi-arrow-left-circle-fill:before{content:""}.bi-arrow-left-circle:before{content:""}.bi-arrow-left-right:before{content:""}.bi-arrow-left-short:before{content:""}.bi-arrow-left-square-fill:before{content:""}.bi-arrow-left-square:before{content:""}.bi-arrow-left:before{content:""}.bi-arrow-repeat:before{content:""}.bi-arrow-return-left:before{content:""}.bi-arrow-return-right:before{content:""}.bi-arrow-right-circle-fill:before{content:""}.bi-arrow-right-circle:before{content:""}.bi-arrow-right-short:before{content:""}.bi-arrow-right-square-fill:before{content:""}.bi-arrow-right-square:before{content:""}.bi-arrow-right:before{content:""}.bi-arrow-up-circle-fill:before{content:""}.bi-arrow-up-circle:before{content:""}.bi-arrow-up-left-circle-fill:before{content:""}.bi-arrow-up-left-circle:before{content:""}.bi-arrow-up-left-square-fill:before{content:""}.bi-arrow-up-left-square:before{content:""}.bi-arrow-up-left:before{content:""}.bi-arrow-up-right-circle-fill:before{content:""}.bi-arrow-up-right-circle:before{content:""}.bi-arrow-up-right-square-fill:before{content:""}.bi-arrow-up-right-square:before{content:""}.bi-arrow-up-right:before{content:""}.bi-arrow-up-short:before{content:""}.bi-arrow-up-square-fill:before{content:""}.bi-arrow-up-square:before{content:""}.bi-arrow-up:before{content:""}.bi-arrows-angle-contract:before{content:""}.bi-arrows-angle-expand:before{content:""}.bi-arrows-collapse:before{content:""}.bi-arrows-expand:before{content:""}.bi-arrows-fullscreen:before{content:""}.bi-arrows-move:before{content:""}.bi-aspect-ratio-fill:before{content:""}.bi-aspect-ratio:before{content:""}.bi-asterisk:before{content:""}.bi-at:before{content:""}.bi-award-fill:before{content:""}.bi-award:before{content:""}.bi-back:before{content:""}.bi-backspace-fill:before{content:""}.bi-backspace-reverse-fill:before{content:""}.bi-backspace-reverse:before{content:""}.bi-backspace:before{content:""}.bi-badge-3d-fill:before{content:""}.bi-badge-3d:before{content:""}.bi-badge-4k-fill:before{content:""}.bi-badge-4k:before{content:""}.bi-badge-8k-fill:before{content:""}.bi-badge-8k:before{content:""}.bi-badge-ad-fill:before{content:""}.bi-badge-ad:before{content:""}.bi-badge-ar-fill:before{content:""}.bi-badge-ar:before{content:""}.bi-badge-cc-fill:before{content:""}.bi-badge-cc:before{content:""}.bi-badge-hd-fill:before{content:""}.bi-badge-hd:before{content:""}.bi-badge-tm-fill:before{content:""}.bi-badge-tm:before{content:""}.bi-badge-vo-fill:before{content:""}.bi-badge-vo:before{content:""}.bi-badge-vr-fill:before{content:""}.bi-badge-vr:before{content:""}.bi-badge-wc-fill:before{content:""}.bi-badge-wc:before{content:""}.bi-bag-check-fill:before{content:""}.bi-bag-check:before{content:""}.bi-bag-dash-fill:before{content:""}.bi-bag-dash:before{content:""}.bi-bag-fill:before{content:""}.bi-bag-plus-fill:before{content:""}.bi-bag-plus:before{content:""}.bi-bag-x-fill:before{content:""}.bi-bag-x:before{content:""}.bi-bag:before{content:""}.bi-bar-chart-fill:before{content:""}.bi-bar-chart-line-fill:before{content:""}.bi-bar-chart-line:before{content:""}.bi-bar-chart-steps:before{content:""}.bi-bar-chart:before{content:""}.bi-basket-fill:before{content:""}.bi-basket:before{content:""}.bi-basket2-fill:before{content:""}.bi-basket2:before{content:""}.bi-basket3-fill:before{content:""}.bi-basket3:before{content:""}.bi-battery-charging:before{content:""}.bi-battery-full:before{content:""}.bi-battery-half:before{content:""}.bi-battery:before{content:""}.bi-bell-fill:before{content:""}.bi-bell:before{content:""}.bi-bezier:before{content:""}.bi-bezier2:before{content:""}.bi-bicycle:before{content:""}.bi-binoculars-fill:before{content:""}.bi-binoculars:before{content:""}.bi-blockquote-left:before{content:""}.bi-blockquote-right:before{content:""}.bi-book-fill:before{content:""}.bi-book-half:before{content:""}.bi-book:before{content:""}.bi-bookmark-check-fill:before{content:""}.bi-bookmark-check:before{content:""}.bi-bookmark-dash-fill:before{content:""}.bi-bookmark-dash:before{content:""}.bi-bookmark-fill:before{content:""}.bi-bookmark-heart-fill:before{content:""}.bi-bookmark-heart:before{content:""}.bi-bookmark-plus-fill:before{content:""}.bi-bookmark-plus:before{content:""}.bi-bookmark-star-fill:before{content:""}.bi-bookmark-star:before{content:""}.bi-bookmark-x-fill:before{content:""}.bi-bookmark-x:before{content:""}.bi-bookmark:before{content:""}.bi-bookmarks-fill:before{content:""}.bi-bookmarks:before{content:""}.bi-bookshelf:before{content:""}.bi-bootstrap-fill:before{content:""}.bi-bootstrap-reboot:before{content:""}.bi-bootstrap:before{content:""}.bi-border-all:before{content:""}.bi-border-bottom:before{content:""}.bi-border-center:before{content:""}.bi-border-inner:before{content:""}.bi-border-left:before{content:""}.bi-border-middle:before{content:""}.bi-border-outer:before{content:""}.bi-border-right:before{content:""}.bi-border-style:before{content:""}.bi-border-top:before{content:""}.bi-border-width:before{content:""}.bi-border:before{content:""}.bi-bounding-box-circles:before{content:""}.bi-bounding-box:before{content:""}.bi-box-arrow-down-left:before{content:""}.bi-box-arrow-down-right:before{content:""}.bi-box-arrow-down:before{content:""}.bi-box-arrow-in-down-left:before{content:""}.bi-box-arrow-in-down-right:before{content:""}.bi-box-arrow-in-down:before{content:""}.bi-box-arrow-in-left:before{content:""}.bi-box-arrow-in-right:before{content:""}.bi-box-arrow-in-up-left:before{content:""}.bi-box-arrow-in-up-right:before{content:""}.bi-box-arrow-in-up:before{content:""}.bi-box-arrow-left:before{content:""}.bi-box-arrow-right:before{content:""}.bi-box-arrow-up-left:before{content:""}.bi-box-arrow-up-right:before{content:""}.bi-box-arrow-up:before{content:""}.bi-box-seam:before{content:""}.bi-box:before{content:""}.bi-braces:before{content:""}.bi-bricks:before{content:""}.bi-briefcase-fill:before{content:""}.bi-briefcase:before{content:""}.bi-brightness-alt-high-fill:before{content:""}.bi-brightness-alt-high:before{content:""}.bi-brightness-alt-low-fill:before{content:""}.bi-brightness-alt-low:before{content:""}.bi-brightness-high-fill:before{content:""}.bi-brightness-high:before{content:""}.bi-brightness-low-fill:before{content:""}.bi-brightness-low:before{content:""}.bi-broadcast-pin:before{content:""}.bi-broadcast:before{content:""}.bi-brush-fill:before{content:""}.bi-brush:before{content:""}.bi-bucket-fill:before{content:""}.bi-bucket:before{content:""}.bi-bug-fill:before{content:""}.bi-bug:before{content:""}.bi-building:before{content:""}.bi-bullseye:before{content:""}.bi-calculator-fill:before{content:""}.bi-calculator:before{content:""}.bi-calendar-check-fill:before{content:""}.bi-calendar-check:before{content:""}.bi-calendar-date-fill:before{content:""}.bi-calendar-date:before{content:""}.bi-calendar-day-fill:before{content:""}.bi-calendar-day:before{content:""}.bi-calendar-event-fill:before{content:""}.bi-calendar-event:before{content:""}.bi-calendar-fill:before{content:""}.bi-calendar-minus-fill:before{content:""}.bi-calendar-minus:before{content:""}.bi-calendar-month-fill:before{content:""}.bi-calendar-month:before{content:""}.bi-calendar-plus-fill:before{content:""}.bi-calendar-plus:before{content:""}.bi-calendar-range-fill:before{content:""}.bi-calendar-range:before{content:""}.bi-calendar-week-fill:before{content:""}.bi-calendar-week:before{content:""}.bi-calendar-x-fill:before{content:""}.bi-calendar-x:before{content:""}.bi-calendar:before{content:""}.bi-calendar2-check-fill:before{content:""}.bi-calendar2-check:before{content:""}.bi-calendar2-date-fill:before{content:""}.bi-calendar2-date:before{content:""}.bi-calendar2-day-fill:before{content:""}.bi-calendar2-day:before{content:""}.bi-calendar2-event-fill:before{content:""}.bi-calendar2-event:before{content:""}.bi-calendar2-fill:before{content:""}.bi-calendar2-minus-fill:before{content:""}.bi-calendar2-minus:before{content:""}.bi-calendar2-month-fill:before{content:""}.bi-calendar2-month:before{content:""}.bi-calendar2-plus-fill:before{content:""}.bi-calendar2-plus:before{content:""}.bi-calendar2-range-fill:before{content:""}.bi-calendar2-range:before{content:""}.bi-calendar2-week-fill:before{content:""}.bi-calendar2-week:before{content:""}.bi-calendar2-x-fill:before{content:""}.bi-calendar2-x:before{content:""}.bi-calendar2:before{content:""}.bi-calendar3-event-fill:before{content:""}.bi-calendar3-event:before{content:""}.bi-calendar3-fill:before{content:""}.bi-calendar3-range-fill:before{content:""}.bi-calendar3-range:before{content:""}.bi-calendar3-week-fill:before{content:""}.bi-calendar3-week:before{content:""}.bi-calendar3:before{content:""}.bi-calendar4-event:before{content:""}.bi-calendar4-range:before{content:""}.bi-calendar4-week:before{content:""}.bi-calendar4:before{content:""}.bi-camera-fill:before{content:""}.bi-camera-reels-fill:before{content:""}.bi-camera-reels:before{content:""}.bi-camera-video-fill:before{content:""}.bi-camera-video-off-fill:before{content:""}.bi-camera-video-off:before{content:""}.bi-camera-video:before{content:""}.bi-camera:before{content:""}.bi-camera2:before{content:""}.bi-capslock-fill:before{content:""}.bi-capslock:before{content:""}.bi-card-checklist:before{content:""}.bi-card-heading:before{content:""}.bi-card-image:before{content:""}.bi-card-list:before{content:""}.bi-card-text:before{content:""}.bi-caret-down-fill:before{content:""}.bi-caret-down-square-fill:before{content:""}.bi-caret-down-square:before{content:""}.bi-caret-down:before{content:""}.bi-caret-left-fill:before{content:""}.bi-caret-left-square-fill:before{content:""}.bi-caret-left-square:before{content:""}.bi-caret-left:before{content:""}.bi-caret-right-fill:before{content:""}.bi-caret-right-square-fill:before{content:""}.bi-caret-right-square:before{content:""}.bi-caret-right:before{content:""}.bi-caret-up-fill:before{content:""}.bi-caret-up-square-fill:before{content:""}.bi-caret-up-square:before{content:""}.bi-caret-up:before{content:""}.bi-cart-check-fill:before{content:""}.bi-cart-check:before{content:""}.bi-cart-dash-fill:before{content:""}.bi-cart-dash:before{content:""}.bi-cart-fill:before{content:""}.bi-cart-plus-fill:before{content:""}.bi-cart-plus:before{content:""}.bi-cart-x-fill:before{content:""}.bi-cart-x:before{content:""}.bi-cart:before{content:""}.bi-cart2:before{content:""}.bi-cart3:before{content:""}.bi-cart4:before{content:""}.bi-cash-stack:before{content:""}.bi-cash:before{content:""}.bi-cast:before{content:""}.bi-chat-dots-fill:before{content:""}.bi-chat-dots:before{content:""}.bi-chat-fill:before{content:""}.bi-chat-left-dots-fill:before{content:""}.bi-chat-left-dots:before{content:""}.bi-chat-left-fill:before{content:""}.bi-chat-left-quote-fill:before{content:""}.bi-chat-left-quote:before{content:""}.bi-chat-left-text-fill:before{content:""}.bi-chat-left-text:before{content:""}.bi-chat-left:before{content:""}.bi-chat-quote-fill:before{content:""}.bi-chat-quote:before{content:""}.bi-chat-right-dots-fill:before{content:""}.bi-chat-right-dots:before{content:""}.bi-chat-right-fill:before{content:""}.bi-chat-right-quote-fill:before{content:""}.bi-chat-right-quote:before{content:""}.bi-chat-right-text-fill:before{content:""}.bi-chat-right-text:before{content:""}.bi-chat-right:before{content:""}.bi-chat-square-dots-fill:before{content:""}.bi-chat-square-dots:before{content:""}.bi-chat-square-fill:before{content:""}.bi-chat-square-quote-fill:before{content:""}.bi-chat-square-quote:before{content:""}.bi-chat-square-text-fill:before{content:""}.bi-chat-square-text:before{content:""}.bi-chat-square:before{content:""}.bi-chat-text-fill:before{content:""}.bi-chat-text:before{content:""}.bi-chat:before{content:""}.bi-check-all:before{content:""}.bi-check-circle-fill:before{content:""}.bi-check-circle:before{content:""}.bi-check-square-fill:before{content:""}.bi-check-square:before{content:""}.bi-check:before{content:""}.bi-check2-all:before{content:""}.bi-check2-circle:before{content:""}.bi-check2-square:before{content:""}.bi-check2:before{content:""}.bi-chevron-bar-contract:before{content:""}.bi-chevron-bar-down:before{content:""}.bi-chevron-bar-expand:before{content:""}.bi-chevron-bar-left:before{content:""}.bi-chevron-bar-right:before{content:""}.bi-chevron-bar-up:before{content:""}.bi-chevron-compact-down:before{content:""}.bi-chevron-compact-left:before{content:""}.bi-chevron-compact-right:before{content:""}.bi-chevron-compact-up:before{content:""}.bi-chevron-contract:before{content:""}.bi-chevron-double-down:before{content:""}.bi-chevron-double-left:before{content:""}.bi-chevron-double-right:before{content:""}.bi-chevron-double-up:before{content:""}.bi-chevron-down:before{content:""}.bi-chevron-expand:before{content:""}.bi-chevron-left:before{content:""}.bi-chevron-right:before{content:""}.bi-chevron-up:before{content:""}.bi-circle-fill:before{content:""}.bi-circle-half:before{content:""}.bi-circle-square:before{content:""}.bi-circle:before{content:""}.bi-clipboard-check:before{content:""}.bi-clipboard-data:before{content:""}.bi-clipboard-minus:before{content:""}.bi-clipboard-plus:before{content:""}.bi-clipboard-x:before{content:""}.bi-clipboard:before{content:""}.bi-clock-fill:before{content:""}.bi-clock-history:before{content:""}.bi-clock:before{content:""}.bi-cloud-arrow-down-fill:before{content:""}.bi-cloud-arrow-down:before{content:""}.bi-cloud-arrow-up-fill:before{content:""}.bi-cloud-arrow-up:before{content:""}.bi-cloud-check-fill:before{content:""}.bi-cloud-check:before{content:""}.bi-cloud-download-fill:before{content:""}.bi-cloud-download:before{content:""}.bi-cloud-drizzle-fill:before{content:""}.bi-cloud-drizzle:before{content:""}.bi-cloud-fill:before{content:""}.bi-cloud-fog-fill:before{content:""}.bi-cloud-fog:before{content:""}.bi-cloud-fog2-fill:before{content:""}.bi-cloud-fog2:before{content:""}.bi-cloud-hail-fill:before{content:""}.bi-cloud-hail:before{content:""}.bi-cloud-haze-fill:before{content:""}.bi-cloud-haze:before{content:""}.bi-cloud-haze2-fill:before{content:""}.bi-cloud-lightning-fill:before{content:""}.bi-cloud-lightning-rain-fill:before{content:""}.bi-cloud-lightning-rain:before{content:""}.bi-cloud-lightning:before{content:""}.bi-cloud-minus-fill:before{content:""}.bi-cloud-minus:before{content:""}.bi-cloud-moon-fill:before{content:""}.bi-cloud-moon:before{content:""}.bi-cloud-plus-fill:before{content:""}.bi-cloud-plus:before{content:""}.bi-cloud-rain-fill:before{content:""}.bi-cloud-rain-heavy-fill:before{content:""}.bi-cloud-rain-heavy:before{content:""}.bi-cloud-rain:before{content:""}.bi-cloud-slash-fill:before{content:""}.bi-cloud-slash:before{content:""}.bi-cloud-sleet-fill:before{content:""}.bi-cloud-sleet:before{content:""}.bi-cloud-snow-fill:before{content:""}.bi-cloud-snow:before{content:""}.bi-cloud-sun-fill:before{content:""}.bi-cloud-sun:before{content:""}.bi-cloud-upload-fill:before{content:""}.bi-cloud-upload:before{content:""}.bi-cloud:before{content:""}.bi-clouds-fill:before{content:""}.bi-clouds:before{content:""}.bi-cloudy-fill:before{content:""}.bi-cloudy:before{content:""}.bi-code-slash:before{content:""}.bi-code-square:before{content:""}.bi-code:before{content:""}.bi-collection-fill:before{content:""}.bi-collection-play-fill:before{content:""}.bi-collection-play:before{content:""}.bi-collection:before{content:""}.bi-columns-gap:before{content:""}.bi-columns:before{content:""}.bi-command:before{content:""}.bi-compass-fill:before{content:""}.bi-compass:before{content:""}.bi-cone-striped:before{content:""}.bi-cone:before{content:""}.bi-controller:before{content:""}.bi-cpu-fill:before{content:""}.bi-cpu:before{content:""}.bi-credit-card-2-back-fill:before{content:""}.bi-credit-card-2-back:before{content:""}.bi-credit-card-2-front-fill:before{content:""}.bi-credit-card-2-front:before{content:""}.bi-credit-card-fill:before{content:""}.bi-credit-card:before{content:""}.bi-crop:before{content:""}.bi-cup-fill:before{content:""}.bi-cup-straw:before{content:""}.bi-cup:before{content:""}.bi-cursor-fill:before{content:""}.bi-cursor-text:before{content:""}.bi-cursor:before{content:""}.bi-dash-circle-dotted:before{content:""}.bi-dash-circle-fill:before{content:""}.bi-dash-circle:before{content:""}.bi-dash-square-dotted:before{content:""}.bi-dash-square-fill:before{content:""}.bi-dash-square:before{content:""}.bi-dash:before{content:""}.bi-diagram-2-fill:before{content:""}.bi-diagram-2:before{content:""}.bi-diagram-3-fill:before{content:""}.bi-diagram-3:before{content:""}.bi-diamond-fill:before{content:""}.bi-diamond-half:before{content:""}.bi-diamond:before{content:""}.bi-dice-1-fill:before{content:""}.bi-dice-1:before{content:""}.bi-dice-2-fill:before{content:""}.bi-dice-2:before{content:""}.bi-dice-3-fill:before{content:""}.bi-dice-3:before{content:""}.bi-dice-4-fill:before{content:""}.bi-dice-4:before{content:""}.bi-dice-5-fill:before{content:""}.bi-dice-5:before{content:""}.bi-dice-6-fill:before{content:""}.bi-dice-6:before{content:""}.bi-disc-fill:before{content:""}.bi-disc:before{content:""}.bi-discord:before{content:""}.bi-display-fill:before{content:""}.bi-display:before{content:""}.bi-distribute-horizontal:before{content:""}.bi-distribute-vertical:before{content:""}.bi-door-closed-fill:before{content:""}.bi-door-closed:before{content:""}.bi-door-open-fill:before{content:""}.bi-door-open:before{content:""}.bi-dot:before{content:""}.bi-download:before{content:""}.bi-droplet-fill:before{content:""}.bi-droplet-half:before{content:""}.bi-droplet:before{content:""}.bi-earbuds:before{content:""}.bi-easel-fill:before{content:""}.bi-easel:before{content:""}.bi-egg-fill:before{content:""}.bi-egg-fried:before{content:""}.bi-egg:before{content:""}.bi-eject-fill:before{content:""}.bi-eject:before{content:""}.bi-emoji-angry-fill:before{content:""}.bi-emoji-angry:before{content:""}.bi-emoji-dizzy-fill:before{content:""}.bi-emoji-dizzy:before{content:""}.bi-emoji-expressionless-fill:before{content:""}.bi-emoji-expressionless:before{content:""}.bi-emoji-frown-fill:before{content:""}.bi-emoji-frown:before{content:""}.bi-emoji-heart-eyes-fill:before{content:""}.bi-emoji-heart-eyes:before{content:""}.bi-emoji-laughing-fill:before{content:""}.bi-emoji-laughing:before{content:""}.bi-emoji-neutral-fill:before{content:""}.bi-emoji-neutral:before{content:""}.bi-emoji-smile-fill:before{content:""}.bi-emoji-smile-upside-down-fill:before{content:""}.bi-emoji-smile-upside-down:before{content:""}.bi-emoji-smile:before{content:""}.bi-emoji-sunglasses-fill:before{content:""}.bi-emoji-sunglasses:before{content:""}.bi-emoji-wink-fill:before{content:""}.bi-emoji-wink:before{content:""}.bi-envelope-fill:before{content:""}.bi-envelope-open-fill:before{content:""}.bi-envelope-open:before{content:""}.bi-envelope:before{content:""}.bi-eraser-fill:before{content:""}.bi-eraser:before{content:""}.bi-exclamation-circle-fill:before{content:""}.bi-exclamation-circle:before{content:""}.bi-exclamation-diamond-fill:before{content:""}.bi-exclamation-diamond:before{content:""}.bi-exclamation-octagon-fill:before{content:""}.bi-exclamation-octagon:before{content:""}.bi-exclamation-square-fill:before{content:""}.bi-exclamation-square:before{content:""}.bi-exclamation-triangle-fill:before{content:""}.bi-exclamation-triangle:before{content:""}.bi-exclamation:before{content:""}.bi-exclude:before{content:""}.bi-eye-fill:before{content:""}.bi-eye-slash-fill:before{content:""}.bi-eye-slash:before{content:""}.bi-eye:before{content:""}.bi-eyedropper:before{content:""}.bi-eyeglasses:before{content:""}.bi-facebook:before{content:""}.bi-file-arrow-down-fill:before{content:""}.bi-file-arrow-down:before{content:""}.bi-file-arrow-up-fill:before{content:""}.bi-file-arrow-up:before{content:""}.bi-file-bar-graph-fill:before{content:""}.bi-file-bar-graph:before{content:""}.bi-file-binary-fill:before{content:""}.bi-file-binary:before{content:""}.bi-file-break-fill:before{content:""}.bi-file-break:before{content:""}.bi-file-check-fill:before{content:""}.bi-file-check:before{content:""}.bi-file-code-fill:before{content:""}.bi-file-code:before{content:""}.bi-file-diff-fill:before{content:""}.bi-file-diff:before{content:""}.bi-file-earmark-arrow-down-fill:before{content:""}.bi-file-earmark-arrow-down:before{content:""}.bi-file-earmark-arrow-up-fill:before{content:""}.bi-file-earmark-arrow-up:before{content:""}.bi-file-earmark-bar-graph-fill:before{content:""}.bi-file-earmark-bar-graph:before{content:""}.bi-file-earmark-binary-fill:before{content:""}.bi-file-earmark-binary:before{content:""}.bi-file-earmark-break-fill:before{content:""}.bi-file-earmark-break:before{content:""}.bi-file-earmark-check-fill:before{content:""}.bi-file-earmark-check:before{content:""}.bi-file-earmark-code-fill:before{content:""}.bi-file-earmark-code:before{content:""}.bi-file-earmark-diff-fill:before{content:""}.bi-file-earmark-diff:before{content:""}.bi-file-earmark-easel-fill:before{content:""}.bi-file-earmark-easel:before{content:""}.bi-file-earmark-excel-fill:before{content:""}.bi-file-earmark-excel:before{content:""}.bi-file-earmark-fill:before{content:""}.bi-file-earmark-font-fill:before{content:""}.bi-file-earmark-font:before{content:""}.bi-file-earmark-image-fill:before{content:""}.bi-file-earmark-image:before{content:""}.bi-file-earmark-lock-fill:before{content:""}.bi-file-earmark-lock:before{content:""}.bi-file-earmark-lock2-fill:before{content:""}.bi-file-earmark-lock2:before{content:""}.bi-file-earmark-medical-fill:before{content:""}.bi-file-earmark-medical:before{content:""}.bi-file-earmark-minus-fill:before{content:""}.bi-file-earmark-minus:before{content:""}.bi-file-earmark-music-fill:before{content:""}.bi-file-earmark-music:before{content:""}.bi-file-earmark-person-fill:before{content:""}.bi-file-earmark-person:before{content:""}.bi-file-earmark-play-fill:before{content:""}.bi-file-earmark-play:before{content:""}.bi-file-earmark-plus-fill:before{content:""}.bi-file-earmark-plus:before{content:""}.bi-file-earmark-post-fill:before{content:""}.bi-file-earmark-post:before{content:""}.bi-file-earmark-ppt-fill:before{content:""}.bi-file-earmark-ppt:before{content:""}.bi-file-earmark-richtext-fill:before{content:""}.bi-file-earmark-richtext:before{content:""}.bi-file-earmark-ruled-fill:before{content:""}.bi-file-earmark-ruled:before{content:""}.bi-file-earmark-slides-fill:before{content:""}.bi-file-earmark-slides:before{content:""}.bi-file-earmark-spreadsheet-fill:before{content:""}.bi-file-earmark-spreadsheet:before{content:""}.bi-file-earmark-text-fill:before{content:""}.bi-file-earmark-text:before{content:""}.bi-file-earmark-word-fill:before{content:""}.bi-file-earmark-word:before{content:""}.bi-file-earmark-x-fill:before{content:""}.bi-file-earmark-x:before{content:""}.bi-file-earmark-zip-fill:before{content:""}.bi-file-earmark-zip:before{content:""}.bi-file-earmark:before{content:""}.bi-file-easel-fill:before{content:""}.bi-file-easel:before{content:""}.bi-file-excel-fill:before{content:""}.bi-file-excel:before{content:""}.bi-file-fill:before{content:""}.bi-file-font-fill:before{content:""}.bi-file-font:before{content:""}.bi-file-image-fill:before{content:""}.bi-file-image:before{content:""}.bi-file-lock-fill:before{content:""}.bi-file-lock:before{content:""}.bi-file-lock2-fill:before{content:""}.bi-file-lock2:before{content:""}.bi-file-medical-fill:before{content:""}.bi-file-medical:before{content:""}.bi-file-minus-fill:before{content:""}.bi-file-minus:before{content:""}.bi-file-music-fill:before{content:""}.bi-file-music:before{content:""}.bi-file-person-fill:before{content:""}.bi-file-person:before{content:""}.bi-file-play-fill:before{content:""}.bi-file-play:before{content:""}.bi-file-plus-fill:before{content:""}.bi-file-plus:before{content:""}.bi-file-post-fill:before{content:""}.bi-file-post:before{content:""}.bi-file-ppt-fill:before{content:""}.bi-file-ppt:before{content:""}.bi-file-richtext-fill:before{content:""}.bi-file-richtext:before{content:""}.bi-file-ruled-fill:before{content:""}.bi-file-ruled:before{content:""}.bi-file-slides-fill:before{content:""}.bi-file-slides:before{content:""}.bi-file-spreadsheet-fill:before{content:""}.bi-file-spreadsheet:before{content:""}.bi-file-text-fill:before{content:""}.bi-file-text:before{content:""}.bi-file-word-fill:before{content:""}.bi-file-word:before{content:""}.bi-file-x-fill:before{content:""}.bi-file-x:before{content:""}.bi-file-zip-fill:before{content:""}.bi-file-zip:before{content:""}.bi-file:before{content:""}.bi-files-alt:before{content:""}.bi-files:before{content:""}.bi-film:before{content:""}.bi-filter-circle-fill:before{content:""}.bi-filter-circle:before{content:""}.bi-filter-left:before{content:""}.bi-filter-right:before{content:""}.bi-filter-square-fill:before{content:""}.bi-filter-square:before{content:""}.bi-filter:before{content:""}.bi-flag-fill:before{content:""}.bi-flag:before{content:""}.bi-flower1:before{content:""}.bi-flower2:before{content:""}.bi-flower3:before{content:""}.bi-folder-check:before{content:""}.bi-folder-fill:before{content:""}.bi-folder-minus:before{content:""}.bi-folder-plus:before{content:""}.bi-folder-symlink-fill:before{content:""}.bi-folder-symlink:before{content:""}.bi-folder-x:before{content:""}.bi-folder:before{content:""}.bi-folder2-open:before{content:""}.bi-folder2:before{content:""}.bi-fonts:before{content:""}.bi-forward-fill:before{content:""}.bi-forward:before{content:""}.bi-front:before{content:""}.bi-fullscreen-exit:before{content:""}.bi-fullscreen:before{content:""}.bi-funnel-fill:before{content:""}.bi-funnel:before{content:""}.bi-gear-fill:before{content:""}.bi-gear-wide-connected:before{content:""}.bi-gear-wide:before{content:""}.bi-gear:before{content:""}.bi-gem:before{content:""}.bi-geo-alt-fill:before{content:""}.bi-geo-alt:before{content:""}.bi-geo-fill:before{content:""}.bi-geo:before{content:""}.bi-gift-fill:before{content:""}.bi-gift:before{content:""}.bi-github:before{content:""}.bi-globe:before{content:""}.bi-globe2:before{content:""}.bi-google:before{content:""}.bi-graph-down:before{content:""}.bi-graph-up:before{content:""}.bi-grid-1x2-fill:before{content:""}.bi-grid-1x2:before{content:""}.bi-grid-3x2-gap-fill:before{content:""}.bi-grid-3x2-gap:before{content:""}.bi-grid-3x2:before{content:""}.bi-grid-3x3-gap-fill:before{content:""}.bi-grid-3x3-gap:before{content:""}.bi-grid-3x3:before{content:""}.bi-grid-fill:before{content:""}.bi-grid:before{content:""}.bi-grip-horizontal:before{content:""}.bi-grip-vertical:before{content:""}.bi-hammer:before{content:""}.bi-hand-index-fill:before{content:""}.bi-hand-index-thumb-fill:before{content:""}.bi-hand-index-thumb:before{content:""}.bi-hand-index:before{content:""}.bi-hand-thumbs-down-fill:before{content:""}.bi-hand-thumbs-down:before{content:""}.bi-hand-thumbs-up-fill:before{content:""}.bi-hand-thumbs-up:before{content:""}.bi-handbag-fill:before{content:""}.bi-handbag:before{content:""}.bi-hash:before{content:""}.bi-hdd-fill:before{content:""}.bi-hdd-network-fill:before{content:""}.bi-hdd-network:before{content:""}.bi-hdd-rack-fill:before{content:""}.bi-hdd-rack:before{content:""}.bi-hdd-stack-fill:before{content:""}.bi-hdd-stack:before{content:""}.bi-hdd:before{content:""}.bi-headphones:before{content:""}.bi-headset:before{content:""}.bi-heart-fill:before{content:""}.bi-heart-half:before{content:""}.bi-heart:before{content:""}.bi-heptagon-fill:before{content:""}.bi-heptagon-half:before{content:""}.bi-heptagon:before{content:""}.bi-hexagon-fill:before{content:""}.bi-hexagon-half:before{content:""}.bi-hexagon:before{content:""}.bi-hourglass-bottom:before{content:""}.bi-hourglass-split:before{content:""}.bi-hourglass-top:before{content:""}.bi-hourglass:before{content:""}.bi-house-door-fill:before{content:""}.bi-house-door:before{content:""}.bi-house-fill:before{content:""}.bi-house:before{content:""}.bi-hr:before{content:""}.bi-hurricane:before{content:""}.bi-image-alt:before{content:""}.bi-image-fill:before{content:""}.bi-image:before{content:""}.bi-images:before{content:""}.bi-inbox-fill:before{content:""}.bi-inbox:before{content:""}.bi-inboxes-fill:before{content:""}.bi-inboxes:before{content:""}.bi-info-circle-fill:before{content:""}.bi-info-circle:before{content:""}.bi-info-square-fill:before{content:""}.bi-info-square:before{content:""}.bi-info:before{content:""}.bi-input-cursor-text:before{content:""}.bi-input-cursor:before{content:""}.bi-instagram:before{content:""}.bi-intersect:before{content:""}.bi-journal-album:before{content:""}.bi-journal-arrow-down:before{content:""}.bi-journal-arrow-up:before{content:""}.bi-journal-bookmark-fill:before{content:""}.bi-journal-bookmark:before{content:""}.bi-journal-check:before{content:""}.bi-journal-code:before{content:""}.bi-journal-medical:before{content:""}.bi-journal-minus:before{content:""}.bi-journal-plus:before{content:""}.bi-journal-richtext:before{content:""}.bi-journal-text:before{content:""}.bi-journal-x:before{content:""}.bi-journal:before{content:""}.bi-journals:before{content:""}.bi-joystick:before{content:""}.bi-justify-left:before{content:""}.bi-justify-right:before{content:""}.bi-justify:before{content:""}.bi-kanban-fill:before{content:""}.bi-kanban:before{content:""}.bi-key-fill:before{content:""}.bi-key:before{content:""}.bi-keyboard-fill:before{content:""}.bi-keyboard:before{content:""}.bi-ladder:before{content:""}.bi-lamp-fill:before{content:""}.bi-lamp:before{content:""}.bi-laptop-fill:before{content:""}.bi-laptop:before{content:""}.bi-layer-backward:before{content:""}.bi-layer-forward:before{content:""}.bi-layers-fill:before{content:""}.bi-layers-half:before{content:""}.bi-layers:before{content:""}.bi-layout-sidebar-inset-reverse:before{content:""}.bi-layout-sidebar-inset:before{content:""}.bi-layout-sidebar-reverse:before{content:""}.bi-layout-sidebar:before{content:""}.bi-layout-split:before{content:""}.bi-layout-text-sidebar-reverse:before{content:""}.bi-layout-text-sidebar:before{content:""}.bi-layout-text-window-reverse:before{content:""}.bi-layout-text-window:before{content:""}.bi-layout-three-columns:before{content:""}.bi-layout-wtf:before{content:""}.bi-life-preserver:before{content:""}.bi-lightbulb-fill:before{content:""}.bi-lightbulb-off-fill:before{content:""}.bi-lightbulb-off:before{content:""}.bi-lightbulb:before{content:""}.bi-lightning-charge-fill:before{content:""}.bi-lightning-charge:before{content:""}.bi-lightning-fill:before{content:""}.bi-lightning:before{content:""}.bi-link-45deg:before{content:""}.bi-link:before{content:""}.bi-linkedin:before{content:""}.bi-list-check:before{content:""}.bi-list-nested:before{content:""}.bi-list-ol:before{content:""}.bi-list-stars:before{content:""}.bi-list-task:before{content:""}.bi-list-ul:before{content:""}.bi-list:before{content:""}.bi-lock-fill:before{content:""}.bi-lock:before{content:""}.bi-mailbox:before{content:""}.bi-mailbox2:before{content:""}.bi-map-fill:before{content:""}.bi-map:before{content:""}.bi-markdown-fill:before{content:""}.bi-markdown:before{content:""}.bi-mask:before{content:""}.bi-megaphone-fill:before{content:""}.bi-megaphone:before{content:""}.bi-menu-app-fill:before{content:""}.bi-menu-app:before{content:""}.bi-menu-button-fill:before{content:""}.bi-menu-button-wide-fill:before{content:""}.bi-menu-button-wide:before{content:""}.bi-menu-button:before{content:""}.bi-menu-down:before{content:""}.bi-menu-up:before{content:""}.bi-mic-fill:before{content:""}.bi-mic-mute-fill:before{content:""}.bi-mic-mute:before{content:""}.bi-mic:before{content:""}.bi-minecart-loaded:before{content:""}.bi-minecart:before{content:""}.bi-moisture:before{content:""}.bi-moon-fill:before{content:""}.bi-moon-stars-fill:before{content:""}.bi-moon-stars:before{content:""}.bi-moon:before{content:""}.bi-mouse-fill:before{content:""}.bi-mouse:before{content:""}.bi-mouse2-fill:before{content:""}.bi-mouse2:before{content:""}.bi-mouse3-fill:before{content:""}.bi-mouse3:before{content:""}.bi-music-note-beamed:before{content:""}.bi-music-note-list:before{content:""}.bi-music-note:before{content:""}.bi-music-player-fill:before{content:""}.bi-music-player:before{content:""}.bi-newspaper:before{content:""}.bi-node-minus-fill:before{content:""}.bi-node-minus:before{content:""}.bi-node-plus-fill:before{content:""}.bi-node-plus:before{content:""}.bi-nut-fill:before{content:""}.bi-nut:before{content:""}.bi-octagon-fill:before{content:""}.bi-octagon-half:before{content:""}.bi-octagon:before{content:""}.bi-option:before{content:""}.bi-outlet:before{content:""}.bi-paint-bucket:before{content:""}.bi-palette-fill:before{content:""}.bi-palette:before{content:""}.bi-palette2:before{content:""}.bi-paperclip:before{content:""}.bi-paragraph:before{content:""}.bi-patch-check-fill:before{content:""}.bi-patch-check:before{content:""}.bi-patch-exclamation-fill:before{content:""}.bi-patch-exclamation:before{content:""}.bi-patch-minus-fill:before{content:""}.bi-patch-minus:before{content:""}.bi-patch-plus-fill:before{content:""}.bi-patch-plus:before{content:""}.bi-patch-question-fill:before{content:""}.bi-patch-question:before{content:""}.bi-pause-btn-fill:before{content:""}.bi-pause-btn:before{content:""}.bi-pause-circle-fill:before{content:""}.bi-pause-circle:before{content:""}.bi-pause-fill:before{content:""}.bi-pause:before{content:""}.bi-peace-fill:before{content:""}.bi-peace:before{content:""}.bi-pen-fill:before{content:""}.bi-pen:before{content:""}.bi-pencil-fill:before{content:""}.bi-pencil-square:before{content:""}.bi-pencil:before{content:""}.bi-pentagon-fill:before{content:""}.bi-pentagon-half:before{content:""}.bi-pentagon:before{content:""}.bi-people-fill:before{content:""}.bi-people:before{content:""}.bi-percent:before{content:""}.bi-person-badge-fill:before{content:""}.bi-person-badge:before{content:""}.bi-person-bounding-box:before{content:""}.bi-person-check-fill:before{content:""}.bi-person-check:before{content:""}.bi-person-circle:before{content:""}.bi-person-dash-fill:before{content:""}.bi-person-dash:before{content:""}.bi-person-fill:before{content:""}.bi-person-lines-fill:before{content:""}.bi-person-plus-fill:before{content:""}.bi-person-plus:before{content:""}.bi-person-square:before{content:""}.bi-person-x-fill:before{content:""}.bi-person-x:before{content:""}.bi-person:before{content:""}.bi-phone-fill:before{content:""}.bi-phone-landscape-fill:before{content:""}.bi-phone-landscape:before{content:""}.bi-phone-vibrate-fill:before{content:""}.bi-phone-vibrate:before{content:""}.bi-phone:before{content:""}.bi-pie-chart-fill:before{content:""}.bi-pie-chart:before{content:""}.bi-pin-angle-fill:before{content:""}.bi-pin-angle:before{content:""}.bi-pin-fill:before{content:""}.bi-pin:before{content:""}.bi-pip-fill:before{content:""}.bi-pip:before{content:""}.bi-play-btn-fill:before{content:""}.bi-play-btn:before{content:""}.bi-play-circle-fill:before{content:""}.bi-play-circle:before{content:""}.bi-play-fill:before{content:""}.bi-play:before{content:""}.bi-plug-fill:before{content:""}.bi-plug:before{content:""}.bi-plus-circle-dotted:before{content:""}.bi-plus-circle-fill:before{content:""}.bi-plus-circle:before{content:""}.bi-plus-square-dotted:before{content:""}.bi-plus-square-fill:before{content:""}.bi-plus-square:before{content:""}.bi-plus:before{content:""}.bi-power:before{content:""}.bi-printer-fill:before{content:""}.bi-printer:before{content:""}.bi-puzzle-fill:before{content:""}.bi-puzzle:before{content:""}.bi-question-circle-fill:before{content:""}.bi-question-circle:before{content:""}.bi-question-diamond-fill:before{content:""}.bi-question-diamond:before{content:""}.bi-question-octagon-fill:before{content:""}.bi-question-octagon:before{content:""}.bi-question-square-fill:before{content:""}.bi-question-square:before{content:""}.bi-question:before{content:""}.bi-rainbow:before{content:""}.bi-receipt-cutoff:before{content:""}.bi-receipt:before{content:""}.bi-reception-0:before{content:""}.bi-reception-1:before{content:""}.bi-reception-2:before{content:""}.bi-reception-3:before{content:""}.bi-reception-4:before{content:""}.bi-record-btn-fill:before{content:""}.bi-record-btn:before{content:""}.bi-record-circle-fill:before{content:""}.bi-record-circle:before{content:""}.bi-record-fill:before{content:""}.bi-record:before{content:""}.bi-record2-fill:before{content:""}.bi-record2:before{content:""}.bi-reply-all-fill:before{content:""}.bi-reply-all:before{content:""}.bi-reply-fill:before{content:""}.bi-reply:before{content:""}.bi-rss-fill:before{content:""}.bi-rss:before{content:""}.bi-rulers:before{content:""}.bi-save-fill:before{content:""}.bi-save:before{content:""}.bi-save2-fill:before{content:""}.bi-save2:before{content:""}.bi-scissors:before{content:""}.bi-screwdriver:before{content:""}.bi-search:before{content:""}.bi-segmented-nav:before{content:""}.bi-server:before{content:""}.bi-share-fill:before{content:""}.bi-share:before{content:""}.bi-shield-check:before{content:""}.bi-shield-exclamation:before{content:""}.bi-shield-fill-check:before{content:""}.bi-shield-fill-exclamation:before{content:""}.bi-shield-fill-minus:before{content:""}.bi-shield-fill-plus:before{content:""}.bi-shield-fill-x:before{content:""}.bi-shield-fill:before{content:""}.bi-shield-lock-fill:before{content:""}.bi-shield-lock:before{content:""}.bi-shield-minus:before{content:""}.bi-shield-plus:before{content:""}.bi-shield-shaded:before{content:""}.bi-shield-slash-fill:before{content:""}.bi-shield-slash:before{content:""}.bi-shield-x:before{content:""}.bi-shield:before{content:""}.bi-shift-fill:before{content:""}.bi-shift:before{content:""}.bi-shop-window:before{content:""}.bi-shop:before{content:""}.bi-shuffle:before{content:""}.bi-signpost-2-fill:before{content:""}.bi-signpost-2:before{content:""}.bi-signpost-fill:before{content:""}.bi-signpost-split-fill:before{content:""}.bi-signpost-split:before{content:""}.bi-signpost:before{content:""}.bi-sim-fill:before{content:""}.bi-sim:before{content:""}.bi-skip-backward-btn-fill:before{content:""}.bi-skip-backward-btn:before{content:""}.bi-skip-backward-circle-fill:before{content:""}.bi-skip-backward-circle:before{content:""}.bi-skip-backward-fill:before{content:""}.bi-skip-backward:before{content:""}.bi-skip-end-btn-fill:before{content:""}.bi-skip-end-btn:before{content:""}.bi-skip-end-circle-fill:before{content:""}.bi-skip-end-circle:before{content:""}.bi-skip-end-fill:before{content:""}.bi-skip-end:before{content:""}.bi-skip-forward-btn-fill:before{content:""}.bi-skip-forward-btn:before{content:""}.bi-skip-forward-circle-fill:before{content:""}.bi-skip-forward-circle:before{content:""}.bi-skip-forward-fill:before{content:""}.bi-skip-forward:before{content:""}.bi-skip-start-btn-fill:before{content:""}.bi-skip-start-btn:before{content:""}.bi-skip-start-circle-fill:before{content:""}.bi-skip-start-circle:before{content:""}.bi-skip-start-fill:before{content:""}.bi-skip-start:before{content:""}.bi-slack:before{content:""}.bi-slash-circle-fill:before{content:""}.bi-slash-circle:before{content:""}.bi-slash-square-fill:before{content:""}.bi-slash-square:before{content:""}.bi-slash:before{content:""}.bi-sliders:before{content:""}.bi-smartwatch:before{content:""}.bi-snow:before{content:""}.bi-snow2:before{content:""}.bi-snow3:before{content:""}.bi-sort-alpha-down-alt:before{content:""}.bi-sort-alpha-down:before{content:""}.bi-sort-alpha-up-alt:before{content:""}.bi-sort-alpha-up:before{content:""}.bi-sort-down-alt:before{content:""}.bi-sort-down:before{content:""}.bi-sort-numeric-down-alt:before{content:""}.bi-sort-numeric-down:before{content:""}.bi-sort-numeric-up-alt:before{content:""}.bi-sort-numeric-up:before{content:""}.bi-sort-up-alt:before{content:""}.bi-sort-up:before{content:""}.bi-soundwave:before{content:""}.bi-speaker-fill:before{content:""}.bi-speaker:before{content:""}.bi-speedometer:before{content:""}.bi-speedometer2:before{content:""}.bi-spellcheck:before{content:""}.bi-square-fill:before{content:""}.bi-square-half:before{content:""}.bi-square:before{content:""}.bi-stack:before{content:""}.bi-star-fill:before{content:""}.bi-star-half:before{content:""}.bi-star:before{content:""}.bi-stars:before{content:""}.bi-stickies-fill:before{content:""}.bi-stickies:before{content:""}.bi-sticky-fill:before{content:""}.bi-sticky:before{content:""}.bi-stop-btn-fill:before{content:""}.bi-stop-btn:before{content:""}.bi-stop-circle-fill:before{content:""}.bi-stop-circle:before{content:""}.bi-stop-fill:before{content:""}.bi-stop:before{content:""}.bi-stoplights-fill:before{content:""}.bi-stoplights:before{content:""}.bi-stopwatch-fill:before{content:""}.bi-stopwatch:before{content:""}.bi-subtract:before{content:""}.bi-suit-club-fill:before{content:""}.bi-suit-club:before{content:""}.bi-suit-diamond-fill:before{content:""}.bi-suit-diamond:before{content:""}.bi-suit-heart-fill:before{content:""}.bi-suit-heart:before{content:""}.bi-suit-spade-fill:before{content:""}.bi-suit-spade:before{content:""}.bi-sun-fill:before{content:""}.bi-sun:before{content:""}.bi-sunglasses:before{content:""}.bi-sunrise-fill:before{content:""}.bi-sunrise:before{content:""}.bi-sunset-fill:before{content:""}.bi-sunset:before{content:""}.bi-symmetry-horizontal:before{content:""}.bi-symmetry-vertical:before{content:""}.bi-table:before{content:""}.bi-tablet-fill:before{content:""}.bi-tablet-landscape-fill:before{content:""}.bi-tablet-landscape:before{content:""}.bi-tablet:before{content:""}.bi-tag-fill:before{content:""}.bi-tag:before{content:""}.bi-tags-fill:before{content:""}.bi-tags:before{content:""}.bi-telegram:before{content:""}.bi-telephone-fill:before{content:""}.bi-telephone-forward-fill:before{content:""}.bi-telephone-forward:before{content:""}.bi-telephone-inbound-fill:before{content:""}.bi-telephone-inbound:before{content:""}.bi-telephone-minus-fill:before{content:""}.bi-telephone-minus:before{content:""}.bi-telephone-outbound-fill:before{content:""}.bi-telephone-outbound:before{content:""}.bi-telephone-plus-fill:before{content:""}.bi-telephone-plus:before{content:""}.bi-telephone-x-fill:before{content:""}.bi-telephone-x:before{content:""}.bi-telephone:before{content:""}.bi-terminal-fill:before{content:""}.bi-terminal:before{content:""}.bi-text-center:before{content:""}.bi-text-indent-left:before{content:""}.bi-text-indent-right:before{content:""}.bi-text-left:before{content:""}.bi-text-paragraph:before{content:""}.bi-text-right:before{content:""}.bi-textarea-resize:before{content:""}.bi-textarea-t:before{content:""}.bi-textarea:before{content:""}.bi-thermometer-half:before{content:""}.bi-thermometer-high:before{content:""}.bi-thermometer-low:before{content:""}.bi-thermometer-snow:before{content:""}.bi-thermometer-sun:before{content:""}.bi-thermometer:before{content:""}.bi-three-dots-vertical:before{content:""}.bi-three-dots:before{content:""}.bi-toggle-off:before{content:""}.bi-toggle-on:before{content:""}.bi-toggle2-off:before{content:""}.bi-toggle2-on:before{content:""}.bi-toggles:before{content:""}.bi-toggles2:before{content:""}.bi-tools:before{content:""}.bi-tornado:before{content:""}.bi-trash-fill:before{content:""}.bi-trash:before{content:""}.bi-trash2-fill:before{content:""}.bi-trash2:before{content:""}.bi-tree-fill:before{content:""}.bi-tree:before{content:""}.bi-triangle-fill:before{content:""}.bi-triangle-half:before{content:""}.bi-triangle:before{content:""}.bi-trophy-fill:before{content:""}.bi-trophy:before{content:""}.bi-tropical-storm:before{content:""}.bi-truck-flatbed:before{content:""}.bi-truck:before{content:""}.bi-tsunami:before{content:""}.bi-tv-fill:before{content:""}.bi-tv:before{content:""}.bi-twitch:before{content:""}.bi-twitter:before{content:""}.bi-type-bold:before{content:""}.bi-type-h1:before{content:""}.bi-type-h2:before{content:""}.bi-type-h3:before{content:""}.bi-type-italic:before{content:""}.bi-type-strikethrough:before{content:""}.bi-type-underline:before{content:""}.bi-type:before{content:""}.bi-ui-checks-grid:before{content:""}.bi-ui-checks:before{content:""}.bi-ui-radios-grid:before{content:""}.bi-ui-radios:before{content:""}.bi-umbrella-fill:before{content:""}.bi-umbrella:before{content:""}.bi-union:before{content:""}.bi-unlock-fill:before{content:""}.bi-unlock:before{content:""}.bi-upc-scan:before{content:""}.bi-upc:before{content:""}.bi-upload:before{content:""}.bi-vector-pen:before{content:""}.bi-view-list:before{content:""}.bi-view-stacked:before{content:""}.bi-vinyl-fill:before{content:""}.bi-vinyl:before{content:""}.bi-voicemail:before{content:""}.bi-volume-down-fill:before{content:""}.bi-volume-down:before{content:""}.bi-volume-mute-fill:before{content:""}.bi-volume-mute:before{content:""}.bi-volume-off-fill:before{content:""}.bi-volume-off:before{content:""}.bi-volume-up-fill:before{content:""}.bi-volume-up:before{content:""}.bi-vr:before{content:""}.bi-wallet-fill:before{content:""}.bi-wallet:before{content:""}.bi-wallet2:before{content:""}.bi-watch:before{content:""}.bi-water:before{content:""}.bi-whatsapp:before{content:""}.bi-wifi-1:before{content:""}.bi-wifi-2:before{content:""}.bi-wifi-off:before{content:""}.bi-wifi:before{content:""}.bi-wind:before{content:""}.bi-window-dock:before{content:""}.bi-window-sidebar:before{content:""}.bi-window:before{content:""}.bi-wrench:before{content:""}.bi-x-circle-fill:before{content:""}.bi-x-circle:before{content:""}.bi-x-diamond-fill:before{content:""}.bi-x-diamond:before{content:""}.bi-x-octagon-fill:before{content:""}.bi-x-octagon:before{content:""}.bi-x-square-fill:before{content:""}.bi-x-square:before{content:""}.bi-x:before{content:""}.bi-youtube:before{content:""}.bi-zoom-in:before{content:""}.bi-zoom-out:before{content:""}.bi-bank:before{content:""}.bi-bank2:before{content:""}.bi-bell-slash-fill:before{content:""}.bi-bell-slash:before{content:""}.bi-cash-coin:before{content:""}.bi-check-lg:before{content:""}.bi-coin:before{content:""}.bi-currency-bitcoin:before{content:""}.bi-currency-dollar:before{content:""}.bi-currency-euro:before{content:""}.bi-currency-exchange:before{content:""}.bi-currency-pound:before{content:""}.bi-currency-yen:before{content:""}.bi-dash-lg:before{content:""}.bi-exclamation-lg:before{content:""}.bi-file-earmark-pdf-fill:before{content:""}.bi-file-earmark-pdf:before{content:""}.bi-file-pdf-fill:before{content:""}.bi-file-pdf:before{content:""}.bi-gender-ambiguous:before{content:""}.bi-gender-female:before{content:""}.bi-gender-male:before{content:""}.bi-gender-trans:before{content:""}.bi-headset-vr:before{content:""}.bi-info-lg:before{content:""}.bi-mastodon:before{content:""}.bi-messenger:before{content:""}.bi-piggy-bank-fill:before{content:""}.bi-piggy-bank:before{content:""}.bi-pin-map-fill:before{content:""}.bi-pin-map:before{content:""}.bi-plus-lg:before{content:""}.bi-question-lg:before{content:""}.bi-recycle:before{content:""}.bi-reddit:before{content:""}.bi-safe-fill:before{content:""}.bi-safe2-fill:before{content:""}.bi-safe2:before{content:""}.bi-sd-card-fill:before{content:""}.bi-sd-card:before{content:""}.bi-skype:before{content:""}.bi-slash-lg:before{content:""}.bi-translate:before{content:""}.bi-x-lg:before{content:""}.bi-safe:before{content:""}.bi-apple:before{content:""}.bi-microsoft:before{content:""}.bi-windows:before{content:""}.bi-behance:before{content:""}.bi-dribbble:before{content:""}.bi-line:before{content:""}.bi-medium:before{content:""}.bi-paypal:before{content:""}.bi-pinterest:before{content:""}.bi-signal:before{content:""}.bi-snapchat:before{content:""}.bi-spotify:before{content:""}.bi-stack-overflow:before{content:""}.bi-strava:before{content:""}.bi-wordpress:before{content:""}.bi-vimeo:before{content:""}.bi-activity:before{content:""}.bi-easel2-fill:before{content:""}.bi-easel2:before{content:""}.bi-easel3-fill:before{content:""}.bi-easel3:before{content:""}.bi-fan:before{content:""}.bi-fingerprint:before{content:""}.bi-graph-down-arrow:before{content:""}.bi-graph-up-arrow:before{content:""}.bi-hypnotize:before{content:""}.bi-magic:before{content:""}.bi-person-rolodex:before{content:""}.bi-person-video:before{content:""}.bi-person-video2:before{content:""}.bi-person-video3:before{content:""}.bi-person-workspace:before{content:""}.bi-radioactive:before{content:""}.bi-webcam-fill:before{content:""}.bi-webcam:before{content:""}.bi-yin-yang:before{content:""}.bi-bandaid-fill:before{content:""}.bi-bandaid:before{content:""}.bi-bluetooth:before{content:""}.bi-body-text:before{content:""}.bi-boombox:before{content:""}.bi-boxes:before{content:""}.bi-dpad-fill:before{content:""}.bi-dpad:before{content:""}.bi-ear-fill:before{content:""}.bi-ear:before{content:""}.bi-envelope-check-fill:before{content:""}.bi-envelope-check:before{content:""}.bi-envelope-dash-fill:before{content:""}.bi-envelope-dash:before{content:""}.bi-envelope-exclamation-fill:before{content:""}.bi-envelope-exclamation:before{content:""}.bi-envelope-plus-fill:before{content:""}.bi-envelope-plus:before{content:""}.bi-envelope-slash-fill:before{content:""}.bi-envelope-slash:before{content:""}.bi-envelope-x-fill:before{content:""}.bi-envelope-x:before{content:""}.bi-explicit-fill:before{content:""}.bi-explicit:before{content:""}.bi-git:before{content:""}.bi-infinity:before{content:""}.bi-list-columns-reverse:before{content:""}.bi-list-columns:before{content:""}.bi-meta:before{content:""}.bi-nintendo-switch:before{content:""}.bi-pc-display-horizontal:before{content:""}.bi-pc-display:before{content:""}.bi-pc-horizontal:before{content:""}.bi-pc:before{content:""}.bi-playstation:before{content:""}.bi-plus-slash-minus:before{content:""}.bi-projector-fill:before{content:""}.bi-projector:before{content:""}.bi-qr-code-scan:before{content:""}.bi-qr-code:before{content:""}.bi-quora:before{content:""}.bi-quote:before{content:""}.bi-robot:before{content:""}.bi-send-check-fill:before{content:""}.bi-send-check:before{content:""}.bi-send-dash-fill:before{content:""}.bi-send-dash:before{content:""}.bi-send-exclamation-fill:before{content:""}.bi-send-exclamation:before{content:""}.bi-send-fill:before{content:""}.bi-send-plus-fill:before{content:""}.bi-send-plus:before{content:""}.bi-send-slash-fill:before{content:""}.bi-send-slash:before{content:""}.bi-send-x-fill:before{content:""}.bi-send-x:before{content:""}.bi-send:before{content:""}.bi-steam:before{content:""}.bi-terminal-dash:before{content:""}.bi-terminal-plus:before{content:""}.bi-terminal-split:before{content:""}.bi-ticket-detailed-fill:before{content:""}.bi-ticket-detailed:before{content:""}.bi-ticket-fill:before{content:""}.bi-ticket-perforated-fill:before{content:""}.bi-ticket-perforated:before{content:""}.bi-ticket:before{content:""}.bi-tiktok:before{content:""}.bi-window-dash:before{content:""}.bi-window-desktop:before{content:""}.bi-window-fullscreen:before{content:""}.bi-window-plus:before{content:""}.bi-window-split:before{content:""}.bi-window-stack:before{content:""}.bi-window-x:before{content:""}.bi-xbox:before{content:""}.bi-ethernet:before{content:""}.bi-hdmi-fill:before{content:""}.bi-hdmi:before{content:""}.bi-usb-c-fill:before{content:""}.bi-usb-c:before{content:""}.bi-usb-fill:before{content:""}.bi-usb-plug-fill:before{content:""}.bi-usb-plug:before{content:""}.bi-usb-symbol:before{content:""}.bi-usb:before{content:""}.bi-boombox-fill:before{content:""}.bi-displayport:before{content:""}.bi-gpu-card:before{content:""}.bi-memory:before{content:""}.bi-modem-fill:before{content:""}.bi-modem:before{content:""}.bi-motherboard-fill:before{content:""}.bi-motherboard:before{content:""}.bi-optical-audio-fill:before{content:""}.bi-optical-audio:before{content:""}.bi-pci-card:before{content:""}.bi-router-fill:before{content:""}.bi-router:before{content:""}.bi-thunderbolt-fill:before{content:""}.bi-thunderbolt:before{content:""}.bi-usb-drive-fill:before{content:""}.bi-usb-drive:before{content:""}.bi-usb-micro-fill:before{content:""}.bi-usb-micro:before{content:""}.bi-usb-mini-fill:before{content:""}.bi-usb-mini:before{content:""}.bi-cloud-haze2:before{content:""}.bi-device-hdd-fill:before{content:""}.bi-device-hdd:before{content:""}.bi-device-ssd-fill:before{content:""}.bi-device-ssd:before{content:""}.bi-displayport-fill:before{content:""}.bi-mortarboard-fill:before{content:""}.bi-mortarboard:before{content:""}.bi-terminal-x:before{content:""}.bi-arrow-through-heart-fill:before{content:""}.bi-arrow-through-heart:before{content:""}.bi-badge-sd-fill:before{content:""}.bi-badge-sd:before{content:""}.bi-bag-heart-fill:before{content:""}.bi-bag-heart:before{content:""}.bi-balloon-fill:before{content:""}.bi-balloon-heart-fill:before{content:""}.bi-balloon-heart:before{content:""}.bi-balloon:before{content:""}.bi-box2-fill:before{content:""}.bi-box2-heart-fill:before{content:""}.bi-box2-heart:before{content:""}.bi-box2:before{content:""}.bi-braces-asterisk:before{content:""}.bi-calendar-heart-fill:before{content:""}.bi-calendar-heart:before{content:""}.bi-calendar2-heart-fill:before{content:""}.bi-calendar2-heart:before{content:""}.bi-chat-heart-fill:before{content:""}.bi-chat-heart:before{content:""}.bi-chat-left-heart-fill:before{content:""}.bi-chat-left-heart:before{content:""}.bi-chat-right-heart-fill:before{content:""}.bi-chat-right-heart:before{content:""}.bi-chat-square-heart-fill:before{content:""}.bi-chat-square-heart:before{content:""}.bi-clipboard-check-fill:before{content:""}.bi-clipboard-data-fill:before{content:""}.bi-clipboard-fill:before{content:""}.bi-clipboard-heart-fill:before{content:""}.bi-clipboard-heart:before{content:""}.bi-clipboard-minus-fill:before{content:""}.bi-clipboard-plus-fill:before{content:""}.bi-clipboard-pulse:before{content:""}.bi-clipboard-x-fill:before{content:""}.bi-clipboard2-check-fill:before{content:""}.bi-clipboard2-check:before{content:""}.bi-clipboard2-data-fill:before{content:""}.bi-clipboard2-data:before{content:""}.bi-clipboard2-fill:before{content:""}.bi-clipboard2-heart-fill:before{content:""}.bi-clipboard2-heart:before{content:""}.bi-clipboard2-minus-fill:before{content:""}.bi-clipboard2-minus:before{content:""}.bi-clipboard2-plus-fill:before{content:""}.bi-clipboard2-plus:before{content:""}.bi-clipboard2-pulse-fill:before{content:""}.bi-clipboard2-pulse:before{content:""}.bi-clipboard2-x-fill:before{content:""}.bi-clipboard2-x:before{content:""}.bi-clipboard2:before{content:""}.bi-emoji-kiss-fill:before{content:""}.bi-emoji-kiss:before{content:""}.bi-envelope-heart-fill:before{content:""}.bi-envelope-heart:before{content:""}.bi-envelope-open-heart-fill:before{content:""}.bi-envelope-open-heart:before{content:""}.bi-envelope-paper-fill:before{content:""}.bi-envelope-paper-heart-fill:before{content:""}.bi-envelope-paper-heart:before{content:""}.bi-envelope-paper:before{content:""}.bi-filetype-aac:before{content:""}.bi-filetype-ai:before{content:""}.bi-filetype-bmp:before{content:""}.bi-filetype-cs:before{content:""}.bi-filetype-css:before{content:""}.bi-filetype-csv:before{content:""}.bi-filetype-doc:before{content:""}.bi-filetype-docx:before{content:""}.bi-filetype-exe:before{content:""}.bi-filetype-gif:before{content:""}.bi-filetype-heic:before{content:""}.bi-filetype-html:before{content:""}.bi-filetype-java:before{content:""}.bi-filetype-jpg:before{content:""}.bi-filetype-js:before{content:""}.bi-filetype-jsx:before{content:""}.bi-filetype-key:before{content:""}.bi-filetype-m4p:before{content:""}.bi-filetype-md:before{content:""}.bi-filetype-mdx:before{content:""}.bi-filetype-mov:before{content:""}.bi-filetype-mp3:before{content:""}.bi-filetype-mp4:before{content:""}.bi-filetype-otf:before{content:""}.bi-filetype-pdf:before{content:""}.bi-filetype-php:before{content:""}.bi-filetype-png:before{content:""}.bi-filetype-ppt:before{content:""}.bi-filetype-psd:before{content:""}.bi-filetype-py:before{content:""}.bi-filetype-raw:before{content:""}.bi-filetype-rb:before{content:""}.bi-filetype-sass:before{content:""}.bi-filetype-scss:before{content:""}.bi-filetype-sh:before{content:""}.bi-filetype-svg:before{content:""}.bi-filetype-tiff:before{content:""}.bi-filetype-tsx:before{content:""}.bi-filetype-ttf:before{content:""}.bi-filetype-txt:before{content:""}.bi-filetype-wav:before{content:""}.bi-filetype-woff:before{content:""}.bi-filetype-xls:before{content:""}.bi-filetype-xml:before{content:""}.bi-filetype-yml:before{content:""}.bi-heart-arrow:before{content:""}.bi-heart-pulse-fill:before{content:""}.bi-heart-pulse:before{content:""}.bi-heartbreak-fill:before{content:""}.bi-heartbreak:before{content:""}.bi-hearts:before{content:""}.bi-hospital-fill:before{content:""}.bi-hospital:before{content:""}.bi-house-heart-fill:before{content:""}.bi-house-heart:before{content:""}.bi-incognito:before{content:""}.bi-magnet-fill:before{content:""}.bi-magnet:before{content:""}.bi-person-heart:before{content:""}.bi-person-hearts:before{content:""}.bi-phone-flip:before{content:""}.bi-plugin:before{content:""}.bi-postage-fill:before{content:""}.bi-postage-heart-fill:before{content:""}.bi-postage-heart:before{content:""}.bi-postage:before{content:""}.bi-postcard-fill:before{content:""}.bi-postcard-heart-fill:before{content:""}.bi-postcard-heart:before{content:""}.bi-postcard:before{content:""}.bi-search-heart-fill:before{content:""}.bi-search-heart:before{content:""}.bi-sliders2-vertical:before{content:""}.bi-sliders2:before{content:""}.bi-trash3-fill:before{content:""}.bi-trash3:before{content:""}.bi-valentine:before{content:""}.bi-valentine2:before{content:""}.bi-wrench-adjustable-circle-fill:before{content:""}.bi-wrench-adjustable-circle:before{content:""}.bi-wrench-adjustable:before{content:""}.bi-filetype-json:before{content:""}.bi-filetype-pptx:before{content:""}.bi-filetype-xlsx:before{content:""}.bi-1-circle-fill:before{content:""}.bi-1-circle:before{content:""}.bi-1-square-fill:before{content:""}.bi-1-square:before{content:""}.bi-2-circle-fill:before{content:""}.bi-2-circle:before{content:""}.bi-2-square-fill:before{content:""}.bi-2-square:before{content:""}.bi-3-circle-fill:before{content:""}.bi-3-circle:before{content:""}.bi-3-square-fill:before{content:""}.bi-3-square:before{content:""}.bi-4-circle-fill:before{content:""}.bi-4-circle:before{content:""}.bi-4-square-fill:before{content:""}.bi-4-square:before{content:""}.bi-5-circle-fill:before{content:""}.bi-5-circle:before{content:""}.bi-5-square-fill:before{content:""}.bi-5-square:before{content:""}.bi-6-circle-fill:before{content:""}.bi-6-circle:before{content:""}.bi-6-square-fill:before{content:""}.bi-6-square:before{content:""}.bi-7-circle-fill:before{content:""}.bi-7-circle:before{content:""}.bi-7-square-fill:before{content:""}.bi-7-square:before{content:""}.bi-8-circle-fill:before{content:""}.bi-8-circle:before{content:""}.bi-8-square-fill:before{content:""}.bi-8-square:before{content:""}.bi-9-circle-fill:before{content:""}.bi-9-circle:before{content:""}.bi-9-square-fill:before{content:""}.bi-9-square:before{content:""}.bi-airplane-engines-fill:before{content:""}.bi-airplane-engines:before{content:""}.bi-airplane-fill:before{content:""}.bi-airplane:before{content:""}.bi-alexa:before{content:""}.bi-alipay:before{content:""}.bi-android:before{content:""}.bi-android2:before{content:""}.bi-box-fill:before{content:""}.bi-box-seam-fill:before{content:""}.bi-browser-chrome:before{content:""}.bi-browser-edge:before{content:""}.bi-browser-firefox:before{content:""}.bi-browser-safari:before{content:""}.bi-c-circle-fill:before{content:""}.bi-c-circle:before{content:""}.bi-c-square-fill:before{content:""}.bi-c-square:before{content:""}.bi-capsule-pill:before{content:""}.bi-capsule:before{content:""}.bi-car-front-fill:before{content:""}.bi-car-front:before{content:""}.bi-cassette-fill:before{content:""}.bi-cassette:before{content:""}.bi-cc-circle-fill:before{content:""}.bi-cc-circle:before{content:""}.bi-cc-square-fill:before{content:""}.bi-cc-square:before{content:""}.bi-cup-hot-fill:before{content:""}.bi-cup-hot:before{content:""}.bi-currency-rupee:before{content:""}.bi-dropbox:before{content:""}.bi-escape:before{content:""}.bi-fast-forward-btn-fill:before{content:""}.bi-fast-forward-btn:before{content:""}.bi-fast-forward-circle-fill:before{content:""}.bi-fast-forward-circle:before{content:""}.bi-fast-forward-fill:before{content:""}.bi-fast-forward:before{content:""}.bi-filetype-sql:before{content:""}.bi-fire:before{content:""}.bi-google-play:before{content:""}.bi-h-circle-fill:before{content:""}.bi-h-circle:before{content:""}.bi-h-square-fill:before{content:""}.bi-h-square:before{content:""}.bi-indent:before{content:""}.bi-lungs-fill:before{content:""}.bi-lungs:before{content:""}.bi-microsoft-teams:before{content:""}.bi-p-circle-fill:before{content:""}.bi-p-circle:before{content:""}.bi-p-square-fill:before{content:""}.bi-p-square:before{content:""}.bi-pass-fill:before{content:""}.bi-pass:before{content:""}.bi-prescription:before{content:""}.bi-prescription2:before{content:""}.bi-r-circle-fill:before{content:""}.bi-r-circle:before{content:""}.bi-r-square-fill:before{content:""}.bi-r-square:before{content:""}.bi-repeat-1:before{content:""}.bi-repeat:before{content:""}.bi-rewind-btn-fill:before{content:""}.bi-rewind-btn:before{content:""}.bi-rewind-circle-fill:before{content:""}.bi-rewind-circle:before{content:""}.bi-rewind-fill:before{content:""}.bi-rewind:before{content:""}.bi-train-freight-front-fill:before{content:""}.bi-train-freight-front:before{content:""}.bi-train-front-fill:before{content:""}.bi-train-front:before{content:""}.bi-train-lightrail-front-fill:before{content:""}.bi-train-lightrail-front:before{content:""}.bi-truck-front-fill:before{content:""}.bi-truck-front:before{content:""}.bi-ubuntu:before{content:""}.bi-unindent:before{content:""}.bi-unity:before{content:""}.bi-universal-access-circle:before{content:""}.bi-universal-access:before{content:""}.bi-virus:before{content:""}.bi-virus2:before{content:""}.bi-wechat:before{content:""}.bi-yelp:before{content:""}.bi-sign-stop-fill:before{content:""}.bi-sign-stop-lights-fill:before{content:""}.bi-sign-stop-lights:before{content:""}.bi-sign-stop:before{content:""}.bi-sign-turn-left-fill:before{content:""}.bi-sign-turn-left:before{content:""}.bi-sign-turn-right-fill:before{content:""}.bi-sign-turn-right:before{content:""}.bi-sign-turn-slight-left-fill:before{content:""}.bi-sign-turn-slight-left:before{content:""}.bi-sign-turn-slight-right-fill:before{content:""}.bi-sign-turn-slight-right:before{content:""}.bi-sign-yield-fill:before{content:""}.bi-sign-yield:before{content:""}.bi-ev-station-fill:before{content:""}.bi-ev-station:before{content:""}.bi-fuel-pump-diesel-fill:before{content:""}.bi-fuel-pump-diesel:before{content:""}.bi-fuel-pump-fill:before{content:""}.bi-fuel-pump:before{content:""}.bi-0-circle-fill:before{content:""}.bi-0-circle:before{content:""}.bi-0-square-fill:before{content:""}.bi-0-square:before{content:""}.bi-rocket-fill:before{content:""}.bi-rocket-takeoff-fill:before{content:""}.bi-rocket-takeoff:before{content:""}.bi-rocket:before{content:""}.bi-stripe:before{content:""}.bi-subscript:before{content:""}.bi-superscript:before{content:""}.bi-trello:before{content:""}.bi-envelope-at-fill:before{content:""}.bi-envelope-at:before{content:""}.bi-regex:before{content:""}.bi-text-wrap:before{content:""}.bi-sign-dead-end-fill:before{content:""}.bi-sign-dead-end:before{content:""}.bi-sign-do-not-enter-fill:before{content:""}.bi-sign-do-not-enter:before{content:""}.bi-sign-intersection-fill:before{content:""}.bi-sign-intersection-side-fill:before{content:""}.bi-sign-intersection-side:before{content:""}.bi-sign-intersection-t-fill:before{content:""}.bi-sign-intersection-t:before{content:""}.bi-sign-intersection-y-fill:before{content:""}.bi-sign-intersection-y:before{content:""}.bi-sign-intersection:before{content:""}.bi-sign-merge-left-fill:before{content:""}.bi-sign-merge-left:before{content:""}.bi-sign-merge-right-fill:before{content:""}.bi-sign-merge-right:before{content:""}.bi-sign-no-left-turn-fill:before{content:""}.bi-sign-no-left-turn:before{content:""}.bi-sign-no-parking-fill:before{content:""}.bi-sign-no-parking:before{content:""}.bi-sign-no-right-turn-fill:before{content:""}.bi-sign-no-right-turn:before{content:""}.bi-sign-railroad-fill:before{content:""}.bi-sign-railroad:before{content:""}.bi-building-add:before{content:""}.bi-building-check:before{content:""}.bi-building-dash:before{content:""}.bi-building-down:before{content:""}.bi-building-exclamation:before{content:""}.bi-building-fill-add:before{content:""}.bi-building-fill-check:before{content:""}.bi-building-fill-dash:before{content:""}.bi-building-fill-down:before{content:""}.bi-building-fill-exclamation:before{content:""}.bi-building-fill-gear:before{content:""}.bi-building-fill-lock:before{content:""}.bi-building-fill-slash:before{content:""}.bi-building-fill-up:before{content:""}.bi-building-fill-x:before{content:""}.bi-building-fill:before{content:""}.bi-building-gear:before{content:""}.bi-building-lock:before{content:""}.bi-building-slash:before{content:""}.bi-building-up:before{content:""}.bi-building-x:before{content:""}.bi-buildings-fill:before{content:""}.bi-buildings:before{content:""}.bi-bus-front-fill:before{content:""}.bi-bus-front:before{content:""}.bi-ev-front-fill:before{content:""}.bi-ev-front:before{content:""}.bi-globe-americas:before{content:""}.bi-globe-asia-australia:before{content:""}.bi-globe-central-south-asia:before{content:""}.bi-globe-europe-africa:before{content:""}.bi-house-add-fill:before{content:""}.bi-house-add:before{content:""}.bi-house-check-fill:before{content:""}.bi-house-check:before{content:""}.bi-house-dash-fill:before{content:""}.bi-house-dash:before{content:""}.bi-house-down-fill:before{content:""}.bi-house-down:before{content:""}.bi-house-exclamation-fill:before{content:""}.bi-house-exclamation:before{content:""}.bi-house-gear-fill:before{content:""}.bi-house-gear:before{content:""}.bi-house-lock-fill:before{content:""}.bi-house-lock:before{content:""}.bi-house-slash-fill:before{content:""}.bi-house-slash:before{content:""}.bi-house-up-fill:before{content:""}.bi-house-up:before{content:""}.bi-house-x-fill:before{content:""}.bi-house-x:before{content:""}.bi-person-add:before{content:""}.bi-person-down:before{content:""}.bi-person-exclamation:before{content:""}.bi-person-fill-add:before{content:""}.bi-person-fill-check:before{content:""}.bi-person-fill-dash:before{content:""}.bi-person-fill-down:before{content:""}.bi-person-fill-exclamation:before{content:""}.bi-person-fill-gear:before{content:""}.bi-person-fill-lock:before{content:""}.bi-person-fill-slash:before{content:""}.bi-person-fill-up:before{content:""}.bi-person-fill-x:before{content:""}.bi-person-gear:before{content:""}.bi-person-lock:before{content:""}.bi-person-slash:before{content:""}.bi-person-up:before{content:""}.bi-scooter:before{content:""}.bi-taxi-front-fill:before{content:""}.bi-taxi-front:before{content:""}.bi-amd:before{content:""}.bi-database-add:before{content:""}.bi-database-check:before{content:""}.bi-database-dash:before{content:""}.bi-database-down:before{content:""}.bi-database-exclamation:before{content:""}.bi-database-fill-add:before{content:""}.bi-database-fill-check:before{content:""}.bi-database-fill-dash:before{content:""}.bi-database-fill-down:before{content:""}.bi-database-fill-exclamation:before{content:""}.bi-database-fill-gear:before{content:""}.bi-database-fill-lock:before{content:""}.bi-database-fill-slash:before{content:""}.bi-database-fill-up:before{content:""}.bi-database-fill-x:before{content:""}.bi-database-fill:before{content:""}.bi-database-gear:before{content:""}.bi-database-lock:before{content:""}.bi-database-slash:before{content:""}.bi-database-up:before{content:""}.bi-database-x:before{content:""}.bi-database:before{content:""}.bi-houses-fill:before{content:""}.bi-houses:before{content:""}.bi-nvidia:before{content:""}.bi-person-vcard-fill:before{content:""}.bi-person-vcard:before{content:""}.bi-sina-weibo:before{content:""}.bi-tencent-qq:before{content:""}.bi-wikipedia:before{content:""}.bi-alphabet-uppercase:before{content:""}.bi-alphabet:before{content:""}.bi-amazon:before{content:""}.bi-arrows-collapse-vertical:before{content:""}.bi-arrows-expand-vertical:before{content:""}.bi-arrows-vertical:before{content:""}.bi-arrows:before{content:""}.bi-ban-fill:before{content:""}.bi-ban:before{content:""}.bi-bing:before{content:""}.bi-cake:before{content:""}.bi-cake2:before{content:""}.bi-cookie:before{content:""}.bi-copy:before{content:""}.bi-crosshair:before{content:""}.bi-crosshair2:before{content:""}.bi-emoji-astonished-fill:before{content:""}.bi-emoji-astonished:before{content:""}.bi-emoji-grimace-fill:before{content:""}.bi-emoji-grimace:before{content:""}.bi-emoji-grin-fill:before{content:""}.bi-emoji-grin:before{content:""}.bi-emoji-surprise-fill:before{content:""}.bi-emoji-surprise:before{content:""}.bi-emoji-tear-fill:before{content:""}.bi-emoji-tear:before{content:""}.bi-envelope-arrow-down-fill:before{content:""}.bi-envelope-arrow-down:before{content:""}.bi-envelope-arrow-up-fill:before{content:""}.bi-envelope-arrow-up:before{content:""}.bi-feather:before{content:""}.bi-feather2:before{content:""}.bi-floppy-fill:before{content:""}.bi-floppy:before{content:""}.bi-floppy2-fill:before{content:""}.bi-floppy2:before{content:""}.bi-gitlab:before{content:""}.bi-highlighter:before{content:""}.bi-marker-tip:before{content:""}.bi-nvme-fill:before{content:""}.bi-nvme:before{content:""}.bi-opencollective:before{content:""}.bi-pci-card-network:before{content:""}.bi-pci-card-sound:before{content:""}.bi-radar:before{content:""}.bi-send-arrow-down-fill:before{content:""}.bi-send-arrow-down:before{content:""}.bi-send-arrow-up-fill:before{content:""}.bi-send-arrow-up:before{content:""}.bi-sim-slash-fill:before{content:""}.bi-sim-slash:before{content:""}.bi-sourceforge:before{content:""}.bi-substack:before{content:""}.bi-threads-fill:before{content:""}.bi-threads:before{content:""}.bi-transparency:before{content:""}.bi-twitter-x:before{content:""}.bi-type-h4:before{content:""}.bi-type-h5:before{content:""}.bi-type-h6:before{content:""}.bi-backpack-fill:before{content:""}.bi-backpack:before{content:""}.bi-backpack2-fill:before{content:""}.bi-backpack2:before{content:""}.bi-backpack3-fill:before{content:""}.bi-backpack3:before{content:""}.bi-backpack4-fill:before{content:""}.bi-backpack4:before{content:""}.bi-brilliance:before{content:""}.bi-cake-fill:before{content:""}.bi-cake2-fill:before{content:""}.bi-duffle-fill:before{content:""}.bi-duffle:before{content:""}.bi-exposure:before{content:""}.bi-gender-neuter:before{content:""}.bi-highlights:before{content:""}.bi-luggage-fill:before{content:""}.bi-luggage:before{content:""}.bi-mailbox-flag:before{content:""}.bi-mailbox2-flag:before{content:""}.bi-noise-reduction:before{content:""}.bi-passport-fill:before{content:""}.bi-passport:before{content:""}.bi-person-arms-up:before{content:""}.bi-person-raised-hand:before{content:""}.bi-person-standing-dress:before{content:""}.bi-person-standing:before{content:""}.bi-person-walking:before{content:""}.bi-person-wheelchair:before{content:""}.bi-shadows:before{content:""}.bi-suitcase-fill:before{content:""}.bi-suitcase-lg-fill:before{content:""}.bi-suitcase-lg:before{content:""}.bi-suitcase:before{content:"豈"}.bi-suitcase2-fill:before{content:"更"}.bi-suitcase2:before{content:"車"}.bi-vignette:before{content:"賈"}.pvtUi{color:#333}table.pvtTable{font-size:8pt;text-align:left;border-collapse:collapse}table.pvtTable thead tr th,table.pvtTable tbody tr th{background-color:#e6eeee;border:1px solid #CDCDCD;font-size:8pt;padding:5px}table.pvtTable .pvtColLabel{text-align:center}table.pvtTable .pvtTotalLabel{text-align:right}table.pvtTable tbody tr td{color:#3d3d3d;padding:5px;background-color:#fff;border:1px solid #CDCDCD;vertical-align:top;text-align:right}.pvtTotal,.pvtGrandTotal{font-weight:700}.pvtVals{text-align:center;white-space:nowrap}.pvtRowOrder,.pvtColOrder{cursor:pointer;width:15px;margin-left:5px;display:inline-block}.pvtAggregator{margin-bottom:5px}.pvtAxisContainer,.pvtVals{border:1px solid gray;background:#eee;padding:5px;min-width:20px;min-height:20px;user-select:none;-webkit-user-select:none;-moz-user-select:none;-khtml-user-select:none;-ms-user-select:none}.pvtAxisContainer li{padding:8px 6px;list-style-type:none;cursor:move}.pvtAxisContainer li.pvtPlaceholder{-webkit-border-radius:5px;padding:3px 15px;-moz-border-radius:5px;border-radius:5px;border:1px dashed #aaa}.pvtAxisContainer li span.pvtAttr{-webkit-text-size-adjust:100%;background:#f3f3f3;border:1px solid #DEDEDE;padding:2px 5px;white-space:nowrap;-webkit-border-radius:5px;-moz-border-radius:5px;border-radius:5px}.pvtTriangle{cursor:pointer;color:gray}.pvtHorizList li{display:inline}.pvtVertList{vertical-align:top}.pvtFilteredAttribute{font-style:italic}.pvtFilterBox{z-index:100;width:300px;border:1px solid gray;background-color:#fff;position:absolute;text-align:center}.pvtFilterBox h4{margin:15px}.pvtFilterBox p{margin:10px auto}.pvtFilterBox label{font-weight:400}.pvtFilterBox input[type=checkbox]{margin-right:10px;margin-left:10px}.pvtFilterBox input[type=text]{width:230px}.pvtFilterBox .count{color:gray;font-weight:400;margin-left:3px}.pvtCheckContainer{text-align:left;font-size:14px;white-space:nowrap;overflow-y:scroll;width:100%;max-height:250px;border-top:1px solid lightgrey;border-bottom:1px solid lightgrey}.pvtCheckContainer p{margin:5px}.pvtRendererArea{padding:5px}:root,[data-bs-theme=light]{--bs-blue: #0d6efd;--bs-indigo: #6610f2;--bs-purple: #6f42c1;--bs-pink: #d63384;--bs-red: #dc3545;--bs-orange: #fd7e14;--bs-yellow: #ffc107;--bs-green: #198754;--bs-teal: #20c997;--bs-cyan: #0dcaf0;--bs-black: #000;--bs-white: #fff;--bs-gray: #6c757d;--bs-gray-dark: #343a40;--bs-gray-100: #f8f9fa;--bs-gray-200: #e9ecef;--bs-gray-300: #dee2e6;--bs-gray-400: #ced4da;--bs-gray-500: #adb5bd;--bs-gray-600: #6c757d;--bs-gray-700: #495057;--bs-gray-800: #343a40;--bs-gray-900: #212529;--bs-primary: #0d6efd;--bs-secondary: #6c757d;--bs-success: #198754;--bs-info: #0dcaf0;--bs-warning: #ffc107;--bs-danger: #dc3545;--bs-light: #f8f9fa;--bs-dark: #212529;--bs-primary-rgb: 13, 110, 253;--bs-secondary-rgb: 108, 117, 125;--bs-success-rgb: 25, 135, 84;--bs-info-rgb: 13, 202, 240;--bs-warning-rgb: 255, 193, 7;--bs-danger-rgb: 220, 53, 69;--bs-light-rgb: 248, 249, 250;--bs-dark-rgb: 33, 37, 41;--bs-primary-text-emphasis: #052c65;--bs-secondary-text-emphasis: #2b2f32;--bs-success-text-emphasis: #0a3622;--bs-info-text-emphasis: #055160;--bs-warning-text-emphasis: #664d03;--bs-danger-text-emphasis: #58151c;--bs-light-text-emphasis: #495057;--bs-dark-text-emphasis: #495057;--bs-primary-bg-subtle: #cfe2ff;--bs-secondary-bg-subtle: #e2e3e5;--bs-success-bg-subtle: #d1e7dd;--bs-info-bg-subtle: #cff4fc;--bs-warning-bg-subtle: #fff3cd;--bs-danger-bg-subtle: #f8d7da;--bs-light-bg-subtle: #fcfcfd;--bs-dark-bg-subtle: #ced4da;--bs-primary-border-subtle: #9ec5fe;--bs-secondary-border-subtle: #c4c8cb;--bs-success-border-subtle: #a3cfbb;--bs-info-border-subtle: #9eeaf9;--bs-warning-border-subtle: #ffe69c;--bs-danger-border-subtle: #f1aeb5;--bs-light-border-subtle: #e9ecef;--bs-dark-border-subtle: #adb5bd;--bs-white-rgb: 255, 255, 255;--bs-black-rgb: 0, 0, 0;--bs-font-sans-serif: system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", "Liberation Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";--bs-font-monospace: SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;--bs-gradient: linear-gradient(180deg, rgba(255, 255, 255, .15), rgba(255, 255, 255, 0));--bs-body-font-family: var(--bs-font-sans-serif);--bs-body-font-size: 1rem;--bs-body-font-weight: 400;--bs-body-line-height: 1.5;--bs-body-color: #212529;--bs-body-color-rgb: 33, 37, 41;--bs-body-bg: #fff;--bs-body-bg-rgb: 255, 255, 255;--bs-emphasis-color: #000;--bs-emphasis-color-rgb: 0, 0, 0;--bs-secondary-color: rgba(33, 37, 41, .75);--bs-secondary-color-rgb: 33, 37, 41;--bs-secondary-bg: #e9ecef;--bs-secondary-bg-rgb: 233, 236, 239;--bs-tertiary-color: rgba(33, 37, 41, .5);--bs-tertiary-color-rgb: 33, 37, 41;--bs-tertiary-bg: #f8f9fa;--bs-tertiary-bg-rgb: 248, 249, 250;--bs-heading-color: inherit;--bs-link-color: #0d6efd;--bs-link-color-rgb: 13, 110, 253;--bs-link-decoration: underline;--bs-link-hover-color: #0a58ca;--bs-link-hover-color-rgb: 10, 88, 202;--bs-code-color: #d63384;--bs-highlight-color: #212529;--bs-highlight-bg: #fff3cd;--bs-border-width: 1px;--bs-border-style: solid;--bs-border-color: #dee2e6;--bs-border-color-translucent: rgba(0, 0, 0, .175);--bs-border-radius: .375rem;--bs-border-radius-sm: .25rem;--bs-border-radius-lg: .5rem;--bs-border-radius-xl: 1rem;--bs-border-radius-xxl: 2rem;--bs-border-radius-2xl: var(--bs-border-radius-xxl);--bs-border-radius-pill: 50rem;--bs-box-shadow: 0 .5rem 1rem rgba(0, 0, 0, .15);--bs-box-shadow-sm: 0 .125rem .25rem rgba(0, 0, 0, .075);--bs-box-shadow-lg: 0 1rem 3rem rgba(0, 0, 0, .175);--bs-box-shadow-inset: inset 0 1px 2px rgba(0, 0, 0, .075);--bs-focus-ring-width: .25rem;--bs-focus-ring-opacity: .25;--bs-focus-ring-color: rgba(13, 110, 253, .25);--bs-form-valid-color: #198754;--bs-form-valid-border-color: #198754;--bs-form-invalid-color: #dc3545;--bs-form-invalid-border-color: #dc3545}[data-bs-theme=dark]{color-scheme:dark;--bs-body-color: #dee2e6;--bs-body-color-rgb: 222, 226, 230;--bs-body-bg: #212529;--bs-body-bg-rgb: 33, 37, 41;--bs-emphasis-color: #fff;--bs-emphasis-color-rgb: 255, 255, 255;--bs-secondary-color: rgba(222, 226, 230, .75);--bs-secondary-color-rgb: 222, 226, 230;--bs-secondary-bg: #343a40;--bs-secondary-bg-rgb: 52, 58, 64;--bs-tertiary-color: rgba(222, 226, 230, .5);--bs-tertiary-color-rgb: 222, 226, 230;--bs-tertiary-bg: #2b3035;--bs-tertiary-bg-rgb: 43, 48, 53;--bs-primary-text-emphasis: #6ea8fe;--bs-secondary-text-emphasis: #a7acb1;--bs-success-text-emphasis: #75b798;--bs-info-text-emphasis: #6edff6;--bs-warning-text-emphasis: #ffda6a;--bs-danger-text-emphasis: #ea868f;--bs-light-text-emphasis: #f8f9fa;--bs-dark-text-emphasis: #dee2e6;--bs-primary-bg-subtle: #031633;--bs-secondary-bg-subtle: #161719;--bs-success-bg-subtle: #051b11;--bs-info-bg-subtle: #032830;--bs-warning-bg-subtle: #332701;--bs-danger-bg-subtle: #2c0b0e;--bs-light-bg-subtle: #343a40;--bs-dark-bg-subtle: #1a1d20;--bs-primary-border-subtle: #084298;--bs-secondary-border-subtle: #41464b;--bs-success-border-subtle: #0f5132;--bs-info-border-subtle: #087990;--bs-warning-border-subtle: #997404;--bs-danger-border-subtle: #842029;--bs-light-border-subtle: #495057;--bs-dark-border-subtle: #343a40;--bs-heading-color: inherit;--bs-link-color: #6ea8fe;--bs-link-hover-color: #8bb9fe;--bs-link-color-rgb: 110, 168, 254;--bs-link-hover-color-rgb: 139, 185, 254;--bs-code-color: #e685b5;--bs-highlight-color: #dee2e6;--bs-highlight-bg: #664d03;--bs-border-color: #495057;--bs-border-color-translucent: rgba(255, 255, 255, .15);--bs-form-valid-color: #75b798;--bs-form-valid-border-color: #75b798;--bs-form-invalid-color: #ea868f;--bs-form-invalid-border-color: #ea868f}*,*:before,*:after{box-sizing:border-box}@media (prefers-reduced-motion: no-preference){:root{scroll-behavior:smooth}}body{margin:0;font-family:var(--bs-body-font-family);font-size:var(--bs-body-font-size);font-weight:var(--bs-body-font-weight);line-height:var(--bs-body-line-height);color:var(--bs-body-color);text-align:var(--bs-body-text-align);background-color:var(--bs-body-bg);-webkit-text-size-adjust:100%;-webkit-tap-highlight-color:rgba(0,0,0,0)}hr{margin:1rem 0;color:inherit;border:0;border-top:var(--bs-border-width) solid;opacity:.25}h6,.h6,h5,.h5,h4,.h4,h3,.h3,h2,.h2,h1,.h1{margin-top:0;margin-bottom:.5rem;font-weight:500;line-height:1.2;color:var(--bs-heading-color)}h1,.h1{font-size:calc(1.375rem + 1.5vw)}@media (min-width: 1200px){h1,.h1{font-size:2.5rem}}h2,.h2{font-size:calc(1.325rem + .9vw)}@media (min-width: 1200px){h2,.h2{font-size:2rem}}h3,.h3{font-size:calc(1.3rem + .6vw)}@media (min-width: 1200px){h3,.h3{font-size:1.75rem}}h4,.h4{font-size:calc(1.275rem + .3vw)}@media (min-width: 1200px){h4,.h4{font-size:1.5rem}}h5,.h5{font-size:1.25rem}h6,.h6{font-size:1rem}p{margin-top:0;margin-bottom:1rem}abbr[title]{text-decoration:underline dotted;cursor:help;text-decoration-skip-ink:none}address{margin-bottom:1rem;font-style:normal;line-height:inherit}ol,ul{padding-left:2rem}ol,ul,dl{margin-top:0;margin-bottom:1rem}ol ol,ul ul,ol ul,ul ol{margin-bottom:0}dt{font-weight:700}dd{margin-bottom:.5rem;margin-left:0}blockquote{margin:0 0 1rem}b,strong{font-weight:bolder}small,.small{font-size:.875em}mark,.mark{padding:.1875em;color:var(--bs-highlight-color);background-color:var(--bs-highlight-bg)}sub,sup{position:relative;font-size:.75em;line-height:0;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}a{color:rgba(var(--bs-link-color-rgb),var(--bs-link-opacity, 1));text-decoration:underline}a:hover{--bs-link-color-rgb: var(--bs-link-hover-color-rgb)}a:not([href]):not([class]),a:not([href]):not([class]):hover{color:inherit;text-decoration:none}pre,code,kbd,samp{font-family:var(--bs-font-monospace);font-size:1em}pre{display:block;margin-top:0;margin-bottom:1rem;overflow:auto;font-size:.875em}pre code{font-size:inherit;color:inherit;word-break:normal}code{font-size:.875em;color:var(--bs-code-color);word-wrap:break-word}a>code{color:inherit}kbd{padding:.1875rem .375rem;font-size:.875em;color:var(--bs-body-bg);background-color:var(--bs-body-color);border-radius:.25rem}kbd kbd{padding:0;font-size:1em}figure{margin:0 0 1rem}img,svg{vertical-align:middle}table{caption-side:bottom;border-collapse:collapse}caption{padding-top:.5rem;padding-bottom:.5rem;color:var(--bs-secondary-color);text-align:left}th{text-align:inherit;text-align:-webkit-match-parent}thead,tbody,tfoot,tr,td,th{border-color:inherit;border-style:solid;border-width:0}label{display:inline-block}button{border-radius:0}button:focus:not(:focus-visible){outline:0}input,button,select,optgroup,textarea{margin:0;font-family:inherit;font-size:inherit;line-height:inherit}button,select{text-transform:none}[role=button]{cursor:pointer}select{word-wrap:normal}select:disabled{opacity:1}[list]:not([type=date]):not([type=datetime-local]):not([type=month]):not([type=week]):not([type=time])::-webkit-calendar-picker-indicator{display:none!important}button,[type=button],[type=reset],[type=submit]{-webkit-appearance:button}button:not(:disabled),[type=button]:not(:disabled),[type=reset]:not(:disabled),[type=submit]:not(:disabled){cursor:pointer}::-moz-focus-inner{padding:0;border-style:none}textarea{resize:vertical}fieldset{min-width:0;padding:0;margin:0;border:0}legend{float:left;width:100%;padding:0;margin-bottom:.5rem;font-size:calc(1.275rem + .3vw);line-height:inherit}@media (min-width: 1200px){legend{font-size:1.5rem}}legend+*{clear:left}::-webkit-datetime-edit-fields-wrapper,::-webkit-datetime-edit-text,::-webkit-datetime-edit-minute,::-webkit-datetime-edit-hour-field,::-webkit-datetime-edit-day-field,::-webkit-datetime-edit-month-field,::-webkit-datetime-edit-year-field{padding:0}::-webkit-inner-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-color-swatch-wrapper{padding:0}::file-selector-button{font:inherit;-webkit-appearance:button}output{display:inline-block}iframe{border:0}summary{display:list-item;cursor:pointer}progress{vertical-align:baseline}[hidden]{display:none!important}.lead{font-size:1.25rem;font-weight:300}.display-1{font-size:calc(1.625rem + 4.5vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-1{font-size:5rem}}.display-2{font-size:calc(1.575rem + 3.9vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-2{font-size:4.5rem}}.display-3{font-size:calc(1.525rem + 3.3vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-3{font-size:4rem}}.display-4{font-size:calc(1.475rem + 2.7vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-4{font-size:3.5rem}}.display-5{font-size:calc(1.425rem + 2.1vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-5{font-size:3rem}}.display-6{font-size:calc(1.375rem + 1.5vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-6{font-size:2.5rem}}.list-unstyled,.list-inline{padding-left:0;list-style:none}.list-inline-item{display:inline-block}.list-inline-item:not(:last-child){margin-right:.5rem}.initialism{font-size:.875em;text-transform:uppercase}.blockquote{margin-bottom:1rem;font-size:1.25rem}.blockquote>:last-child{margin-bottom:0}.blockquote-footer{margin-top:-1rem;margin-bottom:1rem;font-size:.875em;color:#6c757d}.blockquote-footer:before{content:"— "}.img-fluid{max-width:100%;height:auto}.img-thumbnail{padding:.25rem;background-color:var(--bs-body-bg);border:var(--bs-border-width) solid var(--bs-border-color);border-radius:var(--bs-border-radius);max-width:100%;height:auto}.figure{display:inline-block}.figure-img{margin-bottom:.5rem;line-height:1}.figure-caption{font-size:.875em;color:var(--bs-secondary-color)}.container,.container-fluid,.container-xxl,.container-xl,.container-lg,.container-md,.container-sm{--bs-gutter-x: 1.5rem;--bs-gutter-y: 0;width:100%;padding-right:calc(var(--bs-gutter-x) * .5);padding-left:calc(var(--bs-gutter-x) * .5);margin-right:auto;margin-left:auto}@media (min-width: 576px){.container-sm,.container{max-width:540px}}@media (min-width: 768px){.container-md,.container-sm,.container{max-width:720px}}@media (min-width: 992px){.container-lg,.container-md,.container-sm,.container{max-width:960px}}@media (min-width: 1200px){.container-xl,.container-lg,.container-md,.container-sm,.container{max-width:1140px}}@media (min-width: 1400px){.container-xxl,.container-xl,.container-lg,.container-md,.container-sm,.container{max-width:1320px}}:root{--bs-breakpoint-xs: 0;--bs-breakpoint-sm: 576px;--bs-breakpoint-md: 768px;--bs-breakpoint-lg: 992px;--bs-breakpoint-xl: 1200px;--bs-breakpoint-xxl: 1400px}.row{--bs-gutter-x: 1.5rem;--bs-gutter-y: 0;display:flex;flex-wrap:wrap;margin-top:calc(-1 * var(--bs-gutter-y));margin-right:calc(-.5 * var(--bs-gutter-x));margin-left:calc(-.5 * var(--bs-gutter-x))}.row>*{flex-shrink:0;width:100%;max-width:100%;padding-right:calc(var(--bs-gutter-x) * .5);padding-left:calc(var(--bs-gutter-x) * .5);margin-top:var(--bs-gutter-y)}.col{flex:1 0 0%}.row-cols-auto>*{flex:0 0 auto;width:auto}.row-cols-1>*{flex:0 0 auto;width:100%}.row-cols-2>*{flex:0 0 auto;width:50%}.row-cols-3>*{flex:0 0 auto;width:33.33333333%}.row-cols-4>*{flex:0 0 auto;width:25%}.row-cols-5>*{flex:0 0 auto;width:20%}.row-cols-6>*{flex:0 0 auto;width:16.66666667%}.col-auto{flex:0 0 auto;width:auto}.col-1{flex:0 0 auto;width:8.33333333%}.col-2{flex:0 0 auto;width:16.66666667%}.col-3{flex:0 0 auto;width:25%}.col-4{flex:0 0 auto;width:33.33333333%}.col-5{flex:0 0 auto;width:41.66666667%}.col-6{flex:0 0 auto;width:50%}.col-7{flex:0 0 auto;width:58.33333333%}.col-8{flex:0 0 auto;width:66.66666667%}.col-9{flex:0 0 auto;width:75%}.col-10{flex:0 0 auto;width:83.33333333%}.col-11{flex:0 0 auto;width:91.66666667%}.col-12{flex:0 0 auto;width:100%}.offset-1{margin-left:8.33333333%}.offset-2{margin-left:16.66666667%}.offset-3{margin-left:25%}.offset-4{margin-left:33.33333333%}.offset-5{margin-left:41.66666667%}.offset-6{margin-left:50%}.offset-7{margin-left:58.33333333%}.offset-8{margin-left:66.66666667%}.offset-9{margin-left:75%}.offset-10{margin-left:83.33333333%}.offset-11{margin-left:91.66666667%}.g-0,.gx-0{--bs-gutter-x: 0}.g-0,.gy-0{--bs-gutter-y: 0}.g-1,.gx-1{--bs-gutter-x: .25rem}.g-1,.gy-1{--bs-gutter-y: .25rem}.g-2,.gx-2{--bs-gutter-x: .5rem}.g-2,.gy-2{--bs-gutter-y: .5rem}.g-3,.gx-3{--bs-gutter-x: 1rem}.g-3,.gy-3{--bs-gutter-y: 1rem}.g-4,.gx-4{--bs-gutter-x: 1.5rem}.g-4,.gy-4{--bs-gutter-y: 1.5rem}.g-5,.gx-5{--bs-gutter-x: 3rem}.g-5,.gy-5{--bs-gutter-y: 3rem}@media (min-width: 576px){.col-sm{flex:1 0 0%}.row-cols-sm-auto>*{flex:0 0 auto;width:auto}.row-cols-sm-1>*{flex:0 0 auto;width:100%}.row-cols-sm-2>*{flex:0 0 auto;width:50%}.row-cols-sm-3>*{flex:0 0 auto;width:33.33333333%}.row-cols-sm-4>*{flex:0 0 auto;width:25%}.row-cols-sm-5>*{flex:0 0 auto;width:20%}.row-cols-sm-6>*{flex:0 0 auto;width:16.66666667%}.col-sm-auto{flex:0 0 auto;width:auto}.col-sm-1{flex:0 0 auto;width:8.33333333%}.col-sm-2{flex:0 0 auto;width:16.66666667%}.col-sm-3{flex:0 0 auto;width:25%}.col-sm-4{flex:0 0 auto;width:33.33333333%}.col-sm-5{flex:0 0 auto;width:41.66666667%}.col-sm-6{flex:0 0 auto;width:50%}.col-sm-7{flex:0 0 auto;width:58.33333333%}.col-sm-8{flex:0 0 auto;width:66.66666667%}.col-sm-9{flex:0 0 auto;width:75%}.col-sm-10{flex:0 0 auto;width:83.33333333%}.col-sm-11{flex:0 0 auto;width:91.66666667%}.col-sm-12{flex:0 0 auto;width:100%}.offset-sm-0{margin-left:0}.offset-sm-1{margin-left:8.33333333%}.offset-sm-2{margin-left:16.66666667%}.offset-sm-3{margin-left:25%}.offset-sm-4{margin-left:33.33333333%}.offset-sm-5{margin-left:41.66666667%}.offset-sm-6{margin-left:50%}.offset-sm-7{margin-left:58.33333333%}.offset-sm-8{margin-left:66.66666667%}.offset-sm-9{margin-left:75%}.offset-sm-10{margin-left:83.33333333%}.offset-sm-11{margin-left:91.66666667%}.g-sm-0,.gx-sm-0{--bs-gutter-x: 0}.g-sm-0,.gy-sm-0{--bs-gutter-y: 0}.g-sm-1,.gx-sm-1{--bs-gutter-x: .25rem}.g-sm-1,.gy-sm-1{--bs-gutter-y: .25rem}.g-sm-2,.gx-sm-2{--bs-gutter-x: .5rem}.g-sm-2,.gy-sm-2{--bs-gutter-y: .5rem}.g-sm-3,.gx-sm-3{--bs-gutter-x: 1rem}.g-sm-3,.gy-sm-3{--bs-gutter-y: 1rem}.g-sm-4,.gx-sm-4{--bs-gutter-x: 1.5rem}.g-sm-4,.gy-sm-4{--bs-gutter-y: 1.5rem}.g-sm-5,.gx-sm-5{--bs-gutter-x: 3rem}.g-sm-5,.gy-sm-5{--bs-gutter-y: 3rem}}@media (min-width: 768px){.col-md{flex:1 0 0%}.row-cols-md-auto>*{flex:0 0 auto;width:auto}.row-cols-md-1>*{flex:0 0 auto;width:100%}.row-cols-md-2>*{flex:0 0 auto;width:50%}.row-cols-md-3>*{flex:0 0 auto;width:33.33333333%}.row-cols-md-4>*{flex:0 0 auto;width:25%}.row-cols-md-5>*{flex:0 0 auto;width:20%}.row-cols-md-6>*{flex:0 0 auto;width:16.66666667%}.col-md-auto{flex:0 0 auto;width:auto}.col-md-1{flex:0 0 auto;width:8.33333333%}.col-md-2{flex:0 0 auto;width:16.66666667%}.col-md-3{flex:0 0 auto;width:25%}.col-md-4{flex:0 0 auto;width:33.33333333%}.col-md-5{flex:0 0 auto;width:41.66666667%}.col-md-6{flex:0 0 auto;width:50%}.col-md-7{flex:0 0 auto;width:58.33333333%}.col-md-8{flex:0 0 auto;width:66.66666667%}.col-md-9{flex:0 0 auto;width:75%}.col-md-10{flex:0 0 auto;width:83.33333333%}.col-md-11{flex:0 0 auto;width:91.66666667%}.col-md-12{flex:0 0 auto;width:100%}.offset-md-0{margin-left:0}.offset-md-1{margin-left:8.33333333%}.offset-md-2{margin-left:16.66666667%}.offset-md-3{margin-left:25%}.offset-md-4{margin-left:33.33333333%}.offset-md-5{margin-left:41.66666667%}.offset-md-6{margin-left:50%}.offset-md-7{margin-left:58.33333333%}.offset-md-8{margin-left:66.66666667%}.offset-md-9{margin-left:75%}.offset-md-10{margin-left:83.33333333%}.offset-md-11{margin-left:91.66666667%}.g-md-0,.gx-md-0{--bs-gutter-x: 0}.g-md-0,.gy-md-0{--bs-gutter-y: 0}.g-md-1,.gx-md-1{--bs-gutter-x: .25rem}.g-md-1,.gy-md-1{--bs-gutter-y: .25rem}.g-md-2,.gx-md-2{--bs-gutter-x: .5rem}.g-md-2,.gy-md-2{--bs-gutter-y: .5rem}.g-md-3,.gx-md-3{--bs-gutter-x: 1rem}.g-md-3,.gy-md-3{--bs-gutter-y: 1rem}.g-md-4,.gx-md-4{--bs-gutter-x: 1.5rem}.g-md-4,.gy-md-4{--bs-gutter-y: 1.5rem}.g-md-5,.gx-md-5{--bs-gutter-x: 3rem}.g-md-5,.gy-md-5{--bs-gutter-y: 3rem}}@media (min-width: 992px){.col-lg{flex:1 0 0%}.row-cols-lg-auto>*{flex:0 0 auto;width:auto}.row-cols-lg-1>*{flex:0 0 auto;width:100%}.row-cols-lg-2>*{flex:0 0 auto;width:50%}.row-cols-lg-3>*{flex:0 0 auto;width:33.33333333%}.row-cols-lg-4>*{flex:0 0 auto;width:25%}.row-cols-lg-5>*{flex:0 0 auto;width:20%}.row-cols-lg-6>*{flex:0 0 auto;width:16.66666667%}.col-lg-auto{flex:0 0 auto;width:auto}.col-lg-1{flex:0 0 auto;width:8.33333333%}.col-lg-2{flex:0 0 auto;width:16.66666667%}.col-lg-3{flex:0 0 auto;width:25%}.col-lg-4{flex:0 0 auto;width:33.33333333%}.col-lg-5{flex:0 0 auto;width:41.66666667%}.col-lg-6{flex:0 0 auto;width:50%}.col-lg-7{flex:0 0 auto;width:58.33333333%}.col-lg-8{flex:0 0 auto;width:66.66666667%}.col-lg-9{flex:0 0 auto;width:75%}.col-lg-10{flex:0 0 auto;width:83.33333333%}.col-lg-11{flex:0 0 auto;width:91.66666667%}.col-lg-12{flex:0 0 auto;width:100%}.offset-lg-0{margin-left:0}.offset-lg-1{margin-left:8.33333333%}.offset-lg-2{margin-left:16.66666667%}.offset-lg-3{margin-left:25%}.offset-lg-4{margin-left:33.33333333%}.offset-lg-5{margin-left:41.66666667%}.offset-lg-6{margin-left:50%}.offset-lg-7{margin-left:58.33333333%}.offset-lg-8{margin-left:66.66666667%}.offset-lg-9{margin-left:75%}.offset-lg-10{margin-left:83.33333333%}.offset-lg-11{margin-left:91.66666667%}.g-lg-0,.gx-lg-0{--bs-gutter-x: 0}.g-lg-0,.gy-lg-0{--bs-gutter-y: 0}.g-lg-1,.gx-lg-1{--bs-gutter-x: .25rem}.g-lg-1,.gy-lg-1{--bs-gutter-y: .25rem}.g-lg-2,.gx-lg-2{--bs-gutter-x: .5rem}.g-lg-2,.gy-lg-2{--bs-gutter-y: .5rem}.g-lg-3,.gx-lg-3{--bs-gutter-x: 1rem}.g-lg-3,.gy-lg-3{--bs-gutter-y: 1rem}.g-lg-4,.gx-lg-4{--bs-gutter-x: 1.5rem}.g-lg-4,.gy-lg-4{--bs-gutter-y: 1.5rem}.g-lg-5,.gx-lg-5{--bs-gutter-x: 3rem}.g-lg-5,.gy-lg-5{--bs-gutter-y: 3rem}}@media (min-width: 1200px){.col-xl{flex:1 0 0%}.row-cols-xl-auto>*{flex:0 0 auto;width:auto}.row-cols-xl-1>*{flex:0 0 auto;width:100%}.row-cols-xl-2>*{flex:0 0 auto;width:50%}.row-cols-xl-3>*{flex:0 0 auto;width:33.33333333%}.row-cols-xl-4>*{flex:0 0 auto;width:25%}.row-cols-xl-5>*{flex:0 0 auto;width:20%}.row-cols-xl-6>*{flex:0 0 auto;width:16.66666667%}.col-xl-auto{flex:0 0 auto;width:auto}.col-xl-1{flex:0 0 auto;width:8.33333333%}.col-xl-2{flex:0 0 auto;width:16.66666667%}.col-xl-3{flex:0 0 auto;width:25%}.col-xl-4{flex:0 0 auto;width:33.33333333%}.col-xl-5{flex:0 0 auto;width:41.66666667%}.col-xl-6{flex:0 0 auto;width:50%}.col-xl-7{flex:0 0 auto;width:58.33333333%}.col-xl-8{flex:0 0 auto;width:66.66666667%}.col-xl-9{flex:0 0 auto;width:75%}.col-xl-10{flex:0 0 auto;width:83.33333333%}.col-xl-11{flex:0 0 auto;width:91.66666667%}.col-xl-12{flex:0 0 auto;width:100%}.offset-xl-0{margin-left:0}.offset-xl-1{margin-left:8.33333333%}.offset-xl-2{margin-left:16.66666667%}.offset-xl-3{margin-left:25%}.offset-xl-4{margin-left:33.33333333%}.offset-xl-5{margin-left:41.66666667%}.offset-xl-6{margin-left:50%}.offset-xl-7{margin-left:58.33333333%}.offset-xl-8{margin-left:66.66666667%}.offset-xl-9{margin-left:75%}.offset-xl-10{margin-left:83.33333333%}.offset-xl-11{margin-left:91.66666667%}.g-xl-0,.gx-xl-0{--bs-gutter-x: 0}.g-xl-0,.gy-xl-0{--bs-gutter-y: 0}.g-xl-1,.gx-xl-1{--bs-gutter-x: .25rem}.g-xl-1,.gy-xl-1{--bs-gutter-y: .25rem}.g-xl-2,.gx-xl-2{--bs-gutter-x: .5rem}.g-xl-2,.gy-xl-2{--bs-gutter-y: .5rem}.g-xl-3,.gx-xl-3{--bs-gutter-x: 1rem}.g-xl-3,.gy-xl-3{--bs-gutter-y: 1rem}.g-xl-4,.gx-xl-4{--bs-gutter-x: 1.5rem}.g-xl-4,.gy-xl-4{--bs-gutter-y: 1.5rem}.g-xl-5,.gx-xl-5{--bs-gutter-x: 3rem}.g-xl-5,.gy-xl-5{--bs-gutter-y: 3rem}}@media (min-width: 1400px){.col-xxl{flex:1 0 0%}.row-cols-xxl-auto>*{flex:0 0 auto;width:auto}.row-cols-xxl-1>*{flex:0 0 auto;width:100%}.row-cols-xxl-2>*{flex:0 0 auto;width:50%}.row-cols-xxl-3>*{flex:0 0 auto;width:33.33333333%}.row-cols-xxl-4>*{flex:0 0 auto;width:25%}.row-cols-xxl-5>*{flex:0 0 auto;width:20%}.row-cols-xxl-6>*{flex:0 0 auto;width:16.66666667%}.col-xxl-auto{flex:0 0 auto;width:auto}.col-xxl-1{flex:0 0 auto;width:8.33333333%}.col-xxl-2{flex:0 0 auto;width:16.66666667%}.col-xxl-3{flex:0 0 auto;width:25%}.col-xxl-4{flex:0 0 auto;width:33.33333333%}.col-xxl-5{flex:0 0 auto;width:41.66666667%}.col-xxl-6{flex:0 0 auto;width:50%}.col-xxl-7{flex:0 0 auto;width:58.33333333%}.col-xxl-8{flex:0 0 auto;width:66.66666667%}.col-xxl-9{flex:0 0 auto;width:75%}.col-xxl-10{flex:0 0 auto;width:83.33333333%}.col-xxl-11{flex:0 0 auto;width:91.66666667%}.col-xxl-12{flex:0 0 auto;width:100%}.offset-xxl-0{margin-left:0}.offset-xxl-1{margin-left:8.33333333%}.offset-xxl-2{margin-left:16.66666667%}.offset-xxl-3{margin-left:25%}.offset-xxl-4{margin-left:33.33333333%}.offset-xxl-5{margin-left:41.66666667%}.offset-xxl-6{margin-left:50%}.offset-xxl-7{margin-left:58.33333333%}.offset-xxl-8{margin-left:66.66666667%}.offset-xxl-9{margin-left:75%}.offset-xxl-10{margin-left:83.33333333%}.offset-xxl-11{margin-left:91.66666667%}.g-xxl-0,.gx-xxl-0{--bs-gutter-x: 0}.g-xxl-0,.gy-xxl-0{--bs-gutter-y: 0}.g-xxl-1,.gx-xxl-1{--bs-gutter-x: .25rem}.g-xxl-1,.gy-xxl-1{--bs-gutter-y: .25rem}.g-xxl-2,.gx-xxl-2{--bs-gutter-x: .5rem}.g-xxl-2,.gy-xxl-2{--bs-gutter-y: .5rem}.g-xxl-3,.gx-xxl-3{--bs-gutter-x: 1rem}.g-xxl-3,.gy-xxl-3{--bs-gutter-y: 1rem}.g-xxl-4,.gx-xxl-4{--bs-gutter-x: 1.5rem}.g-xxl-4,.gy-xxl-4{--bs-gutter-y: 1.5rem}.g-xxl-5,.gx-xxl-5{--bs-gutter-x: 3rem}.g-xxl-5,.gy-xxl-5{--bs-gutter-y: 3rem}}.table{--bs-table-color-type: initial;--bs-table-bg-type: initial;--bs-table-color-state: initial;--bs-table-bg-state: initial;--bs-table-color: var(--bs-emphasis-color);--bs-table-bg: var(--bs-body-bg);--bs-table-border-color: var(--bs-border-color);--bs-table-accent-bg: transparent;--bs-table-striped-color: var(--bs-emphasis-color);--bs-table-striped-bg: rgba(var(--bs-emphasis-color-rgb), .05);--bs-table-active-color: var(--bs-emphasis-color);--bs-table-active-bg: rgba(var(--bs-emphasis-color-rgb), .1);--bs-table-hover-color: var(--bs-emphasis-color);--bs-table-hover-bg: rgba(var(--bs-emphasis-color-rgb), .075);width:100%;margin-bottom:1rem;vertical-align:top;border-color:var(--bs-table-border-color)}.table>:not(caption)>*>*{padding:.5rem;color:var(--bs-table-color-state, var(--bs-table-color-type, var(--bs-table-color)));background-color:var(--bs-table-bg);border-bottom-width:var(--bs-border-width);box-shadow:inset 0 0 0 9999px var(--bs-table-bg-state, var(--bs-table-bg-type, var(--bs-table-accent-bg)))}.table>tbody{vertical-align:inherit}.table>thead{vertical-align:bottom}.table-group-divider{border-top:calc(var(--bs-border-width) * 2) solid currentcolor}.caption-top{caption-side:top}.table-sm>:not(caption)>*>*{padding:.25rem}.table-bordered>:not(caption)>*{border-width:var(--bs-border-width) 0}.table-bordered>:not(caption)>*>*{border-width:0 var(--bs-border-width)}.table-borderless>:not(caption)>*>*{border-bottom-width:0}.table-borderless>:not(:first-child){border-top-width:0}.table-striped>tbody>tr:nth-of-type(odd)>*{--bs-table-color-type: var(--bs-table-striped-color);--bs-table-bg-type: var(--bs-table-striped-bg)}.table-striped-columns>:not(caption)>tr>:nth-child(2n){--bs-table-color-type: var(--bs-table-striped-color);--bs-table-bg-type: var(--bs-table-striped-bg)}.table-active{--bs-table-color-state: var(--bs-table-active-color);--bs-table-bg-state: var(--bs-table-active-bg)}.table-hover>tbody>tr:hover>*{--bs-table-color-state: var(--bs-table-hover-color);--bs-table-bg-state: var(--bs-table-hover-bg)}.table-primary{--bs-table-color: #000;--bs-table-bg: #cfe2ff;--bs-table-border-color: #a6b5cc;--bs-table-striped-bg: #c5d7f2;--bs-table-striped-color: #000;--bs-table-active-bg: #bacbe6;--bs-table-active-color: #000;--bs-table-hover-bg: #bfd1ec;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-secondary{--bs-table-color: #000;--bs-table-bg: #e2e3e5;--bs-table-border-color: #b5b6b7;--bs-table-striped-bg: #d7d8da;--bs-table-striped-color: #000;--bs-table-active-bg: #cbccce;--bs-table-active-color: #000;--bs-table-hover-bg: #d1d2d4;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-success{--bs-table-color: #000;--bs-table-bg: #d1e7dd;--bs-table-border-color: #a7b9b1;--bs-table-striped-bg: #c7dbd2;--bs-table-striped-color: #000;--bs-table-active-bg: #bcd0c7;--bs-table-active-color: #000;--bs-table-hover-bg: #c1d6cc;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-info{--bs-table-color: #000;--bs-table-bg: #cff4fc;--bs-table-border-color: #a6c3ca;--bs-table-striped-bg: #c5e8ef;--bs-table-striped-color: #000;--bs-table-active-bg: #badce3;--bs-table-active-color: #000;--bs-table-hover-bg: #bfe2e9;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-warning{--bs-table-color: #000;--bs-table-bg: #fff3cd;--bs-table-border-color: #ccc2a4;--bs-table-striped-bg: #f2e7c3;--bs-table-striped-color: #000;--bs-table-active-bg: #e6dbb9;--bs-table-active-color: #000;--bs-table-hover-bg: #ece1be;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-danger{--bs-table-color: #000;--bs-table-bg: #f8d7da;--bs-table-border-color: #c6acae;--bs-table-striped-bg: #eccccf;--bs-table-striped-color: #000;--bs-table-active-bg: #dfc2c4;--bs-table-active-color: #000;--bs-table-hover-bg: #e5c7ca;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-light{--bs-table-color: #000;--bs-table-bg: #f8f9fa;--bs-table-border-color: #c6c7c8;--bs-table-striped-bg: #ecedee;--bs-table-striped-color: #000;--bs-table-active-bg: #dfe0e1;--bs-table-active-color: #000;--bs-table-hover-bg: #e5e6e7;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-dark{--bs-table-color: #fff;--bs-table-bg: #212529;--bs-table-border-color: #4d5154;--bs-table-striped-bg: #2c3034;--bs-table-striped-color: #fff;--bs-table-active-bg: #373b3e;--bs-table-active-color: #fff;--bs-table-hover-bg: #323539;--bs-table-hover-color: #fff;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-responsive{overflow-x:auto;-webkit-overflow-scrolling:touch}@media (max-width: 575.98px){.table-responsive-sm{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 767.98px){.table-responsive-md{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 991.98px){.table-responsive-lg{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 1199.98px){.table-responsive-xl{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 1399.98px){.table-responsive-xxl{overflow-x:auto;-webkit-overflow-scrolling:touch}}.form-label{margin-bottom:.5rem}.col-form-label{padding-top:calc(.375rem + var(--bs-border-width));padding-bottom:calc(.375rem + var(--bs-border-width));margin-bottom:0;font-size:inherit;line-height:1.5}.col-form-label-lg{padding-top:calc(.5rem + var(--bs-border-width));padding-bottom:calc(.5rem + var(--bs-border-width));font-size:1.25rem}.col-form-label-sm{padding-top:calc(.25rem + var(--bs-border-width));padding-bottom:calc(.25rem + var(--bs-border-width));font-size:.875rem}.form-text{margin-top:.25rem;font-size:.875em;color:var(--bs-secondary-color)}.form-control{display:block;width:100%;padding:.375rem .75rem;font-size:1rem;font-weight:400;line-height:1.5;color:var(--bs-body-color);appearance:none;background-color:var(--bs-body-bg);background-clip:padding-box;border:var(--bs-border-width) solid var(--bs-border-color);border-radius:var(--bs-border-radius);transition:border-color .15s ease-in-out,box-shadow .15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-control{transition:none}}.form-control[type=file]{overflow:hidden}.form-control[type=file]:not(:disabled):not([readonly]){cursor:pointer}.form-control:focus{color:var(--bs-body-color);background-color:var(--bs-body-bg);border-color:#86b7fe;outline:0;box-shadow:0 0 0 .25rem #0d6efd40}.form-control::-webkit-date-and-time-value{min-width:85px;height:1.5em;margin:0}.form-control::-webkit-datetime-edit{display:block;padding:0}.form-control::placeholder{color:var(--bs-secondary-color);opacity:1}.form-control:disabled{background-color:var(--bs-secondary-bg);opacity:1}.form-control::file-selector-button{padding:.375rem .75rem;margin:-.375rem -.75rem;margin-inline-end:.75rem;color:var(--bs-body-color);background-color:var(--bs-tertiary-bg);pointer-events:none;border-color:inherit;border-style:solid;border-width:0;border-inline-end-width:var(--bs-border-width);border-radius:0;transition:color .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-control::file-selector-button{transition:none}}.form-control:hover:not(:disabled):not([readonly])::file-selector-button{background-color:var(--bs-secondary-bg)}.form-control-plaintext{display:block;width:100%;padding:.375rem 0;margin-bottom:0;line-height:1.5;color:var(--bs-body-color);background-color:transparent;border:solid transparent;border-width:var(--bs-border-width) 0}.form-control-plaintext:focus{outline:0}.form-control-plaintext.form-control-sm,.form-control-plaintext.form-control-lg{padding-right:0;padding-left:0}.form-control-sm{min-height:calc(1.5em + .5rem + calc(var(--bs-border-width) * 2));padding:.25rem .5rem;font-size:.875rem;border-radius:var(--bs-border-radius-sm)}.form-control-sm::file-selector-button{padding:.25rem .5rem;margin:-.25rem -.5rem;margin-inline-end:.5rem}.form-control-lg{min-height:calc(1.5em + 1rem + calc(var(--bs-border-width) * 2));padding:.5rem 1rem;font-size:1.25rem;border-radius:var(--bs-border-radius-lg)}.form-control-lg::file-selector-button{padding:.5rem 1rem;margin:-.5rem -1rem;margin-inline-end:1rem}textarea.form-control{min-height:calc(1.5em + .75rem + calc(var(--bs-border-width) * 2))}textarea.form-control-sm{min-height:calc(1.5em + .5rem + calc(var(--bs-border-width) * 2))}textarea.form-control-lg{min-height:calc(1.5em + 1rem + calc(var(--bs-border-width) * 2))}.form-control-color{width:3rem;height:calc(1.5em + .75rem + calc(var(--bs-border-width) * 2));padding:.375rem}.form-control-color:not(:disabled):not([readonly]){cursor:pointer}.form-control-color::-moz-color-swatch{border:0!important;border-radius:var(--bs-border-radius)}.form-control-color::-webkit-color-swatch{border:0!important;border-radius:var(--bs-border-radius)}.form-control-color.form-control-sm{height:calc(1.5em + .5rem + calc(var(--bs-border-width) * 2))}.form-control-color.form-control-lg{height:calc(1.5em + 1rem + calc(var(--bs-border-width) * 2))}.form-select{--bs-form-select-bg-img: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23343a40' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e");display:block;width:100%;padding:.375rem 2.25rem .375rem .75rem;font-size:1rem;font-weight:400;line-height:1.5;color:var(--bs-body-color);appearance:none;background-color:var(--bs-body-bg);background-image:var(--bs-form-select-bg-img),var(--bs-form-select-bg-icon, none);background-repeat:no-repeat;background-position:right .75rem center;background-size:16px 12px;border:var(--bs-border-width) solid var(--bs-border-color);border-radius:var(--bs-border-radius);transition:border-color .15s ease-in-out,box-shadow .15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-select{transition:none}}.form-select:focus{border-color:#86b7fe;outline:0;box-shadow:0 0 0 .25rem #0d6efd40}.form-select[multiple],.form-select[size]:not([size="1"]){padding-right:.75rem;background-image:none}.form-select:disabled{background-color:var(--bs-secondary-bg)}.form-select:-moz-focusring{color:transparent;text-shadow:0 0 0 var(--bs-body-color)}.form-select-sm{padding-top:.25rem;padding-bottom:.25rem;padding-left:.5rem;font-size:.875rem;border-radius:var(--bs-border-radius-sm)}.form-select-lg{padding-top:.5rem;padding-bottom:.5rem;padding-left:1rem;font-size:1.25rem;border-radius:var(--bs-border-radius-lg)}[data-bs-theme=dark] .form-select{--bs-form-select-bg-img: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23dee2e6' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e")}.form-check{display:block;min-height:1.5rem;padding-left:1.5em;margin-bottom:.125rem}.form-check .form-check-input{float:left;margin-left:-1.5em}.form-check-reverse{padding-right:1.5em;padding-left:0;text-align:right}.form-check-reverse .form-check-input{float:right;margin-right:-1.5em;margin-left:0}.form-check-input{--bs-form-check-bg: var(--bs-body-bg);flex-shrink:0;width:1em;height:1em;margin-top:.25em;vertical-align:top;appearance:none;background-color:var(--bs-form-check-bg);background-image:var(--bs-form-check-bg-image);background-repeat:no-repeat;background-position:center;background-size:contain;border:var(--bs-border-width) solid var(--bs-border-color);print-color-adjust:exact}.form-check-input[type=checkbox]{border-radius:.25em}.form-check-input[type=radio]{border-radius:50%}.form-check-input:active{filter:brightness(90%)}.form-check-input:focus{border-color:#86b7fe;outline:0;box-shadow:0 0 0 .25rem #0d6efd40}.form-check-input:checked{background-color:#0d6efd;border-color:#0d6efd}.form-check-input:checked[type=checkbox]{--bs-form-check-bg-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 20 20'%3e%3cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='m6 10 3 3 6-6'/%3e%3c/svg%3e")}.form-check-input:checked[type=radio]{--bs-form-check-bg-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='2' fill='%23fff'/%3e%3c/svg%3e")}.form-check-input[type=checkbox]:indeterminate{background-color:#0d6efd;border-color:#0d6efd;--bs-form-check-bg-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 20 20'%3e%3cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='M6 10h8'/%3e%3c/svg%3e")}.form-check-input:disabled{pointer-events:none;filter:none;opacity:.5}.form-check-input[disabled]~.form-check-label,.form-check-input:disabled~.form-check-label{cursor:default;opacity:.5}.form-switch{padding-left:2.5em}.form-switch .form-check-input{--bs-form-switch-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='rgba%280, 0, 0, 0.25%29'/%3e%3c/svg%3e");width:2em;margin-left:-2.5em;background-image:var(--bs-form-switch-bg);background-position:left center;border-radius:2em;transition:background-position .15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-switch .form-check-input{transition:none}}.form-switch .form-check-input:focus{--bs-form-switch-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='%2386b7fe'/%3e%3c/svg%3e")}.form-switch .form-check-input:checked{background-position:right center;--bs-form-switch-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='%23fff'/%3e%3c/svg%3e")}.form-switch.form-check-reverse{padding-right:2.5em;padding-left:0}.form-switch.form-check-reverse .form-check-input{margin-right:-2.5em;margin-left:0}.form-check-inline{display:inline-block;margin-right:1rem}.btn-check{position:absolute;clip:rect(0,0,0,0);pointer-events:none}.btn-check[disabled]+.btn,.btn-check:disabled+.btn{pointer-events:none;filter:none;opacity:.65}[data-bs-theme=dark] .form-switch .form-check-input:not(:checked):not(:focus){--bs-form-switch-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='rgba%28255, 255, 255, 0.25%29'/%3e%3c/svg%3e")}.form-range{width:100%;height:1.5rem;padding:0;appearance:none;background-color:transparent}.form-range:focus{outline:0}.form-range:focus::-webkit-slider-thumb{box-shadow:0 0 0 1px #fff,0 0 0 .25rem #0d6efd40}.form-range:focus::-moz-range-thumb{box-shadow:0 0 0 1px #fff,0 0 0 .25rem #0d6efd40}.form-range::-moz-focus-outer{border:0}.form-range::-webkit-slider-thumb{width:1rem;height:1rem;margin-top:-.25rem;appearance:none;background-color:#0d6efd;border:0;border-radius:1rem;transition:background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-range::-webkit-slider-thumb{transition:none}}.form-range::-webkit-slider-thumb:active{background-color:#b6d4fe}.form-range::-webkit-slider-runnable-track{width:100%;height:.5rem;color:transparent;cursor:pointer;background-color:var(--bs-secondary-bg);border-color:transparent;border-radius:1rem}.form-range::-moz-range-thumb{width:1rem;height:1rem;appearance:none;background-color:#0d6efd;border:0;border-radius:1rem;transition:background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-range::-moz-range-thumb{transition:none}}.form-range::-moz-range-thumb:active{background-color:#b6d4fe}.form-range::-moz-range-track{width:100%;height:.5rem;color:transparent;cursor:pointer;background-color:var(--bs-secondary-bg);border-color:transparent;border-radius:1rem}.form-range:disabled{pointer-events:none}.form-range:disabled::-webkit-slider-thumb{background-color:var(--bs-secondary-color)}.form-range:disabled::-moz-range-thumb{background-color:var(--bs-secondary-color)}.form-floating{position:relative}.form-floating>.form-control,.form-floating>.form-control-plaintext,.form-floating>.form-select{height:calc(3.5rem + calc(var(--bs-border-width) * 2));min-height:calc(3.5rem + calc(var(--bs-border-width) * 2));line-height:1.25}.form-floating>label{position:absolute;top:0;left:0;z-index:2;height:100%;padding:1rem .75rem;overflow:hidden;text-align:start;text-overflow:ellipsis;white-space:nowrap;pointer-events:none;border:var(--bs-border-width) solid transparent;transform-origin:0 0;transition:opacity .1s ease-in-out,transform .1s ease-in-out}@media (prefers-reduced-motion: reduce){.form-floating>label{transition:none}}.form-floating>.form-control,.form-floating>.form-control-plaintext{padding:1rem .75rem}.form-floating>.form-control::placeholder,.form-floating>.form-control-plaintext::placeholder{color:transparent}.form-floating>.form-control:focus,.form-floating>.form-control:not(:placeholder-shown),.form-floating>.form-control-plaintext:focus,.form-floating>.form-control-plaintext:not(:placeholder-shown){padding-top:1.625rem;padding-bottom:.625rem}.form-floating>.form-control:-webkit-autofill,.form-floating>.form-control-plaintext:-webkit-autofill{padding-top:1.625rem;padding-bottom:.625rem}.form-floating>.form-select{padding-top:1.625rem;padding-bottom:.625rem}.form-floating>.form-control:focus~label,.form-floating>.form-control:not(:placeholder-shown)~label,.form-floating>.form-control-plaintext~label,.form-floating>.form-select~label{color:rgba(var(--bs-body-color-rgb),.65);transform:scale(.85) translateY(-.5rem) translate(.15rem)}.form-floating>.form-control:focus~label:after,.form-floating>.form-control:not(:placeholder-shown)~label:after,.form-floating>.form-control-plaintext~label:after,.form-floating>.form-select~label:after{position:absolute;inset:1rem .375rem;z-index:-1;height:1.5em;content:"";background-color:var(--bs-body-bg);border-radius:var(--bs-border-radius)}.form-floating>.form-control:-webkit-autofill~label{color:rgba(var(--bs-body-color-rgb),.65);transform:scale(.85) translateY(-.5rem) translate(.15rem)}.form-floating>.form-control-plaintext~label{border-width:var(--bs-border-width) 0}.form-floating>:disabled~label,.form-floating>.form-control:disabled~label{color:#6c757d}.form-floating>:disabled~label:after,.form-floating>.form-control:disabled~label:after{background-color:var(--bs-secondary-bg)}.input-group{position:relative;display:flex;flex-wrap:wrap;align-items:stretch;width:100%}.input-group>.form-control,.input-group>.form-select,.input-group>.form-floating{position:relative;flex:1 1 auto;width:1%;min-width:0}.input-group>.form-control:focus,.input-group>.form-select:focus,.input-group>.form-floating:focus-within{z-index:5}.input-group .btn{position:relative;z-index:2}.input-group .btn:focus{z-index:5}.input-group-text{display:flex;align-items:center;padding:.375rem .75rem;font-size:1rem;font-weight:400;line-height:1.5;color:var(--bs-body-color);text-align:center;white-space:nowrap;background-color:var(--bs-tertiary-bg);border:var(--bs-border-width) solid var(--bs-border-color);border-radius:var(--bs-border-radius)}.input-group-lg>.form-control,.input-group-lg>.form-select,.input-group-lg>.input-group-text,.input-group-lg>.btn{padding:.5rem 1rem;font-size:1.25rem;border-radius:var(--bs-border-radius-lg)}.input-group-sm>.form-control,.input-group-sm>.form-select,.input-group-sm>.input-group-text,.input-group-sm>.btn{padding:.25rem .5rem;font-size:.875rem;border-radius:var(--bs-border-radius-sm)}.input-group-lg>.form-select,.input-group-sm>.form-select{padding-right:3rem}.input-group:not(.has-validation)>:not(:last-child):not(.dropdown-toggle):not(.dropdown-menu):not(.form-floating),.input-group:not(.has-validation)>.dropdown-toggle:nth-last-child(n+3),.input-group:not(.has-validation)>.form-floating:not(:last-child)>.form-control,.input-group:not(.has-validation)>.form-floating:not(:last-child)>.form-select{border-top-right-radius:0;border-bottom-right-radius:0}.input-group.has-validation>:nth-last-child(n+3):not(.dropdown-toggle):not(.dropdown-menu):not(.form-floating),.input-group.has-validation>.dropdown-toggle:nth-last-child(n+4),.input-group.has-validation>.form-floating:nth-last-child(n+3)>.form-control,.input-group.has-validation>.form-floating:nth-last-child(n+3)>.form-select{border-top-right-radius:0;border-bottom-right-radius:0}.input-group>:not(:first-child):not(.dropdown-menu):not(.valid-tooltip):not(.valid-feedback):not(.invalid-tooltip):not(.invalid-feedback){margin-left:calc(var(--bs-border-width) * -1);border-top-left-radius:0;border-bottom-left-radius:0}.input-group>.form-floating:not(:first-child)>.form-control,.input-group>.form-floating:not(:first-child)>.form-select{border-top-left-radius:0;border-bottom-left-radius:0}.valid-feedback{display:none;width:100%;margin-top:.25rem;font-size:.875em;color:var(--bs-form-valid-color)}.valid-tooltip{position:absolute;top:100%;z-index:5;display:none;max-width:100%;padding:.25rem .5rem;margin-top:.1rem;font-size:.875rem;color:#fff;background-color:var(--bs-success);border-radius:var(--bs-border-radius)}.was-validated :valid~.valid-feedback,.was-validated :valid~.valid-tooltip,.is-valid~.valid-feedback,.is-valid~.valid-tooltip{display:block}.was-validated .form-control:valid,.form-control.is-valid{border-color:var(--bs-form-valid-border-color);padding-right:calc(1.5em + .75rem);background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8 8'%3e%3cpath fill='%23198754' d='M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z'/%3e%3c/svg%3e");background-repeat:no-repeat;background-position:right calc(.375em + .1875rem) center;background-size:calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-control:valid:focus,.form-control.is-valid:focus{border-color:var(--bs-form-valid-border-color);box-shadow:0 0 0 .25rem rgba(var(--bs-success-rgb),.25)}.was-validated textarea.form-control:valid,textarea.form-control.is-valid{padding-right:calc(1.5em + .75rem);background-position:top calc(.375em + .1875rem) right calc(.375em + .1875rem)}.was-validated .form-select:valid,.form-select.is-valid{border-color:var(--bs-form-valid-border-color)}.was-validated .form-select:valid:not([multiple]):not([size]),.was-validated .form-select:valid:not([multiple])[size="1"],.form-select.is-valid:not([multiple]):not([size]),.form-select.is-valid:not([multiple])[size="1"]{--bs-form-select-bg-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8 8'%3e%3cpath fill='%23198754' d='M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z'/%3e%3c/svg%3e");padding-right:4.125rem;background-position:right .75rem center,center right 2.25rem;background-size:16px 12px,calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-select:valid:focus,.form-select.is-valid:focus{border-color:var(--bs-form-valid-border-color);box-shadow:0 0 0 .25rem rgba(var(--bs-success-rgb),.25)}.was-validated .form-control-color:valid,.form-control-color.is-valid{width:calc(3.75rem + 1.5em)}.was-validated .form-check-input:valid,.form-check-input.is-valid{border-color:var(--bs-form-valid-border-color)}.was-validated .form-check-input:valid:checked,.form-check-input.is-valid:checked{background-color:var(--bs-form-valid-color)}.was-validated .form-check-input:valid:focus,.form-check-input.is-valid:focus{box-shadow:0 0 0 .25rem rgba(var(--bs-success-rgb),.25)}.was-validated .form-check-input:valid~.form-check-label,.form-check-input.is-valid~.form-check-label{color:var(--bs-form-valid-color)}.form-check-inline .form-check-input~.valid-feedback{margin-left:.5em}.was-validated .input-group>.form-control:not(:focus):valid,.input-group>.form-control:not(:focus).is-valid,.was-validated .input-group>.form-select:not(:focus):valid,.input-group>.form-select:not(:focus).is-valid,.was-validated .input-group>.form-floating:not(:focus-within):valid,.input-group>.form-floating:not(:focus-within).is-valid{z-index:3}.invalid-feedback{display:none;width:100%;margin-top:.25rem;font-size:.875em;color:var(--bs-form-invalid-color)}.invalid-tooltip{position:absolute;top:100%;z-index:5;display:none;max-width:100%;padding:.25rem .5rem;margin-top:.1rem;font-size:.875rem;color:#fff;background-color:var(--bs-danger);border-radius:var(--bs-border-radius)}.was-validated :invalid~.invalid-feedback,.was-validated :invalid~.invalid-tooltip,.is-invalid~.invalid-feedback,.is-invalid~.invalid-tooltip{display:block}.was-validated .form-control:invalid,.form-control.is-invalid{border-color:var(--bs-form-invalid-border-color);padding-right:calc(1.5em + .75rem);background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12' width='12' height='12' fill='none' stroke='%23dc3545'%3e%3ccircle cx='6' cy='6' r='4.5'/%3e%3cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3e%3ccircle cx='6' cy='8.2' r='.6' fill='%23dc3545' stroke='none'/%3e%3c/svg%3e");background-repeat:no-repeat;background-position:right calc(.375em + .1875rem) center;background-size:calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-control:invalid:focus,.form-control.is-invalid:focus{border-color:var(--bs-form-invalid-border-color);box-shadow:0 0 0 .25rem rgba(var(--bs-danger-rgb),.25)}.was-validated textarea.form-control:invalid,textarea.form-control.is-invalid{padding-right:calc(1.5em + .75rem);background-position:top calc(.375em + .1875rem) right calc(.375em + .1875rem)}.was-validated .form-select:invalid,.form-select.is-invalid{border-color:var(--bs-form-invalid-border-color)}.was-validated .form-select:invalid:not([multiple]):not([size]),.was-validated .form-select:invalid:not([multiple])[size="1"],.form-select.is-invalid:not([multiple]):not([size]),.form-select.is-invalid:not([multiple])[size="1"]{--bs-form-select-bg-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12' width='12' height='12' fill='none' stroke='%23dc3545'%3e%3ccircle cx='6' cy='6' r='4.5'/%3e%3cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3e%3ccircle cx='6' cy='8.2' r='.6' fill='%23dc3545' stroke='none'/%3e%3c/svg%3e");padding-right:4.125rem;background-position:right .75rem center,center right 2.25rem;background-size:16px 12px,calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-select:invalid:focus,.form-select.is-invalid:focus{border-color:var(--bs-form-invalid-border-color);box-shadow:0 0 0 .25rem rgba(var(--bs-danger-rgb),.25)}.was-validated .form-control-color:invalid,.form-control-color.is-invalid{width:calc(3.75rem + 1.5em)}.was-validated .form-check-input:invalid,.form-check-input.is-invalid{border-color:var(--bs-form-invalid-border-color)}.was-validated .form-check-input:invalid:checked,.form-check-input.is-invalid:checked{background-color:var(--bs-form-invalid-color)}.was-validated .form-check-input:invalid:focus,.form-check-input.is-invalid:focus{box-shadow:0 0 0 .25rem rgba(var(--bs-danger-rgb),.25)}.was-validated .form-check-input:invalid~.form-check-label,.form-check-input.is-invalid~.form-check-label{color:var(--bs-form-invalid-color)}.form-check-inline .form-check-input~.invalid-feedback{margin-left:.5em}.was-validated .input-group>.form-control:not(:focus):invalid,.input-group>.form-control:not(:focus).is-invalid,.was-validated .input-group>.form-select:not(:focus):invalid,.input-group>.form-select:not(:focus).is-invalid,.was-validated .input-group>.form-floating:not(:focus-within):invalid,.input-group>.form-floating:not(:focus-within).is-invalid{z-index:4}.btn{--bs-btn-padding-x: .75rem;--bs-btn-padding-y: .375rem;--bs-btn-font-family: ;--bs-btn-font-size: 1rem;--bs-btn-font-weight: 400;--bs-btn-line-height: 1.5;--bs-btn-color: var(--bs-body-color);--bs-btn-bg: transparent;--bs-btn-border-width: var(--bs-border-width);--bs-btn-border-color: transparent;--bs-btn-border-radius: var(--bs-border-radius);--bs-btn-hover-border-color: transparent;--bs-btn-box-shadow: inset 0 1px 0 rgba(255, 255, 255, .15), 0 1px 1px rgba(0, 0, 0, .075);--bs-btn-disabled-opacity: .65;--bs-btn-focus-box-shadow: 0 0 0 .25rem rgba(var(--bs-btn-focus-shadow-rgb), .5);display:inline-block;padding:var(--bs-btn-padding-y) var(--bs-btn-padding-x);font-family:var(--bs-btn-font-family);font-size:var(--bs-btn-font-size);font-weight:var(--bs-btn-font-weight);line-height:var(--bs-btn-line-height);color:var(--bs-btn-color);text-align:center;text-decoration:none;vertical-align:middle;cursor:pointer;user-select:none;border:var(--bs-btn-border-width) solid var(--bs-btn-border-color);border-radius:var(--bs-btn-border-radius);background-color:var(--bs-btn-bg);transition:color .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out}@media (prefers-reduced-motion: reduce){.btn{transition:none}}.btn:hover{color:var(--bs-btn-hover-color);background-color:var(--bs-btn-hover-bg);border-color:var(--bs-btn-hover-border-color)}.btn-check+.btn:hover{color:var(--bs-btn-color);background-color:var(--bs-btn-bg);border-color:var(--bs-btn-border-color)}.btn:focus-visible{color:var(--bs-btn-hover-color);background-color:var(--bs-btn-hover-bg);border-color:var(--bs-btn-hover-border-color);outline:0;box-shadow:var(--bs-btn-focus-box-shadow)}.btn-check:focus-visible+.btn{border-color:var(--bs-btn-hover-border-color);outline:0;box-shadow:var(--bs-btn-focus-box-shadow)}.btn-check:checked+.btn,:not(.btn-check)+.btn:active,.btn:first-child:active,.btn.active,.btn.show{color:var(--bs-btn-active-color);background-color:var(--bs-btn-active-bg);border-color:var(--bs-btn-active-border-color)}.btn-check:checked+.btn:focus-visible,:not(.btn-check)+.btn:active:focus-visible,.btn:first-child:active:focus-visible,.btn.active:focus-visible,.btn.show:focus-visible{box-shadow:var(--bs-btn-focus-box-shadow)}.btn:disabled,.btn.disabled,fieldset:disabled .btn{color:var(--bs-btn-disabled-color);pointer-events:none;background-color:var(--bs-btn-disabled-bg);border-color:var(--bs-btn-disabled-border-color);opacity:var(--bs-btn-disabled-opacity)}.btn-primary{--bs-btn-color: #fff;--bs-btn-bg: #0d6efd;--bs-btn-border-color: #0d6efd;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #0b5ed7;--bs-btn-hover-border-color: #0a58ca;--bs-btn-focus-shadow-rgb: 49, 132, 253;--bs-btn-active-color: #fff;--bs-btn-active-bg: #0a58ca;--bs-btn-active-border-color: #0a53be;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #0d6efd;--bs-btn-disabled-border-color: #0d6efd}.btn-secondary{--bs-btn-color: #fff;--bs-btn-bg: #6c757d;--bs-btn-border-color: #6c757d;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #5c636a;--bs-btn-hover-border-color: #565e64;--bs-btn-focus-shadow-rgb: 130, 138, 145;--bs-btn-active-color: #fff;--bs-btn-active-bg: #565e64;--bs-btn-active-border-color: #51585e;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #6c757d;--bs-btn-disabled-border-color: #6c757d}.btn-success{--bs-btn-color: #fff;--bs-btn-bg: #198754;--bs-btn-border-color: #198754;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #157347;--bs-btn-hover-border-color: #146c43;--bs-btn-focus-shadow-rgb: 60, 153, 110;--bs-btn-active-color: #fff;--bs-btn-active-bg: #146c43;--bs-btn-active-border-color: #13653f;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #198754;--bs-btn-disabled-border-color: #198754}.btn-info{--bs-btn-color: #000;--bs-btn-bg: #0dcaf0;--bs-btn-border-color: #0dcaf0;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #31d2f2;--bs-btn-hover-border-color: #25cff2;--bs-btn-focus-shadow-rgb: 11, 172, 204;--bs-btn-active-color: #000;--bs-btn-active-bg: #3dd5f3;--bs-btn-active-border-color: #25cff2;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #000;--bs-btn-disabled-bg: #0dcaf0;--bs-btn-disabled-border-color: #0dcaf0}.btn-warning{--bs-btn-color: #000;--bs-btn-bg: #ffc107;--bs-btn-border-color: #ffc107;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #ffca2c;--bs-btn-hover-border-color: #ffc720;--bs-btn-focus-shadow-rgb: 217, 164, 6;--bs-btn-active-color: #000;--bs-btn-active-bg: #ffcd39;--bs-btn-active-border-color: #ffc720;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #000;--bs-btn-disabled-bg: #ffc107;--bs-btn-disabled-border-color: #ffc107}.btn-danger{--bs-btn-color: #fff;--bs-btn-bg: #dc3545;--bs-btn-border-color: #dc3545;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #bb2d3b;--bs-btn-hover-border-color: #b02a37;--bs-btn-focus-shadow-rgb: 225, 83, 97;--bs-btn-active-color: #fff;--bs-btn-active-bg: #b02a37;--bs-btn-active-border-color: #a52834;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #dc3545;--bs-btn-disabled-border-color: #dc3545}.btn-light{--bs-btn-color: #000;--bs-btn-bg: #f8f9fa;--bs-btn-border-color: #f8f9fa;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #d3d4d5;--bs-btn-hover-border-color: #c6c7c8;--bs-btn-focus-shadow-rgb: 211, 212, 213;--bs-btn-active-color: #000;--bs-btn-active-bg: #c6c7c8;--bs-btn-active-border-color: #babbbc;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #000;--bs-btn-disabled-bg: #f8f9fa;--bs-btn-disabled-border-color: #f8f9fa}.btn-dark{--bs-btn-color: #fff;--bs-btn-bg: #212529;--bs-btn-border-color: #212529;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #424649;--bs-btn-hover-border-color: #373b3e;--bs-btn-focus-shadow-rgb: 66, 70, 73;--bs-btn-active-color: #fff;--bs-btn-active-bg: #4d5154;--bs-btn-active-border-color: #373b3e;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #212529;--bs-btn-disabled-border-color: #212529}.btn-outline-primary{--bs-btn-color: #0d6efd;--bs-btn-border-color: #0d6efd;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #0d6efd;--bs-btn-hover-border-color: #0d6efd;--bs-btn-focus-shadow-rgb: 13, 110, 253;--bs-btn-active-color: #fff;--bs-btn-active-bg: #0d6efd;--bs-btn-active-border-color: #0d6efd;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #0d6efd;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #0d6efd;--bs-gradient: none}.btn-outline-secondary{--bs-btn-color: #6c757d;--bs-btn-border-color: #6c757d;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #6c757d;--bs-btn-hover-border-color: #6c757d;--bs-btn-focus-shadow-rgb: 108, 117, 125;--bs-btn-active-color: #fff;--bs-btn-active-bg: #6c757d;--bs-btn-active-border-color: #6c757d;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #6c757d;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #6c757d;--bs-gradient: none}.btn-outline-success{--bs-btn-color: #198754;--bs-btn-border-color: #198754;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #198754;--bs-btn-hover-border-color: #198754;--bs-btn-focus-shadow-rgb: 25, 135, 84;--bs-btn-active-color: #fff;--bs-btn-active-bg: #198754;--bs-btn-active-border-color: #198754;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #198754;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #198754;--bs-gradient: none}.btn-outline-info{--bs-btn-color: #0dcaf0;--bs-btn-border-color: #0dcaf0;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #0dcaf0;--bs-btn-hover-border-color: #0dcaf0;--bs-btn-focus-shadow-rgb: 13, 202, 240;--bs-btn-active-color: #000;--bs-btn-active-bg: #0dcaf0;--bs-btn-active-border-color: #0dcaf0;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #0dcaf0;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #0dcaf0;--bs-gradient: none}.btn-outline-warning{--bs-btn-color: #ffc107;--bs-btn-border-color: #ffc107;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #ffc107;--bs-btn-hover-border-color: #ffc107;--bs-btn-focus-shadow-rgb: 255, 193, 7;--bs-btn-active-color: #000;--bs-btn-active-bg: #ffc107;--bs-btn-active-border-color: #ffc107;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #ffc107;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #ffc107;--bs-gradient: none}.btn-outline-danger{--bs-btn-color: #dc3545;--bs-btn-border-color: #dc3545;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #dc3545;--bs-btn-hover-border-color: #dc3545;--bs-btn-focus-shadow-rgb: 220, 53, 69;--bs-btn-active-color: #fff;--bs-btn-active-bg: #dc3545;--bs-btn-active-border-color: #dc3545;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #dc3545;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #dc3545;--bs-gradient: none}.btn-outline-light{--bs-btn-color: #f8f9fa;--bs-btn-border-color: #f8f9fa;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #f8f9fa;--bs-btn-hover-border-color: #f8f9fa;--bs-btn-focus-shadow-rgb: 248, 249, 250;--bs-btn-active-color: #000;--bs-btn-active-bg: #f8f9fa;--bs-btn-active-border-color: #f8f9fa;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #f8f9fa;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #f8f9fa;--bs-gradient: none}.btn-outline-dark{--bs-btn-color: #212529;--bs-btn-border-color: #212529;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #212529;--bs-btn-hover-border-color: #212529;--bs-btn-focus-shadow-rgb: 33, 37, 41;--bs-btn-active-color: #fff;--bs-btn-active-bg: #212529;--bs-btn-active-border-color: #212529;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #212529;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #212529;--bs-gradient: none}.btn-link{--bs-btn-font-weight: 400;--bs-btn-color: var(--bs-link-color);--bs-btn-bg: transparent;--bs-btn-border-color: transparent;--bs-btn-hover-color: var(--bs-link-hover-color);--bs-btn-hover-border-color: transparent;--bs-btn-active-color: var(--bs-link-hover-color);--bs-btn-active-border-color: transparent;--bs-btn-disabled-color: #6c757d;--bs-btn-disabled-border-color: transparent;--bs-btn-box-shadow: 0 0 0 #000;--bs-btn-focus-shadow-rgb: 49, 132, 253;text-decoration:underline}.btn-link:focus-visible{color:var(--bs-btn-color)}.btn-link:hover{color:var(--bs-btn-hover-color)}.btn-lg,.btn-group-lg>.btn{--bs-btn-padding-y: .5rem;--bs-btn-padding-x: 1rem;--bs-btn-font-size: 1.25rem;--bs-btn-border-radius: var(--bs-border-radius-lg)}.btn-sm,.btn-group-sm>.btn{--bs-btn-padding-y: .25rem;--bs-btn-padding-x: .5rem;--bs-btn-font-size: .875rem;--bs-btn-border-radius: var(--bs-border-radius-sm)}.fade{transition:opacity .15s linear}@media (prefers-reduced-motion: reduce){.fade{transition:none}}.fade:not(.show){opacity:0}.collapse:not(.show){display:none}.collapsing{height:0;overflow:hidden;transition:height .35s ease}@media (prefers-reduced-motion: reduce){.collapsing{transition:none}}.collapsing.collapse-horizontal{width:0;height:auto;transition:width .35s ease}@media (prefers-reduced-motion: reduce){.collapsing.collapse-horizontal{transition:none}}.dropup,.dropend,.dropdown,.dropstart,.dropup-center,.dropdown-center{position:relative}.dropdown-toggle{white-space:nowrap}.dropdown-toggle:after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:"";border-top:.3em solid;border-right:.3em solid transparent;border-bottom:0;border-left:.3em solid transparent}.dropdown-toggle:empty:after{margin-left:0}.dropdown-menu{--bs-dropdown-zindex: 1000;--bs-dropdown-min-width: 10rem;--bs-dropdown-padding-x: 0;--bs-dropdown-padding-y: .5rem;--bs-dropdown-spacer: .125rem;--bs-dropdown-font-size: 1rem;--bs-dropdown-color: var(--bs-body-color);--bs-dropdown-bg: var(--bs-body-bg);--bs-dropdown-border-color: var(--bs-border-color-translucent);--bs-dropdown-border-radius: var(--bs-border-radius);--bs-dropdown-border-width: var(--bs-border-width);--bs-dropdown-inner-border-radius: calc(var(--bs-border-radius) - var(--bs-border-width));--bs-dropdown-divider-bg: var(--bs-border-color-translucent);--bs-dropdown-divider-margin-y: .5rem;--bs-dropdown-box-shadow: var(--bs-box-shadow);--bs-dropdown-link-color: var(--bs-body-color);--bs-dropdown-link-hover-color: var(--bs-body-color);--bs-dropdown-link-hover-bg: var(--bs-tertiary-bg);--bs-dropdown-link-active-color: #fff;--bs-dropdown-link-active-bg: #0d6efd;--bs-dropdown-link-disabled-color: var(--bs-tertiary-color);--bs-dropdown-item-padding-x: 1rem;--bs-dropdown-item-padding-y: .25rem;--bs-dropdown-header-color: #6c757d;--bs-dropdown-header-padding-x: 1rem;--bs-dropdown-header-padding-y: .5rem;position:absolute;z-index:var(--bs-dropdown-zindex);display:none;min-width:var(--bs-dropdown-min-width);padding:var(--bs-dropdown-padding-y) var(--bs-dropdown-padding-x);margin:0;font-size:var(--bs-dropdown-font-size);color:var(--bs-dropdown-color);text-align:left;list-style:none;background-color:var(--bs-dropdown-bg);background-clip:padding-box;border:var(--bs-dropdown-border-width) solid var(--bs-dropdown-border-color);border-radius:var(--bs-dropdown-border-radius)}.dropdown-menu[data-bs-popper]{top:100%;left:0;margin-top:var(--bs-dropdown-spacer)}.dropdown-menu-start{--bs-position: start}.dropdown-menu-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-end{--bs-position: end}.dropdown-menu-end[data-bs-popper]{right:0;left:auto}@media (min-width: 576px){.dropdown-menu-sm-start{--bs-position: start}.dropdown-menu-sm-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-sm-end{--bs-position: end}.dropdown-menu-sm-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 768px){.dropdown-menu-md-start{--bs-position: start}.dropdown-menu-md-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-md-end{--bs-position: end}.dropdown-menu-md-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 992px){.dropdown-menu-lg-start{--bs-position: start}.dropdown-menu-lg-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-lg-end{--bs-position: end}.dropdown-menu-lg-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 1200px){.dropdown-menu-xl-start{--bs-position: start}.dropdown-menu-xl-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-xl-end{--bs-position: end}.dropdown-menu-xl-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 1400px){.dropdown-menu-xxl-start{--bs-position: start}.dropdown-menu-xxl-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-xxl-end{--bs-position: end}.dropdown-menu-xxl-end[data-bs-popper]{right:0;left:auto}}.dropup .dropdown-menu[data-bs-popper]{top:auto;bottom:100%;margin-top:0;margin-bottom:var(--bs-dropdown-spacer)}.dropup .dropdown-toggle:after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:"";border-top:0;border-right:.3em solid transparent;border-bottom:.3em solid;border-left:.3em solid transparent}.dropup .dropdown-toggle:empty:after{margin-left:0}.dropend .dropdown-menu[data-bs-popper]{top:0;right:auto;left:100%;margin-top:0;margin-left:var(--bs-dropdown-spacer)}.dropend .dropdown-toggle:after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:"";border-top:.3em solid transparent;border-right:0;border-bottom:.3em solid transparent;border-left:.3em solid}.dropend .dropdown-toggle:empty:after{margin-left:0}.dropend .dropdown-toggle:after{vertical-align:0}.dropstart .dropdown-menu[data-bs-popper]{top:0;right:100%;left:auto;margin-top:0;margin-right:var(--bs-dropdown-spacer)}.dropstart .dropdown-toggle:after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:""}.dropstart .dropdown-toggle:after{display:none}.dropstart .dropdown-toggle:before{display:inline-block;margin-right:.255em;vertical-align:.255em;content:"";border-top:.3em solid transparent;border-right:.3em solid;border-bottom:.3em solid transparent}.dropstart .dropdown-toggle:empty:after{margin-left:0}.dropstart .dropdown-toggle:before{vertical-align:0}.dropdown-divider{height:0;margin:var(--bs-dropdown-divider-margin-y) 0;overflow:hidden;border-top:1px solid var(--bs-dropdown-divider-bg);opacity:1}.dropdown-item{display:block;width:100%;padding:var(--bs-dropdown-item-padding-y) var(--bs-dropdown-item-padding-x);clear:both;font-weight:400;color:var(--bs-dropdown-link-color);text-align:inherit;text-decoration:none;white-space:nowrap;background-color:transparent;border:0;border-radius:var(--bs-dropdown-item-border-radius, 0)}.dropdown-item:hover,.dropdown-item:focus{color:var(--bs-dropdown-link-hover-color);background-color:var(--bs-dropdown-link-hover-bg)}.dropdown-item.active,.dropdown-item:active{color:var(--bs-dropdown-link-active-color);text-decoration:none;background-color:var(--bs-dropdown-link-active-bg)}.dropdown-item.disabled,.dropdown-item:disabled{color:var(--bs-dropdown-link-disabled-color);pointer-events:none;background-color:transparent}.dropdown-menu.show{display:block}.dropdown-header{display:block;padding:var(--bs-dropdown-header-padding-y) var(--bs-dropdown-header-padding-x);margin-bottom:0;font-size:.875rem;color:var(--bs-dropdown-header-color);white-space:nowrap}.dropdown-item-text{display:block;padding:var(--bs-dropdown-item-padding-y) var(--bs-dropdown-item-padding-x);color:var(--bs-dropdown-link-color)}.dropdown-menu-dark{--bs-dropdown-color: #dee2e6;--bs-dropdown-bg: #343a40;--bs-dropdown-border-color: var(--bs-border-color-translucent);--bs-dropdown-box-shadow: ;--bs-dropdown-link-color: #dee2e6;--bs-dropdown-link-hover-color: #fff;--bs-dropdown-divider-bg: var(--bs-border-color-translucent);--bs-dropdown-link-hover-bg: rgba(255, 255, 255, .15);--bs-dropdown-link-active-color: #fff;--bs-dropdown-link-active-bg: #0d6efd;--bs-dropdown-link-disabled-color: #adb5bd;--bs-dropdown-header-color: #adb5bd}.btn-group,.btn-group-vertical{position:relative;display:inline-flex;vertical-align:middle}.btn-group>.btn,.btn-group-vertical>.btn{position:relative;flex:1 1 auto}.btn-group>.btn-check:checked+.btn,.btn-group>.btn-check:focus+.btn,.btn-group>.btn:hover,.btn-group>.btn:focus,.btn-group>.btn:active,.btn-group>.btn.active,.btn-group-vertical>.btn-check:checked+.btn,.btn-group-vertical>.btn-check:focus+.btn,.btn-group-vertical>.btn:hover,.btn-group-vertical>.btn:focus,.btn-group-vertical>.btn:active,.btn-group-vertical>.btn.active{z-index:1}.btn-toolbar{display:flex;flex-wrap:wrap;justify-content:flex-start}.btn-toolbar .input-group{width:auto}.btn-group{border-radius:var(--bs-border-radius)}.btn-group>:not(.btn-check:first-child)+.btn,.btn-group>.btn-group:not(:first-child){margin-left:calc(var(--bs-border-width) * -1)}.btn-group>.btn:not(:last-child):not(.dropdown-toggle),.btn-group>.btn.dropdown-toggle-split:first-child,.btn-group>.btn-group:not(:last-child)>.btn{border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn:nth-child(n+3),.btn-group>:not(.btn-check)+.btn,.btn-group>.btn-group:not(:first-child)>.btn{border-top-left-radius:0;border-bottom-left-radius:0}.dropdown-toggle-split{padding-right:.5625rem;padding-left:.5625rem}.dropdown-toggle-split:after,.dropup .dropdown-toggle-split:after,.dropend .dropdown-toggle-split:after{margin-left:0}.dropstart .dropdown-toggle-split:before{margin-right:0}.btn-sm+.dropdown-toggle-split,.btn-group-sm>.btn+.dropdown-toggle-split{padding-right:.375rem;padding-left:.375rem}.btn-lg+.dropdown-toggle-split,.btn-group-lg>.btn+.dropdown-toggle-split{padding-right:.75rem;padding-left:.75rem}.btn-group-vertical{flex-direction:column;align-items:flex-start;justify-content:center}.btn-group-vertical>.btn,.btn-group-vertical>.btn-group{width:100%}.btn-group-vertical>.btn:not(:first-child),.btn-group-vertical>.btn-group:not(:first-child){margin-top:calc(var(--bs-border-width) * -1)}.btn-group-vertical>.btn:not(:last-child):not(.dropdown-toggle),.btn-group-vertical>.btn-group:not(:last-child)>.btn{border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn~.btn,.btn-group-vertical>.btn-group:not(:first-child)>.btn{border-top-left-radius:0;border-top-right-radius:0}.nav{--bs-nav-link-padding-x: 1rem;--bs-nav-link-padding-y: .5rem;--bs-nav-link-font-weight: ;--bs-nav-link-color: var(--bs-link-color);--bs-nav-link-hover-color: var(--bs-link-hover-color);--bs-nav-link-disabled-color: var(--bs-secondary-color);display:flex;flex-wrap:wrap;padding-left:0;margin-bottom:0;list-style:none}.nav-link{display:block;padding:var(--bs-nav-link-padding-y) var(--bs-nav-link-padding-x);font-size:var(--bs-nav-link-font-size);font-weight:var(--bs-nav-link-font-weight);color:var(--bs-nav-link-color);text-decoration:none;background:none;border:0;transition:color .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out}@media (prefers-reduced-motion: reduce){.nav-link{transition:none}}.nav-link:hover,.nav-link:focus{color:var(--bs-nav-link-hover-color)}.nav-link:focus-visible{outline:0;box-shadow:0 0 0 .25rem #0d6efd40}.nav-link.disabled,.nav-link:disabled{color:var(--bs-nav-link-disabled-color);pointer-events:none;cursor:default}.nav-tabs{--bs-nav-tabs-border-width: var(--bs-border-width);--bs-nav-tabs-border-color: var(--bs-border-color);--bs-nav-tabs-border-radius: var(--bs-border-radius);--bs-nav-tabs-link-hover-border-color: var(--bs-secondary-bg) var(--bs-secondary-bg) var(--bs-border-color);--bs-nav-tabs-link-active-color: var(--bs-emphasis-color);--bs-nav-tabs-link-active-bg: var(--bs-body-bg);--bs-nav-tabs-link-active-border-color: var(--bs-border-color) var(--bs-border-color) var(--bs-body-bg);border-bottom:var(--bs-nav-tabs-border-width) solid var(--bs-nav-tabs-border-color)}.nav-tabs .nav-link{margin-bottom:calc(-1 * var(--bs-nav-tabs-border-width));border:var(--bs-nav-tabs-border-width) solid transparent;border-top-left-radius:var(--bs-nav-tabs-border-radius);border-top-right-radius:var(--bs-nav-tabs-border-radius)}.nav-tabs .nav-link:hover,.nav-tabs .nav-link:focus{isolation:isolate;border-color:var(--bs-nav-tabs-link-hover-border-color)}.nav-tabs .nav-link.active,.nav-tabs .nav-item.show .nav-link{color:var(--bs-nav-tabs-link-active-color);background-color:var(--bs-nav-tabs-link-active-bg);border-color:var(--bs-nav-tabs-link-active-border-color)}.nav-tabs .dropdown-menu{margin-top:calc(-1 * var(--bs-nav-tabs-border-width));border-top-left-radius:0;border-top-right-radius:0}.nav-pills{--bs-nav-pills-border-radius: var(--bs-border-radius);--bs-nav-pills-link-active-color: #fff;--bs-nav-pills-link-active-bg: #0d6efd}.nav-pills .nav-link{border-radius:var(--bs-nav-pills-border-radius)}.nav-pills .nav-link.active,.nav-pills .show>.nav-link{color:var(--bs-nav-pills-link-active-color);background-color:var(--bs-nav-pills-link-active-bg)}.nav-underline{--bs-nav-underline-gap: 1rem;--bs-nav-underline-border-width: .125rem;--bs-nav-underline-link-active-color: var(--bs-emphasis-color);gap:var(--bs-nav-underline-gap)}.nav-underline .nav-link{padding-right:0;padding-left:0;border-bottom:var(--bs-nav-underline-border-width) solid transparent}.nav-underline .nav-link:hover,.nav-underline .nav-link:focus{border-bottom-color:currentcolor}.nav-underline .nav-link.active,.nav-underline .show>.nav-link{font-weight:700;color:var(--bs-nav-underline-link-active-color);border-bottom-color:currentcolor}.nav-fill>.nav-link,.nav-fill .nav-item{flex:1 1 auto;text-align:center}.nav-justified>.nav-link,.nav-justified .nav-item{flex-basis:0;flex-grow:1;text-align:center}.nav-fill .nav-item .nav-link,.nav-justified .nav-item .nav-link{width:100%}.tab-content>.tab-pane{display:none}.tab-content>.active{display:block}.navbar{--bs-navbar-padding-x: 0;--bs-navbar-padding-y: .5rem;--bs-navbar-color: rgba(var(--bs-emphasis-color-rgb), .65);--bs-navbar-hover-color: rgba(var(--bs-emphasis-color-rgb), .8);--bs-navbar-disabled-color: rgba(var(--bs-emphasis-color-rgb), .3);--bs-navbar-active-color: rgba(var(--bs-emphasis-color-rgb), 1);--bs-navbar-brand-padding-y: .3125rem;--bs-navbar-brand-margin-end: 1rem;--bs-navbar-brand-font-size: 1.25rem;--bs-navbar-brand-color: rgba(var(--bs-emphasis-color-rgb), 1);--bs-navbar-brand-hover-color: rgba(var(--bs-emphasis-color-rgb), 1);--bs-navbar-nav-link-padding-x: .5rem;--bs-navbar-toggler-padding-y: .25rem;--bs-navbar-toggler-padding-x: .75rem;--bs-navbar-toggler-font-size: 1.25rem;--bs-navbar-toggler-icon-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%2833, 37, 41, 0.75%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");--bs-navbar-toggler-border-color: rgba(var(--bs-emphasis-color-rgb), .15);--bs-navbar-toggler-border-radius: var(--bs-border-radius);--bs-navbar-toggler-focus-width: .25rem;--bs-navbar-toggler-transition: box-shadow .15s ease-in-out;position:relative;display:flex;flex-wrap:wrap;align-items:center;justify-content:space-between;padding:var(--bs-navbar-padding-y) var(--bs-navbar-padding-x)}.navbar>.container,.navbar>.container-fluid,.navbar>.container-sm,.navbar>.container-md,.navbar>.container-lg,.navbar>.container-xl,.navbar>.container-xxl{display:flex;flex-wrap:inherit;align-items:center;justify-content:space-between}.navbar-brand{padding-top:var(--bs-navbar-brand-padding-y);padding-bottom:var(--bs-navbar-brand-padding-y);margin-right:var(--bs-navbar-brand-margin-end);font-size:var(--bs-navbar-brand-font-size);color:var(--bs-navbar-brand-color);text-decoration:none;white-space:nowrap}.navbar-brand:hover,.navbar-brand:focus{color:var(--bs-navbar-brand-hover-color)}.navbar-nav{--bs-nav-link-padding-x: 0;--bs-nav-link-padding-y: .5rem;--bs-nav-link-font-weight: ;--bs-nav-link-color: var(--bs-navbar-color);--bs-nav-link-hover-color: var(--bs-navbar-hover-color);--bs-nav-link-disabled-color: var(--bs-navbar-disabled-color);display:flex;flex-direction:column;padding-left:0;margin-bottom:0;list-style:none}.navbar-nav .nav-link.active,.navbar-nav .nav-link.show{color:var(--bs-navbar-active-color)}.navbar-nav .dropdown-menu{position:static}.navbar-text{padding-top:.5rem;padding-bottom:.5rem;color:var(--bs-navbar-color)}.navbar-text a,.navbar-text a:hover,.navbar-text a:focus{color:var(--bs-navbar-active-color)}.navbar-collapse{flex-basis:100%;flex-grow:1;align-items:center}.navbar-toggler{padding:var(--bs-navbar-toggler-padding-y) var(--bs-navbar-toggler-padding-x);font-size:var(--bs-navbar-toggler-font-size);line-height:1;color:var(--bs-navbar-color);background-color:transparent;border:var(--bs-border-width) solid var(--bs-navbar-toggler-border-color);border-radius:var(--bs-navbar-toggler-border-radius);transition:var(--bs-navbar-toggler-transition)}@media (prefers-reduced-motion: reduce){.navbar-toggler{transition:none}}.navbar-toggler:hover{text-decoration:none}.navbar-toggler:focus{text-decoration:none;outline:0;box-shadow:0 0 0 var(--bs-navbar-toggler-focus-width)}.navbar-toggler-icon{display:inline-block;width:1.5em;height:1.5em;vertical-align:middle;background-image:var(--bs-navbar-toggler-icon-bg);background-repeat:no-repeat;background-position:center;background-size:100%}.navbar-nav-scroll{max-height:var(--bs-scroll-height, 75vh);overflow-y:auto}@media (min-width: 576px){.navbar-expand-sm{flex-wrap:nowrap;justify-content:flex-start}.navbar-expand-sm .navbar-nav{flex-direction:row}.navbar-expand-sm .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-sm .navbar-nav .nav-link{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-sm .navbar-nav-scroll{overflow:visible}.navbar-expand-sm .navbar-collapse{display:flex!important;flex-basis:auto}.navbar-expand-sm .navbar-toggler{display:none}.navbar-expand-sm .offcanvas{position:static;z-index:auto;flex-grow:1;width:auto!important;height:auto!important;visibility:visible!important;background-color:transparent!important;border:0!important;transform:none!important;transition:none}.navbar-expand-sm .offcanvas .offcanvas-header{display:none}.navbar-expand-sm .offcanvas .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 768px){.navbar-expand-md{flex-wrap:nowrap;justify-content:flex-start}.navbar-expand-md .navbar-nav{flex-direction:row}.navbar-expand-md .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-md .navbar-nav .nav-link{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-md .navbar-nav-scroll{overflow:visible}.navbar-expand-md .navbar-collapse{display:flex!important;flex-basis:auto}.navbar-expand-md .navbar-toggler{display:none}.navbar-expand-md .offcanvas{position:static;z-index:auto;flex-grow:1;width:auto!important;height:auto!important;visibility:visible!important;background-color:transparent!important;border:0!important;transform:none!important;transition:none}.navbar-expand-md .offcanvas .offcanvas-header{display:none}.navbar-expand-md .offcanvas .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 992px){.navbar-expand-lg{flex-wrap:nowrap;justify-content:flex-start}.navbar-expand-lg .navbar-nav{flex-direction:row}.navbar-expand-lg .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-lg .navbar-nav .nav-link{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-lg .navbar-nav-scroll{overflow:visible}.navbar-expand-lg .navbar-collapse{display:flex!important;flex-basis:auto}.navbar-expand-lg .navbar-toggler{display:none}.navbar-expand-lg .offcanvas{position:static;z-index:auto;flex-grow:1;width:auto!important;height:auto!important;visibility:visible!important;background-color:transparent!important;border:0!important;transform:none!important;transition:none}.navbar-expand-lg .offcanvas .offcanvas-header{display:none}.navbar-expand-lg .offcanvas .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 1200px){.navbar-expand-xl{flex-wrap:nowrap;justify-content:flex-start}.navbar-expand-xl .navbar-nav{flex-direction:row}.navbar-expand-xl .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-xl .navbar-nav .nav-link{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-xl .navbar-nav-scroll{overflow:visible}.navbar-expand-xl .navbar-collapse{display:flex!important;flex-basis:auto}.navbar-expand-xl .navbar-toggler{display:none}.navbar-expand-xl .offcanvas{position:static;z-index:auto;flex-grow:1;width:auto!important;height:auto!important;visibility:visible!important;background-color:transparent!important;border:0!important;transform:none!important;transition:none}.navbar-expand-xl .offcanvas .offcanvas-header{display:none}.navbar-expand-xl .offcanvas .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 1400px){.navbar-expand-xxl{flex-wrap:nowrap;justify-content:flex-start}.navbar-expand-xxl .navbar-nav{flex-direction:row}.navbar-expand-xxl .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-xxl .navbar-nav .nav-link{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-xxl .navbar-nav-scroll{overflow:visible}.navbar-expand-xxl .navbar-collapse{display:flex!important;flex-basis:auto}.navbar-expand-xxl .navbar-toggler{display:none}.navbar-expand-xxl .offcanvas{position:static;z-index:auto;flex-grow:1;width:auto!important;height:auto!important;visibility:visible!important;background-color:transparent!important;border:0!important;transform:none!important;transition:none}.navbar-expand-xxl .offcanvas .offcanvas-header{display:none}.navbar-expand-xxl .offcanvas .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible}}.navbar-expand{flex-wrap:nowrap;justify-content:flex-start}.navbar-expand .navbar-nav{flex-direction:row}.navbar-expand .navbar-nav .dropdown-menu{position:absolute}.navbar-expand .navbar-nav .nav-link{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand .navbar-nav-scroll{overflow:visible}.navbar-expand .navbar-collapse{display:flex!important;flex-basis:auto}.navbar-expand .navbar-toggler{display:none}.navbar-expand .offcanvas{position:static;z-index:auto;flex-grow:1;width:auto!important;height:auto!important;visibility:visible!important;background-color:transparent!important;border:0!important;transform:none!important;transition:none}.navbar-expand .offcanvas .offcanvas-header{display:none}.navbar-expand .offcanvas .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible}.navbar-dark,.navbar[data-bs-theme=dark]{--bs-navbar-color: rgba(255, 255, 255, .55);--bs-navbar-hover-color: rgba(255, 255, 255, .75);--bs-navbar-disabled-color: rgba(255, 255, 255, .25);--bs-navbar-active-color: #fff;--bs-navbar-brand-color: #fff;--bs-navbar-brand-hover-color: #fff;--bs-navbar-toggler-border-color: rgba(255, 255, 255, .1);--bs-navbar-toggler-icon-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%28255, 255, 255, 0.55%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e")}[data-bs-theme=dark] .navbar-toggler-icon{--bs-navbar-toggler-icon-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%28255, 255, 255, 0.55%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e")}.card{--bs-card-spacer-y: 1rem;--bs-card-spacer-x: 1rem;--bs-card-title-spacer-y: .5rem;--bs-card-title-color: ;--bs-card-subtitle-color: ;--bs-card-border-width: var(--bs-border-width);--bs-card-border-color: var(--bs-border-color-translucent);--bs-card-border-radius: var(--bs-border-radius);--bs-card-box-shadow: ;--bs-card-inner-border-radius: calc(var(--bs-border-radius) - (var(--bs-border-width)));--bs-card-cap-padding-y: .5rem;--bs-card-cap-padding-x: 1rem;--bs-card-cap-bg: rgba(var(--bs-body-color-rgb), .03);--bs-card-cap-color: ;--bs-card-height: ;--bs-card-color: ;--bs-card-bg: var(--bs-body-bg);--bs-card-img-overlay-padding: 1rem;--bs-card-group-margin: .75rem;position:relative;display:flex;flex-direction:column;min-width:0;height:var(--bs-card-height);color:var(--bs-body-color);word-wrap:break-word;background-color:var(--bs-card-bg);background-clip:border-box;border:var(--bs-card-border-width) solid var(--bs-card-border-color);border-radius:var(--bs-card-border-radius)}.card>hr{margin-right:0;margin-left:0}.card>.list-group{border-top:inherit;border-bottom:inherit}.card>.list-group:first-child{border-top-width:0;border-top-left-radius:var(--bs-card-inner-border-radius);border-top-right-radius:var(--bs-card-inner-border-radius)}.card>.list-group:last-child{border-bottom-width:0;border-bottom-right-radius:var(--bs-card-inner-border-radius);border-bottom-left-radius:var(--bs-card-inner-border-radius)}.card>.card-header+.list-group,.card>.list-group+.card-footer{border-top:0}.card-body{flex:1 1 auto;padding:var(--bs-card-spacer-y) var(--bs-card-spacer-x);color:var(--bs-card-color)}.card-title{margin-bottom:var(--bs-card-title-spacer-y);color:var(--bs-card-title-color)}.card-subtitle{margin-top:calc(-.5 * var(--bs-card-title-spacer-y));margin-bottom:0;color:var(--bs-card-subtitle-color)}.card-text:last-child{margin-bottom:0}.card-link+.card-link{margin-left:var(--bs-card-spacer-x)}.card-header{padding:var(--bs-card-cap-padding-y) var(--bs-card-cap-padding-x);margin-bottom:0;color:var(--bs-card-cap-color);background-color:var(--bs-card-cap-bg);border-bottom:var(--bs-card-border-width) solid var(--bs-card-border-color)}.card-header:first-child{border-radius:var(--bs-card-inner-border-radius) var(--bs-card-inner-border-radius) 0 0}.card-footer{padding:var(--bs-card-cap-padding-y) var(--bs-card-cap-padding-x);color:var(--bs-card-cap-color);background-color:var(--bs-card-cap-bg);border-top:var(--bs-card-border-width) solid var(--bs-card-border-color)}.card-footer:last-child{border-radius:0 0 var(--bs-card-inner-border-radius) var(--bs-card-inner-border-radius)}.card-header-tabs{margin-right:calc(-.5 * var(--bs-card-cap-padding-x));margin-bottom:calc(-1 * var(--bs-card-cap-padding-y));margin-left:calc(-.5 * var(--bs-card-cap-padding-x));border-bottom:0}.card-header-tabs .nav-link.active{background-color:var(--bs-card-bg);border-bottom-color:var(--bs-card-bg)}.card-header-pills{margin-right:calc(-.5 * var(--bs-card-cap-padding-x));margin-left:calc(-.5 * var(--bs-card-cap-padding-x))}.card-img-overlay{position:absolute;inset:0;padding:var(--bs-card-img-overlay-padding);border-radius:var(--bs-card-inner-border-radius)}.card-img,.card-img-top,.card-img-bottom{width:100%}.card-img,.card-img-top{border-top-left-radius:var(--bs-card-inner-border-radius);border-top-right-radius:var(--bs-card-inner-border-radius)}.card-img,.card-img-bottom{border-bottom-right-radius:var(--bs-card-inner-border-radius);border-bottom-left-radius:var(--bs-card-inner-border-radius)}.card-group>.card{margin-bottom:var(--bs-card-group-margin)}@media (min-width: 576px){.card-group{display:flex;flex-flow:row wrap}.card-group>.card{flex:1 0 0%;margin-bottom:0}.card-group>.card+.card{margin-left:0;border-left:0}.card-group>.card:not(:last-child){border-top-right-radius:0;border-bottom-right-radius:0}.card-group>.card:not(:last-child) .card-img-top,.card-group>.card:not(:last-child) .card-header{border-top-right-radius:0}.card-group>.card:not(:last-child) .card-img-bottom,.card-group>.card:not(:last-child) .card-footer{border-bottom-right-radius:0}.card-group>.card:not(:first-child){border-top-left-radius:0;border-bottom-left-radius:0}.card-group>.card:not(:first-child) .card-img-top,.card-group>.card:not(:first-child) .card-header{border-top-left-radius:0}.card-group>.card:not(:first-child) .card-img-bottom,.card-group>.card:not(:first-child) .card-footer{border-bottom-left-radius:0}}.accordion{--bs-accordion-color: var(--bs-body-color);--bs-accordion-bg: var(--bs-body-bg);--bs-accordion-transition: color .15s ease-in-out, background-color .15s ease-in-out, border-color .15s ease-in-out, box-shadow .15s ease-in-out, border-radius .15s ease;--bs-accordion-border-color: var(--bs-border-color);--bs-accordion-border-width: var(--bs-border-width);--bs-accordion-border-radius: var(--bs-border-radius);--bs-accordion-inner-border-radius: calc(var(--bs-border-radius) - (var(--bs-border-width)));--bs-accordion-btn-padding-x: 1.25rem;--bs-accordion-btn-padding-y: 1rem;--bs-accordion-btn-color: var(--bs-body-color);--bs-accordion-btn-bg: var(--bs-accordion-bg);--bs-accordion-btn-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23212529'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");--bs-accordion-btn-icon-width: 1.25rem;--bs-accordion-btn-icon-transform: rotate(-180deg);--bs-accordion-btn-icon-transition: transform .2s ease-in-out;--bs-accordion-btn-active-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23052c65'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");--bs-accordion-btn-focus-border-color: #86b7fe;--bs-accordion-btn-focus-box-shadow: 0 0 0 .25rem rgba(13, 110, 253, .25);--bs-accordion-body-padding-x: 1.25rem;--bs-accordion-body-padding-y: 1rem;--bs-accordion-active-color: var(--bs-primary-text-emphasis);--bs-accordion-active-bg: var(--bs-primary-bg-subtle)}.accordion-button{position:relative;display:flex;align-items:center;width:100%;padding:var(--bs-accordion-btn-padding-y) var(--bs-accordion-btn-padding-x);font-size:1rem;color:var(--bs-accordion-btn-color);text-align:left;background-color:var(--bs-accordion-btn-bg);border:0;border-radius:0;overflow-anchor:none;transition:var(--bs-accordion-transition)}@media (prefers-reduced-motion: reduce){.accordion-button{transition:none}}.accordion-button:not(.collapsed){color:var(--bs-accordion-active-color);background-color:var(--bs-accordion-active-bg);box-shadow:inset 0 calc(-1 * var(--bs-accordion-border-width)) 0 var(--bs-accordion-border-color)}.accordion-button:not(.collapsed):after{background-image:var(--bs-accordion-btn-active-icon);transform:var(--bs-accordion-btn-icon-transform)}.accordion-button:after{flex-shrink:0;width:var(--bs-accordion-btn-icon-width);height:var(--bs-accordion-btn-icon-width);margin-left:auto;content:"";background-image:var(--bs-accordion-btn-icon);background-repeat:no-repeat;background-size:var(--bs-accordion-btn-icon-width);transition:var(--bs-accordion-btn-icon-transition)}@media (prefers-reduced-motion: reduce){.accordion-button:after{transition:none}}.accordion-button:hover{z-index:2}.accordion-button:focus{z-index:3;border-color:var(--bs-accordion-btn-focus-border-color);outline:0;box-shadow:var(--bs-accordion-btn-focus-box-shadow)}.accordion-header{margin-bottom:0}.accordion-item{color:var(--bs-accordion-color);background-color:var(--bs-accordion-bg);border:var(--bs-accordion-border-width) solid var(--bs-accordion-border-color)}.accordion-item:first-of-type{border-top-left-radius:var(--bs-accordion-border-radius);border-top-right-radius:var(--bs-accordion-border-radius)}.accordion-item:first-of-type .accordion-button{border-top-left-radius:var(--bs-accordion-inner-border-radius);border-top-right-radius:var(--bs-accordion-inner-border-radius)}.accordion-item:not(:first-of-type){border-top:0}.accordion-item:last-of-type{border-bottom-right-radius:var(--bs-accordion-border-radius);border-bottom-left-radius:var(--bs-accordion-border-radius)}.accordion-item:last-of-type .accordion-button.collapsed{border-bottom-right-radius:var(--bs-accordion-inner-border-radius);border-bottom-left-radius:var(--bs-accordion-inner-border-radius)}.accordion-item:last-of-type .accordion-collapse{border-bottom-right-radius:var(--bs-accordion-border-radius);border-bottom-left-radius:var(--bs-accordion-border-radius)}.accordion-body{padding:var(--bs-accordion-body-padding-y) var(--bs-accordion-body-padding-x)}.accordion-flush .accordion-collapse{border-width:0}.accordion-flush .accordion-item{border-right:0;border-left:0;border-radius:0}.accordion-flush .accordion-item:first-child{border-top:0}.accordion-flush .accordion-item:last-child{border-bottom:0}.accordion-flush .accordion-item .accordion-button,.accordion-flush .accordion-item .accordion-button.collapsed{border-radius:0}[data-bs-theme=dark] .accordion-button:after{--bs-accordion-btn-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%236ea8fe'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");--bs-accordion-btn-active-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%236ea8fe'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e")}.breadcrumb{--bs-breadcrumb-padding-x: 0;--bs-breadcrumb-padding-y: 0;--bs-breadcrumb-margin-bottom: 1rem;--bs-breadcrumb-bg: ;--bs-breadcrumb-border-radius: ;--bs-breadcrumb-divider-color: var(--bs-secondary-color);--bs-breadcrumb-item-padding-x: .5rem;--bs-breadcrumb-item-active-color: var(--bs-secondary-color);display:flex;flex-wrap:wrap;padding:var(--bs-breadcrumb-padding-y) var(--bs-breadcrumb-padding-x);margin-bottom:var(--bs-breadcrumb-margin-bottom);font-size:var(--bs-breadcrumb-font-size);list-style:none;background-color:var(--bs-breadcrumb-bg);border-radius:var(--bs-breadcrumb-border-radius)}.breadcrumb-item+.breadcrumb-item{padding-left:var(--bs-breadcrumb-item-padding-x)}.breadcrumb-item+.breadcrumb-item:before{float:left;padding-right:var(--bs-breadcrumb-item-padding-x);color:var(--bs-breadcrumb-divider-color);content:var(--bs-breadcrumb-divider, "/")}.breadcrumb-item.active{color:var(--bs-breadcrumb-item-active-color)}.pagination{--bs-pagination-padding-x: .75rem;--bs-pagination-padding-y: .375rem;--bs-pagination-font-size: 1rem;--bs-pagination-color: var(--bs-link-color);--bs-pagination-bg: var(--bs-body-bg);--bs-pagination-border-width: var(--bs-border-width);--bs-pagination-border-color: var(--bs-border-color);--bs-pagination-border-radius: var(--bs-border-radius);--bs-pagination-hover-color: var(--bs-link-hover-color);--bs-pagination-hover-bg: var(--bs-tertiary-bg);--bs-pagination-hover-border-color: var(--bs-border-color);--bs-pagination-focus-color: var(--bs-link-hover-color);--bs-pagination-focus-bg: var(--bs-secondary-bg);--bs-pagination-focus-box-shadow: 0 0 0 .25rem rgba(13, 110, 253, .25);--bs-pagination-active-color: #fff;--bs-pagination-active-bg: #0d6efd;--bs-pagination-active-border-color: #0d6efd;--bs-pagination-disabled-color: var(--bs-secondary-color);--bs-pagination-disabled-bg: var(--bs-secondary-bg);--bs-pagination-disabled-border-color: var(--bs-border-color);display:flex;padding-left:0;list-style:none}.page-link{position:relative;display:block;padding:var(--bs-pagination-padding-y) var(--bs-pagination-padding-x);font-size:var(--bs-pagination-font-size);color:var(--bs-pagination-color);text-decoration:none;background-color:var(--bs-pagination-bg);border:var(--bs-pagination-border-width) solid var(--bs-pagination-border-color);transition:color .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out}@media (prefers-reduced-motion: reduce){.page-link{transition:none}}.page-link:hover{z-index:2;color:var(--bs-pagination-hover-color);background-color:var(--bs-pagination-hover-bg);border-color:var(--bs-pagination-hover-border-color)}.page-link:focus{z-index:3;color:var(--bs-pagination-focus-color);background-color:var(--bs-pagination-focus-bg);outline:0;box-shadow:var(--bs-pagination-focus-box-shadow)}.page-link.active,.active>.page-link{z-index:3;color:var(--bs-pagination-active-color);background-color:var(--bs-pagination-active-bg);border-color:var(--bs-pagination-active-border-color)}.page-link.disabled,.disabled>.page-link{color:var(--bs-pagination-disabled-color);pointer-events:none;background-color:var(--bs-pagination-disabled-bg);border-color:var(--bs-pagination-disabled-border-color)}.page-item:not(:first-child) .page-link{margin-left:calc(var(--bs-border-width) * -1)}.page-item:first-child .page-link{border-top-left-radius:var(--bs-pagination-border-radius);border-bottom-left-radius:var(--bs-pagination-border-radius)}.page-item:last-child .page-link{border-top-right-radius:var(--bs-pagination-border-radius);border-bottom-right-radius:var(--bs-pagination-border-radius)}.pagination-lg{--bs-pagination-padding-x: 1.5rem;--bs-pagination-padding-y: .75rem;--bs-pagination-font-size: 1.25rem;--bs-pagination-border-radius: var(--bs-border-radius-lg)}.pagination-sm{--bs-pagination-padding-x: .5rem;--bs-pagination-padding-y: .25rem;--bs-pagination-font-size: .875rem;--bs-pagination-border-radius: var(--bs-border-radius-sm)}.badge{--bs-badge-padding-x: .65em;--bs-badge-padding-y: .35em;--bs-badge-font-size: .75em;--bs-badge-font-weight: 700;--bs-badge-color: #fff;--bs-badge-border-radius: var(--bs-border-radius);display:inline-block;padding:var(--bs-badge-padding-y) var(--bs-badge-padding-x);font-size:var(--bs-badge-font-size);font-weight:var(--bs-badge-font-weight);line-height:1;color:var(--bs-badge-color);text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:var(--bs-badge-border-radius)}.badge:empty{display:none}.btn .badge{position:relative;top:-1px}.alert{--bs-alert-bg: transparent;--bs-alert-padding-x: 1rem;--bs-alert-padding-y: 1rem;--bs-alert-margin-bottom: 1rem;--bs-alert-color: inherit;--bs-alert-border-color: transparent;--bs-alert-border: var(--bs-border-width) solid var(--bs-alert-border-color);--bs-alert-border-radius: var(--bs-border-radius);--bs-alert-link-color: inherit;position:relative;padding:var(--bs-alert-padding-y) var(--bs-alert-padding-x);margin-bottom:var(--bs-alert-margin-bottom);color:var(--bs-alert-color);background-color:var(--bs-alert-bg);border:var(--bs-alert-border);border-radius:var(--bs-alert-border-radius)}.alert-heading{color:inherit}.alert-link{font-weight:700;color:var(--bs-alert-link-color)}.alert-dismissible{padding-right:3rem}.alert-dismissible .btn-close{position:absolute;top:0;right:0;z-index:2;padding:1.25rem 1rem}.alert-primary{--bs-alert-color: var(--bs-primary-text-emphasis);--bs-alert-bg: var(--bs-primary-bg-subtle);--bs-alert-border-color: var(--bs-primary-border-subtle);--bs-alert-link-color: var(--bs-primary-text-emphasis)}.alert-secondary{--bs-alert-color: var(--bs-secondary-text-emphasis);--bs-alert-bg: var(--bs-secondary-bg-subtle);--bs-alert-border-color: var(--bs-secondary-border-subtle);--bs-alert-link-color: var(--bs-secondary-text-emphasis)}.alert-success{--bs-alert-color: var(--bs-success-text-emphasis);--bs-alert-bg: var(--bs-success-bg-subtle);--bs-alert-border-color: var(--bs-success-border-subtle);--bs-alert-link-color: var(--bs-success-text-emphasis)}.alert-info{--bs-alert-color: var(--bs-info-text-emphasis);--bs-alert-bg: var(--bs-info-bg-subtle);--bs-alert-border-color: var(--bs-info-border-subtle);--bs-alert-link-color: var(--bs-info-text-emphasis)}.alert-warning{--bs-alert-color: var(--bs-warning-text-emphasis);--bs-alert-bg: var(--bs-warning-bg-subtle);--bs-alert-border-color: var(--bs-warning-border-subtle);--bs-alert-link-color: var(--bs-warning-text-emphasis)}.alert-danger{--bs-alert-color: var(--bs-danger-text-emphasis);--bs-alert-bg: var(--bs-danger-bg-subtle);--bs-alert-border-color: var(--bs-danger-border-subtle);--bs-alert-link-color: var(--bs-danger-text-emphasis)}.alert-light{--bs-alert-color: var(--bs-light-text-emphasis);--bs-alert-bg: var(--bs-light-bg-subtle);--bs-alert-border-color: var(--bs-light-border-subtle);--bs-alert-link-color: var(--bs-light-text-emphasis)}.alert-dark{--bs-alert-color: var(--bs-dark-text-emphasis);--bs-alert-bg: var(--bs-dark-bg-subtle);--bs-alert-border-color: var(--bs-dark-border-subtle);--bs-alert-link-color: var(--bs-dark-text-emphasis)}@keyframes progress-bar-stripes{0%{background-position-x:1rem}}.progress,.progress-stacked{--bs-progress-height: 1rem;--bs-progress-font-size: .75rem;--bs-progress-bg: var(--bs-secondary-bg);--bs-progress-border-radius: var(--bs-border-radius);--bs-progress-box-shadow: var(--bs-box-shadow-inset);--bs-progress-bar-color: #fff;--bs-progress-bar-bg: #0d6efd;--bs-progress-bar-transition: width .6s ease;display:flex;height:var(--bs-progress-height);overflow:hidden;font-size:var(--bs-progress-font-size);background-color:var(--bs-progress-bg);border-radius:var(--bs-progress-border-radius)}.progress-bar{display:flex;flex-direction:column;justify-content:center;overflow:hidden;color:var(--bs-progress-bar-color);text-align:center;white-space:nowrap;background-color:var(--bs-progress-bar-bg);transition:var(--bs-progress-bar-transition)}@media (prefers-reduced-motion: reduce){.progress-bar{transition:none}}.progress-bar-striped{background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-size:var(--bs-progress-height) var(--bs-progress-height)}.progress-stacked>.progress{overflow:visible}.progress-stacked>.progress>.progress-bar{width:100%}.progress-bar-animated{animation:1s linear infinite progress-bar-stripes}@media (prefers-reduced-motion: reduce){.progress-bar-animated{animation:none}}.list-group{--bs-list-group-color: var(--bs-body-color);--bs-list-group-bg: var(--bs-body-bg);--bs-list-group-border-color: var(--bs-border-color);--bs-list-group-border-width: var(--bs-border-width);--bs-list-group-border-radius: var(--bs-border-radius);--bs-list-group-item-padding-x: 1rem;--bs-list-group-item-padding-y: .5rem;--bs-list-group-action-color: var(--bs-secondary-color);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-tertiary-bg);--bs-list-group-action-active-color: var(--bs-body-color);--bs-list-group-action-active-bg: var(--bs-secondary-bg);--bs-list-group-disabled-color: var(--bs-secondary-color);--bs-list-group-disabled-bg: var(--bs-body-bg);--bs-list-group-active-color: #fff;--bs-list-group-active-bg: #0d6efd;--bs-list-group-active-border-color: #0d6efd;display:flex;flex-direction:column;padding-left:0;margin-bottom:0;border-radius:var(--bs-list-group-border-radius)}.list-group-numbered{list-style-type:none;counter-reset:section}.list-group-numbered>.list-group-item:before{content:counters(section,".") ". ";counter-increment:section}.list-group-item-action{width:100%;color:var(--bs-list-group-action-color);text-align:inherit}.list-group-item-action:hover,.list-group-item-action:focus{z-index:1;color:var(--bs-list-group-action-hover-color);text-decoration:none;background-color:var(--bs-list-group-action-hover-bg)}.list-group-item-action:active{color:var(--bs-list-group-action-active-color);background-color:var(--bs-list-group-action-active-bg)}.list-group-item{position:relative;display:block;padding:var(--bs-list-group-item-padding-y) var(--bs-list-group-item-padding-x);color:var(--bs-list-group-color);text-decoration:none;background-color:var(--bs-list-group-bg);border:var(--bs-list-group-border-width) solid var(--bs-list-group-border-color)}.list-group-item:first-child{border-top-left-radius:inherit;border-top-right-radius:inherit}.list-group-item:last-child{border-bottom-right-radius:inherit;border-bottom-left-radius:inherit}.list-group-item.disabled,.list-group-item:disabled{color:var(--bs-list-group-disabled-color);pointer-events:none;background-color:var(--bs-list-group-disabled-bg)}.list-group-item.active{z-index:2;color:var(--bs-list-group-active-color);background-color:var(--bs-list-group-active-bg);border-color:var(--bs-list-group-active-border-color)}.list-group-item+.list-group-item{border-top-width:0}.list-group-item+.list-group-item.active{margin-top:calc(-1 * var(--bs-list-group-border-width));border-top-width:var(--bs-list-group-border-width)}.list-group-horizontal{flex-direction:row}.list-group-horizontal>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal>.list-group-item.active{margin-top:0}.list-group-horizontal>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}@media (min-width: 576px){.list-group-horizontal-sm{flex-direction:row}.list-group-horizontal-sm>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-sm>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-sm>.list-group-item.active{margin-top:0}.list-group-horizontal-sm>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-sm>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 768px){.list-group-horizontal-md{flex-direction:row}.list-group-horizontal-md>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-md>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-md>.list-group-item.active{margin-top:0}.list-group-horizontal-md>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-md>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 992px){.list-group-horizontal-lg{flex-direction:row}.list-group-horizontal-lg>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-lg>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-lg>.list-group-item.active{margin-top:0}.list-group-horizontal-lg>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-lg>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 1200px){.list-group-horizontal-xl{flex-direction:row}.list-group-horizontal-xl>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-xl>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-xl>.list-group-item.active{margin-top:0}.list-group-horizontal-xl>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-xl>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 1400px){.list-group-horizontal-xxl{flex-direction:row}.list-group-horizontal-xxl>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-xxl>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-xxl>.list-group-item.active{margin-top:0}.list-group-horizontal-xxl>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-xxl>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}.list-group-flush{border-radius:0}.list-group-flush>.list-group-item{border-width:0 0 var(--bs-list-group-border-width)}.list-group-flush>.list-group-item:last-child{border-bottom-width:0}.list-group-item-primary{--bs-list-group-color: var(--bs-primary-text-emphasis);--bs-list-group-bg: var(--bs-primary-bg-subtle);--bs-list-group-border-color: var(--bs-primary-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-primary-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-primary-border-subtle);--bs-list-group-active-color: var(--bs-primary-bg-subtle);--bs-list-group-active-bg: var(--bs-primary-text-emphasis);--bs-list-group-active-border-color: var(--bs-primary-text-emphasis)}.list-group-item-secondary{--bs-list-group-color: var(--bs-secondary-text-emphasis);--bs-list-group-bg: var(--bs-secondary-bg-subtle);--bs-list-group-border-color: var(--bs-secondary-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-secondary-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-secondary-border-subtle);--bs-list-group-active-color: var(--bs-secondary-bg-subtle);--bs-list-group-active-bg: var(--bs-secondary-text-emphasis);--bs-list-group-active-border-color: var(--bs-secondary-text-emphasis)}.list-group-item-success{--bs-list-group-color: var(--bs-success-text-emphasis);--bs-list-group-bg: var(--bs-success-bg-subtle);--bs-list-group-border-color: var(--bs-success-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-success-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-success-border-subtle);--bs-list-group-active-color: var(--bs-success-bg-subtle);--bs-list-group-active-bg: var(--bs-success-text-emphasis);--bs-list-group-active-border-color: var(--bs-success-text-emphasis)}.list-group-item-info{--bs-list-group-color: var(--bs-info-text-emphasis);--bs-list-group-bg: var(--bs-info-bg-subtle);--bs-list-group-border-color: var(--bs-info-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-info-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-info-border-subtle);--bs-list-group-active-color: var(--bs-info-bg-subtle);--bs-list-group-active-bg: var(--bs-info-text-emphasis);--bs-list-group-active-border-color: var(--bs-info-text-emphasis)}.list-group-item-warning{--bs-list-group-color: var(--bs-warning-text-emphasis);--bs-list-group-bg: var(--bs-warning-bg-subtle);--bs-list-group-border-color: var(--bs-warning-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-warning-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-warning-border-subtle);--bs-list-group-active-color: var(--bs-warning-bg-subtle);--bs-list-group-active-bg: var(--bs-warning-text-emphasis);--bs-list-group-active-border-color: var(--bs-warning-text-emphasis)}.list-group-item-danger{--bs-list-group-color: var(--bs-danger-text-emphasis);--bs-list-group-bg: var(--bs-danger-bg-subtle);--bs-list-group-border-color: var(--bs-danger-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-danger-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-danger-border-subtle);--bs-list-group-active-color: var(--bs-danger-bg-subtle);--bs-list-group-active-bg: var(--bs-danger-text-emphasis);--bs-list-group-active-border-color: var(--bs-danger-text-emphasis)}.list-group-item-light{--bs-list-group-color: var(--bs-light-text-emphasis);--bs-list-group-bg: var(--bs-light-bg-subtle);--bs-list-group-border-color: var(--bs-light-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-light-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-light-border-subtle);--bs-list-group-active-color: var(--bs-light-bg-subtle);--bs-list-group-active-bg: var(--bs-light-text-emphasis);--bs-list-group-active-border-color: var(--bs-light-text-emphasis)}.list-group-item-dark{--bs-list-group-color: var(--bs-dark-text-emphasis);--bs-list-group-bg: var(--bs-dark-bg-subtle);--bs-list-group-border-color: var(--bs-dark-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-dark-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-dark-border-subtle);--bs-list-group-active-color: var(--bs-dark-bg-subtle);--bs-list-group-active-bg: var(--bs-dark-text-emphasis);--bs-list-group-active-border-color: var(--bs-dark-text-emphasis)}.btn-close{--bs-btn-close-color: #000;--bs-btn-close-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23000'%3e%3cpath d='M.293.293a1 1 0 0 1 1.414 0L8 6.586 14.293.293a1 1 0 1 1 1.414 1.414L9.414 8l6.293 6.293a1 1 0 0 1-1.414 1.414L8 9.414l-6.293 6.293a1 1 0 0 1-1.414-1.414L6.586 8 .293 1.707a1 1 0 0 1 0-1.414z'/%3e%3c/svg%3e");--bs-btn-close-opacity: .5;--bs-btn-close-hover-opacity: .75;--bs-btn-close-focus-shadow: 0 0 0 .25rem rgba(13, 110, 253, .25);--bs-btn-close-focus-opacity: 1;--bs-btn-close-disabled-opacity: .25;--bs-btn-close-white-filter: invert(1) grayscale(100%) brightness(200%);box-sizing:content-box;width:1em;height:1em;padding:.25em;color:var(--bs-btn-close-color);background:transparent var(--bs-btn-close-bg) center/1em auto no-repeat;border:0;border-radius:.375rem;opacity:var(--bs-btn-close-opacity)}.btn-close:hover{color:var(--bs-btn-close-color);text-decoration:none;opacity:var(--bs-btn-close-hover-opacity)}.btn-close:focus{outline:0;box-shadow:var(--bs-btn-close-focus-shadow);opacity:var(--bs-btn-close-focus-opacity)}.btn-close:disabled,.btn-close.disabled{pointer-events:none;user-select:none;opacity:var(--bs-btn-close-disabled-opacity)}.btn-close-white,[data-bs-theme=dark] .btn-close{filter:var(--bs-btn-close-white-filter)}.toast{--bs-toast-zindex: 1090;--bs-toast-padding-x: .75rem;--bs-toast-padding-y: .5rem;--bs-toast-spacing: 1.5rem;--bs-toast-max-width: 350px;--bs-toast-font-size: .875rem;--bs-toast-color: ;--bs-toast-bg: rgba(var(--bs-body-bg-rgb), .85);--bs-toast-border-width: var(--bs-border-width);--bs-toast-border-color: var(--bs-border-color-translucent);--bs-toast-border-radius: var(--bs-border-radius);--bs-toast-box-shadow: var(--bs-box-shadow);--bs-toast-header-color: var(--bs-secondary-color);--bs-toast-header-bg: rgba(var(--bs-body-bg-rgb), .85);--bs-toast-header-border-color: var(--bs-border-color-translucent);width:var(--bs-toast-max-width);max-width:100%;font-size:var(--bs-toast-font-size);color:var(--bs-toast-color);pointer-events:auto;background-color:var(--bs-toast-bg);background-clip:padding-box;border:var(--bs-toast-border-width) solid var(--bs-toast-border-color);box-shadow:var(--bs-toast-box-shadow);border-radius:var(--bs-toast-border-radius)}.toast.showing{opacity:0}.toast:not(.show){display:none}.toast-container{--bs-toast-zindex: 1090;position:absolute;z-index:var(--bs-toast-zindex);width:max-content;max-width:100%;pointer-events:none}.toast-container>:not(:last-child){margin-bottom:var(--bs-toast-spacing)}.toast-header{display:flex;align-items:center;padding:var(--bs-toast-padding-y) var(--bs-toast-padding-x);color:var(--bs-toast-header-color);background-color:var(--bs-toast-header-bg);background-clip:padding-box;border-bottom:var(--bs-toast-border-width) solid var(--bs-toast-header-border-color);border-top-left-radius:calc(var(--bs-toast-border-radius) - var(--bs-toast-border-width));border-top-right-radius:calc(var(--bs-toast-border-radius) - var(--bs-toast-border-width))}.toast-header .btn-close{margin-right:calc(-.5 * var(--bs-toast-padding-x));margin-left:var(--bs-toast-padding-x)}.toast-body{padding:var(--bs-toast-padding-x);word-wrap:break-word}.modal{--bs-modal-zindex: 1055;--bs-modal-width: 500px;--bs-modal-padding: 1rem;--bs-modal-margin: .5rem;--bs-modal-color: ;--bs-modal-bg: var(--bs-body-bg);--bs-modal-border-color: var(--bs-border-color-translucent);--bs-modal-border-width: var(--bs-border-width);--bs-modal-border-radius: var(--bs-border-radius-lg);--bs-modal-box-shadow: var(--bs-box-shadow-sm);--bs-modal-inner-border-radius: calc(var(--bs-border-radius-lg) - (var(--bs-border-width)));--bs-modal-header-padding-x: 1rem;--bs-modal-header-padding-y: 1rem;--bs-modal-header-padding: 1rem 1rem;--bs-modal-header-border-color: var(--bs-border-color);--bs-modal-header-border-width: var(--bs-border-width);--bs-modal-title-line-height: 1.5;--bs-modal-footer-gap: .5rem;--bs-modal-footer-bg: ;--bs-modal-footer-border-color: var(--bs-border-color);--bs-modal-footer-border-width: var(--bs-border-width);position:fixed;top:0;left:0;z-index:var(--bs-modal-zindex);display:none;width:100%;height:100%;overflow-x:hidden;overflow-y:auto;outline:0}.modal-dialog{position:relative;width:auto;margin:var(--bs-modal-margin);pointer-events:none}.modal.fade .modal-dialog{transition:transform .3s ease-out;transform:translateY(-50px)}@media (prefers-reduced-motion: reduce){.modal.fade .modal-dialog{transition:none}}.modal.show .modal-dialog{transform:none}.modal.modal-static .modal-dialog{transform:scale(1.02)}.modal-dialog-scrollable{height:calc(100% - var(--bs-modal-margin) * 2)}.modal-dialog-scrollable .modal-content{max-height:100%;overflow:hidden}.modal-dialog-scrollable .modal-body{overflow-y:auto}.modal-dialog-centered{display:flex;align-items:center;min-height:calc(100% - var(--bs-modal-margin) * 2)}.modal-content{position:relative;display:flex;flex-direction:column;width:100%;color:var(--bs-modal-color);pointer-events:auto;background-color:var(--bs-modal-bg);background-clip:padding-box;border:var(--bs-modal-border-width) solid var(--bs-modal-border-color);border-radius:var(--bs-modal-border-radius);outline:0}.modal-backdrop{--bs-backdrop-zindex: 1050;--bs-backdrop-bg: #000;--bs-backdrop-opacity: .5;position:fixed;top:0;left:0;z-index:var(--bs-backdrop-zindex);width:100vw;height:100vh;background-color:var(--bs-backdrop-bg)}.modal-backdrop.fade{opacity:0}.modal-backdrop.show{opacity:var(--bs-backdrop-opacity)}.modal-header{display:flex;flex-shrink:0;align-items:center;justify-content:space-between;padding:var(--bs-modal-header-padding);border-bottom:var(--bs-modal-header-border-width) solid var(--bs-modal-header-border-color);border-top-left-radius:var(--bs-modal-inner-border-radius);border-top-right-radius:var(--bs-modal-inner-border-radius)}.modal-header .btn-close{padding:calc(var(--bs-modal-header-padding-y) * .5) calc(var(--bs-modal-header-padding-x) * .5);margin:calc(-.5 * var(--bs-modal-header-padding-y)) calc(-.5 * var(--bs-modal-header-padding-x)) calc(-.5 * var(--bs-modal-header-padding-y)) auto}.modal-title{margin-bottom:0;line-height:var(--bs-modal-title-line-height)}.modal-body{position:relative;flex:1 1 auto;padding:var(--bs-modal-padding)}.modal-footer{display:flex;flex-shrink:0;flex-wrap:wrap;align-items:center;justify-content:flex-end;padding:calc(var(--bs-modal-padding) - var(--bs-modal-footer-gap) * .5);background-color:var(--bs-modal-footer-bg);border-top:var(--bs-modal-footer-border-width) solid var(--bs-modal-footer-border-color);border-bottom-right-radius:var(--bs-modal-inner-border-radius);border-bottom-left-radius:var(--bs-modal-inner-border-radius)}.modal-footer>*{margin:calc(var(--bs-modal-footer-gap) * .5)}@media (min-width: 576px){.modal{--bs-modal-margin: 1.75rem;--bs-modal-box-shadow: var(--bs-box-shadow)}.modal-dialog{max-width:var(--bs-modal-width);margin-right:auto;margin-left:auto}.modal-sm{--bs-modal-width: 300px}}@media (min-width: 992px){.modal-lg,.modal-xl{--bs-modal-width: 800px}}@media (min-width: 1200px){.modal-xl{--bs-modal-width: 1140px}}.modal-fullscreen{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen .modal-header,.modal-fullscreen .modal-footer{border-radius:0}.modal-fullscreen .modal-body{overflow-y:auto}@media (max-width: 575.98px){.modal-fullscreen-sm-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-sm-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-sm-down .modal-header,.modal-fullscreen-sm-down .modal-footer{border-radius:0}.modal-fullscreen-sm-down .modal-body{overflow-y:auto}}@media (max-width: 767.98px){.modal-fullscreen-md-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-md-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-md-down .modal-header,.modal-fullscreen-md-down .modal-footer{border-radius:0}.modal-fullscreen-md-down .modal-body{overflow-y:auto}}@media (max-width: 991.98px){.modal-fullscreen-lg-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-lg-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-lg-down .modal-header,.modal-fullscreen-lg-down .modal-footer{border-radius:0}.modal-fullscreen-lg-down .modal-body{overflow-y:auto}}@media (max-width: 1199.98px){.modal-fullscreen-xl-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-xl-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-xl-down .modal-header,.modal-fullscreen-xl-down .modal-footer{border-radius:0}.modal-fullscreen-xl-down .modal-body{overflow-y:auto}}@media (max-width: 1399.98px){.modal-fullscreen-xxl-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-xxl-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-xxl-down .modal-header,.modal-fullscreen-xxl-down .modal-footer{border-radius:0}.modal-fullscreen-xxl-down .modal-body{overflow-y:auto}}.tooltip{--bs-tooltip-zindex: 1080;--bs-tooltip-max-width: 200px;--bs-tooltip-padding-x: .5rem;--bs-tooltip-padding-y: .25rem;--bs-tooltip-margin: ;--bs-tooltip-font-size: .875rem;--bs-tooltip-color: var(--bs-body-bg);--bs-tooltip-bg: var(--bs-emphasis-color);--bs-tooltip-border-radius: var(--bs-border-radius);--bs-tooltip-opacity: .9;--bs-tooltip-arrow-width: .8rem;--bs-tooltip-arrow-height: .4rem;z-index:var(--bs-tooltip-zindex);display:block;margin:var(--bs-tooltip-margin);font-family:var(--bs-font-sans-serif);font-style:normal;font-weight:400;line-height:1.5;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;white-space:normal;word-spacing:normal;line-break:auto;font-size:var(--bs-tooltip-font-size);word-wrap:break-word;opacity:0}.tooltip.show{opacity:var(--bs-tooltip-opacity)}.tooltip .tooltip-arrow{display:block;width:var(--bs-tooltip-arrow-width);height:var(--bs-tooltip-arrow-height)}.tooltip .tooltip-arrow:before{position:absolute;content:"";border-color:transparent;border-style:solid}.bs-tooltip-top .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^=top] .tooltip-arrow{bottom:calc(-1 * var(--bs-tooltip-arrow-height))}.bs-tooltip-top .tooltip-arrow:before,.bs-tooltip-auto[data-popper-placement^=top] .tooltip-arrow:before{top:-1px;border-width:var(--bs-tooltip-arrow-height) calc(var(--bs-tooltip-arrow-width) * .5) 0;border-top-color:var(--bs-tooltip-bg)}.bs-tooltip-end .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^=right] .tooltip-arrow{left:calc(-1 * var(--bs-tooltip-arrow-height));width:var(--bs-tooltip-arrow-height);height:var(--bs-tooltip-arrow-width)}.bs-tooltip-end .tooltip-arrow:before,.bs-tooltip-auto[data-popper-placement^=right] .tooltip-arrow:before{right:-1px;border-width:calc(var(--bs-tooltip-arrow-width) * .5) var(--bs-tooltip-arrow-height) calc(var(--bs-tooltip-arrow-width) * .5) 0;border-right-color:var(--bs-tooltip-bg)}.bs-tooltip-bottom .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^=bottom] .tooltip-arrow{top:calc(-1 * var(--bs-tooltip-arrow-height))}.bs-tooltip-bottom .tooltip-arrow:before,.bs-tooltip-auto[data-popper-placement^=bottom] .tooltip-arrow:before{bottom:-1px;border-width:0 calc(var(--bs-tooltip-arrow-width) * .5) var(--bs-tooltip-arrow-height);border-bottom-color:var(--bs-tooltip-bg)}.bs-tooltip-start .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^=left] .tooltip-arrow{right:calc(-1 * var(--bs-tooltip-arrow-height));width:var(--bs-tooltip-arrow-height);height:var(--bs-tooltip-arrow-width)}.bs-tooltip-start .tooltip-arrow:before,.bs-tooltip-auto[data-popper-placement^=left] .tooltip-arrow:before{left:-1px;border-width:calc(var(--bs-tooltip-arrow-width) * .5) 0 calc(var(--bs-tooltip-arrow-width) * .5) var(--bs-tooltip-arrow-height);border-left-color:var(--bs-tooltip-bg)}.tooltip-inner{max-width:var(--bs-tooltip-max-width);padding:var(--bs-tooltip-padding-y) var(--bs-tooltip-padding-x);color:var(--bs-tooltip-color);text-align:center;background-color:var(--bs-tooltip-bg);border-radius:var(--bs-tooltip-border-radius)}.popover{--bs-popover-zindex: 1070;--bs-popover-max-width: 276px;--bs-popover-font-size: .875rem;--bs-popover-bg: var(--bs-body-bg);--bs-popover-border-width: var(--bs-border-width);--bs-popover-border-color: var(--bs-border-color-translucent);--bs-popover-border-radius: var(--bs-border-radius-lg);--bs-popover-inner-border-radius: calc(var(--bs-border-radius-lg) - var(--bs-border-width));--bs-popover-box-shadow: var(--bs-box-shadow);--bs-popover-header-padding-x: 1rem;--bs-popover-header-padding-y: .5rem;--bs-popover-header-font-size: 1rem;--bs-popover-header-color: inherit;--bs-popover-header-bg: var(--bs-secondary-bg);--bs-popover-body-padding-x: 1rem;--bs-popover-body-padding-y: 1rem;--bs-popover-body-color: var(--bs-body-color);--bs-popover-arrow-width: 1rem;--bs-popover-arrow-height: .5rem;--bs-popover-arrow-border: var(--bs-popover-border-color);z-index:var(--bs-popover-zindex);display:block;max-width:var(--bs-popover-max-width);font-family:var(--bs-font-sans-serif);font-style:normal;font-weight:400;line-height:1.5;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;white-space:normal;word-spacing:normal;line-break:auto;font-size:var(--bs-popover-font-size);word-wrap:break-word;background-color:var(--bs-popover-bg);background-clip:padding-box;border:var(--bs-popover-border-width) solid var(--bs-popover-border-color);border-radius:var(--bs-popover-border-radius)}.popover .popover-arrow{display:block;width:var(--bs-popover-arrow-width);height:var(--bs-popover-arrow-height)}.popover .popover-arrow:before,.popover .popover-arrow:after{position:absolute;display:block;content:"";border-color:transparent;border-style:solid;border-width:0}.bs-popover-top>.popover-arrow,.bs-popover-auto[data-popper-placement^=top]>.popover-arrow{bottom:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width))}.bs-popover-top>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=top]>.popover-arrow:before,.bs-popover-top>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=top]>.popover-arrow:after{border-width:var(--bs-popover-arrow-height) calc(var(--bs-popover-arrow-width) * .5) 0}.bs-popover-top>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=top]>.popover-arrow:before{bottom:0;border-top-color:var(--bs-popover-arrow-border)}.bs-popover-top>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=top]>.popover-arrow:after{bottom:var(--bs-popover-border-width);border-top-color:var(--bs-popover-bg)}.bs-popover-end>.popover-arrow,.bs-popover-auto[data-popper-placement^=right]>.popover-arrow{left:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width));width:var(--bs-popover-arrow-height);height:var(--bs-popover-arrow-width)}.bs-popover-end>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=right]>.popover-arrow:before,.bs-popover-end>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=right]>.popover-arrow:after{border-width:calc(var(--bs-popover-arrow-width) * .5) var(--bs-popover-arrow-height) calc(var(--bs-popover-arrow-width) * .5) 0}.bs-popover-end>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=right]>.popover-arrow:before{left:0;border-right-color:var(--bs-popover-arrow-border)}.bs-popover-end>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=right]>.popover-arrow:after{left:var(--bs-popover-border-width);border-right-color:var(--bs-popover-bg)}.bs-popover-bottom>.popover-arrow,.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow{top:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width))}.bs-popover-bottom>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow:before,.bs-popover-bottom>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow:after{border-width:0 calc(var(--bs-popover-arrow-width) * .5) var(--bs-popover-arrow-height)}.bs-popover-bottom>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow:before{top:0;border-bottom-color:var(--bs-popover-arrow-border)}.bs-popover-bottom>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow:after{top:var(--bs-popover-border-width);border-bottom-color:var(--bs-popover-bg)}.bs-popover-bottom .popover-header:before,.bs-popover-auto[data-popper-placement^=bottom] .popover-header:before{position:absolute;top:0;left:50%;display:block;width:var(--bs-popover-arrow-width);margin-left:calc(-.5 * var(--bs-popover-arrow-width));content:"";border-bottom:var(--bs-popover-border-width) solid var(--bs-popover-header-bg)}.bs-popover-start>.popover-arrow,.bs-popover-auto[data-popper-placement^=left]>.popover-arrow{right:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width));width:var(--bs-popover-arrow-height);height:var(--bs-popover-arrow-width)}.bs-popover-start>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=left]>.popover-arrow:before,.bs-popover-start>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=left]>.popover-arrow:after{border-width:calc(var(--bs-popover-arrow-width) * .5) 0 calc(var(--bs-popover-arrow-width) * .5) var(--bs-popover-arrow-height)}.bs-popover-start>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=left]>.popover-arrow:before{right:0;border-left-color:var(--bs-popover-arrow-border)}.bs-popover-start>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=left]>.popover-arrow:after{right:var(--bs-popover-border-width);border-left-color:var(--bs-popover-bg)}.popover-header{padding:var(--bs-popover-header-padding-y) var(--bs-popover-header-padding-x);margin-bottom:0;font-size:var(--bs-popover-header-font-size);color:var(--bs-popover-header-color);background-color:var(--bs-popover-header-bg);border-bottom:var(--bs-popover-border-width) solid var(--bs-popover-border-color);border-top-left-radius:var(--bs-popover-inner-border-radius);border-top-right-radius:var(--bs-popover-inner-border-radius)}.popover-header:empty{display:none}.popover-body{padding:var(--bs-popover-body-padding-y) var(--bs-popover-body-padding-x);color:var(--bs-popover-body-color)}.carousel{position:relative}.carousel.pointer-event{touch-action:pan-y}.carousel-inner{position:relative;width:100%;overflow:hidden}.carousel-inner:after{display:block;clear:both;content:""}.carousel-item{position:relative;display:none;float:left;width:100%;margin-right:-100%;backface-visibility:hidden;transition:transform .6s ease-in-out}@media (prefers-reduced-motion: reduce){.carousel-item{transition:none}}.carousel-item.active,.carousel-item-next,.carousel-item-prev{display:block}.carousel-item-next:not(.carousel-item-start),.active.carousel-item-end{transform:translate(100%)}.carousel-item-prev:not(.carousel-item-end),.active.carousel-item-start{transform:translate(-100%)}.carousel-fade .carousel-item{opacity:0;transition-property:opacity;transform:none}.carousel-fade .carousel-item.active,.carousel-fade .carousel-item-next.carousel-item-start,.carousel-fade .carousel-item-prev.carousel-item-end{z-index:1;opacity:1}.carousel-fade .active.carousel-item-start,.carousel-fade .active.carousel-item-end{z-index:0;opacity:0;transition:opacity 0s .6s}@media (prefers-reduced-motion: reduce){.carousel-fade .active.carousel-item-start,.carousel-fade .active.carousel-item-end{transition:none}}.carousel-control-prev,.carousel-control-next{position:absolute;top:0;bottom:0;z-index:1;display:flex;align-items:center;justify-content:center;width:15%;padding:0;color:#fff;text-align:center;background:none;border:0;opacity:.5;transition:opacity .15s ease}@media (prefers-reduced-motion: reduce){.carousel-control-prev,.carousel-control-next{transition:none}}.carousel-control-prev:hover,.carousel-control-prev:focus,.carousel-control-next:hover,.carousel-control-next:focus{color:#fff;text-decoration:none;outline:0;opacity:.9}.carousel-control-prev{left:0}.carousel-control-next{right:0}.carousel-control-prev-icon,.carousel-control-next-icon{display:inline-block;width:2rem;height:2rem;background-repeat:no-repeat;background-position:50%;background-size:100% 100%}.carousel-control-prev-icon{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23fff'%3e%3cpath d='M11.354 1.646a.5.5 0 0 1 0 .708L5.707 8l5.647 5.646a.5.5 0 0 1-.708.708l-6-6a.5.5 0 0 1 0-.708l6-6a.5.5 0 0 1 .708 0z'/%3e%3c/svg%3e")}.carousel-control-next-icon{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23fff'%3e%3cpath d='M4.646 1.646a.5.5 0 0 1 .708 0l6 6a.5.5 0 0 1 0 .708l-6 6a.5.5 0 0 1-.708-.708L10.293 8 4.646 2.354a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e")}.carousel-indicators{position:absolute;right:0;bottom:0;left:0;z-index:2;display:flex;justify-content:center;padding:0;margin-right:15%;margin-bottom:1rem;margin-left:15%}.carousel-indicators [data-bs-target]{box-sizing:content-box;flex:0 1 auto;width:30px;height:3px;padding:0;margin-right:3px;margin-left:3px;text-indent:-999px;cursor:pointer;background-color:#fff;background-clip:padding-box;border:0;border-top:10px solid transparent;border-bottom:10px solid transparent;opacity:.5;transition:opacity .6s ease}@media (prefers-reduced-motion: reduce){.carousel-indicators [data-bs-target]{transition:none}}.carousel-indicators .active{opacity:1}.carousel-caption{position:absolute;right:15%;bottom:1.25rem;left:15%;padding-top:1.25rem;padding-bottom:1.25rem;color:#fff;text-align:center}.carousel-dark .carousel-control-prev-icon,.carousel-dark .carousel-control-next-icon{filter:invert(1) grayscale(100)}.carousel-dark .carousel-indicators [data-bs-target]{background-color:#000}.carousel-dark .carousel-caption{color:#000}[data-bs-theme=dark] .carousel .carousel-control-prev-icon,[data-bs-theme=dark] .carousel .carousel-control-next-icon,[data-bs-theme=dark].carousel .carousel-control-prev-icon,[data-bs-theme=dark].carousel .carousel-control-next-icon{filter:invert(1) grayscale(100)}[data-bs-theme=dark] .carousel .carousel-indicators [data-bs-target],[data-bs-theme=dark].carousel .carousel-indicators [data-bs-target]{background-color:#000}[data-bs-theme=dark] .carousel .carousel-caption,[data-bs-theme=dark].carousel .carousel-caption{color:#000}.spinner-grow,.spinner-border{display:inline-block;width:var(--bs-spinner-width);height:var(--bs-spinner-height);vertical-align:var(--bs-spinner-vertical-align);border-radius:50%;animation:var(--bs-spinner-animation-speed) linear infinite var(--bs-spinner-animation-name)}@keyframes spinner-border{to{transform:rotate(360deg)}}.spinner-border{--bs-spinner-width: 2rem;--bs-spinner-height: 2rem;--bs-spinner-vertical-align: -.125em;--bs-spinner-border-width: .25em;--bs-spinner-animation-speed: .75s;--bs-spinner-animation-name: spinner-border;border:var(--bs-spinner-border-width) solid currentcolor;border-right-color:transparent}.spinner-border-sm{--bs-spinner-width: 1rem;--bs-spinner-height: 1rem;--bs-spinner-border-width: .2em}@keyframes spinner-grow{0%{transform:scale(0)}50%{opacity:1;transform:none}}.spinner-grow{--bs-spinner-width: 2rem;--bs-spinner-height: 2rem;--bs-spinner-vertical-align: -.125em;--bs-spinner-animation-speed: .75s;--bs-spinner-animation-name: spinner-grow;background-color:currentcolor;opacity:0}.spinner-grow-sm{--bs-spinner-width: 1rem;--bs-spinner-height: 1rem}@media (prefers-reduced-motion: reduce){.spinner-border,.spinner-grow{--bs-spinner-animation-speed: 1.5s}}.offcanvas,.offcanvas-xxl,.offcanvas-xl,.offcanvas-lg,.offcanvas-md,.offcanvas-sm{--bs-offcanvas-zindex: 1045;--bs-offcanvas-width: 400px;--bs-offcanvas-height: 30vh;--bs-offcanvas-padding-x: 1rem;--bs-offcanvas-padding-y: 1rem;--bs-offcanvas-color: var(--bs-body-color);--bs-offcanvas-bg: var(--bs-body-bg);--bs-offcanvas-border-width: var(--bs-border-width);--bs-offcanvas-border-color: var(--bs-border-color-translucent);--bs-offcanvas-box-shadow: var(--bs-box-shadow-sm);--bs-offcanvas-transition: transform .3s ease-in-out;--bs-offcanvas-title-line-height: 1.5}@media (max-width: 575.98px){.offcanvas-sm{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:var(--bs-offcanvas-transition)}}@media (max-width: 575.98px) and (prefers-reduced-motion: reduce){.offcanvas-sm{transition:none}}@media (max-width: 575.98px){.offcanvas-sm.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(-100%)}.offcanvas-sm.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(100%)}.offcanvas-sm.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-sm.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-sm.showing,.offcanvas-sm.show:not(.hiding){transform:none}.offcanvas-sm.showing,.offcanvas-sm.hiding,.offcanvas-sm.show{visibility:visible}}@media (min-width: 576px){.offcanvas-sm{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent!important}.offcanvas-sm .offcanvas-header{display:none}.offcanvas-sm .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible;background-color:transparent!important}}@media (max-width: 767.98px){.offcanvas-md{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:var(--bs-offcanvas-transition)}}@media (max-width: 767.98px) and (prefers-reduced-motion: reduce){.offcanvas-md{transition:none}}@media (max-width: 767.98px){.offcanvas-md.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(-100%)}.offcanvas-md.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(100%)}.offcanvas-md.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-md.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-md.showing,.offcanvas-md.show:not(.hiding){transform:none}.offcanvas-md.showing,.offcanvas-md.hiding,.offcanvas-md.show{visibility:visible}}@media (min-width: 768px){.offcanvas-md{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent!important}.offcanvas-md .offcanvas-header{display:none}.offcanvas-md .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible;background-color:transparent!important}}@media (max-width: 991.98px){.offcanvas-lg{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:var(--bs-offcanvas-transition)}}@media (max-width: 991.98px) and (prefers-reduced-motion: reduce){.offcanvas-lg{transition:none}}@media (max-width: 991.98px){.offcanvas-lg.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(-100%)}.offcanvas-lg.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(100%)}.offcanvas-lg.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-lg.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-lg.showing,.offcanvas-lg.show:not(.hiding){transform:none}.offcanvas-lg.showing,.offcanvas-lg.hiding,.offcanvas-lg.show{visibility:visible}}@media (min-width: 992px){.offcanvas-lg{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent!important}.offcanvas-lg .offcanvas-header{display:none}.offcanvas-lg .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible;background-color:transparent!important}}@media (max-width: 1199.98px){.offcanvas-xl{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:var(--bs-offcanvas-transition)}}@media (max-width: 1199.98px) and (prefers-reduced-motion: reduce){.offcanvas-xl{transition:none}}@media (max-width: 1199.98px){.offcanvas-xl.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(-100%)}.offcanvas-xl.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(100%)}.offcanvas-xl.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-xl.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-xl.showing,.offcanvas-xl.show:not(.hiding){transform:none}.offcanvas-xl.showing,.offcanvas-xl.hiding,.offcanvas-xl.show{visibility:visible}}@media (min-width: 1200px){.offcanvas-xl{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent!important}.offcanvas-xl .offcanvas-header{display:none}.offcanvas-xl .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible;background-color:transparent!important}}@media (max-width: 1399.98px){.offcanvas-xxl{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:var(--bs-offcanvas-transition)}}@media (max-width: 1399.98px) and (prefers-reduced-motion: reduce){.offcanvas-xxl{transition:none}}@media (max-width: 1399.98px){.offcanvas-xxl.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(-100%)}.offcanvas-xxl.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(100%)}.offcanvas-xxl.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-xxl.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-xxl.showing,.offcanvas-xxl.show:not(.hiding){transform:none}.offcanvas-xxl.showing,.offcanvas-xxl.hiding,.offcanvas-xxl.show{visibility:visible}}@media (min-width: 1400px){.offcanvas-xxl{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent!important}.offcanvas-xxl .offcanvas-header{display:none}.offcanvas-xxl .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible;background-color:transparent!important}}.offcanvas{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:var(--bs-offcanvas-transition)}@media (prefers-reduced-motion: reduce){.offcanvas{transition:none}}.offcanvas.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(-100%)}.offcanvas.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(100%)}.offcanvas.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas.showing,.offcanvas.show:not(.hiding){transform:none}.offcanvas.showing,.offcanvas.hiding,.offcanvas.show{visibility:visible}.offcanvas-backdrop{position:fixed;top:0;left:0;z-index:1040;width:100vw;height:100vh;background-color:#000}.offcanvas-backdrop.fade{opacity:0}.offcanvas-backdrop.show{opacity:.5}.offcanvas-header{display:flex;align-items:center;justify-content:space-between;padding:var(--bs-offcanvas-padding-y) var(--bs-offcanvas-padding-x)}.offcanvas-header .btn-close{padding:calc(var(--bs-offcanvas-padding-y) * .5) calc(var(--bs-offcanvas-padding-x) * .5);margin-top:calc(-.5 * var(--bs-offcanvas-padding-y));margin-right:calc(-.5 * var(--bs-offcanvas-padding-x));margin-bottom:calc(-.5 * var(--bs-offcanvas-padding-y))}.offcanvas-title{margin-bottom:0;line-height:var(--bs-offcanvas-title-line-height)}.offcanvas-body{flex-grow:1;padding:var(--bs-offcanvas-padding-y) var(--bs-offcanvas-padding-x);overflow-y:auto}.placeholder{display:inline-block;min-height:1em;vertical-align:middle;cursor:wait;background-color:currentcolor;opacity:.5}.placeholder.btn:before{display:inline-block;content:""}.placeholder-xs{min-height:.6em}.placeholder-sm{min-height:.8em}.placeholder-lg{min-height:1.2em}.placeholder-glow .placeholder{animation:placeholder-glow 2s ease-in-out infinite}@keyframes placeholder-glow{50%{opacity:.2}}.placeholder-wave{mask-image:linear-gradient(130deg,#000 55%,#000c,#000 95%);mask-size:200% 100%;animation:placeholder-wave 2s linear infinite}@keyframes placeholder-wave{to{mask-position:-200% 0%}}.clearfix:after{display:block;clear:both;content:""}.text-bg-primary{color:#fff!important;background-color:RGBA(var(--bs-primary-rgb),var(--bs-bg-opacity, 1))!important}.text-bg-secondary{color:#fff!important;background-color:RGBA(var(--bs-secondary-rgb),var(--bs-bg-opacity, 1))!important}.text-bg-success{color:#fff!important;background-color:RGBA(var(--bs-success-rgb),var(--bs-bg-opacity, 1))!important}.text-bg-info{color:#000!important;background-color:RGBA(var(--bs-info-rgb),var(--bs-bg-opacity, 1))!important}.text-bg-warning{color:#000!important;background-color:RGBA(var(--bs-warning-rgb),var(--bs-bg-opacity, 1))!important}.text-bg-danger{color:#fff!important;background-color:RGBA(var(--bs-danger-rgb),var(--bs-bg-opacity, 1))!important}.text-bg-light{color:#000!important;background-color:RGBA(var(--bs-light-rgb),var(--bs-bg-opacity, 1))!important}.text-bg-dark{color:#fff!important;background-color:RGBA(var(--bs-dark-rgb),var(--bs-bg-opacity, 1))!important}.link-primary{color:RGBA(var(--bs-primary-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-primary-rgb),var(--bs-link-underline-opacity, 1))!important}.link-primary:hover,.link-primary:focus{color:RGBA(10,88,202,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(10,88,202,var(--bs-link-underline-opacity, 1))!important}.link-secondary{color:RGBA(var(--bs-secondary-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-secondary-rgb),var(--bs-link-underline-opacity, 1))!important}.link-secondary:hover,.link-secondary:focus{color:RGBA(86,94,100,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(86,94,100,var(--bs-link-underline-opacity, 1))!important}.link-success{color:RGBA(var(--bs-success-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-success-rgb),var(--bs-link-underline-opacity, 1))!important}.link-success:hover,.link-success:focus{color:RGBA(20,108,67,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(20,108,67,var(--bs-link-underline-opacity, 1))!important}.link-info{color:RGBA(var(--bs-info-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-info-rgb),var(--bs-link-underline-opacity, 1))!important}.link-info:hover,.link-info:focus{color:RGBA(61,213,243,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(61,213,243,var(--bs-link-underline-opacity, 1))!important}.link-warning{color:RGBA(var(--bs-warning-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-warning-rgb),var(--bs-link-underline-opacity, 1))!important}.link-warning:hover,.link-warning:focus{color:RGBA(255,205,57,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(255,205,57,var(--bs-link-underline-opacity, 1))!important}.link-danger{color:RGBA(var(--bs-danger-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-danger-rgb),var(--bs-link-underline-opacity, 1))!important}.link-danger:hover,.link-danger:focus{color:RGBA(176,42,55,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(176,42,55,var(--bs-link-underline-opacity, 1))!important}.link-light{color:RGBA(var(--bs-light-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-light-rgb),var(--bs-link-underline-opacity, 1))!important}.link-light:hover,.link-light:focus{color:RGBA(249,250,251,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(249,250,251,var(--bs-link-underline-opacity, 1))!important}.link-dark{color:RGBA(var(--bs-dark-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-dark-rgb),var(--bs-link-underline-opacity, 1))!important}.link-dark:hover,.link-dark:focus{color:RGBA(26,30,33,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(26,30,33,var(--bs-link-underline-opacity, 1))!important}.link-body-emphasis{color:RGBA(var(--bs-emphasis-color-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-emphasis-color-rgb),var(--bs-link-underline-opacity, 1))!important}.link-body-emphasis:hover,.link-body-emphasis:focus{color:RGBA(var(--bs-emphasis-color-rgb),var(--bs-link-opacity, .75))!important;text-decoration-color:RGBA(var(--bs-emphasis-color-rgb),var(--bs-link-underline-opacity, .75))!important}.focus-ring:focus{outline:0;box-shadow:var(--bs-focus-ring-x, 0) var(--bs-focus-ring-y, 0) var(--bs-focus-ring-blur, 0) var(--bs-focus-ring-width) var(--bs-focus-ring-color)}.icon-link{display:inline-flex;gap:.375rem;align-items:center;text-decoration-color:rgba(var(--bs-link-color-rgb),var(--bs-link-opacity, .5));text-underline-offset:.25em;backface-visibility:hidden}.icon-link>.bi{flex-shrink:0;width:1em;height:1em;fill:currentcolor;transition:.2s ease-in-out transform}@media (prefers-reduced-motion: reduce){.icon-link>.bi{transition:none}}.icon-link-hover:hover>.bi,.icon-link-hover:focus-visible>.bi{transform:var(--bs-icon-link-transform, translate3d(.25em, 0, 0))}.ratio{position:relative;width:100%}.ratio:before{display:block;padding-top:var(--bs-aspect-ratio);content:""}.ratio>*{position:absolute;top:0;left:0;width:100%;height:100%}.ratio-1x1{--bs-aspect-ratio: 100%}.ratio-4x3{--bs-aspect-ratio: 75%}.ratio-16x9{--bs-aspect-ratio: 56.25%}.ratio-21x9{--bs-aspect-ratio: 42.8571428571%}.fixed-top{position:fixed;top:0;right:0;left:0;z-index:1030}.fixed-bottom{position:fixed;right:0;bottom:0;left:0;z-index:1030}.sticky-top{position:sticky;top:0;z-index:1020}.sticky-bottom{position:sticky;bottom:0;z-index:1020}@media (min-width: 576px){.sticky-sm-top{position:sticky;top:0;z-index:1020}.sticky-sm-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 768px){.sticky-md-top{position:sticky;top:0;z-index:1020}.sticky-md-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 992px){.sticky-lg-top{position:sticky;top:0;z-index:1020}.sticky-lg-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 1200px){.sticky-xl-top{position:sticky;top:0;z-index:1020}.sticky-xl-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 1400px){.sticky-xxl-top{position:sticky;top:0;z-index:1020}.sticky-xxl-bottom{position:sticky;bottom:0;z-index:1020}}.hstack{display:flex;flex-direction:row;align-items:center;align-self:stretch}.vstack{display:flex;flex:1 1 auto;flex-direction:column;align-self:stretch}.visually-hidden,.visually-hidden-focusable:not(:focus):not(:focus-within){width:1px!important;height:1px!important;padding:0!important;margin:-1px!important;overflow:hidden!important;clip:rect(0,0,0,0)!important;white-space:nowrap!important;border:0!important}.visually-hidden:not(caption),.visually-hidden-focusable:not(:focus):not(:focus-within):not(caption){position:absolute!important}.stretched-link:after{position:absolute;inset:0;z-index:1;content:""}.text-truncate{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.vr{display:inline-block;align-self:stretch;width:var(--bs-border-width);min-height:1em;background-color:currentcolor;opacity:.25}.align-baseline{vertical-align:baseline!important}.align-top{vertical-align:top!important}.align-middle{vertical-align:middle!important}.align-bottom{vertical-align:bottom!important}.align-text-bottom{vertical-align:text-bottom!important}.align-text-top{vertical-align:text-top!important}.float-start{float:left!important}.float-end{float:right!important}.float-none{float:none!important}.object-fit-contain{object-fit:contain!important}.object-fit-cover{object-fit:cover!important}.object-fit-fill{object-fit:fill!important}.object-fit-scale{object-fit:scale-down!important}.object-fit-none{object-fit:none!important}.opacity-0{opacity:0!important}.opacity-25{opacity:.25!important}.opacity-50{opacity:.5!important}.opacity-75{opacity:.75!important}.opacity-100{opacity:1!important}.overflow-auto{overflow:auto!important}.overflow-hidden{overflow:hidden!important}.overflow-visible{overflow:visible!important}.overflow-scroll{overflow:scroll!important}.overflow-x-auto{overflow-x:auto!important}.overflow-x-hidden{overflow-x:hidden!important}.overflow-x-visible{overflow-x:visible!important}.overflow-x-scroll{overflow-x:scroll!important}.overflow-y-auto{overflow-y:auto!important}.overflow-y-hidden{overflow-y:hidden!important}.overflow-y-visible{overflow-y:visible!important}.overflow-y-scroll{overflow-y:scroll!important}.d-inline{display:inline!important}.d-inline-block{display:inline-block!important}.d-block{display:block!important}.d-grid{display:grid!important}.d-inline-grid{display:inline-grid!important}.d-table{display:table!important}.d-table-row{display:table-row!important}.d-table-cell{display:table-cell!important}.d-flex{display:flex!important}.d-inline-flex{display:inline-flex!important}.d-none{display:none!important}.shadow{box-shadow:var(--bs-box-shadow)!important}.shadow-sm{box-shadow:var(--bs-box-shadow-sm)!important}.shadow-lg{box-shadow:var(--bs-box-shadow-lg)!important}.shadow-none{box-shadow:none!important}.focus-ring-primary{--bs-focus-ring-color: rgba(var(--bs-primary-rgb), var(--bs-focus-ring-opacity))}.focus-ring-secondary{--bs-focus-ring-color: rgba(var(--bs-secondary-rgb), var(--bs-focus-ring-opacity))}.focus-ring-success{--bs-focus-ring-color: rgba(var(--bs-success-rgb), var(--bs-focus-ring-opacity))}.focus-ring-info{--bs-focus-ring-color: rgba(var(--bs-info-rgb), var(--bs-focus-ring-opacity))}.focus-ring-warning{--bs-focus-ring-color: rgba(var(--bs-warning-rgb), var(--bs-focus-ring-opacity))}.focus-ring-danger{--bs-focus-ring-color: rgba(var(--bs-danger-rgb), var(--bs-focus-ring-opacity))}.focus-ring-light{--bs-focus-ring-color: rgba(var(--bs-light-rgb), var(--bs-focus-ring-opacity))}.focus-ring-dark{--bs-focus-ring-color: rgba(var(--bs-dark-rgb), var(--bs-focus-ring-opacity))}.position-static{position:static!important}.position-relative{position:relative!important}.position-absolute{position:absolute!important}.position-fixed{position:fixed!important}.position-sticky{position:sticky!important}.top-0{top:0!important}.top-50{top:50%!important}.top-100{top:100%!important}.bottom-0{bottom:0!important}.bottom-50{bottom:50%!important}.bottom-100{bottom:100%!important}.start-0{left:0!important}.start-50{left:50%!important}.start-100{left:100%!important}.end-0{right:0!important}.end-50{right:50%!important}.end-100{right:100%!important}.translate-middle{transform:translate(-50%,-50%)!important}.translate-middle-x{transform:translate(-50%)!important}.translate-middle-y{transform:translateY(-50%)!important}.border{border:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color)!important}.border-0{border:0!important}.border-top{border-top:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color)!important}.border-top-0{border-top:0!important}.border-end{border-right:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color)!important}.border-end-0{border-right:0!important}.border-bottom{border-bottom:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color)!important}.border-bottom-0{border-bottom:0!important}.border-start{border-left:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color)!important}.border-start-0{border-left:0!important}.border-primary{--bs-border-opacity: 1;border-color:rgba(var(--bs-primary-rgb),var(--bs-border-opacity))!important}.border-secondary{--bs-border-opacity: 1;border-color:rgba(var(--bs-secondary-rgb),var(--bs-border-opacity))!important}.border-success{--bs-border-opacity: 1;border-color:rgba(var(--bs-success-rgb),var(--bs-border-opacity))!important}.border-info{--bs-border-opacity: 1;border-color:rgba(var(--bs-info-rgb),var(--bs-border-opacity))!important}.border-warning{--bs-border-opacity: 1;border-color:rgba(var(--bs-warning-rgb),var(--bs-border-opacity))!important}.border-danger{--bs-border-opacity: 1;border-color:rgba(var(--bs-danger-rgb),var(--bs-border-opacity))!important}.border-light{--bs-border-opacity: 1;border-color:rgba(var(--bs-light-rgb),var(--bs-border-opacity))!important}.border-dark{--bs-border-opacity: 1;border-color:rgba(var(--bs-dark-rgb),var(--bs-border-opacity))!important}.border-black{--bs-border-opacity: 1;border-color:rgba(var(--bs-black-rgb),var(--bs-border-opacity))!important}.border-white{--bs-border-opacity: 1;border-color:rgba(var(--bs-white-rgb),var(--bs-border-opacity))!important}.border-primary-subtle{border-color:var(--bs-primary-border-subtle)!important}.border-secondary-subtle{border-color:var(--bs-secondary-border-subtle)!important}.border-success-subtle{border-color:var(--bs-success-border-subtle)!important}.border-info-subtle{border-color:var(--bs-info-border-subtle)!important}.border-warning-subtle{border-color:var(--bs-warning-border-subtle)!important}.border-danger-subtle{border-color:var(--bs-danger-border-subtle)!important}.border-light-subtle{border-color:var(--bs-light-border-subtle)!important}.border-dark-subtle{border-color:var(--bs-dark-border-subtle)!important}.border-1{border-width:1px!important}.border-2{border-width:2px!important}.border-3{border-width:3px!important}.border-4{border-width:4px!important}.border-5{border-width:5px!important}.border-opacity-10{--bs-border-opacity: .1}.border-opacity-25{--bs-border-opacity: .25}.border-opacity-50{--bs-border-opacity: .5}.border-opacity-75{--bs-border-opacity: .75}.border-opacity-100{--bs-border-opacity: 1}.w-25{width:25%!important}.w-50{width:50%!important}.w-75{width:75%!important}.w-100{width:100%!important}.w-auto{width:auto!important}.mw-100{max-width:100%!important}.vw-100{width:100vw!important}.min-vw-100{min-width:100vw!important}.h-25{height:25%!important}.h-50{height:50%!important}.h-75{height:75%!important}.h-100{height:100%!important}.h-auto{height:auto!important}.mh-100{max-height:100%!important}.vh-100{height:100vh!important}.min-vh-100{min-height:100vh!important}.flex-fill{flex:1 1 auto!important}.flex-row{flex-direction:row!important}.flex-column{flex-direction:column!important}.flex-row-reverse{flex-direction:row-reverse!important}.flex-column-reverse{flex-direction:column-reverse!important}.flex-grow-0{flex-grow:0!important}.flex-grow-1{flex-grow:1!important}.flex-shrink-0{flex-shrink:0!important}.flex-shrink-1{flex-shrink:1!important}.flex-wrap{flex-wrap:wrap!important}.flex-nowrap{flex-wrap:nowrap!important}.flex-wrap-reverse{flex-wrap:wrap-reverse!important}.justify-content-start{justify-content:flex-start!important}.justify-content-end{justify-content:flex-end!important}.justify-content-center{justify-content:center!important}.justify-content-between{justify-content:space-between!important}.justify-content-around{justify-content:space-around!important}.justify-content-evenly{justify-content:space-evenly!important}.align-items-start{align-items:flex-start!important}.align-items-end{align-items:flex-end!important}.align-items-center{align-items:center!important}.align-items-baseline{align-items:baseline!important}.align-items-stretch{align-items:stretch!important}.align-content-start{align-content:flex-start!important}.align-content-end{align-content:flex-end!important}.align-content-center{align-content:center!important}.align-content-between{align-content:space-between!important}.align-content-around{align-content:space-around!important}.align-content-stretch{align-content:stretch!important}.align-self-auto{align-self:auto!important}.align-self-start{align-self:flex-start!important}.align-self-end{align-self:flex-end!important}.align-self-center{align-self:center!important}.align-self-baseline{align-self:baseline!important}.align-self-stretch{align-self:stretch!important}.order-first{order:-1!important}.order-0{order:0!important}.order-1{order:1!important}.order-2{order:2!important}.order-3{order:3!important}.order-4{order:4!important}.order-5{order:5!important}.order-last{order:6!important}.m-0{margin:0!important}.m-1{margin:.25rem!important}.m-2{margin:.5rem!important}.m-3{margin:1rem!important}.m-4{margin:1.5rem!important}.m-5{margin:3rem!important}.m-auto{margin:auto!important}.mx-0{margin-right:0!important;margin-left:0!important}.mx-1{margin-right:.25rem!important;margin-left:.25rem!important}.mx-2{margin-right:.5rem!important;margin-left:.5rem!important}.mx-3{margin-right:1rem!important;margin-left:1rem!important}.mx-4{margin-right:1.5rem!important;margin-left:1.5rem!important}.mx-5{margin-right:3rem!important;margin-left:3rem!important}.mx-auto{margin-right:auto!important;margin-left:auto!important}.my-0{margin-top:0!important;margin-bottom:0!important}.my-1{margin-top:.25rem!important;margin-bottom:.25rem!important}.my-2{margin-top:.5rem!important;margin-bottom:.5rem!important}.my-3{margin-top:1rem!important;margin-bottom:1rem!important}.my-4{margin-top:1.5rem!important;margin-bottom:1.5rem!important}.my-5{margin-top:3rem!important;margin-bottom:3rem!important}.my-auto{margin-top:auto!important;margin-bottom:auto!important}.mt-0{margin-top:0!important}.mt-1{margin-top:.25rem!important}.mt-2{margin-top:.5rem!important}.mt-3{margin-top:1rem!important}.mt-4{margin-top:1.5rem!important}.mt-5{margin-top:3rem!important}.mt-auto{margin-top:auto!important}.me-0{margin-right:0!important}.me-1{margin-right:.25rem!important}.me-2{margin-right:.5rem!important}.me-3{margin-right:1rem!important}.me-4{margin-right:1.5rem!important}.me-5{margin-right:3rem!important}.me-auto{margin-right:auto!important}.mb-0{margin-bottom:0!important}.mb-1{margin-bottom:.25rem!important}.mb-2{margin-bottom:.5rem!important}.mb-3{margin-bottom:1rem!important}.mb-4{margin-bottom:1.5rem!important}.mb-5{margin-bottom:3rem!important}.mb-auto{margin-bottom:auto!important}.ms-0{margin-left:0!important}.ms-1{margin-left:.25rem!important}.ms-2{margin-left:.5rem!important}.ms-3{margin-left:1rem!important}.ms-4{margin-left:1.5rem!important}.ms-5{margin-left:3rem!important}.ms-auto{margin-left:auto!important}.p-0{padding:0!important}.p-1{padding:.25rem!important}.p-2{padding:.5rem!important}.p-3{padding:1rem!important}.p-4{padding:1.5rem!important}.p-5{padding:3rem!important}.px-0{padding-right:0!important;padding-left:0!important}.px-1{padding-right:.25rem!important;padding-left:.25rem!important}.px-2{padding-right:.5rem!important;padding-left:.5rem!important}.px-3{padding-right:1rem!important;padding-left:1rem!important}.px-4{padding-right:1.5rem!important;padding-left:1.5rem!important}.px-5{padding-right:3rem!important;padding-left:3rem!important}.py-0{padding-top:0!important;padding-bottom:0!important}.py-1{padding-top:.25rem!important;padding-bottom:.25rem!important}.py-2{padding-top:.5rem!important;padding-bottom:.5rem!important}.py-3{padding-top:1rem!important;padding-bottom:1rem!important}.py-4{padding-top:1.5rem!important;padding-bottom:1.5rem!important}.py-5{padding-top:3rem!important;padding-bottom:3rem!important}.pt-0{padding-top:0!important}.pt-1{padding-top:.25rem!important}.pt-2{padding-top:.5rem!important}.pt-3{padding-top:1rem!important}.pt-4{padding-top:1.5rem!important}.pt-5{padding-top:3rem!important}.pe-0{padding-right:0!important}.pe-1{padding-right:.25rem!important}.pe-2{padding-right:.5rem!important}.pe-3{padding-right:1rem!important}.pe-4{padding-right:1.5rem!important}.pe-5{padding-right:3rem!important}.pb-0{padding-bottom:0!important}.pb-1{padding-bottom:.25rem!important}.pb-2{padding-bottom:.5rem!important}.pb-3{padding-bottom:1rem!important}.pb-4{padding-bottom:1.5rem!important}.pb-5{padding-bottom:3rem!important}.ps-0{padding-left:0!important}.ps-1{padding-left:.25rem!important}.ps-2{padding-left:.5rem!important}.ps-3{padding-left:1rem!important}.ps-4{padding-left:1.5rem!important}.ps-5{padding-left:3rem!important}.gap-0{gap:0!important}.gap-1{gap:.25rem!important}.gap-2{gap:.5rem!important}.gap-3{gap:1rem!important}.gap-4{gap:1.5rem!important}.gap-5{gap:3rem!important}.row-gap-0{row-gap:0!important}.row-gap-1{row-gap:.25rem!important}.row-gap-2{row-gap:.5rem!important}.row-gap-3{row-gap:1rem!important}.row-gap-4{row-gap:1.5rem!important}.row-gap-5{row-gap:3rem!important}.column-gap-0{column-gap:0!important}.column-gap-1{column-gap:.25rem!important}.column-gap-2{column-gap:.5rem!important}.column-gap-3{column-gap:1rem!important}.column-gap-4{column-gap:1.5rem!important}.column-gap-5{column-gap:3rem!important}.font-monospace{font-family:var(--bs-font-monospace)!important}.fs-1{font-size:calc(1.375rem + 1.5vw)!important}.fs-2{font-size:calc(1.325rem + .9vw)!important}.fs-3{font-size:calc(1.3rem + .6vw)!important}.fs-4{font-size:calc(1.275rem + .3vw)!important}.fs-5{font-size:1.25rem!important}.fs-6{font-size:1rem!important}.fst-italic{font-style:italic!important}.fst-normal{font-style:normal!important}.fw-lighter{font-weight:lighter!important}.fw-light{font-weight:300!important}.fw-normal{font-weight:400!important}.fw-medium{font-weight:500!important}.fw-semibold{font-weight:600!important}.fw-bold{font-weight:700!important}.fw-bolder{font-weight:bolder!important}.lh-1{line-height:1!important}.lh-sm{line-height:1.25!important}.lh-base{line-height:1.5!important}.lh-lg{line-height:2!important}.text-start{text-align:left!important}.text-end{text-align:right!important}.text-center{text-align:center!important}.text-decoration-none{text-decoration:none!important}.text-decoration-underline{text-decoration:underline!important}.text-decoration-line-through{text-decoration:line-through!important}.text-lowercase{text-transform:lowercase!important}.text-uppercase{text-transform:uppercase!important}.text-capitalize{text-transform:capitalize!important}.text-wrap{white-space:normal!important}.text-nowrap{white-space:nowrap!important}.text-break{word-wrap:break-word!important;word-break:break-word!important}.text-primary{--bs-text-opacity: 1;color:rgba(var(--bs-primary-rgb),var(--bs-text-opacity))!important}.text-secondary{--bs-text-opacity: 1;color:rgba(var(--bs-secondary-rgb),var(--bs-text-opacity))!important}.text-success{--bs-text-opacity: 1;color:rgba(var(--bs-success-rgb),var(--bs-text-opacity))!important}.text-info{--bs-text-opacity: 1;color:rgba(var(--bs-info-rgb),var(--bs-text-opacity))!important}.text-warning{--bs-text-opacity: 1;color:rgba(var(--bs-warning-rgb),var(--bs-text-opacity))!important}.text-danger{--bs-text-opacity: 1;color:rgba(var(--bs-danger-rgb),var(--bs-text-opacity))!important}.text-light{--bs-text-opacity: 1;color:rgba(var(--bs-light-rgb),var(--bs-text-opacity))!important}.text-dark{--bs-text-opacity: 1;color:rgba(var(--bs-dark-rgb),var(--bs-text-opacity))!important}.text-black{--bs-text-opacity: 1;color:rgba(var(--bs-black-rgb),var(--bs-text-opacity))!important}.text-white{--bs-text-opacity: 1;color:rgba(var(--bs-white-rgb),var(--bs-text-opacity))!important}.text-body{--bs-text-opacity: 1;color:rgba(var(--bs-body-color-rgb),var(--bs-text-opacity))!important}.text-muted{--bs-text-opacity: 1;color:var(--bs-secondary-color)!important}.text-black-50{--bs-text-opacity: 1;color:#00000080!important}.text-white-50{--bs-text-opacity: 1;color:#ffffff80!important}.text-body-secondary{--bs-text-opacity: 1;color:var(--bs-secondary-color)!important}.text-body-tertiary{--bs-text-opacity: 1;color:var(--bs-tertiary-color)!important}.text-body-emphasis{--bs-text-opacity: 1;color:var(--bs-emphasis-color)!important}.text-reset{--bs-text-opacity: 1;color:inherit!important}.text-opacity-25{--bs-text-opacity: .25}.text-opacity-50{--bs-text-opacity: .5}.text-opacity-75{--bs-text-opacity: .75}.text-opacity-100{--bs-text-opacity: 1}.text-primary-emphasis{color:var(--bs-primary-text-emphasis)!important}.text-secondary-emphasis{color:var(--bs-secondary-text-emphasis)!important}.text-success-emphasis{color:var(--bs-success-text-emphasis)!important}.text-info-emphasis{color:var(--bs-info-text-emphasis)!important}.text-warning-emphasis{color:var(--bs-warning-text-emphasis)!important}.text-danger-emphasis{color:var(--bs-danger-text-emphasis)!important}.text-light-emphasis{color:var(--bs-light-text-emphasis)!important}.text-dark-emphasis{color:var(--bs-dark-text-emphasis)!important}.link-opacity-10,.link-opacity-10-hover:hover{--bs-link-opacity: .1}.link-opacity-25,.link-opacity-25-hover:hover{--bs-link-opacity: .25}.link-opacity-50,.link-opacity-50-hover:hover{--bs-link-opacity: .5}.link-opacity-75,.link-opacity-75-hover:hover{--bs-link-opacity: .75}.link-opacity-100,.link-opacity-100-hover:hover{--bs-link-opacity: 1}.link-offset-1,.link-offset-1-hover:hover{text-underline-offset:.125em!important}.link-offset-2,.link-offset-2-hover:hover{text-underline-offset:.25em!important}.link-offset-3,.link-offset-3-hover:hover{text-underline-offset:.375em!important}.link-underline-primary{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-primary-rgb),var(--bs-link-underline-opacity))!important}.link-underline-secondary{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-secondary-rgb),var(--bs-link-underline-opacity))!important}.link-underline-success{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-success-rgb),var(--bs-link-underline-opacity))!important}.link-underline-info{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-info-rgb),var(--bs-link-underline-opacity))!important}.link-underline-warning{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-warning-rgb),var(--bs-link-underline-opacity))!important}.link-underline-danger{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-danger-rgb),var(--bs-link-underline-opacity))!important}.link-underline-light{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-light-rgb),var(--bs-link-underline-opacity))!important}.link-underline-dark{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-dark-rgb),var(--bs-link-underline-opacity))!important}.link-underline{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-link-color-rgb),var(--bs-link-underline-opacity, 1))!important}.link-underline-opacity-0,.link-underline-opacity-0-hover:hover{--bs-link-underline-opacity: 0}.link-underline-opacity-10,.link-underline-opacity-10-hover:hover{--bs-link-underline-opacity: .1}.link-underline-opacity-25,.link-underline-opacity-25-hover:hover{--bs-link-underline-opacity: .25}.link-underline-opacity-50,.link-underline-opacity-50-hover:hover{--bs-link-underline-opacity: .5}.link-underline-opacity-75,.link-underline-opacity-75-hover:hover{--bs-link-underline-opacity: .75}.link-underline-opacity-100,.link-underline-opacity-100-hover:hover{--bs-link-underline-opacity: 1}.bg-primary{--bs-bg-opacity: 1;background-color:rgba(var(--bs-primary-rgb),var(--bs-bg-opacity))!important}.bg-secondary{--bs-bg-opacity: 1;background-color:rgba(var(--bs-secondary-rgb),var(--bs-bg-opacity))!important}.bg-success{--bs-bg-opacity: 1;background-color:rgba(var(--bs-success-rgb),var(--bs-bg-opacity))!important}.bg-info{--bs-bg-opacity: 1;background-color:rgba(var(--bs-info-rgb),var(--bs-bg-opacity))!important}.bg-warning{--bs-bg-opacity: 1;background-color:rgba(var(--bs-warning-rgb),var(--bs-bg-opacity))!important}.bg-danger{--bs-bg-opacity: 1;background-color:rgba(var(--bs-danger-rgb),var(--bs-bg-opacity))!important}.bg-light{--bs-bg-opacity: 1;background-color:rgba(var(--bs-light-rgb),var(--bs-bg-opacity))!important}.bg-dark{--bs-bg-opacity: 1;background-color:rgba(var(--bs-dark-rgb),var(--bs-bg-opacity))!important}.bg-black{--bs-bg-opacity: 1;background-color:rgba(var(--bs-black-rgb),var(--bs-bg-opacity))!important}.bg-white{--bs-bg-opacity: 1;background-color:rgba(var(--bs-white-rgb),var(--bs-bg-opacity))!important}.bg-body{--bs-bg-opacity: 1;background-color:rgba(var(--bs-body-bg-rgb),var(--bs-bg-opacity))!important}.bg-transparent{--bs-bg-opacity: 1;background-color:transparent!important}.bg-body-secondary{--bs-bg-opacity: 1;background-color:rgba(var(--bs-secondary-bg-rgb),var(--bs-bg-opacity))!important}.bg-body-tertiary{--bs-bg-opacity: 1;background-color:rgba(var(--bs-tertiary-bg-rgb),var(--bs-bg-opacity))!important}.bg-opacity-10{--bs-bg-opacity: .1}.bg-opacity-25{--bs-bg-opacity: .25}.bg-opacity-50{--bs-bg-opacity: .5}.bg-opacity-75{--bs-bg-opacity: .75}.bg-opacity-100{--bs-bg-opacity: 1}.bg-primary-subtle{background-color:var(--bs-primary-bg-subtle)!important}.bg-secondary-subtle{background-color:var(--bs-secondary-bg-subtle)!important}.bg-success-subtle{background-color:var(--bs-success-bg-subtle)!important}.bg-info-subtle{background-color:var(--bs-info-bg-subtle)!important}.bg-warning-subtle{background-color:var(--bs-warning-bg-subtle)!important}.bg-danger-subtle{background-color:var(--bs-danger-bg-subtle)!important}.bg-light-subtle{background-color:var(--bs-light-bg-subtle)!important}.bg-dark-subtle{background-color:var(--bs-dark-bg-subtle)!important}.bg-gradient{background-image:var(--bs-gradient)!important}.user-select-all{user-select:all!important}.user-select-auto{user-select:auto!important}.user-select-none{user-select:none!important}.pe-none{pointer-events:none!important}.pe-auto{pointer-events:auto!important}.rounded{border-radius:var(--bs-border-radius)!important}.rounded-0{border-radius:0!important}.rounded-1{border-radius:var(--bs-border-radius-sm)!important}.rounded-2{border-radius:var(--bs-border-radius)!important}.rounded-3{border-radius:var(--bs-border-radius-lg)!important}.rounded-4{border-radius:var(--bs-border-radius-xl)!important}.rounded-5{border-radius:var(--bs-border-radius-xxl)!important}.rounded-circle{border-radius:50%!important}.rounded-pill{border-radius:var(--bs-border-radius-pill)!important}.rounded-top{border-top-left-radius:var(--bs-border-radius)!important;border-top-right-radius:var(--bs-border-radius)!important}.rounded-top-0{border-top-left-radius:0!important;border-top-right-radius:0!important}.rounded-top-1{border-top-left-radius:var(--bs-border-radius-sm)!important;border-top-right-radius:var(--bs-border-radius-sm)!important}.rounded-top-2{border-top-left-radius:var(--bs-border-radius)!important;border-top-right-radius:var(--bs-border-radius)!important}.rounded-top-3{border-top-left-radius:var(--bs-border-radius-lg)!important;border-top-right-radius:var(--bs-border-radius-lg)!important}.rounded-top-4{border-top-left-radius:var(--bs-border-radius-xl)!important;border-top-right-radius:var(--bs-border-radius-xl)!important}.rounded-top-5{border-top-left-radius:var(--bs-border-radius-xxl)!important;border-top-right-radius:var(--bs-border-radius-xxl)!important}.rounded-top-circle{border-top-left-radius:50%!important;border-top-right-radius:50%!important}.rounded-top-pill{border-top-left-radius:var(--bs-border-radius-pill)!important;border-top-right-radius:var(--bs-border-radius-pill)!important}.rounded-end{border-top-right-radius:var(--bs-border-radius)!important;border-bottom-right-radius:var(--bs-border-radius)!important}.rounded-end-0{border-top-right-radius:0!important;border-bottom-right-radius:0!important}.rounded-end-1{border-top-right-radius:var(--bs-border-radius-sm)!important;border-bottom-right-radius:var(--bs-border-radius-sm)!important}.rounded-end-2{border-top-right-radius:var(--bs-border-radius)!important;border-bottom-right-radius:var(--bs-border-radius)!important}.rounded-end-3{border-top-right-radius:var(--bs-border-radius-lg)!important;border-bottom-right-radius:var(--bs-border-radius-lg)!important}.rounded-end-4{border-top-right-radius:var(--bs-border-radius-xl)!important;border-bottom-right-radius:var(--bs-border-radius-xl)!important}.rounded-end-5{border-top-right-radius:var(--bs-border-radius-xxl)!important;border-bottom-right-radius:var(--bs-border-radius-xxl)!important}.rounded-end-circle{border-top-right-radius:50%!important;border-bottom-right-radius:50%!important}.rounded-end-pill{border-top-right-radius:var(--bs-border-radius-pill)!important;border-bottom-right-radius:var(--bs-border-radius-pill)!important}.rounded-bottom{border-bottom-right-radius:var(--bs-border-radius)!important;border-bottom-left-radius:var(--bs-border-radius)!important}.rounded-bottom-0{border-bottom-right-radius:0!important;border-bottom-left-radius:0!important}.rounded-bottom-1{border-bottom-right-radius:var(--bs-border-radius-sm)!important;border-bottom-left-radius:var(--bs-border-radius-sm)!important}.rounded-bottom-2{border-bottom-right-radius:var(--bs-border-radius)!important;border-bottom-left-radius:var(--bs-border-radius)!important}.rounded-bottom-3{border-bottom-right-radius:var(--bs-border-radius-lg)!important;border-bottom-left-radius:var(--bs-border-radius-lg)!important}.rounded-bottom-4{border-bottom-right-radius:var(--bs-border-radius-xl)!important;border-bottom-left-radius:var(--bs-border-radius-xl)!important}.rounded-bottom-5{border-bottom-right-radius:var(--bs-border-radius-xxl)!important;border-bottom-left-radius:var(--bs-border-radius-xxl)!important}.rounded-bottom-circle{border-bottom-right-radius:50%!important;border-bottom-left-radius:50%!important}.rounded-bottom-pill{border-bottom-right-radius:var(--bs-border-radius-pill)!important;border-bottom-left-radius:var(--bs-border-radius-pill)!important}.rounded-start{border-bottom-left-radius:var(--bs-border-radius)!important;border-top-left-radius:var(--bs-border-radius)!important}.rounded-start-0{border-bottom-left-radius:0!important;border-top-left-radius:0!important}.rounded-start-1{border-bottom-left-radius:var(--bs-border-radius-sm)!important;border-top-left-radius:var(--bs-border-radius-sm)!important}.rounded-start-2{border-bottom-left-radius:var(--bs-border-radius)!important;border-top-left-radius:var(--bs-border-radius)!important}.rounded-start-3{border-bottom-left-radius:var(--bs-border-radius-lg)!important;border-top-left-radius:var(--bs-border-radius-lg)!important}.rounded-start-4{border-bottom-left-radius:var(--bs-border-radius-xl)!important;border-top-left-radius:var(--bs-border-radius-xl)!important}.rounded-start-5{border-bottom-left-radius:var(--bs-border-radius-xxl)!important;border-top-left-radius:var(--bs-border-radius-xxl)!important}.rounded-start-circle{border-bottom-left-radius:50%!important;border-top-left-radius:50%!important}.rounded-start-pill{border-bottom-left-radius:var(--bs-border-radius-pill)!important;border-top-left-radius:var(--bs-border-radius-pill)!important}.visible{visibility:visible!important}.invisible{visibility:hidden!important}.z-n1{z-index:-1!important}.z-0{z-index:0!important}.z-1{z-index:1!important}.z-2{z-index:2!important}.z-3{z-index:3!important}@media (min-width: 576px){.float-sm-start{float:left!important}.float-sm-end{float:right!important}.float-sm-none{float:none!important}.object-fit-sm-contain{object-fit:contain!important}.object-fit-sm-cover{object-fit:cover!important}.object-fit-sm-fill{object-fit:fill!important}.object-fit-sm-scale{object-fit:scale-down!important}.object-fit-sm-none{object-fit:none!important}.d-sm-inline{display:inline!important}.d-sm-inline-block{display:inline-block!important}.d-sm-block{display:block!important}.d-sm-grid{display:grid!important}.d-sm-inline-grid{display:inline-grid!important}.d-sm-table{display:table!important}.d-sm-table-row{display:table-row!important}.d-sm-table-cell{display:table-cell!important}.d-sm-flex{display:flex!important}.d-sm-inline-flex{display:inline-flex!important}.d-sm-none{display:none!important}.flex-sm-fill{flex:1 1 auto!important}.flex-sm-row{flex-direction:row!important}.flex-sm-column{flex-direction:column!important}.flex-sm-row-reverse{flex-direction:row-reverse!important}.flex-sm-column-reverse{flex-direction:column-reverse!important}.flex-sm-grow-0{flex-grow:0!important}.flex-sm-grow-1{flex-grow:1!important}.flex-sm-shrink-0{flex-shrink:0!important}.flex-sm-shrink-1{flex-shrink:1!important}.flex-sm-wrap{flex-wrap:wrap!important}.flex-sm-nowrap{flex-wrap:nowrap!important}.flex-sm-wrap-reverse{flex-wrap:wrap-reverse!important}.justify-content-sm-start{justify-content:flex-start!important}.justify-content-sm-end{justify-content:flex-end!important}.justify-content-sm-center{justify-content:center!important}.justify-content-sm-between{justify-content:space-between!important}.justify-content-sm-around{justify-content:space-around!important}.justify-content-sm-evenly{justify-content:space-evenly!important}.align-items-sm-start{align-items:flex-start!important}.align-items-sm-end{align-items:flex-end!important}.align-items-sm-center{align-items:center!important}.align-items-sm-baseline{align-items:baseline!important}.align-items-sm-stretch{align-items:stretch!important}.align-content-sm-start{align-content:flex-start!important}.align-content-sm-end{align-content:flex-end!important}.align-content-sm-center{align-content:center!important}.align-content-sm-between{align-content:space-between!important}.align-content-sm-around{align-content:space-around!important}.align-content-sm-stretch{align-content:stretch!important}.align-self-sm-auto{align-self:auto!important}.align-self-sm-start{align-self:flex-start!important}.align-self-sm-end{align-self:flex-end!important}.align-self-sm-center{align-self:center!important}.align-self-sm-baseline{align-self:baseline!important}.align-self-sm-stretch{align-self:stretch!important}.order-sm-first{order:-1!important}.order-sm-0{order:0!important}.order-sm-1{order:1!important}.order-sm-2{order:2!important}.order-sm-3{order:3!important}.order-sm-4{order:4!important}.order-sm-5{order:5!important}.order-sm-last{order:6!important}.m-sm-0{margin:0!important}.m-sm-1{margin:.25rem!important}.m-sm-2{margin:.5rem!important}.m-sm-3{margin:1rem!important}.m-sm-4{margin:1.5rem!important}.m-sm-5{margin:3rem!important}.m-sm-auto{margin:auto!important}.mx-sm-0{margin-right:0!important;margin-left:0!important}.mx-sm-1{margin-right:.25rem!important;margin-left:.25rem!important}.mx-sm-2{margin-right:.5rem!important;margin-left:.5rem!important}.mx-sm-3{margin-right:1rem!important;margin-left:1rem!important}.mx-sm-4{margin-right:1.5rem!important;margin-left:1.5rem!important}.mx-sm-5{margin-right:3rem!important;margin-left:3rem!important}.mx-sm-auto{margin-right:auto!important;margin-left:auto!important}.my-sm-0{margin-top:0!important;margin-bottom:0!important}.my-sm-1{margin-top:.25rem!important;margin-bottom:.25rem!important}.my-sm-2{margin-top:.5rem!important;margin-bottom:.5rem!important}.my-sm-3{margin-top:1rem!important;margin-bottom:1rem!important}.my-sm-4{margin-top:1.5rem!important;margin-bottom:1.5rem!important}.my-sm-5{margin-top:3rem!important;margin-bottom:3rem!important}.my-sm-auto{margin-top:auto!important;margin-bottom:auto!important}.mt-sm-0{margin-top:0!important}.mt-sm-1{margin-top:.25rem!important}.mt-sm-2{margin-top:.5rem!important}.mt-sm-3{margin-top:1rem!important}.mt-sm-4{margin-top:1.5rem!important}.mt-sm-5{margin-top:3rem!important}.mt-sm-auto{margin-top:auto!important}.me-sm-0{margin-right:0!important}.me-sm-1{margin-right:.25rem!important}.me-sm-2{margin-right:.5rem!important}.me-sm-3{margin-right:1rem!important}.me-sm-4{margin-right:1.5rem!important}.me-sm-5{margin-right:3rem!important}.me-sm-auto{margin-right:auto!important}.mb-sm-0{margin-bottom:0!important}.mb-sm-1{margin-bottom:.25rem!important}.mb-sm-2{margin-bottom:.5rem!important}.mb-sm-3{margin-bottom:1rem!important}.mb-sm-4{margin-bottom:1.5rem!important}.mb-sm-5{margin-bottom:3rem!important}.mb-sm-auto{margin-bottom:auto!important}.ms-sm-0{margin-left:0!important}.ms-sm-1{margin-left:.25rem!important}.ms-sm-2{margin-left:.5rem!important}.ms-sm-3{margin-left:1rem!important}.ms-sm-4{margin-left:1.5rem!important}.ms-sm-5{margin-left:3rem!important}.ms-sm-auto{margin-left:auto!important}.p-sm-0{padding:0!important}.p-sm-1{padding:.25rem!important}.p-sm-2{padding:.5rem!important}.p-sm-3{padding:1rem!important}.p-sm-4{padding:1.5rem!important}.p-sm-5{padding:3rem!important}.px-sm-0{padding-right:0!important;padding-left:0!important}.px-sm-1{padding-right:.25rem!important;padding-left:.25rem!important}.px-sm-2{padding-right:.5rem!important;padding-left:.5rem!important}.px-sm-3{padding-right:1rem!important;padding-left:1rem!important}.px-sm-4{padding-right:1.5rem!important;padding-left:1.5rem!important}.px-sm-5{padding-right:3rem!important;padding-left:3rem!important}.py-sm-0{padding-top:0!important;padding-bottom:0!important}.py-sm-1{padding-top:.25rem!important;padding-bottom:.25rem!important}.py-sm-2{padding-top:.5rem!important;padding-bottom:.5rem!important}.py-sm-3{padding-top:1rem!important;padding-bottom:1rem!important}.py-sm-4{padding-top:1.5rem!important;padding-bottom:1.5rem!important}.py-sm-5{padding-top:3rem!important;padding-bottom:3rem!important}.pt-sm-0{padding-top:0!important}.pt-sm-1{padding-top:.25rem!important}.pt-sm-2{padding-top:.5rem!important}.pt-sm-3{padding-top:1rem!important}.pt-sm-4{padding-top:1.5rem!important}.pt-sm-5{padding-top:3rem!important}.pe-sm-0{padding-right:0!important}.pe-sm-1{padding-right:.25rem!important}.pe-sm-2{padding-right:.5rem!important}.pe-sm-3{padding-right:1rem!important}.pe-sm-4{padding-right:1.5rem!important}.pe-sm-5{padding-right:3rem!important}.pb-sm-0{padding-bottom:0!important}.pb-sm-1{padding-bottom:.25rem!important}.pb-sm-2{padding-bottom:.5rem!important}.pb-sm-3{padding-bottom:1rem!important}.pb-sm-4{padding-bottom:1.5rem!important}.pb-sm-5{padding-bottom:3rem!important}.ps-sm-0{padding-left:0!important}.ps-sm-1{padding-left:.25rem!important}.ps-sm-2{padding-left:.5rem!important}.ps-sm-3{padding-left:1rem!important}.ps-sm-4{padding-left:1.5rem!important}.ps-sm-5{padding-left:3rem!important}.gap-sm-0{gap:0!important}.gap-sm-1{gap:.25rem!important}.gap-sm-2{gap:.5rem!important}.gap-sm-3{gap:1rem!important}.gap-sm-4{gap:1.5rem!important}.gap-sm-5{gap:3rem!important}.row-gap-sm-0{row-gap:0!important}.row-gap-sm-1{row-gap:.25rem!important}.row-gap-sm-2{row-gap:.5rem!important}.row-gap-sm-3{row-gap:1rem!important}.row-gap-sm-4{row-gap:1.5rem!important}.row-gap-sm-5{row-gap:3rem!important}.column-gap-sm-0{column-gap:0!important}.column-gap-sm-1{column-gap:.25rem!important}.column-gap-sm-2{column-gap:.5rem!important}.column-gap-sm-3{column-gap:1rem!important}.column-gap-sm-4{column-gap:1.5rem!important}.column-gap-sm-5{column-gap:3rem!important}.text-sm-start{text-align:left!important}.text-sm-end{text-align:right!important}.text-sm-center{text-align:center!important}}@media (min-width: 768px){.float-md-start{float:left!important}.float-md-end{float:right!important}.float-md-none{float:none!important}.object-fit-md-contain{object-fit:contain!important}.object-fit-md-cover{object-fit:cover!important}.object-fit-md-fill{object-fit:fill!important}.object-fit-md-scale{object-fit:scale-down!important}.object-fit-md-none{object-fit:none!important}.d-md-inline{display:inline!important}.d-md-inline-block{display:inline-block!important}.d-md-block{display:block!important}.d-md-grid{display:grid!important}.d-md-inline-grid{display:inline-grid!important}.d-md-table{display:table!important}.d-md-table-row{display:table-row!important}.d-md-table-cell{display:table-cell!important}.d-md-flex{display:flex!important}.d-md-inline-flex{display:inline-flex!important}.d-md-none{display:none!important}.flex-md-fill{flex:1 1 auto!important}.flex-md-row{flex-direction:row!important}.flex-md-column{flex-direction:column!important}.flex-md-row-reverse{flex-direction:row-reverse!important}.flex-md-column-reverse{flex-direction:column-reverse!important}.flex-md-grow-0{flex-grow:0!important}.flex-md-grow-1{flex-grow:1!important}.flex-md-shrink-0{flex-shrink:0!important}.flex-md-shrink-1{flex-shrink:1!important}.flex-md-wrap{flex-wrap:wrap!important}.flex-md-nowrap{flex-wrap:nowrap!important}.flex-md-wrap-reverse{flex-wrap:wrap-reverse!important}.justify-content-md-start{justify-content:flex-start!important}.justify-content-md-end{justify-content:flex-end!important}.justify-content-md-center{justify-content:center!important}.justify-content-md-between{justify-content:space-between!important}.justify-content-md-around{justify-content:space-around!important}.justify-content-md-evenly{justify-content:space-evenly!important}.align-items-md-start{align-items:flex-start!important}.align-items-md-end{align-items:flex-end!important}.align-items-md-center{align-items:center!important}.align-items-md-baseline{align-items:baseline!important}.align-items-md-stretch{align-items:stretch!important}.align-content-md-start{align-content:flex-start!important}.align-content-md-end{align-content:flex-end!important}.align-content-md-center{align-content:center!important}.align-content-md-between{align-content:space-between!important}.align-content-md-around{align-content:space-around!important}.align-content-md-stretch{align-content:stretch!important}.align-self-md-auto{align-self:auto!important}.align-self-md-start{align-self:flex-start!important}.align-self-md-end{align-self:flex-end!important}.align-self-md-center{align-self:center!important}.align-self-md-baseline{align-self:baseline!important}.align-self-md-stretch{align-self:stretch!important}.order-md-first{order:-1!important}.order-md-0{order:0!important}.order-md-1{order:1!important}.order-md-2{order:2!important}.order-md-3{order:3!important}.order-md-4{order:4!important}.order-md-5{order:5!important}.order-md-last{order:6!important}.m-md-0{margin:0!important}.m-md-1{margin:.25rem!important}.m-md-2{margin:.5rem!important}.m-md-3{margin:1rem!important}.m-md-4{margin:1.5rem!important}.m-md-5{margin:3rem!important}.m-md-auto{margin:auto!important}.mx-md-0{margin-right:0!important;margin-left:0!important}.mx-md-1{margin-right:.25rem!important;margin-left:.25rem!important}.mx-md-2{margin-right:.5rem!important;margin-left:.5rem!important}.mx-md-3{margin-right:1rem!important;margin-left:1rem!important}.mx-md-4{margin-right:1.5rem!important;margin-left:1.5rem!important}.mx-md-5{margin-right:3rem!important;margin-left:3rem!important}.mx-md-auto{margin-right:auto!important;margin-left:auto!important}.my-md-0{margin-top:0!important;margin-bottom:0!important}.my-md-1{margin-top:.25rem!important;margin-bottom:.25rem!important}.my-md-2{margin-top:.5rem!important;margin-bottom:.5rem!important}.my-md-3{margin-top:1rem!important;margin-bottom:1rem!important}.my-md-4{margin-top:1.5rem!important;margin-bottom:1.5rem!important}.my-md-5{margin-top:3rem!important;margin-bottom:3rem!important}.my-md-auto{margin-top:auto!important;margin-bottom:auto!important}.mt-md-0{margin-top:0!important}.mt-md-1{margin-top:.25rem!important}.mt-md-2{margin-top:.5rem!important}.mt-md-3{margin-top:1rem!important}.mt-md-4{margin-top:1.5rem!important}.mt-md-5{margin-top:3rem!important}.mt-md-auto{margin-top:auto!important}.me-md-0{margin-right:0!important}.me-md-1{margin-right:.25rem!important}.me-md-2{margin-right:.5rem!important}.me-md-3{margin-right:1rem!important}.me-md-4{margin-right:1.5rem!important}.me-md-5{margin-right:3rem!important}.me-md-auto{margin-right:auto!important}.mb-md-0{margin-bottom:0!important}.mb-md-1{margin-bottom:.25rem!important}.mb-md-2{margin-bottom:.5rem!important}.mb-md-3{margin-bottom:1rem!important}.mb-md-4{margin-bottom:1.5rem!important}.mb-md-5{margin-bottom:3rem!important}.mb-md-auto{margin-bottom:auto!important}.ms-md-0{margin-left:0!important}.ms-md-1{margin-left:.25rem!important}.ms-md-2{margin-left:.5rem!important}.ms-md-3{margin-left:1rem!important}.ms-md-4{margin-left:1.5rem!important}.ms-md-5{margin-left:3rem!important}.ms-md-auto{margin-left:auto!important}.p-md-0{padding:0!important}.p-md-1{padding:.25rem!important}.p-md-2{padding:.5rem!important}.p-md-3{padding:1rem!important}.p-md-4{padding:1.5rem!important}.p-md-5{padding:3rem!important}.px-md-0{padding-right:0!important;padding-left:0!important}.px-md-1{padding-right:.25rem!important;padding-left:.25rem!important}.px-md-2{padding-right:.5rem!important;padding-left:.5rem!important}.px-md-3{padding-right:1rem!important;padding-left:1rem!important}.px-md-4{padding-right:1.5rem!important;padding-left:1.5rem!important}.px-md-5{padding-right:3rem!important;padding-left:3rem!important}.py-md-0{padding-top:0!important;padding-bottom:0!important}.py-md-1{padding-top:.25rem!important;padding-bottom:.25rem!important}.py-md-2{padding-top:.5rem!important;padding-bottom:.5rem!important}.py-md-3{padding-top:1rem!important;padding-bottom:1rem!important}.py-md-4{padding-top:1.5rem!important;padding-bottom:1.5rem!important}.py-md-5{padding-top:3rem!important;padding-bottom:3rem!important}.pt-md-0{padding-top:0!important}.pt-md-1{padding-top:.25rem!important}.pt-md-2{padding-top:.5rem!important}.pt-md-3{padding-top:1rem!important}.pt-md-4{padding-top:1.5rem!important}.pt-md-5{padding-top:3rem!important}.pe-md-0{padding-right:0!important}.pe-md-1{padding-right:.25rem!important}.pe-md-2{padding-right:.5rem!important}.pe-md-3{padding-right:1rem!important}.pe-md-4{padding-right:1.5rem!important}.pe-md-5{padding-right:3rem!important}.pb-md-0{padding-bottom:0!important}.pb-md-1{padding-bottom:.25rem!important}.pb-md-2{padding-bottom:.5rem!important}.pb-md-3{padding-bottom:1rem!important}.pb-md-4{padding-bottom:1.5rem!important}.pb-md-5{padding-bottom:3rem!important}.ps-md-0{padding-left:0!important}.ps-md-1{padding-left:.25rem!important}.ps-md-2{padding-left:.5rem!important}.ps-md-3{padding-left:1rem!important}.ps-md-4{padding-left:1.5rem!important}.ps-md-5{padding-left:3rem!important}.gap-md-0{gap:0!important}.gap-md-1{gap:.25rem!important}.gap-md-2{gap:.5rem!important}.gap-md-3{gap:1rem!important}.gap-md-4{gap:1.5rem!important}.gap-md-5{gap:3rem!important}.row-gap-md-0{row-gap:0!important}.row-gap-md-1{row-gap:.25rem!important}.row-gap-md-2{row-gap:.5rem!important}.row-gap-md-3{row-gap:1rem!important}.row-gap-md-4{row-gap:1.5rem!important}.row-gap-md-5{row-gap:3rem!important}.column-gap-md-0{column-gap:0!important}.column-gap-md-1{column-gap:.25rem!important}.column-gap-md-2{column-gap:.5rem!important}.column-gap-md-3{column-gap:1rem!important}.column-gap-md-4{column-gap:1.5rem!important}.column-gap-md-5{column-gap:3rem!important}.text-md-start{text-align:left!important}.text-md-end{text-align:right!important}.text-md-center{text-align:center!important}}@media (min-width: 992px){.float-lg-start{float:left!important}.float-lg-end{float:right!important}.float-lg-none{float:none!important}.object-fit-lg-contain{object-fit:contain!important}.object-fit-lg-cover{object-fit:cover!important}.object-fit-lg-fill{object-fit:fill!important}.object-fit-lg-scale{object-fit:scale-down!important}.object-fit-lg-none{object-fit:none!important}.d-lg-inline{display:inline!important}.d-lg-inline-block{display:inline-block!important}.d-lg-block{display:block!important}.d-lg-grid{display:grid!important}.d-lg-inline-grid{display:inline-grid!important}.d-lg-table{display:table!important}.d-lg-table-row{display:table-row!important}.d-lg-table-cell{display:table-cell!important}.d-lg-flex{display:flex!important}.d-lg-inline-flex{display:inline-flex!important}.d-lg-none{display:none!important}.flex-lg-fill{flex:1 1 auto!important}.flex-lg-row{flex-direction:row!important}.flex-lg-column{flex-direction:column!important}.flex-lg-row-reverse{flex-direction:row-reverse!important}.flex-lg-column-reverse{flex-direction:column-reverse!important}.flex-lg-grow-0{flex-grow:0!important}.flex-lg-grow-1{flex-grow:1!important}.flex-lg-shrink-0{flex-shrink:0!important}.flex-lg-shrink-1{flex-shrink:1!important}.flex-lg-wrap{flex-wrap:wrap!important}.flex-lg-nowrap{flex-wrap:nowrap!important}.flex-lg-wrap-reverse{flex-wrap:wrap-reverse!important}.justify-content-lg-start{justify-content:flex-start!important}.justify-content-lg-end{justify-content:flex-end!important}.justify-content-lg-center{justify-content:center!important}.justify-content-lg-between{justify-content:space-between!important}.justify-content-lg-around{justify-content:space-around!important}.justify-content-lg-evenly{justify-content:space-evenly!important}.align-items-lg-start{align-items:flex-start!important}.align-items-lg-end{align-items:flex-end!important}.align-items-lg-center{align-items:center!important}.align-items-lg-baseline{align-items:baseline!important}.align-items-lg-stretch{align-items:stretch!important}.align-content-lg-start{align-content:flex-start!important}.align-content-lg-end{align-content:flex-end!important}.align-content-lg-center{align-content:center!important}.align-content-lg-between{align-content:space-between!important}.align-content-lg-around{align-content:space-around!important}.align-content-lg-stretch{align-content:stretch!important}.align-self-lg-auto{align-self:auto!important}.align-self-lg-start{align-self:flex-start!important}.align-self-lg-end{align-self:flex-end!important}.align-self-lg-center{align-self:center!important}.align-self-lg-baseline{align-self:baseline!important}.align-self-lg-stretch{align-self:stretch!important}.order-lg-first{order:-1!important}.order-lg-0{order:0!important}.order-lg-1{order:1!important}.order-lg-2{order:2!important}.order-lg-3{order:3!important}.order-lg-4{order:4!important}.order-lg-5{order:5!important}.order-lg-last{order:6!important}.m-lg-0{margin:0!important}.m-lg-1{margin:.25rem!important}.m-lg-2{margin:.5rem!important}.m-lg-3{margin:1rem!important}.m-lg-4{margin:1.5rem!important}.m-lg-5{margin:3rem!important}.m-lg-auto{margin:auto!important}.mx-lg-0{margin-right:0!important;margin-left:0!important}.mx-lg-1{margin-right:.25rem!important;margin-left:.25rem!important}.mx-lg-2{margin-right:.5rem!important;margin-left:.5rem!important}.mx-lg-3{margin-right:1rem!important;margin-left:1rem!important}.mx-lg-4{margin-right:1.5rem!important;margin-left:1.5rem!important}.mx-lg-5{margin-right:3rem!important;margin-left:3rem!important}.mx-lg-auto{margin-right:auto!important;margin-left:auto!important}.my-lg-0{margin-top:0!important;margin-bottom:0!important}.my-lg-1{margin-top:.25rem!important;margin-bottom:.25rem!important}.my-lg-2{margin-top:.5rem!important;margin-bottom:.5rem!important}.my-lg-3{margin-top:1rem!important;margin-bottom:1rem!important}.my-lg-4{margin-top:1.5rem!important;margin-bottom:1.5rem!important}.my-lg-5{margin-top:3rem!important;margin-bottom:3rem!important}.my-lg-auto{margin-top:auto!important;margin-bottom:auto!important}.mt-lg-0{margin-top:0!important}.mt-lg-1{margin-top:.25rem!important}.mt-lg-2{margin-top:.5rem!important}.mt-lg-3{margin-top:1rem!important}.mt-lg-4{margin-top:1.5rem!important}.mt-lg-5{margin-top:3rem!important}.mt-lg-auto{margin-top:auto!important}.me-lg-0{margin-right:0!important}.me-lg-1{margin-right:.25rem!important}.me-lg-2{margin-right:.5rem!important}.me-lg-3{margin-right:1rem!important}.me-lg-4{margin-right:1.5rem!important}.me-lg-5{margin-right:3rem!important}.me-lg-auto{margin-right:auto!important}.mb-lg-0{margin-bottom:0!important}.mb-lg-1{margin-bottom:.25rem!important}.mb-lg-2{margin-bottom:.5rem!important}.mb-lg-3{margin-bottom:1rem!important}.mb-lg-4{margin-bottom:1.5rem!important}.mb-lg-5{margin-bottom:3rem!important}.mb-lg-auto{margin-bottom:auto!important}.ms-lg-0{margin-left:0!important}.ms-lg-1{margin-left:.25rem!important}.ms-lg-2{margin-left:.5rem!important}.ms-lg-3{margin-left:1rem!important}.ms-lg-4{margin-left:1.5rem!important}.ms-lg-5{margin-left:3rem!important}.ms-lg-auto{margin-left:auto!important}.p-lg-0{padding:0!important}.p-lg-1{padding:.25rem!important}.p-lg-2{padding:.5rem!important}.p-lg-3{padding:1rem!important}.p-lg-4{padding:1.5rem!important}.p-lg-5{padding:3rem!important}.px-lg-0{padding-right:0!important;padding-left:0!important}.px-lg-1{padding-right:.25rem!important;padding-left:.25rem!important}.px-lg-2{padding-right:.5rem!important;padding-left:.5rem!important}.px-lg-3{padding-right:1rem!important;padding-left:1rem!important}.px-lg-4{padding-right:1.5rem!important;padding-left:1.5rem!important}.px-lg-5{padding-right:3rem!important;padding-left:3rem!important}.py-lg-0{padding-top:0!important;padding-bottom:0!important}.py-lg-1{padding-top:.25rem!important;padding-bottom:.25rem!important}.py-lg-2{padding-top:.5rem!important;padding-bottom:.5rem!important}.py-lg-3{padding-top:1rem!important;padding-bottom:1rem!important}.py-lg-4{padding-top:1.5rem!important;padding-bottom:1.5rem!important}.py-lg-5{padding-top:3rem!important;padding-bottom:3rem!important}.pt-lg-0{padding-top:0!important}.pt-lg-1{padding-top:.25rem!important}.pt-lg-2{padding-top:.5rem!important}.pt-lg-3{padding-top:1rem!important}.pt-lg-4{padding-top:1.5rem!important}.pt-lg-5{padding-top:3rem!important}.pe-lg-0{padding-right:0!important}.pe-lg-1{padding-right:.25rem!important}.pe-lg-2{padding-right:.5rem!important}.pe-lg-3{padding-right:1rem!important}.pe-lg-4{padding-right:1.5rem!important}.pe-lg-5{padding-right:3rem!important}.pb-lg-0{padding-bottom:0!important}.pb-lg-1{padding-bottom:.25rem!important}.pb-lg-2{padding-bottom:.5rem!important}.pb-lg-3{padding-bottom:1rem!important}.pb-lg-4{padding-bottom:1.5rem!important}.pb-lg-5{padding-bottom:3rem!important}.ps-lg-0{padding-left:0!important}.ps-lg-1{padding-left:.25rem!important}.ps-lg-2{padding-left:.5rem!important}.ps-lg-3{padding-left:1rem!important}.ps-lg-4{padding-left:1.5rem!important}.ps-lg-5{padding-left:3rem!important}.gap-lg-0{gap:0!important}.gap-lg-1{gap:.25rem!important}.gap-lg-2{gap:.5rem!important}.gap-lg-3{gap:1rem!important}.gap-lg-4{gap:1.5rem!important}.gap-lg-5{gap:3rem!important}.row-gap-lg-0{row-gap:0!important}.row-gap-lg-1{row-gap:.25rem!important}.row-gap-lg-2{row-gap:.5rem!important}.row-gap-lg-3{row-gap:1rem!important}.row-gap-lg-4{row-gap:1.5rem!important}.row-gap-lg-5{row-gap:3rem!important}.column-gap-lg-0{column-gap:0!important}.column-gap-lg-1{column-gap:.25rem!important}.column-gap-lg-2{column-gap:.5rem!important}.column-gap-lg-3{column-gap:1rem!important}.column-gap-lg-4{column-gap:1.5rem!important}.column-gap-lg-5{column-gap:3rem!important}.text-lg-start{text-align:left!important}.text-lg-end{text-align:right!important}.text-lg-center{text-align:center!important}}@media (min-width: 1200px){.float-xl-start{float:left!important}.float-xl-end{float:right!important}.float-xl-none{float:none!important}.object-fit-xl-contain{object-fit:contain!important}.object-fit-xl-cover{object-fit:cover!important}.object-fit-xl-fill{object-fit:fill!important}.object-fit-xl-scale{object-fit:scale-down!important}.object-fit-xl-none{object-fit:none!important}.d-xl-inline{display:inline!important}.d-xl-inline-block{display:inline-block!important}.d-xl-block{display:block!important}.d-xl-grid{display:grid!important}.d-xl-inline-grid{display:inline-grid!important}.d-xl-table{display:table!important}.d-xl-table-row{display:table-row!important}.d-xl-table-cell{display:table-cell!important}.d-xl-flex{display:flex!important}.d-xl-inline-flex{display:inline-flex!important}.d-xl-none{display:none!important}.flex-xl-fill{flex:1 1 auto!important}.flex-xl-row{flex-direction:row!important}.flex-xl-column{flex-direction:column!important}.flex-xl-row-reverse{flex-direction:row-reverse!important}.flex-xl-column-reverse{flex-direction:column-reverse!important}.flex-xl-grow-0{flex-grow:0!important}.flex-xl-grow-1{flex-grow:1!important}.flex-xl-shrink-0{flex-shrink:0!important}.flex-xl-shrink-1{flex-shrink:1!important}.flex-xl-wrap{flex-wrap:wrap!important}.flex-xl-nowrap{flex-wrap:nowrap!important}.flex-xl-wrap-reverse{flex-wrap:wrap-reverse!important}.justify-content-xl-start{justify-content:flex-start!important}.justify-content-xl-end{justify-content:flex-end!important}.justify-content-xl-center{justify-content:center!important}.justify-content-xl-between{justify-content:space-between!important}.justify-content-xl-around{justify-content:space-around!important}.justify-content-xl-evenly{justify-content:space-evenly!important}.align-items-xl-start{align-items:flex-start!important}.align-items-xl-end{align-items:flex-end!important}.align-items-xl-center{align-items:center!important}.align-items-xl-baseline{align-items:baseline!important}.align-items-xl-stretch{align-items:stretch!important}.align-content-xl-start{align-content:flex-start!important}.align-content-xl-end{align-content:flex-end!important}.align-content-xl-center{align-content:center!important}.align-content-xl-between{align-content:space-between!important}.align-content-xl-around{align-content:space-around!important}.align-content-xl-stretch{align-content:stretch!important}.align-self-xl-auto{align-self:auto!important}.align-self-xl-start{align-self:flex-start!important}.align-self-xl-end{align-self:flex-end!important}.align-self-xl-center{align-self:center!important}.align-self-xl-baseline{align-self:baseline!important}.align-self-xl-stretch{align-self:stretch!important}.order-xl-first{order:-1!important}.order-xl-0{order:0!important}.order-xl-1{order:1!important}.order-xl-2{order:2!important}.order-xl-3{order:3!important}.order-xl-4{order:4!important}.order-xl-5{order:5!important}.order-xl-last{order:6!important}.m-xl-0{margin:0!important}.m-xl-1{margin:.25rem!important}.m-xl-2{margin:.5rem!important}.m-xl-3{margin:1rem!important}.m-xl-4{margin:1.5rem!important}.m-xl-5{margin:3rem!important}.m-xl-auto{margin:auto!important}.mx-xl-0{margin-right:0!important;margin-left:0!important}.mx-xl-1{margin-right:.25rem!important;margin-left:.25rem!important}.mx-xl-2{margin-right:.5rem!important;margin-left:.5rem!important}.mx-xl-3{margin-right:1rem!important;margin-left:1rem!important}.mx-xl-4{margin-right:1.5rem!important;margin-left:1.5rem!important}.mx-xl-5{margin-right:3rem!important;margin-left:3rem!important}.mx-xl-auto{margin-right:auto!important;margin-left:auto!important}.my-xl-0{margin-top:0!important;margin-bottom:0!important}.my-xl-1{margin-top:.25rem!important;margin-bottom:.25rem!important}.my-xl-2{margin-top:.5rem!important;margin-bottom:.5rem!important}.my-xl-3{margin-top:1rem!important;margin-bottom:1rem!important}.my-xl-4{margin-top:1.5rem!important;margin-bottom:1.5rem!important}.my-xl-5{margin-top:3rem!important;margin-bottom:3rem!important}.my-xl-auto{margin-top:auto!important;margin-bottom:auto!important}.mt-xl-0{margin-top:0!important}.mt-xl-1{margin-top:.25rem!important}.mt-xl-2{margin-top:.5rem!important}.mt-xl-3{margin-top:1rem!important}.mt-xl-4{margin-top:1.5rem!important}.mt-xl-5{margin-top:3rem!important}.mt-xl-auto{margin-top:auto!important}.me-xl-0{margin-right:0!important}.me-xl-1{margin-right:.25rem!important}.me-xl-2{margin-right:.5rem!important}.me-xl-3{margin-right:1rem!important}.me-xl-4{margin-right:1.5rem!important}.me-xl-5{margin-right:3rem!important}.me-xl-auto{margin-right:auto!important}.mb-xl-0{margin-bottom:0!important}.mb-xl-1{margin-bottom:.25rem!important}.mb-xl-2{margin-bottom:.5rem!important}.mb-xl-3{margin-bottom:1rem!important}.mb-xl-4{margin-bottom:1.5rem!important}.mb-xl-5{margin-bottom:3rem!important}.mb-xl-auto{margin-bottom:auto!important}.ms-xl-0{margin-left:0!important}.ms-xl-1{margin-left:.25rem!important}.ms-xl-2{margin-left:.5rem!important}.ms-xl-3{margin-left:1rem!important}.ms-xl-4{margin-left:1.5rem!important}.ms-xl-5{margin-left:3rem!important}.ms-xl-auto{margin-left:auto!important}.p-xl-0{padding:0!important}.p-xl-1{padding:.25rem!important}.p-xl-2{padding:.5rem!important}.p-xl-3{padding:1rem!important}.p-xl-4{padding:1.5rem!important}.p-xl-5{padding:3rem!important}.px-xl-0{padding-right:0!important;padding-left:0!important}.px-xl-1{padding-right:.25rem!important;padding-left:.25rem!important}.px-xl-2{padding-right:.5rem!important;padding-left:.5rem!important}.px-xl-3{padding-right:1rem!important;padding-left:1rem!important}.px-xl-4{padding-right:1.5rem!important;padding-left:1.5rem!important}.px-xl-5{padding-right:3rem!important;padding-left:3rem!important}.py-xl-0{padding-top:0!important;padding-bottom:0!important}.py-xl-1{padding-top:.25rem!important;padding-bottom:.25rem!important}.py-xl-2{padding-top:.5rem!important;padding-bottom:.5rem!important}.py-xl-3{padding-top:1rem!important;padding-bottom:1rem!important}.py-xl-4{padding-top:1.5rem!important;padding-bottom:1.5rem!important}.py-xl-5{padding-top:3rem!important;padding-bottom:3rem!important}.pt-xl-0{padding-top:0!important}.pt-xl-1{padding-top:.25rem!important}.pt-xl-2{padding-top:.5rem!important}.pt-xl-3{padding-top:1rem!important}.pt-xl-4{padding-top:1.5rem!important}.pt-xl-5{padding-top:3rem!important}.pe-xl-0{padding-right:0!important}.pe-xl-1{padding-right:.25rem!important}.pe-xl-2{padding-right:.5rem!important}.pe-xl-3{padding-right:1rem!important}.pe-xl-4{padding-right:1.5rem!important}.pe-xl-5{padding-right:3rem!important}.pb-xl-0{padding-bottom:0!important}.pb-xl-1{padding-bottom:.25rem!important}.pb-xl-2{padding-bottom:.5rem!important}.pb-xl-3{padding-bottom:1rem!important}.pb-xl-4{padding-bottom:1.5rem!important}.pb-xl-5{padding-bottom:3rem!important}.ps-xl-0{padding-left:0!important}.ps-xl-1{padding-left:.25rem!important}.ps-xl-2{padding-left:.5rem!important}.ps-xl-3{padding-left:1rem!important}.ps-xl-4{padding-left:1.5rem!important}.ps-xl-5{padding-left:3rem!important}.gap-xl-0{gap:0!important}.gap-xl-1{gap:.25rem!important}.gap-xl-2{gap:.5rem!important}.gap-xl-3{gap:1rem!important}.gap-xl-4{gap:1.5rem!important}.gap-xl-5{gap:3rem!important}.row-gap-xl-0{row-gap:0!important}.row-gap-xl-1{row-gap:.25rem!important}.row-gap-xl-2{row-gap:.5rem!important}.row-gap-xl-3{row-gap:1rem!important}.row-gap-xl-4{row-gap:1.5rem!important}.row-gap-xl-5{row-gap:3rem!important}.column-gap-xl-0{column-gap:0!important}.column-gap-xl-1{column-gap:.25rem!important}.column-gap-xl-2{column-gap:.5rem!important}.column-gap-xl-3{column-gap:1rem!important}.column-gap-xl-4{column-gap:1.5rem!important}.column-gap-xl-5{column-gap:3rem!important}.text-xl-start{text-align:left!important}.text-xl-end{text-align:right!important}.text-xl-center{text-align:center!important}}@media (min-width: 1400px){.float-xxl-start{float:left!important}.float-xxl-end{float:right!important}.float-xxl-none{float:none!important}.object-fit-xxl-contain{object-fit:contain!important}.object-fit-xxl-cover{object-fit:cover!important}.object-fit-xxl-fill{object-fit:fill!important}.object-fit-xxl-scale{object-fit:scale-down!important}.object-fit-xxl-none{object-fit:none!important}.d-xxl-inline{display:inline!important}.d-xxl-inline-block{display:inline-block!important}.d-xxl-block{display:block!important}.d-xxl-grid{display:grid!important}.d-xxl-inline-grid{display:inline-grid!important}.d-xxl-table{display:table!important}.d-xxl-table-row{display:table-row!important}.d-xxl-table-cell{display:table-cell!important}.d-xxl-flex{display:flex!important}.d-xxl-inline-flex{display:inline-flex!important}.d-xxl-none{display:none!important}.flex-xxl-fill{flex:1 1 auto!important}.flex-xxl-row{flex-direction:row!important}.flex-xxl-column{flex-direction:column!important}.flex-xxl-row-reverse{flex-direction:row-reverse!important}.flex-xxl-column-reverse{flex-direction:column-reverse!important}.flex-xxl-grow-0{flex-grow:0!important}.flex-xxl-grow-1{flex-grow:1!important}.flex-xxl-shrink-0{flex-shrink:0!important}.flex-xxl-shrink-1{flex-shrink:1!important}.flex-xxl-wrap{flex-wrap:wrap!important}.flex-xxl-nowrap{flex-wrap:nowrap!important}.flex-xxl-wrap-reverse{flex-wrap:wrap-reverse!important}.justify-content-xxl-start{justify-content:flex-start!important}.justify-content-xxl-end{justify-content:flex-end!important}.justify-content-xxl-center{justify-content:center!important}.justify-content-xxl-between{justify-content:space-between!important}.justify-content-xxl-around{justify-content:space-around!important}.justify-content-xxl-evenly{justify-content:space-evenly!important}.align-items-xxl-start{align-items:flex-start!important}.align-items-xxl-end{align-items:flex-end!important}.align-items-xxl-center{align-items:center!important}.align-items-xxl-baseline{align-items:baseline!important}.align-items-xxl-stretch{align-items:stretch!important}.align-content-xxl-start{align-content:flex-start!important}.align-content-xxl-end{align-content:flex-end!important}.align-content-xxl-center{align-content:center!important}.align-content-xxl-between{align-content:space-between!important}.align-content-xxl-around{align-content:space-around!important}.align-content-xxl-stretch{align-content:stretch!important}.align-self-xxl-auto{align-self:auto!important}.align-self-xxl-start{align-self:flex-start!important}.align-self-xxl-end{align-self:flex-end!important}.align-self-xxl-center{align-self:center!important}.align-self-xxl-baseline{align-self:baseline!important}.align-self-xxl-stretch{align-self:stretch!important}.order-xxl-first{order:-1!important}.order-xxl-0{order:0!important}.order-xxl-1{order:1!important}.order-xxl-2{order:2!important}.order-xxl-3{order:3!important}.order-xxl-4{order:4!important}.order-xxl-5{order:5!important}.order-xxl-last{order:6!important}.m-xxl-0{margin:0!important}.m-xxl-1{margin:.25rem!important}.m-xxl-2{margin:.5rem!important}.m-xxl-3{margin:1rem!important}.m-xxl-4{margin:1.5rem!important}.m-xxl-5{margin:3rem!important}.m-xxl-auto{margin:auto!important}.mx-xxl-0{margin-right:0!important;margin-left:0!important}.mx-xxl-1{margin-right:.25rem!important;margin-left:.25rem!important}.mx-xxl-2{margin-right:.5rem!important;margin-left:.5rem!important}.mx-xxl-3{margin-right:1rem!important;margin-left:1rem!important}.mx-xxl-4{margin-right:1.5rem!important;margin-left:1.5rem!important}.mx-xxl-5{margin-right:3rem!important;margin-left:3rem!important}.mx-xxl-auto{margin-right:auto!important;margin-left:auto!important}.my-xxl-0{margin-top:0!important;margin-bottom:0!important}.my-xxl-1{margin-top:.25rem!important;margin-bottom:.25rem!important}.my-xxl-2{margin-top:.5rem!important;margin-bottom:.5rem!important}.my-xxl-3{margin-top:1rem!important;margin-bottom:1rem!important}.my-xxl-4{margin-top:1.5rem!important;margin-bottom:1.5rem!important}.my-xxl-5{margin-top:3rem!important;margin-bottom:3rem!important}.my-xxl-auto{margin-top:auto!important;margin-bottom:auto!important}.mt-xxl-0{margin-top:0!important}.mt-xxl-1{margin-top:.25rem!important}.mt-xxl-2{margin-top:.5rem!important}.mt-xxl-3{margin-top:1rem!important}.mt-xxl-4{margin-top:1.5rem!important}.mt-xxl-5{margin-top:3rem!important}.mt-xxl-auto{margin-top:auto!important}.me-xxl-0{margin-right:0!important}.me-xxl-1{margin-right:.25rem!important}.me-xxl-2{margin-right:.5rem!important}.me-xxl-3{margin-right:1rem!important}.me-xxl-4{margin-right:1.5rem!important}.me-xxl-5{margin-right:3rem!important}.me-xxl-auto{margin-right:auto!important}.mb-xxl-0{margin-bottom:0!important}.mb-xxl-1{margin-bottom:.25rem!important}.mb-xxl-2{margin-bottom:.5rem!important}.mb-xxl-3{margin-bottom:1rem!important}.mb-xxl-4{margin-bottom:1.5rem!important}.mb-xxl-5{margin-bottom:3rem!important}.mb-xxl-auto{margin-bottom:auto!important}.ms-xxl-0{margin-left:0!important}.ms-xxl-1{margin-left:.25rem!important}.ms-xxl-2{margin-left:.5rem!important}.ms-xxl-3{margin-left:1rem!important}.ms-xxl-4{margin-left:1.5rem!important}.ms-xxl-5{margin-left:3rem!important}.ms-xxl-auto{margin-left:auto!important}.p-xxl-0{padding:0!important}.p-xxl-1{padding:.25rem!important}.p-xxl-2{padding:.5rem!important}.p-xxl-3{padding:1rem!important}.p-xxl-4{padding:1.5rem!important}.p-xxl-5{padding:3rem!important}.px-xxl-0{padding-right:0!important;padding-left:0!important}.px-xxl-1{padding-right:.25rem!important;padding-left:.25rem!important}.px-xxl-2{padding-right:.5rem!important;padding-left:.5rem!important}.px-xxl-3{padding-right:1rem!important;padding-left:1rem!important}.px-xxl-4{padding-right:1.5rem!important;padding-left:1.5rem!important}.px-xxl-5{padding-right:3rem!important;padding-left:3rem!important}.py-xxl-0{padding-top:0!important;padding-bottom:0!important}.py-xxl-1{padding-top:.25rem!important;padding-bottom:.25rem!important}.py-xxl-2{padding-top:.5rem!important;padding-bottom:.5rem!important}.py-xxl-3{padding-top:1rem!important;padding-bottom:1rem!important}.py-xxl-4{padding-top:1.5rem!important;padding-bottom:1.5rem!important}.py-xxl-5{padding-top:3rem!important;padding-bottom:3rem!important}.pt-xxl-0{padding-top:0!important}.pt-xxl-1{padding-top:.25rem!important}.pt-xxl-2{padding-top:.5rem!important}.pt-xxl-3{padding-top:1rem!important}.pt-xxl-4{padding-top:1.5rem!important}.pt-xxl-5{padding-top:3rem!important}.pe-xxl-0{padding-right:0!important}.pe-xxl-1{padding-right:.25rem!important}.pe-xxl-2{padding-right:.5rem!important}.pe-xxl-3{padding-right:1rem!important}.pe-xxl-4{padding-right:1.5rem!important}.pe-xxl-5{padding-right:3rem!important}.pb-xxl-0{padding-bottom:0!important}.pb-xxl-1{padding-bottom:.25rem!important}.pb-xxl-2{padding-bottom:.5rem!important}.pb-xxl-3{padding-bottom:1rem!important}.pb-xxl-4{padding-bottom:1.5rem!important}.pb-xxl-5{padding-bottom:3rem!important}.ps-xxl-0{padding-left:0!important}.ps-xxl-1{padding-left:.25rem!important}.ps-xxl-2{padding-left:.5rem!important}.ps-xxl-3{padding-left:1rem!important}.ps-xxl-4{padding-left:1.5rem!important}.ps-xxl-5{padding-left:3rem!important}.gap-xxl-0{gap:0!important}.gap-xxl-1{gap:.25rem!important}.gap-xxl-2{gap:.5rem!important}.gap-xxl-3{gap:1rem!important}.gap-xxl-4{gap:1.5rem!important}.gap-xxl-5{gap:3rem!important}.row-gap-xxl-0{row-gap:0!important}.row-gap-xxl-1{row-gap:.25rem!important}.row-gap-xxl-2{row-gap:.5rem!important}.row-gap-xxl-3{row-gap:1rem!important}.row-gap-xxl-4{row-gap:1.5rem!important}.row-gap-xxl-5{row-gap:3rem!important}.column-gap-xxl-0{column-gap:0!important}.column-gap-xxl-1{column-gap:.25rem!important}.column-gap-xxl-2{column-gap:.5rem!important}.column-gap-xxl-3{column-gap:1rem!important}.column-gap-xxl-4{column-gap:1.5rem!important}.column-gap-xxl-5{column-gap:3rem!important}.text-xxl-start{text-align:left!important}.text-xxl-end{text-align:right!important}.text-xxl-center{text-align:center!important}}@media (min-width: 1200px){.fs-1{font-size:2.5rem!important}.fs-2{font-size:2rem!important}.fs-3{font-size:1.75rem!important}.fs-4{font-size:1.5rem!important}}@media print{.d-print-inline{display:inline!important}.d-print-inline-block{display:inline-block!important}.d-print-block{display:block!important}.d-print-grid{display:grid!important}.d-print-inline-grid{display:inline-grid!important}.d-print-table{display:table!important}.d-print-table-row{display:table-row!important}.d-print-table-cell{display:table-cell!important}.d-print-flex{display:flex!important}.d-print-inline-flex{display:inline-flex!important}.d-print-none{display:none!important}}:root{--bs-dark-rgb: 44, 62, 80}.cm-editor{outline:none!important}.cm-scroller{overflow:auto;min-height:400px;max-height:400px}.cm-content,.cm-gutter{min-height:400px!important}.link-primary{cursor:pointer}.rows-input{text-align:center;width:40px}.overflow-wrapper{overflow:auto;height:500px}.data-headers{background:#fff;position:sticky;top:0}.log-sql{word-wrap:break-word;white-space:normal!important}.list{-webkit-padding-start:0;list-style:none}.schema-wrapper{overflow:hidden}.toggle{cursor:pointer}td.name.indented{padding-left:30px}.stats-expand{cursor:pointer}.stats-th .counter{border:0 solid white}.table>thead>tr>th.preview-header{white-space:nowrap;border:0 solid white}div.sort{cursor:pointer}#schema_frame{width:100%;border:0}.schema-header{cursor:pointer}.counter{background-color:#ecf0f1;font-family:monospace}.sql{width:33%}.query_favorite_toggle{cursor:pointer}.query_favourite_detail{float:right}.btn-save-only{border-radius:0!important}.vite-not-running-canary{display:none}nav.navbar .nav-link{color:#fff}nav.navbar nav.nav-link:hover,nav.navbar .nav-link:focus{color:var(--bs-primary-bg-subtle)}nav.navbar .nav-pills .nav-link.active,nav.navbar .nav-pills .show>.nav-link{color:var(--bs-nav-pills-link-active-color);border:1px solid var(--bs-secondary-bg);background:none}nav.navbar .nav-link:hover,nav.navbar .navbar-brand:hover{background:none;color:var(--bs-primary-bg-subtle)!important}.dropdown-toggle:after{margin-left:0!important}#assistant_description_label{white-space:pre-wrap}#assistant_response pre{position:relative;background:#faebd7}#assistant_response .copy-btn{position:absolute;top:5px;right:5px;cursor:pointer}#additional_table_container{overflow-y:auto;max-height:10rem}#assistant_input_parent{max-height:120px;overflow:hidden}#response_block:after{content:"";position:absolute;top:-20px;right:10px;border-width:10px;border-style:solid;border-color:transparent transparent var(--bs-border-color) transparent}
+ */@font-face{font-display:block;font-family:bootstrap-icons;src:url(./bootstrap-icons.woff2?7141511ac37f13e1a387fb9fc6646256) format("woff2"),url(./bootstrap-icons.woff?7141511ac37f13e1a387fb9fc6646256) format("woff")}.bi:before,[class^=bi-]:before,[class*=" bi-"]:before{display:inline-block;font-family:bootstrap-icons!important;font-style:normal;font-weight:400!important;font-variant:normal;text-transform:none;line-height:1;vertical-align:-.125em;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.bi-123:before{content:""}.bi-alarm-fill:before{content:""}.bi-alarm:before{content:""}.bi-align-bottom:before{content:""}.bi-align-center:before{content:""}.bi-align-end:before{content:""}.bi-align-middle:before{content:""}.bi-align-start:before{content:""}.bi-align-top:before{content:""}.bi-alt:before{content:""}.bi-app-indicator:before{content:""}.bi-app:before{content:""}.bi-archive-fill:before{content:""}.bi-archive:before{content:""}.bi-arrow-90deg-down:before{content:""}.bi-arrow-90deg-left:before{content:""}.bi-arrow-90deg-right:before{content:""}.bi-arrow-90deg-up:before{content:""}.bi-arrow-bar-down:before{content:""}.bi-arrow-bar-left:before{content:""}.bi-arrow-bar-right:before{content:""}.bi-arrow-bar-up:before{content:""}.bi-arrow-clockwise:before{content:""}.bi-arrow-counterclockwise:before{content:""}.bi-arrow-down-circle-fill:before{content:""}.bi-arrow-down-circle:before{content:""}.bi-arrow-down-left-circle-fill:before{content:""}.bi-arrow-down-left-circle:before{content:""}.bi-arrow-down-left-square-fill:before{content:""}.bi-arrow-down-left-square:before{content:""}.bi-arrow-down-left:before{content:""}.bi-arrow-down-right-circle-fill:before{content:""}.bi-arrow-down-right-circle:before{content:""}.bi-arrow-down-right-square-fill:before{content:""}.bi-arrow-down-right-square:before{content:""}.bi-arrow-down-right:before{content:""}.bi-arrow-down-short:before{content:""}.bi-arrow-down-square-fill:before{content:""}.bi-arrow-down-square:before{content:""}.bi-arrow-down-up:before{content:""}.bi-arrow-down:before{content:""}.bi-arrow-left-circle-fill:before{content:""}.bi-arrow-left-circle:before{content:""}.bi-arrow-left-right:before{content:""}.bi-arrow-left-short:before{content:""}.bi-arrow-left-square-fill:before{content:""}.bi-arrow-left-square:before{content:""}.bi-arrow-left:before{content:""}.bi-arrow-repeat:before{content:""}.bi-arrow-return-left:before{content:""}.bi-arrow-return-right:before{content:""}.bi-arrow-right-circle-fill:before{content:""}.bi-arrow-right-circle:before{content:""}.bi-arrow-right-short:before{content:""}.bi-arrow-right-square-fill:before{content:""}.bi-arrow-right-square:before{content:""}.bi-arrow-right:before{content:""}.bi-arrow-up-circle-fill:before{content:""}.bi-arrow-up-circle:before{content:""}.bi-arrow-up-left-circle-fill:before{content:""}.bi-arrow-up-left-circle:before{content:""}.bi-arrow-up-left-square-fill:before{content:""}.bi-arrow-up-left-square:before{content:""}.bi-arrow-up-left:before{content:""}.bi-arrow-up-right-circle-fill:before{content:""}.bi-arrow-up-right-circle:before{content:""}.bi-arrow-up-right-square-fill:before{content:""}.bi-arrow-up-right-square:before{content:""}.bi-arrow-up-right:before{content:""}.bi-arrow-up-short:before{content:""}.bi-arrow-up-square-fill:before{content:""}.bi-arrow-up-square:before{content:""}.bi-arrow-up:before{content:""}.bi-arrows-angle-contract:before{content:""}.bi-arrows-angle-expand:before{content:""}.bi-arrows-collapse:before{content:""}.bi-arrows-expand:before{content:""}.bi-arrows-fullscreen:before{content:""}.bi-arrows-move:before{content:""}.bi-aspect-ratio-fill:before{content:""}.bi-aspect-ratio:before{content:""}.bi-asterisk:before{content:""}.bi-at:before{content:""}.bi-award-fill:before{content:""}.bi-award:before{content:""}.bi-back:before{content:""}.bi-backspace-fill:before{content:""}.bi-backspace-reverse-fill:before{content:""}.bi-backspace-reverse:before{content:""}.bi-backspace:before{content:""}.bi-badge-3d-fill:before{content:""}.bi-badge-3d:before{content:""}.bi-badge-4k-fill:before{content:""}.bi-badge-4k:before{content:""}.bi-badge-8k-fill:before{content:""}.bi-badge-8k:before{content:""}.bi-badge-ad-fill:before{content:""}.bi-badge-ad:before{content:""}.bi-badge-ar-fill:before{content:""}.bi-badge-ar:before{content:""}.bi-badge-cc-fill:before{content:""}.bi-badge-cc:before{content:""}.bi-badge-hd-fill:before{content:""}.bi-badge-hd:before{content:""}.bi-badge-tm-fill:before{content:""}.bi-badge-tm:before{content:""}.bi-badge-vo-fill:before{content:""}.bi-badge-vo:before{content:""}.bi-badge-vr-fill:before{content:""}.bi-badge-vr:before{content:""}.bi-badge-wc-fill:before{content:""}.bi-badge-wc:before{content:""}.bi-bag-check-fill:before{content:""}.bi-bag-check:before{content:""}.bi-bag-dash-fill:before{content:""}.bi-bag-dash:before{content:""}.bi-bag-fill:before{content:""}.bi-bag-plus-fill:before{content:""}.bi-bag-plus:before{content:""}.bi-bag-x-fill:before{content:""}.bi-bag-x:before{content:""}.bi-bag:before{content:""}.bi-bar-chart-fill:before{content:""}.bi-bar-chart-line-fill:before{content:""}.bi-bar-chart-line:before{content:""}.bi-bar-chart-steps:before{content:""}.bi-bar-chart:before{content:""}.bi-basket-fill:before{content:""}.bi-basket:before{content:""}.bi-basket2-fill:before{content:""}.bi-basket2:before{content:""}.bi-basket3-fill:before{content:""}.bi-basket3:before{content:""}.bi-battery-charging:before{content:""}.bi-battery-full:before{content:""}.bi-battery-half:before{content:""}.bi-battery:before{content:""}.bi-bell-fill:before{content:""}.bi-bell:before{content:""}.bi-bezier:before{content:""}.bi-bezier2:before{content:""}.bi-bicycle:before{content:""}.bi-binoculars-fill:before{content:""}.bi-binoculars:before{content:""}.bi-blockquote-left:before{content:""}.bi-blockquote-right:before{content:""}.bi-book-fill:before{content:""}.bi-book-half:before{content:""}.bi-book:before{content:""}.bi-bookmark-check-fill:before{content:""}.bi-bookmark-check:before{content:""}.bi-bookmark-dash-fill:before{content:""}.bi-bookmark-dash:before{content:""}.bi-bookmark-fill:before{content:""}.bi-bookmark-heart-fill:before{content:""}.bi-bookmark-heart:before{content:""}.bi-bookmark-plus-fill:before{content:""}.bi-bookmark-plus:before{content:""}.bi-bookmark-star-fill:before{content:""}.bi-bookmark-star:before{content:""}.bi-bookmark-x-fill:before{content:""}.bi-bookmark-x:before{content:""}.bi-bookmark:before{content:""}.bi-bookmarks-fill:before{content:""}.bi-bookmarks:before{content:""}.bi-bookshelf:before{content:""}.bi-bootstrap-fill:before{content:""}.bi-bootstrap-reboot:before{content:""}.bi-bootstrap:before{content:""}.bi-border-all:before{content:""}.bi-border-bottom:before{content:""}.bi-border-center:before{content:""}.bi-border-inner:before{content:""}.bi-border-left:before{content:""}.bi-border-middle:before{content:""}.bi-border-outer:before{content:""}.bi-border-right:before{content:""}.bi-border-style:before{content:""}.bi-border-top:before{content:""}.bi-border-width:before{content:""}.bi-border:before{content:""}.bi-bounding-box-circles:before{content:""}.bi-bounding-box:before{content:""}.bi-box-arrow-down-left:before{content:""}.bi-box-arrow-down-right:before{content:""}.bi-box-arrow-down:before{content:""}.bi-box-arrow-in-down-left:before{content:""}.bi-box-arrow-in-down-right:before{content:""}.bi-box-arrow-in-down:before{content:""}.bi-box-arrow-in-left:before{content:""}.bi-box-arrow-in-right:before{content:""}.bi-box-arrow-in-up-left:before{content:""}.bi-box-arrow-in-up-right:before{content:""}.bi-box-arrow-in-up:before{content:""}.bi-box-arrow-left:before{content:""}.bi-box-arrow-right:before{content:""}.bi-box-arrow-up-left:before{content:""}.bi-box-arrow-up-right:before{content:""}.bi-box-arrow-up:before{content:""}.bi-box-seam:before{content:""}.bi-box:before{content:""}.bi-braces:before{content:""}.bi-bricks:before{content:""}.bi-briefcase-fill:before{content:""}.bi-briefcase:before{content:""}.bi-brightness-alt-high-fill:before{content:""}.bi-brightness-alt-high:before{content:""}.bi-brightness-alt-low-fill:before{content:""}.bi-brightness-alt-low:before{content:""}.bi-brightness-high-fill:before{content:""}.bi-brightness-high:before{content:""}.bi-brightness-low-fill:before{content:""}.bi-brightness-low:before{content:""}.bi-broadcast-pin:before{content:""}.bi-broadcast:before{content:""}.bi-brush-fill:before{content:""}.bi-brush:before{content:""}.bi-bucket-fill:before{content:""}.bi-bucket:before{content:""}.bi-bug-fill:before{content:""}.bi-bug:before{content:""}.bi-building:before{content:""}.bi-bullseye:before{content:""}.bi-calculator-fill:before{content:""}.bi-calculator:before{content:""}.bi-calendar-check-fill:before{content:""}.bi-calendar-check:before{content:""}.bi-calendar-date-fill:before{content:""}.bi-calendar-date:before{content:""}.bi-calendar-day-fill:before{content:""}.bi-calendar-day:before{content:""}.bi-calendar-event-fill:before{content:""}.bi-calendar-event:before{content:""}.bi-calendar-fill:before{content:""}.bi-calendar-minus-fill:before{content:""}.bi-calendar-minus:before{content:""}.bi-calendar-month-fill:before{content:""}.bi-calendar-month:before{content:""}.bi-calendar-plus-fill:before{content:""}.bi-calendar-plus:before{content:""}.bi-calendar-range-fill:before{content:""}.bi-calendar-range:before{content:""}.bi-calendar-week-fill:before{content:""}.bi-calendar-week:before{content:""}.bi-calendar-x-fill:before{content:""}.bi-calendar-x:before{content:""}.bi-calendar:before{content:""}.bi-calendar2-check-fill:before{content:""}.bi-calendar2-check:before{content:""}.bi-calendar2-date-fill:before{content:""}.bi-calendar2-date:before{content:""}.bi-calendar2-day-fill:before{content:""}.bi-calendar2-day:before{content:""}.bi-calendar2-event-fill:before{content:""}.bi-calendar2-event:before{content:""}.bi-calendar2-fill:before{content:""}.bi-calendar2-minus-fill:before{content:""}.bi-calendar2-minus:before{content:""}.bi-calendar2-month-fill:before{content:""}.bi-calendar2-month:before{content:""}.bi-calendar2-plus-fill:before{content:""}.bi-calendar2-plus:before{content:""}.bi-calendar2-range-fill:before{content:""}.bi-calendar2-range:before{content:""}.bi-calendar2-week-fill:before{content:""}.bi-calendar2-week:before{content:""}.bi-calendar2-x-fill:before{content:""}.bi-calendar2-x:before{content:""}.bi-calendar2:before{content:""}.bi-calendar3-event-fill:before{content:""}.bi-calendar3-event:before{content:""}.bi-calendar3-fill:before{content:""}.bi-calendar3-range-fill:before{content:""}.bi-calendar3-range:before{content:""}.bi-calendar3-week-fill:before{content:""}.bi-calendar3-week:before{content:""}.bi-calendar3:before{content:""}.bi-calendar4-event:before{content:""}.bi-calendar4-range:before{content:""}.bi-calendar4-week:before{content:""}.bi-calendar4:before{content:""}.bi-camera-fill:before{content:""}.bi-camera-reels-fill:before{content:""}.bi-camera-reels:before{content:""}.bi-camera-video-fill:before{content:""}.bi-camera-video-off-fill:before{content:""}.bi-camera-video-off:before{content:""}.bi-camera-video:before{content:""}.bi-camera:before{content:""}.bi-camera2:before{content:""}.bi-capslock-fill:before{content:""}.bi-capslock:before{content:""}.bi-card-checklist:before{content:""}.bi-card-heading:before{content:""}.bi-card-image:before{content:""}.bi-card-list:before{content:""}.bi-card-text:before{content:""}.bi-caret-down-fill:before{content:""}.bi-caret-down-square-fill:before{content:""}.bi-caret-down-square:before{content:""}.bi-caret-down:before{content:""}.bi-caret-left-fill:before{content:""}.bi-caret-left-square-fill:before{content:""}.bi-caret-left-square:before{content:""}.bi-caret-left:before{content:""}.bi-caret-right-fill:before{content:""}.bi-caret-right-square-fill:before{content:""}.bi-caret-right-square:before{content:""}.bi-caret-right:before{content:""}.bi-caret-up-fill:before{content:""}.bi-caret-up-square-fill:before{content:""}.bi-caret-up-square:before{content:""}.bi-caret-up:before{content:""}.bi-cart-check-fill:before{content:""}.bi-cart-check:before{content:""}.bi-cart-dash-fill:before{content:""}.bi-cart-dash:before{content:""}.bi-cart-fill:before{content:""}.bi-cart-plus-fill:before{content:""}.bi-cart-plus:before{content:""}.bi-cart-x-fill:before{content:""}.bi-cart-x:before{content:""}.bi-cart:before{content:""}.bi-cart2:before{content:""}.bi-cart3:before{content:""}.bi-cart4:before{content:""}.bi-cash-stack:before{content:""}.bi-cash:before{content:""}.bi-cast:before{content:""}.bi-chat-dots-fill:before{content:""}.bi-chat-dots:before{content:""}.bi-chat-fill:before{content:""}.bi-chat-left-dots-fill:before{content:""}.bi-chat-left-dots:before{content:""}.bi-chat-left-fill:before{content:""}.bi-chat-left-quote-fill:before{content:""}.bi-chat-left-quote:before{content:""}.bi-chat-left-text-fill:before{content:""}.bi-chat-left-text:before{content:""}.bi-chat-left:before{content:""}.bi-chat-quote-fill:before{content:""}.bi-chat-quote:before{content:""}.bi-chat-right-dots-fill:before{content:""}.bi-chat-right-dots:before{content:""}.bi-chat-right-fill:before{content:""}.bi-chat-right-quote-fill:before{content:""}.bi-chat-right-quote:before{content:""}.bi-chat-right-text-fill:before{content:""}.bi-chat-right-text:before{content:""}.bi-chat-right:before{content:""}.bi-chat-square-dots-fill:before{content:""}.bi-chat-square-dots:before{content:""}.bi-chat-square-fill:before{content:""}.bi-chat-square-quote-fill:before{content:""}.bi-chat-square-quote:before{content:""}.bi-chat-square-text-fill:before{content:""}.bi-chat-square-text:before{content:""}.bi-chat-square:before{content:""}.bi-chat-text-fill:before{content:""}.bi-chat-text:before{content:""}.bi-chat:before{content:""}.bi-check-all:before{content:""}.bi-check-circle-fill:before{content:""}.bi-check-circle:before{content:""}.bi-check-square-fill:before{content:""}.bi-check-square:before{content:""}.bi-check:before{content:""}.bi-check2-all:before{content:""}.bi-check2-circle:before{content:""}.bi-check2-square:before{content:""}.bi-check2:before{content:""}.bi-chevron-bar-contract:before{content:""}.bi-chevron-bar-down:before{content:""}.bi-chevron-bar-expand:before{content:""}.bi-chevron-bar-left:before{content:""}.bi-chevron-bar-right:before{content:""}.bi-chevron-bar-up:before{content:""}.bi-chevron-compact-down:before{content:""}.bi-chevron-compact-left:before{content:""}.bi-chevron-compact-right:before{content:""}.bi-chevron-compact-up:before{content:""}.bi-chevron-contract:before{content:""}.bi-chevron-double-down:before{content:""}.bi-chevron-double-left:before{content:""}.bi-chevron-double-right:before{content:""}.bi-chevron-double-up:before{content:""}.bi-chevron-down:before{content:""}.bi-chevron-expand:before{content:""}.bi-chevron-left:before{content:""}.bi-chevron-right:before{content:""}.bi-chevron-up:before{content:""}.bi-circle-fill:before{content:""}.bi-circle-half:before{content:""}.bi-circle-square:before{content:""}.bi-circle:before{content:""}.bi-clipboard-check:before{content:""}.bi-clipboard-data:before{content:""}.bi-clipboard-minus:before{content:""}.bi-clipboard-plus:before{content:""}.bi-clipboard-x:before{content:""}.bi-clipboard:before{content:""}.bi-clock-fill:before{content:""}.bi-clock-history:before{content:""}.bi-clock:before{content:""}.bi-cloud-arrow-down-fill:before{content:""}.bi-cloud-arrow-down:before{content:""}.bi-cloud-arrow-up-fill:before{content:""}.bi-cloud-arrow-up:before{content:""}.bi-cloud-check-fill:before{content:""}.bi-cloud-check:before{content:""}.bi-cloud-download-fill:before{content:""}.bi-cloud-download:before{content:""}.bi-cloud-drizzle-fill:before{content:""}.bi-cloud-drizzle:before{content:""}.bi-cloud-fill:before{content:""}.bi-cloud-fog-fill:before{content:""}.bi-cloud-fog:before{content:""}.bi-cloud-fog2-fill:before{content:""}.bi-cloud-fog2:before{content:""}.bi-cloud-hail-fill:before{content:""}.bi-cloud-hail:before{content:""}.bi-cloud-haze-fill:before{content:""}.bi-cloud-haze:before{content:""}.bi-cloud-haze2-fill:before{content:""}.bi-cloud-lightning-fill:before{content:""}.bi-cloud-lightning-rain-fill:before{content:""}.bi-cloud-lightning-rain:before{content:""}.bi-cloud-lightning:before{content:""}.bi-cloud-minus-fill:before{content:""}.bi-cloud-minus:before{content:""}.bi-cloud-moon-fill:before{content:""}.bi-cloud-moon:before{content:""}.bi-cloud-plus-fill:before{content:""}.bi-cloud-plus:before{content:""}.bi-cloud-rain-fill:before{content:""}.bi-cloud-rain-heavy-fill:before{content:""}.bi-cloud-rain-heavy:before{content:""}.bi-cloud-rain:before{content:""}.bi-cloud-slash-fill:before{content:""}.bi-cloud-slash:before{content:""}.bi-cloud-sleet-fill:before{content:""}.bi-cloud-sleet:before{content:""}.bi-cloud-snow-fill:before{content:""}.bi-cloud-snow:before{content:""}.bi-cloud-sun-fill:before{content:""}.bi-cloud-sun:before{content:""}.bi-cloud-upload-fill:before{content:""}.bi-cloud-upload:before{content:""}.bi-cloud:before{content:""}.bi-clouds-fill:before{content:""}.bi-clouds:before{content:""}.bi-cloudy-fill:before{content:""}.bi-cloudy:before{content:""}.bi-code-slash:before{content:""}.bi-code-square:before{content:""}.bi-code:before{content:""}.bi-collection-fill:before{content:""}.bi-collection-play-fill:before{content:""}.bi-collection-play:before{content:""}.bi-collection:before{content:""}.bi-columns-gap:before{content:""}.bi-columns:before{content:""}.bi-command:before{content:""}.bi-compass-fill:before{content:""}.bi-compass:before{content:""}.bi-cone-striped:before{content:""}.bi-cone:before{content:""}.bi-controller:before{content:""}.bi-cpu-fill:before{content:""}.bi-cpu:before{content:""}.bi-credit-card-2-back-fill:before{content:""}.bi-credit-card-2-back:before{content:""}.bi-credit-card-2-front-fill:before{content:""}.bi-credit-card-2-front:before{content:""}.bi-credit-card-fill:before{content:""}.bi-credit-card:before{content:""}.bi-crop:before{content:""}.bi-cup-fill:before{content:""}.bi-cup-straw:before{content:""}.bi-cup:before{content:""}.bi-cursor-fill:before{content:""}.bi-cursor-text:before{content:""}.bi-cursor:before{content:""}.bi-dash-circle-dotted:before{content:""}.bi-dash-circle-fill:before{content:""}.bi-dash-circle:before{content:""}.bi-dash-square-dotted:before{content:""}.bi-dash-square-fill:before{content:""}.bi-dash-square:before{content:""}.bi-dash:before{content:""}.bi-diagram-2-fill:before{content:""}.bi-diagram-2:before{content:""}.bi-diagram-3-fill:before{content:""}.bi-diagram-3:before{content:""}.bi-diamond-fill:before{content:""}.bi-diamond-half:before{content:""}.bi-diamond:before{content:""}.bi-dice-1-fill:before{content:""}.bi-dice-1:before{content:""}.bi-dice-2-fill:before{content:""}.bi-dice-2:before{content:""}.bi-dice-3-fill:before{content:""}.bi-dice-3:before{content:""}.bi-dice-4-fill:before{content:""}.bi-dice-4:before{content:""}.bi-dice-5-fill:before{content:""}.bi-dice-5:before{content:""}.bi-dice-6-fill:before{content:""}.bi-dice-6:before{content:""}.bi-disc-fill:before{content:""}.bi-disc:before{content:""}.bi-discord:before{content:""}.bi-display-fill:before{content:""}.bi-display:before{content:""}.bi-distribute-horizontal:before{content:""}.bi-distribute-vertical:before{content:""}.bi-door-closed-fill:before{content:""}.bi-door-closed:before{content:""}.bi-door-open-fill:before{content:""}.bi-door-open:before{content:""}.bi-dot:before{content:""}.bi-download:before{content:""}.bi-droplet-fill:before{content:""}.bi-droplet-half:before{content:""}.bi-droplet:before{content:""}.bi-earbuds:before{content:""}.bi-easel-fill:before{content:""}.bi-easel:before{content:""}.bi-egg-fill:before{content:""}.bi-egg-fried:before{content:""}.bi-egg:before{content:""}.bi-eject-fill:before{content:""}.bi-eject:before{content:""}.bi-emoji-angry-fill:before{content:""}.bi-emoji-angry:before{content:""}.bi-emoji-dizzy-fill:before{content:""}.bi-emoji-dizzy:before{content:""}.bi-emoji-expressionless-fill:before{content:""}.bi-emoji-expressionless:before{content:""}.bi-emoji-frown-fill:before{content:""}.bi-emoji-frown:before{content:""}.bi-emoji-heart-eyes-fill:before{content:""}.bi-emoji-heart-eyes:before{content:""}.bi-emoji-laughing-fill:before{content:""}.bi-emoji-laughing:before{content:""}.bi-emoji-neutral-fill:before{content:""}.bi-emoji-neutral:before{content:""}.bi-emoji-smile-fill:before{content:""}.bi-emoji-smile-upside-down-fill:before{content:""}.bi-emoji-smile-upside-down:before{content:""}.bi-emoji-smile:before{content:""}.bi-emoji-sunglasses-fill:before{content:""}.bi-emoji-sunglasses:before{content:""}.bi-emoji-wink-fill:before{content:""}.bi-emoji-wink:before{content:""}.bi-envelope-fill:before{content:""}.bi-envelope-open-fill:before{content:""}.bi-envelope-open:before{content:""}.bi-envelope:before{content:""}.bi-eraser-fill:before{content:""}.bi-eraser:before{content:""}.bi-exclamation-circle-fill:before{content:""}.bi-exclamation-circle:before{content:""}.bi-exclamation-diamond-fill:before{content:""}.bi-exclamation-diamond:before{content:""}.bi-exclamation-octagon-fill:before{content:""}.bi-exclamation-octagon:before{content:""}.bi-exclamation-square-fill:before{content:""}.bi-exclamation-square:before{content:""}.bi-exclamation-triangle-fill:before{content:""}.bi-exclamation-triangle:before{content:""}.bi-exclamation:before{content:""}.bi-exclude:before{content:""}.bi-eye-fill:before{content:""}.bi-eye-slash-fill:before{content:""}.bi-eye-slash:before{content:""}.bi-eye:before{content:""}.bi-eyedropper:before{content:""}.bi-eyeglasses:before{content:""}.bi-facebook:before{content:""}.bi-file-arrow-down-fill:before{content:""}.bi-file-arrow-down:before{content:""}.bi-file-arrow-up-fill:before{content:""}.bi-file-arrow-up:before{content:""}.bi-file-bar-graph-fill:before{content:""}.bi-file-bar-graph:before{content:""}.bi-file-binary-fill:before{content:""}.bi-file-binary:before{content:""}.bi-file-break-fill:before{content:""}.bi-file-break:before{content:""}.bi-file-check-fill:before{content:""}.bi-file-check:before{content:""}.bi-file-code-fill:before{content:""}.bi-file-code:before{content:""}.bi-file-diff-fill:before{content:""}.bi-file-diff:before{content:""}.bi-file-earmark-arrow-down-fill:before{content:""}.bi-file-earmark-arrow-down:before{content:""}.bi-file-earmark-arrow-up-fill:before{content:""}.bi-file-earmark-arrow-up:before{content:""}.bi-file-earmark-bar-graph-fill:before{content:""}.bi-file-earmark-bar-graph:before{content:""}.bi-file-earmark-binary-fill:before{content:""}.bi-file-earmark-binary:before{content:""}.bi-file-earmark-break-fill:before{content:""}.bi-file-earmark-break:before{content:""}.bi-file-earmark-check-fill:before{content:""}.bi-file-earmark-check:before{content:""}.bi-file-earmark-code-fill:before{content:""}.bi-file-earmark-code:before{content:""}.bi-file-earmark-diff-fill:before{content:""}.bi-file-earmark-diff:before{content:""}.bi-file-earmark-easel-fill:before{content:""}.bi-file-earmark-easel:before{content:""}.bi-file-earmark-excel-fill:before{content:""}.bi-file-earmark-excel:before{content:""}.bi-file-earmark-fill:before{content:""}.bi-file-earmark-font-fill:before{content:""}.bi-file-earmark-font:before{content:""}.bi-file-earmark-image-fill:before{content:""}.bi-file-earmark-image:before{content:""}.bi-file-earmark-lock-fill:before{content:""}.bi-file-earmark-lock:before{content:""}.bi-file-earmark-lock2-fill:before{content:""}.bi-file-earmark-lock2:before{content:""}.bi-file-earmark-medical-fill:before{content:""}.bi-file-earmark-medical:before{content:""}.bi-file-earmark-minus-fill:before{content:""}.bi-file-earmark-minus:before{content:""}.bi-file-earmark-music-fill:before{content:""}.bi-file-earmark-music:before{content:""}.bi-file-earmark-person-fill:before{content:""}.bi-file-earmark-person:before{content:""}.bi-file-earmark-play-fill:before{content:""}.bi-file-earmark-play:before{content:""}.bi-file-earmark-plus-fill:before{content:""}.bi-file-earmark-plus:before{content:""}.bi-file-earmark-post-fill:before{content:""}.bi-file-earmark-post:before{content:""}.bi-file-earmark-ppt-fill:before{content:""}.bi-file-earmark-ppt:before{content:""}.bi-file-earmark-richtext-fill:before{content:""}.bi-file-earmark-richtext:before{content:""}.bi-file-earmark-ruled-fill:before{content:""}.bi-file-earmark-ruled:before{content:""}.bi-file-earmark-slides-fill:before{content:""}.bi-file-earmark-slides:before{content:""}.bi-file-earmark-spreadsheet-fill:before{content:""}.bi-file-earmark-spreadsheet:before{content:""}.bi-file-earmark-text-fill:before{content:""}.bi-file-earmark-text:before{content:""}.bi-file-earmark-word-fill:before{content:""}.bi-file-earmark-word:before{content:""}.bi-file-earmark-x-fill:before{content:""}.bi-file-earmark-x:before{content:""}.bi-file-earmark-zip-fill:before{content:""}.bi-file-earmark-zip:before{content:""}.bi-file-earmark:before{content:""}.bi-file-easel-fill:before{content:""}.bi-file-easel:before{content:""}.bi-file-excel-fill:before{content:""}.bi-file-excel:before{content:""}.bi-file-fill:before{content:""}.bi-file-font-fill:before{content:""}.bi-file-font:before{content:""}.bi-file-image-fill:before{content:""}.bi-file-image:before{content:""}.bi-file-lock-fill:before{content:""}.bi-file-lock:before{content:""}.bi-file-lock2-fill:before{content:""}.bi-file-lock2:before{content:""}.bi-file-medical-fill:before{content:""}.bi-file-medical:before{content:""}.bi-file-minus-fill:before{content:""}.bi-file-minus:before{content:""}.bi-file-music-fill:before{content:""}.bi-file-music:before{content:""}.bi-file-person-fill:before{content:""}.bi-file-person:before{content:""}.bi-file-play-fill:before{content:""}.bi-file-play:before{content:""}.bi-file-plus-fill:before{content:""}.bi-file-plus:before{content:""}.bi-file-post-fill:before{content:""}.bi-file-post:before{content:""}.bi-file-ppt-fill:before{content:""}.bi-file-ppt:before{content:""}.bi-file-richtext-fill:before{content:""}.bi-file-richtext:before{content:""}.bi-file-ruled-fill:before{content:""}.bi-file-ruled:before{content:""}.bi-file-slides-fill:before{content:""}.bi-file-slides:before{content:""}.bi-file-spreadsheet-fill:before{content:""}.bi-file-spreadsheet:before{content:""}.bi-file-text-fill:before{content:""}.bi-file-text:before{content:""}.bi-file-word-fill:before{content:""}.bi-file-word:before{content:""}.bi-file-x-fill:before{content:""}.bi-file-x:before{content:""}.bi-file-zip-fill:before{content:""}.bi-file-zip:before{content:""}.bi-file:before{content:""}.bi-files-alt:before{content:""}.bi-files:before{content:""}.bi-film:before{content:""}.bi-filter-circle-fill:before{content:""}.bi-filter-circle:before{content:""}.bi-filter-left:before{content:""}.bi-filter-right:before{content:""}.bi-filter-square-fill:before{content:""}.bi-filter-square:before{content:""}.bi-filter:before{content:""}.bi-flag-fill:before{content:""}.bi-flag:before{content:""}.bi-flower1:before{content:""}.bi-flower2:before{content:""}.bi-flower3:before{content:""}.bi-folder-check:before{content:""}.bi-folder-fill:before{content:""}.bi-folder-minus:before{content:""}.bi-folder-plus:before{content:""}.bi-folder-symlink-fill:before{content:""}.bi-folder-symlink:before{content:""}.bi-folder-x:before{content:""}.bi-folder:before{content:""}.bi-folder2-open:before{content:""}.bi-folder2:before{content:""}.bi-fonts:before{content:""}.bi-forward-fill:before{content:""}.bi-forward:before{content:""}.bi-front:before{content:""}.bi-fullscreen-exit:before{content:""}.bi-fullscreen:before{content:""}.bi-funnel-fill:before{content:""}.bi-funnel:before{content:""}.bi-gear-fill:before{content:""}.bi-gear-wide-connected:before{content:""}.bi-gear-wide:before{content:""}.bi-gear:before{content:""}.bi-gem:before{content:""}.bi-geo-alt-fill:before{content:""}.bi-geo-alt:before{content:""}.bi-geo-fill:before{content:""}.bi-geo:before{content:""}.bi-gift-fill:before{content:""}.bi-gift:before{content:""}.bi-github:before{content:""}.bi-globe:before{content:""}.bi-globe2:before{content:""}.bi-google:before{content:""}.bi-graph-down:before{content:""}.bi-graph-up:before{content:""}.bi-grid-1x2-fill:before{content:""}.bi-grid-1x2:before{content:""}.bi-grid-3x2-gap-fill:before{content:""}.bi-grid-3x2-gap:before{content:""}.bi-grid-3x2:before{content:""}.bi-grid-3x3-gap-fill:before{content:""}.bi-grid-3x3-gap:before{content:""}.bi-grid-3x3:before{content:""}.bi-grid-fill:before{content:""}.bi-grid:before{content:""}.bi-grip-horizontal:before{content:""}.bi-grip-vertical:before{content:""}.bi-hammer:before{content:""}.bi-hand-index-fill:before{content:""}.bi-hand-index-thumb-fill:before{content:""}.bi-hand-index-thumb:before{content:""}.bi-hand-index:before{content:""}.bi-hand-thumbs-down-fill:before{content:""}.bi-hand-thumbs-down:before{content:""}.bi-hand-thumbs-up-fill:before{content:""}.bi-hand-thumbs-up:before{content:""}.bi-handbag-fill:before{content:""}.bi-handbag:before{content:""}.bi-hash:before{content:""}.bi-hdd-fill:before{content:""}.bi-hdd-network-fill:before{content:""}.bi-hdd-network:before{content:""}.bi-hdd-rack-fill:before{content:""}.bi-hdd-rack:before{content:""}.bi-hdd-stack-fill:before{content:""}.bi-hdd-stack:before{content:""}.bi-hdd:before{content:""}.bi-headphones:before{content:""}.bi-headset:before{content:""}.bi-heart-fill:before{content:""}.bi-heart-half:before{content:""}.bi-heart:before{content:""}.bi-heptagon-fill:before{content:""}.bi-heptagon-half:before{content:""}.bi-heptagon:before{content:""}.bi-hexagon-fill:before{content:""}.bi-hexagon-half:before{content:""}.bi-hexagon:before{content:""}.bi-hourglass-bottom:before{content:""}.bi-hourglass-split:before{content:""}.bi-hourglass-top:before{content:""}.bi-hourglass:before{content:""}.bi-house-door-fill:before{content:""}.bi-house-door:before{content:""}.bi-house-fill:before{content:""}.bi-house:before{content:""}.bi-hr:before{content:""}.bi-hurricane:before{content:""}.bi-image-alt:before{content:""}.bi-image-fill:before{content:""}.bi-image:before{content:""}.bi-images:before{content:""}.bi-inbox-fill:before{content:""}.bi-inbox:before{content:""}.bi-inboxes-fill:before{content:""}.bi-inboxes:before{content:""}.bi-info-circle-fill:before{content:""}.bi-info-circle:before{content:""}.bi-info-square-fill:before{content:""}.bi-info-square:before{content:""}.bi-info:before{content:""}.bi-input-cursor-text:before{content:""}.bi-input-cursor:before{content:""}.bi-instagram:before{content:""}.bi-intersect:before{content:""}.bi-journal-album:before{content:""}.bi-journal-arrow-down:before{content:""}.bi-journal-arrow-up:before{content:""}.bi-journal-bookmark-fill:before{content:""}.bi-journal-bookmark:before{content:""}.bi-journal-check:before{content:""}.bi-journal-code:before{content:""}.bi-journal-medical:before{content:""}.bi-journal-minus:before{content:""}.bi-journal-plus:before{content:""}.bi-journal-richtext:before{content:""}.bi-journal-text:before{content:""}.bi-journal-x:before{content:""}.bi-journal:before{content:""}.bi-journals:before{content:""}.bi-joystick:before{content:""}.bi-justify-left:before{content:""}.bi-justify-right:before{content:""}.bi-justify:before{content:""}.bi-kanban-fill:before{content:""}.bi-kanban:before{content:""}.bi-key-fill:before{content:""}.bi-key:before{content:""}.bi-keyboard-fill:before{content:""}.bi-keyboard:before{content:""}.bi-ladder:before{content:""}.bi-lamp-fill:before{content:""}.bi-lamp:before{content:""}.bi-laptop-fill:before{content:""}.bi-laptop:before{content:""}.bi-layer-backward:before{content:""}.bi-layer-forward:before{content:""}.bi-layers-fill:before{content:""}.bi-layers-half:before{content:""}.bi-layers:before{content:""}.bi-layout-sidebar-inset-reverse:before{content:""}.bi-layout-sidebar-inset:before{content:""}.bi-layout-sidebar-reverse:before{content:""}.bi-layout-sidebar:before{content:""}.bi-layout-split:before{content:""}.bi-layout-text-sidebar-reverse:before{content:""}.bi-layout-text-sidebar:before{content:""}.bi-layout-text-window-reverse:before{content:""}.bi-layout-text-window:before{content:""}.bi-layout-three-columns:before{content:""}.bi-layout-wtf:before{content:""}.bi-life-preserver:before{content:""}.bi-lightbulb-fill:before{content:""}.bi-lightbulb-off-fill:before{content:""}.bi-lightbulb-off:before{content:""}.bi-lightbulb:before{content:""}.bi-lightning-charge-fill:before{content:""}.bi-lightning-charge:before{content:""}.bi-lightning-fill:before{content:""}.bi-lightning:before{content:""}.bi-link-45deg:before{content:""}.bi-link:before{content:""}.bi-linkedin:before{content:""}.bi-list-check:before{content:""}.bi-list-nested:before{content:""}.bi-list-ol:before{content:""}.bi-list-stars:before{content:""}.bi-list-task:before{content:""}.bi-list-ul:before{content:""}.bi-list:before{content:""}.bi-lock-fill:before{content:""}.bi-lock:before{content:""}.bi-mailbox:before{content:""}.bi-mailbox2:before{content:""}.bi-map-fill:before{content:""}.bi-map:before{content:""}.bi-markdown-fill:before{content:""}.bi-markdown:before{content:""}.bi-mask:before{content:""}.bi-megaphone-fill:before{content:""}.bi-megaphone:before{content:""}.bi-menu-app-fill:before{content:""}.bi-menu-app:before{content:""}.bi-menu-button-fill:before{content:""}.bi-menu-button-wide-fill:before{content:""}.bi-menu-button-wide:before{content:""}.bi-menu-button:before{content:""}.bi-menu-down:before{content:""}.bi-menu-up:before{content:""}.bi-mic-fill:before{content:""}.bi-mic-mute-fill:before{content:""}.bi-mic-mute:before{content:""}.bi-mic:before{content:""}.bi-minecart-loaded:before{content:""}.bi-minecart:before{content:""}.bi-moisture:before{content:""}.bi-moon-fill:before{content:""}.bi-moon-stars-fill:before{content:""}.bi-moon-stars:before{content:""}.bi-moon:before{content:""}.bi-mouse-fill:before{content:""}.bi-mouse:before{content:""}.bi-mouse2-fill:before{content:""}.bi-mouse2:before{content:""}.bi-mouse3-fill:before{content:""}.bi-mouse3:before{content:""}.bi-music-note-beamed:before{content:""}.bi-music-note-list:before{content:""}.bi-music-note:before{content:""}.bi-music-player-fill:before{content:""}.bi-music-player:before{content:""}.bi-newspaper:before{content:""}.bi-node-minus-fill:before{content:""}.bi-node-minus:before{content:""}.bi-node-plus-fill:before{content:""}.bi-node-plus:before{content:""}.bi-nut-fill:before{content:""}.bi-nut:before{content:""}.bi-octagon-fill:before{content:""}.bi-octagon-half:before{content:""}.bi-octagon:before{content:""}.bi-option:before{content:""}.bi-outlet:before{content:""}.bi-paint-bucket:before{content:""}.bi-palette-fill:before{content:""}.bi-palette:before{content:""}.bi-palette2:before{content:""}.bi-paperclip:before{content:""}.bi-paragraph:before{content:""}.bi-patch-check-fill:before{content:""}.bi-patch-check:before{content:""}.bi-patch-exclamation-fill:before{content:""}.bi-patch-exclamation:before{content:""}.bi-patch-minus-fill:before{content:""}.bi-patch-minus:before{content:""}.bi-patch-plus-fill:before{content:""}.bi-patch-plus:before{content:""}.bi-patch-question-fill:before{content:""}.bi-patch-question:before{content:""}.bi-pause-btn-fill:before{content:""}.bi-pause-btn:before{content:""}.bi-pause-circle-fill:before{content:""}.bi-pause-circle:before{content:""}.bi-pause-fill:before{content:""}.bi-pause:before{content:""}.bi-peace-fill:before{content:""}.bi-peace:before{content:""}.bi-pen-fill:before{content:""}.bi-pen:before{content:""}.bi-pencil-fill:before{content:""}.bi-pencil-square:before{content:""}.bi-pencil:before{content:""}.bi-pentagon-fill:before{content:""}.bi-pentagon-half:before{content:""}.bi-pentagon:before{content:""}.bi-people-fill:before{content:""}.bi-people:before{content:""}.bi-percent:before{content:""}.bi-person-badge-fill:before{content:""}.bi-person-badge:before{content:""}.bi-person-bounding-box:before{content:""}.bi-person-check-fill:before{content:""}.bi-person-check:before{content:""}.bi-person-circle:before{content:""}.bi-person-dash-fill:before{content:""}.bi-person-dash:before{content:""}.bi-person-fill:before{content:""}.bi-person-lines-fill:before{content:""}.bi-person-plus-fill:before{content:""}.bi-person-plus:before{content:""}.bi-person-square:before{content:""}.bi-person-x-fill:before{content:""}.bi-person-x:before{content:""}.bi-person:before{content:""}.bi-phone-fill:before{content:""}.bi-phone-landscape-fill:before{content:""}.bi-phone-landscape:before{content:""}.bi-phone-vibrate-fill:before{content:""}.bi-phone-vibrate:before{content:""}.bi-phone:before{content:""}.bi-pie-chart-fill:before{content:""}.bi-pie-chart:before{content:""}.bi-pin-angle-fill:before{content:""}.bi-pin-angle:before{content:""}.bi-pin-fill:before{content:""}.bi-pin:before{content:""}.bi-pip-fill:before{content:""}.bi-pip:before{content:""}.bi-play-btn-fill:before{content:""}.bi-play-btn:before{content:""}.bi-play-circle-fill:before{content:""}.bi-play-circle:before{content:""}.bi-play-fill:before{content:""}.bi-play:before{content:""}.bi-plug-fill:before{content:""}.bi-plug:before{content:""}.bi-plus-circle-dotted:before{content:""}.bi-plus-circle-fill:before{content:""}.bi-plus-circle:before{content:""}.bi-plus-square-dotted:before{content:""}.bi-plus-square-fill:before{content:""}.bi-plus-square:before{content:""}.bi-plus:before{content:""}.bi-power:before{content:""}.bi-printer-fill:before{content:""}.bi-printer:before{content:""}.bi-puzzle-fill:before{content:""}.bi-puzzle:before{content:""}.bi-question-circle-fill:before{content:""}.bi-question-circle:before{content:""}.bi-question-diamond-fill:before{content:""}.bi-question-diamond:before{content:""}.bi-question-octagon-fill:before{content:""}.bi-question-octagon:before{content:""}.bi-question-square-fill:before{content:""}.bi-question-square:before{content:""}.bi-question:before{content:""}.bi-rainbow:before{content:""}.bi-receipt-cutoff:before{content:""}.bi-receipt:before{content:""}.bi-reception-0:before{content:""}.bi-reception-1:before{content:""}.bi-reception-2:before{content:""}.bi-reception-3:before{content:""}.bi-reception-4:before{content:""}.bi-record-btn-fill:before{content:""}.bi-record-btn:before{content:""}.bi-record-circle-fill:before{content:""}.bi-record-circle:before{content:""}.bi-record-fill:before{content:""}.bi-record:before{content:""}.bi-record2-fill:before{content:""}.bi-record2:before{content:""}.bi-reply-all-fill:before{content:""}.bi-reply-all:before{content:""}.bi-reply-fill:before{content:""}.bi-reply:before{content:""}.bi-rss-fill:before{content:""}.bi-rss:before{content:""}.bi-rulers:before{content:""}.bi-save-fill:before{content:""}.bi-save:before{content:""}.bi-save2-fill:before{content:""}.bi-save2:before{content:""}.bi-scissors:before{content:""}.bi-screwdriver:before{content:""}.bi-search:before{content:""}.bi-segmented-nav:before{content:""}.bi-server:before{content:""}.bi-share-fill:before{content:""}.bi-share:before{content:""}.bi-shield-check:before{content:""}.bi-shield-exclamation:before{content:""}.bi-shield-fill-check:before{content:""}.bi-shield-fill-exclamation:before{content:""}.bi-shield-fill-minus:before{content:""}.bi-shield-fill-plus:before{content:""}.bi-shield-fill-x:before{content:""}.bi-shield-fill:before{content:""}.bi-shield-lock-fill:before{content:""}.bi-shield-lock:before{content:""}.bi-shield-minus:before{content:""}.bi-shield-plus:before{content:""}.bi-shield-shaded:before{content:""}.bi-shield-slash-fill:before{content:""}.bi-shield-slash:before{content:""}.bi-shield-x:before{content:""}.bi-shield:before{content:""}.bi-shift-fill:before{content:""}.bi-shift:before{content:""}.bi-shop-window:before{content:""}.bi-shop:before{content:""}.bi-shuffle:before{content:""}.bi-signpost-2-fill:before{content:""}.bi-signpost-2:before{content:""}.bi-signpost-fill:before{content:""}.bi-signpost-split-fill:before{content:""}.bi-signpost-split:before{content:""}.bi-signpost:before{content:""}.bi-sim-fill:before{content:""}.bi-sim:before{content:""}.bi-skip-backward-btn-fill:before{content:""}.bi-skip-backward-btn:before{content:""}.bi-skip-backward-circle-fill:before{content:""}.bi-skip-backward-circle:before{content:""}.bi-skip-backward-fill:before{content:""}.bi-skip-backward:before{content:""}.bi-skip-end-btn-fill:before{content:""}.bi-skip-end-btn:before{content:""}.bi-skip-end-circle-fill:before{content:""}.bi-skip-end-circle:before{content:""}.bi-skip-end-fill:before{content:""}.bi-skip-end:before{content:""}.bi-skip-forward-btn-fill:before{content:""}.bi-skip-forward-btn:before{content:""}.bi-skip-forward-circle-fill:before{content:""}.bi-skip-forward-circle:before{content:""}.bi-skip-forward-fill:before{content:""}.bi-skip-forward:before{content:""}.bi-skip-start-btn-fill:before{content:""}.bi-skip-start-btn:before{content:""}.bi-skip-start-circle-fill:before{content:""}.bi-skip-start-circle:before{content:""}.bi-skip-start-fill:before{content:""}.bi-skip-start:before{content:""}.bi-slack:before{content:""}.bi-slash-circle-fill:before{content:""}.bi-slash-circle:before{content:""}.bi-slash-square-fill:before{content:""}.bi-slash-square:before{content:""}.bi-slash:before{content:""}.bi-sliders:before{content:""}.bi-smartwatch:before{content:""}.bi-snow:before{content:""}.bi-snow2:before{content:""}.bi-snow3:before{content:""}.bi-sort-alpha-down-alt:before{content:""}.bi-sort-alpha-down:before{content:""}.bi-sort-alpha-up-alt:before{content:""}.bi-sort-alpha-up:before{content:""}.bi-sort-down-alt:before{content:""}.bi-sort-down:before{content:""}.bi-sort-numeric-down-alt:before{content:""}.bi-sort-numeric-down:before{content:""}.bi-sort-numeric-up-alt:before{content:""}.bi-sort-numeric-up:before{content:""}.bi-sort-up-alt:before{content:""}.bi-sort-up:before{content:""}.bi-soundwave:before{content:""}.bi-speaker-fill:before{content:""}.bi-speaker:before{content:""}.bi-speedometer:before{content:""}.bi-speedometer2:before{content:""}.bi-spellcheck:before{content:""}.bi-square-fill:before{content:""}.bi-square-half:before{content:""}.bi-square:before{content:""}.bi-stack:before{content:""}.bi-star-fill:before{content:""}.bi-star-half:before{content:""}.bi-star:before{content:""}.bi-stars:before{content:""}.bi-stickies-fill:before{content:""}.bi-stickies:before{content:""}.bi-sticky-fill:before{content:""}.bi-sticky:before{content:""}.bi-stop-btn-fill:before{content:""}.bi-stop-btn:before{content:""}.bi-stop-circle-fill:before{content:""}.bi-stop-circle:before{content:""}.bi-stop-fill:before{content:""}.bi-stop:before{content:""}.bi-stoplights-fill:before{content:""}.bi-stoplights:before{content:""}.bi-stopwatch-fill:before{content:""}.bi-stopwatch:before{content:""}.bi-subtract:before{content:""}.bi-suit-club-fill:before{content:""}.bi-suit-club:before{content:""}.bi-suit-diamond-fill:before{content:""}.bi-suit-diamond:before{content:""}.bi-suit-heart-fill:before{content:""}.bi-suit-heart:before{content:""}.bi-suit-spade-fill:before{content:""}.bi-suit-spade:before{content:""}.bi-sun-fill:before{content:""}.bi-sun:before{content:""}.bi-sunglasses:before{content:""}.bi-sunrise-fill:before{content:""}.bi-sunrise:before{content:""}.bi-sunset-fill:before{content:""}.bi-sunset:before{content:""}.bi-symmetry-horizontal:before{content:""}.bi-symmetry-vertical:before{content:""}.bi-table:before{content:""}.bi-tablet-fill:before{content:""}.bi-tablet-landscape-fill:before{content:""}.bi-tablet-landscape:before{content:""}.bi-tablet:before{content:""}.bi-tag-fill:before{content:""}.bi-tag:before{content:""}.bi-tags-fill:before{content:""}.bi-tags:before{content:""}.bi-telegram:before{content:""}.bi-telephone-fill:before{content:""}.bi-telephone-forward-fill:before{content:""}.bi-telephone-forward:before{content:""}.bi-telephone-inbound-fill:before{content:""}.bi-telephone-inbound:before{content:""}.bi-telephone-minus-fill:before{content:""}.bi-telephone-minus:before{content:""}.bi-telephone-outbound-fill:before{content:""}.bi-telephone-outbound:before{content:""}.bi-telephone-plus-fill:before{content:""}.bi-telephone-plus:before{content:""}.bi-telephone-x-fill:before{content:""}.bi-telephone-x:before{content:""}.bi-telephone:before{content:""}.bi-terminal-fill:before{content:""}.bi-terminal:before{content:""}.bi-text-center:before{content:""}.bi-text-indent-left:before{content:""}.bi-text-indent-right:before{content:""}.bi-text-left:before{content:""}.bi-text-paragraph:before{content:""}.bi-text-right:before{content:""}.bi-textarea-resize:before{content:""}.bi-textarea-t:before{content:""}.bi-textarea:before{content:""}.bi-thermometer-half:before{content:""}.bi-thermometer-high:before{content:""}.bi-thermometer-low:before{content:""}.bi-thermometer-snow:before{content:""}.bi-thermometer-sun:before{content:""}.bi-thermometer:before{content:""}.bi-three-dots-vertical:before{content:""}.bi-three-dots:before{content:""}.bi-toggle-off:before{content:""}.bi-toggle-on:before{content:""}.bi-toggle2-off:before{content:""}.bi-toggle2-on:before{content:""}.bi-toggles:before{content:""}.bi-toggles2:before{content:""}.bi-tools:before{content:""}.bi-tornado:before{content:""}.bi-trash-fill:before{content:""}.bi-trash:before{content:""}.bi-trash2-fill:before{content:""}.bi-trash2:before{content:""}.bi-tree-fill:before{content:""}.bi-tree:before{content:""}.bi-triangle-fill:before{content:""}.bi-triangle-half:before{content:""}.bi-triangle:before{content:""}.bi-trophy-fill:before{content:""}.bi-trophy:before{content:""}.bi-tropical-storm:before{content:""}.bi-truck-flatbed:before{content:""}.bi-truck:before{content:""}.bi-tsunami:before{content:""}.bi-tv-fill:before{content:""}.bi-tv:before{content:""}.bi-twitch:before{content:""}.bi-twitter:before{content:""}.bi-type-bold:before{content:""}.bi-type-h1:before{content:""}.bi-type-h2:before{content:""}.bi-type-h3:before{content:""}.bi-type-italic:before{content:""}.bi-type-strikethrough:before{content:""}.bi-type-underline:before{content:""}.bi-type:before{content:""}.bi-ui-checks-grid:before{content:""}.bi-ui-checks:before{content:""}.bi-ui-radios-grid:before{content:""}.bi-ui-radios:before{content:""}.bi-umbrella-fill:before{content:""}.bi-umbrella:before{content:""}.bi-union:before{content:""}.bi-unlock-fill:before{content:""}.bi-unlock:before{content:""}.bi-upc-scan:before{content:""}.bi-upc:before{content:""}.bi-upload:before{content:""}.bi-vector-pen:before{content:""}.bi-view-list:before{content:""}.bi-view-stacked:before{content:""}.bi-vinyl-fill:before{content:""}.bi-vinyl:before{content:""}.bi-voicemail:before{content:""}.bi-volume-down-fill:before{content:""}.bi-volume-down:before{content:""}.bi-volume-mute-fill:before{content:""}.bi-volume-mute:before{content:""}.bi-volume-off-fill:before{content:""}.bi-volume-off:before{content:""}.bi-volume-up-fill:before{content:""}.bi-volume-up:before{content:""}.bi-vr:before{content:""}.bi-wallet-fill:before{content:""}.bi-wallet:before{content:""}.bi-wallet2:before{content:""}.bi-watch:before{content:""}.bi-water:before{content:""}.bi-whatsapp:before{content:""}.bi-wifi-1:before{content:""}.bi-wifi-2:before{content:""}.bi-wifi-off:before{content:""}.bi-wifi:before{content:""}.bi-wind:before{content:""}.bi-window-dock:before{content:""}.bi-window-sidebar:before{content:""}.bi-window:before{content:""}.bi-wrench:before{content:""}.bi-x-circle-fill:before{content:""}.bi-x-circle:before{content:""}.bi-x-diamond-fill:before{content:""}.bi-x-diamond:before{content:""}.bi-x-octagon-fill:before{content:""}.bi-x-octagon:before{content:""}.bi-x-square-fill:before{content:""}.bi-x-square:before{content:""}.bi-x:before{content:""}.bi-youtube:before{content:""}.bi-zoom-in:before{content:""}.bi-zoom-out:before{content:""}.bi-bank:before{content:""}.bi-bank2:before{content:""}.bi-bell-slash-fill:before{content:""}.bi-bell-slash:before{content:""}.bi-cash-coin:before{content:""}.bi-check-lg:before{content:""}.bi-coin:before{content:""}.bi-currency-bitcoin:before{content:""}.bi-currency-dollar:before{content:""}.bi-currency-euro:before{content:""}.bi-currency-exchange:before{content:""}.bi-currency-pound:before{content:""}.bi-currency-yen:before{content:""}.bi-dash-lg:before{content:""}.bi-exclamation-lg:before{content:""}.bi-file-earmark-pdf-fill:before{content:""}.bi-file-earmark-pdf:before{content:""}.bi-file-pdf-fill:before{content:""}.bi-file-pdf:before{content:""}.bi-gender-ambiguous:before{content:""}.bi-gender-female:before{content:""}.bi-gender-male:before{content:""}.bi-gender-trans:before{content:""}.bi-headset-vr:before{content:""}.bi-info-lg:before{content:""}.bi-mastodon:before{content:""}.bi-messenger:before{content:""}.bi-piggy-bank-fill:before{content:""}.bi-piggy-bank:before{content:""}.bi-pin-map-fill:before{content:""}.bi-pin-map:before{content:""}.bi-plus-lg:before{content:""}.bi-question-lg:before{content:""}.bi-recycle:before{content:""}.bi-reddit:before{content:""}.bi-safe-fill:before{content:""}.bi-safe2-fill:before{content:""}.bi-safe2:before{content:""}.bi-sd-card-fill:before{content:""}.bi-sd-card:before{content:""}.bi-skype:before{content:""}.bi-slash-lg:before{content:""}.bi-translate:before{content:""}.bi-x-lg:before{content:""}.bi-safe:before{content:""}.bi-apple:before{content:""}.bi-microsoft:before{content:""}.bi-windows:before{content:""}.bi-behance:before{content:""}.bi-dribbble:before{content:""}.bi-line:before{content:""}.bi-medium:before{content:""}.bi-paypal:before{content:""}.bi-pinterest:before{content:""}.bi-signal:before{content:""}.bi-snapchat:before{content:""}.bi-spotify:before{content:""}.bi-stack-overflow:before{content:""}.bi-strava:before{content:""}.bi-wordpress:before{content:""}.bi-vimeo:before{content:""}.bi-activity:before{content:""}.bi-easel2-fill:before{content:""}.bi-easel2:before{content:""}.bi-easel3-fill:before{content:""}.bi-easel3:before{content:""}.bi-fan:before{content:""}.bi-fingerprint:before{content:""}.bi-graph-down-arrow:before{content:""}.bi-graph-up-arrow:before{content:""}.bi-hypnotize:before{content:""}.bi-magic:before{content:""}.bi-person-rolodex:before{content:""}.bi-person-video:before{content:""}.bi-person-video2:before{content:""}.bi-person-video3:before{content:""}.bi-person-workspace:before{content:""}.bi-radioactive:before{content:""}.bi-webcam-fill:before{content:""}.bi-webcam:before{content:""}.bi-yin-yang:before{content:""}.bi-bandaid-fill:before{content:""}.bi-bandaid:before{content:""}.bi-bluetooth:before{content:""}.bi-body-text:before{content:""}.bi-boombox:before{content:""}.bi-boxes:before{content:""}.bi-dpad-fill:before{content:""}.bi-dpad:before{content:""}.bi-ear-fill:before{content:""}.bi-ear:before{content:""}.bi-envelope-check-fill:before{content:""}.bi-envelope-check:before{content:""}.bi-envelope-dash-fill:before{content:""}.bi-envelope-dash:before{content:""}.bi-envelope-exclamation-fill:before{content:""}.bi-envelope-exclamation:before{content:""}.bi-envelope-plus-fill:before{content:""}.bi-envelope-plus:before{content:""}.bi-envelope-slash-fill:before{content:""}.bi-envelope-slash:before{content:""}.bi-envelope-x-fill:before{content:""}.bi-envelope-x:before{content:""}.bi-explicit-fill:before{content:""}.bi-explicit:before{content:""}.bi-git:before{content:""}.bi-infinity:before{content:""}.bi-list-columns-reverse:before{content:""}.bi-list-columns:before{content:""}.bi-meta:before{content:""}.bi-nintendo-switch:before{content:""}.bi-pc-display-horizontal:before{content:""}.bi-pc-display:before{content:""}.bi-pc-horizontal:before{content:""}.bi-pc:before{content:""}.bi-playstation:before{content:""}.bi-plus-slash-minus:before{content:""}.bi-projector-fill:before{content:""}.bi-projector:before{content:""}.bi-qr-code-scan:before{content:""}.bi-qr-code:before{content:""}.bi-quora:before{content:""}.bi-quote:before{content:""}.bi-robot:before{content:""}.bi-send-check-fill:before{content:""}.bi-send-check:before{content:""}.bi-send-dash-fill:before{content:""}.bi-send-dash:before{content:""}.bi-send-exclamation-fill:before{content:""}.bi-send-exclamation:before{content:""}.bi-send-fill:before{content:""}.bi-send-plus-fill:before{content:""}.bi-send-plus:before{content:""}.bi-send-slash-fill:before{content:""}.bi-send-slash:before{content:""}.bi-send-x-fill:before{content:""}.bi-send-x:before{content:""}.bi-send:before{content:""}.bi-steam:before{content:""}.bi-terminal-dash:before{content:""}.bi-terminal-plus:before{content:""}.bi-terminal-split:before{content:""}.bi-ticket-detailed-fill:before{content:""}.bi-ticket-detailed:before{content:""}.bi-ticket-fill:before{content:""}.bi-ticket-perforated-fill:before{content:""}.bi-ticket-perforated:before{content:""}.bi-ticket:before{content:""}.bi-tiktok:before{content:""}.bi-window-dash:before{content:""}.bi-window-desktop:before{content:""}.bi-window-fullscreen:before{content:""}.bi-window-plus:before{content:""}.bi-window-split:before{content:""}.bi-window-stack:before{content:""}.bi-window-x:before{content:""}.bi-xbox:before{content:""}.bi-ethernet:before{content:""}.bi-hdmi-fill:before{content:""}.bi-hdmi:before{content:""}.bi-usb-c-fill:before{content:""}.bi-usb-c:before{content:""}.bi-usb-fill:before{content:""}.bi-usb-plug-fill:before{content:""}.bi-usb-plug:before{content:""}.bi-usb-symbol:before{content:""}.bi-usb:before{content:""}.bi-boombox-fill:before{content:""}.bi-displayport:before{content:""}.bi-gpu-card:before{content:""}.bi-memory:before{content:""}.bi-modem-fill:before{content:""}.bi-modem:before{content:""}.bi-motherboard-fill:before{content:""}.bi-motherboard:before{content:""}.bi-optical-audio-fill:before{content:""}.bi-optical-audio:before{content:""}.bi-pci-card:before{content:""}.bi-router-fill:before{content:""}.bi-router:before{content:""}.bi-thunderbolt-fill:before{content:""}.bi-thunderbolt:before{content:""}.bi-usb-drive-fill:before{content:""}.bi-usb-drive:before{content:""}.bi-usb-micro-fill:before{content:""}.bi-usb-micro:before{content:""}.bi-usb-mini-fill:before{content:""}.bi-usb-mini:before{content:""}.bi-cloud-haze2:before{content:""}.bi-device-hdd-fill:before{content:""}.bi-device-hdd:before{content:""}.bi-device-ssd-fill:before{content:""}.bi-device-ssd:before{content:""}.bi-displayport-fill:before{content:""}.bi-mortarboard-fill:before{content:""}.bi-mortarboard:before{content:""}.bi-terminal-x:before{content:""}.bi-arrow-through-heart-fill:before{content:""}.bi-arrow-through-heart:before{content:""}.bi-badge-sd-fill:before{content:""}.bi-badge-sd:before{content:""}.bi-bag-heart-fill:before{content:""}.bi-bag-heart:before{content:""}.bi-balloon-fill:before{content:""}.bi-balloon-heart-fill:before{content:""}.bi-balloon-heart:before{content:""}.bi-balloon:before{content:""}.bi-box2-fill:before{content:""}.bi-box2-heart-fill:before{content:""}.bi-box2-heart:before{content:""}.bi-box2:before{content:""}.bi-braces-asterisk:before{content:""}.bi-calendar-heart-fill:before{content:""}.bi-calendar-heart:before{content:""}.bi-calendar2-heart-fill:before{content:""}.bi-calendar2-heart:before{content:""}.bi-chat-heart-fill:before{content:""}.bi-chat-heart:before{content:""}.bi-chat-left-heart-fill:before{content:""}.bi-chat-left-heart:before{content:""}.bi-chat-right-heart-fill:before{content:""}.bi-chat-right-heart:before{content:""}.bi-chat-square-heart-fill:before{content:""}.bi-chat-square-heart:before{content:""}.bi-clipboard-check-fill:before{content:""}.bi-clipboard-data-fill:before{content:""}.bi-clipboard-fill:before{content:""}.bi-clipboard-heart-fill:before{content:""}.bi-clipboard-heart:before{content:""}.bi-clipboard-minus-fill:before{content:""}.bi-clipboard-plus-fill:before{content:""}.bi-clipboard-pulse:before{content:""}.bi-clipboard-x-fill:before{content:""}.bi-clipboard2-check-fill:before{content:""}.bi-clipboard2-check:before{content:""}.bi-clipboard2-data-fill:before{content:""}.bi-clipboard2-data:before{content:""}.bi-clipboard2-fill:before{content:""}.bi-clipboard2-heart-fill:before{content:""}.bi-clipboard2-heart:before{content:""}.bi-clipboard2-minus-fill:before{content:""}.bi-clipboard2-minus:before{content:""}.bi-clipboard2-plus-fill:before{content:""}.bi-clipboard2-plus:before{content:""}.bi-clipboard2-pulse-fill:before{content:""}.bi-clipboard2-pulse:before{content:""}.bi-clipboard2-x-fill:before{content:""}.bi-clipboard2-x:before{content:""}.bi-clipboard2:before{content:""}.bi-emoji-kiss-fill:before{content:""}.bi-emoji-kiss:before{content:""}.bi-envelope-heart-fill:before{content:""}.bi-envelope-heart:before{content:""}.bi-envelope-open-heart-fill:before{content:""}.bi-envelope-open-heart:before{content:""}.bi-envelope-paper-fill:before{content:""}.bi-envelope-paper-heart-fill:before{content:""}.bi-envelope-paper-heart:before{content:""}.bi-envelope-paper:before{content:""}.bi-filetype-aac:before{content:""}.bi-filetype-ai:before{content:""}.bi-filetype-bmp:before{content:""}.bi-filetype-cs:before{content:""}.bi-filetype-css:before{content:""}.bi-filetype-csv:before{content:""}.bi-filetype-doc:before{content:""}.bi-filetype-docx:before{content:""}.bi-filetype-exe:before{content:""}.bi-filetype-gif:before{content:""}.bi-filetype-heic:before{content:""}.bi-filetype-html:before{content:""}.bi-filetype-java:before{content:""}.bi-filetype-jpg:before{content:""}.bi-filetype-js:before{content:""}.bi-filetype-jsx:before{content:""}.bi-filetype-key:before{content:""}.bi-filetype-m4p:before{content:""}.bi-filetype-md:before{content:""}.bi-filetype-mdx:before{content:""}.bi-filetype-mov:before{content:""}.bi-filetype-mp3:before{content:""}.bi-filetype-mp4:before{content:""}.bi-filetype-otf:before{content:""}.bi-filetype-pdf:before{content:""}.bi-filetype-php:before{content:""}.bi-filetype-png:before{content:""}.bi-filetype-ppt:before{content:""}.bi-filetype-psd:before{content:""}.bi-filetype-py:before{content:""}.bi-filetype-raw:before{content:""}.bi-filetype-rb:before{content:""}.bi-filetype-sass:before{content:""}.bi-filetype-scss:before{content:""}.bi-filetype-sh:before{content:""}.bi-filetype-svg:before{content:""}.bi-filetype-tiff:before{content:""}.bi-filetype-tsx:before{content:""}.bi-filetype-ttf:before{content:""}.bi-filetype-txt:before{content:""}.bi-filetype-wav:before{content:""}.bi-filetype-woff:before{content:""}.bi-filetype-xls:before{content:""}.bi-filetype-xml:before{content:""}.bi-filetype-yml:before{content:""}.bi-heart-arrow:before{content:""}.bi-heart-pulse-fill:before{content:""}.bi-heart-pulse:before{content:""}.bi-heartbreak-fill:before{content:""}.bi-heartbreak:before{content:""}.bi-hearts:before{content:""}.bi-hospital-fill:before{content:""}.bi-hospital:before{content:""}.bi-house-heart-fill:before{content:""}.bi-house-heart:before{content:""}.bi-incognito:before{content:""}.bi-magnet-fill:before{content:""}.bi-magnet:before{content:""}.bi-person-heart:before{content:""}.bi-person-hearts:before{content:""}.bi-phone-flip:before{content:""}.bi-plugin:before{content:""}.bi-postage-fill:before{content:""}.bi-postage-heart-fill:before{content:""}.bi-postage-heart:before{content:""}.bi-postage:before{content:""}.bi-postcard-fill:before{content:""}.bi-postcard-heart-fill:before{content:""}.bi-postcard-heart:before{content:""}.bi-postcard:before{content:""}.bi-search-heart-fill:before{content:""}.bi-search-heart:before{content:""}.bi-sliders2-vertical:before{content:""}.bi-sliders2:before{content:""}.bi-trash3-fill:before{content:""}.bi-trash3:before{content:""}.bi-valentine:before{content:""}.bi-valentine2:before{content:""}.bi-wrench-adjustable-circle-fill:before{content:""}.bi-wrench-adjustable-circle:before{content:""}.bi-wrench-adjustable:before{content:""}.bi-filetype-json:before{content:""}.bi-filetype-pptx:before{content:""}.bi-filetype-xlsx:before{content:""}.bi-1-circle-fill:before{content:""}.bi-1-circle:before{content:""}.bi-1-square-fill:before{content:""}.bi-1-square:before{content:""}.bi-2-circle-fill:before{content:""}.bi-2-circle:before{content:""}.bi-2-square-fill:before{content:""}.bi-2-square:before{content:""}.bi-3-circle-fill:before{content:""}.bi-3-circle:before{content:""}.bi-3-square-fill:before{content:""}.bi-3-square:before{content:""}.bi-4-circle-fill:before{content:""}.bi-4-circle:before{content:""}.bi-4-square-fill:before{content:""}.bi-4-square:before{content:""}.bi-5-circle-fill:before{content:""}.bi-5-circle:before{content:""}.bi-5-square-fill:before{content:""}.bi-5-square:before{content:""}.bi-6-circle-fill:before{content:""}.bi-6-circle:before{content:""}.bi-6-square-fill:before{content:""}.bi-6-square:before{content:""}.bi-7-circle-fill:before{content:""}.bi-7-circle:before{content:""}.bi-7-square-fill:before{content:""}.bi-7-square:before{content:""}.bi-8-circle-fill:before{content:""}.bi-8-circle:before{content:""}.bi-8-square-fill:before{content:""}.bi-8-square:before{content:""}.bi-9-circle-fill:before{content:""}.bi-9-circle:before{content:""}.bi-9-square-fill:before{content:""}.bi-9-square:before{content:""}.bi-airplane-engines-fill:before{content:""}.bi-airplane-engines:before{content:""}.bi-airplane-fill:before{content:""}.bi-airplane:before{content:""}.bi-alexa:before{content:""}.bi-alipay:before{content:""}.bi-android:before{content:""}.bi-android2:before{content:""}.bi-box-fill:before{content:""}.bi-box-seam-fill:before{content:""}.bi-browser-chrome:before{content:""}.bi-browser-edge:before{content:""}.bi-browser-firefox:before{content:""}.bi-browser-safari:before{content:""}.bi-c-circle-fill:before{content:""}.bi-c-circle:before{content:""}.bi-c-square-fill:before{content:""}.bi-c-square:before{content:""}.bi-capsule-pill:before{content:""}.bi-capsule:before{content:""}.bi-car-front-fill:before{content:""}.bi-car-front:before{content:""}.bi-cassette-fill:before{content:""}.bi-cassette:before{content:""}.bi-cc-circle-fill:before{content:""}.bi-cc-circle:before{content:""}.bi-cc-square-fill:before{content:""}.bi-cc-square:before{content:""}.bi-cup-hot-fill:before{content:""}.bi-cup-hot:before{content:""}.bi-currency-rupee:before{content:""}.bi-dropbox:before{content:""}.bi-escape:before{content:""}.bi-fast-forward-btn-fill:before{content:""}.bi-fast-forward-btn:before{content:""}.bi-fast-forward-circle-fill:before{content:""}.bi-fast-forward-circle:before{content:""}.bi-fast-forward-fill:before{content:""}.bi-fast-forward:before{content:""}.bi-filetype-sql:before{content:""}.bi-fire:before{content:""}.bi-google-play:before{content:""}.bi-h-circle-fill:before{content:""}.bi-h-circle:before{content:""}.bi-h-square-fill:before{content:""}.bi-h-square:before{content:""}.bi-indent:before{content:""}.bi-lungs-fill:before{content:""}.bi-lungs:before{content:""}.bi-microsoft-teams:before{content:""}.bi-p-circle-fill:before{content:""}.bi-p-circle:before{content:""}.bi-p-square-fill:before{content:""}.bi-p-square:before{content:""}.bi-pass-fill:before{content:""}.bi-pass:before{content:""}.bi-prescription:before{content:""}.bi-prescription2:before{content:""}.bi-r-circle-fill:before{content:""}.bi-r-circle:before{content:""}.bi-r-square-fill:before{content:""}.bi-r-square:before{content:""}.bi-repeat-1:before{content:""}.bi-repeat:before{content:""}.bi-rewind-btn-fill:before{content:""}.bi-rewind-btn:before{content:""}.bi-rewind-circle-fill:before{content:""}.bi-rewind-circle:before{content:""}.bi-rewind-fill:before{content:""}.bi-rewind:before{content:""}.bi-train-freight-front-fill:before{content:""}.bi-train-freight-front:before{content:""}.bi-train-front-fill:before{content:""}.bi-train-front:before{content:""}.bi-train-lightrail-front-fill:before{content:""}.bi-train-lightrail-front:before{content:""}.bi-truck-front-fill:before{content:""}.bi-truck-front:before{content:""}.bi-ubuntu:before{content:""}.bi-unindent:before{content:""}.bi-unity:before{content:""}.bi-universal-access-circle:before{content:""}.bi-universal-access:before{content:""}.bi-virus:before{content:""}.bi-virus2:before{content:""}.bi-wechat:before{content:""}.bi-yelp:before{content:""}.bi-sign-stop-fill:before{content:""}.bi-sign-stop-lights-fill:before{content:""}.bi-sign-stop-lights:before{content:""}.bi-sign-stop:before{content:""}.bi-sign-turn-left-fill:before{content:""}.bi-sign-turn-left:before{content:""}.bi-sign-turn-right-fill:before{content:""}.bi-sign-turn-right:before{content:""}.bi-sign-turn-slight-left-fill:before{content:""}.bi-sign-turn-slight-left:before{content:""}.bi-sign-turn-slight-right-fill:before{content:""}.bi-sign-turn-slight-right:before{content:""}.bi-sign-yield-fill:before{content:""}.bi-sign-yield:before{content:""}.bi-ev-station-fill:before{content:""}.bi-ev-station:before{content:""}.bi-fuel-pump-diesel-fill:before{content:""}.bi-fuel-pump-diesel:before{content:""}.bi-fuel-pump-fill:before{content:""}.bi-fuel-pump:before{content:""}.bi-0-circle-fill:before{content:""}.bi-0-circle:before{content:""}.bi-0-square-fill:before{content:""}.bi-0-square:before{content:""}.bi-rocket-fill:before{content:""}.bi-rocket-takeoff-fill:before{content:""}.bi-rocket-takeoff:before{content:""}.bi-rocket:before{content:""}.bi-stripe:before{content:""}.bi-subscript:before{content:""}.bi-superscript:before{content:""}.bi-trello:before{content:""}.bi-envelope-at-fill:before{content:""}.bi-envelope-at:before{content:""}.bi-regex:before{content:""}.bi-text-wrap:before{content:""}.bi-sign-dead-end-fill:before{content:""}.bi-sign-dead-end:before{content:""}.bi-sign-do-not-enter-fill:before{content:""}.bi-sign-do-not-enter:before{content:""}.bi-sign-intersection-fill:before{content:""}.bi-sign-intersection-side-fill:before{content:""}.bi-sign-intersection-side:before{content:""}.bi-sign-intersection-t-fill:before{content:""}.bi-sign-intersection-t:before{content:""}.bi-sign-intersection-y-fill:before{content:""}.bi-sign-intersection-y:before{content:""}.bi-sign-intersection:before{content:""}.bi-sign-merge-left-fill:before{content:""}.bi-sign-merge-left:before{content:""}.bi-sign-merge-right-fill:before{content:""}.bi-sign-merge-right:before{content:""}.bi-sign-no-left-turn-fill:before{content:""}.bi-sign-no-left-turn:before{content:""}.bi-sign-no-parking-fill:before{content:""}.bi-sign-no-parking:before{content:""}.bi-sign-no-right-turn-fill:before{content:""}.bi-sign-no-right-turn:before{content:""}.bi-sign-railroad-fill:before{content:""}.bi-sign-railroad:before{content:""}.bi-building-add:before{content:""}.bi-building-check:before{content:""}.bi-building-dash:before{content:""}.bi-building-down:before{content:""}.bi-building-exclamation:before{content:""}.bi-building-fill-add:before{content:""}.bi-building-fill-check:before{content:""}.bi-building-fill-dash:before{content:""}.bi-building-fill-down:before{content:""}.bi-building-fill-exclamation:before{content:""}.bi-building-fill-gear:before{content:""}.bi-building-fill-lock:before{content:""}.bi-building-fill-slash:before{content:""}.bi-building-fill-up:before{content:""}.bi-building-fill-x:before{content:""}.bi-building-fill:before{content:""}.bi-building-gear:before{content:""}.bi-building-lock:before{content:""}.bi-building-slash:before{content:""}.bi-building-up:before{content:""}.bi-building-x:before{content:""}.bi-buildings-fill:before{content:""}.bi-buildings:before{content:""}.bi-bus-front-fill:before{content:""}.bi-bus-front:before{content:""}.bi-ev-front-fill:before{content:""}.bi-ev-front:before{content:""}.bi-globe-americas:before{content:""}.bi-globe-asia-australia:before{content:""}.bi-globe-central-south-asia:before{content:""}.bi-globe-europe-africa:before{content:""}.bi-house-add-fill:before{content:""}.bi-house-add:before{content:""}.bi-house-check-fill:before{content:""}.bi-house-check:before{content:""}.bi-house-dash-fill:before{content:""}.bi-house-dash:before{content:""}.bi-house-down-fill:before{content:""}.bi-house-down:before{content:""}.bi-house-exclamation-fill:before{content:""}.bi-house-exclamation:before{content:""}.bi-house-gear-fill:before{content:""}.bi-house-gear:before{content:""}.bi-house-lock-fill:before{content:""}.bi-house-lock:before{content:""}.bi-house-slash-fill:before{content:""}.bi-house-slash:before{content:""}.bi-house-up-fill:before{content:""}.bi-house-up:before{content:""}.bi-house-x-fill:before{content:""}.bi-house-x:before{content:""}.bi-person-add:before{content:""}.bi-person-down:before{content:""}.bi-person-exclamation:before{content:""}.bi-person-fill-add:before{content:""}.bi-person-fill-check:before{content:""}.bi-person-fill-dash:before{content:""}.bi-person-fill-down:before{content:""}.bi-person-fill-exclamation:before{content:""}.bi-person-fill-gear:before{content:""}.bi-person-fill-lock:before{content:""}.bi-person-fill-slash:before{content:""}.bi-person-fill-up:before{content:""}.bi-person-fill-x:before{content:""}.bi-person-gear:before{content:""}.bi-person-lock:before{content:""}.bi-person-slash:before{content:""}.bi-person-up:before{content:""}.bi-scooter:before{content:""}.bi-taxi-front-fill:before{content:""}.bi-taxi-front:before{content:""}.bi-amd:before{content:""}.bi-database-add:before{content:""}.bi-database-check:before{content:""}.bi-database-dash:before{content:""}.bi-database-down:before{content:""}.bi-database-exclamation:before{content:""}.bi-database-fill-add:before{content:""}.bi-database-fill-check:before{content:""}.bi-database-fill-dash:before{content:""}.bi-database-fill-down:before{content:""}.bi-database-fill-exclamation:before{content:""}.bi-database-fill-gear:before{content:""}.bi-database-fill-lock:before{content:""}.bi-database-fill-slash:before{content:""}.bi-database-fill-up:before{content:""}.bi-database-fill-x:before{content:""}.bi-database-fill:before{content:""}.bi-database-gear:before{content:""}.bi-database-lock:before{content:""}.bi-database-slash:before{content:""}.bi-database-up:before{content:""}.bi-database-x:before{content:""}.bi-database:before{content:""}.bi-houses-fill:before{content:""}.bi-houses:before{content:""}.bi-nvidia:before{content:""}.bi-person-vcard-fill:before{content:""}.bi-person-vcard:before{content:""}.bi-sina-weibo:before{content:""}.bi-tencent-qq:before{content:""}.bi-wikipedia:before{content:""}.bi-alphabet-uppercase:before{content:""}.bi-alphabet:before{content:""}.bi-amazon:before{content:""}.bi-arrows-collapse-vertical:before{content:""}.bi-arrows-expand-vertical:before{content:""}.bi-arrows-vertical:before{content:""}.bi-arrows:before{content:""}.bi-ban-fill:before{content:""}.bi-ban:before{content:""}.bi-bing:before{content:""}.bi-cake:before{content:""}.bi-cake2:before{content:""}.bi-cookie:before{content:""}.bi-copy:before{content:""}.bi-crosshair:before{content:""}.bi-crosshair2:before{content:""}.bi-emoji-astonished-fill:before{content:""}.bi-emoji-astonished:before{content:""}.bi-emoji-grimace-fill:before{content:""}.bi-emoji-grimace:before{content:""}.bi-emoji-grin-fill:before{content:""}.bi-emoji-grin:before{content:""}.bi-emoji-surprise-fill:before{content:""}.bi-emoji-surprise:before{content:""}.bi-emoji-tear-fill:before{content:""}.bi-emoji-tear:before{content:""}.bi-envelope-arrow-down-fill:before{content:""}.bi-envelope-arrow-down:before{content:""}.bi-envelope-arrow-up-fill:before{content:""}.bi-envelope-arrow-up:before{content:""}.bi-feather:before{content:""}.bi-feather2:before{content:""}.bi-floppy-fill:before{content:""}.bi-floppy:before{content:""}.bi-floppy2-fill:before{content:""}.bi-floppy2:before{content:""}.bi-gitlab:before{content:""}.bi-highlighter:before{content:""}.bi-marker-tip:before{content:""}.bi-nvme-fill:before{content:""}.bi-nvme:before{content:""}.bi-opencollective:before{content:""}.bi-pci-card-network:before{content:""}.bi-pci-card-sound:before{content:""}.bi-radar:before{content:""}.bi-send-arrow-down-fill:before{content:""}.bi-send-arrow-down:before{content:""}.bi-send-arrow-up-fill:before{content:""}.bi-send-arrow-up:before{content:""}.bi-sim-slash-fill:before{content:""}.bi-sim-slash:before{content:""}.bi-sourceforge:before{content:""}.bi-substack:before{content:""}.bi-threads-fill:before{content:""}.bi-threads:before{content:""}.bi-transparency:before{content:""}.bi-twitter-x:before{content:""}.bi-type-h4:before{content:""}.bi-type-h5:before{content:""}.bi-type-h6:before{content:""}.bi-backpack-fill:before{content:""}.bi-backpack:before{content:""}.bi-backpack2-fill:before{content:""}.bi-backpack2:before{content:""}.bi-backpack3-fill:before{content:""}.bi-backpack3:before{content:""}.bi-backpack4-fill:before{content:""}.bi-backpack4:before{content:""}.bi-brilliance:before{content:""}.bi-cake-fill:before{content:""}.bi-cake2-fill:before{content:""}.bi-duffle-fill:before{content:""}.bi-duffle:before{content:""}.bi-exposure:before{content:""}.bi-gender-neuter:before{content:""}.bi-highlights:before{content:""}.bi-luggage-fill:before{content:""}.bi-luggage:before{content:""}.bi-mailbox-flag:before{content:""}.bi-mailbox2-flag:before{content:""}.bi-noise-reduction:before{content:""}.bi-passport-fill:before{content:""}.bi-passport:before{content:""}.bi-person-arms-up:before{content:""}.bi-person-raised-hand:before{content:""}.bi-person-standing-dress:before{content:""}.bi-person-standing:before{content:""}.bi-person-walking:before{content:""}.bi-person-wheelchair:before{content:""}.bi-shadows:before{content:""}.bi-suitcase-fill:before{content:""}.bi-suitcase-lg-fill:before{content:""}.bi-suitcase-lg:before{content:""}.bi-suitcase:before{content:"豈"}.bi-suitcase2-fill:before{content:"更"}.bi-suitcase2:before{content:"車"}.bi-vignette:before{content:"賈"}.pvtUi{color:#333}table.pvtTable{font-size:8pt;text-align:left;border-collapse:collapse}table.pvtTable thead tr th,table.pvtTable tbody tr th{background-color:#e6eeee;border:1px solid #CDCDCD;font-size:8pt;padding:5px}table.pvtTable .pvtColLabel{text-align:center}table.pvtTable .pvtTotalLabel{text-align:right}table.pvtTable tbody tr td{color:#3d3d3d;padding:5px;background-color:#fff;border:1px solid #CDCDCD;vertical-align:top;text-align:right}.pvtTotal,.pvtGrandTotal{font-weight:700}.pvtVals{text-align:center;white-space:nowrap}.pvtRowOrder,.pvtColOrder{cursor:pointer;width:15px;margin-left:5px;display:inline-block}.pvtAggregator{margin-bottom:5px}.pvtAxisContainer,.pvtVals{border:1px solid gray;background:#eee;padding:5px;min-width:20px;min-height:20px;user-select:none;-webkit-user-select:none;-moz-user-select:none;-khtml-user-select:none;-ms-user-select:none}.pvtAxisContainer li{padding:8px 6px;list-style-type:none;cursor:move}.pvtAxisContainer li.pvtPlaceholder{-webkit-border-radius:5px;padding:3px 15px;-moz-border-radius:5px;border-radius:5px;border:1px dashed #aaa}.pvtAxisContainer li span.pvtAttr{-webkit-text-size-adjust:100%;background:#f3f3f3;border:1px solid #DEDEDE;padding:2px 5px;white-space:nowrap;-webkit-border-radius:5px;-moz-border-radius:5px;border-radius:5px}.pvtTriangle{cursor:pointer;color:gray}.pvtHorizList li{display:inline}.pvtVertList{vertical-align:top}.pvtFilteredAttribute{font-style:italic}.pvtFilterBox{z-index:100;width:300px;border:1px solid gray;background-color:#fff;position:absolute;text-align:center}.pvtFilterBox h4{margin:15px}.pvtFilterBox p{margin:10px auto}.pvtFilterBox label{font-weight:400}.pvtFilterBox input[type=checkbox]{margin-right:10px;margin-left:10px}.pvtFilterBox input[type=text]{width:230px}.pvtFilterBox .count{color:gray;font-weight:400;margin-left:3px}.pvtCheckContainer{text-align:left;font-size:14px;white-space:nowrap;overflow-y:scroll;width:100%;max-height:250px;border-top:1px solid lightgrey;border-bottom:1px solid lightgrey}.pvtCheckContainer p{margin:5px}.pvtRendererArea{padding:5px}:root,[data-bs-theme=light]{--bs-blue: #0d6efd;--bs-indigo: #6610f2;--bs-purple: #6f42c1;--bs-pink: #d63384;--bs-red: #dc3545;--bs-orange: #fd7e14;--bs-yellow: #ffc107;--bs-green: #198754;--bs-teal: #20c997;--bs-cyan: #0dcaf0;--bs-black: #000;--bs-white: #fff;--bs-gray: #6c757d;--bs-gray-dark: #343a40;--bs-gray-100: #f8f9fa;--bs-gray-200: #e9ecef;--bs-gray-300: #dee2e6;--bs-gray-400: #ced4da;--bs-gray-500: #adb5bd;--bs-gray-600: #6c757d;--bs-gray-700: #495057;--bs-gray-800: #343a40;--bs-gray-900: #212529;--bs-primary: #0d6efd;--bs-secondary: #6c757d;--bs-success: #198754;--bs-info: #0dcaf0;--bs-warning: #ffc107;--bs-danger: #dc3545;--bs-light: #f8f9fa;--bs-dark: #212529;--bs-primary-rgb: 13, 110, 253;--bs-secondary-rgb: 108, 117, 125;--bs-success-rgb: 25, 135, 84;--bs-info-rgb: 13, 202, 240;--bs-warning-rgb: 255, 193, 7;--bs-danger-rgb: 220, 53, 69;--bs-light-rgb: 248, 249, 250;--bs-dark-rgb: 33, 37, 41;--bs-primary-text-emphasis: #052c65;--bs-secondary-text-emphasis: #2b2f32;--bs-success-text-emphasis: #0a3622;--bs-info-text-emphasis: #055160;--bs-warning-text-emphasis: #664d03;--bs-danger-text-emphasis: #58151c;--bs-light-text-emphasis: #495057;--bs-dark-text-emphasis: #495057;--bs-primary-bg-subtle: #cfe2ff;--bs-secondary-bg-subtle: #e2e3e5;--bs-success-bg-subtle: #d1e7dd;--bs-info-bg-subtle: #cff4fc;--bs-warning-bg-subtle: #fff3cd;--bs-danger-bg-subtle: #f8d7da;--bs-light-bg-subtle: #fcfcfd;--bs-dark-bg-subtle: #ced4da;--bs-primary-border-subtle: #9ec5fe;--bs-secondary-border-subtle: #c4c8cb;--bs-success-border-subtle: #a3cfbb;--bs-info-border-subtle: #9eeaf9;--bs-warning-border-subtle: #ffe69c;--bs-danger-border-subtle: #f1aeb5;--bs-light-border-subtle: #e9ecef;--bs-dark-border-subtle: #adb5bd;--bs-white-rgb: 255, 255, 255;--bs-black-rgb: 0, 0, 0;--bs-font-sans-serif: system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", "Liberation Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";--bs-font-monospace: SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;--bs-gradient: linear-gradient(180deg, rgba(255, 255, 255, .15), rgba(255, 255, 255, 0));--bs-body-font-family: var(--bs-font-sans-serif);--bs-body-font-size: 1rem;--bs-body-font-weight: 400;--bs-body-line-height: 1.5;--bs-body-color: #212529;--bs-body-color-rgb: 33, 37, 41;--bs-body-bg: #fff;--bs-body-bg-rgb: 255, 255, 255;--bs-emphasis-color: #000;--bs-emphasis-color-rgb: 0, 0, 0;--bs-secondary-color: rgba(33, 37, 41, .75);--bs-secondary-color-rgb: 33, 37, 41;--bs-secondary-bg: #e9ecef;--bs-secondary-bg-rgb: 233, 236, 239;--bs-tertiary-color: rgba(33, 37, 41, .5);--bs-tertiary-color-rgb: 33, 37, 41;--bs-tertiary-bg: #f8f9fa;--bs-tertiary-bg-rgb: 248, 249, 250;--bs-heading-color: inherit;--bs-link-color: #0d6efd;--bs-link-color-rgb: 13, 110, 253;--bs-link-decoration: underline;--bs-link-hover-color: #0a58ca;--bs-link-hover-color-rgb: 10, 88, 202;--bs-code-color: #d63384;--bs-highlight-color: #212529;--bs-highlight-bg: #fff3cd;--bs-border-width: 1px;--bs-border-style: solid;--bs-border-color: #dee2e6;--bs-border-color-translucent: rgba(0, 0, 0, .175);--bs-border-radius: .375rem;--bs-border-radius-sm: .25rem;--bs-border-radius-lg: .5rem;--bs-border-radius-xl: 1rem;--bs-border-radius-xxl: 2rem;--bs-border-radius-2xl: var(--bs-border-radius-xxl);--bs-border-radius-pill: 50rem;--bs-box-shadow: 0 .5rem 1rem rgba(0, 0, 0, .15);--bs-box-shadow-sm: 0 .125rem .25rem rgba(0, 0, 0, .075);--bs-box-shadow-lg: 0 1rem 3rem rgba(0, 0, 0, .175);--bs-box-shadow-inset: inset 0 1px 2px rgba(0, 0, 0, .075);--bs-focus-ring-width: .25rem;--bs-focus-ring-opacity: .25;--bs-focus-ring-color: rgba(13, 110, 253, .25);--bs-form-valid-color: #198754;--bs-form-valid-border-color: #198754;--bs-form-invalid-color: #dc3545;--bs-form-invalid-border-color: #dc3545}[data-bs-theme=dark]{color-scheme:dark;--bs-body-color: #dee2e6;--bs-body-color-rgb: 222, 226, 230;--bs-body-bg: #212529;--bs-body-bg-rgb: 33, 37, 41;--bs-emphasis-color: #fff;--bs-emphasis-color-rgb: 255, 255, 255;--bs-secondary-color: rgba(222, 226, 230, .75);--bs-secondary-color-rgb: 222, 226, 230;--bs-secondary-bg: #343a40;--bs-secondary-bg-rgb: 52, 58, 64;--bs-tertiary-color: rgba(222, 226, 230, .5);--bs-tertiary-color-rgb: 222, 226, 230;--bs-tertiary-bg: #2b3035;--bs-tertiary-bg-rgb: 43, 48, 53;--bs-primary-text-emphasis: #6ea8fe;--bs-secondary-text-emphasis: #a7acb1;--bs-success-text-emphasis: #75b798;--bs-info-text-emphasis: #6edff6;--bs-warning-text-emphasis: #ffda6a;--bs-danger-text-emphasis: #ea868f;--bs-light-text-emphasis: #f8f9fa;--bs-dark-text-emphasis: #dee2e6;--bs-primary-bg-subtle: #031633;--bs-secondary-bg-subtle: #161719;--bs-success-bg-subtle: #051b11;--bs-info-bg-subtle: #032830;--bs-warning-bg-subtle: #332701;--bs-danger-bg-subtle: #2c0b0e;--bs-light-bg-subtle: #343a40;--bs-dark-bg-subtle: #1a1d20;--bs-primary-border-subtle: #084298;--bs-secondary-border-subtle: #41464b;--bs-success-border-subtle: #0f5132;--bs-info-border-subtle: #087990;--bs-warning-border-subtle: #997404;--bs-danger-border-subtle: #842029;--bs-light-border-subtle: #495057;--bs-dark-border-subtle: #343a40;--bs-heading-color: inherit;--bs-link-color: #6ea8fe;--bs-link-hover-color: #8bb9fe;--bs-link-color-rgb: 110, 168, 254;--bs-link-hover-color-rgb: 139, 185, 254;--bs-code-color: #e685b5;--bs-highlight-color: #dee2e6;--bs-highlight-bg: #664d03;--bs-border-color: #495057;--bs-border-color-translucent: rgba(255, 255, 255, .15);--bs-form-valid-color: #75b798;--bs-form-valid-border-color: #75b798;--bs-form-invalid-color: #ea868f;--bs-form-invalid-border-color: #ea868f}*,*:before,*:after{box-sizing:border-box}@media (prefers-reduced-motion: no-preference){:root{scroll-behavior:smooth}}body{margin:0;font-family:var(--bs-body-font-family);font-size:var(--bs-body-font-size);font-weight:var(--bs-body-font-weight);line-height:var(--bs-body-line-height);color:var(--bs-body-color);text-align:var(--bs-body-text-align);background-color:var(--bs-body-bg);-webkit-text-size-adjust:100%;-webkit-tap-highlight-color:rgba(0,0,0,0)}hr{margin:1rem 0;color:inherit;border:0;border-top:var(--bs-border-width) solid;opacity:.25}h6,.h6,h5,.h5,h4,.h4,h3,.h3,h2,.h2,h1,.h1{margin-top:0;margin-bottom:.5rem;font-weight:500;line-height:1.2;color:var(--bs-heading-color)}h1,.h1{font-size:calc(1.375rem + 1.5vw)}@media (min-width: 1200px){h1,.h1{font-size:2.5rem}}h2,.h2{font-size:calc(1.325rem + .9vw)}@media (min-width: 1200px){h2,.h2{font-size:2rem}}h3,.h3{font-size:calc(1.3rem + .6vw)}@media (min-width: 1200px){h3,.h3{font-size:1.75rem}}h4,.h4{font-size:calc(1.275rem + .3vw)}@media (min-width: 1200px){h4,.h4{font-size:1.5rem}}h5,.h5{font-size:1.25rem}h6,.h6{font-size:1rem}p{margin-top:0;margin-bottom:1rem}abbr[title]{text-decoration:underline dotted;cursor:help;text-decoration-skip-ink:none}address{margin-bottom:1rem;font-style:normal;line-height:inherit}ol,ul{padding-left:2rem}ol,ul,dl{margin-top:0;margin-bottom:1rem}ol ol,ul ul,ol ul,ul ol{margin-bottom:0}dt{font-weight:700}dd{margin-bottom:.5rem;margin-left:0}blockquote{margin:0 0 1rem}b,strong{font-weight:bolder}small,.small{font-size:.875em}mark,.mark{padding:.1875em;color:var(--bs-highlight-color);background-color:var(--bs-highlight-bg)}sub,sup{position:relative;font-size:.75em;line-height:0;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}a{color:rgba(var(--bs-link-color-rgb),var(--bs-link-opacity, 1));text-decoration:underline}a:hover{--bs-link-color-rgb: var(--bs-link-hover-color-rgb)}a:not([href]):not([class]),a:not([href]):not([class]):hover{color:inherit;text-decoration:none}pre,code,kbd,samp{font-family:var(--bs-font-monospace);font-size:1em}pre{display:block;margin-top:0;margin-bottom:1rem;overflow:auto;font-size:.875em}pre code{font-size:inherit;color:inherit;word-break:normal}code{font-size:.875em;color:var(--bs-code-color);word-wrap:break-word}a>code{color:inherit}kbd{padding:.1875rem .375rem;font-size:.875em;color:var(--bs-body-bg);background-color:var(--bs-body-color);border-radius:.25rem}kbd kbd{padding:0;font-size:1em}figure{margin:0 0 1rem}img,svg{vertical-align:middle}table{caption-side:bottom;border-collapse:collapse}caption{padding-top:.5rem;padding-bottom:.5rem;color:var(--bs-secondary-color);text-align:left}th{text-align:inherit;text-align:-webkit-match-parent}thead,tbody,tfoot,tr,td,th{border-color:inherit;border-style:solid;border-width:0}label{display:inline-block}button{border-radius:0}button:focus:not(:focus-visible){outline:0}input,button,select,optgroup,textarea{margin:0;font-family:inherit;font-size:inherit;line-height:inherit}button,select{text-transform:none}[role=button]{cursor:pointer}select{word-wrap:normal}select:disabled{opacity:1}[list]:not([type=date]):not([type=datetime-local]):not([type=month]):not([type=week]):not([type=time])::-webkit-calendar-picker-indicator{display:none!important}button,[type=button],[type=reset],[type=submit]{-webkit-appearance:button}button:not(:disabled),[type=button]:not(:disabled),[type=reset]:not(:disabled),[type=submit]:not(:disabled){cursor:pointer}::-moz-focus-inner{padding:0;border-style:none}textarea{resize:vertical}fieldset{min-width:0;padding:0;margin:0;border:0}legend{float:left;width:100%;padding:0;margin-bottom:.5rem;font-size:calc(1.275rem + .3vw);line-height:inherit}@media (min-width: 1200px){legend{font-size:1.5rem}}legend+*{clear:left}::-webkit-datetime-edit-fields-wrapper,::-webkit-datetime-edit-text,::-webkit-datetime-edit-minute,::-webkit-datetime-edit-hour-field,::-webkit-datetime-edit-day-field,::-webkit-datetime-edit-month-field,::-webkit-datetime-edit-year-field{padding:0}::-webkit-inner-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-color-swatch-wrapper{padding:0}::file-selector-button{font:inherit;-webkit-appearance:button}output{display:inline-block}iframe{border:0}summary{display:list-item;cursor:pointer}progress{vertical-align:baseline}[hidden]{display:none!important}.lead{font-size:1.25rem;font-weight:300}.display-1{font-size:calc(1.625rem + 4.5vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-1{font-size:5rem}}.display-2{font-size:calc(1.575rem + 3.9vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-2{font-size:4.5rem}}.display-3{font-size:calc(1.525rem + 3.3vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-3{font-size:4rem}}.display-4{font-size:calc(1.475rem + 2.7vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-4{font-size:3.5rem}}.display-5{font-size:calc(1.425rem + 2.1vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-5{font-size:3rem}}.display-6{font-size:calc(1.375rem + 1.5vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-6{font-size:2.5rem}}.list-unstyled,.list-inline{padding-left:0;list-style:none}.list-inline-item{display:inline-block}.list-inline-item:not(:last-child){margin-right:.5rem}.initialism{font-size:.875em;text-transform:uppercase}.blockquote{margin-bottom:1rem;font-size:1.25rem}.blockquote>:last-child{margin-bottom:0}.blockquote-footer{margin-top:-1rem;margin-bottom:1rem;font-size:.875em;color:#6c757d}.blockquote-footer:before{content:"— "}.img-fluid{max-width:100%;height:auto}.img-thumbnail{padding:.25rem;background-color:var(--bs-body-bg);border:var(--bs-border-width) solid var(--bs-border-color);border-radius:var(--bs-border-radius);max-width:100%;height:auto}.figure{display:inline-block}.figure-img{margin-bottom:.5rem;line-height:1}.figure-caption{font-size:.875em;color:var(--bs-secondary-color)}.container,.container-fluid,.container-xxl,.container-xl,.container-lg,.container-md,.container-sm{--bs-gutter-x: 1.5rem;--bs-gutter-y: 0;width:100%;padding-right:calc(var(--bs-gutter-x) * .5);padding-left:calc(var(--bs-gutter-x) * .5);margin-right:auto;margin-left:auto}@media (min-width: 576px){.container-sm,.container{max-width:540px}}@media (min-width: 768px){.container-md,.container-sm,.container{max-width:720px}}@media (min-width: 992px){.container-lg,.container-md,.container-sm,.container{max-width:960px}}@media (min-width: 1200px){.container-xl,.container-lg,.container-md,.container-sm,.container{max-width:1140px}}@media (min-width: 1400px){.container-xxl,.container-xl,.container-lg,.container-md,.container-sm,.container{max-width:1320px}}:root{--bs-breakpoint-xs: 0;--bs-breakpoint-sm: 576px;--bs-breakpoint-md: 768px;--bs-breakpoint-lg: 992px;--bs-breakpoint-xl: 1200px;--bs-breakpoint-xxl: 1400px}.row{--bs-gutter-x: 1.5rem;--bs-gutter-y: 0;display:flex;flex-wrap:wrap;margin-top:calc(-1 * var(--bs-gutter-y));margin-right:calc(-.5 * var(--bs-gutter-x));margin-left:calc(-.5 * var(--bs-gutter-x))}.row>*{flex-shrink:0;width:100%;max-width:100%;padding-right:calc(var(--bs-gutter-x) * .5);padding-left:calc(var(--bs-gutter-x) * .5);margin-top:var(--bs-gutter-y)}.col{flex:1 0 0%}.row-cols-auto>*{flex:0 0 auto;width:auto}.row-cols-1>*{flex:0 0 auto;width:100%}.row-cols-2>*{flex:0 0 auto;width:50%}.row-cols-3>*{flex:0 0 auto;width:33.33333333%}.row-cols-4>*{flex:0 0 auto;width:25%}.row-cols-5>*{flex:0 0 auto;width:20%}.row-cols-6>*{flex:0 0 auto;width:16.66666667%}.col-auto{flex:0 0 auto;width:auto}.col-1{flex:0 0 auto;width:8.33333333%}.col-2{flex:0 0 auto;width:16.66666667%}.col-3{flex:0 0 auto;width:25%}.col-4{flex:0 0 auto;width:33.33333333%}.col-5{flex:0 0 auto;width:41.66666667%}.col-6{flex:0 0 auto;width:50%}.col-7{flex:0 0 auto;width:58.33333333%}.col-8{flex:0 0 auto;width:66.66666667%}.col-9{flex:0 0 auto;width:75%}.col-10{flex:0 0 auto;width:83.33333333%}.col-11{flex:0 0 auto;width:91.66666667%}.col-12{flex:0 0 auto;width:100%}.offset-1{margin-left:8.33333333%}.offset-2{margin-left:16.66666667%}.offset-3{margin-left:25%}.offset-4{margin-left:33.33333333%}.offset-5{margin-left:41.66666667%}.offset-6{margin-left:50%}.offset-7{margin-left:58.33333333%}.offset-8{margin-left:66.66666667%}.offset-9{margin-left:75%}.offset-10{margin-left:83.33333333%}.offset-11{margin-left:91.66666667%}.g-0,.gx-0{--bs-gutter-x: 0}.g-0,.gy-0{--bs-gutter-y: 0}.g-1,.gx-1{--bs-gutter-x: .25rem}.g-1,.gy-1{--bs-gutter-y: .25rem}.g-2,.gx-2{--bs-gutter-x: .5rem}.g-2,.gy-2{--bs-gutter-y: .5rem}.g-3,.gx-3{--bs-gutter-x: 1rem}.g-3,.gy-3{--bs-gutter-y: 1rem}.g-4,.gx-4{--bs-gutter-x: 1.5rem}.g-4,.gy-4{--bs-gutter-y: 1.5rem}.g-5,.gx-5{--bs-gutter-x: 3rem}.g-5,.gy-5{--bs-gutter-y: 3rem}@media (min-width: 576px){.col-sm{flex:1 0 0%}.row-cols-sm-auto>*{flex:0 0 auto;width:auto}.row-cols-sm-1>*{flex:0 0 auto;width:100%}.row-cols-sm-2>*{flex:0 0 auto;width:50%}.row-cols-sm-3>*{flex:0 0 auto;width:33.33333333%}.row-cols-sm-4>*{flex:0 0 auto;width:25%}.row-cols-sm-5>*{flex:0 0 auto;width:20%}.row-cols-sm-6>*{flex:0 0 auto;width:16.66666667%}.col-sm-auto{flex:0 0 auto;width:auto}.col-sm-1{flex:0 0 auto;width:8.33333333%}.col-sm-2{flex:0 0 auto;width:16.66666667%}.col-sm-3{flex:0 0 auto;width:25%}.col-sm-4{flex:0 0 auto;width:33.33333333%}.col-sm-5{flex:0 0 auto;width:41.66666667%}.col-sm-6{flex:0 0 auto;width:50%}.col-sm-7{flex:0 0 auto;width:58.33333333%}.col-sm-8{flex:0 0 auto;width:66.66666667%}.col-sm-9{flex:0 0 auto;width:75%}.col-sm-10{flex:0 0 auto;width:83.33333333%}.col-sm-11{flex:0 0 auto;width:91.66666667%}.col-sm-12{flex:0 0 auto;width:100%}.offset-sm-0{margin-left:0}.offset-sm-1{margin-left:8.33333333%}.offset-sm-2{margin-left:16.66666667%}.offset-sm-3{margin-left:25%}.offset-sm-4{margin-left:33.33333333%}.offset-sm-5{margin-left:41.66666667%}.offset-sm-6{margin-left:50%}.offset-sm-7{margin-left:58.33333333%}.offset-sm-8{margin-left:66.66666667%}.offset-sm-9{margin-left:75%}.offset-sm-10{margin-left:83.33333333%}.offset-sm-11{margin-left:91.66666667%}.g-sm-0,.gx-sm-0{--bs-gutter-x: 0}.g-sm-0,.gy-sm-0{--bs-gutter-y: 0}.g-sm-1,.gx-sm-1{--bs-gutter-x: .25rem}.g-sm-1,.gy-sm-1{--bs-gutter-y: .25rem}.g-sm-2,.gx-sm-2{--bs-gutter-x: .5rem}.g-sm-2,.gy-sm-2{--bs-gutter-y: .5rem}.g-sm-3,.gx-sm-3{--bs-gutter-x: 1rem}.g-sm-3,.gy-sm-3{--bs-gutter-y: 1rem}.g-sm-4,.gx-sm-4{--bs-gutter-x: 1.5rem}.g-sm-4,.gy-sm-4{--bs-gutter-y: 1.5rem}.g-sm-5,.gx-sm-5{--bs-gutter-x: 3rem}.g-sm-5,.gy-sm-5{--bs-gutter-y: 3rem}}@media (min-width: 768px){.col-md{flex:1 0 0%}.row-cols-md-auto>*{flex:0 0 auto;width:auto}.row-cols-md-1>*{flex:0 0 auto;width:100%}.row-cols-md-2>*{flex:0 0 auto;width:50%}.row-cols-md-3>*{flex:0 0 auto;width:33.33333333%}.row-cols-md-4>*{flex:0 0 auto;width:25%}.row-cols-md-5>*{flex:0 0 auto;width:20%}.row-cols-md-6>*{flex:0 0 auto;width:16.66666667%}.col-md-auto{flex:0 0 auto;width:auto}.col-md-1{flex:0 0 auto;width:8.33333333%}.col-md-2{flex:0 0 auto;width:16.66666667%}.col-md-3{flex:0 0 auto;width:25%}.col-md-4{flex:0 0 auto;width:33.33333333%}.col-md-5{flex:0 0 auto;width:41.66666667%}.col-md-6{flex:0 0 auto;width:50%}.col-md-7{flex:0 0 auto;width:58.33333333%}.col-md-8{flex:0 0 auto;width:66.66666667%}.col-md-9{flex:0 0 auto;width:75%}.col-md-10{flex:0 0 auto;width:83.33333333%}.col-md-11{flex:0 0 auto;width:91.66666667%}.col-md-12{flex:0 0 auto;width:100%}.offset-md-0{margin-left:0}.offset-md-1{margin-left:8.33333333%}.offset-md-2{margin-left:16.66666667%}.offset-md-3{margin-left:25%}.offset-md-4{margin-left:33.33333333%}.offset-md-5{margin-left:41.66666667%}.offset-md-6{margin-left:50%}.offset-md-7{margin-left:58.33333333%}.offset-md-8{margin-left:66.66666667%}.offset-md-9{margin-left:75%}.offset-md-10{margin-left:83.33333333%}.offset-md-11{margin-left:91.66666667%}.g-md-0,.gx-md-0{--bs-gutter-x: 0}.g-md-0,.gy-md-0{--bs-gutter-y: 0}.g-md-1,.gx-md-1{--bs-gutter-x: .25rem}.g-md-1,.gy-md-1{--bs-gutter-y: .25rem}.g-md-2,.gx-md-2{--bs-gutter-x: .5rem}.g-md-2,.gy-md-2{--bs-gutter-y: .5rem}.g-md-3,.gx-md-3{--bs-gutter-x: 1rem}.g-md-3,.gy-md-3{--bs-gutter-y: 1rem}.g-md-4,.gx-md-4{--bs-gutter-x: 1.5rem}.g-md-4,.gy-md-4{--bs-gutter-y: 1.5rem}.g-md-5,.gx-md-5{--bs-gutter-x: 3rem}.g-md-5,.gy-md-5{--bs-gutter-y: 3rem}}@media (min-width: 992px){.col-lg{flex:1 0 0%}.row-cols-lg-auto>*{flex:0 0 auto;width:auto}.row-cols-lg-1>*{flex:0 0 auto;width:100%}.row-cols-lg-2>*{flex:0 0 auto;width:50%}.row-cols-lg-3>*{flex:0 0 auto;width:33.33333333%}.row-cols-lg-4>*{flex:0 0 auto;width:25%}.row-cols-lg-5>*{flex:0 0 auto;width:20%}.row-cols-lg-6>*{flex:0 0 auto;width:16.66666667%}.col-lg-auto{flex:0 0 auto;width:auto}.col-lg-1{flex:0 0 auto;width:8.33333333%}.col-lg-2{flex:0 0 auto;width:16.66666667%}.col-lg-3{flex:0 0 auto;width:25%}.col-lg-4{flex:0 0 auto;width:33.33333333%}.col-lg-5{flex:0 0 auto;width:41.66666667%}.col-lg-6{flex:0 0 auto;width:50%}.col-lg-7{flex:0 0 auto;width:58.33333333%}.col-lg-8{flex:0 0 auto;width:66.66666667%}.col-lg-9{flex:0 0 auto;width:75%}.col-lg-10{flex:0 0 auto;width:83.33333333%}.col-lg-11{flex:0 0 auto;width:91.66666667%}.col-lg-12{flex:0 0 auto;width:100%}.offset-lg-0{margin-left:0}.offset-lg-1{margin-left:8.33333333%}.offset-lg-2{margin-left:16.66666667%}.offset-lg-3{margin-left:25%}.offset-lg-4{margin-left:33.33333333%}.offset-lg-5{margin-left:41.66666667%}.offset-lg-6{margin-left:50%}.offset-lg-7{margin-left:58.33333333%}.offset-lg-8{margin-left:66.66666667%}.offset-lg-9{margin-left:75%}.offset-lg-10{margin-left:83.33333333%}.offset-lg-11{margin-left:91.66666667%}.g-lg-0,.gx-lg-0{--bs-gutter-x: 0}.g-lg-0,.gy-lg-0{--bs-gutter-y: 0}.g-lg-1,.gx-lg-1{--bs-gutter-x: .25rem}.g-lg-1,.gy-lg-1{--bs-gutter-y: .25rem}.g-lg-2,.gx-lg-2{--bs-gutter-x: .5rem}.g-lg-2,.gy-lg-2{--bs-gutter-y: .5rem}.g-lg-3,.gx-lg-3{--bs-gutter-x: 1rem}.g-lg-3,.gy-lg-3{--bs-gutter-y: 1rem}.g-lg-4,.gx-lg-4{--bs-gutter-x: 1.5rem}.g-lg-4,.gy-lg-4{--bs-gutter-y: 1.5rem}.g-lg-5,.gx-lg-5{--bs-gutter-x: 3rem}.g-lg-5,.gy-lg-5{--bs-gutter-y: 3rem}}@media (min-width: 1200px){.col-xl{flex:1 0 0%}.row-cols-xl-auto>*{flex:0 0 auto;width:auto}.row-cols-xl-1>*{flex:0 0 auto;width:100%}.row-cols-xl-2>*{flex:0 0 auto;width:50%}.row-cols-xl-3>*{flex:0 0 auto;width:33.33333333%}.row-cols-xl-4>*{flex:0 0 auto;width:25%}.row-cols-xl-5>*{flex:0 0 auto;width:20%}.row-cols-xl-6>*{flex:0 0 auto;width:16.66666667%}.col-xl-auto{flex:0 0 auto;width:auto}.col-xl-1{flex:0 0 auto;width:8.33333333%}.col-xl-2{flex:0 0 auto;width:16.66666667%}.col-xl-3{flex:0 0 auto;width:25%}.col-xl-4{flex:0 0 auto;width:33.33333333%}.col-xl-5{flex:0 0 auto;width:41.66666667%}.col-xl-6{flex:0 0 auto;width:50%}.col-xl-7{flex:0 0 auto;width:58.33333333%}.col-xl-8{flex:0 0 auto;width:66.66666667%}.col-xl-9{flex:0 0 auto;width:75%}.col-xl-10{flex:0 0 auto;width:83.33333333%}.col-xl-11{flex:0 0 auto;width:91.66666667%}.col-xl-12{flex:0 0 auto;width:100%}.offset-xl-0{margin-left:0}.offset-xl-1{margin-left:8.33333333%}.offset-xl-2{margin-left:16.66666667%}.offset-xl-3{margin-left:25%}.offset-xl-4{margin-left:33.33333333%}.offset-xl-5{margin-left:41.66666667%}.offset-xl-6{margin-left:50%}.offset-xl-7{margin-left:58.33333333%}.offset-xl-8{margin-left:66.66666667%}.offset-xl-9{margin-left:75%}.offset-xl-10{margin-left:83.33333333%}.offset-xl-11{margin-left:91.66666667%}.g-xl-0,.gx-xl-0{--bs-gutter-x: 0}.g-xl-0,.gy-xl-0{--bs-gutter-y: 0}.g-xl-1,.gx-xl-1{--bs-gutter-x: .25rem}.g-xl-1,.gy-xl-1{--bs-gutter-y: .25rem}.g-xl-2,.gx-xl-2{--bs-gutter-x: .5rem}.g-xl-2,.gy-xl-2{--bs-gutter-y: .5rem}.g-xl-3,.gx-xl-3{--bs-gutter-x: 1rem}.g-xl-3,.gy-xl-3{--bs-gutter-y: 1rem}.g-xl-4,.gx-xl-4{--bs-gutter-x: 1.5rem}.g-xl-4,.gy-xl-4{--bs-gutter-y: 1.5rem}.g-xl-5,.gx-xl-5{--bs-gutter-x: 3rem}.g-xl-5,.gy-xl-5{--bs-gutter-y: 3rem}}@media (min-width: 1400px){.col-xxl{flex:1 0 0%}.row-cols-xxl-auto>*{flex:0 0 auto;width:auto}.row-cols-xxl-1>*{flex:0 0 auto;width:100%}.row-cols-xxl-2>*{flex:0 0 auto;width:50%}.row-cols-xxl-3>*{flex:0 0 auto;width:33.33333333%}.row-cols-xxl-4>*{flex:0 0 auto;width:25%}.row-cols-xxl-5>*{flex:0 0 auto;width:20%}.row-cols-xxl-6>*{flex:0 0 auto;width:16.66666667%}.col-xxl-auto{flex:0 0 auto;width:auto}.col-xxl-1{flex:0 0 auto;width:8.33333333%}.col-xxl-2{flex:0 0 auto;width:16.66666667%}.col-xxl-3{flex:0 0 auto;width:25%}.col-xxl-4{flex:0 0 auto;width:33.33333333%}.col-xxl-5{flex:0 0 auto;width:41.66666667%}.col-xxl-6{flex:0 0 auto;width:50%}.col-xxl-7{flex:0 0 auto;width:58.33333333%}.col-xxl-8{flex:0 0 auto;width:66.66666667%}.col-xxl-9{flex:0 0 auto;width:75%}.col-xxl-10{flex:0 0 auto;width:83.33333333%}.col-xxl-11{flex:0 0 auto;width:91.66666667%}.col-xxl-12{flex:0 0 auto;width:100%}.offset-xxl-0{margin-left:0}.offset-xxl-1{margin-left:8.33333333%}.offset-xxl-2{margin-left:16.66666667%}.offset-xxl-3{margin-left:25%}.offset-xxl-4{margin-left:33.33333333%}.offset-xxl-5{margin-left:41.66666667%}.offset-xxl-6{margin-left:50%}.offset-xxl-7{margin-left:58.33333333%}.offset-xxl-8{margin-left:66.66666667%}.offset-xxl-9{margin-left:75%}.offset-xxl-10{margin-left:83.33333333%}.offset-xxl-11{margin-left:91.66666667%}.g-xxl-0,.gx-xxl-0{--bs-gutter-x: 0}.g-xxl-0,.gy-xxl-0{--bs-gutter-y: 0}.g-xxl-1,.gx-xxl-1{--bs-gutter-x: .25rem}.g-xxl-1,.gy-xxl-1{--bs-gutter-y: .25rem}.g-xxl-2,.gx-xxl-2{--bs-gutter-x: .5rem}.g-xxl-2,.gy-xxl-2{--bs-gutter-y: .5rem}.g-xxl-3,.gx-xxl-3{--bs-gutter-x: 1rem}.g-xxl-3,.gy-xxl-3{--bs-gutter-y: 1rem}.g-xxl-4,.gx-xxl-4{--bs-gutter-x: 1.5rem}.g-xxl-4,.gy-xxl-4{--bs-gutter-y: 1.5rem}.g-xxl-5,.gx-xxl-5{--bs-gutter-x: 3rem}.g-xxl-5,.gy-xxl-5{--bs-gutter-y: 3rem}}.table{--bs-table-color-type: initial;--bs-table-bg-type: initial;--bs-table-color-state: initial;--bs-table-bg-state: initial;--bs-table-color: var(--bs-emphasis-color);--bs-table-bg: var(--bs-body-bg);--bs-table-border-color: var(--bs-border-color);--bs-table-accent-bg: transparent;--bs-table-striped-color: var(--bs-emphasis-color);--bs-table-striped-bg: rgba(var(--bs-emphasis-color-rgb), .05);--bs-table-active-color: var(--bs-emphasis-color);--bs-table-active-bg: rgba(var(--bs-emphasis-color-rgb), .1);--bs-table-hover-color: var(--bs-emphasis-color);--bs-table-hover-bg: rgba(var(--bs-emphasis-color-rgb), .075);width:100%;margin-bottom:1rem;vertical-align:top;border-color:var(--bs-table-border-color)}.table>:not(caption)>*>*{padding:.5rem;color:var(--bs-table-color-state, var(--bs-table-color-type, var(--bs-table-color)));background-color:var(--bs-table-bg);border-bottom-width:var(--bs-border-width);box-shadow:inset 0 0 0 9999px var(--bs-table-bg-state, var(--bs-table-bg-type, var(--bs-table-accent-bg)))}.table>tbody{vertical-align:inherit}.table>thead{vertical-align:bottom}.table-group-divider{border-top:calc(var(--bs-border-width) * 2) solid currentcolor}.caption-top{caption-side:top}.table-sm>:not(caption)>*>*{padding:.25rem}.table-bordered>:not(caption)>*{border-width:var(--bs-border-width) 0}.table-bordered>:not(caption)>*>*{border-width:0 var(--bs-border-width)}.table-borderless>:not(caption)>*>*{border-bottom-width:0}.table-borderless>:not(:first-child){border-top-width:0}.table-striped>tbody>tr:nth-of-type(odd)>*{--bs-table-color-type: var(--bs-table-striped-color);--bs-table-bg-type: var(--bs-table-striped-bg)}.table-striped-columns>:not(caption)>tr>:nth-child(2n){--bs-table-color-type: var(--bs-table-striped-color);--bs-table-bg-type: var(--bs-table-striped-bg)}.table-active{--bs-table-color-state: var(--bs-table-active-color);--bs-table-bg-state: var(--bs-table-active-bg)}.table-hover>tbody>tr:hover>*{--bs-table-color-state: var(--bs-table-hover-color);--bs-table-bg-state: var(--bs-table-hover-bg)}.table-primary{--bs-table-color: #000;--bs-table-bg: #cfe2ff;--bs-table-border-color: #a6b5cc;--bs-table-striped-bg: #c5d7f2;--bs-table-striped-color: #000;--bs-table-active-bg: #bacbe6;--bs-table-active-color: #000;--bs-table-hover-bg: #bfd1ec;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-secondary{--bs-table-color: #000;--bs-table-bg: #e2e3e5;--bs-table-border-color: #b5b6b7;--bs-table-striped-bg: #d7d8da;--bs-table-striped-color: #000;--bs-table-active-bg: #cbccce;--bs-table-active-color: #000;--bs-table-hover-bg: #d1d2d4;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-success{--bs-table-color: #000;--bs-table-bg: #d1e7dd;--bs-table-border-color: #a7b9b1;--bs-table-striped-bg: #c7dbd2;--bs-table-striped-color: #000;--bs-table-active-bg: #bcd0c7;--bs-table-active-color: #000;--bs-table-hover-bg: #c1d6cc;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-info{--bs-table-color: #000;--bs-table-bg: #cff4fc;--bs-table-border-color: #a6c3ca;--bs-table-striped-bg: #c5e8ef;--bs-table-striped-color: #000;--bs-table-active-bg: #badce3;--bs-table-active-color: #000;--bs-table-hover-bg: #bfe2e9;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-warning{--bs-table-color: #000;--bs-table-bg: #fff3cd;--bs-table-border-color: #ccc2a4;--bs-table-striped-bg: #f2e7c3;--bs-table-striped-color: #000;--bs-table-active-bg: #e6dbb9;--bs-table-active-color: #000;--bs-table-hover-bg: #ece1be;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-danger{--bs-table-color: #000;--bs-table-bg: #f8d7da;--bs-table-border-color: #c6acae;--bs-table-striped-bg: #eccccf;--bs-table-striped-color: #000;--bs-table-active-bg: #dfc2c4;--bs-table-active-color: #000;--bs-table-hover-bg: #e5c7ca;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-light{--bs-table-color: #000;--bs-table-bg: #f8f9fa;--bs-table-border-color: #c6c7c8;--bs-table-striped-bg: #ecedee;--bs-table-striped-color: #000;--bs-table-active-bg: #dfe0e1;--bs-table-active-color: #000;--bs-table-hover-bg: #e5e6e7;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-dark{--bs-table-color: #fff;--bs-table-bg: #212529;--bs-table-border-color: #4d5154;--bs-table-striped-bg: #2c3034;--bs-table-striped-color: #fff;--bs-table-active-bg: #373b3e;--bs-table-active-color: #fff;--bs-table-hover-bg: #323539;--bs-table-hover-color: #fff;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-responsive{overflow-x:auto;-webkit-overflow-scrolling:touch}@media (max-width: 575.98px){.table-responsive-sm{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 767.98px){.table-responsive-md{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 991.98px){.table-responsive-lg{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 1199.98px){.table-responsive-xl{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 1399.98px){.table-responsive-xxl{overflow-x:auto;-webkit-overflow-scrolling:touch}}.form-label{margin-bottom:.5rem}.col-form-label{padding-top:calc(.375rem + var(--bs-border-width));padding-bottom:calc(.375rem + var(--bs-border-width));margin-bottom:0;font-size:inherit;line-height:1.5}.col-form-label-lg{padding-top:calc(.5rem + var(--bs-border-width));padding-bottom:calc(.5rem + var(--bs-border-width));font-size:1.25rem}.col-form-label-sm{padding-top:calc(.25rem + var(--bs-border-width));padding-bottom:calc(.25rem + var(--bs-border-width));font-size:.875rem}.form-text{margin-top:.25rem;font-size:.875em;color:var(--bs-secondary-color)}.form-control{display:block;width:100%;padding:.375rem .75rem;font-size:1rem;font-weight:400;line-height:1.5;color:var(--bs-body-color);appearance:none;background-color:var(--bs-body-bg);background-clip:padding-box;border:var(--bs-border-width) solid var(--bs-border-color);border-radius:var(--bs-border-radius);transition:border-color .15s ease-in-out,box-shadow .15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-control{transition:none}}.form-control[type=file]{overflow:hidden}.form-control[type=file]:not(:disabled):not([readonly]){cursor:pointer}.form-control:focus{color:var(--bs-body-color);background-color:var(--bs-body-bg);border-color:#86b7fe;outline:0;box-shadow:0 0 0 .25rem #0d6efd40}.form-control::-webkit-date-and-time-value{min-width:85px;height:1.5em;margin:0}.form-control::-webkit-datetime-edit{display:block;padding:0}.form-control::placeholder{color:var(--bs-secondary-color);opacity:1}.form-control:disabled{background-color:var(--bs-secondary-bg);opacity:1}.form-control::file-selector-button{padding:.375rem .75rem;margin:-.375rem -.75rem;margin-inline-end:.75rem;color:var(--bs-body-color);background-color:var(--bs-tertiary-bg);pointer-events:none;border-color:inherit;border-style:solid;border-width:0;border-inline-end-width:var(--bs-border-width);border-radius:0;transition:color .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-control::file-selector-button{transition:none}}.form-control:hover:not(:disabled):not([readonly])::file-selector-button{background-color:var(--bs-secondary-bg)}.form-control-plaintext{display:block;width:100%;padding:.375rem 0;margin-bottom:0;line-height:1.5;color:var(--bs-body-color);background-color:transparent;border:solid transparent;border-width:var(--bs-border-width) 0}.form-control-plaintext:focus{outline:0}.form-control-plaintext.form-control-sm,.form-control-plaintext.form-control-lg{padding-right:0;padding-left:0}.form-control-sm{min-height:calc(1.5em + .5rem + calc(var(--bs-border-width) * 2));padding:.25rem .5rem;font-size:.875rem;border-radius:var(--bs-border-radius-sm)}.form-control-sm::file-selector-button{padding:.25rem .5rem;margin:-.25rem -.5rem;margin-inline-end:.5rem}.form-control-lg{min-height:calc(1.5em + 1rem + calc(var(--bs-border-width) * 2));padding:.5rem 1rem;font-size:1.25rem;border-radius:var(--bs-border-radius-lg)}.form-control-lg::file-selector-button{padding:.5rem 1rem;margin:-.5rem -1rem;margin-inline-end:1rem}textarea.form-control{min-height:calc(1.5em + .75rem + calc(var(--bs-border-width) * 2))}textarea.form-control-sm{min-height:calc(1.5em + .5rem + calc(var(--bs-border-width) * 2))}textarea.form-control-lg{min-height:calc(1.5em + 1rem + calc(var(--bs-border-width) * 2))}.form-control-color{width:3rem;height:calc(1.5em + .75rem + calc(var(--bs-border-width) * 2));padding:.375rem}.form-control-color:not(:disabled):not([readonly]){cursor:pointer}.form-control-color::-moz-color-swatch{border:0!important;border-radius:var(--bs-border-radius)}.form-control-color::-webkit-color-swatch{border:0!important;border-radius:var(--bs-border-radius)}.form-control-color.form-control-sm{height:calc(1.5em + .5rem + calc(var(--bs-border-width) * 2))}.form-control-color.form-control-lg{height:calc(1.5em + 1rem + calc(var(--bs-border-width) * 2))}.form-select{--bs-form-select-bg-img: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23343a40' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e");display:block;width:100%;padding:.375rem 2.25rem .375rem .75rem;font-size:1rem;font-weight:400;line-height:1.5;color:var(--bs-body-color);appearance:none;background-color:var(--bs-body-bg);background-image:var(--bs-form-select-bg-img),var(--bs-form-select-bg-icon, none);background-repeat:no-repeat;background-position:right .75rem center;background-size:16px 12px;border:var(--bs-border-width) solid var(--bs-border-color);border-radius:var(--bs-border-radius);transition:border-color .15s ease-in-out,box-shadow .15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-select{transition:none}}.form-select:focus{border-color:#86b7fe;outline:0;box-shadow:0 0 0 .25rem #0d6efd40}.form-select[multiple],.form-select[size]:not([size="1"]){padding-right:.75rem;background-image:none}.form-select:disabled{background-color:var(--bs-secondary-bg)}.form-select:-moz-focusring{color:transparent;text-shadow:0 0 0 var(--bs-body-color)}.form-select-sm{padding-top:.25rem;padding-bottom:.25rem;padding-left:.5rem;font-size:.875rem;border-radius:var(--bs-border-radius-sm)}.form-select-lg{padding-top:.5rem;padding-bottom:.5rem;padding-left:1rem;font-size:1.25rem;border-radius:var(--bs-border-radius-lg)}[data-bs-theme=dark] .form-select{--bs-form-select-bg-img: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23dee2e6' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e")}.form-check{display:block;min-height:1.5rem;padding-left:1.5em;margin-bottom:.125rem}.form-check .form-check-input{float:left;margin-left:-1.5em}.form-check-reverse{padding-right:1.5em;padding-left:0;text-align:right}.form-check-reverse .form-check-input{float:right;margin-right:-1.5em;margin-left:0}.form-check-input{--bs-form-check-bg: var(--bs-body-bg);flex-shrink:0;width:1em;height:1em;margin-top:.25em;vertical-align:top;appearance:none;background-color:var(--bs-form-check-bg);background-image:var(--bs-form-check-bg-image);background-repeat:no-repeat;background-position:center;background-size:contain;border:var(--bs-border-width) solid var(--bs-border-color);print-color-adjust:exact}.form-check-input[type=checkbox]{border-radius:.25em}.form-check-input[type=radio]{border-radius:50%}.form-check-input:active{filter:brightness(90%)}.form-check-input:focus{border-color:#86b7fe;outline:0;box-shadow:0 0 0 .25rem #0d6efd40}.form-check-input:checked{background-color:#0d6efd;border-color:#0d6efd}.form-check-input:checked[type=checkbox]{--bs-form-check-bg-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 20 20'%3e%3cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='m6 10 3 3 6-6'/%3e%3c/svg%3e")}.form-check-input:checked[type=radio]{--bs-form-check-bg-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='2' fill='%23fff'/%3e%3c/svg%3e")}.form-check-input[type=checkbox]:indeterminate{background-color:#0d6efd;border-color:#0d6efd;--bs-form-check-bg-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 20 20'%3e%3cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='M6 10h8'/%3e%3c/svg%3e")}.form-check-input:disabled{pointer-events:none;filter:none;opacity:.5}.form-check-input[disabled]~.form-check-label,.form-check-input:disabled~.form-check-label{cursor:default;opacity:.5}.form-switch{padding-left:2.5em}.form-switch .form-check-input{--bs-form-switch-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='rgba%280, 0, 0, 0.25%29'/%3e%3c/svg%3e");width:2em;margin-left:-2.5em;background-image:var(--bs-form-switch-bg);background-position:left center;border-radius:2em;transition:background-position .15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-switch .form-check-input{transition:none}}.form-switch .form-check-input:focus{--bs-form-switch-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='%2386b7fe'/%3e%3c/svg%3e")}.form-switch .form-check-input:checked{background-position:right center;--bs-form-switch-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='%23fff'/%3e%3c/svg%3e")}.form-switch.form-check-reverse{padding-right:2.5em;padding-left:0}.form-switch.form-check-reverse .form-check-input{margin-right:-2.5em;margin-left:0}.form-check-inline{display:inline-block;margin-right:1rem}.btn-check{position:absolute;clip:rect(0,0,0,0);pointer-events:none}.btn-check[disabled]+.btn,.btn-check:disabled+.btn{pointer-events:none;filter:none;opacity:.65}[data-bs-theme=dark] .form-switch .form-check-input:not(:checked):not(:focus){--bs-form-switch-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='rgba%28255, 255, 255, 0.25%29'/%3e%3c/svg%3e")}.form-range{width:100%;height:1.5rem;padding:0;appearance:none;background-color:transparent}.form-range:focus{outline:0}.form-range:focus::-webkit-slider-thumb{box-shadow:0 0 0 1px #fff,0 0 0 .25rem #0d6efd40}.form-range:focus::-moz-range-thumb{box-shadow:0 0 0 1px #fff,0 0 0 .25rem #0d6efd40}.form-range::-moz-focus-outer{border:0}.form-range::-webkit-slider-thumb{width:1rem;height:1rem;margin-top:-.25rem;appearance:none;background-color:#0d6efd;border:0;border-radius:1rem;transition:background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-range::-webkit-slider-thumb{transition:none}}.form-range::-webkit-slider-thumb:active{background-color:#b6d4fe}.form-range::-webkit-slider-runnable-track{width:100%;height:.5rem;color:transparent;cursor:pointer;background-color:var(--bs-secondary-bg);border-color:transparent;border-radius:1rem}.form-range::-moz-range-thumb{width:1rem;height:1rem;appearance:none;background-color:#0d6efd;border:0;border-radius:1rem;transition:background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-range::-moz-range-thumb{transition:none}}.form-range::-moz-range-thumb:active{background-color:#b6d4fe}.form-range::-moz-range-track{width:100%;height:.5rem;color:transparent;cursor:pointer;background-color:var(--bs-secondary-bg);border-color:transparent;border-radius:1rem}.form-range:disabled{pointer-events:none}.form-range:disabled::-webkit-slider-thumb{background-color:var(--bs-secondary-color)}.form-range:disabled::-moz-range-thumb{background-color:var(--bs-secondary-color)}.form-floating{position:relative}.form-floating>.form-control,.form-floating>.form-control-plaintext,.form-floating>.form-select{height:calc(3.5rem + calc(var(--bs-border-width) * 2));min-height:calc(3.5rem + calc(var(--bs-border-width) * 2));line-height:1.25}.form-floating>label{position:absolute;top:0;left:0;z-index:2;height:100%;padding:1rem .75rem;overflow:hidden;text-align:start;text-overflow:ellipsis;white-space:nowrap;pointer-events:none;border:var(--bs-border-width) solid transparent;transform-origin:0 0;transition:opacity .1s ease-in-out,transform .1s ease-in-out}@media (prefers-reduced-motion: reduce){.form-floating>label{transition:none}}.form-floating>.form-control,.form-floating>.form-control-plaintext{padding:1rem .75rem}.form-floating>.form-control::placeholder,.form-floating>.form-control-plaintext::placeholder{color:transparent}.form-floating>.form-control:focus,.form-floating>.form-control:not(:placeholder-shown),.form-floating>.form-control-plaintext:focus,.form-floating>.form-control-plaintext:not(:placeholder-shown){padding-top:1.625rem;padding-bottom:.625rem}.form-floating>.form-control:-webkit-autofill,.form-floating>.form-control-plaintext:-webkit-autofill{padding-top:1.625rem;padding-bottom:.625rem}.form-floating>.form-select{padding-top:1.625rem;padding-bottom:.625rem}.form-floating>.form-control:focus~label,.form-floating>.form-control:not(:placeholder-shown)~label,.form-floating>.form-control-plaintext~label,.form-floating>.form-select~label{color:rgba(var(--bs-body-color-rgb),.65);transform:scale(.85) translateY(-.5rem) translate(.15rem)}.form-floating>.form-control:focus~label:after,.form-floating>.form-control:not(:placeholder-shown)~label:after,.form-floating>.form-control-plaintext~label:after,.form-floating>.form-select~label:after{position:absolute;inset:1rem .375rem;z-index:-1;height:1.5em;content:"";background-color:var(--bs-body-bg);border-radius:var(--bs-border-radius)}.form-floating>.form-control:-webkit-autofill~label{color:rgba(var(--bs-body-color-rgb),.65);transform:scale(.85) translateY(-.5rem) translate(.15rem)}.form-floating>.form-control-plaintext~label{border-width:var(--bs-border-width) 0}.form-floating>:disabled~label,.form-floating>.form-control:disabled~label{color:#6c757d}.form-floating>:disabled~label:after,.form-floating>.form-control:disabled~label:after{background-color:var(--bs-secondary-bg)}.input-group{position:relative;display:flex;flex-wrap:wrap;align-items:stretch;width:100%}.input-group>.form-control,.input-group>.form-select,.input-group>.form-floating{position:relative;flex:1 1 auto;width:1%;min-width:0}.input-group>.form-control:focus,.input-group>.form-select:focus,.input-group>.form-floating:focus-within{z-index:5}.input-group .btn{position:relative;z-index:2}.input-group .btn:focus{z-index:5}.input-group-text{display:flex;align-items:center;padding:.375rem .75rem;font-size:1rem;font-weight:400;line-height:1.5;color:var(--bs-body-color);text-align:center;white-space:nowrap;background-color:var(--bs-tertiary-bg);border:var(--bs-border-width) solid var(--bs-border-color);border-radius:var(--bs-border-radius)}.input-group-lg>.form-control,.input-group-lg>.form-select,.input-group-lg>.input-group-text,.input-group-lg>.btn{padding:.5rem 1rem;font-size:1.25rem;border-radius:var(--bs-border-radius-lg)}.input-group-sm>.form-control,.input-group-sm>.form-select,.input-group-sm>.input-group-text,.input-group-sm>.btn{padding:.25rem .5rem;font-size:.875rem;border-radius:var(--bs-border-radius-sm)}.input-group-lg>.form-select,.input-group-sm>.form-select{padding-right:3rem}.input-group:not(.has-validation)>:not(:last-child):not(.dropdown-toggle):not(.dropdown-menu):not(.form-floating),.input-group:not(.has-validation)>.dropdown-toggle:nth-last-child(n+3),.input-group:not(.has-validation)>.form-floating:not(:last-child)>.form-control,.input-group:not(.has-validation)>.form-floating:not(:last-child)>.form-select{border-top-right-radius:0;border-bottom-right-radius:0}.input-group.has-validation>:nth-last-child(n+3):not(.dropdown-toggle):not(.dropdown-menu):not(.form-floating),.input-group.has-validation>.dropdown-toggle:nth-last-child(n+4),.input-group.has-validation>.form-floating:nth-last-child(n+3)>.form-control,.input-group.has-validation>.form-floating:nth-last-child(n+3)>.form-select{border-top-right-radius:0;border-bottom-right-radius:0}.input-group>:not(:first-child):not(.dropdown-menu):not(.valid-tooltip):not(.valid-feedback):not(.invalid-tooltip):not(.invalid-feedback){margin-left:calc(var(--bs-border-width) * -1);border-top-left-radius:0;border-bottom-left-radius:0}.input-group>.form-floating:not(:first-child)>.form-control,.input-group>.form-floating:not(:first-child)>.form-select{border-top-left-radius:0;border-bottom-left-radius:0}.valid-feedback{display:none;width:100%;margin-top:.25rem;font-size:.875em;color:var(--bs-form-valid-color)}.valid-tooltip{position:absolute;top:100%;z-index:5;display:none;max-width:100%;padding:.25rem .5rem;margin-top:.1rem;font-size:.875rem;color:#fff;background-color:var(--bs-success);border-radius:var(--bs-border-radius)}.was-validated :valid~.valid-feedback,.was-validated :valid~.valid-tooltip,.is-valid~.valid-feedback,.is-valid~.valid-tooltip{display:block}.was-validated .form-control:valid,.form-control.is-valid{border-color:var(--bs-form-valid-border-color);padding-right:calc(1.5em + .75rem);background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8 8'%3e%3cpath fill='%23198754' d='M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z'/%3e%3c/svg%3e");background-repeat:no-repeat;background-position:right calc(.375em + .1875rem) center;background-size:calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-control:valid:focus,.form-control.is-valid:focus{border-color:var(--bs-form-valid-border-color);box-shadow:0 0 0 .25rem rgba(var(--bs-success-rgb),.25)}.was-validated textarea.form-control:valid,textarea.form-control.is-valid{padding-right:calc(1.5em + .75rem);background-position:top calc(.375em + .1875rem) right calc(.375em + .1875rem)}.was-validated .form-select:valid,.form-select.is-valid{border-color:var(--bs-form-valid-border-color)}.was-validated .form-select:valid:not([multiple]):not([size]),.was-validated .form-select:valid:not([multiple])[size="1"],.form-select.is-valid:not([multiple]):not([size]),.form-select.is-valid:not([multiple])[size="1"]{--bs-form-select-bg-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8 8'%3e%3cpath fill='%23198754' d='M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z'/%3e%3c/svg%3e");padding-right:4.125rem;background-position:right .75rem center,center right 2.25rem;background-size:16px 12px,calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-select:valid:focus,.form-select.is-valid:focus{border-color:var(--bs-form-valid-border-color);box-shadow:0 0 0 .25rem rgba(var(--bs-success-rgb),.25)}.was-validated .form-control-color:valid,.form-control-color.is-valid{width:calc(3.75rem + 1.5em)}.was-validated .form-check-input:valid,.form-check-input.is-valid{border-color:var(--bs-form-valid-border-color)}.was-validated .form-check-input:valid:checked,.form-check-input.is-valid:checked{background-color:var(--bs-form-valid-color)}.was-validated .form-check-input:valid:focus,.form-check-input.is-valid:focus{box-shadow:0 0 0 .25rem rgba(var(--bs-success-rgb),.25)}.was-validated .form-check-input:valid~.form-check-label,.form-check-input.is-valid~.form-check-label{color:var(--bs-form-valid-color)}.form-check-inline .form-check-input~.valid-feedback{margin-left:.5em}.was-validated .input-group>.form-control:not(:focus):valid,.input-group>.form-control:not(:focus).is-valid,.was-validated .input-group>.form-select:not(:focus):valid,.input-group>.form-select:not(:focus).is-valid,.was-validated .input-group>.form-floating:not(:focus-within):valid,.input-group>.form-floating:not(:focus-within).is-valid{z-index:3}.invalid-feedback{display:none;width:100%;margin-top:.25rem;font-size:.875em;color:var(--bs-form-invalid-color)}.invalid-tooltip{position:absolute;top:100%;z-index:5;display:none;max-width:100%;padding:.25rem .5rem;margin-top:.1rem;font-size:.875rem;color:#fff;background-color:var(--bs-danger);border-radius:var(--bs-border-radius)}.was-validated :invalid~.invalid-feedback,.was-validated :invalid~.invalid-tooltip,.is-invalid~.invalid-feedback,.is-invalid~.invalid-tooltip{display:block}.was-validated .form-control:invalid,.form-control.is-invalid{border-color:var(--bs-form-invalid-border-color);padding-right:calc(1.5em + .75rem);background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12' width='12' height='12' fill='none' stroke='%23dc3545'%3e%3ccircle cx='6' cy='6' r='4.5'/%3e%3cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3e%3ccircle cx='6' cy='8.2' r='.6' fill='%23dc3545' stroke='none'/%3e%3c/svg%3e");background-repeat:no-repeat;background-position:right calc(.375em + .1875rem) center;background-size:calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-control:invalid:focus,.form-control.is-invalid:focus{border-color:var(--bs-form-invalid-border-color);box-shadow:0 0 0 .25rem rgba(var(--bs-danger-rgb),.25)}.was-validated textarea.form-control:invalid,textarea.form-control.is-invalid{padding-right:calc(1.5em + .75rem);background-position:top calc(.375em + .1875rem) right calc(.375em + .1875rem)}.was-validated .form-select:invalid,.form-select.is-invalid{border-color:var(--bs-form-invalid-border-color)}.was-validated .form-select:invalid:not([multiple]):not([size]),.was-validated .form-select:invalid:not([multiple])[size="1"],.form-select.is-invalid:not([multiple]):not([size]),.form-select.is-invalid:not([multiple])[size="1"]{--bs-form-select-bg-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12' width='12' height='12' fill='none' stroke='%23dc3545'%3e%3ccircle cx='6' cy='6' r='4.5'/%3e%3cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3e%3ccircle cx='6' cy='8.2' r='.6' fill='%23dc3545' stroke='none'/%3e%3c/svg%3e");padding-right:4.125rem;background-position:right .75rem center,center right 2.25rem;background-size:16px 12px,calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-select:invalid:focus,.form-select.is-invalid:focus{border-color:var(--bs-form-invalid-border-color);box-shadow:0 0 0 .25rem rgba(var(--bs-danger-rgb),.25)}.was-validated .form-control-color:invalid,.form-control-color.is-invalid{width:calc(3.75rem + 1.5em)}.was-validated .form-check-input:invalid,.form-check-input.is-invalid{border-color:var(--bs-form-invalid-border-color)}.was-validated .form-check-input:invalid:checked,.form-check-input.is-invalid:checked{background-color:var(--bs-form-invalid-color)}.was-validated .form-check-input:invalid:focus,.form-check-input.is-invalid:focus{box-shadow:0 0 0 .25rem rgba(var(--bs-danger-rgb),.25)}.was-validated .form-check-input:invalid~.form-check-label,.form-check-input.is-invalid~.form-check-label{color:var(--bs-form-invalid-color)}.form-check-inline .form-check-input~.invalid-feedback{margin-left:.5em}.was-validated .input-group>.form-control:not(:focus):invalid,.input-group>.form-control:not(:focus).is-invalid,.was-validated .input-group>.form-select:not(:focus):invalid,.input-group>.form-select:not(:focus).is-invalid,.was-validated .input-group>.form-floating:not(:focus-within):invalid,.input-group>.form-floating:not(:focus-within).is-invalid{z-index:4}.btn{--bs-btn-padding-x: .75rem;--bs-btn-padding-y: .375rem;--bs-btn-font-family: ;--bs-btn-font-size: 1rem;--bs-btn-font-weight: 400;--bs-btn-line-height: 1.5;--bs-btn-color: var(--bs-body-color);--bs-btn-bg: transparent;--bs-btn-border-width: var(--bs-border-width);--bs-btn-border-color: transparent;--bs-btn-border-radius: var(--bs-border-radius);--bs-btn-hover-border-color: transparent;--bs-btn-box-shadow: inset 0 1px 0 rgba(255, 255, 255, .15), 0 1px 1px rgba(0, 0, 0, .075);--bs-btn-disabled-opacity: .65;--bs-btn-focus-box-shadow: 0 0 0 .25rem rgba(var(--bs-btn-focus-shadow-rgb), .5);display:inline-block;padding:var(--bs-btn-padding-y) var(--bs-btn-padding-x);font-family:var(--bs-btn-font-family);font-size:var(--bs-btn-font-size);font-weight:var(--bs-btn-font-weight);line-height:var(--bs-btn-line-height);color:var(--bs-btn-color);text-align:center;text-decoration:none;vertical-align:middle;cursor:pointer;user-select:none;border:var(--bs-btn-border-width) solid var(--bs-btn-border-color);border-radius:var(--bs-btn-border-radius);background-color:var(--bs-btn-bg);transition:color .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out}@media (prefers-reduced-motion: reduce){.btn{transition:none}}.btn:hover{color:var(--bs-btn-hover-color);background-color:var(--bs-btn-hover-bg);border-color:var(--bs-btn-hover-border-color)}.btn-check+.btn:hover{color:var(--bs-btn-color);background-color:var(--bs-btn-bg);border-color:var(--bs-btn-border-color)}.btn:focus-visible{color:var(--bs-btn-hover-color);background-color:var(--bs-btn-hover-bg);border-color:var(--bs-btn-hover-border-color);outline:0;box-shadow:var(--bs-btn-focus-box-shadow)}.btn-check:focus-visible+.btn{border-color:var(--bs-btn-hover-border-color);outline:0;box-shadow:var(--bs-btn-focus-box-shadow)}.btn-check:checked+.btn,:not(.btn-check)+.btn:active,.btn:first-child:active,.btn.active,.btn.show{color:var(--bs-btn-active-color);background-color:var(--bs-btn-active-bg);border-color:var(--bs-btn-active-border-color)}.btn-check:checked+.btn:focus-visible,:not(.btn-check)+.btn:active:focus-visible,.btn:first-child:active:focus-visible,.btn.active:focus-visible,.btn.show:focus-visible{box-shadow:var(--bs-btn-focus-box-shadow)}.btn:disabled,.btn.disabled,fieldset:disabled .btn{color:var(--bs-btn-disabled-color);pointer-events:none;background-color:var(--bs-btn-disabled-bg);border-color:var(--bs-btn-disabled-border-color);opacity:var(--bs-btn-disabled-opacity)}.btn-primary{--bs-btn-color: #fff;--bs-btn-bg: #0d6efd;--bs-btn-border-color: #0d6efd;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #0b5ed7;--bs-btn-hover-border-color: #0a58ca;--bs-btn-focus-shadow-rgb: 49, 132, 253;--bs-btn-active-color: #fff;--bs-btn-active-bg: #0a58ca;--bs-btn-active-border-color: #0a53be;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #0d6efd;--bs-btn-disabled-border-color: #0d6efd}.btn-secondary{--bs-btn-color: #fff;--bs-btn-bg: #6c757d;--bs-btn-border-color: #6c757d;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #5c636a;--bs-btn-hover-border-color: #565e64;--bs-btn-focus-shadow-rgb: 130, 138, 145;--bs-btn-active-color: #fff;--bs-btn-active-bg: #565e64;--bs-btn-active-border-color: #51585e;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #6c757d;--bs-btn-disabled-border-color: #6c757d}.btn-success{--bs-btn-color: #fff;--bs-btn-bg: #198754;--bs-btn-border-color: #198754;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #157347;--bs-btn-hover-border-color: #146c43;--bs-btn-focus-shadow-rgb: 60, 153, 110;--bs-btn-active-color: #fff;--bs-btn-active-bg: #146c43;--bs-btn-active-border-color: #13653f;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #198754;--bs-btn-disabled-border-color: #198754}.btn-info{--bs-btn-color: #000;--bs-btn-bg: #0dcaf0;--bs-btn-border-color: #0dcaf0;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #31d2f2;--bs-btn-hover-border-color: #25cff2;--bs-btn-focus-shadow-rgb: 11, 172, 204;--bs-btn-active-color: #000;--bs-btn-active-bg: #3dd5f3;--bs-btn-active-border-color: #25cff2;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #000;--bs-btn-disabled-bg: #0dcaf0;--bs-btn-disabled-border-color: #0dcaf0}.btn-warning{--bs-btn-color: #000;--bs-btn-bg: #ffc107;--bs-btn-border-color: #ffc107;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #ffca2c;--bs-btn-hover-border-color: #ffc720;--bs-btn-focus-shadow-rgb: 217, 164, 6;--bs-btn-active-color: #000;--bs-btn-active-bg: #ffcd39;--bs-btn-active-border-color: #ffc720;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #000;--bs-btn-disabled-bg: #ffc107;--bs-btn-disabled-border-color: #ffc107}.btn-danger{--bs-btn-color: #fff;--bs-btn-bg: #dc3545;--bs-btn-border-color: #dc3545;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #bb2d3b;--bs-btn-hover-border-color: #b02a37;--bs-btn-focus-shadow-rgb: 225, 83, 97;--bs-btn-active-color: #fff;--bs-btn-active-bg: #b02a37;--bs-btn-active-border-color: #a52834;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #dc3545;--bs-btn-disabled-border-color: #dc3545}.btn-light{--bs-btn-color: #000;--bs-btn-bg: #f8f9fa;--bs-btn-border-color: #f8f9fa;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #d3d4d5;--bs-btn-hover-border-color: #c6c7c8;--bs-btn-focus-shadow-rgb: 211, 212, 213;--bs-btn-active-color: #000;--bs-btn-active-bg: #c6c7c8;--bs-btn-active-border-color: #babbbc;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #000;--bs-btn-disabled-bg: #f8f9fa;--bs-btn-disabled-border-color: #f8f9fa}.btn-dark{--bs-btn-color: #fff;--bs-btn-bg: #212529;--bs-btn-border-color: #212529;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #424649;--bs-btn-hover-border-color: #373b3e;--bs-btn-focus-shadow-rgb: 66, 70, 73;--bs-btn-active-color: #fff;--bs-btn-active-bg: #4d5154;--bs-btn-active-border-color: #373b3e;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #212529;--bs-btn-disabled-border-color: #212529}.btn-outline-primary{--bs-btn-color: #0d6efd;--bs-btn-border-color: #0d6efd;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #0d6efd;--bs-btn-hover-border-color: #0d6efd;--bs-btn-focus-shadow-rgb: 13, 110, 253;--bs-btn-active-color: #fff;--bs-btn-active-bg: #0d6efd;--bs-btn-active-border-color: #0d6efd;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #0d6efd;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #0d6efd;--bs-gradient: none}.btn-outline-secondary{--bs-btn-color: #6c757d;--bs-btn-border-color: #6c757d;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #6c757d;--bs-btn-hover-border-color: #6c757d;--bs-btn-focus-shadow-rgb: 108, 117, 125;--bs-btn-active-color: #fff;--bs-btn-active-bg: #6c757d;--bs-btn-active-border-color: #6c757d;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #6c757d;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #6c757d;--bs-gradient: none}.btn-outline-success{--bs-btn-color: #198754;--bs-btn-border-color: #198754;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #198754;--bs-btn-hover-border-color: #198754;--bs-btn-focus-shadow-rgb: 25, 135, 84;--bs-btn-active-color: #fff;--bs-btn-active-bg: #198754;--bs-btn-active-border-color: #198754;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #198754;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #198754;--bs-gradient: none}.btn-outline-info{--bs-btn-color: #0dcaf0;--bs-btn-border-color: #0dcaf0;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #0dcaf0;--bs-btn-hover-border-color: #0dcaf0;--bs-btn-focus-shadow-rgb: 13, 202, 240;--bs-btn-active-color: #000;--bs-btn-active-bg: #0dcaf0;--bs-btn-active-border-color: #0dcaf0;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #0dcaf0;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #0dcaf0;--bs-gradient: none}.btn-outline-warning{--bs-btn-color: #ffc107;--bs-btn-border-color: #ffc107;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #ffc107;--bs-btn-hover-border-color: #ffc107;--bs-btn-focus-shadow-rgb: 255, 193, 7;--bs-btn-active-color: #000;--bs-btn-active-bg: #ffc107;--bs-btn-active-border-color: #ffc107;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #ffc107;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #ffc107;--bs-gradient: none}.btn-outline-danger{--bs-btn-color: #dc3545;--bs-btn-border-color: #dc3545;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #dc3545;--bs-btn-hover-border-color: #dc3545;--bs-btn-focus-shadow-rgb: 220, 53, 69;--bs-btn-active-color: #fff;--bs-btn-active-bg: #dc3545;--bs-btn-active-border-color: #dc3545;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #dc3545;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #dc3545;--bs-gradient: none}.btn-outline-light{--bs-btn-color: #f8f9fa;--bs-btn-border-color: #f8f9fa;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #f8f9fa;--bs-btn-hover-border-color: #f8f9fa;--bs-btn-focus-shadow-rgb: 248, 249, 250;--bs-btn-active-color: #000;--bs-btn-active-bg: #f8f9fa;--bs-btn-active-border-color: #f8f9fa;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #f8f9fa;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #f8f9fa;--bs-gradient: none}.btn-outline-dark{--bs-btn-color: #212529;--bs-btn-border-color: #212529;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #212529;--bs-btn-hover-border-color: #212529;--bs-btn-focus-shadow-rgb: 33, 37, 41;--bs-btn-active-color: #fff;--bs-btn-active-bg: #212529;--bs-btn-active-border-color: #212529;--bs-btn-active-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);--bs-btn-disabled-color: #212529;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #212529;--bs-gradient: none}.btn-link{--bs-btn-font-weight: 400;--bs-btn-color: var(--bs-link-color);--bs-btn-bg: transparent;--bs-btn-border-color: transparent;--bs-btn-hover-color: var(--bs-link-hover-color);--bs-btn-hover-border-color: transparent;--bs-btn-active-color: var(--bs-link-hover-color);--bs-btn-active-border-color: transparent;--bs-btn-disabled-color: #6c757d;--bs-btn-disabled-border-color: transparent;--bs-btn-box-shadow: 0 0 0 #000;--bs-btn-focus-shadow-rgb: 49, 132, 253;text-decoration:underline}.btn-link:focus-visible{color:var(--bs-btn-color)}.btn-link:hover{color:var(--bs-btn-hover-color)}.btn-lg,.btn-group-lg>.btn{--bs-btn-padding-y: .5rem;--bs-btn-padding-x: 1rem;--bs-btn-font-size: 1.25rem;--bs-btn-border-radius: var(--bs-border-radius-lg)}.btn-sm,.btn-group-sm>.btn{--bs-btn-padding-y: .25rem;--bs-btn-padding-x: .5rem;--bs-btn-font-size: .875rem;--bs-btn-border-radius: var(--bs-border-radius-sm)}.fade{transition:opacity .15s linear}@media (prefers-reduced-motion: reduce){.fade{transition:none}}.fade:not(.show){opacity:0}.collapse:not(.show){display:none}.collapsing{height:0;overflow:hidden;transition:height .35s ease}@media (prefers-reduced-motion: reduce){.collapsing{transition:none}}.collapsing.collapse-horizontal{width:0;height:auto;transition:width .35s ease}@media (prefers-reduced-motion: reduce){.collapsing.collapse-horizontal{transition:none}}.dropup,.dropend,.dropdown,.dropstart,.dropup-center,.dropdown-center{position:relative}.dropdown-toggle{white-space:nowrap}.dropdown-toggle:after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:"";border-top:.3em solid;border-right:.3em solid transparent;border-bottom:0;border-left:.3em solid transparent}.dropdown-toggle:empty:after{margin-left:0}.dropdown-menu{--bs-dropdown-zindex: 1000;--bs-dropdown-min-width: 10rem;--bs-dropdown-padding-x: 0;--bs-dropdown-padding-y: .5rem;--bs-dropdown-spacer: .125rem;--bs-dropdown-font-size: 1rem;--bs-dropdown-color: var(--bs-body-color);--bs-dropdown-bg: var(--bs-body-bg);--bs-dropdown-border-color: var(--bs-border-color-translucent);--bs-dropdown-border-radius: var(--bs-border-radius);--bs-dropdown-border-width: var(--bs-border-width);--bs-dropdown-inner-border-radius: calc(var(--bs-border-radius) - var(--bs-border-width));--bs-dropdown-divider-bg: var(--bs-border-color-translucent);--bs-dropdown-divider-margin-y: .5rem;--bs-dropdown-box-shadow: var(--bs-box-shadow);--bs-dropdown-link-color: var(--bs-body-color);--bs-dropdown-link-hover-color: var(--bs-body-color);--bs-dropdown-link-hover-bg: var(--bs-tertiary-bg);--bs-dropdown-link-active-color: #fff;--bs-dropdown-link-active-bg: #0d6efd;--bs-dropdown-link-disabled-color: var(--bs-tertiary-color);--bs-dropdown-item-padding-x: 1rem;--bs-dropdown-item-padding-y: .25rem;--bs-dropdown-header-color: #6c757d;--bs-dropdown-header-padding-x: 1rem;--bs-dropdown-header-padding-y: .5rem;position:absolute;z-index:var(--bs-dropdown-zindex);display:none;min-width:var(--bs-dropdown-min-width);padding:var(--bs-dropdown-padding-y) var(--bs-dropdown-padding-x);margin:0;font-size:var(--bs-dropdown-font-size);color:var(--bs-dropdown-color);text-align:left;list-style:none;background-color:var(--bs-dropdown-bg);background-clip:padding-box;border:var(--bs-dropdown-border-width) solid var(--bs-dropdown-border-color);border-radius:var(--bs-dropdown-border-radius)}.dropdown-menu[data-bs-popper]{top:100%;left:0;margin-top:var(--bs-dropdown-spacer)}.dropdown-menu-start{--bs-position: start}.dropdown-menu-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-end{--bs-position: end}.dropdown-menu-end[data-bs-popper]{right:0;left:auto}@media (min-width: 576px){.dropdown-menu-sm-start{--bs-position: start}.dropdown-menu-sm-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-sm-end{--bs-position: end}.dropdown-menu-sm-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 768px){.dropdown-menu-md-start{--bs-position: start}.dropdown-menu-md-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-md-end{--bs-position: end}.dropdown-menu-md-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 992px){.dropdown-menu-lg-start{--bs-position: start}.dropdown-menu-lg-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-lg-end{--bs-position: end}.dropdown-menu-lg-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 1200px){.dropdown-menu-xl-start{--bs-position: start}.dropdown-menu-xl-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-xl-end{--bs-position: end}.dropdown-menu-xl-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 1400px){.dropdown-menu-xxl-start{--bs-position: start}.dropdown-menu-xxl-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-xxl-end{--bs-position: end}.dropdown-menu-xxl-end[data-bs-popper]{right:0;left:auto}}.dropup .dropdown-menu[data-bs-popper]{top:auto;bottom:100%;margin-top:0;margin-bottom:var(--bs-dropdown-spacer)}.dropup .dropdown-toggle:after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:"";border-top:0;border-right:.3em solid transparent;border-bottom:.3em solid;border-left:.3em solid transparent}.dropup .dropdown-toggle:empty:after{margin-left:0}.dropend .dropdown-menu[data-bs-popper]{top:0;right:auto;left:100%;margin-top:0;margin-left:var(--bs-dropdown-spacer)}.dropend .dropdown-toggle:after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:"";border-top:.3em solid transparent;border-right:0;border-bottom:.3em solid transparent;border-left:.3em solid}.dropend .dropdown-toggle:empty:after{margin-left:0}.dropend .dropdown-toggle:after{vertical-align:0}.dropstart .dropdown-menu[data-bs-popper]{top:0;right:100%;left:auto;margin-top:0;margin-right:var(--bs-dropdown-spacer)}.dropstart .dropdown-toggle:after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:""}.dropstart .dropdown-toggle:after{display:none}.dropstart .dropdown-toggle:before{display:inline-block;margin-right:.255em;vertical-align:.255em;content:"";border-top:.3em solid transparent;border-right:.3em solid;border-bottom:.3em solid transparent}.dropstart .dropdown-toggle:empty:after{margin-left:0}.dropstart .dropdown-toggle:before{vertical-align:0}.dropdown-divider{height:0;margin:var(--bs-dropdown-divider-margin-y) 0;overflow:hidden;border-top:1px solid var(--bs-dropdown-divider-bg);opacity:1}.dropdown-item{display:block;width:100%;padding:var(--bs-dropdown-item-padding-y) var(--bs-dropdown-item-padding-x);clear:both;font-weight:400;color:var(--bs-dropdown-link-color);text-align:inherit;text-decoration:none;white-space:nowrap;background-color:transparent;border:0;border-radius:var(--bs-dropdown-item-border-radius, 0)}.dropdown-item:hover,.dropdown-item:focus{color:var(--bs-dropdown-link-hover-color);background-color:var(--bs-dropdown-link-hover-bg)}.dropdown-item.active,.dropdown-item:active{color:var(--bs-dropdown-link-active-color);text-decoration:none;background-color:var(--bs-dropdown-link-active-bg)}.dropdown-item.disabled,.dropdown-item:disabled{color:var(--bs-dropdown-link-disabled-color);pointer-events:none;background-color:transparent}.dropdown-menu.show{display:block}.dropdown-header{display:block;padding:var(--bs-dropdown-header-padding-y) var(--bs-dropdown-header-padding-x);margin-bottom:0;font-size:.875rem;color:var(--bs-dropdown-header-color);white-space:nowrap}.dropdown-item-text{display:block;padding:var(--bs-dropdown-item-padding-y) var(--bs-dropdown-item-padding-x);color:var(--bs-dropdown-link-color)}.dropdown-menu-dark{--bs-dropdown-color: #dee2e6;--bs-dropdown-bg: #343a40;--bs-dropdown-border-color: var(--bs-border-color-translucent);--bs-dropdown-box-shadow: ;--bs-dropdown-link-color: #dee2e6;--bs-dropdown-link-hover-color: #fff;--bs-dropdown-divider-bg: var(--bs-border-color-translucent);--bs-dropdown-link-hover-bg: rgba(255, 255, 255, .15);--bs-dropdown-link-active-color: #fff;--bs-dropdown-link-active-bg: #0d6efd;--bs-dropdown-link-disabled-color: #adb5bd;--bs-dropdown-header-color: #adb5bd}.btn-group,.btn-group-vertical{position:relative;display:inline-flex;vertical-align:middle}.btn-group>.btn,.btn-group-vertical>.btn{position:relative;flex:1 1 auto}.btn-group>.btn-check:checked+.btn,.btn-group>.btn-check:focus+.btn,.btn-group>.btn:hover,.btn-group>.btn:focus,.btn-group>.btn:active,.btn-group>.btn.active,.btn-group-vertical>.btn-check:checked+.btn,.btn-group-vertical>.btn-check:focus+.btn,.btn-group-vertical>.btn:hover,.btn-group-vertical>.btn:focus,.btn-group-vertical>.btn:active,.btn-group-vertical>.btn.active{z-index:1}.btn-toolbar{display:flex;flex-wrap:wrap;justify-content:flex-start}.btn-toolbar .input-group{width:auto}.btn-group{border-radius:var(--bs-border-radius)}.btn-group>:not(.btn-check:first-child)+.btn,.btn-group>.btn-group:not(:first-child){margin-left:calc(var(--bs-border-width) * -1)}.btn-group>.btn:not(:last-child):not(.dropdown-toggle),.btn-group>.btn.dropdown-toggle-split:first-child,.btn-group>.btn-group:not(:last-child)>.btn{border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn:nth-child(n+3),.btn-group>:not(.btn-check)+.btn,.btn-group>.btn-group:not(:first-child)>.btn{border-top-left-radius:0;border-bottom-left-radius:0}.dropdown-toggle-split{padding-right:.5625rem;padding-left:.5625rem}.dropdown-toggle-split:after,.dropup .dropdown-toggle-split:after,.dropend .dropdown-toggle-split:after{margin-left:0}.dropstart .dropdown-toggle-split:before{margin-right:0}.btn-sm+.dropdown-toggle-split,.btn-group-sm>.btn+.dropdown-toggle-split{padding-right:.375rem;padding-left:.375rem}.btn-lg+.dropdown-toggle-split,.btn-group-lg>.btn+.dropdown-toggle-split{padding-right:.75rem;padding-left:.75rem}.btn-group-vertical{flex-direction:column;align-items:flex-start;justify-content:center}.btn-group-vertical>.btn,.btn-group-vertical>.btn-group{width:100%}.btn-group-vertical>.btn:not(:first-child),.btn-group-vertical>.btn-group:not(:first-child){margin-top:calc(var(--bs-border-width) * -1)}.btn-group-vertical>.btn:not(:last-child):not(.dropdown-toggle),.btn-group-vertical>.btn-group:not(:last-child)>.btn{border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn~.btn,.btn-group-vertical>.btn-group:not(:first-child)>.btn{border-top-left-radius:0;border-top-right-radius:0}.nav{--bs-nav-link-padding-x: 1rem;--bs-nav-link-padding-y: .5rem;--bs-nav-link-font-weight: ;--bs-nav-link-color: var(--bs-link-color);--bs-nav-link-hover-color: var(--bs-link-hover-color);--bs-nav-link-disabled-color: var(--bs-secondary-color);display:flex;flex-wrap:wrap;padding-left:0;margin-bottom:0;list-style:none}.nav-link{display:block;padding:var(--bs-nav-link-padding-y) var(--bs-nav-link-padding-x);font-size:var(--bs-nav-link-font-size);font-weight:var(--bs-nav-link-font-weight);color:var(--bs-nav-link-color);text-decoration:none;background:none;border:0;transition:color .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out}@media (prefers-reduced-motion: reduce){.nav-link{transition:none}}.nav-link:hover,.nav-link:focus{color:var(--bs-nav-link-hover-color)}.nav-link:focus-visible{outline:0;box-shadow:0 0 0 .25rem #0d6efd40}.nav-link.disabled,.nav-link:disabled{color:var(--bs-nav-link-disabled-color);pointer-events:none;cursor:default}.nav-tabs{--bs-nav-tabs-border-width: var(--bs-border-width);--bs-nav-tabs-border-color: var(--bs-border-color);--bs-nav-tabs-border-radius: var(--bs-border-radius);--bs-nav-tabs-link-hover-border-color: var(--bs-secondary-bg) var(--bs-secondary-bg) var(--bs-border-color);--bs-nav-tabs-link-active-color: var(--bs-emphasis-color);--bs-nav-tabs-link-active-bg: var(--bs-body-bg);--bs-nav-tabs-link-active-border-color: var(--bs-border-color) var(--bs-border-color) var(--bs-body-bg);border-bottom:var(--bs-nav-tabs-border-width) solid var(--bs-nav-tabs-border-color)}.nav-tabs .nav-link{margin-bottom:calc(-1 * var(--bs-nav-tabs-border-width));border:var(--bs-nav-tabs-border-width) solid transparent;border-top-left-radius:var(--bs-nav-tabs-border-radius);border-top-right-radius:var(--bs-nav-tabs-border-radius)}.nav-tabs .nav-link:hover,.nav-tabs .nav-link:focus{isolation:isolate;border-color:var(--bs-nav-tabs-link-hover-border-color)}.nav-tabs .nav-link.active,.nav-tabs .nav-item.show .nav-link{color:var(--bs-nav-tabs-link-active-color);background-color:var(--bs-nav-tabs-link-active-bg);border-color:var(--bs-nav-tabs-link-active-border-color)}.nav-tabs .dropdown-menu{margin-top:calc(-1 * var(--bs-nav-tabs-border-width));border-top-left-radius:0;border-top-right-radius:0}.nav-pills{--bs-nav-pills-border-radius: var(--bs-border-radius);--bs-nav-pills-link-active-color: #fff;--bs-nav-pills-link-active-bg: #0d6efd}.nav-pills .nav-link{border-radius:var(--bs-nav-pills-border-radius)}.nav-pills .nav-link.active,.nav-pills .show>.nav-link{color:var(--bs-nav-pills-link-active-color);background-color:var(--bs-nav-pills-link-active-bg)}.nav-underline{--bs-nav-underline-gap: 1rem;--bs-nav-underline-border-width: .125rem;--bs-nav-underline-link-active-color: var(--bs-emphasis-color);gap:var(--bs-nav-underline-gap)}.nav-underline .nav-link{padding-right:0;padding-left:0;border-bottom:var(--bs-nav-underline-border-width) solid transparent}.nav-underline .nav-link:hover,.nav-underline .nav-link:focus{border-bottom-color:currentcolor}.nav-underline .nav-link.active,.nav-underline .show>.nav-link{font-weight:700;color:var(--bs-nav-underline-link-active-color);border-bottom-color:currentcolor}.nav-fill>.nav-link,.nav-fill .nav-item{flex:1 1 auto;text-align:center}.nav-justified>.nav-link,.nav-justified .nav-item{flex-basis:0;flex-grow:1;text-align:center}.nav-fill .nav-item .nav-link,.nav-justified .nav-item .nav-link{width:100%}.tab-content>.tab-pane{display:none}.tab-content>.active{display:block}.navbar{--bs-navbar-padding-x: 0;--bs-navbar-padding-y: .5rem;--bs-navbar-color: rgba(var(--bs-emphasis-color-rgb), .65);--bs-navbar-hover-color: rgba(var(--bs-emphasis-color-rgb), .8);--bs-navbar-disabled-color: rgba(var(--bs-emphasis-color-rgb), .3);--bs-navbar-active-color: rgba(var(--bs-emphasis-color-rgb), 1);--bs-navbar-brand-padding-y: .3125rem;--bs-navbar-brand-margin-end: 1rem;--bs-navbar-brand-font-size: 1.25rem;--bs-navbar-brand-color: rgba(var(--bs-emphasis-color-rgb), 1);--bs-navbar-brand-hover-color: rgba(var(--bs-emphasis-color-rgb), 1);--bs-navbar-nav-link-padding-x: .5rem;--bs-navbar-toggler-padding-y: .25rem;--bs-navbar-toggler-padding-x: .75rem;--bs-navbar-toggler-font-size: 1.25rem;--bs-navbar-toggler-icon-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%2833, 37, 41, 0.75%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");--bs-navbar-toggler-border-color: rgba(var(--bs-emphasis-color-rgb), .15);--bs-navbar-toggler-border-radius: var(--bs-border-radius);--bs-navbar-toggler-focus-width: .25rem;--bs-navbar-toggler-transition: box-shadow .15s ease-in-out;position:relative;display:flex;flex-wrap:wrap;align-items:center;justify-content:space-between;padding:var(--bs-navbar-padding-y) var(--bs-navbar-padding-x)}.navbar>.container,.navbar>.container-fluid,.navbar>.container-sm,.navbar>.container-md,.navbar>.container-lg,.navbar>.container-xl,.navbar>.container-xxl{display:flex;flex-wrap:inherit;align-items:center;justify-content:space-between}.navbar-brand{padding-top:var(--bs-navbar-brand-padding-y);padding-bottom:var(--bs-navbar-brand-padding-y);margin-right:var(--bs-navbar-brand-margin-end);font-size:var(--bs-navbar-brand-font-size);color:var(--bs-navbar-brand-color);text-decoration:none;white-space:nowrap}.navbar-brand:hover,.navbar-brand:focus{color:var(--bs-navbar-brand-hover-color)}.navbar-nav{--bs-nav-link-padding-x: 0;--bs-nav-link-padding-y: .5rem;--bs-nav-link-font-weight: ;--bs-nav-link-color: var(--bs-navbar-color);--bs-nav-link-hover-color: var(--bs-navbar-hover-color);--bs-nav-link-disabled-color: var(--bs-navbar-disabled-color);display:flex;flex-direction:column;padding-left:0;margin-bottom:0;list-style:none}.navbar-nav .nav-link.active,.navbar-nav .nav-link.show{color:var(--bs-navbar-active-color)}.navbar-nav .dropdown-menu{position:static}.navbar-text{padding-top:.5rem;padding-bottom:.5rem;color:var(--bs-navbar-color)}.navbar-text a,.navbar-text a:hover,.navbar-text a:focus{color:var(--bs-navbar-active-color)}.navbar-collapse{flex-basis:100%;flex-grow:1;align-items:center}.navbar-toggler{padding:var(--bs-navbar-toggler-padding-y) var(--bs-navbar-toggler-padding-x);font-size:var(--bs-navbar-toggler-font-size);line-height:1;color:var(--bs-navbar-color);background-color:transparent;border:var(--bs-border-width) solid var(--bs-navbar-toggler-border-color);border-radius:var(--bs-navbar-toggler-border-radius);transition:var(--bs-navbar-toggler-transition)}@media (prefers-reduced-motion: reduce){.navbar-toggler{transition:none}}.navbar-toggler:hover{text-decoration:none}.navbar-toggler:focus{text-decoration:none;outline:0;box-shadow:0 0 0 var(--bs-navbar-toggler-focus-width)}.navbar-toggler-icon{display:inline-block;width:1.5em;height:1.5em;vertical-align:middle;background-image:var(--bs-navbar-toggler-icon-bg);background-repeat:no-repeat;background-position:center;background-size:100%}.navbar-nav-scroll{max-height:var(--bs-scroll-height, 75vh);overflow-y:auto}@media (min-width: 576px){.navbar-expand-sm{flex-wrap:nowrap;justify-content:flex-start}.navbar-expand-sm .navbar-nav{flex-direction:row}.navbar-expand-sm .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-sm .navbar-nav .nav-link{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-sm .navbar-nav-scroll{overflow:visible}.navbar-expand-sm .navbar-collapse{display:flex!important;flex-basis:auto}.navbar-expand-sm .navbar-toggler{display:none}.navbar-expand-sm .offcanvas{position:static;z-index:auto;flex-grow:1;width:auto!important;height:auto!important;visibility:visible!important;background-color:transparent!important;border:0!important;transform:none!important;transition:none}.navbar-expand-sm .offcanvas .offcanvas-header{display:none}.navbar-expand-sm .offcanvas .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 768px){.navbar-expand-md{flex-wrap:nowrap;justify-content:flex-start}.navbar-expand-md .navbar-nav{flex-direction:row}.navbar-expand-md .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-md .navbar-nav .nav-link{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-md .navbar-nav-scroll{overflow:visible}.navbar-expand-md .navbar-collapse{display:flex!important;flex-basis:auto}.navbar-expand-md .navbar-toggler{display:none}.navbar-expand-md .offcanvas{position:static;z-index:auto;flex-grow:1;width:auto!important;height:auto!important;visibility:visible!important;background-color:transparent!important;border:0!important;transform:none!important;transition:none}.navbar-expand-md .offcanvas .offcanvas-header{display:none}.navbar-expand-md .offcanvas .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 992px){.navbar-expand-lg{flex-wrap:nowrap;justify-content:flex-start}.navbar-expand-lg .navbar-nav{flex-direction:row}.navbar-expand-lg .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-lg .navbar-nav .nav-link{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-lg .navbar-nav-scroll{overflow:visible}.navbar-expand-lg .navbar-collapse{display:flex!important;flex-basis:auto}.navbar-expand-lg .navbar-toggler{display:none}.navbar-expand-lg .offcanvas{position:static;z-index:auto;flex-grow:1;width:auto!important;height:auto!important;visibility:visible!important;background-color:transparent!important;border:0!important;transform:none!important;transition:none}.navbar-expand-lg .offcanvas .offcanvas-header{display:none}.navbar-expand-lg .offcanvas .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 1200px){.navbar-expand-xl{flex-wrap:nowrap;justify-content:flex-start}.navbar-expand-xl .navbar-nav{flex-direction:row}.navbar-expand-xl .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-xl .navbar-nav .nav-link{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-xl .navbar-nav-scroll{overflow:visible}.navbar-expand-xl .navbar-collapse{display:flex!important;flex-basis:auto}.navbar-expand-xl .navbar-toggler{display:none}.navbar-expand-xl .offcanvas{position:static;z-index:auto;flex-grow:1;width:auto!important;height:auto!important;visibility:visible!important;background-color:transparent!important;border:0!important;transform:none!important;transition:none}.navbar-expand-xl .offcanvas .offcanvas-header{display:none}.navbar-expand-xl .offcanvas .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 1400px){.navbar-expand-xxl{flex-wrap:nowrap;justify-content:flex-start}.navbar-expand-xxl .navbar-nav{flex-direction:row}.navbar-expand-xxl .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-xxl .navbar-nav .nav-link{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-xxl .navbar-nav-scroll{overflow:visible}.navbar-expand-xxl .navbar-collapse{display:flex!important;flex-basis:auto}.navbar-expand-xxl .navbar-toggler{display:none}.navbar-expand-xxl .offcanvas{position:static;z-index:auto;flex-grow:1;width:auto!important;height:auto!important;visibility:visible!important;background-color:transparent!important;border:0!important;transform:none!important;transition:none}.navbar-expand-xxl .offcanvas .offcanvas-header{display:none}.navbar-expand-xxl .offcanvas .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible}}.navbar-expand{flex-wrap:nowrap;justify-content:flex-start}.navbar-expand .navbar-nav{flex-direction:row}.navbar-expand .navbar-nav .dropdown-menu{position:absolute}.navbar-expand .navbar-nav .nav-link{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand .navbar-nav-scroll{overflow:visible}.navbar-expand .navbar-collapse{display:flex!important;flex-basis:auto}.navbar-expand .navbar-toggler{display:none}.navbar-expand .offcanvas{position:static;z-index:auto;flex-grow:1;width:auto!important;height:auto!important;visibility:visible!important;background-color:transparent!important;border:0!important;transform:none!important;transition:none}.navbar-expand .offcanvas .offcanvas-header{display:none}.navbar-expand .offcanvas .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible}.navbar-dark,.navbar[data-bs-theme=dark]{--bs-navbar-color: rgba(255, 255, 255, .55);--bs-navbar-hover-color: rgba(255, 255, 255, .75);--bs-navbar-disabled-color: rgba(255, 255, 255, .25);--bs-navbar-active-color: #fff;--bs-navbar-brand-color: #fff;--bs-navbar-brand-hover-color: #fff;--bs-navbar-toggler-border-color: rgba(255, 255, 255, .1);--bs-navbar-toggler-icon-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%28255, 255, 255, 0.55%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e")}[data-bs-theme=dark] .navbar-toggler-icon{--bs-navbar-toggler-icon-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%28255, 255, 255, 0.55%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e")}.card{--bs-card-spacer-y: 1rem;--bs-card-spacer-x: 1rem;--bs-card-title-spacer-y: .5rem;--bs-card-title-color: ;--bs-card-subtitle-color: ;--bs-card-border-width: var(--bs-border-width);--bs-card-border-color: var(--bs-border-color-translucent);--bs-card-border-radius: var(--bs-border-radius);--bs-card-box-shadow: ;--bs-card-inner-border-radius: calc(var(--bs-border-radius) - (var(--bs-border-width)));--bs-card-cap-padding-y: .5rem;--bs-card-cap-padding-x: 1rem;--bs-card-cap-bg: rgba(var(--bs-body-color-rgb), .03);--bs-card-cap-color: ;--bs-card-height: ;--bs-card-color: ;--bs-card-bg: var(--bs-body-bg);--bs-card-img-overlay-padding: 1rem;--bs-card-group-margin: .75rem;position:relative;display:flex;flex-direction:column;min-width:0;height:var(--bs-card-height);color:var(--bs-body-color);word-wrap:break-word;background-color:var(--bs-card-bg);background-clip:border-box;border:var(--bs-card-border-width) solid var(--bs-card-border-color);border-radius:var(--bs-card-border-radius)}.card>hr{margin-right:0;margin-left:0}.card>.list-group{border-top:inherit;border-bottom:inherit}.card>.list-group:first-child{border-top-width:0;border-top-left-radius:var(--bs-card-inner-border-radius);border-top-right-radius:var(--bs-card-inner-border-radius)}.card>.list-group:last-child{border-bottom-width:0;border-bottom-right-radius:var(--bs-card-inner-border-radius);border-bottom-left-radius:var(--bs-card-inner-border-radius)}.card>.card-header+.list-group,.card>.list-group+.card-footer{border-top:0}.card-body{flex:1 1 auto;padding:var(--bs-card-spacer-y) var(--bs-card-spacer-x);color:var(--bs-card-color)}.card-title{margin-bottom:var(--bs-card-title-spacer-y);color:var(--bs-card-title-color)}.card-subtitle{margin-top:calc(-.5 * var(--bs-card-title-spacer-y));margin-bottom:0;color:var(--bs-card-subtitle-color)}.card-text:last-child{margin-bottom:0}.card-link+.card-link{margin-left:var(--bs-card-spacer-x)}.card-header{padding:var(--bs-card-cap-padding-y) var(--bs-card-cap-padding-x);margin-bottom:0;color:var(--bs-card-cap-color);background-color:var(--bs-card-cap-bg);border-bottom:var(--bs-card-border-width) solid var(--bs-card-border-color)}.card-header:first-child{border-radius:var(--bs-card-inner-border-radius) var(--bs-card-inner-border-radius) 0 0}.card-footer{padding:var(--bs-card-cap-padding-y) var(--bs-card-cap-padding-x);color:var(--bs-card-cap-color);background-color:var(--bs-card-cap-bg);border-top:var(--bs-card-border-width) solid var(--bs-card-border-color)}.card-footer:last-child{border-radius:0 0 var(--bs-card-inner-border-radius) var(--bs-card-inner-border-radius)}.card-header-tabs{margin-right:calc(-.5 * var(--bs-card-cap-padding-x));margin-bottom:calc(-1 * var(--bs-card-cap-padding-y));margin-left:calc(-.5 * var(--bs-card-cap-padding-x));border-bottom:0}.card-header-tabs .nav-link.active{background-color:var(--bs-card-bg);border-bottom-color:var(--bs-card-bg)}.card-header-pills{margin-right:calc(-.5 * var(--bs-card-cap-padding-x));margin-left:calc(-.5 * var(--bs-card-cap-padding-x))}.card-img-overlay{position:absolute;inset:0;padding:var(--bs-card-img-overlay-padding);border-radius:var(--bs-card-inner-border-radius)}.card-img,.card-img-top,.card-img-bottom{width:100%}.card-img,.card-img-top{border-top-left-radius:var(--bs-card-inner-border-radius);border-top-right-radius:var(--bs-card-inner-border-radius)}.card-img,.card-img-bottom{border-bottom-right-radius:var(--bs-card-inner-border-radius);border-bottom-left-radius:var(--bs-card-inner-border-radius)}.card-group>.card{margin-bottom:var(--bs-card-group-margin)}@media (min-width: 576px){.card-group{display:flex;flex-flow:row wrap}.card-group>.card{flex:1 0 0%;margin-bottom:0}.card-group>.card+.card{margin-left:0;border-left:0}.card-group>.card:not(:last-child){border-top-right-radius:0;border-bottom-right-radius:0}.card-group>.card:not(:last-child) .card-img-top,.card-group>.card:not(:last-child) .card-header{border-top-right-radius:0}.card-group>.card:not(:last-child) .card-img-bottom,.card-group>.card:not(:last-child) .card-footer{border-bottom-right-radius:0}.card-group>.card:not(:first-child){border-top-left-radius:0;border-bottom-left-radius:0}.card-group>.card:not(:first-child) .card-img-top,.card-group>.card:not(:first-child) .card-header{border-top-left-radius:0}.card-group>.card:not(:first-child) .card-img-bottom,.card-group>.card:not(:first-child) .card-footer{border-bottom-left-radius:0}}.accordion{--bs-accordion-color: var(--bs-body-color);--bs-accordion-bg: var(--bs-body-bg);--bs-accordion-transition: color .15s ease-in-out, background-color .15s ease-in-out, border-color .15s ease-in-out, box-shadow .15s ease-in-out, border-radius .15s ease;--bs-accordion-border-color: var(--bs-border-color);--bs-accordion-border-width: var(--bs-border-width);--bs-accordion-border-radius: var(--bs-border-radius);--bs-accordion-inner-border-radius: calc(var(--bs-border-radius) - (var(--bs-border-width)));--bs-accordion-btn-padding-x: 1.25rem;--bs-accordion-btn-padding-y: 1rem;--bs-accordion-btn-color: var(--bs-body-color);--bs-accordion-btn-bg: var(--bs-accordion-bg);--bs-accordion-btn-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23212529'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");--bs-accordion-btn-icon-width: 1.25rem;--bs-accordion-btn-icon-transform: rotate(-180deg);--bs-accordion-btn-icon-transition: transform .2s ease-in-out;--bs-accordion-btn-active-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23052c65'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");--bs-accordion-btn-focus-border-color: #86b7fe;--bs-accordion-btn-focus-box-shadow: 0 0 0 .25rem rgba(13, 110, 253, .25);--bs-accordion-body-padding-x: 1.25rem;--bs-accordion-body-padding-y: 1rem;--bs-accordion-active-color: var(--bs-primary-text-emphasis);--bs-accordion-active-bg: var(--bs-primary-bg-subtle)}.accordion-button{position:relative;display:flex;align-items:center;width:100%;padding:var(--bs-accordion-btn-padding-y) var(--bs-accordion-btn-padding-x);font-size:1rem;color:var(--bs-accordion-btn-color);text-align:left;background-color:var(--bs-accordion-btn-bg);border:0;border-radius:0;overflow-anchor:none;transition:var(--bs-accordion-transition)}@media (prefers-reduced-motion: reduce){.accordion-button{transition:none}}.accordion-button:not(.collapsed){color:var(--bs-accordion-active-color);background-color:var(--bs-accordion-active-bg);box-shadow:inset 0 calc(-1 * var(--bs-accordion-border-width)) 0 var(--bs-accordion-border-color)}.accordion-button:not(.collapsed):after{background-image:var(--bs-accordion-btn-active-icon);transform:var(--bs-accordion-btn-icon-transform)}.accordion-button:after{flex-shrink:0;width:var(--bs-accordion-btn-icon-width);height:var(--bs-accordion-btn-icon-width);margin-left:auto;content:"";background-image:var(--bs-accordion-btn-icon);background-repeat:no-repeat;background-size:var(--bs-accordion-btn-icon-width);transition:var(--bs-accordion-btn-icon-transition)}@media (prefers-reduced-motion: reduce){.accordion-button:after{transition:none}}.accordion-button:hover{z-index:2}.accordion-button:focus{z-index:3;border-color:var(--bs-accordion-btn-focus-border-color);outline:0;box-shadow:var(--bs-accordion-btn-focus-box-shadow)}.accordion-header{margin-bottom:0}.accordion-item{color:var(--bs-accordion-color);background-color:var(--bs-accordion-bg);border:var(--bs-accordion-border-width) solid var(--bs-accordion-border-color)}.accordion-item:first-of-type{border-top-left-radius:var(--bs-accordion-border-radius);border-top-right-radius:var(--bs-accordion-border-radius)}.accordion-item:first-of-type .accordion-button{border-top-left-radius:var(--bs-accordion-inner-border-radius);border-top-right-radius:var(--bs-accordion-inner-border-radius)}.accordion-item:not(:first-of-type){border-top:0}.accordion-item:last-of-type{border-bottom-right-radius:var(--bs-accordion-border-radius);border-bottom-left-radius:var(--bs-accordion-border-radius)}.accordion-item:last-of-type .accordion-button.collapsed{border-bottom-right-radius:var(--bs-accordion-inner-border-radius);border-bottom-left-radius:var(--bs-accordion-inner-border-radius)}.accordion-item:last-of-type .accordion-collapse{border-bottom-right-radius:var(--bs-accordion-border-radius);border-bottom-left-radius:var(--bs-accordion-border-radius)}.accordion-body{padding:var(--bs-accordion-body-padding-y) var(--bs-accordion-body-padding-x)}.accordion-flush .accordion-collapse{border-width:0}.accordion-flush .accordion-item{border-right:0;border-left:0;border-radius:0}.accordion-flush .accordion-item:first-child{border-top:0}.accordion-flush .accordion-item:last-child{border-bottom:0}.accordion-flush .accordion-item .accordion-button,.accordion-flush .accordion-item .accordion-button.collapsed{border-radius:0}[data-bs-theme=dark] .accordion-button:after{--bs-accordion-btn-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%236ea8fe'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");--bs-accordion-btn-active-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%236ea8fe'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e")}.breadcrumb{--bs-breadcrumb-padding-x: 0;--bs-breadcrumb-padding-y: 0;--bs-breadcrumb-margin-bottom: 1rem;--bs-breadcrumb-bg: ;--bs-breadcrumb-border-radius: ;--bs-breadcrumb-divider-color: var(--bs-secondary-color);--bs-breadcrumb-item-padding-x: .5rem;--bs-breadcrumb-item-active-color: var(--bs-secondary-color);display:flex;flex-wrap:wrap;padding:var(--bs-breadcrumb-padding-y) var(--bs-breadcrumb-padding-x);margin-bottom:var(--bs-breadcrumb-margin-bottom);font-size:var(--bs-breadcrumb-font-size);list-style:none;background-color:var(--bs-breadcrumb-bg);border-radius:var(--bs-breadcrumb-border-radius)}.breadcrumb-item+.breadcrumb-item{padding-left:var(--bs-breadcrumb-item-padding-x)}.breadcrumb-item+.breadcrumb-item:before{float:left;padding-right:var(--bs-breadcrumb-item-padding-x);color:var(--bs-breadcrumb-divider-color);content:var(--bs-breadcrumb-divider, "/")}.breadcrumb-item.active{color:var(--bs-breadcrumb-item-active-color)}.pagination{--bs-pagination-padding-x: .75rem;--bs-pagination-padding-y: .375rem;--bs-pagination-font-size: 1rem;--bs-pagination-color: var(--bs-link-color);--bs-pagination-bg: var(--bs-body-bg);--bs-pagination-border-width: var(--bs-border-width);--bs-pagination-border-color: var(--bs-border-color);--bs-pagination-border-radius: var(--bs-border-radius);--bs-pagination-hover-color: var(--bs-link-hover-color);--bs-pagination-hover-bg: var(--bs-tertiary-bg);--bs-pagination-hover-border-color: var(--bs-border-color);--bs-pagination-focus-color: var(--bs-link-hover-color);--bs-pagination-focus-bg: var(--bs-secondary-bg);--bs-pagination-focus-box-shadow: 0 0 0 .25rem rgba(13, 110, 253, .25);--bs-pagination-active-color: #fff;--bs-pagination-active-bg: #0d6efd;--bs-pagination-active-border-color: #0d6efd;--bs-pagination-disabled-color: var(--bs-secondary-color);--bs-pagination-disabled-bg: var(--bs-secondary-bg);--bs-pagination-disabled-border-color: var(--bs-border-color);display:flex;padding-left:0;list-style:none}.page-link{position:relative;display:block;padding:var(--bs-pagination-padding-y) var(--bs-pagination-padding-x);font-size:var(--bs-pagination-font-size);color:var(--bs-pagination-color);text-decoration:none;background-color:var(--bs-pagination-bg);border:var(--bs-pagination-border-width) solid var(--bs-pagination-border-color);transition:color .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out}@media (prefers-reduced-motion: reduce){.page-link{transition:none}}.page-link:hover{z-index:2;color:var(--bs-pagination-hover-color);background-color:var(--bs-pagination-hover-bg);border-color:var(--bs-pagination-hover-border-color)}.page-link:focus{z-index:3;color:var(--bs-pagination-focus-color);background-color:var(--bs-pagination-focus-bg);outline:0;box-shadow:var(--bs-pagination-focus-box-shadow)}.page-link.active,.active>.page-link{z-index:3;color:var(--bs-pagination-active-color);background-color:var(--bs-pagination-active-bg);border-color:var(--bs-pagination-active-border-color)}.page-link.disabled,.disabled>.page-link{color:var(--bs-pagination-disabled-color);pointer-events:none;background-color:var(--bs-pagination-disabled-bg);border-color:var(--bs-pagination-disabled-border-color)}.page-item:not(:first-child) .page-link{margin-left:calc(var(--bs-border-width) * -1)}.page-item:first-child .page-link{border-top-left-radius:var(--bs-pagination-border-radius);border-bottom-left-radius:var(--bs-pagination-border-radius)}.page-item:last-child .page-link{border-top-right-radius:var(--bs-pagination-border-radius);border-bottom-right-radius:var(--bs-pagination-border-radius)}.pagination-lg{--bs-pagination-padding-x: 1.5rem;--bs-pagination-padding-y: .75rem;--bs-pagination-font-size: 1.25rem;--bs-pagination-border-radius: var(--bs-border-radius-lg)}.pagination-sm{--bs-pagination-padding-x: .5rem;--bs-pagination-padding-y: .25rem;--bs-pagination-font-size: .875rem;--bs-pagination-border-radius: var(--bs-border-radius-sm)}.badge{--bs-badge-padding-x: .65em;--bs-badge-padding-y: .35em;--bs-badge-font-size: .75em;--bs-badge-font-weight: 700;--bs-badge-color: #fff;--bs-badge-border-radius: var(--bs-border-radius);display:inline-block;padding:var(--bs-badge-padding-y) var(--bs-badge-padding-x);font-size:var(--bs-badge-font-size);font-weight:var(--bs-badge-font-weight);line-height:1;color:var(--bs-badge-color);text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:var(--bs-badge-border-radius)}.badge:empty{display:none}.btn .badge{position:relative;top:-1px}.alert{--bs-alert-bg: transparent;--bs-alert-padding-x: 1rem;--bs-alert-padding-y: 1rem;--bs-alert-margin-bottom: 1rem;--bs-alert-color: inherit;--bs-alert-border-color: transparent;--bs-alert-border: var(--bs-border-width) solid var(--bs-alert-border-color);--bs-alert-border-radius: var(--bs-border-radius);--bs-alert-link-color: inherit;position:relative;padding:var(--bs-alert-padding-y) var(--bs-alert-padding-x);margin-bottom:var(--bs-alert-margin-bottom);color:var(--bs-alert-color);background-color:var(--bs-alert-bg);border:var(--bs-alert-border);border-radius:var(--bs-alert-border-radius)}.alert-heading{color:inherit}.alert-link{font-weight:700;color:var(--bs-alert-link-color)}.alert-dismissible{padding-right:3rem}.alert-dismissible .btn-close{position:absolute;top:0;right:0;z-index:2;padding:1.25rem 1rem}.alert-primary{--bs-alert-color: var(--bs-primary-text-emphasis);--bs-alert-bg: var(--bs-primary-bg-subtle);--bs-alert-border-color: var(--bs-primary-border-subtle);--bs-alert-link-color: var(--bs-primary-text-emphasis)}.alert-secondary{--bs-alert-color: var(--bs-secondary-text-emphasis);--bs-alert-bg: var(--bs-secondary-bg-subtle);--bs-alert-border-color: var(--bs-secondary-border-subtle);--bs-alert-link-color: var(--bs-secondary-text-emphasis)}.alert-success{--bs-alert-color: var(--bs-success-text-emphasis);--bs-alert-bg: var(--bs-success-bg-subtle);--bs-alert-border-color: var(--bs-success-border-subtle);--bs-alert-link-color: var(--bs-success-text-emphasis)}.alert-info{--bs-alert-color: var(--bs-info-text-emphasis);--bs-alert-bg: var(--bs-info-bg-subtle);--bs-alert-border-color: var(--bs-info-border-subtle);--bs-alert-link-color: var(--bs-info-text-emphasis)}.alert-warning{--bs-alert-color: var(--bs-warning-text-emphasis);--bs-alert-bg: var(--bs-warning-bg-subtle);--bs-alert-border-color: var(--bs-warning-border-subtle);--bs-alert-link-color: var(--bs-warning-text-emphasis)}.alert-danger{--bs-alert-color: var(--bs-danger-text-emphasis);--bs-alert-bg: var(--bs-danger-bg-subtle);--bs-alert-border-color: var(--bs-danger-border-subtle);--bs-alert-link-color: var(--bs-danger-text-emphasis)}.alert-light{--bs-alert-color: var(--bs-light-text-emphasis);--bs-alert-bg: var(--bs-light-bg-subtle);--bs-alert-border-color: var(--bs-light-border-subtle);--bs-alert-link-color: var(--bs-light-text-emphasis)}.alert-dark{--bs-alert-color: var(--bs-dark-text-emphasis);--bs-alert-bg: var(--bs-dark-bg-subtle);--bs-alert-border-color: var(--bs-dark-border-subtle);--bs-alert-link-color: var(--bs-dark-text-emphasis)}@keyframes progress-bar-stripes{0%{background-position-x:1rem}}.progress,.progress-stacked{--bs-progress-height: 1rem;--bs-progress-font-size: .75rem;--bs-progress-bg: var(--bs-secondary-bg);--bs-progress-border-radius: var(--bs-border-radius);--bs-progress-box-shadow: var(--bs-box-shadow-inset);--bs-progress-bar-color: #fff;--bs-progress-bar-bg: #0d6efd;--bs-progress-bar-transition: width .6s ease;display:flex;height:var(--bs-progress-height);overflow:hidden;font-size:var(--bs-progress-font-size);background-color:var(--bs-progress-bg);border-radius:var(--bs-progress-border-radius)}.progress-bar{display:flex;flex-direction:column;justify-content:center;overflow:hidden;color:var(--bs-progress-bar-color);text-align:center;white-space:nowrap;background-color:var(--bs-progress-bar-bg);transition:var(--bs-progress-bar-transition)}@media (prefers-reduced-motion: reduce){.progress-bar{transition:none}}.progress-bar-striped{background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-size:var(--bs-progress-height) var(--bs-progress-height)}.progress-stacked>.progress{overflow:visible}.progress-stacked>.progress>.progress-bar{width:100%}.progress-bar-animated{animation:1s linear infinite progress-bar-stripes}@media (prefers-reduced-motion: reduce){.progress-bar-animated{animation:none}}.list-group{--bs-list-group-color: var(--bs-body-color);--bs-list-group-bg: var(--bs-body-bg);--bs-list-group-border-color: var(--bs-border-color);--bs-list-group-border-width: var(--bs-border-width);--bs-list-group-border-radius: var(--bs-border-radius);--bs-list-group-item-padding-x: 1rem;--bs-list-group-item-padding-y: .5rem;--bs-list-group-action-color: var(--bs-secondary-color);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-tertiary-bg);--bs-list-group-action-active-color: var(--bs-body-color);--bs-list-group-action-active-bg: var(--bs-secondary-bg);--bs-list-group-disabled-color: var(--bs-secondary-color);--bs-list-group-disabled-bg: var(--bs-body-bg);--bs-list-group-active-color: #fff;--bs-list-group-active-bg: #0d6efd;--bs-list-group-active-border-color: #0d6efd;display:flex;flex-direction:column;padding-left:0;margin-bottom:0;border-radius:var(--bs-list-group-border-radius)}.list-group-numbered{list-style-type:none;counter-reset:section}.list-group-numbered>.list-group-item:before{content:counters(section,".") ". ";counter-increment:section}.list-group-item-action{width:100%;color:var(--bs-list-group-action-color);text-align:inherit}.list-group-item-action:hover,.list-group-item-action:focus{z-index:1;color:var(--bs-list-group-action-hover-color);text-decoration:none;background-color:var(--bs-list-group-action-hover-bg)}.list-group-item-action:active{color:var(--bs-list-group-action-active-color);background-color:var(--bs-list-group-action-active-bg)}.list-group-item{position:relative;display:block;padding:var(--bs-list-group-item-padding-y) var(--bs-list-group-item-padding-x);color:var(--bs-list-group-color);text-decoration:none;background-color:var(--bs-list-group-bg);border:var(--bs-list-group-border-width) solid var(--bs-list-group-border-color)}.list-group-item:first-child{border-top-left-radius:inherit;border-top-right-radius:inherit}.list-group-item:last-child{border-bottom-right-radius:inherit;border-bottom-left-radius:inherit}.list-group-item.disabled,.list-group-item:disabled{color:var(--bs-list-group-disabled-color);pointer-events:none;background-color:var(--bs-list-group-disabled-bg)}.list-group-item.active{z-index:2;color:var(--bs-list-group-active-color);background-color:var(--bs-list-group-active-bg);border-color:var(--bs-list-group-active-border-color)}.list-group-item+.list-group-item{border-top-width:0}.list-group-item+.list-group-item.active{margin-top:calc(-1 * var(--bs-list-group-border-width));border-top-width:var(--bs-list-group-border-width)}.list-group-horizontal{flex-direction:row}.list-group-horizontal>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal>.list-group-item.active{margin-top:0}.list-group-horizontal>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}@media (min-width: 576px){.list-group-horizontal-sm{flex-direction:row}.list-group-horizontal-sm>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-sm>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-sm>.list-group-item.active{margin-top:0}.list-group-horizontal-sm>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-sm>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 768px){.list-group-horizontal-md{flex-direction:row}.list-group-horizontal-md>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-md>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-md>.list-group-item.active{margin-top:0}.list-group-horizontal-md>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-md>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 992px){.list-group-horizontal-lg{flex-direction:row}.list-group-horizontal-lg>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-lg>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-lg>.list-group-item.active{margin-top:0}.list-group-horizontal-lg>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-lg>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 1200px){.list-group-horizontal-xl{flex-direction:row}.list-group-horizontal-xl>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-xl>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-xl>.list-group-item.active{margin-top:0}.list-group-horizontal-xl>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-xl>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 1400px){.list-group-horizontal-xxl{flex-direction:row}.list-group-horizontal-xxl>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-xxl>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-xxl>.list-group-item.active{margin-top:0}.list-group-horizontal-xxl>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-xxl>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}.list-group-flush{border-radius:0}.list-group-flush>.list-group-item{border-width:0 0 var(--bs-list-group-border-width)}.list-group-flush>.list-group-item:last-child{border-bottom-width:0}.list-group-item-primary{--bs-list-group-color: var(--bs-primary-text-emphasis);--bs-list-group-bg: var(--bs-primary-bg-subtle);--bs-list-group-border-color: var(--bs-primary-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-primary-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-primary-border-subtle);--bs-list-group-active-color: var(--bs-primary-bg-subtle);--bs-list-group-active-bg: var(--bs-primary-text-emphasis);--bs-list-group-active-border-color: var(--bs-primary-text-emphasis)}.list-group-item-secondary{--bs-list-group-color: var(--bs-secondary-text-emphasis);--bs-list-group-bg: var(--bs-secondary-bg-subtle);--bs-list-group-border-color: var(--bs-secondary-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-secondary-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-secondary-border-subtle);--bs-list-group-active-color: var(--bs-secondary-bg-subtle);--bs-list-group-active-bg: var(--bs-secondary-text-emphasis);--bs-list-group-active-border-color: var(--bs-secondary-text-emphasis)}.list-group-item-success{--bs-list-group-color: var(--bs-success-text-emphasis);--bs-list-group-bg: var(--bs-success-bg-subtle);--bs-list-group-border-color: var(--bs-success-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-success-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-success-border-subtle);--bs-list-group-active-color: var(--bs-success-bg-subtle);--bs-list-group-active-bg: var(--bs-success-text-emphasis);--bs-list-group-active-border-color: var(--bs-success-text-emphasis)}.list-group-item-info{--bs-list-group-color: var(--bs-info-text-emphasis);--bs-list-group-bg: var(--bs-info-bg-subtle);--bs-list-group-border-color: var(--bs-info-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-info-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-info-border-subtle);--bs-list-group-active-color: var(--bs-info-bg-subtle);--bs-list-group-active-bg: var(--bs-info-text-emphasis);--bs-list-group-active-border-color: var(--bs-info-text-emphasis)}.list-group-item-warning{--bs-list-group-color: var(--bs-warning-text-emphasis);--bs-list-group-bg: var(--bs-warning-bg-subtle);--bs-list-group-border-color: var(--bs-warning-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-warning-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-warning-border-subtle);--bs-list-group-active-color: var(--bs-warning-bg-subtle);--bs-list-group-active-bg: var(--bs-warning-text-emphasis);--bs-list-group-active-border-color: var(--bs-warning-text-emphasis)}.list-group-item-danger{--bs-list-group-color: var(--bs-danger-text-emphasis);--bs-list-group-bg: var(--bs-danger-bg-subtle);--bs-list-group-border-color: var(--bs-danger-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-danger-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-danger-border-subtle);--bs-list-group-active-color: var(--bs-danger-bg-subtle);--bs-list-group-active-bg: var(--bs-danger-text-emphasis);--bs-list-group-active-border-color: var(--bs-danger-text-emphasis)}.list-group-item-light{--bs-list-group-color: var(--bs-light-text-emphasis);--bs-list-group-bg: var(--bs-light-bg-subtle);--bs-list-group-border-color: var(--bs-light-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-light-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-light-border-subtle);--bs-list-group-active-color: var(--bs-light-bg-subtle);--bs-list-group-active-bg: var(--bs-light-text-emphasis);--bs-list-group-active-border-color: var(--bs-light-text-emphasis)}.list-group-item-dark{--bs-list-group-color: var(--bs-dark-text-emphasis);--bs-list-group-bg: var(--bs-dark-bg-subtle);--bs-list-group-border-color: var(--bs-dark-border-subtle);--bs-list-group-action-hover-color: var(--bs-emphasis-color);--bs-list-group-action-hover-bg: var(--bs-dark-border-subtle);--bs-list-group-action-active-color: var(--bs-emphasis-color);--bs-list-group-action-active-bg: var(--bs-dark-border-subtle);--bs-list-group-active-color: var(--bs-dark-bg-subtle);--bs-list-group-active-bg: var(--bs-dark-text-emphasis);--bs-list-group-active-border-color: var(--bs-dark-text-emphasis)}.btn-close{--bs-btn-close-color: #000;--bs-btn-close-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23000'%3e%3cpath d='M.293.293a1 1 0 0 1 1.414 0L8 6.586 14.293.293a1 1 0 1 1 1.414 1.414L9.414 8l6.293 6.293a1 1 0 0 1-1.414 1.414L8 9.414l-6.293 6.293a1 1 0 0 1-1.414-1.414L6.586 8 .293 1.707a1 1 0 0 1 0-1.414z'/%3e%3c/svg%3e");--bs-btn-close-opacity: .5;--bs-btn-close-hover-opacity: .75;--bs-btn-close-focus-shadow: 0 0 0 .25rem rgba(13, 110, 253, .25);--bs-btn-close-focus-opacity: 1;--bs-btn-close-disabled-opacity: .25;--bs-btn-close-white-filter: invert(1) grayscale(100%) brightness(200%);box-sizing:content-box;width:1em;height:1em;padding:.25em;color:var(--bs-btn-close-color);background:transparent var(--bs-btn-close-bg) center/1em auto no-repeat;border:0;border-radius:.375rem;opacity:var(--bs-btn-close-opacity)}.btn-close:hover{color:var(--bs-btn-close-color);text-decoration:none;opacity:var(--bs-btn-close-hover-opacity)}.btn-close:focus{outline:0;box-shadow:var(--bs-btn-close-focus-shadow);opacity:var(--bs-btn-close-focus-opacity)}.btn-close:disabled,.btn-close.disabled{pointer-events:none;user-select:none;opacity:var(--bs-btn-close-disabled-opacity)}.btn-close-white,[data-bs-theme=dark] .btn-close{filter:var(--bs-btn-close-white-filter)}.toast{--bs-toast-zindex: 1090;--bs-toast-padding-x: .75rem;--bs-toast-padding-y: .5rem;--bs-toast-spacing: 1.5rem;--bs-toast-max-width: 350px;--bs-toast-font-size: .875rem;--bs-toast-color: ;--bs-toast-bg: rgba(var(--bs-body-bg-rgb), .85);--bs-toast-border-width: var(--bs-border-width);--bs-toast-border-color: var(--bs-border-color-translucent);--bs-toast-border-radius: var(--bs-border-radius);--bs-toast-box-shadow: var(--bs-box-shadow);--bs-toast-header-color: var(--bs-secondary-color);--bs-toast-header-bg: rgba(var(--bs-body-bg-rgb), .85);--bs-toast-header-border-color: var(--bs-border-color-translucent);width:var(--bs-toast-max-width);max-width:100%;font-size:var(--bs-toast-font-size);color:var(--bs-toast-color);pointer-events:auto;background-color:var(--bs-toast-bg);background-clip:padding-box;border:var(--bs-toast-border-width) solid var(--bs-toast-border-color);box-shadow:var(--bs-toast-box-shadow);border-radius:var(--bs-toast-border-radius)}.toast.showing{opacity:0}.toast:not(.show){display:none}.toast-container{--bs-toast-zindex: 1090;position:absolute;z-index:var(--bs-toast-zindex);width:max-content;max-width:100%;pointer-events:none}.toast-container>:not(:last-child){margin-bottom:var(--bs-toast-spacing)}.toast-header{display:flex;align-items:center;padding:var(--bs-toast-padding-y) var(--bs-toast-padding-x);color:var(--bs-toast-header-color);background-color:var(--bs-toast-header-bg);background-clip:padding-box;border-bottom:var(--bs-toast-border-width) solid var(--bs-toast-header-border-color);border-top-left-radius:calc(var(--bs-toast-border-radius) - var(--bs-toast-border-width));border-top-right-radius:calc(var(--bs-toast-border-radius) - var(--bs-toast-border-width))}.toast-header .btn-close{margin-right:calc(-.5 * var(--bs-toast-padding-x));margin-left:var(--bs-toast-padding-x)}.toast-body{padding:var(--bs-toast-padding-x);word-wrap:break-word}.modal{--bs-modal-zindex: 1055;--bs-modal-width: 500px;--bs-modal-padding: 1rem;--bs-modal-margin: .5rem;--bs-modal-color: ;--bs-modal-bg: var(--bs-body-bg);--bs-modal-border-color: var(--bs-border-color-translucent);--bs-modal-border-width: var(--bs-border-width);--bs-modal-border-radius: var(--bs-border-radius-lg);--bs-modal-box-shadow: var(--bs-box-shadow-sm);--bs-modal-inner-border-radius: calc(var(--bs-border-radius-lg) - (var(--bs-border-width)));--bs-modal-header-padding-x: 1rem;--bs-modal-header-padding-y: 1rem;--bs-modal-header-padding: 1rem 1rem;--bs-modal-header-border-color: var(--bs-border-color);--bs-modal-header-border-width: var(--bs-border-width);--bs-modal-title-line-height: 1.5;--bs-modal-footer-gap: .5rem;--bs-modal-footer-bg: ;--bs-modal-footer-border-color: var(--bs-border-color);--bs-modal-footer-border-width: var(--bs-border-width);position:fixed;top:0;left:0;z-index:var(--bs-modal-zindex);display:none;width:100%;height:100%;overflow-x:hidden;overflow-y:auto;outline:0}.modal-dialog{position:relative;width:auto;margin:var(--bs-modal-margin);pointer-events:none}.modal.fade .modal-dialog{transition:transform .3s ease-out;transform:translateY(-50px)}@media (prefers-reduced-motion: reduce){.modal.fade .modal-dialog{transition:none}}.modal.show .modal-dialog{transform:none}.modal.modal-static .modal-dialog{transform:scale(1.02)}.modal-dialog-scrollable{height:calc(100% - var(--bs-modal-margin) * 2)}.modal-dialog-scrollable .modal-content{max-height:100%;overflow:hidden}.modal-dialog-scrollable .modal-body{overflow-y:auto}.modal-dialog-centered{display:flex;align-items:center;min-height:calc(100% - var(--bs-modal-margin) * 2)}.modal-content{position:relative;display:flex;flex-direction:column;width:100%;color:var(--bs-modal-color);pointer-events:auto;background-color:var(--bs-modal-bg);background-clip:padding-box;border:var(--bs-modal-border-width) solid var(--bs-modal-border-color);border-radius:var(--bs-modal-border-radius);outline:0}.modal-backdrop{--bs-backdrop-zindex: 1050;--bs-backdrop-bg: #000;--bs-backdrop-opacity: .5;position:fixed;top:0;left:0;z-index:var(--bs-backdrop-zindex);width:100vw;height:100vh;background-color:var(--bs-backdrop-bg)}.modal-backdrop.fade{opacity:0}.modal-backdrop.show{opacity:var(--bs-backdrop-opacity)}.modal-header{display:flex;flex-shrink:0;align-items:center;justify-content:space-between;padding:var(--bs-modal-header-padding);border-bottom:var(--bs-modal-header-border-width) solid var(--bs-modal-header-border-color);border-top-left-radius:var(--bs-modal-inner-border-radius);border-top-right-radius:var(--bs-modal-inner-border-radius)}.modal-header .btn-close{padding:calc(var(--bs-modal-header-padding-y) * .5) calc(var(--bs-modal-header-padding-x) * .5);margin:calc(-.5 * var(--bs-modal-header-padding-y)) calc(-.5 * var(--bs-modal-header-padding-x)) calc(-.5 * var(--bs-modal-header-padding-y)) auto}.modal-title{margin-bottom:0;line-height:var(--bs-modal-title-line-height)}.modal-body{position:relative;flex:1 1 auto;padding:var(--bs-modal-padding)}.modal-footer{display:flex;flex-shrink:0;flex-wrap:wrap;align-items:center;justify-content:flex-end;padding:calc(var(--bs-modal-padding) - var(--bs-modal-footer-gap) * .5);background-color:var(--bs-modal-footer-bg);border-top:var(--bs-modal-footer-border-width) solid var(--bs-modal-footer-border-color);border-bottom-right-radius:var(--bs-modal-inner-border-radius);border-bottom-left-radius:var(--bs-modal-inner-border-radius)}.modal-footer>*{margin:calc(var(--bs-modal-footer-gap) * .5)}@media (min-width: 576px){.modal{--bs-modal-margin: 1.75rem;--bs-modal-box-shadow: var(--bs-box-shadow)}.modal-dialog{max-width:var(--bs-modal-width);margin-right:auto;margin-left:auto}.modal-sm{--bs-modal-width: 300px}}@media (min-width: 992px){.modal-lg,.modal-xl{--bs-modal-width: 800px}}@media (min-width: 1200px){.modal-xl{--bs-modal-width: 1140px}}.modal-fullscreen{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen .modal-header,.modal-fullscreen .modal-footer{border-radius:0}.modal-fullscreen .modal-body{overflow-y:auto}@media (max-width: 575.98px){.modal-fullscreen-sm-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-sm-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-sm-down .modal-header,.modal-fullscreen-sm-down .modal-footer{border-radius:0}.modal-fullscreen-sm-down .modal-body{overflow-y:auto}}@media (max-width: 767.98px){.modal-fullscreen-md-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-md-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-md-down .modal-header,.modal-fullscreen-md-down .modal-footer{border-radius:0}.modal-fullscreen-md-down .modal-body{overflow-y:auto}}@media (max-width: 991.98px){.modal-fullscreen-lg-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-lg-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-lg-down .modal-header,.modal-fullscreen-lg-down .modal-footer{border-radius:0}.modal-fullscreen-lg-down .modal-body{overflow-y:auto}}@media (max-width: 1199.98px){.modal-fullscreen-xl-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-xl-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-xl-down .modal-header,.modal-fullscreen-xl-down .modal-footer{border-radius:0}.modal-fullscreen-xl-down .modal-body{overflow-y:auto}}@media (max-width: 1399.98px){.modal-fullscreen-xxl-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-xxl-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-xxl-down .modal-header,.modal-fullscreen-xxl-down .modal-footer{border-radius:0}.modal-fullscreen-xxl-down .modal-body{overflow-y:auto}}.tooltip{--bs-tooltip-zindex: 1080;--bs-tooltip-max-width: 200px;--bs-tooltip-padding-x: .5rem;--bs-tooltip-padding-y: .25rem;--bs-tooltip-margin: ;--bs-tooltip-font-size: .875rem;--bs-tooltip-color: var(--bs-body-bg);--bs-tooltip-bg: var(--bs-emphasis-color);--bs-tooltip-border-radius: var(--bs-border-radius);--bs-tooltip-opacity: .9;--bs-tooltip-arrow-width: .8rem;--bs-tooltip-arrow-height: .4rem;z-index:var(--bs-tooltip-zindex);display:block;margin:var(--bs-tooltip-margin);font-family:var(--bs-font-sans-serif);font-style:normal;font-weight:400;line-height:1.5;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;white-space:normal;word-spacing:normal;line-break:auto;font-size:var(--bs-tooltip-font-size);word-wrap:break-word;opacity:0}.tooltip.show{opacity:var(--bs-tooltip-opacity)}.tooltip .tooltip-arrow{display:block;width:var(--bs-tooltip-arrow-width);height:var(--bs-tooltip-arrow-height)}.tooltip .tooltip-arrow:before{position:absolute;content:"";border-color:transparent;border-style:solid}.bs-tooltip-top .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^=top] .tooltip-arrow{bottom:calc(-1 * var(--bs-tooltip-arrow-height))}.bs-tooltip-top .tooltip-arrow:before,.bs-tooltip-auto[data-popper-placement^=top] .tooltip-arrow:before{top:-1px;border-width:var(--bs-tooltip-arrow-height) calc(var(--bs-tooltip-arrow-width) * .5) 0;border-top-color:var(--bs-tooltip-bg)}.bs-tooltip-end .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^=right] .tooltip-arrow{left:calc(-1 * var(--bs-tooltip-arrow-height));width:var(--bs-tooltip-arrow-height);height:var(--bs-tooltip-arrow-width)}.bs-tooltip-end .tooltip-arrow:before,.bs-tooltip-auto[data-popper-placement^=right] .tooltip-arrow:before{right:-1px;border-width:calc(var(--bs-tooltip-arrow-width) * .5) var(--bs-tooltip-arrow-height) calc(var(--bs-tooltip-arrow-width) * .5) 0;border-right-color:var(--bs-tooltip-bg)}.bs-tooltip-bottom .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^=bottom] .tooltip-arrow{top:calc(-1 * var(--bs-tooltip-arrow-height))}.bs-tooltip-bottom .tooltip-arrow:before,.bs-tooltip-auto[data-popper-placement^=bottom] .tooltip-arrow:before{bottom:-1px;border-width:0 calc(var(--bs-tooltip-arrow-width) * .5) var(--bs-tooltip-arrow-height);border-bottom-color:var(--bs-tooltip-bg)}.bs-tooltip-start .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^=left] .tooltip-arrow{right:calc(-1 * var(--bs-tooltip-arrow-height));width:var(--bs-tooltip-arrow-height);height:var(--bs-tooltip-arrow-width)}.bs-tooltip-start .tooltip-arrow:before,.bs-tooltip-auto[data-popper-placement^=left] .tooltip-arrow:before{left:-1px;border-width:calc(var(--bs-tooltip-arrow-width) * .5) 0 calc(var(--bs-tooltip-arrow-width) * .5) var(--bs-tooltip-arrow-height);border-left-color:var(--bs-tooltip-bg)}.tooltip-inner{max-width:var(--bs-tooltip-max-width);padding:var(--bs-tooltip-padding-y) var(--bs-tooltip-padding-x);color:var(--bs-tooltip-color);text-align:center;background-color:var(--bs-tooltip-bg);border-radius:var(--bs-tooltip-border-radius)}.popover{--bs-popover-zindex: 1070;--bs-popover-max-width: 276px;--bs-popover-font-size: .875rem;--bs-popover-bg: var(--bs-body-bg);--bs-popover-border-width: var(--bs-border-width);--bs-popover-border-color: var(--bs-border-color-translucent);--bs-popover-border-radius: var(--bs-border-radius-lg);--bs-popover-inner-border-radius: calc(var(--bs-border-radius-lg) - var(--bs-border-width));--bs-popover-box-shadow: var(--bs-box-shadow);--bs-popover-header-padding-x: 1rem;--bs-popover-header-padding-y: .5rem;--bs-popover-header-font-size: 1rem;--bs-popover-header-color: inherit;--bs-popover-header-bg: var(--bs-secondary-bg);--bs-popover-body-padding-x: 1rem;--bs-popover-body-padding-y: 1rem;--bs-popover-body-color: var(--bs-body-color);--bs-popover-arrow-width: 1rem;--bs-popover-arrow-height: .5rem;--bs-popover-arrow-border: var(--bs-popover-border-color);z-index:var(--bs-popover-zindex);display:block;max-width:var(--bs-popover-max-width);font-family:var(--bs-font-sans-serif);font-style:normal;font-weight:400;line-height:1.5;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;white-space:normal;word-spacing:normal;line-break:auto;font-size:var(--bs-popover-font-size);word-wrap:break-word;background-color:var(--bs-popover-bg);background-clip:padding-box;border:var(--bs-popover-border-width) solid var(--bs-popover-border-color);border-radius:var(--bs-popover-border-radius)}.popover .popover-arrow{display:block;width:var(--bs-popover-arrow-width);height:var(--bs-popover-arrow-height)}.popover .popover-arrow:before,.popover .popover-arrow:after{position:absolute;display:block;content:"";border-color:transparent;border-style:solid;border-width:0}.bs-popover-top>.popover-arrow,.bs-popover-auto[data-popper-placement^=top]>.popover-arrow{bottom:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width))}.bs-popover-top>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=top]>.popover-arrow:before,.bs-popover-top>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=top]>.popover-arrow:after{border-width:var(--bs-popover-arrow-height) calc(var(--bs-popover-arrow-width) * .5) 0}.bs-popover-top>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=top]>.popover-arrow:before{bottom:0;border-top-color:var(--bs-popover-arrow-border)}.bs-popover-top>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=top]>.popover-arrow:after{bottom:var(--bs-popover-border-width);border-top-color:var(--bs-popover-bg)}.bs-popover-end>.popover-arrow,.bs-popover-auto[data-popper-placement^=right]>.popover-arrow{left:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width));width:var(--bs-popover-arrow-height);height:var(--bs-popover-arrow-width)}.bs-popover-end>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=right]>.popover-arrow:before,.bs-popover-end>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=right]>.popover-arrow:after{border-width:calc(var(--bs-popover-arrow-width) * .5) var(--bs-popover-arrow-height) calc(var(--bs-popover-arrow-width) * .5) 0}.bs-popover-end>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=right]>.popover-arrow:before{left:0;border-right-color:var(--bs-popover-arrow-border)}.bs-popover-end>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=right]>.popover-arrow:after{left:var(--bs-popover-border-width);border-right-color:var(--bs-popover-bg)}.bs-popover-bottom>.popover-arrow,.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow{top:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width))}.bs-popover-bottom>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow:before,.bs-popover-bottom>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow:after{border-width:0 calc(var(--bs-popover-arrow-width) * .5) var(--bs-popover-arrow-height)}.bs-popover-bottom>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow:before{top:0;border-bottom-color:var(--bs-popover-arrow-border)}.bs-popover-bottom>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow:after{top:var(--bs-popover-border-width);border-bottom-color:var(--bs-popover-bg)}.bs-popover-bottom .popover-header:before,.bs-popover-auto[data-popper-placement^=bottom] .popover-header:before{position:absolute;top:0;left:50%;display:block;width:var(--bs-popover-arrow-width);margin-left:calc(-.5 * var(--bs-popover-arrow-width));content:"";border-bottom:var(--bs-popover-border-width) solid var(--bs-popover-header-bg)}.bs-popover-start>.popover-arrow,.bs-popover-auto[data-popper-placement^=left]>.popover-arrow{right:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width));width:var(--bs-popover-arrow-height);height:var(--bs-popover-arrow-width)}.bs-popover-start>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=left]>.popover-arrow:before,.bs-popover-start>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=left]>.popover-arrow:after{border-width:calc(var(--bs-popover-arrow-width) * .5) 0 calc(var(--bs-popover-arrow-width) * .5) var(--bs-popover-arrow-height)}.bs-popover-start>.popover-arrow:before,.bs-popover-auto[data-popper-placement^=left]>.popover-arrow:before{right:0;border-left-color:var(--bs-popover-arrow-border)}.bs-popover-start>.popover-arrow:after,.bs-popover-auto[data-popper-placement^=left]>.popover-arrow:after{right:var(--bs-popover-border-width);border-left-color:var(--bs-popover-bg)}.popover-header{padding:var(--bs-popover-header-padding-y) var(--bs-popover-header-padding-x);margin-bottom:0;font-size:var(--bs-popover-header-font-size);color:var(--bs-popover-header-color);background-color:var(--bs-popover-header-bg);border-bottom:var(--bs-popover-border-width) solid var(--bs-popover-border-color);border-top-left-radius:var(--bs-popover-inner-border-radius);border-top-right-radius:var(--bs-popover-inner-border-radius)}.popover-header:empty{display:none}.popover-body{padding:var(--bs-popover-body-padding-y) var(--bs-popover-body-padding-x);color:var(--bs-popover-body-color)}.carousel{position:relative}.carousel.pointer-event{touch-action:pan-y}.carousel-inner{position:relative;width:100%;overflow:hidden}.carousel-inner:after{display:block;clear:both;content:""}.carousel-item{position:relative;display:none;float:left;width:100%;margin-right:-100%;backface-visibility:hidden;transition:transform .6s ease-in-out}@media (prefers-reduced-motion: reduce){.carousel-item{transition:none}}.carousel-item.active,.carousel-item-next,.carousel-item-prev{display:block}.carousel-item-next:not(.carousel-item-start),.active.carousel-item-end{transform:translate(100%)}.carousel-item-prev:not(.carousel-item-end),.active.carousel-item-start{transform:translate(-100%)}.carousel-fade .carousel-item{opacity:0;transition-property:opacity;transform:none}.carousel-fade .carousel-item.active,.carousel-fade .carousel-item-next.carousel-item-start,.carousel-fade .carousel-item-prev.carousel-item-end{z-index:1;opacity:1}.carousel-fade .active.carousel-item-start,.carousel-fade .active.carousel-item-end{z-index:0;opacity:0;transition:opacity 0s .6s}@media (prefers-reduced-motion: reduce){.carousel-fade .active.carousel-item-start,.carousel-fade .active.carousel-item-end{transition:none}}.carousel-control-prev,.carousel-control-next{position:absolute;top:0;bottom:0;z-index:1;display:flex;align-items:center;justify-content:center;width:15%;padding:0;color:#fff;text-align:center;background:none;border:0;opacity:.5;transition:opacity .15s ease}@media (prefers-reduced-motion: reduce){.carousel-control-prev,.carousel-control-next{transition:none}}.carousel-control-prev:hover,.carousel-control-prev:focus,.carousel-control-next:hover,.carousel-control-next:focus{color:#fff;text-decoration:none;outline:0;opacity:.9}.carousel-control-prev{left:0}.carousel-control-next{right:0}.carousel-control-prev-icon,.carousel-control-next-icon{display:inline-block;width:2rem;height:2rem;background-repeat:no-repeat;background-position:50%;background-size:100% 100%}.carousel-control-prev-icon{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23fff'%3e%3cpath d='M11.354 1.646a.5.5 0 0 1 0 .708L5.707 8l5.647 5.646a.5.5 0 0 1-.708.708l-6-6a.5.5 0 0 1 0-.708l6-6a.5.5 0 0 1 .708 0z'/%3e%3c/svg%3e")}.carousel-control-next-icon{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23fff'%3e%3cpath d='M4.646 1.646a.5.5 0 0 1 .708 0l6 6a.5.5 0 0 1 0 .708l-6 6a.5.5 0 0 1-.708-.708L10.293 8 4.646 2.354a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e")}.carousel-indicators{position:absolute;right:0;bottom:0;left:0;z-index:2;display:flex;justify-content:center;padding:0;margin-right:15%;margin-bottom:1rem;margin-left:15%}.carousel-indicators [data-bs-target]{box-sizing:content-box;flex:0 1 auto;width:30px;height:3px;padding:0;margin-right:3px;margin-left:3px;text-indent:-999px;cursor:pointer;background-color:#fff;background-clip:padding-box;border:0;border-top:10px solid transparent;border-bottom:10px solid transparent;opacity:.5;transition:opacity .6s ease}@media (prefers-reduced-motion: reduce){.carousel-indicators [data-bs-target]{transition:none}}.carousel-indicators .active{opacity:1}.carousel-caption{position:absolute;right:15%;bottom:1.25rem;left:15%;padding-top:1.25rem;padding-bottom:1.25rem;color:#fff;text-align:center}.carousel-dark .carousel-control-prev-icon,.carousel-dark .carousel-control-next-icon{filter:invert(1) grayscale(100)}.carousel-dark .carousel-indicators [data-bs-target]{background-color:#000}.carousel-dark .carousel-caption{color:#000}[data-bs-theme=dark] .carousel .carousel-control-prev-icon,[data-bs-theme=dark] .carousel .carousel-control-next-icon,[data-bs-theme=dark].carousel .carousel-control-prev-icon,[data-bs-theme=dark].carousel .carousel-control-next-icon{filter:invert(1) grayscale(100)}[data-bs-theme=dark] .carousel .carousel-indicators [data-bs-target],[data-bs-theme=dark].carousel .carousel-indicators [data-bs-target]{background-color:#000}[data-bs-theme=dark] .carousel .carousel-caption,[data-bs-theme=dark].carousel .carousel-caption{color:#000}.spinner-grow,.spinner-border{display:inline-block;width:var(--bs-spinner-width);height:var(--bs-spinner-height);vertical-align:var(--bs-spinner-vertical-align);border-radius:50%;animation:var(--bs-spinner-animation-speed) linear infinite var(--bs-spinner-animation-name)}@keyframes spinner-border{to{transform:rotate(360deg)}}.spinner-border{--bs-spinner-width: 2rem;--bs-spinner-height: 2rem;--bs-spinner-vertical-align: -.125em;--bs-spinner-border-width: .25em;--bs-spinner-animation-speed: .75s;--bs-spinner-animation-name: spinner-border;border:var(--bs-spinner-border-width) solid currentcolor;border-right-color:transparent}.spinner-border-sm{--bs-spinner-width: 1rem;--bs-spinner-height: 1rem;--bs-spinner-border-width: .2em}@keyframes spinner-grow{0%{transform:scale(0)}50%{opacity:1;transform:none}}.spinner-grow{--bs-spinner-width: 2rem;--bs-spinner-height: 2rem;--bs-spinner-vertical-align: -.125em;--bs-spinner-animation-speed: .75s;--bs-spinner-animation-name: spinner-grow;background-color:currentcolor;opacity:0}.spinner-grow-sm{--bs-spinner-width: 1rem;--bs-spinner-height: 1rem}@media (prefers-reduced-motion: reduce){.spinner-border,.spinner-grow{--bs-spinner-animation-speed: 1.5s}}.offcanvas,.offcanvas-xxl,.offcanvas-xl,.offcanvas-lg,.offcanvas-md,.offcanvas-sm{--bs-offcanvas-zindex: 1045;--bs-offcanvas-width: 400px;--bs-offcanvas-height: 30vh;--bs-offcanvas-padding-x: 1rem;--bs-offcanvas-padding-y: 1rem;--bs-offcanvas-color: var(--bs-body-color);--bs-offcanvas-bg: var(--bs-body-bg);--bs-offcanvas-border-width: var(--bs-border-width);--bs-offcanvas-border-color: var(--bs-border-color-translucent);--bs-offcanvas-box-shadow: var(--bs-box-shadow-sm);--bs-offcanvas-transition: transform .3s ease-in-out;--bs-offcanvas-title-line-height: 1.5}@media (max-width: 575.98px){.offcanvas-sm{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:var(--bs-offcanvas-transition)}}@media (max-width: 575.98px) and (prefers-reduced-motion: reduce){.offcanvas-sm{transition:none}}@media (max-width: 575.98px){.offcanvas-sm.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(-100%)}.offcanvas-sm.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(100%)}.offcanvas-sm.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-sm.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-sm.showing,.offcanvas-sm.show:not(.hiding){transform:none}.offcanvas-sm.showing,.offcanvas-sm.hiding,.offcanvas-sm.show{visibility:visible}}@media (min-width: 576px){.offcanvas-sm{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent!important}.offcanvas-sm .offcanvas-header{display:none}.offcanvas-sm .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible;background-color:transparent!important}}@media (max-width: 767.98px){.offcanvas-md{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:var(--bs-offcanvas-transition)}}@media (max-width: 767.98px) and (prefers-reduced-motion: reduce){.offcanvas-md{transition:none}}@media (max-width: 767.98px){.offcanvas-md.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(-100%)}.offcanvas-md.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(100%)}.offcanvas-md.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-md.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-md.showing,.offcanvas-md.show:not(.hiding){transform:none}.offcanvas-md.showing,.offcanvas-md.hiding,.offcanvas-md.show{visibility:visible}}@media (min-width: 768px){.offcanvas-md{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent!important}.offcanvas-md .offcanvas-header{display:none}.offcanvas-md .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible;background-color:transparent!important}}@media (max-width: 991.98px){.offcanvas-lg{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:var(--bs-offcanvas-transition)}}@media (max-width: 991.98px) and (prefers-reduced-motion: reduce){.offcanvas-lg{transition:none}}@media (max-width: 991.98px){.offcanvas-lg.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(-100%)}.offcanvas-lg.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(100%)}.offcanvas-lg.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-lg.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-lg.showing,.offcanvas-lg.show:not(.hiding){transform:none}.offcanvas-lg.showing,.offcanvas-lg.hiding,.offcanvas-lg.show{visibility:visible}}@media (min-width: 992px){.offcanvas-lg{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent!important}.offcanvas-lg .offcanvas-header{display:none}.offcanvas-lg .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible;background-color:transparent!important}}@media (max-width: 1199.98px){.offcanvas-xl{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:var(--bs-offcanvas-transition)}}@media (max-width: 1199.98px) and (prefers-reduced-motion: reduce){.offcanvas-xl{transition:none}}@media (max-width: 1199.98px){.offcanvas-xl.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(-100%)}.offcanvas-xl.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(100%)}.offcanvas-xl.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-xl.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-xl.showing,.offcanvas-xl.show:not(.hiding){transform:none}.offcanvas-xl.showing,.offcanvas-xl.hiding,.offcanvas-xl.show{visibility:visible}}@media (min-width: 1200px){.offcanvas-xl{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent!important}.offcanvas-xl .offcanvas-header{display:none}.offcanvas-xl .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible;background-color:transparent!important}}@media (max-width: 1399.98px){.offcanvas-xxl{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:var(--bs-offcanvas-transition)}}@media (max-width: 1399.98px) and (prefers-reduced-motion: reduce){.offcanvas-xxl{transition:none}}@media (max-width: 1399.98px){.offcanvas-xxl.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(-100%)}.offcanvas-xxl.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(100%)}.offcanvas-xxl.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-xxl.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-xxl.showing,.offcanvas-xxl.show:not(.hiding){transform:none}.offcanvas-xxl.showing,.offcanvas-xxl.hiding,.offcanvas-xxl.show{visibility:visible}}@media (min-width: 1400px){.offcanvas-xxl{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent!important}.offcanvas-xxl .offcanvas-header{display:none}.offcanvas-xxl .offcanvas-body{display:flex;flex-grow:0;padding:0;overflow-y:visible;background-color:transparent!important}}.offcanvas{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:var(--bs-offcanvas-transition)}@media (prefers-reduced-motion: reduce){.offcanvas{transition:none}}.offcanvas.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(-100%)}.offcanvas.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translate(100%)}.offcanvas.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas.showing,.offcanvas.show:not(.hiding){transform:none}.offcanvas.showing,.offcanvas.hiding,.offcanvas.show{visibility:visible}.offcanvas-backdrop{position:fixed;top:0;left:0;z-index:1040;width:100vw;height:100vh;background-color:#000}.offcanvas-backdrop.fade{opacity:0}.offcanvas-backdrop.show{opacity:.5}.offcanvas-header{display:flex;align-items:center;justify-content:space-between;padding:var(--bs-offcanvas-padding-y) var(--bs-offcanvas-padding-x)}.offcanvas-header .btn-close{padding:calc(var(--bs-offcanvas-padding-y) * .5) calc(var(--bs-offcanvas-padding-x) * .5);margin-top:calc(-.5 * var(--bs-offcanvas-padding-y));margin-right:calc(-.5 * var(--bs-offcanvas-padding-x));margin-bottom:calc(-.5 * var(--bs-offcanvas-padding-y))}.offcanvas-title{margin-bottom:0;line-height:var(--bs-offcanvas-title-line-height)}.offcanvas-body{flex-grow:1;padding:var(--bs-offcanvas-padding-y) var(--bs-offcanvas-padding-x);overflow-y:auto}.placeholder{display:inline-block;min-height:1em;vertical-align:middle;cursor:wait;background-color:currentcolor;opacity:.5}.placeholder.btn:before{display:inline-block;content:""}.placeholder-xs{min-height:.6em}.placeholder-sm{min-height:.8em}.placeholder-lg{min-height:1.2em}.placeholder-glow .placeholder{animation:placeholder-glow 2s ease-in-out infinite}@keyframes placeholder-glow{50%{opacity:.2}}.placeholder-wave{mask-image:linear-gradient(130deg,#000 55%,#000c,#000 95%);mask-size:200% 100%;animation:placeholder-wave 2s linear infinite}@keyframes placeholder-wave{to{mask-position:-200% 0%}}.clearfix:after{display:block;clear:both;content:""}.text-bg-primary{color:#fff!important;background-color:RGBA(var(--bs-primary-rgb),var(--bs-bg-opacity, 1))!important}.text-bg-secondary{color:#fff!important;background-color:RGBA(var(--bs-secondary-rgb),var(--bs-bg-opacity, 1))!important}.text-bg-success{color:#fff!important;background-color:RGBA(var(--bs-success-rgb),var(--bs-bg-opacity, 1))!important}.text-bg-info{color:#000!important;background-color:RGBA(var(--bs-info-rgb),var(--bs-bg-opacity, 1))!important}.text-bg-warning{color:#000!important;background-color:RGBA(var(--bs-warning-rgb),var(--bs-bg-opacity, 1))!important}.text-bg-danger{color:#fff!important;background-color:RGBA(var(--bs-danger-rgb),var(--bs-bg-opacity, 1))!important}.text-bg-light{color:#000!important;background-color:RGBA(var(--bs-light-rgb),var(--bs-bg-opacity, 1))!important}.text-bg-dark{color:#fff!important;background-color:RGBA(var(--bs-dark-rgb),var(--bs-bg-opacity, 1))!important}.link-primary{color:RGBA(var(--bs-primary-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-primary-rgb),var(--bs-link-underline-opacity, 1))!important}.link-primary:hover,.link-primary:focus{color:RGBA(10,88,202,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(10,88,202,var(--bs-link-underline-opacity, 1))!important}.link-secondary{color:RGBA(var(--bs-secondary-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-secondary-rgb),var(--bs-link-underline-opacity, 1))!important}.link-secondary:hover,.link-secondary:focus{color:RGBA(86,94,100,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(86,94,100,var(--bs-link-underline-opacity, 1))!important}.link-success{color:RGBA(var(--bs-success-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-success-rgb),var(--bs-link-underline-opacity, 1))!important}.link-success:hover,.link-success:focus{color:RGBA(20,108,67,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(20,108,67,var(--bs-link-underline-opacity, 1))!important}.link-info{color:RGBA(var(--bs-info-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-info-rgb),var(--bs-link-underline-opacity, 1))!important}.link-info:hover,.link-info:focus{color:RGBA(61,213,243,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(61,213,243,var(--bs-link-underline-opacity, 1))!important}.link-warning{color:RGBA(var(--bs-warning-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-warning-rgb),var(--bs-link-underline-opacity, 1))!important}.link-warning:hover,.link-warning:focus{color:RGBA(255,205,57,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(255,205,57,var(--bs-link-underline-opacity, 1))!important}.link-danger{color:RGBA(var(--bs-danger-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-danger-rgb),var(--bs-link-underline-opacity, 1))!important}.link-danger:hover,.link-danger:focus{color:RGBA(176,42,55,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(176,42,55,var(--bs-link-underline-opacity, 1))!important}.link-light{color:RGBA(var(--bs-light-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-light-rgb),var(--bs-link-underline-opacity, 1))!important}.link-light:hover,.link-light:focus{color:RGBA(249,250,251,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(249,250,251,var(--bs-link-underline-opacity, 1))!important}.link-dark{color:RGBA(var(--bs-dark-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-dark-rgb),var(--bs-link-underline-opacity, 1))!important}.link-dark:hover,.link-dark:focus{color:RGBA(26,30,33,var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(26,30,33,var(--bs-link-underline-opacity, 1))!important}.link-body-emphasis{color:RGBA(var(--bs-emphasis-color-rgb),var(--bs-link-opacity, 1))!important;text-decoration-color:RGBA(var(--bs-emphasis-color-rgb),var(--bs-link-underline-opacity, 1))!important}.link-body-emphasis:hover,.link-body-emphasis:focus{color:RGBA(var(--bs-emphasis-color-rgb),var(--bs-link-opacity, .75))!important;text-decoration-color:RGBA(var(--bs-emphasis-color-rgb),var(--bs-link-underline-opacity, .75))!important}.focus-ring:focus{outline:0;box-shadow:var(--bs-focus-ring-x, 0) var(--bs-focus-ring-y, 0) var(--bs-focus-ring-blur, 0) var(--bs-focus-ring-width) var(--bs-focus-ring-color)}.icon-link{display:inline-flex;gap:.375rem;align-items:center;text-decoration-color:rgba(var(--bs-link-color-rgb),var(--bs-link-opacity, .5));text-underline-offset:.25em;backface-visibility:hidden}.icon-link>.bi{flex-shrink:0;width:1em;height:1em;fill:currentcolor;transition:.2s ease-in-out transform}@media (prefers-reduced-motion: reduce){.icon-link>.bi{transition:none}}.icon-link-hover:hover>.bi,.icon-link-hover:focus-visible>.bi{transform:var(--bs-icon-link-transform, translate3d(.25em, 0, 0))}.ratio{position:relative;width:100%}.ratio:before{display:block;padding-top:var(--bs-aspect-ratio);content:""}.ratio>*{position:absolute;top:0;left:0;width:100%;height:100%}.ratio-1x1{--bs-aspect-ratio: 100%}.ratio-4x3{--bs-aspect-ratio: 75%}.ratio-16x9{--bs-aspect-ratio: 56.25%}.ratio-21x9{--bs-aspect-ratio: 42.8571428571%}.fixed-top{position:fixed;top:0;right:0;left:0;z-index:1030}.fixed-bottom{position:fixed;right:0;bottom:0;left:0;z-index:1030}.sticky-top{position:sticky;top:0;z-index:1020}.sticky-bottom{position:sticky;bottom:0;z-index:1020}@media (min-width: 576px){.sticky-sm-top{position:sticky;top:0;z-index:1020}.sticky-sm-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 768px){.sticky-md-top{position:sticky;top:0;z-index:1020}.sticky-md-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 992px){.sticky-lg-top{position:sticky;top:0;z-index:1020}.sticky-lg-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 1200px){.sticky-xl-top{position:sticky;top:0;z-index:1020}.sticky-xl-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 1400px){.sticky-xxl-top{position:sticky;top:0;z-index:1020}.sticky-xxl-bottom{position:sticky;bottom:0;z-index:1020}}.hstack{display:flex;flex-direction:row;align-items:center;align-self:stretch}.vstack{display:flex;flex:1 1 auto;flex-direction:column;align-self:stretch}.visually-hidden,.visually-hidden-focusable:not(:focus):not(:focus-within){width:1px!important;height:1px!important;padding:0!important;margin:-1px!important;overflow:hidden!important;clip:rect(0,0,0,0)!important;white-space:nowrap!important;border:0!important}.visually-hidden:not(caption),.visually-hidden-focusable:not(:focus):not(:focus-within):not(caption){position:absolute!important}.stretched-link:after{position:absolute;inset:0;z-index:1;content:""}.text-truncate{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.vr{display:inline-block;align-self:stretch;width:var(--bs-border-width);min-height:1em;background-color:currentcolor;opacity:.25}.align-baseline{vertical-align:baseline!important}.align-top{vertical-align:top!important}.align-middle{vertical-align:middle!important}.align-bottom{vertical-align:bottom!important}.align-text-bottom{vertical-align:text-bottom!important}.align-text-top{vertical-align:text-top!important}.float-start{float:left!important}.float-end{float:right!important}.float-none{float:none!important}.object-fit-contain{object-fit:contain!important}.object-fit-cover{object-fit:cover!important}.object-fit-fill{object-fit:fill!important}.object-fit-scale{object-fit:scale-down!important}.object-fit-none{object-fit:none!important}.opacity-0{opacity:0!important}.opacity-25{opacity:.25!important}.opacity-50{opacity:.5!important}.opacity-75{opacity:.75!important}.opacity-100{opacity:1!important}.overflow-auto{overflow:auto!important}.overflow-hidden{overflow:hidden!important}.overflow-visible{overflow:visible!important}.overflow-scroll{overflow:scroll!important}.overflow-x-auto{overflow-x:auto!important}.overflow-x-hidden{overflow-x:hidden!important}.overflow-x-visible{overflow-x:visible!important}.overflow-x-scroll{overflow-x:scroll!important}.overflow-y-auto{overflow-y:auto!important}.overflow-y-hidden{overflow-y:hidden!important}.overflow-y-visible{overflow-y:visible!important}.overflow-y-scroll{overflow-y:scroll!important}.d-inline{display:inline!important}.d-inline-block{display:inline-block!important}.d-block{display:block!important}.d-grid{display:grid!important}.d-inline-grid{display:inline-grid!important}.d-table{display:table!important}.d-table-row{display:table-row!important}.d-table-cell{display:table-cell!important}.d-flex{display:flex!important}.d-inline-flex{display:inline-flex!important}.d-none{display:none!important}.shadow{box-shadow:var(--bs-box-shadow)!important}.shadow-sm{box-shadow:var(--bs-box-shadow-sm)!important}.shadow-lg{box-shadow:var(--bs-box-shadow-lg)!important}.shadow-none{box-shadow:none!important}.focus-ring-primary{--bs-focus-ring-color: rgba(var(--bs-primary-rgb), var(--bs-focus-ring-opacity))}.focus-ring-secondary{--bs-focus-ring-color: rgba(var(--bs-secondary-rgb), var(--bs-focus-ring-opacity))}.focus-ring-success{--bs-focus-ring-color: rgba(var(--bs-success-rgb), var(--bs-focus-ring-opacity))}.focus-ring-info{--bs-focus-ring-color: rgba(var(--bs-info-rgb), var(--bs-focus-ring-opacity))}.focus-ring-warning{--bs-focus-ring-color: rgba(var(--bs-warning-rgb), var(--bs-focus-ring-opacity))}.focus-ring-danger{--bs-focus-ring-color: rgba(var(--bs-danger-rgb), var(--bs-focus-ring-opacity))}.focus-ring-light{--bs-focus-ring-color: rgba(var(--bs-light-rgb), var(--bs-focus-ring-opacity))}.focus-ring-dark{--bs-focus-ring-color: rgba(var(--bs-dark-rgb), var(--bs-focus-ring-opacity))}.position-static{position:static!important}.position-relative{position:relative!important}.position-absolute{position:absolute!important}.position-fixed{position:fixed!important}.position-sticky{position:sticky!important}.top-0{top:0!important}.top-50{top:50%!important}.top-100{top:100%!important}.bottom-0{bottom:0!important}.bottom-50{bottom:50%!important}.bottom-100{bottom:100%!important}.start-0{left:0!important}.start-50{left:50%!important}.start-100{left:100%!important}.end-0{right:0!important}.end-50{right:50%!important}.end-100{right:100%!important}.translate-middle{transform:translate(-50%,-50%)!important}.translate-middle-x{transform:translate(-50%)!important}.translate-middle-y{transform:translateY(-50%)!important}.border{border:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color)!important}.border-0{border:0!important}.border-top{border-top:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color)!important}.border-top-0{border-top:0!important}.border-end{border-right:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color)!important}.border-end-0{border-right:0!important}.border-bottom{border-bottom:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color)!important}.border-bottom-0{border-bottom:0!important}.border-start{border-left:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color)!important}.border-start-0{border-left:0!important}.border-primary{--bs-border-opacity: 1;border-color:rgba(var(--bs-primary-rgb),var(--bs-border-opacity))!important}.border-secondary{--bs-border-opacity: 1;border-color:rgba(var(--bs-secondary-rgb),var(--bs-border-opacity))!important}.border-success{--bs-border-opacity: 1;border-color:rgba(var(--bs-success-rgb),var(--bs-border-opacity))!important}.border-info{--bs-border-opacity: 1;border-color:rgba(var(--bs-info-rgb),var(--bs-border-opacity))!important}.border-warning{--bs-border-opacity: 1;border-color:rgba(var(--bs-warning-rgb),var(--bs-border-opacity))!important}.border-danger{--bs-border-opacity: 1;border-color:rgba(var(--bs-danger-rgb),var(--bs-border-opacity))!important}.border-light{--bs-border-opacity: 1;border-color:rgba(var(--bs-light-rgb),var(--bs-border-opacity))!important}.border-dark{--bs-border-opacity: 1;border-color:rgba(var(--bs-dark-rgb),var(--bs-border-opacity))!important}.border-black{--bs-border-opacity: 1;border-color:rgba(var(--bs-black-rgb),var(--bs-border-opacity))!important}.border-white{--bs-border-opacity: 1;border-color:rgba(var(--bs-white-rgb),var(--bs-border-opacity))!important}.border-primary-subtle{border-color:var(--bs-primary-border-subtle)!important}.border-secondary-subtle{border-color:var(--bs-secondary-border-subtle)!important}.border-success-subtle{border-color:var(--bs-success-border-subtle)!important}.border-info-subtle{border-color:var(--bs-info-border-subtle)!important}.border-warning-subtle{border-color:var(--bs-warning-border-subtle)!important}.border-danger-subtle{border-color:var(--bs-danger-border-subtle)!important}.border-light-subtle{border-color:var(--bs-light-border-subtle)!important}.border-dark-subtle{border-color:var(--bs-dark-border-subtle)!important}.border-1{border-width:1px!important}.border-2{border-width:2px!important}.border-3{border-width:3px!important}.border-4{border-width:4px!important}.border-5{border-width:5px!important}.border-opacity-10{--bs-border-opacity: .1}.border-opacity-25{--bs-border-opacity: .25}.border-opacity-50{--bs-border-opacity: .5}.border-opacity-75{--bs-border-opacity: .75}.border-opacity-100{--bs-border-opacity: 1}.w-25{width:25%!important}.w-50{width:50%!important}.w-75{width:75%!important}.w-100{width:100%!important}.w-auto{width:auto!important}.mw-100{max-width:100%!important}.vw-100{width:100vw!important}.min-vw-100{min-width:100vw!important}.h-25{height:25%!important}.h-50{height:50%!important}.h-75{height:75%!important}.h-100{height:100%!important}.h-auto{height:auto!important}.mh-100{max-height:100%!important}.vh-100{height:100vh!important}.min-vh-100{min-height:100vh!important}.flex-fill{flex:1 1 auto!important}.flex-row{flex-direction:row!important}.flex-column{flex-direction:column!important}.flex-row-reverse{flex-direction:row-reverse!important}.flex-column-reverse{flex-direction:column-reverse!important}.flex-grow-0{flex-grow:0!important}.flex-grow-1{flex-grow:1!important}.flex-shrink-0{flex-shrink:0!important}.flex-shrink-1{flex-shrink:1!important}.flex-wrap{flex-wrap:wrap!important}.flex-nowrap{flex-wrap:nowrap!important}.flex-wrap-reverse{flex-wrap:wrap-reverse!important}.justify-content-start{justify-content:flex-start!important}.justify-content-end{justify-content:flex-end!important}.justify-content-center{justify-content:center!important}.justify-content-between{justify-content:space-between!important}.justify-content-around{justify-content:space-around!important}.justify-content-evenly{justify-content:space-evenly!important}.align-items-start{align-items:flex-start!important}.align-items-end{align-items:flex-end!important}.align-items-center{align-items:center!important}.align-items-baseline{align-items:baseline!important}.align-items-stretch{align-items:stretch!important}.align-content-start{align-content:flex-start!important}.align-content-end{align-content:flex-end!important}.align-content-center{align-content:center!important}.align-content-between{align-content:space-between!important}.align-content-around{align-content:space-around!important}.align-content-stretch{align-content:stretch!important}.align-self-auto{align-self:auto!important}.align-self-start{align-self:flex-start!important}.align-self-end{align-self:flex-end!important}.align-self-center{align-self:center!important}.align-self-baseline{align-self:baseline!important}.align-self-stretch{align-self:stretch!important}.order-first{order:-1!important}.order-0{order:0!important}.order-1{order:1!important}.order-2{order:2!important}.order-3{order:3!important}.order-4{order:4!important}.order-5{order:5!important}.order-last{order:6!important}.m-0{margin:0!important}.m-1{margin:.25rem!important}.m-2{margin:.5rem!important}.m-3{margin:1rem!important}.m-4{margin:1.5rem!important}.m-5{margin:3rem!important}.m-auto{margin:auto!important}.mx-0{margin-right:0!important;margin-left:0!important}.mx-1{margin-right:.25rem!important;margin-left:.25rem!important}.mx-2{margin-right:.5rem!important;margin-left:.5rem!important}.mx-3{margin-right:1rem!important;margin-left:1rem!important}.mx-4{margin-right:1.5rem!important;margin-left:1.5rem!important}.mx-5{margin-right:3rem!important;margin-left:3rem!important}.mx-auto{margin-right:auto!important;margin-left:auto!important}.my-0{margin-top:0!important;margin-bottom:0!important}.my-1{margin-top:.25rem!important;margin-bottom:.25rem!important}.my-2{margin-top:.5rem!important;margin-bottom:.5rem!important}.my-3{margin-top:1rem!important;margin-bottom:1rem!important}.my-4{margin-top:1.5rem!important;margin-bottom:1.5rem!important}.my-5{margin-top:3rem!important;margin-bottom:3rem!important}.my-auto{margin-top:auto!important;margin-bottom:auto!important}.mt-0{margin-top:0!important}.mt-1{margin-top:.25rem!important}.mt-2{margin-top:.5rem!important}.mt-3{margin-top:1rem!important}.mt-4{margin-top:1.5rem!important}.mt-5{margin-top:3rem!important}.mt-auto{margin-top:auto!important}.me-0{margin-right:0!important}.me-1{margin-right:.25rem!important}.me-2{margin-right:.5rem!important}.me-3{margin-right:1rem!important}.me-4{margin-right:1.5rem!important}.me-5{margin-right:3rem!important}.me-auto{margin-right:auto!important}.mb-0{margin-bottom:0!important}.mb-1{margin-bottom:.25rem!important}.mb-2{margin-bottom:.5rem!important}.mb-3{margin-bottom:1rem!important}.mb-4{margin-bottom:1.5rem!important}.mb-5{margin-bottom:3rem!important}.mb-auto{margin-bottom:auto!important}.ms-0{margin-left:0!important}.ms-1{margin-left:.25rem!important}.ms-2{margin-left:.5rem!important}.ms-3{margin-left:1rem!important}.ms-4{margin-left:1.5rem!important}.ms-5{margin-left:3rem!important}.ms-auto{margin-left:auto!important}.p-0{padding:0!important}.p-1{padding:.25rem!important}.p-2{padding:.5rem!important}.p-3{padding:1rem!important}.p-4{padding:1.5rem!important}.p-5{padding:3rem!important}.px-0{padding-right:0!important;padding-left:0!important}.px-1{padding-right:.25rem!important;padding-left:.25rem!important}.px-2{padding-right:.5rem!important;padding-left:.5rem!important}.px-3{padding-right:1rem!important;padding-left:1rem!important}.px-4{padding-right:1.5rem!important;padding-left:1.5rem!important}.px-5{padding-right:3rem!important;padding-left:3rem!important}.py-0{padding-top:0!important;padding-bottom:0!important}.py-1{padding-top:.25rem!important;padding-bottom:.25rem!important}.py-2{padding-top:.5rem!important;padding-bottom:.5rem!important}.py-3{padding-top:1rem!important;padding-bottom:1rem!important}.py-4{padding-top:1.5rem!important;padding-bottom:1.5rem!important}.py-5{padding-top:3rem!important;padding-bottom:3rem!important}.pt-0{padding-top:0!important}.pt-1{padding-top:.25rem!important}.pt-2{padding-top:.5rem!important}.pt-3{padding-top:1rem!important}.pt-4{padding-top:1.5rem!important}.pt-5{padding-top:3rem!important}.pe-0{padding-right:0!important}.pe-1{padding-right:.25rem!important}.pe-2{padding-right:.5rem!important}.pe-3{padding-right:1rem!important}.pe-4{padding-right:1.5rem!important}.pe-5{padding-right:3rem!important}.pb-0{padding-bottom:0!important}.pb-1{padding-bottom:.25rem!important}.pb-2{padding-bottom:.5rem!important}.pb-3{padding-bottom:1rem!important}.pb-4{padding-bottom:1.5rem!important}.pb-5{padding-bottom:3rem!important}.ps-0{padding-left:0!important}.ps-1{padding-left:.25rem!important}.ps-2{padding-left:.5rem!important}.ps-3{padding-left:1rem!important}.ps-4{padding-left:1.5rem!important}.ps-5{padding-left:3rem!important}.gap-0{gap:0!important}.gap-1{gap:.25rem!important}.gap-2{gap:.5rem!important}.gap-3{gap:1rem!important}.gap-4{gap:1.5rem!important}.gap-5{gap:3rem!important}.row-gap-0{row-gap:0!important}.row-gap-1{row-gap:.25rem!important}.row-gap-2{row-gap:.5rem!important}.row-gap-3{row-gap:1rem!important}.row-gap-4{row-gap:1.5rem!important}.row-gap-5{row-gap:3rem!important}.column-gap-0{column-gap:0!important}.column-gap-1{column-gap:.25rem!important}.column-gap-2{column-gap:.5rem!important}.column-gap-3{column-gap:1rem!important}.column-gap-4{column-gap:1.5rem!important}.column-gap-5{column-gap:3rem!important}.font-monospace{font-family:var(--bs-font-monospace)!important}.fs-1{font-size:calc(1.375rem + 1.5vw)!important}.fs-2{font-size:calc(1.325rem + .9vw)!important}.fs-3{font-size:calc(1.3rem + .6vw)!important}.fs-4{font-size:calc(1.275rem + .3vw)!important}.fs-5{font-size:1.25rem!important}.fs-6{font-size:1rem!important}.fst-italic{font-style:italic!important}.fst-normal{font-style:normal!important}.fw-lighter{font-weight:lighter!important}.fw-light{font-weight:300!important}.fw-normal{font-weight:400!important}.fw-medium{font-weight:500!important}.fw-semibold{font-weight:600!important}.fw-bold{font-weight:700!important}.fw-bolder{font-weight:bolder!important}.lh-1{line-height:1!important}.lh-sm{line-height:1.25!important}.lh-base{line-height:1.5!important}.lh-lg{line-height:2!important}.text-start{text-align:left!important}.text-end{text-align:right!important}.text-center{text-align:center!important}.text-decoration-none{text-decoration:none!important}.text-decoration-underline{text-decoration:underline!important}.text-decoration-line-through{text-decoration:line-through!important}.text-lowercase{text-transform:lowercase!important}.text-uppercase{text-transform:uppercase!important}.text-capitalize{text-transform:capitalize!important}.text-wrap{white-space:normal!important}.text-nowrap{white-space:nowrap!important}.text-break{word-wrap:break-word!important;word-break:break-word!important}.text-primary{--bs-text-opacity: 1;color:rgba(var(--bs-primary-rgb),var(--bs-text-opacity))!important}.text-secondary{--bs-text-opacity: 1;color:rgba(var(--bs-secondary-rgb),var(--bs-text-opacity))!important}.text-success{--bs-text-opacity: 1;color:rgba(var(--bs-success-rgb),var(--bs-text-opacity))!important}.text-info{--bs-text-opacity: 1;color:rgba(var(--bs-info-rgb),var(--bs-text-opacity))!important}.text-warning{--bs-text-opacity: 1;color:rgba(var(--bs-warning-rgb),var(--bs-text-opacity))!important}.text-danger{--bs-text-opacity: 1;color:rgba(var(--bs-danger-rgb),var(--bs-text-opacity))!important}.text-light{--bs-text-opacity: 1;color:rgba(var(--bs-light-rgb),var(--bs-text-opacity))!important}.text-dark{--bs-text-opacity: 1;color:rgba(var(--bs-dark-rgb),var(--bs-text-opacity))!important}.text-black{--bs-text-opacity: 1;color:rgba(var(--bs-black-rgb),var(--bs-text-opacity))!important}.text-white{--bs-text-opacity: 1;color:rgba(var(--bs-white-rgb),var(--bs-text-opacity))!important}.text-body{--bs-text-opacity: 1;color:rgba(var(--bs-body-color-rgb),var(--bs-text-opacity))!important}.text-muted{--bs-text-opacity: 1;color:var(--bs-secondary-color)!important}.text-black-50{--bs-text-opacity: 1;color:#00000080!important}.text-white-50{--bs-text-opacity: 1;color:#ffffff80!important}.text-body-secondary{--bs-text-opacity: 1;color:var(--bs-secondary-color)!important}.text-body-tertiary{--bs-text-opacity: 1;color:var(--bs-tertiary-color)!important}.text-body-emphasis{--bs-text-opacity: 1;color:var(--bs-emphasis-color)!important}.text-reset{--bs-text-opacity: 1;color:inherit!important}.text-opacity-25{--bs-text-opacity: .25}.text-opacity-50{--bs-text-opacity: .5}.text-opacity-75{--bs-text-opacity: .75}.text-opacity-100{--bs-text-opacity: 1}.text-primary-emphasis{color:var(--bs-primary-text-emphasis)!important}.text-secondary-emphasis{color:var(--bs-secondary-text-emphasis)!important}.text-success-emphasis{color:var(--bs-success-text-emphasis)!important}.text-info-emphasis{color:var(--bs-info-text-emphasis)!important}.text-warning-emphasis{color:var(--bs-warning-text-emphasis)!important}.text-danger-emphasis{color:var(--bs-danger-text-emphasis)!important}.text-light-emphasis{color:var(--bs-light-text-emphasis)!important}.text-dark-emphasis{color:var(--bs-dark-text-emphasis)!important}.link-opacity-10,.link-opacity-10-hover:hover{--bs-link-opacity: .1}.link-opacity-25,.link-opacity-25-hover:hover{--bs-link-opacity: .25}.link-opacity-50,.link-opacity-50-hover:hover{--bs-link-opacity: .5}.link-opacity-75,.link-opacity-75-hover:hover{--bs-link-opacity: .75}.link-opacity-100,.link-opacity-100-hover:hover{--bs-link-opacity: 1}.link-offset-1,.link-offset-1-hover:hover{text-underline-offset:.125em!important}.link-offset-2,.link-offset-2-hover:hover{text-underline-offset:.25em!important}.link-offset-3,.link-offset-3-hover:hover{text-underline-offset:.375em!important}.link-underline-primary{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-primary-rgb),var(--bs-link-underline-opacity))!important}.link-underline-secondary{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-secondary-rgb),var(--bs-link-underline-opacity))!important}.link-underline-success{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-success-rgb),var(--bs-link-underline-opacity))!important}.link-underline-info{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-info-rgb),var(--bs-link-underline-opacity))!important}.link-underline-warning{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-warning-rgb),var(--bs-link-underline-opacity))!important}.link-underline-danger{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-danger-rgb),var(--bs-link-underline-opacity))!important}.link-underline-light{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-light-rgb),var(--bs-link-underline-opacity))!important}.link-underline-dark{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-dark-rgb),var(--bs-link-underline-opacity))!important}.link-underline{--bs-link-underline-opacity: 1;text-decoration-color:rgba(var(--bs-link-color-rgb),var(--bs-link-underline-opacity, 1))!important}.link-underline-opacity-0,.link-underline-opacity-0-hover:hover{--bs-link-underline-opacity: 0}.link-underline-opacity-10,.link-underline-opacity-10-hover:hover{--bs-link-underline-opacity: .1}.link-underline-opacity-25,.link-underline-opacity-25-hover:hover{--bs-link-underline-opacity: .25}.link-underline-opacity-50,.link-underline-opacity-50-hover:hover{--bs-link-underline-opacity: .5}.link-underline-opacity-75,.link-underline-opacity-75-hover:hover{--bs-link-underline-opacity: .75}.link-underline-opacity-100,.link-underline-opacity-100-hover:hover{--bs-link-underline-opacity: 1}.bg-primary{--bs-bg-opacity: 1;background-color:rgba(var(--bs-primary-rgb),var(--bs-bg-opacity))!important}.bg-secondary{--bs-bg-opacity: 1;background-color:rgba(var(--bs-secondary-rgb),var(--bs-bg-opacity))!important}.bg-success{--bs-bg-opacity: 1;background-color:rgba(var(--bs-success-rgb),var(--bs-bg-opacity))!important}.bg-info{--bs-bg-opacity: 1;background-color:rgba(var(--bs-info-rgb),var(--bs-bg-opacity))!important}.bg-warning{--bs-bg-opacity: 1;background-color:rgba(var(--bs-warning-rgb),var(--bs-bg-opacity))!important}.bg-danger{--bs-bg-opacity: 1;background-color:rgba(var(--bs-danger-rgb),var(--bs-bg-opacity))!important}.bg-light{--bs-bg-opacity: 1;background-color:rgba(var(--bs-light-rgb),var(--bs-bg-opacity))!important}.bg-dark{--bs-bg-opacity: 1;background-color:rgba(var(--bs-dark-rgb),var(--bs-bg-opacity))!important}.bg-black{--bs-bg-opacity: 1;background-color:rgba(var(--bs-black-rgb),var(--bs-bg-opacity))!important}.bg-white{--bs-bg-opacity: 1;background-color:rgba(var(--bs-white-rgb),var(--bs-bg-opacity))!important}.bg-body{--bs-bg-opacity: 1;background-color:rgba(var(--bs-body-bg-rgb),var(--bs-bg-opacity))!important}.bg-transparent{--bs-bg-opacity: 1;background-color:transparent!important}.bg-body-secondary{--bs-bg-opacity: 1;background-color:rgba(var(--bs-secondary-bg-rgb),var(--bs-bg-opacity))!important}.bg-body-tertiary{--bs-bg-opacity: 1;background-color:rgba(var(--bs-tertiary-bg-rgb),var(--bs-bg-opacity))!important}.bg-opacity-10{--bs-bg-opacity: .1}.bg-opacity-25{--bs-bg-opacity: .25}.bg-opacity-50{--bs-bg-opacity: .5}.bg-opacity-75{--bs-bg-opacity: .75}.bg-opacity-100{--bs-bg-opacity: 1}.bg-primary-subtle{background-color:var(--bs-primary-bg-subtle)!important}.bg-secondary-subtle{background-color:var(--bs-secondary-bg-subtle)!important}.bg-success-subtle{background-color:var(--bs-success-bg-subtle)!important}.bg-info-subtle{background-color:var(--bs-info-bg-subtle)!important}.bg-warning-subtle{background-color:var(--bs-warning-bg-subtle)!important}.bg-danger-subtle{background-color:var(--bs-danger-bg-subtle)!important}.bg-light-subtle{background-color:var(--bs-light-bg-subtle)!important}.bg-dark-subtle{background-color:var(--bs-dark-bg-subtle)!important}.bg-gradient{background-image:var(--bs-gradient)!important}.user-select-all{user-select:all!important}.user-select-auto{user-select:auto!important}.user-select-none{user-select:none!important}.pe-none{pointer-events:none!important}.pe-auto{pointer-events:auto!important}.rounded{border-radius:var(--bs-border-radius)!important}.rounded-0{border-radius:0!important}.rounded-1{border-radius:var(--bs-border-radius-sm)!important}.rounded-2{border-radius:var(--bs-border-radius)!important}.rounded-3{border-radius:var(--bs-border-radius-lg)!important}.rounded-4{border-radius:var(--bs-border-radius-xl)!important}.rounded-5{border-radius:var(--bs-border-radius-xxl)!important}.rounded-circle{border-radius:50%!important}.rounded-pill{border-radius:var(--bs-border-radius-pill)!important}.rounded-top{border-top-left-radius:var(--bs-border-radius)!important;border-top-right-radius:var(--bs-border-radius)!important}.rounded-top-0{border-top-left-radius:0!important;border-top-right-radius:0!important}.rounded-top-1{border-top-left-radius:var(--bs-border-radius-sm)!important;border-top-right-radius:var(--bs-border-radius-sm)!important}.rounded-top-2{border-top-left-radius:var(--bs-border-radius)!important;border-top-right-radius:var(--bs-border-radius)!important}.rounded-top-3{border-top-left-radius:var(--bs-border-radius-lg)!important;border-top-right-radius:var(--bs-border-radius-lg)!important}.rounded-top-4{border-top-left-radius:var(--bs-border-radius-xl)!important;border-top-right-radius:var(--bs-border-radius-xl)!important}.rounded-top-5{border-top-left-radius:var(--bs-border-radius-xxl)!important;border-top-right-radius:var(--bs-border-radius-xxl)!important}.rounded-top-circle{border-top-left-radius:50%!important;border-top-right-radius:50%!important}.rounded-top-pill{border-top-left-radius:var(--bs-border-radius-pill)!important;border-top-right-radius:var(--bs-border-radius-pill)!important}.rounded-end{border-top-right-radius:var(--bs-border-radius)!important;border-bottom-right-radius:var(--bs-border-radius)!important}.rounded-end-0{border-top-right-radius:0!important;border-bottom-right-radius:0!important}.rounded-end-1{border-top-right-radius:var(--bs-border-radius-sm)!important;border-bottom-right-radius:var(--bs-border-radius-sm)!important}.rounded-end-2{border-top-right-radius:var(--bs-border-radius)!important;border-bottom-right-radius:var(--bs-border-radius)!important}.rounded-end-3{border-top-right-radius:var(--bs-border-radius-lg)!important;border-bottom-right-radius:var(--bs-border-radius-lg)!important}.rounded-end-4{border-top-right-radius:var(--bs-border-radius-xl)!important;border-bottom-right-radius:var(--bs-border-radius-xl)!important}.rounded-end-5{border-top-right-radius:var(--bs-border-radius-xxl)!important;border-bottom-right-radius:var(--bs-border-radius-xxl)!important}.rounded-end-circle{border-top-right-radius:50%!important;border-bottom-right-radius:50%!important}.rounded-end-pill{border-top-right-radius:var(--bs-border-radius-pill)!important;border-bottom-right-radius:var(--bs-border-radius-pill)!important}.rounded-bottom{border-bottom-right-radius:var(--bs-border-radius)!important;border-bottom-left-radius:var(--bs-border-radius)!important}.rounded-bottom-0{border-bottom-right-radius:0!important;border-bottom-left-radius:0!important}.rounded-bottom-1{border-bottom-right-radius:var(--bs-border-radius-sm)!important;border-bottom-left-radius:var(--bs-border-radius-sm)!important}.rounded-bottom-2{border-bottom-right-radius:var(--bs-border-radius)!important;border-bottom-left-radius:var(--bs-border-radius)!important}.rounded-bottom-3{border-bottom-right-radius:var(--bs-border-radius-lg)!important;border-bottom-left-radius:var(--bs-border-radius-lg)!important}.rounded-bottom-4{border-bottom-right-radius:var(--bs-border-radius-xl)!important;border-bottom-left-radius:var(--bs-border-radius-xl)!important}.rounded-bottom-5{border-bottom-right-radius:var(--bs-border-radius-xxl)!important;border-bottom-left-radius:var(--bs-border-radius-xxl)!important}.rounded-bottom-circle{border-bottom-right-radius:50%!important;border-bottom-left-radius:50%!important}.rounded-bottom-pill{border-bottom-right-radius:var(--bs-border-radius-pill)!important;border-bottom-left-radius:var(--bs-border-radius-pill)!important}.rounded-start{border-bottom-left-radius:var(--bs-border-radius)!important;border-top-left-radius:var(--bs-border-radius)!important}.rounded-start-0{border-bottom-left-radius:0!important;border-top-left-radius:0!important}.rounded-start-1{border-bottom-left-radius:var(--bs-border-radius-sm)!important;border-top-left-radius:var(--bs-border-radius-sm)!important}.rounded-start-2{border-bottom-left-radius:var(--bs-border-radius)!important;border-top-left-radius:var(--bs-border-radius)!important}.rounded-start-3{border-bottom-left-radius:var(--bs-border-radius-lg)!important;border-top-left-radius:var(--bs-border-radius-lg)!important}.rounded-start-4{border-bottom-left-radius:var(--bs-border-radius-xl)!important;border-top-left-radius:var(--bs-border-radius-xl)!important}.rounded-start-5{border-bottom-left-radius:var(--bs-border-radius-xxl)!important;border-top-left-radius:var(--bs-border-radius-xxl)!important}.rounded-start-circle{border-bottom-left-radius:50%!important;border-top-left-radius:50%!important}.rounded-start-pill{border-bottom-left-radius:var(--bs-border-radius-pill)!important;border-top-left-radius:var(--bs-border-radius-pill)!important}.visible{visibility:visible!important}.invisible{visibility:hidden!important}.z-n1{z-index:-1!important}.z-0{z-index:0!important}.z-1{z-index:1!important}.z-2{z-index:2!important}.z-3{z-index:3!important}@media (min-width: 576px){.float-sm-start{float:left!important}.float-sm-end{float:right!important}.float-sm-none{float:none!important}.object-fit-sm-contain{object-fit:contain!important}.object-fit-sm-cover{object-fit:cover!important}.object-fit-sm-fill{object-fit:fill!important}.object-fit-sm-scale{object-fit:scale-down!important}.object-fit-sm-none{object-fit:none!important}.d-sm-inline{display:inline!important}.d-sm-inline-block{display:inline-block!important}.d-sm-block{display:block!important}.d-sm-grid{display:grid!important}.d-sm-inline-grid{display:inline-grid!important}.d-sm-table{display:table!important}.d-sm-table-row{display:table-row!important}.d-sm-table-cell{display:table-cell!important}.d-sm-flex{display:flex!important}.d-sm-inline-flex{display:inline-flex!important}.d-sm-none{display:none!important}.flex-sm-fill{flex:1 1 auto!important}.flex-sm-row{flex-direction:row!important}.flex-sm-column{flex-direction:column!important}.flex-sm-row-reverse{flex-direction:row-reverse!important}.flex-sm-column-reverse{flex-direction:column-reverse!important}.flex-sm-grow-0{flex-grow:0!important}.flex-sm-grow-1{flex-grow:1!important}.flex-sm-shrink-0{flex-shrink:0!important}.flex-sm-shrink-1{flex-shrink:1!important}.flex-sm-wrap{flex-wrap:wrap!important}.flex-sm-nowrap{flex-wrap:nowrap!important}.flex-sm-wrap-reverse{flex-wrap:wrap-reverse!important}.justify-content-sm-start{justify-content:flex-start!important}.justify-content-sm-end{justify-content:flex-end!important}.justify-content-sm-center{justify-content:center!important}.justify-content-sm-between{justify-content:space-between!important}.justify-content-sm-around{justify-content:space-around!important}.justify-content-sm-evenly{justify-content:space-evenly!important}.align-items-sm-start{align-items:flex-start!important}.align-items-sm-end{align-items:flex-end!important}.align-items-sm-center{align-items:center!important}.align-items-sm-baseline{align-items:baseline!important}.align-items-sm-stretch{align-items:stretch!important}.align-content-sm-start{align-content:flex-start!important}.align-content-sm-end{align-content:flex-end!important}.align-content-sm-center{align-content:center!important}.align-content-sm-between{align-content:space-between!important}.align-content-sm-around{align-content:space-around!important}.align-content-sm-stretch{align-content:stretch!important}.align-self-sm-auto{align-self:auto!important}.align-self-sm-start{align-self:flex-start!important}.align-self-sm-end{align-self:flex-end!important}.align-self-sm-center{align-self:center!important}.align-self-sm-baseline{align-self:baseline!important}.align-self-sm-stretch{align-self:stretch!important}.order-sm-first{order:-1!important}.order-sm-0{order:0!important}.order-sm-1{order:1!important}.order-sm-2{order:2!important}.order-sm-3{order:3!important}.order-sm-4{order:4!important}.order-sm-5{order:5!important}.order-sm-last{order:6!important}.m-sm-0{margin:0!important}.m-sm-1{margin:.25rem!important}.m-sm-2{margin:.5rem!important}.m-sm-3{margin:1rem!important}.m-sm-4{margin:1.5rem!important}.m-sm-5{margin:3rem!important}.m-sm-auto{margin:auto!important}.mx-sm-0{margin-right:0!important;margin-left:0!important}.mx-sm-1{margin-right:.25rem!important;margin-left:.25rem!important}.mx-sm-2{margin-right:.5rem!important;margin-left:.5rem!important}.mx-sm-3{margin-right:1rem!important;margin-left:1rem!important}.mx-sm-4{margin-right:1.5rem!important;margin-left:1.5rem!important}.mx-sm-5{margin-right:3rem!important;margin-left:3rem!important}.mx-sm-auto{margin-right:auto!important;margin-left:auto!important}.my-sm-0{margin-top:0!important;margin-bottom:0!important}.my-sm-1{margin-top:.25rem!important;margin-bottom:.25rem!important}.my-sm-2{margin-top:.5rem!important;margin-bottom:.5rem!important}.my-sm-3{margin-top:1rem!important;margin-bottom:1rem!important}.my-sm-4{margin-top:1.5rem!important;margin-bottom:1.5rem!important}.my-sm-5{margin-top:3rem!important;margin-bottom:3rem!important}.my-sm-auto{margin-top:auto!important;margin-bottom:auto!important}.mt-sm-0{margin-top:0!important}.mt-sm-1{margin-top:.25rem!important}.mt-sm-2{margin-top:.5rem!important}.mt-sm-3{margin-top:1rem!important}.mt-sm-4{margin-top:1.5rem!important}.mt-sm-5{margin-top:3rem!important}.mt-sm-auto{margin-top:auto!important}.me-sm-0{margin-right:0!important}.me-sm-1{margin-right:.25rem!important}.me-sm-2{margin-right:.5rem!important}.me-sm-3{margin-right:1rem!important}.me-sm-4{margin-right:1.5rem!important}.me-sm-5{margin-right:3rem!important}.me-sm-auto{margin-right:auto!important}.mb-sm-0{margin-bottom:0!important}.mb-sm-1{margin-bottom:.25rem!important}.mb-sm-2{margin-bottom:.5rem!important}.mb-sm-3{margin-bottom:1rem!important}.mb-sm-4{margin-bottom:1.5rem!important}.mb-sm-5{margin-bottom:3rem!important}.mb-sm-auto{margin-bottom:auto!important}.ms-sm-0{margin-left:0!important}.ms-sm-1{margin-left:.25rem!important}.ms-sm-2{margin-left:.5rem!important}.ms-sm-3{margin-left:1rem!important}.ms-sm-4{margin-left:1.5rem!important}.ms-sm-5{margin-left:3rem!important}.ms-sm-auto{margin-left:auto!important}.p-sm-0{padding:0!important}.p-sm-1{padding:.25rem!important}.p-sm-2{padding:.5rem!important}.p-sm-3{padding:1rem!important}.p-sm-4{padding:1.5rem!important}.p-sm-5{padding:3rem!important}.px-sm-0{padding-right:0!important;padding-left:0!important}.px-sm-1{padding-right:.25rem!important;padding-left:.25rem!important}.px-sm-2{padding-right:.5rem!important;padding-left:.5rem!important}.px-sm-3{padding-right:1rem!important;padding-left:1rem!important}.px-sm-4{padding-right:1.5rem!important;padding-left:1.5rem!important}.px-sm-5{padding-right:3rem!important;padding-left:3rem!important}.py-sm-0{padding-top:0!important;padding-bottom:0!important}.py-sm-1{padding-top:.25rem!important;padding-bottom:.25rem!important}.py-sm-2{padding-top:.5rem!important;padding-bottom:.5rem!important}.py-sm-3{padding-top:1rem!important;padding-bottom:1rem!important}.py-sm-4{padding-top:1.5rem!important;padding-bottom:1.5rem!important}.py-sm-5{padding-top:3rem!important;padding-bottom:3rem!important}.pt-sm-0{padding-top:0!important}.pt-sm-1{padding-top:.25rem!important}.pt-sm-2{padding-top:.5rem!important}.pt-sm-3{padding-top:1rem!important}.pt-sm-4{padding-top:1.5rem!important}.pt-sm-5{padding-top:3rem!important}.pe-sm-0{padding-right:0!important}.pe-sm-1{padding-right:.25rem!important}.pe-sm-2{padding-right:.5rem!important}.pe-sm-3{padding-right:1rem!important}.pe-sm-4{padding-right:1.5rem!important}.pe-sm-5{padding-right:3rem!important}.pb-sm-0{padding-bottom:0!important}.pb-sm-1{padding-bottom:.25rem!important}.pb-sm-2{padding-bottom:.5rem!important}.pb-sm-3{padding-bottom:1rem!important}.pb-sm-4{padding-bottom:1.5rem!important}.pb-sm-5{padding-bottom:3rem!important}.ps-sm-0{padding-left:0!important}.ps-sm-1{padding-left:.25rem!important}.ps-sm-2{padding-left:.5rem!important}.ps-sm-3{padding-left:1rem!important}.ps-sm-4{padding-left:1.5rem!important}.ps-sm-5{padding-left:3rem!important}.gap-sm-0{gap:0!important}.gap-sm-1{gap:.25rem!important}.gap-sm-2{gap:.5rem!important}.gap-sm-3{gap:1rem!important}.gap-sm-4{gap:1.5rem!important}.gap-sm-5{gap:3rem!important}.row-gap-sm-0{row-gap:0!important}.row-gap-sm-1{row-gap:.25rem!important}.row-gap-sm-2{row-gap:.5rem!important}.row-gap-sm-3{row-gap:1rem!important}.row-gap-sm-4{row-gap:1.5rem!important}.row-gap-sm-5{row-gap:3rem!important}.column-gap-sm-0{column-gap:0!important}.column-gap-sm-1{column-gap:.25rem!important}.column-gap-sm-2{column-gap:.5rem!important}.column-gap-sm-3{column-gap:1rem!important}.column-gap-sm-4{column-gap:1.5rem!important}.column-gap-sm-5{column-gap:3rem!important}.text-sm-start{text-align:left!important}.text-sm-end{text-align:right!important}.text-sm-center{text-align:center!important}}@media (min-width: 768px){.float-md-start{float:left!important}.float-md-end{float:right!important}.float-md-none{float:none!important}.object-fit-md-contain{object-fit:contain!important}.object-fit-md-cover{object-fit:cover!important}.object-fit-md-fill{object-fit:fill!important}.object-fit-md-scale{object-fit:scale-down!important}.object-fit-md-none{object-fit:none!important}.d-md-inline{display:inline!important}.d-md-inline-block{display:inline-block!important}.d-md-block{display:block!important}.d-md-grid{display:grid!important}.d-md-inline-grid{display:inline-grid!important}.d-md-table{display:table!important}.d-md-table-row{display:table-row!important}.d-md-table-cell{display:table-cell!important}.d-md-flex{display:flex!important}.d-md-inline-flex{display:inline-flex!important}.d-md-none{display:none!important}.flex-md-fill{flex:1 1 auto!important}.flex-md-row{flex-direction:row!important}.flex-md-column{flex-direction:column!important}.flex-md-row-reverse{flex-direction:row-reverse!important}.flex-md-column-reverse{flex-direction:column-reverse!important}.flex-md-grow-0{flex-grow:0!important}.flex-md-grow-1{flex-grow:1!important}.flex-md-shrink-0{flex-shrink:0!important}.flex-md-shrink-1{flex-shrink:1!important}.flex-md-wrap{flex-wrap:wrap!important}.flex-md-nowrap{flex-wrap:nowrap!important}.flex-md-wrap-reverse{flex-wrap:wrap-reverse!important}.justify-content-md-start{justify-content:flex-start!important}.justify-content-md-end{justify-content:flex-end!important}.justify-content-md-center{justify-content:center!important}.justify-content-md-between{justify-content:space-between!important}.justify-content-md-around{justify-content:space-around!important}.justify-content-md-evenly{justify-content:space-evenly!important}.align-items-md-start{align-items:flex-start!important}.align-items-md-end{align-items:flex-end!important}.align-items-md-center{align-items:center!important}.align-items-md-baseline{align-items:baseline!important}.align-items-md-stretch{align-items:stretch!important}.align-content-md-start{align-content:flex-start!important}.align-content-md-end{align-content:flex-end!important}.align-content-md-center{align-content:center!important}.align-content-md-between{align-content:space-between!important}.align-content-md-around{align-content:space-around!important}.align-content-md-stretch{align-content:stretch!important}.align-self-md-auto{align-self:auto!important}.align-self-md-start{align-self:flex-start!important}.align-self-md-end{align-self:flex-end!important}.align-self-md-center{align-self:center!important}.align-self-md-baseline{align-self:baseline!important}.align-self-md-stretch{align-self:stretch!important}.order-md-first{order:-1!important}.order-md-0{order:0!important}.order-md-1{order:1!important}.order-md-2{order:2!important}.order-md-3{order:3!important}.order-md-4{order:4!important}.order-md-5{order:5!important}.order-md-last{order:6!important}.m-md-0{margin:0!important}.m-md-1{margin:.25rem!important}.m-md-2{margin:.5rem!important}.m-md-3{margin:1rem!important}.m-md-4{margin:1.5rem!important}.m-md-5{margin:3rem!important}.m-md-auto{margin:auto!important}.mx-md-0{margin-right:0!important;margin-left:0!important}.mx-md-1{margin-right:.25rem!important;margin-left:.25rem!important}.mx-md-2{margin-right:.5rem!important;margin-left:.5rem!important}.mx-md-3{margin-right:1rem!important;margin-left:1rem!important}.mx-md-4{margin-right:1.5rem!important;margin-left:1.5rem!important}.mx-md-5{margin-right:3rem!important;margin-left:3rem!important}.mx-md-auto{margin-right:auto!important;margin-left:auto!important}.my-md-0{margin-top:0!important;margin-bottom:0!important}.my-md-1{margin-top:.25rem!important;margin-bottom:.25rem!important}.my-md-2{margin-top:.5rem!important;margin-bottom:.5rem!important}.my-md-3{margin-top:1rem!important;margin-bottom:1rem!important}.my-md-4{margin-top:1.5rem!important;margin-bottom:1.5rem!important}.my-md-5{margin-top:3rem!important;margin-bottom:3rem!important}.my-md-auto{margin-top:auto!important;margin-bottom:auto!important}.mt-md-0{margin-top:0!important}.mt-md-1{margin-top:.25rem!important}.mt-md-2{margin-top:.5rem!important}.mt-md-3{margin-top:1rem!important}.mt-md-4{margin-top:1.5rem!important}.mt-md-5{margin-top:3rem!important}.mt-md-auto{margin-top:auto!important}.me-md-0{margin-right:0!important}.me-md-1{margin-right:.25rem!important}.me-md-2{margin-right:.5rem!important}.me-md-3{margin-right:1rem!important}.me-md-4{margin-right:1.5rem!important}.me-md-5{margin-right:3rem!important}.me-md-auto{margin-right:auto!important}.mb-md-0{margin-bottom:0!important}.mb-md-1{margin-bottom:.25rem!important}.mb-md-2{margin-bottom:.5rem!important}.mb-md-3{margin-bottom:1rem!important}.mb-md-4{margin-bottom:1.5rem!important}.mb-md-5{margin-bottom:3rem!important}.mb-md-auto{margin-bottom:auto!important}.ms-md-0{margin-left:0!important}.ms-md-1{margin-left:.25rem!important}.ms-md-2{margin-left:.5rem!important}.ms-md-3{margin-left:1rem!important}.ms-md-4{margin-left:1.5rem!important}.ms-md-5{margin-left:3rem!important}.ms-md-auto{margin-left:auto!important}.p-md-0{padding:0!important}.p-md-1{padding:.25rem!important}.p-md-2{padding:.5rem!important}.p-md-3{padding:1rem!important}.p-md-4{padding:1.5rem!important}.p-md-5{padding:3rem!important}.px-md-0{padding-right:0!important;padding-left:0!important}.px-md-1{padding-right:.25rem!important;padding-left:.25rem!important}.px-md-2{padding-right:.5rem!important;padding-left:.5rem!important}.px-md-3{padding-right:1rem!important;padding-left:1rem!important}.px-md-4{padding-right:1.5rem!important;padding-left:1.5rem!important}.px-md-5{padding-right:3rem!important;padding-left:3rem!important}.py-md-0{padding-top:0!important;padding-bottom:0!important}.py-md-1{padding-top:.25rem!important;padding-bottom:.25rem!important}.py-md-2{padding-top:.5rem!important;padding-bottom:.5rem!important}.py-md-3{padding-top:1rem!important;padding-bottom:1rem!important}.py-md-4{padding-top:1.5rem!important;padding-bottom:1.5rem!important}.py-md-5{padding-top:3rem!important;padding-bottom:3rem!important}.pt-md-0{padding-top:0!important}.pt-md-1{padding-top:.25rem!important}.pt-md-2{padding-top:.5rem!important}.pt-md-3{padding-top:1rem!important}.pt-md-4{padding-top:1.5rem!important}.pt-md-5{padding-top:3rem!important}.pe-md-0{padding-right:0!important}.pe-md-1{padding-right:.25rem!important}.pe-md-2{padding-right:.5rem!important}.pe-md-3{padding-right:1rem!important}.pe-md-4{padding-right:1.5rem!important}.pe-md-5{padding-right:3rem!important}.pb-md-0{padding-bottom:0!important}.pb-md-1{padding-bottom:.25rem!important}.pb-md-2{padding-bottom:.5rem!important}.pb-md-3{padding-bottom:1rem!important}.pb-md-4{padding-bottom:1.5rem!important}.pb-md-5{padding-bottom:3rem!important}.ps-md-0{padding-left:0!important}.ps-md-1{padding-left:.25rem!important}.ps-md-2{padding-left:.5rem!important}.ps-md-3{padding-left:1rem!important}.ps-md-4{padding-left:1.5rem!important}.ps-md-5{padding-left:3rem!important}.gap-md-0{gap:0!important}.gap-md-1{gap:.25rem!important}.gap-md-2{gap:.5rem!important}.gap-md-3{gap:1rem!important}.gap-md-4{gap:1.5rem!important}.gap-md-5{gap:3rem!important}.row-gap-md-0{row-gap:0!important}.row-gap-md-1{row-gap:.25rem!important}.row-gap-md-2{row-gap:.5rem!important}.row-gap-md-3{row-gap:1rem!important}.row-gap-md-4{row-gap:1.5rem!important}.row-gap-md-5{row-gap:3rem!important}.column-gap-md-0{column-gap:0!important}.column-gap-md-1{column-gap:.25rem!important}.column-gap-md-2{column-gap:.5rem!important}.column-gap-md-3{column-gap:1rem!important}.column-gap-md-4{column-gap:1.5rem!important}.column-gap-md-5{column-gap:3rem!important}.text-md-start{text-align:left!important}.text-md-end{text-align:right!important}.text-md-center{text-align:center!important}}@media (min-width: 992px){.float-lg-start{float:left!important}.float-lg-end{float:right!important}.float-lg-none{float:none!important}.object-fit-lg-contain{object-fit:contain!important}.object-fit-lg-cover{object-fit:cover!important}.object-fit-lg-fill{object-fit:fill!important}.object-fit-lg-scale{object-fit:scale-down!important}.object-fit-lg-none{object-fit:none!important}.d-lg-inline{display:inline!important}.d-lg-inline-block{display:inline-block!important}.d-lg-block{display:block!important}.d-lg-grid{display:grid!important}.d-lg-inline-grid{display:inline-grid!important}.d-lg-table{display:table!important}.d-lg-table-row{display:table-row!important}.d-lg-table-cell{display:table-cell!important}.d-lg-flex{display:flex!important}.d-lg-inline-flex{display:inline-flex!important}.d-lg-none{display:none!important}.flex-lg-fill{flex:1 1 auto!important}.flex-lg-row{flex-direction:row!important}.flex-lg-column{flex-direction:column!important}.flex-lg-row-reverse{flex-direction:row-reverse!important}.flex-lg-column-reverse{flex-direction:column-reverse!important}.flex-lg-grow-0{flex-grow:0!important}.flex-lg-grow-1{flex-grow:1!important}.flex-lg-shrink-0{flex-shrink:0!important}.flex-lg-shrink-1{flex-shrink:1!important}.flex-lg-wrap{flex-wrap:wrap!important}.flex-lg-nowrap{flex-wrap:nowrap!important}.flex-lg-wrap-reverse{flex-wrap:wrap-reverse!important}.justify-content-lg-start{justify-content:flex-start!important}.justify-content-lg-end{justify-content:flex-end!important}.justify-content-lg-center{justify-content:center!important}.justify-content-lg-between{justify-content:space-between!important}.justify-content-lg-around{justify-content:space-around!important}.justify-content-lg-evenly{justify-content:space-evenly!important}.align-items-lg-start{align-items:flex-start!important}.align-items-lg-end{align-items:flex-end!important}.align-items-lg-center{align-items:center!important}.align-items-lg-baseline{align-items:baseline!important}.align-items-lg-stretch{align-items:stretch!important}.align-content-lg-start{align-content:flex-start!important}.align-content-lg-end{align-content:flex-end!important}.align-content-lg-center{align-content:center!important}.align-content-lg-between{align-content:space-between!important}.align-content-lg-around{align-content:space-around!important}.align-content-lg-stretch{align-content:stretch!important}.align-self-lg-auto{align-self:auto!important}.align-self-lg-start{align-self:flex-start!important}.align-self-lg-end{align-self:flex-end!important}.align-self-lg-center{align-self:center!important}.align-self-lg-baseline{align-self:baseline!important}.align-self-lg-stretch{align-self:stretch!important}.order-lg-first{order:-1!important}.order-lg-0{order:0!important}.order-lg-1{order:1!important}.order-lg-2{order:2!important}.order-lg-3{order:3!important}.order-lg-4{order:4!important}.order-lg-5{order:5!important}.order-lg-last{order:6!important}.m-lg-0{margin:0!important}.m-lg-1{margin:.25rem!important}.m-lg-2{margin:.5rem!important}.m-lg-3{margin:1rem!important}.m-lg-4{margin:1.5rem!important}.m-lg-5{margin:3rem!important}.m-lg-auto{margin:auto!important}.mx-lg-0{margin-right:0!important;margin-left:0!important}.mx-lg-1{margin-right:.25rem!important;margin-left:.25rem!important}.mx-lg-2{margin-right:.5rem!important;margin-left:.5rem!important}.mx-lg-3{margin-right:1rem!important;margin-left:1rem!important}.mx-lg-4{margin-right:1.5rem!important;margin-left:1.5rem!important}.mx-lg-5{margin-right:3rem!important;margin-left:3rem!important}.mx-lg-auto{margin-right:auto!important;margin-left:auto!important}.my-lg-0{margin-top:0!important;margin-bottom:0!important}.my-lg-1{margin-top:.25rem!important;margin-bottom:.25rem!important}.my-lg-2{margin-top:.5rem!important;margin-bottom:.5rem!important}.my-lg-3{margin-top:1rem!important;margin-bottom:1rem!important}.my-lg-4{margin-top:1.5rem!important;margin-bottom:1.5rem!important}.my-lg-5{margin-top:3rem!important;margin-bottom:3rem!important}.my-lg-auto{margin-top:auto!important;margin-bottom:auto!important}.mt-lg-0{margin-top:0!important}.mt-lg-1{margin-top:.25rem!important}.mt-lg-2{margin-top:.5rem!important}.mt-lg-3{margin-top:1rem!important}.mt-lg-4{margin-top:1.5rem!important}.mt-lg-5{margin-top:3rem!important}.mt-lg-auto{margin-top:auto!important}.me-lg-0{margin-right:0!important}.me-lg-1{margin-right:.25rem!important}.me-lg-2{margin-right:.5rem!important}.me-lg-3{margin-right:1rem!important}.me-lg-4{margin-right:1.5rem!important}.me-lg-5{margin-right:3rem!important}.me-lg-auto{margin-right:auto!important}.mb-lg-0{margin-bottom:0!important}.mb-lg-1{margin-bottom:.25rem!important}.mb-lg-2{margin-bottom:.5rem!important}.mb-lg-3{margin-bottom:1rem!important}.mb-lg-4{margin-bottom:1.5rem!important}.mb-lg-5{margin-bottom:3rem!important}.mb-lg-auto{margin-bottom:auto!important}.ms-lg-0{margin-left:0!important}.ms-lg-1{margin-left:.25rem!important}.ms-lg-2{margin-left:.5rem!important}.ms-lg-3{margin-left:1rem!important}.ms-lg-4{margin-left:1.5rem!important}.ms-lg-5{margin-left:3rem!important}.ms-lg-auto{margin-left:auto!important}.p-lg-0{padding:0!important}.p-lg-1{padding:.25rem!important}.p-lg-2{padding:.5rem!important}.p-lg-3{padding:1rem!important}.p-lg-4{padding:1.5rem!important}.p-lg-5{padding:3rem!important}.px-lg-0{padding-right:0!important;padding-left:0!important}.px-lg-1{padding-right:.25rem!important;padding-left:.25rem!important}.px-lg-2{padding-right:.5rem!important;padding-left:.5rem!important}.px-lg-3{padding-right:1rem!important;padding-left:1rem!important}.px-lg-4{padding-right:1.5rem!important;padding-left:1.5rem!important}.px-lg-5{padding-right:3rem!important;padding-left:3rem!important}.py-lg-0{padding-top:0!important;padding-bottom:0!important}.py-lg-1{padding-top:.25rem!important;padding-bottom:.25rem!important}.py-lg-2{padding-top:.5rem!important;padding-bottom:.5rem!important}.py-lg-3{padding-top:1rem!important;padding-bottom:1rem!important}.py-lg-4{padding-top:1.5rem!important;padding-bottom:1.5rem!important}.py-lg-5{padding-top:3rem!important;padding-bottom:3rem!important}.pt-lg-0{padding-top:0!important}.pt-lg-1{padding-top:.25rem!important}.pt-lg-2{padding-top:.5rem!important}.pt-lg-3{padding-top:1rem!important}.pt-lg-4{padding-top:1.5rem!important}.pt-lg-5{padding-top:3rem!important}.pe-lg-0{padding-right:0!important}.pe-lg-1{padding-right:.25rem!important}.pe-lg-2{padding-right:.5rem!important}.pe-lg-3{padding-right:1rem!important}.pe-lg-4{padding-right:1.5rem!important}.pe-lg-5{padding-right:3rem!important}.pb-lg-0{padding-bottom:0!important}.pb-lg-1{padding-bottom:.25rem!important}.pb-lg-2{padding-bottom:.5rem!important}.pb-lg-3{padding-bottom:1rem!important}.pb-lg-4{padding-bottom:1.5rem!important}.pb-lg-5{padding-bottom:3rem!important}.ps-lg-0{padding-left:0!important}.ps-lg-1{padding-left:.25rem!important}.ps-lg-2{padding-left:.5rem!important}.ps-lg-3{padding-left:1rem!important}.ps-lg-4{padding-left:1.5rem!important}.ps-lg-5{padding-left:3rem!important}.gap-lg-0{gap:0!important}.gap-lg-1{gap:.25rem!important}.gap-lg-2{gap:.5rem!important}.gap-lg-3{gap:1rem!important}.gap-lg-4{gap:1.5rem!important}.gap-lg-5{gap:3rem!important}.row-gap-lg-0{row-gap:0!important}.row-gap-lg-1{row-gap:.25rem!important}.row-gap-lg-2{row-gap:.5rem!important}.row-gap-lg-3{row-gap:1rem!important}.row-gap-lg-4{row-gap:1.5rem!important}.row-gap-lg-5{row-gap:3rem!important}.column-gap-lg-0{column-gap:0!important}.column-gap-lg-1{column-gap:.25rem!important}.column-gap-lg-2{column-gap:.5rem!important}.column-gap-lg-3{column-gap:1rem!important}.column-gap-lg-4{column-gap:1.5rem!important}.column-gap-lg-5{column-gap:3rem!important}.text-lg-start{text-align:left!important}.text-lg-end{text-align:right!important}.text-lg-center{text-align:center!important}}@media (min-width: 1200px){.float-xl-start{float:left!important}.float-xl-end{float:right!important}.float-xl-none{float:none!important}.object-fit-xl-contain{object-fit:contain!important}.object-fit-xl-cover{object-fit:cover!important}.object-fit-xl-fill{object-fit:fill!important}.object-fit-xl-scale{object-fit:scale-down!important}.object-fit-xl-none{object-fit:none!important}.d-xl-inline{display:inline!important}.d-xl-inline-block{display:inline-block!important}.d-xl-block{display:block!important}.d-xl-grid{display:grid!important}.d-xl-inline-grid{display:inline-grid!important}.d-xl-table{display:table!important}.d-xl-table-row{display:table-row!important}.d-xl-table-cell{display:table-cell!important}.d-xl-flex{display:flex!important}.d-xl-inline-flex{display:inline-flex!important}.d-xl-none{display:none!important}.flex-xl-fill{flex:1 1 auto!important}.flex-xl-row{flex-direction:row!important}.flex-xl-column{flex-direction:column!important}.flex-xl-row-reverse{flex-direction:row-reverse!important}.flex-xl-column-reverse{flex-direction:column-reverse!important}.flex-xl-grow-0{flex-grow:0!important}.flex-xl-grow-1{flex-grow:1!important}.flex-xl-shrink-0{flex-shrink:0!important}.flex-xl-shrink-1{flex-shrink:1!important}.flex-xl-wrap{flex-wrap:wrap!important}.flex-xl-nowrap{flex-wrap:nowrap!important}.flex-xl-wrap-reverse{flex-wrap:wrap-reverse!important}.justify-content-xl-start{justify-content:flex-start!important}.justify-content-xl-end{justify-content:flex-end!important}.justify-content-xl-center{justify-content:center!important}.justify-content-xl-between{justify-content:space-between!important}.justify-content-xl-around{justify-content:space-around!important}.justify-content-xl-evenly{justify-content:space-evenly!important}.align-items-xl-start{align-items:flex-start!important}.align-items-xl-end{align-items:flex-end!important}.align-items-xl-center{align-items:center!important}.align-items-xl-baseline{align-items:baseline!important}.align-items-xl-stretch{align-items:stretch!important}.align-content-xl-start{align-content:flex-start!important}.align-content-xl-end{align-content:flex-end!important}.align-content-xl-center{align-content:center!important}.align-content-xl-between{align-content:space-between!important}.align-content-xl-around{align-content:space-around!important}.align-content-xl-stretch{align-content:stretch!important}.align-self-xl-auto{align-self:auto!important}.align-self-xl-start{align-self:flex-start!important}.align-self-xl-end{align-self:flex-end!important}.align-self-xl-center{align-self:center!important}.align-self-xl-baseline{align-self:baseline!important}.align-self-xl-stretch{align-self:stretch!important}.order-xl-first{order:-1!important}.order-xl-0{order:0!important}.order-xl-1{order:1!important}.order-xl-2{order:2!important}.order-xl-3{order:3!important}.order-xl-4{order:4!important}.order-xl-5{order:5!important}.order-xl-last{order:6!important}.m-xl-0{margin:0!important}.m-xl-1{margin:.25rem!important}.m-xl-2{margin:.5rem!important}.m-xl-3{margin:1rem!important}.m-xl-4{margin:1.5rem!important}.m-xl-5{margin:3rem!important}.m-xl-auto{margin:auto!important}.mx-xl-0{margin-right:0!important;margin-left:0!important}.mx-xl-1{margin-right:.25rem!important;margin-left:.25rem!important}.mx-xl-2{margin-right:.5rem!important;margin-left:.5rem!important}.mx-xl-3{margin-right:1rem!important;margin-left:1rem!important}.mx-xl-4{margin-right:1.5rem!important;margin-left:1.5rem!important}.mx-xl-5{margin-right:3rem!important;margin-left:3rem!important}.mx-xl-auto{margin-right:auto!important;margin-left:auto!important}.my-xl-0{margin-top:0!important;margin-bottom:0!important}.my-xl-1{margin-top:.25rem!important;margin-bottom:.25rem!important}.my-xl-2{margin-top:.5rem!important;margin-bottom:.5rem!important}.my-xl-3{margin-top:1rem!important;margin-bottom:1rem!important}.my-xl-4{margin-top:1.5rem!important;margin-bottom:1.5rem!important}.my-xl-5{margin-top:3rem!important;margin-bottom:3rem!important}.my-xl-auto{margin-top:auto!important;margin-bottom:auto!important}.mt-xl-0{margin-top:0!important}.mt-xl-1{margin-top:.25rem!important}.mt-xl-2{margin-top:.5rem!important}.mt-xl-3{margin-top:1rem!important}.mt-xl-4{margin-top:1.5rem!important}.mt-xl-5{margin-top:3rem!important}.mt-xl-auto{margin-top:auto!important}.me-xl-0{margin-right:0!important}.me-xl-1{margin-right:.25rem!important}.me-xl-2{margin-right:.5rem!important}.me-xl-3{margin-right:1rem!important}.me-xl-4{margin-right:1.5rem!important}.me-xl-5{margin-right:3rem!important}.me-xl-auto{margin-right:auto!important}.mb-xl-0{margin-bottom:0!important}.mb-xl-1{margin-bottom:.25rem!important}.mb-xl-2{margin-bottom:.5rem!important}.mb-xl-3{margin-bottom:1rem!important}.mb-xl-4{margin-bottom:1.5rem!important}.mb-xl-5{margin-bottom:3rem!important}.mb-xl-auto{margin-bottom:auto!important}.ms-xl-0{margin-left:0!important}.ms-xl-1{margin-left:.25rem!important}.ms-xl-2{margin-left:.5rem!important}.ms-xl-3{margin-left:1rem!important}.ms-xl-4{margin-left:1.5rem!important}.ms-xl-5{margin-left:3rem!important}.ms-xl-auto{margin-left:auto!important}.p-xl-0{padding:0!important}.p-xl-1{padding:.25rem!important}.p-xl-2{padding:.5rem!important}.p-xl-3{padding:1rem!important}.p-xl-4{padding:1.5rem!important}.p-xl-5{padding:3rem!important}.px-xl-0{padding-right:0!important;padding-left:0!important}.px-xl-1{padding-right:.25rem!important;padding-left:.25rem!important}.px-xl-2{padding-right:.5rem!important;padding-left:.5rem!important}.px-xl-3{padding-right:1rem!important;padding-left:1rem!important}.px-xl-4{padding-right:1.5rem!important;padding-left:1.5rem!important}.px-xl-5{padding-right:3rem!important;padding-left:3rem!important}.py-xl-0{padding-top:0!important;padding-bottom:0!important}.py-xl-1{padding-top:.25rem!important;padding-bottom:.25rem!important}.py-xl-2{padding-top:.5rem!important;padding-bottom:.5rem!important}.py-xl-3{padding-top:1rem!important;padding-bottom:1rem!important}.py-xl-4{padding-top:1.5rem!important;padding-bottom:1.5rem!important}.py-xl-5{padding-top:3rem!important;padding-bottom:3rem!important}.pt-xl-0{padding-top:0!important}.pt-xl-1{padding-top:.25rem!important}.pt-xl-2{padding-top:.5rem!important}.pt-xl-3{padding-top:1rem!important}.pt-xl-4{padding-top:1.5rem!important}.pt-xl-5{padding-top:3rem!important}.pe-xl-0{padding-right:0!important}.pe-xl-1{padding-right:.25rem!important}.pe-xl-2{padding-right:.5rem!important}.pe-xl-3{padding-right:1rem!important}.pe-xl-4{padding-right:1.5rem!important}.pe-xl-5{padding-right:3rem!important}.pb-xl-0{padding-bottom:0!important}.pb-xl-1{padding-bottom:.25rem!important}.pb-xl-2{padding-bottom:.5rem!important}.pb-xl-3{padding-bottom:1rem!important}.pb-xl-4{padding-bottom:1.5rem!important}.pb-xl-5{padding-bottom:3rem!important}.ps-xl-0{padding-left:0!important}.ps-xl-1{padding-left:.25rem!important}.ps-xl-2{padding-left:.5rem!important}.ps-xl-3{padding-left:1rem!important}.ps-xl-4{padding-left:1.5rem!important}.ps-xl-5{padding-left:3rem!important}.gap-xl-0{gap:0!important}.gap-xl-1{gap:.25rem!important}.gap-xl-2{gap:.5rem!important}.gap-xl-3{gap:1rem!important}.gap-xl-4{gap:1.5rem!important}.gap-xl-5{gap:3rem!important}.row-gap-xl-0{row-gap:0!important}.row-gap-xl-1{row-gap:.25rem!important}.row-gap-xl-2{row-gap:.5rem!important}.row-gap-xl-3{row-gap:1rem!important}.row-gap-xl-4{row-gap:1.5rem!important}.row-gap-xl-5{row-gap:3rem!important}.column-gap-xl-0{column-gap:0!important}.column-gap-xl-1{column-gap:.25rem!important}.column-gap-xl-2{column-gap:.5rem!important}.column-gap-xl-3{column-gap:1rem!important}.column-gap-xl-4{column-gap:1.5rem!important}.column-gap-xl-5{column-gap:3rem!important}.text-xl-start{text-align:left!important}.text-xl-end{text-align:right!important}.text-xl-center{text-align:center!important}}@media (min-width: 1400px){.float-xxl-start{float:left!important}.float-xxl-end{float:right!important}.float-xxl-none{float:none!important}.object-fit-xxl-contain{object-fit:contain!important}.object-fit-xxl-cover{object-fit:cover!important}.object-fit-xxl-fill{object-fit:fill!important}.object-fit-xxl-scale{object-fit:scale-down!important}.object-fit-xxl-none{object-fit:none!important}.d-xxl-inline{display:inline!important}.d-xxl-inline-block{display:inline-block!important}.d-xxl-block{display:block!important}.d-xxl-grid{display:grid!important}.d-xxl-inline-grid{display:inline-grid!important}.d-xxl-table{display:table!important}.d-xxl-table-row{display:table-row!important}.d-xxl-table-cell{display:table-cell!important}.d-xxl-flex{display:flex!important}.d-xxl-inline-flex{display:inline-flex!important}.d-xxl-none{display:none!important}.flex-xxl-fill{flex:1 1 auto!important}.flex-xxl-row{flex-direction:row!important}.flex-xxl-column{flex-direction:column!important}.flex-xxl-row-reverse{flex-direction:row-reverse!important}.flex-xxl-column-reverse{flex-direction:column-reverse!important}.flex-xxl-grow-0{flex-grow:0!important}.flex-xxl-grow-1{flex-grow:1!important}.flex-xxl-shrink-0{flex-shrink:0!important}.flex-xxl-shrink-1{flex-shrink:1!important}.flex-xxl-wrap{flex-wrap:wrap!important}.flex-xxl-nowrap{flex-wrap:nowrap!important}.flex-xxl-wrap-reverse{flex-wrap:wrap-reverse!important}.justify-content-xxl-start{justify-content:flex-start!important}.justify-content-xxl-end{justify-content:flex-end!important}.justify-content-xxl-center{justify-content:center!important}.justify-content-xxl-between{justify-content:space-between!important}.justify-content-xxl-around{justify-content:space-around!important}.justify-content-xxl-evenly{justify-content:space-evenly!important}.align-items-xxl-start{align-items:flex-start!important}.align-items-xxl-end{align-items:flex-end!important}.align-items-xxl-center{align-items:center!important}.align-items-xxl-baseline{align-items:baseline!important}.align-items-xxl-stretch{align-items:stretch!important}.align-content-xxl-start{align-content:flex-start!important}.align-content-xxl-end{align-content:flex-end!important}.align-content-xxl-center{align-content:center!important}.align-content-xxl-between{align-content:space-between!important}.align-content-xxl-around{align-content:space-around!important}.align-content-xxl-stretch{align-content:stretch!important}.align-self-xxl-auto{align-self:auto!important}.align-self-xxl-start{align-self:flex-start!important}.align-self-xxl-end{align-self:flex-end!important}.align-self-xxl-center{align-self:center!important}.align-self-xxl-baseline{align-self:baseline!important}.align-self-xxl-stretch{align-self:stretch!important}.order-xxl-first{order:-1!important}.order-xxl-0{order:0!important}.order-xxl-1{order:1!important}.order-xxl-2{order:2!important}.order-xxl-3{order:3!important}.order-xxl-4{order:4!important}.order-xxl-5{order:5!important}.order-xxl-last{order:6!important}.m-xxl-0{margin:0!important}.m-xxl-1{margin:.25rem!important}.m-xxl-2{margin:.5rem!important}.m-xxl-3{margin:1rem!important}.m-xxl-4{margin:1.5rem!important}.m-xxl-5{margin:3rem!important}.m-xxl-auto{margin:auto!important}.mx-xxl-0{margin-right:0!important;margin-left:0!important}.mx-xxl-1{margin-right:.25rem!important;margin-left:.25rem!important}.mx-xxl-2{margin-right:.5rem!important;margin-left:.5rem!important}.mx-xxl-3{margin-right:1rem!important;margin-left:1rem!important}.mx-xxl-4{margin-right:1.5rem!important;margin-left:1.5rem!important}.mx-xxl-5{margin-right:3rem!important;margin-left:3rem!important}.mx-xxl-auto{margin-right:auto!important;margin-left:auto!important}.my-xxl-0{margin-top:0!important;margin-bottom:0!important}.my-xxl-1{margin-top:.25rem!important;margin-bottom:.25rem!important}.my-xxl-2{margin-top:.5rem!important;margin-bottom:.5rem!important}.my-xxl-3{margin-top:1rem!important;margin-bottom:1rem!important}.my-xxl-4{margin-top:1.5rem!important;margin-bottom:1.5rem!important}.my-xxl-5{margin-top:3rem!important;margin-bottom:3rem!important}.my-xxl-auto{margin-top:auto!important;margin-bottom:auto!important}.mt-xxl-0{margin-top:0!important}.mt-xxl-1{margin-top:.25rem!important}.mt-xxl-2{margin-top:.5rem!important}.mt-xxl-3{margin-top:1rem!important}.mt-xxl-4{margin-top:1.5rem!important}.mt-xxl-5{margin-top:3rem!important}.mt-xxl-auto{margin-top:auto!important}.me-xxl-0{margin-right:0!important}.me-xxl-1{margin-right:.25rem!important}.me-xxl-2{margin-right:.5rem!important}.me-xxl-3{margin-right:1rem!important}.me-xxl-4{margin-right:1.5rem!important}.me-xxl-5{margin-right:3rem!important}.me-xxl-auto{margin-right:auto!important}.mb-xxl-0{margin-bottom:0!important}.mb-xxl-1{margin-bottom:.25rem!important}.mb-xxl-2{margin-bottom:.5rem!important}.mb-xxl-3{margin-bottom:1rem!important}.mb-xxl-4{margin-bottom:1.5rem!important}.mb-xxl-5{margin-bottom:3rem!important}.mb-xxl-auto{margin-bottom:auto!important}.ms-xxl-0{margin-left:0!important}.ms-xxl-1{margin-left:.25rem!important}.ms-xxl-2{margin-left:.5rem!important}.ms-xxl-3{margin-left:1rem!important}.ms-xxl-4{margin-left:1.5rem!important}.ms-xxl-5{margin-left:3rem!important}.ms-xxl-auto{margin-left:auto!important}.p-xxl-0{padding:0!important}.p-xxl-1{padding:.25rem!important}.p-xxl-2{padding:.5rem!important}.p-xxl-3{padding:1rem!important}.p-xxl-4{padding:1.5rem!important}.p-xxl-5{padding:3rem!important}.px-xxl-0{padding-right:0!important;padding-left:0!important}.px-xxl-1{padding-right:.25rem!important;padding-left:.25rem!important}.px-xxl-2{padding-right:.5rem!important;padding-left:.5rem!important}.px-xxl-3{padding-right:1rem!important;padding-left:1rem!important}.px-xxl-4{padding-right:1.5rem!important;padding-left:1.5rem!important}.px-xxl-5{padding-right:3rem!important;padding-left:3rem!important}.py-xxl-0{padding-top:0!important;padding-bottom:0!important}.py-xxl-1{padding-top:.25rem!important;padding-bottom:.25rem!important}.py-xxl-2{padding-top:.5rem!important;padding-bottom:.5rem!important}.py-xxl-3{padding-top:1rem!important;padding-bottom:1rem!important}.py-xxl-4{padding-top:1.5rem!important;padding-bottom:1.5rem!important}.py-xxl-5{padding-top:3rem!important;padding-bottom:3rem!important}.pt-xxl-0{padding-top:0!important}.pt-xxl-1{padding-top:.25rem!important}.pt-xxl-2{padding-top:.5rem!important}.pt-xxl-3{padding-top:1rem!important}.pt-xxl-4{padding-top:1.5rem!important}.pt-xxl-5{padding-top:3rem!important}.pe-xxl-0{padding-right:0!important}.pe-xxl-1{padding-right:.25rem!important}.pe-xxl-2{padding-right:.5rem!important}.pe-xxl-3{padding-right:1rem!important}.pe-xxl-4{padding-right:1.5rem!important}.pe-xxl-5{padding-right:3rem!important}.pb-xxl-0{padding-bottom:0!important}.pb-xxl-1{padding-bottom:.25rem!important}.pb-xxl-2{padding-bottom:.5rem!important}.pb-xxl-3{padding-bottom:1rem!important}.pb-xxl-4{padding-bottom:1.5rem!important}.pb-xxl-5{padding-bottom:3rem!important}.ps-xxl-0{padding-left:0!important}.ps-xxl-1{padding-left:.25rem!important}.ps-xxl-2{padding-left:.5rem!important}.ps-xxl-3{padding-left:1rem!important}.ps-xxl-4{padding-left:1.5rem!important}.ps-xxl-5{padding-left:3rem!important}.gap-xxl-0{gap:0!important}.gap-xxl-1{gap:.25rem!important}.gap-xxl-2{gap:.5rem!important}.gap-xxl-3{gap:1rem!important}.gap-xxl-4{gap:1.5rem!important}.gap-xxl-5{gap:3rem!important}.row-gap-xxl-0{row-gap:0!important}.row-gap-xxl-1{row-gap:.25rem!important}.row-gap-xxl-2{row-gap:.5rem!important}.row-gap-xxl-3{row-gap:1rem!important}.row-gap-xxl-4{row-gap:1.5rem!important}.row-gap-xxl-5{row-gap:3rem!important}.column-gap-xxl-0{column-gap:0!important}.column-gap-xxl-1{column-gap:.25rem!important}.column-gap-xxl-2{column-gap:.5rem!important}.column-gap-xxl-3{column-gap:1rem!important}.column-gap-xxl-4{column-gap:1.5rem!important}.column-gap-xxl-5{column-gap:3rem!important}.text-xxl-start{text-align:left!important}.text-xxl-end{text-align:right!important}.text-xxl-center{text-align:center!important}}@media (min-width: 1200px){.fs-1{font-size:2.5rem!important}.fs-2{font-size:2rem!important}.fs-3{font-size:1.75rem!important}.fs-4{font-size:1.5rem!important}}@media print{.d-print-inline{display:inline!important}.d-print-inline-block{display:inline-block!important}.d-print-block{display:block!important}.d-print-grid{display:grid!important}.d-print-inline-grid{display:inline-grid!important}.d-print-table{display:table!important}.d-print-table-row{display:table-row!important}.d-print-table-cell{display:table-cell!important}.d-print-flex{display:flex!important}.d-print-inline-flex{display:inline-flex!important}.d-print-none{display:none!important}}:root{--bs-dark-rgb: 44, 62, 80}.cm-editor{outline:none!important}.cm-scroller{overflow:auto;min-height:400px;max-height:400px}.cm-content,.cm-gutter{min-height:400px!important}.link-primary{cursor:pointer}.rows-input{text-align:center;width:40px}.overflow-wrapper{overflow:auto;height:500px}.data-headers{background:#fff;position:sticky;top:0}.log-sql{word-wrap:break-word;white-space:normal!important}.list{-webkit-padding-start:0;list-style:none}.schema-wrapper{overflow:hidden}.toggle{cursor:pointer}td.name.indented{padding-left:30px}.stats-expand{cursor:pointer}.stats-th .counter{border:0 solid white}.table>thead>tr>th.preview-header{white-space:nowrap;border:0 solid white}div.sort{cursor:pointer}#schema_frame{width:100%;border:0}.schema-header{cursor:pointer}.counter{background-color:#ecf0f1;font-family:monospace}.sql{width:33%}.query_favorite_toggle{cursor:pointer}.query_favourite_detail{float:right}.btn-save-only{border-radius:0!important}.vite-not-running-canary{display:none}nav.navbar .nav-link{color:#fff}nav.navbar nav.nav-link:hover,nav.navbar .nav-link:focus{color:var(--bs-primary-bg-subtle)}nav.navbar .nav-pills .nav-link.active,nav.navbar .nav-pills .show>.nav-link{color:var(--bs-nav-pills-link-active-color);border:1px solid var(--bs-secondary-bg);background:none}nav.navbar .nav-link:hover,nav.navbar .navbar-brand:hover{background:none;color:var(--bs-primary-bg-subtle)!important}.dropdown-toggle:after{margin-left:0!important}#assistant_description_label{white-space:pre-wrap}#assistant_response pre{position:relative;background:#faebd7}#assistant_response .copy-btn{position:absolute;top:5px;right:5px;cursor:pointer}#additional_table_container{overflow-y:auto;max-height:120px}#assistant_input_parent{max-height:120px;overflow:hidden}#response_block:after{content:"";position:absolute;top:-20px;right:10px;border-width:10px;border-style:solid;border-color:transparent transparent var(--bs-border-color) transparent}
```

### Comparing `django_sql_explorer-4.2/explorer/tasks.py` & `django_sql_explorer-4.2b1/explorer/tasks.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/telemetry.py` & `django_sql_explorer-4.2b1/explorer/telemetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from django.conf import settings
 
 logger = logging.getLogger(__name__)
 
 
 def instance_identifier():
     from explorer.models import ExplorerValue
-    key = "explorer_instance_uuid"
+    key = "explorer_instance_identifier"
     r = cache.get(key)
     if not r:
         r = ExplorerValue.objects.get_uuid()
         cache.set(key, r, 60 * 60 * 24)
     return r
```

### Comparing `django_sql_explorer-4.2/explorer/templates/explorer/assistant.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/assistant.html`

 * *Files 26% similar despite different names*

```diff
@@ -6,41 +6,47 @@
                 <label for="id_assistant_input">SQL Assistant</label>
             </button>
         </div>
     </div>
     <div id="assistant_collapse" class="accordion-collapse collapse" aria-labelledby="assistant_accordion_header" data-bs-parent="#assistant_accordion">
         <div class="accordion-body">
             <div class="row assistant_input_parent">
-                <div class="mt-3 col-8" id="assistant_input_wrapper">
+                <div class="mt-3 col-12" id="assistant_input_wrapper">
                     <textarea
                         class="form-control mb-4" id="id_assistant_input"
-                        name="sql_assistant" rows="5" placeholder="What do you need help with?"></textarea>
+                        name="sql_assistant" rows="3" placeholder="What do you need help with?"></textarea>
                     <label for="id_assistant_input" class="form-label d-none" id="id_assistant_input_label">Assistant prompt</label>
                     <div id="id_error_help_message" class="d-none text-secondary small">
                         Hit "Ask Assistant" to try and fix the issue. The assistant is automatically aware of error messages & context.
                     </div>
                 </div>
-                <div id="additional_table_container" class="col-4">
+                <div id="additional_table_container" class="d-none col-3">
                     <input id="search_assistant_tables" class="search" placeholder="{% trans "Search Tables" %}" />
-                    <a class="small text-secondary" style="cursor: pointer; text-decoration: none;"
-                        data-bs-toggle="tooltip" data-bs-placement="top"
-                        data-bs-title="SQL Assistant builds a prompt with your query, your request, relevant schema (tables referenced in your query) and sample data from those tables. You can optionally include other tables (schema + data sample) that you'd like SQL Assistant to know about.">(?)</a>
                     <label for="search_assistant_tables" class="d-none" id="search_assistant_tables_label">Search tables</label>
                     <div id="table-list" class="list"></div>
                 </div>
             </div>
 
             <div class="row">
-                <div class="col-12 text-center">
+                <div class="col-6">
+                    <div class="form-check form-check-inline">
+                        <input type="checkbox" class="form-check-input" name="assistant-include-other-tables" id="include_other_tables" autocomplete="off">
+                        <label class="form-check-label" for="include_other_tables">Include Other Tables (<a class="small text-secondary" style="cursor: pointer;"
+                            data-bs-toggle="tooltip" data-bs-placement="top"
+                            data-bs-title="SQL Assistant builds a prompt with your query, your request, relevant schema (tables referenced in your query) and sample data from those tables. You can optionally include other tables (schema + data sample) that you'd like SQL Assistant to know about.">?</a>)</label>
+                    </div>
+                </div>
+                <div class="col-6 text-end">
                     <div class="btn-group" role="group">
                         <button type="button" class="btn btn-outline-primary" id="ask_assistant_btn">Ask Assistant</button>
                     </div>
                 </div>
             </div>
 
+
             <div id="response_block" class="position-relative d-none">
                 <div class="mt-3 p-2 pt-4 rounded-2 border bg-light">
                     <div id="assistant_response"></div>
                     <p class="spinner-border text-primary d-none" id="assistant_spinner" role="status">
                         <span class="visually-hidden">Loading...</span>
                     </p>
                 </div>
```

### Comparing `django_sql_explorer-4.2/explorer/templates/explorer/base.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/base.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/templates/explorer/export_buttons.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/export_buttons.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/templates/explorer/fullscreen.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/fullscreen.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/templates/explorer/params.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/params.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/templates/explorer/pdf_template.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/pdf_template.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/templates/explorer/play.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/play.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/templates/explorer/preview_pane.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/preview_pane.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/templates/explorer/query.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/query.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/templates/explorer/query_confirm_delete.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/query_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/templates/explorer/query_favorites.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/query_favorites.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/templates/explorer/query_list.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/query_list.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/templates/explorer/querylog_list.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/querylog_list.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/templates/explorer/schema.html` & `django_sql_explorer-4.2b1/explorer/templates/explorer/schema.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/templatetags/explorer_tags.py` & `django_sql_explorer-4.2b1/explorer/templatetags/explorer_tags.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/templatetags/vite.py` & `django_sql_explorer-4.2b1/explorer/templatetags/vite.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/tests/factories.py` & `django_sql_explorer-4.2b1/explorer/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/tests/settings.py` & `django_sql_explorer-4.2b1/explorer/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/tests/test_actions.py` & `django_sql_explorer-4.2b1/explorer/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/tests/test_apps.py` & `django_sql_explorer-4.2b1/explorer/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/tests/test_csrf_cookie_name.py` & `django_sql_explorer-4.2b1/explorer/tests/test_csrf_cookie_name.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/tests/test_exporters.py` & `django_sql_explorer-4.2b1/explorer/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/tests/test_forms.py` & `django_sql_explorer-4.2b1/explorer/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/tests/test_models.py` & `django_sql_explorer-4.2b1/explorer/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/tests/test_schema.py` & `django_sql_explorer-4.2b1/explorer/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/tests/test_tasks.py` & `django_sql_explorer-4.2b1/explorer/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/tests/test_telemetry.py` & `django_sql_explorer-4.2b1/explorer/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/tests/test_utils.py` & `django_sql_explorer-4.2b1/explorer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/tests/test_views.py` & `django_sql_explorer-4.2b1/explorer/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/urls.py` & `django_sql_explorer-4.2b1/explorer/urls.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/utils.py` & `django_sql_explorer-4.2b1/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/views/__init__.py` & `django_sql_explorer-4.2b1/explorer/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/views/auth.py` & `django_sql_explorer-4.2b1/explorer/views/auth.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/views/create.py` & `django_sql_explorer-4.2b1/explorer/views/create.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/views/download.py` & `django_sql_explorer-4.2b1/explorer/views/download.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/views/email.py` & `django_sql_explorer-4.2b1/explorer/views/email.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/views/export.py` & `django_sql_explorer-4.2b1/explorer/views/export.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/views/list.py` & `django_sql_explorer-4.2b1/explorer/views/list.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/views/mixins.py` & `django_sql_explorer-4.2b1/explorer/views/mixins.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/views/query.py` & `django_sql_explorer-4.2b1/explorer/views/query.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/views/query_favorite.py` & `django_sql_explorer-4.2b1/explorer/views/query_favorite.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/views/schema.py` & `django_sql_explorer-4.2b1/explorer/views/schema.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/views/stream.py` & `django_sql_explorer-4.2b1/explorer/views/stream.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/explorer/views/utils.py` & `django_sql_explorer-4.2b1/explorer/views/utils.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/package.json` & `django_sql_explorer-4.2b1/package.json`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/setup.cfg` & `django_sql_explorer-4.2b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/setup.py` & `django_sql_explorer-4.2b1/setup.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.2/vite.config.js` & `django_sql_explorer-4.2b1/vite.config.js`

 * *Files identical despite different names*

