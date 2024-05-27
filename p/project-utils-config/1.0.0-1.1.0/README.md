# Comparing `tmp/project-utils-config-1.0.0.tar.gz` & `tmp/project-utils-config-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project-utils-config-1.0.0.tar", last modified: Mon May 20 06:07:55 2024, max compression
+gzip compressed data, was "project-utils-config-1.1.0.tar", last modified: Mon May 27 03:22:28 2024, max compression
```

## Comparing `project-utils-config-1.0.0.tar` & `project-utils-config-1.1.0.tar`

### file list

```diff
@@ -1,147 +1,150 @@
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.019765 project-utils-config-1.0.0/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 07:03:44.000000 project-utils-config-1.0.0/LICENSE
--rw-r--r--   0 mylx2014   (501) staff       (20)     1666 2024-05-20 06:07:55.019591 project-utils-config-1.0.0/PKG-INFO
--rw-r--r--   0 mylx2014   (501) staff       (20)     1289 2023-11-24 01:16:34.000000 project-utils-config-1.0.0/README.md
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.974422 project-utils-config-1.0.0/project_utils/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.0.0/project_utils/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.975186 project-utils-config-1.0.0/project_utils/collection/
--rw-r--r--   0 mylx2014   (501) staff       (20)      140 2023-10-14 01:51:03.000000 project-utils-config-1.0.0/project_utils/collection/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      596 2023-10-13 02:35:45.000000 project-utils-config-1.0.0/project_utils/collection/list_util.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.975918 project-utils-config-1.0.0/project_utils/conf/
--rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 01:51:03.000000 project-utils-config-1.0.0/project_utils/conf/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.979605 project-utils-config-1.0.0/project_utils/conf/addr_config/
--rw-r--r--   0 mylx2014   (501) staff       (20)      652 2023-10-14 01:51:03.000000 project-utils-config-1.0.0/project_utils/conf/addr_config/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      739 2023-11-24 01:16:34.000000 project-utils-config-1.0.0/project_utils/conf/addr_config/base_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)       86 2023-10-14 01:51:03.000000 project-utils-config-1.0.0/project_utils/conf/addr_config/hbase_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      777 2023-10-14 01:51:03.000000 project-utils-config-1.0.0/project_utils/conf/addr_config/kafka_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      695 2023-10-14 01:51:03.000000 project-utils-config-1.0.0/project_utils/conf/addr_config/mysql_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1703 2024-05-20 06:02:43.000000 project-utils-config-1.0.0/project_utils/conf/addr_config/redis_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1039 2023-10-14 01:51:03.000000 project-utils-config-1.0.0/project_utils/conf/base_config.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.980218 project-utils-config-1.0.0/project_utils/conf/path_config/
--rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 01:51:03.000000 project-utils-config-1.0.0/project_utils/conf/path_config/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      970 2023-10-13 02:35:45.000000 project-utils-config-1.0.0/project_utils/conf/path_config/path_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1977 2023-10-14 01:51:03.000000 project-utils-config-1.0.0/project_utils/conf/template.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.980445 project-utils-config-1.0.0/project_utils/db/
--rw-r--r--   0 mylx2014   (501) staff       (20)      164 2023-10-14 01:57:29.000000 project-utils-config-1.0.0/project_utils/db/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.984858 project-utils-config-1.0.0/project_utils/db/mysql/
--rw-r--r--   0 mylx2014   (501) staff       (20)      257 2023-10-14 01:57:29.000000 project-utils-config-1.0.0/project_utils/db/mysql/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3484 2023-11-28 08:48:43.000000 project-utils-config-1.0.0/project_utils/db/mysql/_collection.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2291 2023-12-15 01:39:50.000000 project-utils-config-1.0.0/project_utils/db/mysql/_pool.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      832 2023-11-24 01:16:34.000000 project-utils-config-1.0.0/project_utils/db/mysql/_result.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      107 2023-10-13 02:35:45.000000 project-utils-config-1.0.0/project_utils/db/mysql/_types.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.985883 project-utils-config-1.0.0/project_utils/exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      811 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      148 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/exception/collection_exception.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      144 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/exception/config_exception.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.986356 project-utils-config-1.0.0/project_utils/exception/db_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      141 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/exception/db_exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      118 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/exception/db_exception/mysql_exception.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      507 2023-10-13 02:35:45.000000 project-utils-config-1.0.0/project_utils/exception/my_base_exception.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.986632 project-utils-config-1.0.0/project_utils/exception/web_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/exception/web_exception/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.987232 project-utils-config-1.0.0/project_utils/exception/web_exception/django_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      125 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/exception/web_exception/django_exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      127 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/exception/web_exception/django_exception/model_exception.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.987766 project-utils-config-1.0.0/project_utils/exception/web_exception/django_exception/view_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      275 2023-10-18 02:20:38.000000 project-utils-config-1.0.0/project_utils/exception/web_exception/django_exception/view_exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      120 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/exception/web_exception/django_exception/view_exception/response_exception.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1255 2023-10-13 02:35:45.000000 project-utils-config-1.0.0/project_utils/io.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.991892 project-utils-config-1.0.0/project_utils/os/
--rw-r--r--   0 mylx2014   (501) staff       (20)       98 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/os/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      760 2023-10-13 02:35:45.000000 project-utils-config-1.0.0/project_utils/os/dir.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2029 2024-01-16 07:43:03.000000 project-utils-config-1.0.0/project_utils/time.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.992221 project-utils-config-1.0.0/project_utils/web/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.0.0/project_utils/web/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.992374 project-utils-config-1.0.0/project_utils/web/aiohttp/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.0.0/project_utils/web/aiohttp/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.992761 project-utils-config-1.0.0/project_utils/web/django/
--rw-r--r--   0 mylx2014   (501) staff       (20)      463 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/web/django/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.993277 project-utils-config-1.0.0/project_utils/web/django/celery/
--rw-r--r--   0 mylx2014   (501) staff       (20)       84 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/web/django/celery/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.993927 project-utils-config-1.0.0/project_utils/web/django/celery/_conf/
--rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/web/django/celery/_conf/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1061 2023-11-24 01:16:34.000000 project-utils-config-1.0.0/project_utils/web/django/celery/_conf/_celery_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      334 2023-10-18 01:14:46.000000 project-utils-config-1.0.0/project_utils/web/django/celery/create_app.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.994587 project-utils-config-1.0.0/project_utils/web/django/conf/
--rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/web/django/conf/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2145 2023-11-24 01:16:34.000000 project-utils-config-1.0.0/project_utils/web/django/conf/_django_config.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.996581 project-utils-config-1.0.0/project_utils/web/django/middle/
--rw-r--r--   0 mylx2014   (501) staff       (20)      124 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/web/django/middle/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1161 2023-11-24 01:16:34.000000 project-utils-config-1.0.0/project_utils/web/django/middle/_base_middle.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.997974 project-utils-config-1.0.0/project_utils/web/django/model/
--rw-r--r--   0 mylx2014   (501) staff       (20)      434 2024-01-15 14:04:29.000000 project-utils-config-1.0.0/project_utils/web/django/model/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      106 2023-12-10 05:49:34.000000 project-utils-config-1.0.0/project_utils/web/django/model/_base_meta.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1511 2024-01-15 14:04:29.000000 project-utils-config-1.0.0/project_utils/web/django/model/_base_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      487 2023-12-08 06:57:16.000000 project-utils-config-1.0.0/project_utils/web/django/model/_id_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      461 2024-01-15 14:04:29.000000 project-utils-config-1.0.0/project_utils/web/django/model/_model_type.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.998392 project-utils-config-1.0.0/project_utils/web/django/pagination/
--rw-r--r--   0 mylx2014   (501) staff       (20)      197 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/web/django/pagination/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1011 2023-11-24 01:16:34.000000 project-utils-config-1.0.0/project_utils/web/django/pagination/_base_pagination.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:54.998816 project-utils-config-1.0.0/project_utils/web/django/request/
--rw-r--r--   0 mylx2014   (501) staff       (20)      102 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/web/django/request/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1379 2023-11-24 01:16:34.000000 project-utils-config-1.0.0/project_utils/web/django/request/_request.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.002685 project-utils-config-1.0.0/project_utils/web/django/response/
--rw-r--r--   0 mylx2014   (501) staff       (20)      153 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/web/django/response/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1291 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/web/django/response/_response_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      213 2023-11-24 01:16:34.000000 project-utils-config-1.0.0/project_utils/web/django/response/_response_types.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.003328 project-utils-config-1.0.0/project_utils/web/django/serializer/
--rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/web/django/serializer/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      284 2023-10-13 02:35:45.000000 project-utils-config-1.0.0/project_utils/web/django/serializer/_base_meta.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      418 2023-10-14 02:37:02.000000 project-utils-config-1.0.0/project_utils/web/django/serializer/_base_serializer.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.003838 project-utils-config-1.0.0/project_utils/web/django/swagger/
--rw-r--r--   0 mylx2014   (501) staff       (20)      499 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.007748 project-utils-config-1.0.0/project_utils/web/django/swagger/_params/
--rw-r--r--   0 mylx2014   (501) staff       (20)      675 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/_params/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/_params/_base.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1025 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/_params/_form.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1164 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/_params/_params.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      978 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/_params/_query.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2065 2023-12-10 07:17:18.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/_params/_response.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      412 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/_params/_types.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      268 2023-12-10 07:15:26.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/_urls.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.008499 project-utils-config-1.0.0/project_utils/web/django/swagger/config/
--rw-r--r--   0 mylx2014   (501) staff       (20)       69 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/config/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      488 2023-12-10 07:15:01.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/config/_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1274 2023-12-10 07:15:01.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/config/_swagger.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.009212 project-utils-config-1.0.0/project_utils/web/django/swagger/document/
--rw-r--r--   0 mylx2014   (501) staff       (20)      256 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/document/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1169 2023-12-10 07:15:01.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/document/_document.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      273 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/swagger/document/_types.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      678 2023-11-24 01:16:34.000000 project-utils-config-1.0.0/project_utils/web/django/utils.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.010711 project-utils-config-1.0.0/project_utils/web/django/view/
--rw-r--r--   0 mylx2014   (501) staff       (20)      478 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/view/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/view/_async_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2086 2023-12-10 15:11:23.000000 project-utils-config-1.0.0/project_utils/web/django/view/_base.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.011460 project-utils-config-1.0.0/project_utils/web/django/view/_base_api/
--rw-r--r--   0 mylx2014   (501) staff       (20)       57 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/view/_base_api/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3277 2023-12-10 15:07:50.000000 project-utils-config-1.0.0/project_utils/web/django/view/_base_api/api.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      908 2023-12-10 15:07:50.000000 project-utils-config-1.0.0/project_utils/web/django/view/_base_api/api_util.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.012550 project-utils-config-1.0.0/project_utils/web/django/view/_rest_api/
--rw-r--r--   0 mylx2014   (501) staff       (20)      296 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/view/_rest_api/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1921 2023-12-10 15:07:50.000000 project-utils-config-1.0.0/project_utils/web/django/view/_rest_api/api.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      480 2023-12-10 15:08:55.000000 project-utils-config-1.0.0/project_utils/web/django/view/_rest_api/api_utils.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2020 2023-12-10 15:08:55.000000 project-utils-config-1.0.0/project_utils/web/django/view/_rest_api/async_api.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.016689 project-utils-config-1.0.0/project_utils/web/django/view/_rest_view/
--rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/view/_rest_view/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)    12607 2023-12-10 15:16:37.000000 project-utils-config-1.0.0/project_utils/web/django/view/_rest_view/_async_base_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 15:11:23.000000 project-utils-config-1.0.0/project_utils/web/django/view/_rest_view/_async_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)    12432 2023-12-10 15:11:23.000000 project-utils-config-1.0.0/project_utils/web/django/view/_rest_view/_base_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 15:11:23.000000 project-utils-config-1.0.0/project_utils/web/django/view/_rest_view/_swagger_base.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 07:27:29.000000 project-utils-config-1.0.0/project_utils/web/django/view/_swagger_base.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      750 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/view/_types.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.018005 project-utils-config-1.0.0/project_utils/web/django/view/_user_view/
--rw-r--r--   0 mylx2014   (501) staff       (20)      185 2023-12-10 07:02:32.000000 project-utils-config-1.0.0/project_utils/web/django/view/_user_view/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      239 2023-12-10 15:11:23.000000 project-utils-config-1.0.0/project_utils/web/django/view/_user_view/_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)    11333 2023-12-10 15:11:23.000000 project-utils-config-1.0.0/project_utils/web/django/view/_user_view/_view.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.018370 project-utils-config-1.0.0/project_utils/web/fastapi/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.0.0/project_utils/web/fastapi/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.018522 project-utils-config-1.0.0/project_utils/web/flask/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.0.0/project_utils/web/flask/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-20 06:07:55.019371 project-utils-config-1.0.0/project_utils_config.egg-info/
--rw-r--r--   0 mylx2014   (501) staff       (20)     1666 2024-05-20 06:07:54.000000 project-utils-config-1.0.0/project_utils_config.egg-info/PKG-INFO
--rw-r--r--   0 mylx2014   (501) staff       (20)     4832 2024-05-20 06:07:54.000000 project-utils-config-1.0.0/project_utils_config.egg-info/SOURCES.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)        1 2024-05-20 06:07:54.000000 project-utils-config-1.0.0/project_utils_config.egg-info/dependency_links.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)       31 2024-05-20 06:07:54.000000 project-utils-config-1.0.0/project_utils_config.egg-info/requires.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)       14 2024-05-20 06:07:54.000000 project-utils-config-1.0.0/project_utils_config.egg-info/top_level.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)       38 2024-05-20 06:07:55.019806 project-utils-config-1.0.0/setup.cfg
--rw-r--r--   0 mylx2014   (501) staff       (20)      733 2024-05-20 06:06:22.000000 project-utils-config-1.0.0/setup.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.443342 project-utils-config-1.1.0/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 07:03:44.000000 project-utils-config-1.1.0/LICENSE
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1666 2024-05-27 03:22:28.443194 project-utils-config-1.1.0/PKG-INFO
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1289 2023-11-24 01:16:34.000000 project-utils-config-1.1.0/README.md
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.425085 project-utils-config-1.1.0/project_utils/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.0/project_utils/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.425636 project-utils-config-1.1.0/project_utils/collection/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      140 2023-10-14 01:51:03.000000 project-utils-config-1.1.0/project_utils/collection/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      596 2023-10-13 02:35:45.000000 project-utils-config-1.1.0/project_utils/collection/list_util.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.426337 project-utils-config-1.1.0/project_utils/conf/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 01:51:03.000000 project-utils-config-1.1.0/project_utils/conf/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.427453 project-utils-config-1.1.0/project_utils/conf/addr_config/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      652 2023-10-14 01:51:03.000000 project-utils-config-1.1.0/project_utils/conf/addr_config/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      739 2023-11-24 01:16:34.000000 project-utils-config-1.1.0/project_utils/conf/addr_config/base_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)       86 2023-10-14 01:51:03.000000 project-utils-config-1.1.0/project_utils/conf/addr_config/hbase_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      777 2023-10-14 01:51:03.000000 project-utils-config-1.1.0/project_utils/conf/addr_config/kafka_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      695 2023-10-14 01:51:03.000000 project-utils-config-1.1.0/project_utils/conf/addr_config/mysql_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1703 2024-05-20 06:02:43.000000 project-utils-config-1.1.0/project_utils/conf/addr_config/redis_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1039 2023-10-14 01:51:03.000000 project-utils-config-1.1.0/project_utils/conf/base_config.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.427832 project-utils-config-1.1.0/project_utils/conf/path_config/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 01:51:03.000000 project-utils-config-1.1.0/project_utils/conf/path_config/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      970 2023-10-13 02:35:45.000000 project-utils-config-1.1.0/project_utils/conf/path_config/path_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1977 2023-10-14 01:51:03.000000 project-utils-config-1.1.0/project_utils/conf/template.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.427991 project-utils-config-1.1.0/project_utils/db/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      164 2023-10-14 01:57:29.000000 project-utils-config-1.1.0/project_utils/db/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.429337 project-utils-config-1.1.0/project_utils/db/mysql/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      257 2023-10-14 01:57:29.000000 project-utils-config-1.1.0/project_utils/db/mysql/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3484 2023-11-28 08:48:43.000000 project-utils-config-1.1.0/project_utils/db/mysql/_collection.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2291 2023-12-15 01:39:50.000000 project-utils-config-1.1.0/project_utils/db/mysql/_pool.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      832 2023-11-24 01:16:34.000000 project-utils-config-1.1.0/project_utils/db/mysql/_result.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      107 2023-10-13 02:35:45.000000 project-utils-config-1.1.0/project_utils/db/mysql/_types.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.430030 project-utils-config-1.1.0/project_utils/exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      811 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      148 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/exception/collection_exception.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      144 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/exception/config_exception.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.430293 project-utils-config-1.1.0/project_utils/exception/db_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      141 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/exception/db_exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      118 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/exception/db_exception/mysql_exception.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      507 2023-10-13 02:35:45.000000 project-utils-config-1.1.0/project_utils/exception/my_base_exception.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.430442 project-utils-config-1.1.0/project_utils/exception/web_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/exception/web_exception/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.430707 project-utils-config-1.1.0/project_utils/exception/web_exception/django_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      125 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/exception/web_exception/django_exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      127 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/exception/web_exception/django_exception/model_exception.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.430989 project-utils-config-1.1.0/project_utils/exception/web_exception/django_exception/view_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      275 2023-10-18 02:20:38.000000 project-utils-config-1.1.0/project_utils/exception/web_exception/django_exception/view_exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      120 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/exception/web_exception/django_exception/view_exception/response_exception.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1255 2023-10-13 02:35:45.000000 project-utils-config-1.1.0/project_utils/io.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.431390 project-utils-config-1.1.0/project_utils/os/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       98 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/os/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      788 2024-05-20 06:29:51.000000 project-utils-config-1.1.0/project_utils/os/dir.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.431865 project-utils-config-1.1.0/project_utils/scripts/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       61 2024-05-27 03:21:01.000000 project-utils-config-1.1.0/project_utils/scripts/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      648 2024-05-27 03:21:01.000000 project-utils-config-1.1.0/project_utils/scripts/_base.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2029 2024-01-16 07:43:03.000000 project-utils-config-1.1.0/project_utils/time.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.432063 project-utils-config-1.1.0/project_utils/web/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.0/project_utils/web/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.432176 project-utils-config-1.1.0/project_utils/web/aiohttp/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.0/project_utils/web/aiohttp/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.432448 project-utils-config-1.1.0/project_utils/web/django/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      463 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/web/django/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.432882 project-utils-config-1.1.0/project_utils/web/django/celery/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       84 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/web/django/celery/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.433259 project-utils-config-1.1.0/project_utils/web/django/celery/_conf/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/web/django/celery/_conf/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1061 2023-11-24 01:16:34.000000 project-utils-config-1.1.0/project_utils/web/django/celery/_conf/_celery_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      334 2023-10-18 01:14:46.000000 project-utils-config-1.1.0/project_utils/web/django/celery/create_app.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.433639 project-utils-config-1.1.0/project_utils/web/django/conf/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/web/django/conf/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2145 2023-11-24 01:16:34.000000 project-utils-config-1.1.0/project_utils/web/django/conf/_django_config.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.434002 project-utils-config-1.1.0/project_utils/web/django/middle/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      124 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/web/django/middle/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1161 2023-11-24 01:16:34.000000 project-utils-config-1.1.0/project_utils/web/django/middle/_base_middle.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.435219 project-utils-config-1.1.0/project_utils/web/django/model/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      434 2024-01-15 14:04:29.000000 project-utils-config-1.1.0/project_utils/web/django/model/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      106 2023-12-10 05:49:34.000000 project-utils-config-1.1.0/project_utils/web/django/model/_base_meta.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1511 2024-01-15 14:04:29.000000 project-utils-config-1.1.0/project_utils/web/django/model/_base_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      487 2023-12-08 06:57:16.000000 project-utils-config-1.1.0/project_utils/web/django/model/_id_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      461 2024-01-15 14:04:29.000000 project-utils-config-1.1.0/project_utils/web/django/model/_model_type.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.435566 project-utils-config-1.1.0/project_utils/web/django/pagination/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      197 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/web/django/pagination/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1011 2023-11-24 01:16:34.000000 project-utils-config-1.1.0/project_utils/web/django/pagination/_base_pagination.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.436151 project-utils-config-1.1.0/project_utils/web/django/request/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      102 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/web/django/request/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1379 2023-11-24 01:16:34.000000 project-utils-config-1.1.0/project_utils/web/django/request/_request.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.436865 project-utils-config-1.1.0/project_utils/web/django/response/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      153 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/web/django/response/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1291 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/web/django/response/_response_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      213 2023-11-24 01:16:34.000000 project-utils-config-1.1.0/project_utils/web/django/response/_response_types.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.437304 project-utils-config-1.1.0/project_utils/web/django/serializer/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/web/django/serializer/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      284 2023-10-13 02:35:45.000000 project-utils-config-1.1.0/project_utils/web/django/serializer/_base_meta.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      418 2023-10-14 02:37:02.000000 project-utils-config-1.1.0/project_utils/web/django/serializer/_base_serializer.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.437658 project-utils-config-1.1.0/project_utils/web/django/swagger/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      499 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.438680 project-utils-config-1.1.0/project_utils/web/django/swagger/_params/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      675 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/_params/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/_params/_base.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1025 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/_params/_form.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1164 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/_params/_params.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      978 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/_params/_query.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2065 2023-12-10 07:17:18.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/_params/_response.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      412 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/_params/_types.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      268 2023-12-10 07:15:26.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/_urls.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.439098 project-utils-config-1.1.0/project_utils/web/django/swagger/config/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       69 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/config/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      488 2023-12-10 07:15:01.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/config/_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1274 2023-12-10 07:15:01.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/config/_swagger.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.439503 project-utils-config-1.1.0/project_utils/web/django/swagger/document/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      256 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/document/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1169 2023-12-10 07:15:01.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/document/_document.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      273 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/swagger/document/_types.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      678 2023-11-24 01:16:34.000000 project-utils-config-1.1.0/project_utils/web/django/utils.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.440159 project-utils-config-1.1.0/project_utils/web/django/view/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      478 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/view/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/view/_async_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2086 2023-12-10 15:11:23.000000 project-utils-config-1.1.0/project_utils/web/django/view/_base.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.440554 project-utils-config-1.1.0/project_utils/web/django/view/_base_api/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       57 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/view/_base_api/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3277 2023-12-10 15:07:50.000000 project-utils-config-1.1.0/project_utils/web/django/view/_base_api/api.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      908 2023-12-10 15:07:50.000000 project-utils-config-1.1.0/project_utils/web/django/view/_base_api/api_util.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.441062 project-utils-config-1.1.0/project_utils/web/django/view/_rest_api/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      296 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/view/_rest_api/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1921 2023-12-10 15:07:50.000000 project-utils-config-1.1.0/project_utils/web/django/view/_rest_api/api.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      480 2023-12-10 15:08:55.000000 project-utils-config-1.1.0/project_utils/web/django/view/_rest_api/api_utils.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2020 2023-12-10 15:08:55.000000 project-utils-config-1.1.0/project_utils/web/django/view/_rest_api/async_api.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.441887 project-utils-config-1.1.0/project_utils/web/django/view/_rest_view/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/view/_rest_view/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)    12607 2023-12-10 15:16:37.000000 project-utils-config-1.1.0/project_utils/web/django/view/_rest_view/_async_base_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 15:11:23.000000 project-utils-config-1.1.0/project_utils/web/django/view/_rest_view/_async_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)    12432 2023-12-10 15:11:23.000000 project-utils-config-1.1.0/project_utils/web/django/view/_rest_view/_base_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 15:11:23.000000 project-utils-config-1.1.0/project_utils/web/django/view/_rest_view/_swagger_base.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 07:27:29.000000 project-utils-config-1.1.0/project_utils/web/django/view/_swagger_base.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      750 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/view/_types.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.442265 project-utils-config-1.1.0/project_utils/web/django/view/_user_view/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      185 2023-12-10 07:02:32.000000 project-utils-config-1.1.0/project_utils/web/django/view/_user_view/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      239 2023-12-10 15:11:23.000000 project-utils-config-1.1.0/project_utils/web/django/view/_user_view/_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)    11333 2023-12-10 15:11:23.000000 project-utils-config-1.1.0/project_utils/web/django/view/_user_view/_view.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.442485 project-utils-config-1.1.0/project_utils/web/fastapi/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.0/project_utils/web/fastapi/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.442562 project-utils-config-1.1.0/project_utils/web/flask/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.0/project_utils/web/flask/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:22:28.443029 project-utils-config-1.1.0/project_utils_config.egg-info/
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1666 2024-05-27 03:22:28.000000 project-utils-config-1.1.0/project_utils_config.egg-info/PKG-INFO
+-rw-r--r--   0 mylx2014   (501) staff       (20)     4897 2024-05-27 03:22:28.000000 project-utils-config-1.1.0/project_utils_config.egg-info/SOURCES.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)        1 2024-05-27 03:22:28.000000 project-utils-config-1.1.0/project_utils_config.egg-info/dependency_links.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)       31 2024-05-27 03:22:28.000000 project-utils-config-1.1.0/project_utils_config.egg-info/requires.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)       14 2024-05-27 03:22:28.000000 project-utils-config-1.1.0/project_utils_config.egg-info/top_level.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)       38 2024-05-27 03:22:28.443374 project-utils-config-1.1.0/setup.cfg
+-rw-r--r--   0 mylx2014   (501) staff       (20)      733 2024-05-27 03:22:22.000000 project-utils-config-1.1.0/setup.py
```

### Comparing `project-utils-config-1.0.0/PKG-INFO` & `project-utils-config-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-utils-config
-Version: 1.0.0
+Version: 1.1.0
 Summary: python project_utils tools
 Home-page: https://gitee.com/mylx2014/project-utils.git
 Author: mylx2014
 Author-email: mylx2014@163.com
 License: MIT
 Keywords: python,utils,project utils,aiofiles
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `project-utils-config-1.0.0/README.md` & `project-utils-config-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/collection/list_util.py` & `project-utils-config-1.1.0/project_utils/collection/list_util.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/conf/addr_config/__init__.py` & `project-utils-config-1.1.0/project_utils/conf/addr_config/__init__.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/conf/addr_config/base_config.py` & `project-utils-config-1.1.0/project_utils/conf/addr_config/base_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/conf/addr_config/kafka_config.py` & `project-utils-config-1.1.0/project_utils/conf/addr_config/kafka_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/conf/addr_config/mysql_config.py` & `project-utils-config-1.1.0/project_utils/conf/addr_config/mysql_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/conf/addr_config/redis_config.py` & `project-utils-config-1.1.0/project_utils/conf/addr_config/redis_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/conf/base_config.py` & `project-utils-config-1.1.0/project_utils/conf/base_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/conf/path_config/path_config.py` & `project-utils-config-1.1.0/project_utils/conf/path_config/path_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/conf/template.py` & `project-utils-config-1.1.0/project_utils/conf/template.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/db/mysql/_collection.py` & `project-utils-config-1.1.0/project_utils/db/mysql/_collection.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/db/mysql/_pool.py` & `project-utils-config-1.1.0/project_utils/db/mysql/_pool.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/db/mysql/_result.py` & `project-utils-config-1.1.0/project_utils/db/mysql/_result.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/exception/__init__.py` & `project-utils-config-1.1.0/project_utils/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/io.py` & `project-utils-config-1.1.0/project_utils/io.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/os/dir.py` & `project-utils-config-1.1.0/project_utils/os/dir.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 ﻿import os
 
+from pathlib import Path
+
 
 def mkdir(path: str) -> bool:
     try:
         os.mkdir(path)
     except:
         return False
     else:
```

