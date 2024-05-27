# Comparing `tmp/project-utils-config-1.1.1.tar.gz` & `tmp/project-utils-config-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project-utils-config-1.1.1.tar", last modified: Mon May 27 03:33:12 2024, max compression
+gzip compressed data, was "project-utils-config-1.1.2.tar", last modified: Mon May 27 03:55:45 2024, max compression
```

## Comparing `project-utils-config-1.1.1.tar` & `project-utils-config-1.1.2.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.628331 project-utils-config-1.1.1/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 07:03:44.000000 project-utils-config-1.1.1/LICENSE
--rw-r--r--   0 mylx2014   (501) staff       (20)     1666 2024-05-27 03:33:12.628192 project-utils-config-1.1.1/PKG-INFO
--rw-r--r--   0 mylx2014   (501) staff       (20)     1289 2023-11-24 01:16:34.000000 project-utils-config-1.1.1/README.md
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.607548 project-utils-config-1.1.1/project_utils/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.1/project_utils/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.608144 project-utils-config-1.1.1/project_utils/collection/
--rw-r--r--   0 mylx2014   (501) staff       (20)      140 2023-10-14 01:51:03.000000 project-utils-config-1.1.1/project_utils/collection/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      596 2023-10-13 02:35:45.000000 project-utils-config-1.1.1/project_utils/collection/list_util.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.609814 project-utils-config-1.1.1/project_utils/conf/
--rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 01:51:03.000000 project-utils-config-1.1.1/project_utils/conf/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.612399 project-utils-config-1.1.1/project_utils/conf/addr_config/
--rw-r--r--   0 mylx2014   (501) staff       (20)      652 2023-10-14 01:51:03.000000 project-utils-config-1.1.1/project_utils/conf/addr_config/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      739 2023-11-24 01:16:34.000000 project-utils-config-1.1.1/project_utils/conf/addr_config/base_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)       86 2023-10-14 01:51:03.000000 project-utils-config-1.1.1/project_utils/conf/addr_config/hbase_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      777 2023-10-14 01:51:03.000000 project-utils-config-1.1.1/project_utils/conf/addr_config/kafka_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      695 2023-10-14 01:51:03.000000 project-utils-config-1.1.1/project_utils/conf/addr_config/mysql_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1703 2024-05-20 06:02:43.000000 project-utils-config-1.1.1/project_utils/conf/addr_config/redis_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1039 2023-10-14 01:51:03.000000 project-utils-config-1.1.1/project_utils/conf/base_config.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.613214 project-utils-config-1.1.1/project_utils/conf/path_config/
--rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 01:51:03.000000 project-utils-config-1.1.1/project_utils/conf/path_config/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      970 2023-10-13 02:35:45.000000 project-utils-config-1.1.1/project_utils/conf/path_config/path_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2285 2024-05-27 03:33:05.000000 project-utils-config-1.1.1/project_utils/conf/template.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.613717 project-utils-config-1.1.1/project_utils/db/
--rw-r--r--   0 mylx2014   (501) staff       (20)      164 2023-10-14 01:57:29.000000 project-utils-config-1.1.1/project_utils/db/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.614889 project-utils-config-1.1.1/project_utils/db/mysql/
--rw-r--r--   0 mylx2014   (501) staff       (20)      257 2023-10-14 01:57:29.000000 project-utils-config-1.1.1/project_utils/db/mysql/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3484 2023-11-28 08:48:43.000000 project-utils-config-1.1.1/project_utils/db/mysql/_collection.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2291 2023-12-15 01:39:50.000000 project-utils-config-1.1.1/project_utils/db/mysql/_pool.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      832 2023-11-24 01:16:34.000000 project-utils-config-1.1.1/project_utils/db/mysql/_result.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      107 2023-10-13 02:35:45.000000 project-utils-config-1.1.1/project_utils/db/mysql/_types.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.615496 project-utils-config-1.1.1/project_utils/exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      811 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      148 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/exception/collection_exception.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      144 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/exception/config_exception.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.615757 project-utils-config-1.1.1/project_utils/exception/db_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      141 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/exception/db_exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      118 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/exception/db_exception/mysql_exception.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      507 2023-10-13 02:35:45.000000 project-utils-config-1.1.1/project_utils/exception/my_base_exception.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.615894 project-utils-config-1.1.1/project_utils/exception/web_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/exception/web_exception/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.616147 project-utils-config-1.1.1/project_utils/exception/web_exception/django_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      125 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/exception/web_exception/django_exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      127 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/exception/web_exception/django_exception/model_exception.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.616471 project-utils-config-1.1.1/project_utils/exception/web_exception/django_exception/view_exception/
--rw-r--r--   0 mylx2014   (501) staff       (20)      275 2023-10-18 02:20:38.000000 project-utils-config-1.1.1/project_utils/exception/web_exception/django_exception/view_exception/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      120 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/exception/web_exception/django_exception/view_exception/response_exception.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1255 2024-05-27 03:30:53.000000 project-utils-config-1.1.1/project_utils/io.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.616850 project-utils-config-1.1.1/project_utils/os/
--rw-r--r--   0 mylx2014   (501) staff       (20)       98 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/os/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      788 2024-05-20 06:29:51.000000 project-utils-config-1.1.1/project_utils/os/dir.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.617358 project-utils-config-1.1.1/project_utils/scripts/
--rw-r--r--   0 mylx2014   (501) staff       (20)       61 2024-05-27 03:21:01.000000 project-utils-config-1.1.1/project_utils/scripts/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      648 2024-05-27 03:21:01.000000 project-utils-config-1.1.1/project_utils/scripts/_base.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2029 2024-01-16 07:43:03.000000 project-utils-config-1.1.1/project_utils/time.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.617546 project-utils-config-1.1.1/project_utils/web/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.1/project_utils/web/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.617652 project-utils-config-1.1.1/project_utils/web/aiohttp/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.1/project_utils/web/aiohttp/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.617910 project-utils-config-1.1.1/project_utils/web/django/
--rw-r--r--   0 mylx2014   (501) staff       (20)      463 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/web/django/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.618317 project-utils-config-1.1.1/project_utils/web/django/celery/
--rw-r--r--   0 mylx2014   (501) staff       (20)       84 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/web/django/celery/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.618673 project-utils-config-1.1.1/project_utils/web/django/celery/_conf/
--rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/web/django/celery/_conf/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1061 2023-11-24 01:16:34.000000 project-utils-config-1.1.1/project_utils/web/django/celery/_conf/_celery_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      334 2023-10-18 01:14:46.000000 project-utils-config-1.1.1/project_utils/web/django/celery/create_app.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.619125 project-utils-config-1.1.1/project_utils/web/django/conf/
--rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/web/django/conf/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2145 2023-11-24 01:16:34.000000 project-utils-config-1.1.1/project_utils/web/django/conf/_django_config.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.619512 project-utils-config-1.1.1/project_utils/web/django/middle/
--rw-r--r--   0 mylx2014   (501) staff       (20)      124 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/web/django/middle/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1161 2023-11-24 01:16:34.000000 project-utils-config-1.1.1/project_utils/web/django/middle/_base_middle.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.620241 project-utils-config-1.1.1/project_utils/web/django/model/
--rw-r--r--   0 mylx2014   (501) staff       (20)      434 2024-01-15 14:04:29.000000 project-utils-config-1.1.1/project_utils/web/django/model/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      106 2023-12-10 05:49:34.000000 project-utils-config-1.1.1/project_utils/web/django/model/_base_meta.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1511 2024-01-15 14:04:29.000000 project-utils-config-1.1.1/project_utils/web/django/model/_base_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      487 2023-12-08 06:57:16.000000 project-utils-config-1.1.1/project_utils/web/django/model/_id_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      461 2024-01-15 14:04:29.000000 project-utils-config-1.1.1/project_utils/web/django/model/_model_type.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.620578 project-utils-config-1.1.1/project_utils/web/django/pagination/
--rw-r--r--   0 mylx2014   (501) staff       (20)      197 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/web/django/pagination/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1011 2023-11-24 01:16:34.000000 project-utils-config-1.1.1/project_utils/web/django/pagination/_base_pagination.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.620927 project-utils-config-1.1.1/project_utils/web/django/request/
--rw-r--r--   0 mylx2014   (501) staff       (20)      102 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/web/django/request/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1379 2023-11-24 01:16:34.000000 project-utils-config-1.1.1/project_utils/web/django/request/_request.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.621424 project-utils-config-1.1.1/project_utils/web/django/response/
--rw-r--r--   0 mylx2014   (501) staff       (20)      153 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/web/django/response/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1291 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/web/django/response/_response_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      213 2023-11-24 01:16:34.000000 project-utils-config-1.1.1/project_utils/web/django/response/_response_types.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.621812 project-utils-config-1.1.1/project_utils/web/django/serializer/
--rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/web/django/serializer/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      284 2023-10-13 02:35:45.000000 project-utils-config-1.1.1/project_utils/web/django/serializer/_base_meta.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      418 2023-10-14 02:37:02.000000 project-utils-config-1.1.1/project_utils/web/django/serializer/_base_serializer.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.622089 project-utils-config-1.1.1/project_utils/web/django/swagger/
--rw-r--r--   0 mylx2014   (501) staff       (20)      499 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.623337 project-utils-config-1.1.1/project_utils/web/django/swagger/_params/
--rw-r--r--   0 mylx2014   (501) staff       (20)      675 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/_params/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/_params/_base.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1025 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/_params/_form.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1164 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/_params/_params.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      978 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/_params/_query.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2065 2023-12-10 07:17:18.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/_params/_response.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      412 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/_params/_types.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      268 2023-12-10 07:15:26.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/_urls.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.623720 project-utils-config-1.1.1/project_utils/web/django/swagger/config/
--rw-r--r--   0 mylx2014   (501) staff       (20)       69 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/config/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      488 2023-12-10 07:15:01.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/config/_config.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1274 2023-12-10 07:15:01.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/config/_swagger.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.624183 project-utils-config-1.1.1/project_utils/web/django/swagger/document/
--rw-r--r--   0 mylx2014   (501) staff       (20)      256 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/document/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1169 2023-12-10 07:15:01.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/document/_document.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      273 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/swagger/document/_types.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      678 2023-11-24 01:16:34.000000 project-utils-config-1.1.1/project_utils/web/django/utils.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.624921 project-utils-config-1.1.1/project_utils/web/django/view/
--rw-r--r--   0 mylx2014   (501) staff       (20)      478 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/view/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/view/_async_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2086 2023-12-10 15:11:23.000000 project-utils-config-1.1.1/project_utils/web/django/view/_base.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.625508 project-utils-config-1.1.1/project_utils/web/django/view/_base_api/
--rw-r--r--   0 mylx2014   (501) staff       (20)       57 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/view/_base_api/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3277 2023-12-10 15:07:50.000000 project-utils-config-1.1.1/project_utils/web/django/view/_base_api/api.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      908 2023-12-10 15:07:50.000000 project-utils-config-1.1.1/project_utils/web/django/view/_base_api/api_util.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.626000 project-utils-config-1.1.1/project_utils/web/django/view/_rest_api/
--rw-r--r--   0 mylx2014   (501) staff       (20)      296 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/view/_rest_api/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1921 2023-12-10 15:07:50.000000 project-utils-config-1.1.1/project_utils/web/django/view/_rest_api/api.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      480 2023-12-10 15:08:55.000000 project-utils-config-1.1.1/project_utils/web/django/view/_rest_api/api_utils.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     2020 2023-12-10 15:08:55.000000 project-utils-config-1.1.1/project_utils/web/django/view/_rest_api/async_api.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.626851 project-utils-config-1.1.1/project_utils/web/django/view/_rest_view/
--rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/view/_rest_view/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)    12607 2023-12-10 15:16:37.000000 project-utils-config-1.1.1/project_utils/web/django/view/_rest_view/_async_base_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 15:11:23.000000 project-utils-config-1.1.1/project_utils/web/django/view/_rest_view/_async_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)    12432 2023-12-10 15:11:23.000000 project-utils-config-1.1.1/project_utils/web/django/view/_rest_view/_base_view.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 15:11:23.000000 project-utils-config-1.1.1/project_utils/web/django/view/_rest_view/_swagger_base.py
--rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 07:27:29.000000 project-utils-config-1.1.1/project_utils/web/django/view/_swagger_base.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      750 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/view/_types.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.627260 project-utils-config-1.1.1/project_utils/web/django/view/_user_view/
--rw-r--r--   0 mylx2014   (501) staff       (20)      185 2023-12-10 07:02:32.000000 project-utils-config-1.1.1/project_utils/web/django/view/_user_view/__init__.py
--rw-r--r--   0 mylx2014   (501) staff       (20)      239 2023-12-10 15:11:23.000000 project-utils-config-1.1.1/project_utils/web/django/view/_user_view/_model.py
--rw-r--r--   0 mylx2014   (501) staff       (20)    11333 2023-12-10 15:11:23.000000 project-utils-config-1.1.1/project_utils/web/django/view/_user_view/_view.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.627474 project-utils-config-1.1.1/project_utils/web/fastapi/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.1/project_utils/web/fastapi/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.627549 project-utils-config-1.1.1/project_utils/web/flask/
--rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.1/project_utils/web/flask/__init__.py
-drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:33:12.628012 project-utils-config-1.1.1/project_utils_config.egg-info/
--rw-r--r--   0 mylx2014   (501) staff       (20)     1666 2024-05-27 03:33:12.000000 project-utils-config-1.1.1/project_utils_config.egg-info/PKG-INFO
--rw-r--r--   0 mylx2014   (501) staff       (20)     4897 2024-05-27 03:33:12.000000 project-utils-config-1.1.1/project_utils_config.egg-info/SOURCES.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)        1 2024-05-27 03:33:12.000000 project-utils-config-1.1.1/project_utils_config.egg-info/dependency_links.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)       31 2024-05-27 03:33:12.000000 project-utils-config-1.1.1/project_utils_config.egg-info/requires.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)       14 2024-05-27 03:33:12.000000 project-utils-config-1.1.1/project_utils_config.egg-info/top_level.txt
--rw-r--r--   0 mylx2014   (501) staff       (20)       38 2024-05-27 03:33:12.628361 project-utils-config-1.1.1/setup.cfg
--rw-r--r--   0 mylx2014   (501) staff       (20)      733 2024-05-27 03:33:05.000000 project-utils-config-1.1.1/setup.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.308678 project-utils-config-1.1.2/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 07:03:44.000000 project-utils-config-1.1.2/LICENSE
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1666 2024-05-27 03:55:45.308529 project-utils-config-1.1.2/PKG-INFO
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1289 2023-11-24 01:16:34.000000 project-utils-config-1.1.2/README.md
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.290226 project-utils-config-1.1.2/project_utils/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.2/project_utils/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.290840 project-utils-config-1.1.2/project_utils/collection/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      140 2023-10-14 01:51:03.000000 project-utils-config-1.1.2/project_utils/collection/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      596 2023-10-13 02:35:45.000000 project-utils-config-1.1.2/project_utils/collection/list_util.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.291503 project-utils-config-1.1.2/project_utils/conf/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 01:51:03.000000 project-utils-config-1.1.2/project_utils/conf/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.292766 project-utils-config-1.1.2/project_utils/conf/addr_config/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      652 2023-10-14 01:51:03.000000 project-utils-config-1.1.2/project_utils/conf/addr_config/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      739 2023-11-24 01:16:34.000000 project-utils-config-1.1.2/project_utils/conf/addr_config/base_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)       86 2023-10-14 01:51:03.000000 project-utils-config-1.1.2/project_utils/conf/addr_config/hbase_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      777 2023-10-14 01:51:03.000000 project-utils-config-1.1.2/project_utils/conf/addr_config/kafka_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      695 2023-10-14 01:51:03.000000 project-utils-config-1.1.2/project_utils/conf/addr_config/mysql_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1703 2024-05-20 06:02:43.000000 project-utils-config-1.1.2/project_utils/conf/addr_config/redis_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1039 2023-10-14 01:51:03.000000 project-utils-config-1.1.2/project_utils/conf/base_config.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.293136 project-utils-config-1.1.2/project_utils/conf/path_config/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 01:51:03.000000 project-utils-config-1.1.2/project_utils/conf/path_config/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      970 2023-10-13 02:35:45.000000 project-utils-config-1.1.2/project_utils/conf/path_config/path_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2285 2024-05-27 03:33:05.000000 project-utils-config-1.1.2/project_utils/conf/template.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.293274 project-utils-config-1.1.2/project_utils/db/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      164 2023-10-14 01:57:29.000000 project-utils-config-1.1.2/project_utils/db/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.294219 project-utils-config-1.1.2/project_utils/db/mysql/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      257 2023-10-14 01:57:29.000000 project-utils-config-1.1.2/project_utils/db/mysql/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3484 2023-11-28 08:48:43.000000 project-utils-config-1.1.2/project_utils/db/mysql/_collection.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2291 2023-12-15 01:39:50.000000 project-utils-config-1.1.2/project_utils/db/mysql/_pool.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      832 2023-11-24 01:16:34.000000 project-utils-config-1.1.2/project_utils/db/mysql/_result.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      107 2023-10-13 02:35:45.000000 project-utils-config-1.1.2/project_utils/db/mysql/_types.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.294851 project-utils-config-1.1.2/project_utils/exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      811 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      148 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/exception/collection_exception.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      144 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/exception/config_exception.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.295107 project-utils-config-1.1.2/project_utils/exception/db_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      141 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/exception/db_exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      118 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/exception/db_exception/mysql_exception.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      507 2023-10-13 02:35:45.000000 project-utils-config-1.1.2/project_utils/exception/my_base_exception.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.295231 project-utils-config-1.1.2/project_utils/exception/web_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/exception/web_exception/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.296862 project-utils-config-1.1.2/project_utils/exception/web_exception/django_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      125 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/exception/web_exception/django_exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      127 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/exception/web_exception/django_exception/model_exception.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.297113 project-utils-config-1.1.2/project_utils/exception/web_exception/django_exception/view_exception/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      275 2023-10-18 02:20:38.000000 project-utils-config-1.1.2/project_utils/exception/web_exception/django_exception/view_exception/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      120 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/exception/web_exception/django_exception/view_exception/response_exception.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1255 2024-05-27 03:30:53.000000 project-utils-config-1.1.2/project_utils/io.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.297460 project-utils-config-1.1.2/project_utils/os/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       98 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/os/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      788 2024-05-20 06:29:51.000000 project-utils-config-1.1.2/project_utils/os/dir.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.297864 project-utils-config-1.1.2/project_utils/scripts/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       61 2024-05-27 03:21:01.000000 project-utils-config-1.1.2/project_utils/scripts/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      642 2024-05-27 03:55:32.000000 project-utils-config-1.1.2/project_utils/scripts/_base.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2029 2024-01-16 07:43:03.000000 project-utils-config-1.1.2/project_utils/time.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.297959 project-utils-config-1.1.2/project_utils/web/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.2/project_utils/web/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.298039 project-utils-config-1.1.2/project_utils/web/aiohttp/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.2/project_utils/web/aiohttp/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.298253 project-utils-config-1.1.2/project_utils/web/django/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      463 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/web/django/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.298603 project-utils-config-1.1.2/project_utils/web/django/celery/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       84 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/web/django/celery/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.298943 project-utils-config-1.1.2/project_utils/web/django/celery/_conf/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      142 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/web/django/celery/_conf/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1061 2023-11-24 01:16:34.000000 project-utils-config-1.1.2/project_utils/web/django/celery/_conf/_celery_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      334 2023-10-18 01:14:46.000000 project-utils-config-1.1.2/project_utils/web/django/celery/create_app.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.299255 project-utils-config-1.1.2/project_utils/web/django/conf/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      155 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/web/django/conf/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2145 2023-11-24 01:16:34.000000 project-utils-config-1.1.2/project_utils/web/django/conf/_django_config.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.299635 project-utils-config-1.1.2/project_utils/web/django/middle/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      124 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/web/django/middle/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1161 2023-11-24 01:16:34.000000 project-utils-config-1.1.2/project_utils/web/django/middle/_base_middle.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.300401 project-utils-config-1.1.2/project_utils/web/django/model/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      434 2024-01-15 14:04:29.000000 project-utils-config-1.1.2/project_utils/web/django/model/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      106 2023-12-10 05:49:34.000000 project-utils-config-1.1.2/project_utils/web/django/model/_base_meta.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1511 2024-01-15 14:04:29.000000 project-utils-config-1.1.2/project_utils/web/django/model/_base_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      487 2023-12-08 06:57:16.000000 project-utils-config-1.1.2/project_utils/web/django/model/_id_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      461 2024-01-15 14:04:29.000000 project-utils-config-1.1.2/project_utils/web/django/model/_model_type.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.300707 project-utils-config-1.1.2/project_utils/web/django/pagination/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      197 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/web/django/pagination/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1011 2023-11-24 01:16:34.000000 project-utils-config-1.1.2/project_utils/web/django/pagination/_base_pagination.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.301029 project-utils-config-1.1.2/project_utils/web/django/request/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      102 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/web/django/request/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1379 2023-11-24 01:16:34.000000 project-utils-config-1.1.2/project_utils/web/django/request/_request.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.301556 project-utils-config-1.1.2/project_utils/web/django/response/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      153 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/web/django/response/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1291 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/web/django/response/_response_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      213 2023-11-24 01:16:34.000000 project-utils-config-1.1.2/project_utils/web/django/response/_response_types.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.302035 project-utils-config-1.1.2/project_utils/web/django/serializer/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      130 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/web/django/serializer/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      284 2023-10-13 02:35:45.000000 project-utils-config-1.1.2/project_utils/web/django/serializer/_base_meta.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      418 2023-10-14 02:37:02.000000 project-utils-config-1.1.2/project_utils/web/django/serializer/_base_serializer.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.302359 project-utils-config-1.1.2/project_utils/web/django/swagger/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      499 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.303576 project-utils-config-1.1.2/project_utils/web/django/swagger/_params/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      675 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/_params/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/_params/_base.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1025 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/_params/_form.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1164 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/_params/_params.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      978 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/_params/_query.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2065 2023-12-10 07:17:18.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/_params/_response.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      412 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/_params/_types.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      268 2023-12-10 07:15:26.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/_urls.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.304013 project-utils-config-1.1.2/project_utils/web/django/swagger/config/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       69 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/config/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      488 2023-12-10 07:15:01.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/config/_config.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1274 2023-12-10 07:15:01.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/config/_swagger.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.304498 project-utils-config-1.1.2/project_utils/web/django/swagger/document/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      256 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/document/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1169 2023-12-10 07:15:01.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/document/_document.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      273 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/swagger/document/_types.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      678 2023-11-24 01:16:34.000000 project-utils-config-1.1.2/project_utils/web/django/utils.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.305185 project-utils-config-1.1.2/project_utils/web/django/view/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      478 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/view/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/view/_async_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2086 2023-12-10 15:11:23.000000 project-utils-config-1.1.2/project_utils/web/django/view/_base.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.305586 project-utils-config-1.1.2/project_utils/web/django/view/_base_api/
+-rw-r--r--   0 mylx2014   (501) staff       (20)       57 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/view/_base_api/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3277 2023-12-10 15:07:50.000000 project-utils-config-1.1.2/project_utils/web/django/view/_base_api/api.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      908 2023-12-10 15:07:50.000000 project-utils-config-1.1.2/project_utils/web/django/view/_base_api/api_util.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.306154 project-utils-config-1.1.2/project_utils/web/django/view/_rest_api/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      296 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/view/_rest_api/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1921 2023-12-10 15:07:50.000000 project-utils-config-1.1.2/project_utils/web/django/view/_rest_api/api.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      480 2023-12-10 15:08:55.000000 project-utils-config-1.1.2/project_utils/web/django/view/_rest_api/api_utils.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     2020 2023-12-10 15:08:55.000000 project-utils-config-1.1.2/project_utils/web/django/view/_rest_api/async_api.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.307159 project-utils-config-1.1.2/project_utils/web/django/view/_rest_view/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      307 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/view/_rest_view/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)    12607 2023-12-10 15:16:37.000000 project-utils-config-1.1.2/project_utils/web/django/view/_rest_view/_async_base_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     3840 2023-12-10 15:11:23.000000 project-utils-config-1.1.2/project_utils/web/django/view/_rest_view/_async_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)    12432 2023-12-10 15:11:23.000000 project-utils-config-1.1.2/project_utils/web/django/view/_rest_view/_base_view.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 15:11:23.000000 project-utils-config-1.1.2/project_utils/web/django/view/_rest_view/_swagger_base.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1243 2023-12-10 07:27:29.000000 project-utils-config-1.1.2/project_utils/web/django/view/_swagger_base.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      750 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/view/_types.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.307543 project-utils-config-1.1.2/project_utils/web/django/view/_user_view/
+-rw-r--r--   0 mylx2014   (501) staff       (20)      185 2023-12-10 07:02:32.000000 project-utils-config-1.1.2/project_utils/web/django/view/_user_view/__init__.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)      239 2023-12-10 15:11:23.000000 project-utils-config-1.1.2/project_utils/web/django/view/_user_view/_model.py
+-rw-r--r--   0 mylx2014   (501) staff       (20)    11333 2023-12-10 15:11:23.000000 project-utils-config-1.1.2/project_utils/web/django/view/_user_view/_view.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.307756 project-utils-config-1.1.2/project_utils/web/fastapi/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.2/project_utils/web/fastapi/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.307838 project-utils-config-1.1.2/project_utils/web/flask/
+-rw-r--r--   0 mylx2014   (501) staff       (20)        0 2023-10-13 02:35:45.000000 project-utils-config-1.1.2/project_utils/web/flask/__init__.py
+drwxr-xr-x   0 mylx2014   (501) staff       (20)        0 2024-05-27 03:55:45.308338 project-utils-config-1.1.2/project_utils_config.egg-info/
+-rw-r--r--   0 mylx2014   (501) staff       (20)     1666 2024-05-27 03:55:45.000000 project-utils-config-1.1.2/project_utils_config.egg-info/PKG-INFO
+-rw-r--r--   0 mylx2014   (501) staff       (20)     4897 2024-05-27 03:55:45.000000 project-utils-config-1.1.2/project_utils_config.egg-info/SOURCES.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)        1 2024-05-27 03:55:45.000000 project-utils-config-1.1.2/project_utils_config.egg-info/dependency_links.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)       31 2024-05-27 03:55:45.000000 project-utils-config-1.1.2/project_utils_config.egg-info/requires.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)       14 2024-05-27 03:55:45.000000 project-utils-config-1.1.2/project_utils_config.egg-info/top_level.txt
+-rw-r--r--   0 mylx2014   (501) staff       (20)       38 2024-05-27 03:55:45.308710 project-utils-config-1.1.2/setup.cfg
+-rw-r--r--   0 mylx2014   (501) staff       (20)      733 2024-05-27 03:55:43.000000 project-utils-config-1.1.2/setup.py
```

### Comparing `project-utils-config-1.1.1/PKG-INFO` & `project-utils-config-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-utils-config
-Version: 1.1.1
+Version: 1.1.2
 Summary: python project_utils tools
 Home-page: https://gitee.com/mylx2014/project-utils.git
 Author: mylx2014
 Author-email: mylx2014@163.com
 License: MIT
 Keywords: python,utils,project utils,aiofiles
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `project-utils-config-1.1.1/README.md` & `project-utils-config-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/collection/list_util.py` & `project-utils-config-1.1.2/project_utils/collection/list_util.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/conf/addr_config/__init__.py` & `project-utils-config-1.1.2/project_utils/conf/addr_config/__init__.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/conf/addr_config/base_config.py` & `project-utils-config-1.1.2/project_utils/conf/addr_config/base_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/conf/addr_config/kafka_config.py` & `project-utils-config-1.1.2/project_utils/conf/addr_config/kafka_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/conf/addr_config/mysql_config.py` & `project-utils-config-1.1.2/project_utils/conf/addr_config/mysql_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/conf/addr_config/redis_config.py` & `project-utils-config-1.1.2/project_utils/conf/addr_config/redis_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/conf/base_config.py` & `project-utils-config-1.1.2/project_utils/conf/base_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/conf/path_config/path_config.py` & `project-utils-config-1.1.2/project_utils/conf/path_config/path_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/conf/template.py` & `project-utils-config-1.1.2/project_utils/conf/template.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/db/mysql/_collection.py` & `project-utils-config-1.1.2/project_utils/db/mysql/_collection.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/db/mysql/_pool.py` & `project-utils-config-1.1.2/project_utils/db/mysql/_pool.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/db/mysql/_result.py` & `project-utils-config-1.1.2/project_utils/db/mysql/_result.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/exception/__init__.py` & `project-utils-config-1.1.2/project_utils/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/io.py` & `project-utils-config-1.1.2/project_utils/io.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/os/dir.py` & `project-utils-config-1.1.2/project_utils/os/dir.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/scripts/_base.py` & `project-utils-config-1.1.2/project_utils/scripts/_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class BaseScript(metaclass=ABCMeta):
     config: ConfigTemplate
 
     def __init__(self, config: ConfigTemplate):
         self.config = config
         self.loop = asyncio.get_event_loop()
 
-    async def async_start(self, *args, **kwargs):
+    def async_start(self, *args, **kwargs):
         self.loop.run_until_complete(self.handler(*args, **kwargs))
 
     @abstractmethod
     async def handler(self, *args, **kwargs):
         ...
 
     @classmethod
```

