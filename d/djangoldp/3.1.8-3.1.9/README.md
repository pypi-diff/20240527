# Comparing `tmp/djangoldp-3.1.8.tar.gz` & `tmp/djangoldp-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp-3.1.8.tar", last modified: Wed Jan 24 20:12:02 2024, max compression
+gzip compressed data, was "djangoldp-3.1.9.tar", last modified: Fri Jan 26 12:45:36 2024, max compression
```

## Comparing `djangoldp-3.1.8.tar` & `djangoldp-3.1.9.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.397447 djangoldp-3.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-01-24 20:11:35.000000 djangoldp-3.1.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-01-24 20:11:35.000000 djangoldp-3.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      322 2024-01-24 20:12:02.397447 djangoldp-3.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3664 2024-01-24 20:11:35.000000 djangoldp-3.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.373446 djangoldp-3.1.8/djangoldp/
--rw-rw-rw-   0 root         (0) root         (0)      401 2024-01-24 20:11:54.000000 djangoldp-3.1.8/djangoldp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.377446 djangoldp-3.1.8/djangoldp/activities/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/activities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/activities/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     5050 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/activities/objects.py
--rw-rw-rw-   0 root         (0) root         (0)    31027 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/activities/services.py
--rw-rw-rw-   0 root         (0) root         (0)     3584 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/activities/verbs.py
--rw-rw-rw-   0 root         (0) root         (0)     2631 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     5144 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/check_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     4622 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.377446 djangoldp-3.1.8/djangoldp/conf/
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5287 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/default_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     5272 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/ldpsettings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.377446 djangoldp-3.1.8/djangoldp/conf/package_template/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/package_template/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.381446 djangoldp-3.1.8/djangoldp/conf/package_template/app_name/
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/package_template/app_name/__init__.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/package_template/app_name/admin.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/package_template/app_name/apps.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      262 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/package_template/app_name/djangoldp_settings.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      179 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/package_template/app_name/djangoldp_urls.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/package_template/app_name/models.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/package_template/app_name/tests.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/package_template/app_name/views.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      374 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/package_template/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/package_template/setup.py-tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.381446 djangoldp-3.1.8/djangoldp/conf/server_template/
--rwxrwxrwx   0 root         (0) root         (0)      816 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/server_template/manage.py-tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.381446 djangoldp-3.1.8/djangoldp/conf/server_template/server/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/server_template/server/__init__.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      996 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/server_template/server/urls.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      598 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/server_template/server/wsgi.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      368 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/conf/server_template/settings.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.381446 djangoldp-3.1.8/djangoldp/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3043 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/endpoints/webfinger.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     5249 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.381446 djangoldp-3.1.8/djangoldp/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.381446 djangoldp-3.1.8/djangoldp/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/management/commands/check_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/management/commands/configure.py
--rw-rw-rw-   0 root         (0) root         (0)     2524 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/management/commands/federate.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/management/commands/mock_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1440 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.385446 djangoldp-3.1.8/djangoldp/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0002_auto_20190906_0642.py
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0003_auto_20190911_0931.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0004_auto_20200221_1118.py
--rw-rw-rw-   0 root         (0) root         (0)      491 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0005_auto_20200221_1127.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0006_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0007_auto_20200429_1346.py
--rw-rw-rw-   0 root         (0) root         (0)      765 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0008_auto_20200501_1207.py
--rw-rw-rw-   0 root         (0) root         (0)      601 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0009_auto_20200505_1733.py
--rw-rw-rw-   0 root         (0) root         (0)     1176 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0010_follower.py
--rw-rw-rw-   0 root         (0) root         (0)     1024 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0011_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)      992 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0012_auto_20200617_1817.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0013_auto_20200624_1709.py
--rw-rw-rw-   0 root         (0) root         (0)     3177 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0014_auto_20200909_2206.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0015_auto_20210125_1847.py
--rw-rw-rw-   0 root         (0) root         (0)      950 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0016_alter_activity_options_alter_follower_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      894 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0017_alter_activity_urlid_alter_follower_urlid_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/0018_alter_activity_payload_alter_activity_response_body.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14415 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1188 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)    17174 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/related.py
--rw-rw-rw-   0 root         (0) root         (0)    40132 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.385446 djangoldp-3.1.8/djangoldp/templates/
--rw-rw-rw-   0 root         (0) root         (0)      895 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/templates/swagger-ui.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.393447 djangoldp-3.1.8/djangoldp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/djangoldp_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.393447 djangoldp-3.1.8/djangoldp/tests/dummy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/dummy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/dummy/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/dummy/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)    15314 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)      778 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/performance_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     1716 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1220 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.393447 djangoldp-3.1.8/djangoldp/tests/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2209 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/scripts/prod_data_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     1324 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/scripts/test_data_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     5102 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/scripts/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      770 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/server_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1528 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_anonymous_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_auto_author.py
--rw-rw-rw-   0 root         (0) root         (0)    18371 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_backlinks_service.py
--rw-rw-rw-   0 root         (0) root         (0)    14537 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_cache.py
--rw-rw-rw-   0 root         (0) root         (0)      610 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_delete.py
--rw-rw-rw-   0 root         (0) root         (0)    13228 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_get.py
--rw-rw-rw-   0 root         (0) root         (0)     7813 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_guardian.py
--rw-rw-rw-   0 root         (0) root         (0)    29323 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_inbox.py
--rw-rw-rw-   0 root         (0) root         (0)     2056 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_ldp_model.py
--rw-rw-rw-   0 root         (0) root         (0)     5943 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_ldp_viewset.py
--rw-rw-rw-   0 root         (0) root         (0)    36663 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_model_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     5943 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_perf_get.py
--rw-rw-rw-   0 root         (0) root         (0)     1625 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_performance.py
--rw-rw-rw-   0 root         (0) root         (0)    10601 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)    12193 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_post.py
--rw-rw-rw-   0 root         (0) root         (0)     2031 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_sources.py
--rw-rw-rw-   0 root         (0) root         (0)    28899 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_update.py
--rw-rw-rw-   0 root         (0) root         (0)    22303 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/tests/tests_user_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     3294 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    27038 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.373446 djangoldp-3.1.8/djangoldp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      322 2024-01-24 20:12:02.000000 djangoldp-3.1.8/djangoldp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4584 2024-01-24 20:12:02.000000 djangoldp-3.1.8/djangoldp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-24 20:12:02.000000 djangoldp-3.1.8/djangoldp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-01-24 20:12:02.000000 djangoldp-3.1.8/djangoldp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-24 20:12:02.000000 djangoldp-3.1.8/djangoldp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      303 2024-01-24 20:12:02.000000 djangoldp-3.1.8/djangoldp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-01-24 20:12:02.000000 djangoldp-3.1.8/djangoldp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.393447 djangoldp-3.1.8/djangoldp_crypto/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp_crypto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      331 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp_crypto/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.393447 djangoldp-3.1.8/djangoldp_crypto/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp_crypto/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.397447 djangoldp-3.1.8/djangoldp_crypto/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp_crypto/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp_crypto/management/commands/creatersakey.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 20:12:02.397447 djangoldp-3.1.8/djangoldp_crypto/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      685 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp_crypto/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp_crypto/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-01-24 20:11:35.000000 djangoldp-3.1.8/djangoldp_crypto/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1012 2024-01-24 20:12:02.397447 djangoldp-3.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-01-24 20:11:35.000000 djangoldp-3.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.470735 djangoldp-3.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-01-26 12:45:11.000000 djangoldp-3.1.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-01-26 12:45:11.000000 djangoldp-3.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      322 2024-01-26 12:45:36.470735 djangoldp-3.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3664 2024-01-26 12:45:11.000000 djangoldp-3.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.454734 djangoldp-3.1.9/djangoldp/
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-01-26 12:45:28.000000 djangoldp-3.1.9/djangoldp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.458734 djangoldp-3.1.9/djangoldp/activities/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/activities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/activities/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5050 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/activities/objects.py
+-rw-rw-rw-   0 root         (0) root         (0)    31027 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/activities/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/activities/verbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     5144 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/check_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     4622 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.458734 djangoldp-3.1.9/djangoldp/conf/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5287 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/default_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/ldpsettings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.458734 djangoldp-3.1.9/djangoldp/conf/package_template/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/package_template/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.458734 djangoldp-3.1.9/djangoldp/conf/package_template/app_name/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/package_template/app_name/__init__.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/package_template/app_name/admin.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/package_template/app_name/apps.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      262 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/package_template/app_name/djangoldp_settings.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/package_template/app_name/djangoldp_urls.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/package_template/app_name/models.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/package_template/app_name/tests.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/package_template/app_name/views.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      374 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/package_template/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/package_template/setup.py-tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.458734 djangoldp-3.1.9/djangoldp/conf/server_template/
+-rwxrwxrwx   0 root         (0) root         (0)      816 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/server_template/manage.py-tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.458734 djangoldp-3.1.9/djangoldp/conf/server_template/server/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/server_template/server/__init__.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      996 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/server_template/server/urls.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      598 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/server_template/server/wsgi.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      368 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/conf/server_template/settings.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.458734 djangoldp-3.1.9/djangoldp/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/endpoints/webfinger.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     5249 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.458734 djangoldp-3.1.9/djangoldp/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.458734 djangoldp-3.1.9/djangoldp/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/management/commands/check_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/management/commands/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     2524 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/management/commands/federate.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/management/commands/mock_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1440 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.462735 djangoldp-3.1.9/djangoldp/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0002_auto_20190906_0642.py
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0003_auto_20190911_0931.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0004_auto_20200221_1118.py
+-rw-rw-rw-   0 root         (0) root         (0)      491 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0005_auto_20200221_1127.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0006_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0007_auto_20200429_1346.py
+-rw-rw-rw-   0 root         (0) root         (0)      765 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0008_auto_20200501_1207.py
+-rw-rw-rw-   0 root         (0) root         (0)      601 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0009_auto_20200505_1733.py
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0010_follower.py
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0011_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)      992 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0012_auto_20200617_1817.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0013_auto_20200624_1709.py
+-rw-rw-rw-   0 root         (0) root         (0)     3177 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0014_auto_20200909_2206.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0015_auto_20210125_1847.py
+-rw-rw-rw-   0 root         (0) root         (0)      950 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0016_alter_activity_options_alter_follower_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      894 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0017_alter_activity_urlid_alter_follower_urlid_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/0018_alter_activity_payload_alter_activity_response_body.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14415 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1188 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)    17174 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/related.py
+-rw-rw-rw-   0 root         (0) root         (0)    40092 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.462735 djangoldp-3.1.9/djangoldp/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      895 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/templates/swagger-ui.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.466735 djangoldp-3.1.9/djangoldp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/djangoldp_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.466735 djangoldp-3.1.9/djangoldp/tests/dummy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/dummy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/dummy/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/dummy/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)    15314 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      778 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/performance_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1716 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1220 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.466735 djangoldp-3.1.9/djangoldp/tests/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2209 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/scripts/prod_data_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1324 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/scripts/test_data_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5102 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/scripts/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      770 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/server_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1528 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_anonymous_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_auto_author.py
+-rw-rw-rw-   0 root         (0) root         (0)    18371 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_backlinks_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    14537 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      610 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    13228 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_get.py
+-rw-rw-rw-   0 root         (0) root         (0)     7783 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_guardian.py
+-rw-rw-rw-   0 root         (0) root         (0)    29323 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_inbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     2056 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_ldp_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     5943 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_ldp_viewset.py
+-rw-rw-rw-   0 root         (0) root         (0)    36663 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_model_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     5943 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_perf_get.py
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_performance.py
+-rw-rw-rw-   0 root         (0) root         (0)    10601 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12193 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_post.py
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_sources.py
+-rw-rw-rw-   0 root         (0) root         (0)    28899 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_update.py
+-rw-rw-rw-   0 root         (0) root         (0)    22177 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/tests/tests_user_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3294 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    27038 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.454734 djangoldp-3.1.9/djangoldp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      322 2024-01-26 12:45:36.000000 djangoldp-3.1.9/djangoldp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4584 2024-01-26 12:45:36.000000 djangoldp-3.1.9/djangoldp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-26 12:45:36.000000 djangoldp-3.1.9/djangoldp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-01-26 12:45:36.000000 djangoldp-3.1.9/djangoldp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-26 12:45:36.000000 djangoldp-3.1.9/djangoldp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      303 2024-01-26 12:45:36.000000 djangoldp-3.1.9/djangoldp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-01-26 12:45:36.000000 djangoldp-3.1.9/djangoldp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.466735 djangoldp-3.1.9/djangoldp_crypto/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp_crypto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp_crypto/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.466735 djangoldp-3.1.9/djangoldp_crypto/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp_crypto/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.470735 djangoldp-3.1.9/djangoldp_crypto/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp_crypto/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp_crypto/management/commands/creatersakey.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 12:45:36.470735 djangoldp-3.1.9/djangoldp_crypto/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      685 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp_crypto/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp_crypto/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-01-26 12:45:11.000000 djangoldp-3.1.9/djangoldp_crypto/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2024-01-26 12:45:36.470735 djangoldp-3.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-01-26 12:45:11.000000 djangoldp-3.1.9/setup.py
```

### Comparing `djangoldp-3.1.8/LICENSE` & `djangoldp-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/README.md` & `djangoldp-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/activities/objects.py` & `djangoldp-3.1.9/djangoldp/activities/objects.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/activities/services.py` & `djangoldp-3.1.9/djangoldp/activities/services.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/activities/verbs.py` & `djangoldp-3.1.9/djangoldp/activities/verbs.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/admin.py` & `djangoldp-3.1.9/djangoldp/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/apps.py` & `djangoldp-3.1.9/djangoldp/apps.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/check_integrity.py` & `djangoldp-3.1.9/djangoldp/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/cli.py` & `djangoldp-3.1.9/djangoldp/cli.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/conf/default_settings.py` & `djangoldp-3.1.9/djangoldp/conf/default_settings.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/conf/ldpsettings.py` & `djangoldp-3.1.9/djangoldp/conf/ldpsettings.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/conf/server_template/manage.py-tpl` & `djangoldp-3.1.9/djangoldp/conf/server_template/manage.py-tpl`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/conf/server_template/server/urls.py-tpl` & `djangoldp-3.1.9/djangoldp/conf/server_template/server/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/conf/server_template/server/wsgi.py-tpl` & `djangoldp-3.1.9/djangoldp/conf/server_template/server/wsgi.py-tpl`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/endpoints/webfinger.py` & `djangoldp-3.1.9/djangoldp/endpoints/webfinger.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/filters.py` & `djangoldp-3.1.9/djangoldp/filters.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/management/commands/check_integrity.py` & `djangoldp-3.1.9/djangoldp/management/commands/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/management/commands/configure.py` & `djangoldp-3.1.9/djangoldp/management/commands/configure.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/management/commands/federate.py` & `djangoldp-3.1.9/djangoldp/management/commands/federate.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/middleware.py` & `djangoldp-3.1.9/djangoldp/middleware.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0001_initial.py` & `djangoldp-3.1.9/djangoldp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0002_auto_20190906_0642.py` & `djangoldp-3.1.9/djangoldp/migrations/0002_auto_20190906_0642.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0006_activity.py` & `djangoldp-3.1.9/djangoldp/migrations/0006_activity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0007_auto_20200429_1346.py` & `djangoldp-3.1.9/djangoldp/migrations/0007_auto_20200429_1346.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0008_auto_20200501_1207.py` & `djangoldp-3.1.9/djangoldp/migrations/0008_auto_20200501_1207.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0009_auto_20200505_1733.py` & `djangoldp-3.1.9/djangoldp/migrations/0009_auto_20200505_1733.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0010_follower.py` & `djangoldp-3.1.9/djangoldp/migrations/0010_follower.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0011_auto_20200610_1323.py` & `djangoldp-3.1.9/djangoldp/migrations/0011_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0012_auto_20200617_1817.py` & `djangoldp-3.1.9/djangoldp/migrations/0012_auto_20200617_1817.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0013_auto_20200624_1709.py` & `djangoldp-3.1.9/djangoldp/migrations/0013_auto_20200624_1709.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0014_auto_20200909_2206.py` & `djangoldp-3.1.9/djangoldp/migrations/0014_auto_20200909_2206.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0015_auto_20210125_1847.py` & `djangoldp-3.1.9/djangoldp/migrations/0015_auto_20210125_1847.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0016_alter_activity_options_alter_follower_options_and_more.py` & `djangoldp-3.1.9/djangoldp/migrations/0016_alter_activity_options_alter_follower_options_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0017_alter_activity_urlid_alter_follower_urlid_and_more.py` & `djangoldp-3.1.9/djangoldp/migrations/0017_alter_activity_urlid_alter_follower_urlid_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/migrations/0018_alter_activity_payload_alter_activity_response_body.py` & `djangoldp-3.1.9/djangoldp/migrations/0018_alter_activity_payload_alter_activity_response_body.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/models.py` & `djangoldp-3.1.9/djangoldp/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/pagination.py` & `djangoldp-3.1.9/djangoldp/pagination.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/permissions.py` & `djangoldp-3.1.9/djangoldp/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/related.py` & `djangoldp-3.1.9/djangoldp/related.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/serializers.py` & `djangoldp-3.1.9/djangoldp/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         if not permission_classes:
             return data
         # The permissions must be given by all permission classes to be granted
         permissions = set.intersection(*[permission().get_permissions(user, model, obj) for permission in permission_classes])
         # Don't grant delete permissions on containers
         if not obj and 'delete' in permissions:
             permissions.remove('delete')
