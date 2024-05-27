# Comparing `tmp/djpress-0.3.1.tar.gz` & `tmp/djpress-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djpress-0.3.1.tar", last modified: Sat May 25 22:36:25 2024, max compression
+gzip compressed data, was "djpress-0.3.2.tar", last modified: Mon May 27 13:05:06 2024, max compression
```

## Comparing `djpress-0.3.1.tar` & `djpress-0.3.2.tar`

### file list

```diff
@@ -1,56 +1,55 @@
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 22:36:25.915588 djpress-0.3.1/
--rw-r--r--   0 stuart     (501) staff       (20)     1071 2024-05-25 02:51:53.000000 djpress-0.3.1/LICENSE
--rw-r--r--   0 stuart     (501) staff       (20)      132 2024-05-25 03:38:25.000000 djpress-0.3.1/MANIFEST.in
--rw-r--r--   0 stuart     (501) staff       (20)     3710 2024-05-25 22:36:25.915380 djpress-0.3.1/PKG-INFO
--rw-r--r--   0 stuart     (501) staff       (20)     1208 2024-05-25 22:35:25.000000 djpress-0.3.1/README.md
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 22:36:25.909056 djpress-0.3.1/djpress/
--rw-r--r--   0 stuart     (501) staff       (20)       22 2024-04-24 12:01:53.000000 djpress-0.3.1/djpress/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)      197 2024-05-11 07:24:31.000000 djpress-0.3.1/djpress/admin.py
--rw-r--r--   0 stuart     (501) staff       (20)      733 2024-05-25 04:49:43.000000 djpress-0.3.1/djpress/app_settings.py
--rw-r--r--   0 stuart     (501) staff       (20)      362 2024-05-25 03:38:21.000000 djpress-0.3.1/djpress/apps.py
--rw-r--r--   0 stuart     (501) staff       (20)      907 2024-05-25 05:08:15.000000 djpress-0.3.1/djpress/conf.py
--rw-r--r--   0 stuart     (501) staff       (20)     1254 2024-05-11 07:24:31.000000 djpress-0.3.1/djpress/feeds.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 22:36:25.910562 djpress-0.3.1/djpress/migrations/
--rw-r--r--   0 stuart     (501) staff       (20)     2077 2024-05-11 07:24:31.000000 djpress-0.3.1/djpress/migrations/0001_initial.py
--rw-r--r--   0 stuart     (501) staff       (20)      359 2024-05-11 07:24:31.000000 djpress-0.3.1/djpress/migrations/0002_rename_content_type_post_post_type.py
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-11 07:24:31.000000 djpress-0.3.1/djpress/migrations/__init__.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 22:36:25.911142 djpress-0.3.1/djpress/models/
--rw-r--r--   0 stuart     (501) staff       (20)      149 2024-05-11 07:24:31.000000 djpress-0.3.1/djpress/models/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     3137 2024-05-25 05:11:16.000000 djpress-0.3.1/djpress/models/category.py
--rw-r--r--   0 stuart     (501) staff       (20)     9716 2024-05-25 05:11:32.000000 djpress-0.3.1/djpress/models/post.py
--rw-r--r--   0 stuart     (501) staff       (20)      798 2024-05-11 07:24:31.000000 djpress-0.3.1/djpress/signals.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 22:36:25.904674 djpress-0.3.1/djpress/static/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 22:36:25.904731 djpress-0.3.1/djpress/static/djpress/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 22:36:25.911797 djpress-0.3.1/djpress/static/djpress/css/
--rw-r--r--   0 stuart     (501) staff       (20)     3388 2024-05-25 12:51:02.000000 djpress-0.3.1/djpress/static/djpress/css/style.css
--rw-r--r--   0 stuart     (501) staff       (20)     1104 2024-05-25 10:57:09.000000 djpress-0.3.1/djpress/static/djpress/css/style.min.css
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 22:36:25.904858 djpress-0.3.1/djpress/templates/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 22:36:25.912045 djpress-0.3.1/djpress/templates/djpress/
--rw-r--r--   0 stuart     (501) staff       (20)     2150 2024-05-25 22:15:06.000000 djpress-0.3.1/djpress/templates/djpress/index.html
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 22:36:25.912515 djpress-0.3.1/djpress/templatetags/
--rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.3.1/djpress/templatetags/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     8228 2024-05-25 22:11:54.000000 djpress-0.3.1/djpress/templatetags/djpress_tags.py
--rw-r--r--   0 stuart     (501) staff       (20)     2196 2024-05-25 22:14:02.000000 djpress-0.3.1/djpress/templatetags/helpers.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 22:36:25.914506 djpress-0.3.1/djpress/tests/
--rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.3.1/djpress/tests/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     2804 2024-05-11 07:24:31.000000 djpress-0.3.1/djpress/tests/test_category_cache.py
--rw-r--r--   0 stuart     (501) staff       (20)    14772 2024-05-25 22:18:09.000000 djpress-0.3.1/djpress/tests/test_djpress_tags.py
--rw-r--r--   0 stuart     (501) staff       (20)     2279 2024-05-25 05:11:50.000000 djpress-0.3.1/djpress/tests/test_feeds.py
--rw-r--r--   0 stuart     (501) staff       (20)    14353 2024-05-25 05:12:00.000000 djpress-0.3.1/djpress/tests/test_models.py
--rw-r--r--   0 stuart     (501) staff       (20)     1083 2024-05-11 07:24:31.000000 djpress-0.3.1/djpress/tests/test_post_authors.py
--rw-r--r--   0 stuart     (501) staff       (20)     3903 2024-05-11 07:24:31.000000 djpress-0.3.1/djpress/tests/test_published_posts_cache.py
--rw-r--r--   0 stuart     (501) staff       (20)     4665 2024-05-25 05:11:55.000000 djpress-0.3.1/djpress/tests/test_views.py
--rw-r--r--   0 stuart     (501) staff       (20)     1558 2024-05-25 05:10:42.000000 djpress-0.3.1/djpress/urls.py
--rw-r--r--   0 stuart     (501) staff       (20)      869 2024-05-25 05:10:58.000000 djpress-0.3.1/djpress/utils.py
--rw-r--r--   0 stuart     (501) staff       (20)     3845 2024-05-22 08:34:14.000000 djpress-0.3.1/djpress/views.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 22:36:25.915031 djpress-0.3.1/djpress.egg-info/
--rw-r--r--   0 stuart     (501) staff       (20)     3710 2024-05-25 22:36:25.000000 djpress-0.3.1/djpress.egg-info/PKG-INFO
--rw-r--r--   0 stuart     (501) staff       (20)     1084 2024-05-25 22:36:25.000000 djpress-0.3.1/djpress.egg-info/SOURCES.txt
--rw-r--r--   0 stuart     (501) staff       (20)        1 2024-05-25 22:36:25.000000 djpress-0.3.1/djpress.egg-info/dependency_links.txt
--rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 22:36:25.000000 djpress-0.3.1/djpress.egg-info/requires.txt
--rw-r--r--   0 stuart     (501) staff       (20)        8 2024-05-25 22:36:25.000000 djpress-0.3.1/djpress.egg-info/top_level.txt
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 22:36:25.914754 djpress-0.3.1/docs/
--rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 03:04:28.000000 djpress-0.3.1/docs/index.md
--rw-r--r--   0 stuart     (501) staff       (20)     1256 2024-05-25 22:20:06.000000 djpress-0.3.1/pyproject.toml
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 22:36:25.915768 djpress-0.3.1/setup.cfg
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 03:38:24.000000 djpress-0.3.1/setup.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.593070 djpress-0.3.2/
+-rw-r--r--   0 stuart     (501) staff       (20)     1071 2024-05-25 02:51:53.000000 djpress-0.3.2/LICENSE
+-rw-r--r--   0 stuart     (501) staff       (20)      132 2024-05-25 03:38:25.000000 djpress-0.3.2/MANIFEST.in
+-rw-r--r--   0 stuart     (501) staff       (20)     3907 2024-05-27 13:05:06.592801 djpress-0.3.2/PKG-INFO
+-rw-r--r--   0 stuart     (501) staff       (20)     1208 2024-05-25 22:35:25.000000 djpress-0.3.2/README.md
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.585769 djpress-0.3.2/djpress/
+-rw-r--r--   0 stuart     (501) staff       (20)       22 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)      197 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/admin.py
+-rw-r--r--   0 stuart     (501) staff       (20)      784 2024-05-27 13:00:19.000000 djpress-0.3.2/djpress/app_settings.py
+-rw-r--r--   0 stuart     (501) staff       (20)      362 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/apps.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1154 2024-05-27 13:00:19.000000 djpress-0.3.2/djpress/conf.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1254 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/feeds.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.587271 djpress-0.3.2/djpress/migrations/
+-rw-r--r--   0 stuart     (501) staff       (20)     2929 2024-05-27 10:44:59.000000 djpress-0.3.2/djpress/migrations/0001_initial.py
+-rw-r--r--   0 stuart     (501) staff       (20)      358 2024-05-27 10:44:59.000000 djpress-0.3.2/djpress/migrations/0002_rename_content_type_post_post_type.py
+-rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/migrations/__init__.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.587774 djpress-0.3.2/djpress/models/
+-rw-r--r--   0 stuart     (501) staff       (20)      149 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/models/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3137 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/models/category.py
+-rw-r--r--   0 stuart     (501) staff       (20)     9716 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/models/post.py
+-rw-r--r--   0 stuart     (501) staff       (20)      798 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/signals.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.581971 djpress-0.3.2/djpress/static/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.582022 djpress-0.3.2/djpress/static/djpress/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.588332 djpress-0.3.2/djpress/static/djpress/css/
+-rw-r--r--   0 stuart     (501) staff       (20)     3325 2024-05-27 10:57:47.000000 djpress-0.3.2/djpress/static/djpress/css/style.css
+-rw-r--r--   0 stuart     (501) staff       (20)     2449 2024-05-27 10:58:33.000000 djpress-0.3.2/djpress/static/djpress/css/style.min.css
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.582139 djpress-0.3.2/djpress/templates/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.588637 djpress-0.3.2/djpress/templates/djpress/
+-rw-r--r--   0 stuart     (501) staff       (20)     2150 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/templates/djpress/index.html
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.589280 djpress-0.3.2/djpress/templatetags/
+-rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/templatetags/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)     8228 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/templatetags/djpress_tags.py
+-rw-r--r--   0 stuart     (501) staff       (20)     2196 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/templatetags/helpers.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1558 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/urls.py
+-rw-r--r--   0 stuart     (501) staff       (20)      869 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/utils.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3845 2024-05-27 10:09:15.000000 djpress-0.3.2/djpress/views.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.592249 djpress-0.3.2/djpress.egg-info/
+-rw-r--r--   0 stuart     (501) staff       (20)     3907 2024-05-27 13:05:06.000000 djpress-0.3.2/djpress.egg-info/PKG-INFO
+-rw-r--r--   0 stuart     (501) staff       (20)     1002 2024-05-27 13:05:06.000000 djpress-0.3.2/djpress.egg-info/SOURCES.txt
+-rw-r--r--   0 stuart     (501) staff       (20)        1 2024-05-27 13:05:06.000000 djpress-0.3.2/djpress.egg-info/dependency_links.txt
+-rw-r--r--   0 stuart     (501) staff       (20)       71 2024-05-27 13:05:06.000000 djpress-0.3.2/djpress.egg-info/requires.txt
+-rw-r--r--   0 stuart     (501) staff       (20)        8 2024-05-27 13:05:06.000000 djpress-0.3.2/djpress.egg-info/top_level.txt
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.589451 djpress-0.3.2/docs/
+-rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 03:04:28.000000 djpress-0.3.2/docs/index.md
+-rw-r--r--   0 stuart     (501) staff       (20)     2064 2024-05-27 13:00:19.000000 djpress-0.3.2/pyproject.toml
+-rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-27 13:05:06.593120 djpress-0.3.2/setup.cfg
+-rw-r--r--   0 stuart     (501) staff       (20)       69 2024-05-27 09:29:30.000000 djpress-0.3.2/setup.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-27 13:05:06.591874 djpress-0.3.2/tests/
+-rw-r--r--   0 stuart     (501) staff       (20)     2804 2024-05-11 07:24:31.000000 djpress-0.3.2/tests/test_category_cache.py
+-rw-r--r--   0 stuart     (501) staff       (20)    14772 2024-05-25 22:18:09.000000 djpress-0.3.2/tests/test_djpress_tags.py
+-rw-r--r--   0 stuart     (501) staff       (20)     2279 2024-05-25 05:11:50.000000 djpress-0.3.2/tests/test_feeds.py
+-rw-r--r--   0 stuart     (501) staff       (20)    14353 2024-05-25 05:12:00.000000 djpress-0.3.2/tests/test_models.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1083 2024-05-11 07:24:31.000000 djpress-0.3.2/tests/test_post_authors.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3903 2024-05-11 07:24:31.000000 djpress-0.3.2/tests/test_published_posts_cache.py
+-rw-r--r--   0 stuart     (501) staff       (20)     4686 2024-05-27 13:00:19.000000 djpress-0.3.2/tests/test_views.py
```

### Comparing `djpress-0.3.1/LICENSE` & `djpress-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/PKG-INFO` & `djpress-0.3.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpress
-Version: 0.3.1
+Version: 0.3.2
 Summary: A blog application for Django sites, inspired by classic WordPress.
 Author-email: Stuart Maxwell <stuart@amanzi.nz>
 License: MIT License
         
         Copyright (c) 2024 Stuart Maxwell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,14 +45,20 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django
 Requires-Dist: markdown