### Comparing `project-utils-config-1.0.0/project_utils/time.py` & `project-utils-config-1.1.0/project_utils/time.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/celery/_conf/_celery_config.py` & `project-utils-config-1.1.0/project_utils/web/django/celery/_conf/_celery_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/conf/_django_config.py` & `project-utils-config-1.1.0/project_utils/web/django/conf/_django_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/middle/_base_middle.py` & `project-utils-config-1.1.0/project_utils/web/django/middle/_base_middle.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/model/_base_model.py` & `project-utils-config-1.1.0/project_utils/web/django/model/_base_model.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/pagination/_base_pagination.py` & `project-utils-config-1.1.0/project_utils/web/django/pagination/_base_pagination.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/request/_request.py` & `project-utils-config-1.1.0/project_utils/web/django/request/_request.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/response/_response_model.py` & `project-utils-config-1.1.0/project_utils/web/django/response/_response_model.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/swagger/_params/__init__.py` & `project-utils-config-1.1.0/project_utils/web/django/swagger/_params/__init__.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/swagger/_params/_form.py` & `project-utils-config-1.1.0/project_utils/web/django/swagger/_params/_form.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/swagger/_params/_params.py` & `project-utils-config-1.1.0/project_utils/web/django/swagger/_params/_params.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/swagger/_params/_query.py` & `project-utils-config-1.1.0/project_utils/web/django/swagger/_params/_query.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/swagger/_params/_response.py` & `project-utils-config-1.1.0/project_utils/web/django/swagger/_params/_response.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/swagger/config/_swagger.py` & `project-utils-config-1.1.0/project_utils/web/django/swagger/config/_swagger.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/swagger/document/_document.py` & `project-utils-config-1.1.0/project_utils/web/django/swagger/document/_document.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/utils.py` & `project-utils-config-1.1.0/project_utils/web/django/utils.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/view/_async_view.py` & `project-utils-config-1.1.0/project_utils/web/django/view/_async_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/view/_base.py` & `project-utils-config-1.1.0/project_utils/web/django/view/_base.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/view/_base_api/api.py` & `project-utils-config-1.1.0/project_utils/web/django/view/_base_api/api.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/view/_base_api/api_util.py` & `project-utils-config-1.1.0/project_utils/web/django/view/_base_api/api_util.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/view/_rest_api/api.py` & `project-utils-config-1.1.0/project_utils/web/django/view/_rest_api/api.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/view/_rest_api/async_api.py` & `project-utils-config-1.1.0/project_utils/web/django/view/_rest_api/async_api.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/view/_rest_view/_async_base_view.py` & `project-utils-config-1.1.0/project_utils/web/django/view/_rest_view/_async_base_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/view/_rest_view/_async_view.py` & `project-utils-config-1.1.0/project_utils/web/django/view/_rest_view/_async_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/view/_rest_view/_base_view.py` & `project-utils-config-1.1.0/project_utils/web/django/view/_rest_view/_base_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/view/_rest_view/_swagger_base.py` & `project-utils-config-1.1.0/project_utils/web/django/view/_rest_view/_swagger_base.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/view/_swagger_base.py` & `project-utils-config-1.1.0/project_utils/web/django/view/_swagger_base.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/view/_types.py` & `project-utils-config-1.1.0/project_utils/web/django/view/_types.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils/web/django/view/_user_view/_view.py` & `project-utils-config-1.1.0/project_utils/web/django/view/_user_view/_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.0.0/project_utils_config.egg-info/PKG-INFO` & `project-utils-config-1.1.0/project_utils_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-utils-config
-Version: 1.0.0
+Version: 1.1.0
 Summary: python project_utils tools
 Home-page: https://gitee.com/mylx2014/project-utils.git
 Author: mylx2014
 Author-email: mylx2014@163.com
 License: MIT
 Keywords: python,utils,project utils,aiofiles
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `project-utils-config-1.0.0/project_utils_config.egg-info/SOURCES.txt` & `project-utils-config-1.1.0/project_utils_config.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 project_utils/exception/web_exception/__init__.py
 project_utils/exception/web_exception/django_exception/__init__.py
 project_utils/exception/web_exception/django_exception/model_exception.py
 project_utils/exception/web_exception/django_exception/view_exception/__init__.py
 project_utils/exception/web_exception/django_exception/view_exception/response_exception.py
 project_utils/os/__init__.py
 project_utils/os/dir.py
+project_utils/scripts/__init__.py
+project_utils/scripts/_base.py
 project_utils/web/__init__.py
 project_utils/web/aiohttp/__init__.py
 project_utils/web/django/__init__.py
 project_utils/web/django/utils.py
 project_utils/web/django/celery/__init__.py
 project_utils/web/django/celery/create_app.py
 project_utils/web/django/celery/_conf/__init__.py
```

### Comparing `project-utils-config-1.0.0/setup.py` & `project-utils-config-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.0.0"
+VERSION = "1.1.0"
 DESCRIPTION = "python project_utils tools"
 setup(
     name="project-utils-config",
     version=VERSION,
     author="mylx2014",
     author_email="mylx2014@163.com",
     description=DESCRIPTION,
```