-        data['permissions'] = [{'mode': {'@type': name}} for name in permissions]
+        data['permissions'] = permissions
         return data
     
     def serialize_rdf_fields(self, obj, data, include_context=False):
         '''adds the @type and the @context to the data'''
         rdf_type = getattr(obj._meta, 'rdf_type', None)
         rdf_context = getattr(obj._meta, 'rdf_context', None)
         if rdf_type:
```

### Comparing `djangoldp-3.1.8/djangoldp/templates/swagger-ui.html` & `djangoldp-3.1.9/djangoldp/templates/swagger-ui.html`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/djangoldp_urls.py` & `djangoldp-3.1.9/djangoldp/tests/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/models.py` & `djangoldp-3.1.9/djangoldp/tests/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/performance_runner.py` & `djangoldp-3.1.9/djangoldp/tests/performance_runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/permissions.py` & `djangoldp-3.1.9/djangoldp/tests/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/runner.py` & `djangoldp-3.1.9/djangoldp/tests/runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/scripts/prod_data_generator.py` & `djangoldp-3.1.9/djangoldp/tests/scripts/prod_data_generator.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/scripts/test_data_generator.py` & `djangoldp-3.1.9/djangoldp/tests/scripts/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/scripts/utils.py` & `djangoldp-3.1.9/djangoldp/tests/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/server_settings.py` & `djangoldp-3.1.9/djangoldp/tests/server_settings.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_anonymous_permissions.py` & `djangoldp-3.1.9/djangoldp/tests/tests_anonymous_permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_auto_author.py` & `djangoldp-3.1.9/djangoldp/tests/tests_auto_author.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_backlinks_service.py` & `djangoldp-3.1.9/djangoldp/tests/tests_backlinks_service.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_cache.py` & `djangoldp-3.1.9/djangoldp/tests/tests_cache.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_delete.py` & `djangoldp-3.1.9/djangoldp/tests/tests_delete.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_get.py` & `djangoldp-3.1.9/djangoldp/tests/tests_get.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_guardian.py` & `djangoldp-3.1.9/djangoldp/tests/tests_guardian.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     # optional setup for testing PermissionlessDummy model with parameterised perms
     def setUpGuardianDummyWithPerms(self, perms=None, parent=None, group=False):
         self.dummy = self._get_dummy_with_perms(perms, parent, group)
 
     # auxiliary function converts permission format for test
     def _unpack_permissions(self, perms_from_response):
-        return [p['mode']['@type'] for p in perms_from_response]
+        return perms_from_response
 
     # test that dummy with no permissions set returns no results
     def test_get_dummy_no_permissions(self):
         self.setUpLoggedInUser()
         self.setUpGuardianDummyWithPerms()
         response = self.client.get('/permissionless-dummys/{}/'.format(self.dummy.slug))
         self.assertEqual(response.status_code, 404)
```

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_inbox.py` & `djangoldp-3.1.9/djangoldp/tests/tests_inbox.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_ldp_model.py` & `djangoldp-3.1.9/djangoldp/tests/tests_ldp_model.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_ldp_viewset.py` & `djangoldp-3.1.9/djangoldp/tests/tests_ldp_viewset.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_model_serializer.py` & `djangoldp-3.1.9/djangoldp/tests/tests_model_serializer.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_pagination.py` & `djangoldp-3.1.9/djangoldp/tests/tests_pagination.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_perf_get.py` & `djangoldp-3.1.9/djangoldp/tests/tests_perf_get.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_performance.py` & `djangoldp-3.1.9/djangoldp/tests/tests_performance.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_permissions.py` & `djangoldp-3.1.9/djangoldp/tests/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_post.py` & `djangoldp-3.1.9/djangoldp/tests/tests_post.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_settings.py` & `djangoldp-3.1.9/djangoldp/tests/tests_settings.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_sources.py` & `djangoldp-3.1.9/djangoldp/tests/tests_sources.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_update.py` & `djangoldp-3.1.9/djangoldp/tests/tests_update.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/tests/tests_user_permissions.py` & `djangoldp-3.1.9/djangoldp/tests/tests_user_permissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,17 +29,17 @@
         self.user.save()
 
     # list - simple
     def test_get_for_authenticated_user(self):
         response = self.client.get('/job-offers/')
         self.assertEqual(response.status_code, 200)
         # test serialized permissions