+Requires-Dist: pygments
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-django; extra == "tests"
+Provides-Extra: linting
+Requires-Dist: ruff; extra == "linting"
 
 # DJ Press
 
 A blog application for Django sites, inspired by classic WordPress.
 
 > Warning - very alpha.
```

### Comparing `djpress-0.3.1/README.md` & `djpress-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/app_settings.py` & `djpress-0.3.2/djpress/app_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+"""Settings file for DJ Press."""
+
 # DJPress settings
 TRUNCATE_TAG = "<!--more-->"
 CACHE_CATEGORIES: bool = True
 CACHE_RECENT_PUBLISHED_POSTS: bool = False
 RECENT_PUBLISHED_POSTS_COUNT: int = 20
 MARKDOWN_EXTENSIONS: list = ["fenced_code", "codehilite", "tables"]
-BLOG_TITLE: str = ""
+BLOG_TITLE: str = "My DJ Press Blog"
 
 # DJPress URL settings
 CATEGORY_PATH_ENABLED: bool = True
 CATEGORY_PATH: str = "category"
 AUTHOR_PATH_ENABLED: bool = True
 AUTHOR_PATH: str = "author"
 ARCHIVES_PATH_ENABLED: bool = True
```

### Comparing `djpress-0.3.1/djpress/conf.py` & `djpress-0.3.2/djpress/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,33 @@
-"""Configuration settings for DJ Press"""
+"""Configuration settings for DJ Press."""
 
 from django.conf import settings as django_settings
 
 from . import app_settings as default_settings
 
 
 class Settings:
