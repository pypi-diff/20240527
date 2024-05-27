# Comparing `tmp/metasdk-1.7.9.tar.gz` & `tmp/metasdk-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasdk-1.7.9.tar", last modified: Fri Apr 12 07:54:38 2024, max compression
+gzip compressed data, was "metasdk-1.8.0.tar", last modified: Mon May 27 13:42:17 2024, max compression
```

## Comparing `metasdk-1.7.9.tar` & `metasdk-1.8.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-12 07:54:38.211857 metasdk-1.7.9/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1074 2022-08-11 12:23:20.000000 metasdk-1.7.9/LICENSE
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.7.9/MANIFEST.in
--rw-r--r--   0 zhas      (1000) zhas      (1000)     2830 2024-04-12 07:54:38.211857 metasdk-1.7.9/PKG-INFO
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2236 2024-02-12 19:35:51.000000 metasdk-1.7.9/README.md
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-12 07:54:38.203857 metasdk-1.7.9/metasdk/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)    16426 2024-04-11 12:36:26.000000 metasdk-1.7.9/metasdk/__init__.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      190 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/__state.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     3803 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/apiclient.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     6152 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/event_bus.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     3523 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/exceptions.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      102 2024-04-12 07:54:23.000000 metasdk-1.7.9/metasdk/info.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1815 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/internal.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-12 07:54:38.203857 metasdk-1.7.9/metasdk/logger/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     6374 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/logger/__init__.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1862 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/logger/bulk_logger.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     3478 2024-01-25 19:39:16.000000 metasdk-1.7.9/metasdk/logger/logger.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-12 07:54:38.207857 metasdk-1.7.9/metasdk/services/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     8667 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/ApiProxyService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     5097 2024-04-12 07:54:23.000000 metasdk-1.7.9/metasdk/services/AuthService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      634 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/CacheService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     5086 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/DbQueryService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2924 2024-01-25 19:39:16.000000 metasdk-1.7.9/metasdk/services/DbService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1355 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/DevService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1066 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/ExportService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2563 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/ExternalSystemService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)    21782 2024-04-03 11:33:07.000000 metasdk-1.7.9/metasdk/services/FeedService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1939 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/IssueService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     5823 2024-01-25 19:39:16.000000 metasdk-1.7.9/metasdk/services/LockService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1394 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/MailService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1936 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/MediaService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1362 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/MetaqlService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      968 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/ObjectLogService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2554 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/SettingsService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     9916 2024-04-12 07:54:23.000000 metasdk-1.7.9/metasdk/services/StarterService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      691 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/UserManagementService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1157 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/__init__.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-12 07:54:38.207857 metasdk-1.7.9/metasdk/tools/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/tools/__init__.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1079 2024-01-25 19:39:16.000000 metasdk-1.7.9/metasdk/tools/extract_event_handlers.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2252 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/utils.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2051 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/worker.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-12 07:54:38.203857 metasdk-1.7.9/metasdk.egg-info/
--rw-r--r--   0 zhas      (1000) zhas      (1000)     2830 2024-04-12 07:54:38.000000 metasdk-1.7.9/metasdk.egg-info/PKG-INFO
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1172 2024-04-12 07:54:38.000000 metasdk-1.7.9/metasdk.egg-info/SOURCES.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        1 2024-04-12 07:54:38.000000 metasdk-1.7.9/metasdk.egg-info/dependency_links.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      172 2024-04-12 07:54:38.000000 metasdk-1.7.9/metasdk.egg-info/requires.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        8 2024-04-12 07:54:38.000000 metasdk-1.7.9/metasdk.egg-info/top_level.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      205 2024-04-12 07:54:38.211857 metasdk-1.7.9/setup.cfg
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1193 2022-08-11 12:23:20.000000 metasdk-1.7.9/setup.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-05-27 13:42:17.724128 metasdk-1.8.0/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1074 2022-08-11 12:23:20.000000 metasdk-1.8.0/LICENSE
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.8.0/MANIFEST.in
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2737 2024-05-27 13:42:17.724128 metasdk-1.8.0/PKG-INFO
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2465 2024-05-27 13:39:37.000000 metasdk-1.8.0/README.md
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-05-27 13:42:17.724128 metasdk-1.8.0/metasdk/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)    16426 2024-04-11 12:36:26.000000 metasdk-1.8.0/metasdk/__init__.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      190 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/__state.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     3803 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/apiclient.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     6152 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/event_bus.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     3523 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/exceptions.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      102 2024-05-27 13:39:37.000000 metasdk-1.8.0/metasdk/info.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1815 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/internal.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-05-27 13:42:17.724128 metasdk-1.8.0/metasdk/logger/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     6374 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/logger/__init__.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1862 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/logger/bulk_logger.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     3478 2024-01-25 19:39:16.000000 metasdk-1.8.0/metasdk/logger/logger.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-05-27 13:42:17.724128 metasdk-1.8.0/metasdk/services/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     8667 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/services/ApiProxyService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     5097 2024-04-12 07:54:23.000000 metasdk-1.8.0/metasdk/services/AuthService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      634 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/services/CacheService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     5086 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/services/DbQueryService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2924 2024-01-25 19:39:16.000000 metasdk-1.8.0/metasdk/services/DbService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1355 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/services/DevService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1066 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/services/ExportService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2563 2024-05-20 16:05:07.000000 metasdk-1.8.0/metasdk/services/ExternalSystemService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)    21977 2024-05-27 10:45:44.000000 metasdk-1.8.0/metasdk/services/FeedService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1939 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/services/IssueService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     5820 2024-05-27 13:39:37.000000 metasdk-1.8.0/metasdk/services/LockService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1394 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/services/MailService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1936 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/services/MediaService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1362 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/services/MetaqlService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      968 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/services/ObjectLogService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2554 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/services/SettingsService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     9916 2024-04-12 07:54:23.000000 metasdk-1.8.0/metasdk/services/StarterService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      691 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/services/UserManagementService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1157 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/services/__init__.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-05-27 13:42:17.724128 metasdk-1.8.0/metasdk/tools/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/tools/__init__.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1079 2024-01-25 19:39:16.000000 metasdk-1.8.0/metasdk/tools/extract_event_handlers.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     3105 2024-05-27 13:39:37.000000 metasdk-1.8.0/metasdk/utils.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2051 2022-08-11 12:23:20.000000 metasdk-1.8.0/metasdk/worker.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-05-27 13:42:17.724128 metasdk-1.8.0/metasdk.egg-info/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2737 2024-05-27 13:42:17.000000 metasdk-1.8.0/metasdk.egg-info/PKG-INFO
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1172 2024-05-27 13:42:17.000000 metasdk-1.8.0/metasdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        1 2024-05-27 13:42:17.000000 metasdk-1.8.0/metasdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      172 2024-05-27 13:42:17.000000 metasdk-1.8.0/metasdk.egg-info/requires.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        8 2024-05-27 13:42:17.000000 metasdk-1.8.0/metasdk.egg-info/top_level.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      205 2024-05-27 13:42:17.724128 metasdk-1.8.0/setup.cfg
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1193 2022-08-11 12:23:20.000000 metasdk-1.8.0/setup.py
```

### Comparing `metasdk-1.7.9/LICENSE` & `metasdk-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/README.md` & `metasdk-1.8.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # MetaSDK Python
 
 [Документация](http://metasdk.readthedocs.io/)
 
 [Полный список примеров](https://github.com/devision-io/metasdk/tree/master/metasdk/examples/)
 
-#### Как обновить metasdk в pypi.org
+### Как обновить metasdk в pypi.org
 
 1. Если кто-то из новых людей будет пробовать обновлять - надо дописать гайд как зарегаться на pypi.org и получить возможность обновлять метасдк
 
 2. Обновляем наш репозиторий в соответствии с общими правилами, не забываем апнуть версию (version) в info.py, как обычно в пайтон-либах (на момент написания это - обновляем мастер, создаём ветку с номером задачи из мастера, заливаем коммиты в ветку, создаём пулл-реквест в стеше, при необходимости мержимся с актуальным мастером, проходим ревью, заливаем в мастер)
 
 3. Если не устанавливали, устанавливаем pip3 install wheel && pip3 install twine (если ещё не делали (это как раз тот этап, когда у кого-то может деплоиться, а у кого-то нет)
 
 4. Делаем make publish. С 1 января 2024 года pypi больше не использует логин/пароль юзера для обновления проектов. Теперь сначала нужно включить двухфакторную аутентификацию.
 Затем можно выпустить API токен для своего аккаунта. При make publish передать в username: "__token__", в password: <полученый токен>. Подробности: https://pypi.org/help/#apitoken
 
 5. Обновить версию в тех репозиториях, для которых, собственно, делаются изменения (например, metafeedconnectors)
 
 
+### Рекомендации пользователям MetaSDK Python
+- Не устанавливать отдельно зависимости прописанные в MetaSDK. Например: библиотеку requests.
+
 Связанные задачи:
 - META-2941
 - META-2571
```

### Comparing `metasdk-1.7.9/metasdk/__init__.py` & `metasdk-1.8.0/metasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/apiclient.py` & `metasdk-1.8.0/metasdk/apiclient.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/event_bus.py` & `metasdk-1.8.0/metasdk/event_bus.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/exceptions.py` & `metasdk-1.8.0/metasdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/internal.py` & `metasdk-1.8.0/metasdk/internal.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/logger/__init__.py` & `metasdk-1.8.0/metasdk/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/logger/bulk_logger.py` & `metasdk-1.8.0/metasdk/logger/bulk_logger.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/logger/logger.py` & `metasdk-1.8.0/metasdk/logger/logger.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/ApiProxyService.py` & `metasdk-1.8.0/metasdk/services/ApiProxyService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/AuthService.py` & `metasdk-1.8.0/metasdk/services/AuthService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/CacheService.py` & `metasdk-1.8.0/metasdk/services/CacheService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/DbQueryService.py` & `metasdk-1.8.0/metasdk/services/DbQueryService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/DbService.py` & `metasdk-1.8.0/metasdk/services/DbService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/DevService.py` & `metasdk-1.8.0/metasdk/services/DevService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/ExportService.py` & `metasdk-1.8.0/metasdk/services/ExportService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/ExternalSystemService.py` & `metasdk-1.8.0/metasdk/services/ExternalSystemService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/FeedService.py` & `metasdk-1.8.0/metasdk/services/FeedService.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,14 +249,19 @@
         """
         if not filters:
             return ""
 
         special_types = {
             "state": "meta.feed_datasource_state_type",
             "user_status": "meta.user_status_type",
+            "parent_id": "uuid",
+            "share_type_id": "uuid",
+            "connector_id": "uuid",
+            "connector_type_id": "uuid",
+            "connector_type_preset_id": "uuid",
         }
         filters_sql = []
         for key, value in filters.items():
             if key == "tags":
                 tags = self._generate_tags_query(tags=value)
                 filter_expr = f"AND {tags}"
             else:
```

### Comparing `metasdk-1.7.9/metasdk/services/IssueService.py` & `metasdk-1.8.0/metasdk/services/IssueService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/LockService.py` & `metasdk-1.8.0/metasdk/services/LockService.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self.__connect_to_redis()
         waiting_time = random.randint(1, 3)
         time.sleep(0.0001 * waiting_time)
         key = key + str(random.randint(1, queue_width))
 
         try:
             while timeout_in_sec > 0:
-                is_set = self.__redis_storage.set(name=key, value=True, ex=ttl_in_sec, nx=True)
+                is_set = self.__redis_storage.set(name=key, value=1, ex=ttl_in_sec, nx=True)
                 if is_set:
                     yield
                     break
                 else:
                     time.sleep(waiting_time)
                     timeout_in_sec -= waiting_time
             else:
```

### Comparing `metasdk-1.7.9/metasdk/services/MailService.py` & `metasdk-1.8.0/metasdk/services/MailService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/MediaService.py` & `metasdk-1.8.0/metasdk/services/MediaService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/MetaqlService.py` & `metasdk-1.8.0/metasdk/services/MetaqlService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/ObjectLogService.py` & `metasdk-1.8.0/metasdk/services/ObjectLogService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/SettingsService.py` & `metasdk-1.8.0/metasdk/services/SettingsService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/StarterService.py` & `metasdk-1.8.0/metasdk/services/StarterService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/UserManagementService.py` & `metasdk-1.8.0/metasdk/services/UserManagementService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/services/__init__.py` & `metasdk-1.8.0/metasdk/services/__init__.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/tools/extract_event_handlers.py` & `metasdk-1.8.0/metasdk/tools/extract_event_handlers.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk/utils.py` & `metasdk-1.8.0/metasdk/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -44,26 +44,44 @@
     Представить объект в вище json красиво отформатированной строки
     :param obj:
     :return:
     """
     return json.dumps(obj, sort_keys=True, indent=4, separators=(',', ': '), ensure_ascii=False)
 
 
+def get_decode_algorithms(token: str | bytes) -> list[str]:
+    """
+    Получает алгоритмы декодирования токена.
+
+    jwt.decode() требует передачи списка алгоритмов для декодирования.
+    Стандратно это 'HS256' и 'RS256'. На случай другого алгоритма, проверяем заголовок токена.
+    :param token: токен.
+    :return: список алгоритмов.
+    """
+    default_algorithms = ["HS256", "RS256"]
+    headers = jwt.get_unverified_header(token)
+    header_alg = headers.get("alg")
+    if header_alg and header_alg not in default_algorithms:
+        default_algorithms.append(header_alg)
+    return default_algorithms
+
+
 def decode_jwt(input_text, secure_key):
     """
     Раскодирование строки на основе ключа
     :param input_text: исходная строка
     :param secure_key: секретный ключ
     :return:
     """
     if input_text is None:
         return None
 
     encoded = (input_text.split(":")[1]).encode('utf-8')
-    decoded = jwt.decode(encoded, secure_key)
+    algorithms = get_decode_algorithms(token=encoded)
+    decoded = jwt.decode(encoded, secure_key, algorithms=algorithms)
     return decoded['sub']
 
 
 def file_hash_sum(file_full_path: str) -> str:
     """
     Хэш от содержимого файла
     :param file_full_path: полный путь к файлу
```

### Comparing `metasdk-1.7.9/metasdk/worker.py` & `metasdk-1.8.0/metasdk/worker.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/metasdk.egg-info/SOURCES.txt` & `metasdk-1.8.0/metasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.9/setup.py` & `metasdk-1.8.0/setup.py`

 * *Files identical despite different names*