-        self.assertIn({'mode': {'@type': 'view'}}, response.data['permissions'])
-        self.assertNotIn({'mode': {'@type': 'inherit'}}, response.data['permissions'])
-        # self.assertNotIn({'mode': {'@type': 'delete'}}, response.data['permissions'])
+        self.assertIn('view', response.data['permissions'])
+        self.assertNotIn('inherit', response.data['permissions'])
+        # self.assertNotIn('delete', response.data['permissions'])
 
     # TODO: list - I do not have permission from the model, but I do have permission via a Group I am assigned
     #  https://git.startinblox.com/djangoldp-packages/djangoldp/issues/291
     '''def test_group_list_access(self):
         self.setUpGroup()
         dummy = PermissionlessDummy.objects.create()
 
@@ -115,16 +115,16 @@
     # TODO: test for DELETE scenario   
     '''
 
     @override_settings(SERIALIZE_OBJECT_EXCLUDE_PERMISSIONS=['inherit'])
     def test_get_1_for_authenticated_user(self):
         response = self.client.get('/job-offers/{}/'.format(self.job.slug))
         self.assertEqual(response.status_code, 200)
-        self.assertIn({'mode': {'@type': 'view'}}, response.data['permissions'])
-        self.assertNotIn({'mode': {'@type': 'inherit'}}, response.data['permissions'])
+        self.assertIn('view', response.data['permissions'])
+        self.assertNotIn('inherit', response.data['permissions'])
 
     def test_post_request_for_authenticated_user(self):
         post = {'https://cdn.startinblox.com/owl#title': "job_created", "https://cdn.startinblox.com/owl#slug": 'slug2'}
         response = self.client.post('/job-offers/', data=json.dumps(post), content_type='application/ld+json')
         self.assertEqual(response.status_code, 201)
 
     # denied because I don't have model permissions