### Comparing `project-utils-config-1.1.1/project_utils/time.py` & `project-utils-config-1.1.2/project_utils/time.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/celery/_conf/_celery_config.py` & `project-utils-config-1.1.2/project_utils/web/django/celery/_conf/_celery_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/conf/_django_config.py` & `project-utils-config-1.1.2/project_utils/web/django/conf/_django_config.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/middle/_base_middle.py` & `project-utils-config-1.1.2/project_utils/web/django/middle/_base_middle.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/model/_base_model.py` & `project-utils-config-1.1.2/project_utils/web/django/model/_base_model.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/pagination/_base_pagination.py` & `project-utils-config-1.1.2/project_utils/web/django/pagination/_base_pagination.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/request/_request.py` & `project-utils-config-1.1.2/project_utils/web/django/request/_request.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/response/_response_model.py` & `project-utils-config-1.1.2/project_utils/web/django/response/_response_model.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/swagger/_params/__init__.py` & `project-utils-config-1.1.2/project_utils/web/django/swagger/_params/__init__.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/swagger/_params/_form.py` & `project-utils-config-1.1.2/project_utils/web/django/swagger/_params/_form.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/swagger/_params/_params.py` & `project-utils-config-1.1.2/project_utils/web/django/swagger/_params/_params.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/swagger/_params/_query.py` & `project-utils-config-1.1.2/project_utils/web/django/swagger/_params/_query.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/swagger/_params/_response.py` & `project-utils-config-1.1.2/project_utils/web/django/swagger/_params/_response.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/swagger/config/_swagger.py` & `project-utils-config-1.1.2/project_utils/web/django/swagger/config/_swagger.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/swagger/document/_document.py` & `project-utils-config-1.1.2/project_utils/web/django/swagger/document/_document.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/utils.py` & `project-utils-config-1.1.2/project_utils/web/django/utils.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/view/_async_view.py` & `project-utils-config-1.1.2/project_utils/web/django/view/_async_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/view/_base.py` & `project-utils-config-1.1.2/project_utils/web/django/view/_base.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/view/_base_api/api.py` & `project-utils-config-1.1.2/project_utils/web/django/view/_base_api/api.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/view/_base_api/api_util.py` & `project-utils-config-1.1.2/project_utils/web/django/view/_base_api/api_util.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/view/_rest_api/api.py` & `project-utils-config-1.1.2/project_utils/web/django/view/_rest_api/api.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/view/_rest_api/async_api.py` & `project-utils-config-1.1.2/project_utils/web/django/view/_rest_api/async_api.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/view/_rest_view/_async_base_view.py` & `project-utils-config-1.1.2/project_utils/web/django/view/_rest_view/_async_base_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/view/_rest_view/_async_view.py` & `project-utils-config-1.1.2/project_utils/web/django/view/_rest_view/_async_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/view/_rest_view/_base_view.py` & `project-utils-config-1.1.2/project_utils/web/django/view/_rest_view/_base_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/view/_rest_view/_swagger_base.py` & `project-utils-config-1.1.2/project_utils/web/django/view/_rest_view/_swagger_base.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/view/_swagger_base.py` & `project-utils-config-1.1.2/project_utils/web/django/view/_swagger_base.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/view/_types.py` & `project-utils-config-1.1.2/project_utils/web/django/view/_types.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils/web/django/view/_user_view/_view.py` & `project-utils-config-1.1.2/project_utils/web/django/view/_user_view/_view.py`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/project_utils_config.egg-info/PKG-INFO` & `project-utils-config-1.1.2/project_utils_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-utils-config
-Version: 1.1.1
+Version: 1.1.2
 Summary: python project_utils tools
 Home-page: https://gitee.com/mylx2014/project-utils.git
 Author: mylx2014
 Author-email: mylx2014@163.com
 License: MIT
 Keywords: python,utils,project utils,aiofiles
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `project-utils-config-1.1.1/project_utils_config.egg-info/SOURCES.txt` & `project-utils-config-1.1.2/project_utils_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `project-utils-config-1.1.1/setup.py` & `project-utils-config-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.1.1"
+VERSION = "1.1.2"
 DESCRIPTION = "python project_utils tools"
 setup(
     name="project-utils-config",
     version=VERSION,
     author="mylx2014",
     author_email="mylx2014@163.com",
     description=DESCRIPTION,
```

