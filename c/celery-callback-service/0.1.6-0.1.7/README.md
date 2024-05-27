# Comparing `tmp/celery-callback-service-0.1.6.tar.gz` & `tmp/celery-callback-service-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery-callback-service-0.1.6.tar", last modified: Sat May 25 09:06:12 2024, max compression
+gzip compressed data, was "celery-callback-service-0.1.7.tar", last modified: Mon May 27 06:54:58 2024, max compression
```

## Comparing `celery-callback-service-0.1.6.tar` & `celery-callback-service-0.1.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-25 09:06:12.596089 celery-callback-service-0.1.6/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-22 22:04:02.000000 celery-callback-service-0.1.6/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      239 2024-05-22 22:04:46.000000 celery-callback-service-0.1.6/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     4722 2024-05-25 09:06:12.595966 celery-callback-service-0.1.6/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     4000 2024-05-25 08:55:48.000000 celery-callback-service-0.1.6/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-25 09:06:12.589481 celery-callback-service-0.1.6/celery_callback_server/
--rw-r--r--   0 test       (501) staff       (20)        0 2024-05-22 14:28:20.000000 celery-callback-service-0.1.6/celery_callback_server/__init__.py
--rw-r--r--   0 test       (501) staff       (20)      421 2024-05-22 14:28:20.000000 celery-callback-service-0.1.6/celery_callback_server/asgi.py
--rw-r--r--   0 test       (501) staff       (20)     3870 2024-05-24 15:54:46.000000 celery-callback-service-0.1.6/celery_callback_server/settings.py
--rw-r--r--   0 test       (501) staff       (20)      987 2024-05-24 15:54:26.000000 celery-callback-service-0.1.6/celery_callback_server/urls.py
--rw-r--r--   0 test       (501) staff       (20)      421 2024-05-22 14:28:20.000000 celery-callback-service-0.1.6/celery_callback_server/wsgi.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-25 09:06:12.593562 celery-callback-service-0.1.6/celery_callback_service/
--rw-r--r--   0 test       (501) staff       (20)       60 2024-05-22 23:23:01.000000 celery-callback-service-0.1.6/celery_callback_service/__init__.py
--rw-r--r--   0 test       (501) staff       (20)      580 2024-05-25 00:54:32.000000 celery-callback-service-0.1.6/celery_callback_service/actions.py
--rw-r--r--   0 test       (501) staff       (20)     2324 2024-05-25 03:20:17.000000 celery-callback-service-0.1.6/celery_callback_service/admin.py
--rw-r--r--   0 test       (501) staff       (20)      225 2024-05-22 16:05:05.000000 celery-callback-service-0.1.6/celery_callback_service/apps.py
--rw-r--r--   0 test       (501) staff       (20)     3213 2024-05-25 08:15:24.000000 celery-callback-service-0.1.6/celery_callback_service/celery_tasks.py
--rw-r--r--   0 test       (501) staff       (20)      129 2024-05-24 15:13:56.000000 celery-callback-service-0.1.6/celery_callback_service/client.py
--rw-r--r--   0 test       (501) staff       (20)       71 2024-05-22 15:04:16.000000 celery-callback-service-0.1.6/celery_callback_service/constants.py
--rw-r--r--   0 test       (501) staff       (20)      151 2024-05-22 15:30:42.000000 celery-callback-service-0.1.6/celery_callback_service/forms.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-25 09:06:12.595790 celery-callback-service-0.1.6/celery_callback_service/migrations/
--rw-r--r--   0 test       (501) staff       (20)     2109 2024-05-22 15:58:51.000000 celery-callback-service-0.1.6/celery_callback_service/migrations/0001_initial.py
--rw-r--r--   0 test       (501) staff       (20)     1256 2024-05-22 22:39:50.000000 celery-callback-service-0.1.6/celery_callback_service/migrations/0002_alter_task_options_task_error_data_and_more.py
--rw-r--r--   0 test       (501) staff       (20)      889 2024-05-24 15:47:04.000000 celery-callback-service-0.1.6/celery_callback_service/migrations/0003_remove_task_done_time_remove_task_ready_time_and_more.py
--rw-r--r--   0 test       (501) staff       (20)      796 2024-05-25 01:36:58.000000 celery-callback-service-0.1.6/celery_callback_service/migrations/0004_alter_task_options.py
--rw-r--r--   0 test       (501) staff       (20)        0 2024-05-22 14:28:38.000000 celery-callback-service-0.1.6/celery_callback_service/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)     3025 2024-05-25 08:17:33.000000 celery-callback-service-0.1.6/celery_callback_service/models.py
--rw-r--r--   0 test       (501) staff       (20)     2070 2024-05-25 08:06:02.000000 celery-callback-service-0.1.6/celery_callback_service/services.py
--rw-r--r--   0 test       (501) staff       (20)      987 2024-05-25 00:16:58.000000 celery-callback-service-0.1.6/celery_callback_service/settings.py
--rw-r--r--   0 test       (501) staff       (20)      556 2024-05-25 08:18:49.000000 celery-callback-service-0.1.6/celery_callback_service/tests.py
--rw-r--r--   0 test       (501) staff       (20)      215 2024-05-22 15:31:59.000000 celery-callback-service-0.1.6/celery_callback_service/urls.py
--rw-r--r--   0 test       (501) staff       (20)      313 2024-05-25 08:18:15.000000 celery-callback-service-0.1.6/celery_callback_service/utils.py
--rw-r--r--   0 test       (501) staff       (20)      749 2024-05-24 16:04:18.000000 celery-callback-service-0.1.6/celery_callback_service/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-25 09:06:12.594502 celery-callback-service-0.1.6/celery_callback_service.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     4722 2024-05-25 09:06:12.000000 celery-callback-service-0.1.6/celery_callback_service.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     1442 2024-05-25 09:06:12.000000 celery-callback-service-0.1.6/celery_callback_service.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-25 09:06:12.000000 celery-callback-service-0.1.6/celery_callback_service.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)       85 2024-05-25 09:06:12.000000 celery-callback-service-0.1.6/celery_callback_service.egg-info/entry_points.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-25 09:06:12.000000 celery-callback-service-0.1.6/celery_callback_service.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)      239 2024-05-25 09:06:12.000000 celery-callback-service-0.1.6/celery_callback_service.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       77 2024-05-25 09:06:12.000000 celery-callback-service-0.1.6/celery_callback_service.egg-info/top_level.txt
--rwxr-xr-x   0 test       (501) staff       (20)      678 2024-05-22 14:28:20.000000 celery-callback-service-0.1.6/manage_celery_callback_server.py
--rw-r--r--   0 test       (501) staff       (20)      239 2024-05-25 08:22:25.000000 celery-callback-service-0.1.6/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-05-25 09:06:12.596130 celery-callback-service-0.1.6/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1547 2024-05-25 02:52:53.000000 celery-callback-service-0.1.6/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 06:54:58.350027 celery-callback-service-0.1.7/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-22 22:04:02.000000 celery-callback-service-0.1.7/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      239 2024-05-22 22:04:46.000000 celery-callback-service-0.1.7/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     4831 2024-05-27 06:54:58.349886 celery-callback-service-0.1.7/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     4109 2024-05-27 06:54:35.000000 celery-callback-service-0.1.7/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 06:54:58.342904 celery-callback-service-0.1.7/celery_callback_server/
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-05-22 14:28:20.000000 celery-callback-service-0.1.7/celery_callback_server/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      421 2024-05-22 14:28:20.000000 celery-callback-service-0.1.7/celery_callback_server/asgi.py
+-rw-r--r--   0 test       (501) staff       (20)     3870 2024-05-24 15:54:46.000000 celery-callback-service-0.1.7/celery_callback_server/settings.py
+-rw-r--r--   0 test       (501) staff       (20)      987 2024-05-24 15:54:26.000000 celery-callback-service-0.1.7/celery_callback_server/urls.py
+-rw-r--r--   0 test       (501) staff       (20)      421 2024-05-22 14:28:20.000000 celery-callback-service-0.1.7/celery_callback_server/wsgi.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 06:54:58.347187 celery-callback-service-0.1.7/celery_callback_service/
+-rw-r--r--   0 test       (501) staff       (20)       60 2024-05-22 23:23:01.000000 celery-callback-service-0.1.7/celery_callback_service/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      580 2024-05-25 00:54:32.000000 celery-callback-service-0.1.7/celery_callback_service/actions.py
+-rw-r--r--   0 test       (501) staff       (20)     2324 2024-05-25 03:20:17.000000 celery-callback-service-0.1.7/celery_callback_service/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      225 2024-05-22 16:05:05.000000 celery-callback-service-0.1.7/celery_callback_service/apps.py
+-rw-r--r--   0 test       (501) staff       (20)     3213 2024-05-25 08:15:24.000000 celery-callback-service-0.1.7/celery_callback_service/celery_tasks.py
+-rw-r--r--   0 test       (501) staff       (20)      129 2024-05-24 15:13:56.000000 celery-callback-service-0.1.7/celery_callback_service/client.py
+-rw-r--r--   0 test       (501) staff       (20)       71 2024-05-22 15:04:16.000000 celery-callback-service-0.1.7/celery_callback_service/constants.py
+-rw-r--r--   0 test       (501) staff       (20)      151 2024-05-22 15:30:42.000000 celery-callback-service-0.1.7/celery_callback_service/forms.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 06:54:58.349675 celery-callback-service-0.1.7/celery_callback_service/migrations/
+-rw-r--r--   0 test       (501) staff       (20)     2109 2024-05-22 15:58:51.000000 celery-callback-service-0.1.7/celery_callback_service/migrations/0001_initial.py
+-rw-r--r--   0 test       (501) staff       (20)     1256 2024-05-22 22:39:50.000000 celery-callback-service-0.1.7/celery_callback_service/migrations/0002_alter_task_options_task_error_data_and_more.py
+-rw-r--r--   0 test       (501) staff       (20)      889 2024-05-24 15:47:04.000000 celery-callback-service-0.1.7/celery_callback_service/migrations/0003_remove_task_done_time_remove_task_ready_time_and_more.py
+-rw-r--r--   0 test       (501) staff       (20)      796 2024-05-25 01:36:58.000000 celery-callback-service-0.1.7/celery_callback_service/migrations/0004_alter_task_options.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-05-22 14:28:38.000000 celery-callback-service-0.1.7/celery_callback_service/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     3025 2024-05-25 08:17:33.000000 celery-callback-service-0.1.7/celery_callback_service/models.py
+-rw-r--r--   0 test       (501) staff       (20)     2070 2024-05-25 08:06:02.000000 celery-callback-service-0.1.7/celery_callback_service/services.py
+-rw-r--r--   0 test       (501) staff       (20)      987 2024-05-25 00:16:58.000000 celery-callback-service-0.1.7/celery_callback_service/settings.py
+-rw-r--r--   0 test       (501) staff       (20)      556 2024-05-25 08:18:49.000000 celery-callback-service-0.1.7/celery_callback_service/tests.py
+-rw-r--r--   0 test       (501) staff       (20)      215 2024-05-22 15:31:59.000000 celery-callback-service-0.1.7/celery_callback_service/urls.py
+-rw-r--r--   0 test       (501) staff       (20)      313 2024-05-25 08:18:15.000000 celery-callback-service-0.1.7/celery_callback_service/utils.py
+-rw-r--r--   0 test       (501) staff       (20)      749 2024-05-24 16:04:18.000000 celery-callback-service-0.1.7/celery_callback_service/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 06:54:58.348244 celery-callback-service-0.1.7/celery_callback_service.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     4831 2024-05-27 06:54:58.000000 celery-callback-service-0.1.7/celery_callback_service.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     1442 2024-05-27 06:54:58.000000 celery-callback-service-0.1.7/celery_callback_service.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-27 06:54:58.000000 celery-callback-service-0.1.7/celery_callback_service.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)       85 2024-05-27 06:54:58.000000 celery-callback-service-0.1.7/celery_callback_service.egg-info/entry_points.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-27 06:54:58.000000 celery-callback-service-0.1.7/celery_callback_service.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)      239 2024-05-27 06:54:58.000000 celery-callback-service-0.1.7/celery_callback_service.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       77 2024-05-27 06:54:58.000000 celery-callback-service-0.1.7/celery_callback_service.egg-info/top_level.txt
+-rwxr-xr-x   0 test       (501) staff       (20)      678 2024-05-22 14:28:20.000000 celery-callback-service-0.1.7/manage_celery_callback_server.py
+-rw-r--r--   0 test       (501) staff       (20)      239 2024-05-25 08:22:25.000000 celery-callback-service-0.1.7/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-27 06:54:58.350089 celery-callback-service-0.1.7/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1547 2024-05-27 06:54:40.000000 celery-callback-service-0.1.7/setup.py
```

### Comparing `celery-callback-service-0.1.6/LICENSE` & `celery-callback-service-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/PKG-INFO` & `celery-callback-service-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery-callback-service
-Version: 0.1.6
+Version: 0.1.7
 Summary: 基于celery的回调服务。业务系统创建celery回调任务，celery-callback-worker执行回调任务，业务系统在回调任务中处理异步任务。
 Author: Sun XiaoWei
 Maintainer: Sun XiaoWei
 License: MIT
 Keywords: celery callback service
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -155,7 +155,11 @@
     - 重试延迟规则是：5秒（可配置） * 重试次数，最大延迟300秒（可配置）。
 
 ## 版本记录
 
 ### v0.1.6
 
 - 版本首发。