-    def __init__(self, default_settings_module, user_settings_module):
+    """Class to manage DJ Press settings."""
+
+    def __init__(
+        self: "Settings",
+        default_settings_module: object,
+        user_settings_module: object,
+    ) -> None:
+        """Initialize the settings object."""
         self._default_settings = default_settings_module
         self._user_settings = user_settings_module
 
-    def __getattr__(self, name):
+    def __getattr__(self: "Settings", name: str) -> object:
+        """Get the value of a setting."""
         # If the setting is found in the user settings, return it
         if hasattr(self._user_settings, name):
             return getattr(self._user_settings, name)
         # If the setting is found in the default settings, return it
         if hasattr(self._default_settings, name):
             return getattr(self._default_settings, name)
         # If the setting is not found in either, raise an AttributeError
-        raise AttributeError(f"Setting '{name}' not found")
+        msg = f"Setting '{name}' not found"
+        raise AttributeError(msg)
 
 
 settings = Settings(default_settings, django_settings)
```

### Comparing `djpress-0.3.1/djpress/feeds.py` & `djpress-0.3.2/djpress/feeds.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/migrations/0001_initial.py` & `djpress-0.3.2/djpress/migrations/0001_initial.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,48 +3,86 @@
 import django.db.models.deletion
 import django.utils.timezone
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='Category',
+            name="Category",
             fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=100)),