@@ -235,15 +235,15 @@
         my_resource = OwnedResource.objects.create(description='test', user=self.user)
         another_user = get_user_model().objects.create_user(username='test', email='test@test.com', password='test')
         their_resource = OwnedResource.objects.create(description='another test', user=another_user)
 
         response = self.client.get('/ownedresources/{}/'.format(my_resource.pk))
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.data['@id'], my_resource.urlid)
-        self.assertIn({'mode': {'@type': 'delete'}}, response.data['permissions'])
+        self.assertIn('delete', response.data['permissions'])
 
         # I have permission to view this resource
         response = self.client.patch('/ownedresources/{}/'.format(their_resource.pk))
         self.assertEqual(response.status_code, 404)
 
     def test_patch_owned_resource(self):
         my_profile = UserProfile.objects.create(user=self.user, slug=self.user.username, description='about me')
```

### Comparing `djangoldp-3.1.8/djangoldp/urls.py` & `djangoldp-3.1.9/djangoldp/urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/utils.py` & `djangoldp-3.1.9/djangoldp/utils.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp/views.py` & `djangoldp-3.1.9/djangoldp/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp.egg-info/SOURCES.txt` & `djangoldp-3.1.9/djangoldp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp_crypto/management/commands/creatersakey.py` & `djangoldp-3.1.9/djangoldp_crypto/management/commands/creatersakey.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp_crypto/migrations/0001_initial.py` & `djangoldp-3.1.9/djangoldp_crypto/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/djangoldp_crypto/models.py` & `djangoldp-3.1.9/djangoldp_crypto/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.1.8/setup.cfg` & `djangoldp-3.1.9/setup.cfg`

 * *Files identical despite different names*