+
+### v0.1.7
+
+- 管理界面添加重新推送、添加删除标记、取消删除标记等指处理动作。
```

### Comparing `celery-callback-service-0.1.6/README.md` & `celery-callback-service-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -138,7 +138,11 @@
     - 重试延迟规则是：5秒（可配置） * 重试次数，最大延迟300秒（可配置）。
 
 ## 版本记录
 
 ### v0.1.6
 
 - 版本首发。
+
+### v0.1.7
+
+- 管理界面添加重新推送、添加删除标记、取消删除标记等指处理动作。
```

### Comparing `celery-callback-service-0.1.6/celery_callback_server/settings.py` & `celery-callback-service-0.1.7/celery_callback_server/settings.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/celery_callback_server/urls.py` & `celery-callback-service-0.1.7/celery_callback_server/urls.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/celery_callback_service/actions.py` & `celery-callback-service-0.1.7/celery_callback_service/actions.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/celery_callback_service/admin.py` & `celery-callback-service-0.1.7/celery_callback_service/admin.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/celery_callback_service/celery_tasks.py` & `celery-callback-service-0.1.7/celery_callback_service/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/celery_callback_service/migrations/0001_initial.py` & `celery-callback-service-0.1.7/celery_callback_service/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/celery_callback_service/migrations/0002_alter_task_options_task_error_data_and_more.py` & `celery-callback-service-0.1.7/celery_callback_service/migrations/0002_alter_task_options_task_error_data_and_more.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/celery_callback_service/migrations/0003_remove_task_done_time_remove_task_ready_time_and_more.py` & `celery-callback-service-0.1.7/celery_callback_service/migrations/0003_remove_task_done_time_remove_task_ready_time_and_more.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/celery_callback_service/migrations/0004_alter_task_options.py` & `celery-callback-service-0.1.7/celery_callback_service/migrations/0004_alter_task_options.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/celery_callback_service/models.py` & `celery-callback-service-0.1.7/celery_callback_service/models.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/celery_callback_service/services.py` & `celery-callback-service-0.1.7/celery_callback_service/services.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/celery_callback_service/settings.py` & `celery-callback-service-0.1.7/celery_callback_service/settings.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/celery_callback_service/tests.py` & `celery-callback-service-0.1.7/celery_callback_service/tests.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/celery_callback_service/views.py` & `celery-callback-service-0.1.7/celery_callback_service/views.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/celery_callback_service.egg-info/PKG-INFO` & `celery-callback-service-0.1.7/celery_callback_service.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery-callback-service
-Version: 0.1.6
+Version: 0.1.7
 Summary: 基于celery的回调服务。业务系统创建celery回调任务，celery-callback-worker执行回调任务，业务系统在回调任务中处理异步任务。
 Author: Sun XiaoWei
 Maintainer: Sun XiaoWei
 License: MIT
 Keywords: celery callback service
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -155,7 +155,11 @@
     - 重试延迟规则是：5秒（可配置） * 重试次数，最大延迟300秒（可配置）。
 
 ## 版本记录
 
 ### v0.1.6
 
 - 版本首发。
+
+### v0.1.7
+
+- 管理界面添加重新推送、添加删除标记、取消删除标记等指处理动作。
```

### Comparing `celery-callback-service-0.1.6/celery_callback_service.egg-info/SOURCES.txt` & `celery-callback-service-0.1.7/celery_callback_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/manage_celery_callback_server.py` & `celery-callback-service-0.1.7/manage_celery_callback_server.py`

 * *Files identical despite different names*

### Comparing `celery-callback-service-0.1.6/setup.py` & `celery-callback-service-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="celery-callback-service",
-    version="0.1.6",
+    version="0.1.7",
     description="基于celery的回调服务。业务系统创建celery回调任务，celery-callback-worker执行回调任务，业务系统在回调任务中处理异步任务。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Sun XiaoWei",
     maintainer="Sun XiaoWei",
     license="MIT",
     classifiers=[
```