-                ('slug', models.SlugField(blank=True, unique=True)),
-                ('description', models.TextField(blank=True)),
+                (
+                    "id",
+                    models.BigAutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("name", models.CharField(max_length=100)),
+                ("slug", models.SlugField(blank=True, unique=True)),
+                ("description", models.TextField(blank=True)),
             ],
             options={
-                'verbose_name': 'category',
-                'verbose_name_plural': 'categories',
+                "verbose_name": "category",
+                "verbose_name_plural": "categories",
             },
         ),
         migrations.CreateModel(
-            name='Post',
+            name="Post",
             fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('title', models.CharField(max_length=200)),
-                ('slug', models.SlugField(blank=True, unique=True)),
-                ('content', models.TextField()),
-                ('date', models.DateTimeField(default=django.utils.timezone.now)),
-                ('modified_date', models.DateTimeField(auto_now=True)),
-                ('status', models.CharField(choices=[('draft', 'Draft'), ('published', 'Published')], default='draft', max_length=10)),
-                ('content_type', models.CharField(choices=[('post', 'Post'), ('page', 'Page')], default='post', max_length=10)),
-                ('author', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
-                ('categories', models.ManyToManyField(blank=True, to='djpress.category')),
+                (
+                    "id",
+                    models.BigAutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("title", models.CharField(max_length=200)),
+                ("slug", models.SlugField(blank=True, unique=True)),
+                ("content", models.TextField()),
+                ("date", models.DateTimeField(default=django.utils.timezone.now)),
+                ("modified_date", models.DateTimeField(auto_now=True)),
+                (
+                    "status",
+                    models.CharField(
+                        choices=[("draft", "Draft"), ("published", "Published")],
+                        default="draft",
+                        max_length=10,
+                    ),
+                ),
+                (
+                    "content_type",
+                    models.CharField(
+                        choices=[("post", "Post"), ("page", "Page")],
+                        default="post",
+                        max_length=10,
+                    ),
+                ),
+                (
+                    "author",
+                    models.ForeignKey(
+                        on_delete=django.db.models.deletion.CASCADE,
+                        to=settings.AUTH_USER_MODEL,
+                    ),
+                ),
+                (
+                    "categories",
+                    models.ManyToManyField(blank=True, to="djpress.category"),
+                ),
             ],
             options={
-                'verbose_name': 'post',
-                'verbose_name_plural': 'posts',
+                "verbose_name": "post",
+                "verbose_name_plural": "posts",
             },
         ),
     ]
```

### Comparing `djpress-0.3.1/djpress/models/category.py` & `djpress-0.3.2/djpress/models/category.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/models/post.py` & `djpress-0.3.2/djpress/models/post.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/signals.py` & `djpress-0.3.2/djpress/signals.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/static/djpress/css/style.css` & `djpress-0.3.2/djpress/static/djpress/css/style.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 /* Stylesheet for the DJ Press default template. */
 
 :root {
   --dark0: #2e3440;
-  --dark1-bright: #3b4252;
-  --dark3-bright: #4c566a;
+  --dark1: #3b4252;
+  --dark2: #434c5e;
+  --dark3: #4c566a;
   --light4: #d8dee9;
   --light5: #e5e9f0;
-  --light6-bright: #eceff4;
+  --light6: #eceff4;
   --primary7: #8fbcbb;
   --primary8: #88c0d0;
   --secondary9: #81a1c1;
-  --secondary10: #5e81ac;
-  --danger11: #bf616a;
-  --error12: #d08770;
+  --tertiary10: #5e81ac;
+  --error11: #bf616a;
+  --danger12: #d08770;
   --warning13: #ebcb8b;
   --success14: #a3be8c;
   --info15: #b48ead;
 }
 
 body {
   font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Ubuntu,
-    sans-serif;
+               sans-serif;
   color: var(--dark0);
   margin: 0;
   padding: 0;
   box-sizing: border-box;
   background-color: var(--light5);
 }
 
 /* Top header */
 
 body > header {
-  background-color: var(--dark1-bright);
+  background-color: var(--dark1);
   padding: 1rem;
   padding-left: calc((100% - 992px) / 2);
   padding-right: calc((100% - 992px) / 2);
   display: flex;
   align-items: center;
   justify-content: space-between;
 }
 
 body > header h1 {
   margin: 0;
   font-size: 1.5rem;
 }
 
 body > header h1 a {
-  color: var(--light6-bright);
+  color: var(--light6);
   text-decoration: none;
   padding: 0.5rem 1rem;
 }
 
 body > header ul {
   list-style: none;
   margin: 0;
@@ -59,49 +60,49 @@
 }
 
 body > header ul li {
   margin-left: 1rem;
 }
 
 body > header ul li a {
-  color: var(--light6-bright);
+  color: var(--light6);
   text-decoration: none;
   padding: 0.5rem 1rem;
   border-radius: 0.25rem;
   transition: background-color 0.2s;
 }
 
 body > header ul li a:hover {
-  background-color: var(--dark3-bright);
+  background-color: var(--dark3);
   color: var(--primary8);
 }
 
 /* Main section */
 
 main {
   padding: 2em;
   max-width: 992px;
   margin: 0 auto;
 }
 
 main > h1 {
   font-size: 2rem;
   margin: 0 0.5em 1em;
-  color: var(--dark3-bright);
+  color: var(--dark3);
 }
 /* Articles */
 
 /* General article styles */
 article {
   margin: 0;
   margin-bottom: 2em;
   padding: 2em;
   border: 1px solid var(--light4);
   border-radius: 0.5em;
-  background-color: var(--light6-bright);
+  background-color: var(--light6);
   box-shadow: 0 2px 4px hsl(0deg 0% 0% / 0.1);
 }
 
 /* Article header styles */
 article > header {
   margin-bottom: 1rem;
   border-bottom: 1px solid var(--light4);
@@ -111,26 +112,26 @@
 article > header h1 {
   font-size: 1.75rem;
   margin: 0;
 }
 
 article > header h1 a {
   text-decoration: none;
-  color: var(--secondary10);
+  color: var(--tertiary10);
   transition: color 0.2s;
 }
 
 article > header h1 a:hover {
   color: var(--primary8);
 }
 
 article > header p {
   margin: 0.5em 0;
   font-size: 0.875rem;
-  color: var(--dark3-bright);
+  color: var(--dark3);
 }
 
 /* Article section styles */
 article > section {
   margin-bottom: 1em;
 }
 
@@ -154,38 +155,38 @@
   font-size: 0.875rem;
   margin-right: 0.5em;
   font-weight: bold;
   text-decoration: none;
 }
 
 .badge:hover {
-  background-color: var(--secondary10);
+  background-color: var(--tertiary10);
   color: var(--light4);
 }
 
 /* Footer section */
 
 body > footer {
-  background-color: var(--dark1-bright);
+  background-color: var(--dark1);
   padding: 1rem;
   padding-left: calc((100% - 992px) / 2);
   padding-right: calc((100% - 992px) / 2);
   display: flex;
   align-items: center;
   justify-content: space-between;
   position: fixed;
   bottom: 0;
   width: 100%;
-  color: var(--light6-bright);
+  color: var(--light6);
 }
 
 body > footer p {
   font-size: 1rem;
   margin: 0;
 }
 
 body > footer a {
-  color: var(--light6-bright);
+  color: var(--light6);
 }
 body > footer a:hover {
   color: var(--primary8);
 }
```

### Comparing `djpress-0.3.1/djpress/templates/djpress/index.html` & `djpress-0.3.2/djpress/templates/djpress/index.html`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/templatetags/djpress_tags.py` & `djpress-0.3.2/djpress/templatetags/djpress_tags.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/templatetags/helpers.py` & `djpress-0.3.2/djpress/templatetags/helpers.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/tests/test_category_cache.py` & `djpress-0.3.2/tests/test_category_cache.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/tests/test_djpress_tags.py` & `djpress-0.3.2/tests/test_djpress_tags.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/tests/test_feeds.py` & `djpress-0.3.2/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/tests/test_models.py` & `djpress-0.3.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/tests/test_post_authors.py` & `djpress-0.3.2/tests/test_post_authors.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/tests/test_published_posts_cache.py` & `djpress-0.3.2/tests/test_published_posts_cache.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/tests/test_views.py` & `djpress-0.3.2/tests/test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     post = Post.post_objects.create(
         title="Test Post",
         slug="test-post",
         content="This is a test post.",
         author=user,
         status="published",
         post_type="post",
-        date=timezone.datetime(2024, 1, 1),
+        date=timezone.make_aware(timezone.datetime(2024, 1, 1)),
     )
     post.categories.set([category])
     return post
 
 
 @pytest.mark.django_db
 def test_index_view(client):
```

### Comparing `djpress-0.3.1/djpress/urls.py` & `djpress-0.3.2/djpress/urls.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/utils.py` & `djpress-0.3.2/djpress/utils.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress/views.py` & `djpress-0.3.2/djpress/views.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.1/djpress.egg-info/PKG-INFO` & `djpress-0.3.2/djpress.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpress
-Version: 0.3.1
+Version: 0.3.2
 Summary: A blog application for Django sites, inspired by classic WordPress.
 Author-email: Stuart Maxwell <stuart@amanzi.nz>
 License: MIT License
         
         Copyright (c) 2024 Stuart Maxwell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,14 +45,20 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django
 Requires-Dist: markdown
+Requires-Dist: pygments
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-django; extra == "tests"
+Provides-Extra: linting
+Requires-Dist: ruff; extra == "linting"
 
 # DJ Press
 
 A blog application for Django sites, inspired by classic WordPress.
 
 > Warning - very alpha.
```

