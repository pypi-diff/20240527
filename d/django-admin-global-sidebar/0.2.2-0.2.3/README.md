# Comparing `tmp/django-admin-global-sidebar-0.2.2.tar.gz` & `tmp/django-admin-global-sidebar-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-global-sidebar-0.2.2.tar", last modified: Wed Sep 13 06:46:04 2023, max compression
+gzip compressed data, was "django-admin-global-sidebar-0.2.3.tar", last modified: Mon May 27 08:36:13 2024, max compression
```

## Comparing `django-admin-global-sidebar-0.2.2.tar` & `django-admin-global-sidebar-0.2.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 06:46:04.975375 django-admin-global-sidebar-0.2.2/
--rw-r--r--   0 test       (501) staff       (20)     1067 2022-12-16 04:29:20.000000 django-admin-global-sidebar-0.2.2/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      271 2023-09-13 06:36:39.000000 django-admin-global-sidebar-0.2.2/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     7108 2023-09-13 06:46:04.975196 django-admin-global-sidebar-0.2.2/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     6383 2023-09-13 06:44:57.000000 django-admin-global-sidebar-0.2.2/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 06:46:04.972218 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/
--rw-r--r--   0 test       (501) staff       (20)       87 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       66 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/admin.py
--rw-r--r--   0 test       (501) staff       (20)      131 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 06:46:04.973396 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       60 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/models.py
--rw-r--r--   0 test       (501) staff       (20)      316 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/settings.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 06:46:04.969375 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/static/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 06:46:04.969474 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/static/django-admin-global-sidebar/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 06:46:04.973507 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/static/django-admin-global-sidebar/css/
--rw-r--r--   0 test       (501) staff       (20)     4094 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/static/django-admin-global-sidebar/css/django-admin-global-sidebar.css
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 06:46:04.973690 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/static/django-admin-global-sidebar/js/
--rw-r--r--   0 test       (501) staff       (20)     4402 2022-12-16 04:20:57.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/static/django-admin-global-sidebar/js/django-admin-global-sidebar.js
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 06:46:04.969571 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/templates/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 06:46:04.974689 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/templates/admin/
--rw-r--r--   0 test       (501) staff       (20)       76 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/templates/admin/base.html
--rw-r--r--   0 test       (501) staff       (20)     1081 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/templates/admin/base_site.html
--rw-r--r--   0 test       (501) staff       (20)     1558 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/templates/admin/django-admin-global-sidebar.html
--rw-r--r--   0 test       (501) staff       (20)      154 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/templates/admin/login.html
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 06:46:04.974945 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/templatetags/
--rw-r--r--   0 test       (501) staff       (20)        0 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/templatetags/__init__.py
--rw-r--r--   0 test       (501) staff       (20)     2335 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/templatetags/django_admin_global_sidebar.py
--rw-r--r--   0 test       (501) staff       (20)       63 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/tests.py
--rw-r--r--   0 test       (501) staff       (20)     3058 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/utils.py
--rw-r--r--   0 test       (501) staff       (20)       66 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-09-13 06:46:04.973221 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     7108 2023-09-13 06:46:04.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     1278 2023-09-13 06:46:04.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-13 06:46:04.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-09-13 06:46:04.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       75 2023-09-13 06:46:04.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       28 2023-09-13 06:46:04.000000 django-admin-global-sidebar-0.2.2/django_admin_global_sidebar.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)       79 2023-09-13 06:45:41.000000 django-admin-global-sidebar-0.2.2/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2023-09-13 06:46:04.975530 django-admin-global-sidebar-0.2.2/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1573 2023-09-13 06:37:13.000000 django-admin-global-sidebar-0.2.2/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 08:36:13.751618 django-admin-global-sidebar-0.2.3/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-27 08:35:22.000000 django-admin-global-sidebar-0.2.3/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      271 2023-09-13 06:36:39.000000 django-admin-global-sidebar-0.2.3/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     7168 2024-05-27 08:36:13.751490 django-admin-global-sidebar-0.2.3/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     6476 2024-05-27 08:34:59.000000 django-admin-global-sidebar-0.2.3/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 08:36:13.749561 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/
+-rw-r--r--   0 test       (501) staff       (20)       87 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       66 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      131 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 08:36:13.750365 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       60 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/models.py
+-rw-r--r--   0 test       (501) staff       (20)      316 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/settings.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 08:36:13.747580 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/static/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 08:36:13.747697 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/static/django-admin-global-sidebar/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 08:36:13.750466 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/static/django-admin-global-sidebar/css/
+-rw-r--r--   0 test       (501) staff       (20)     4094 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/static/django-admin-global-sidebar/css/django-admin-global-sidebar.css
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 08:36:13.750587 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/static/django-admin-global-sidebar/js/
+-rw-r--r--   0 test       (501) staff       (20)     4402 2022-12-16 04:20:57.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/static/django-admin-global-sidebar/js/django-admin-global-sidebar.js
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 08:36:13.747816 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/templates/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 08:36:13.751073 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/templates/admin/
+-rw-r--r--   0 test       (501) staff       (20)       76 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/templates/admin/base.html
+-rw-r--r--   0 test       (501) staff       (20)     1081 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/templates/admin/base_site.html
+-rw-r--r--   0 test       (501) staff       (20)     1558 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/templates/admin/django-admin-global-sidebar.html
+-rw-r--r--   0 test       (501) staff       (20)      154 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/templates/admin/login.html
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 08:36:13.751285 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/templatetags/
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/templatetags/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     2335 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/templatetags/django_admin_global_sidebar.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/tests.py
+-rw-r--r--   0 test       (501) staff       (20)     3130 2024-05-27 08:33:08.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/utils.py
+-rw-r--r--   0 test       (501) staff       (20)       66 2022-12-16 04:20:22.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-27 08:36:13.750256 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     7168 2024-05-27 08:36:13.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     1278 2024-05-27 08:36:13.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-27 08:36:13.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-27 08:36:13.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       75 2024-05-27 08:36:13.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       28 2024-05-27 08:36:13.000000 django-admin-global-sidebar-0.2.3/django_admin_global_sidebar.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)       79 2023-09-13 06:45:41.000000 django-admin-global-sidebar-0.2.3/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-27 08:36:13.751662 django-admin-global-sidebar-0.2.3/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1489 2024-05-27 08:35:14.000000 django-admin-global-sidebar-0.2.3/setup.py
```

### Comparing `django-admin-global-sidebar-0.2.2/LICENSE` & `django-admin-global-sidebar-0.2.3/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 MIT License
 
-Copyright (c) 2020 zencore.cn
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django-admin-global-sidebar-0.2.2/PKG-INFO` & `django-admin-global-sidebar-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-admin-global-sidebar
-Version: 0.2.2
+Version: 0.2.3
 Summary: Provides a configurable left navigation bar for Django's admin site.
+Home-page: UNKNOWN
 Author: Li HaoRan
-Author-email: lihaoran@zencore.cn
 Maintainer: Li HaoRan
-Maintainer-email: lihaoran@zencore.cn
 License: MIT
 Keywords: django admin extentions,django admin global admin
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -208,7 +208,13 @@
 ### v0.2.1
 
 - Fix sidebar height.
 
 ### v0.2.2
 
 - Doc update.
+
+### v0.2.3
+
+- 修正1级菜单children字段缺失导致的大量DEBUG异常输出问题。
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-admin-global-sidebar-0.2.2/README.md` & `django-admin-global-sidebar-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -189,7 +189,11 @@
 ### v0.2.1
 
 - Fix sidebar height.
 
 ### v0.2.2
 
 - Doc update.
+
+### v0.2.3
+
+- 修正1级菜单children字段缺失导致的大量DEBUG异常输出问题。
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/static/django-admin-global-sidebar/css/django-admin-global-sidebar.css` & `django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/static/django-admin-global-sidebar/css/django-admin-global-sidebar.css`

 * *Files identical despite different names*

### Comparing `django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/static/django-admin-global-sidebar/js/django-admin-global-sidebar.js` & `django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/static/django-admin-global-sidebar/js/django-admin-global-sidebar.js`

 * *Files identical despite different names*

### Comparing `django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/templates/admin/base_site.html` & `django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/templates/admin/django-admin-global-sidebar.html` & `django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/templates/admin/django-admin-global-sidebar.html`

 * *Files identical despite different names*

### Comparing `django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/templatetags/django_admin_global_sidebar.py` & `django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/templatetags/django_admin_global_sidebar.py`

 * *Files identical despite different names*

### Comparing `django-admin-global-sidebar-0.2.2/django_admin_global_sidebar/utils.py` & `django-admin-global-sidebar-0.2.3/django_admin_global_sidebar/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,45 +3,50 @@
 import hashlib
 
 import magic_import
 
 from django.urls import reverse
 from .settings import DJANGO_ADMIN_GLOBAL_SIDEBAR_MENUS
 
+
 def has_menu_permissions(user, menu):
     if not "permissions" in menu:
         return True
     for permissions in menu["permissions"]:
         if isinstance(permissions, str):
             permissions = [permissions]
         if user.has_perms(permissions):
             return True
     return False
 
+
 def get_menu_url(menu):
     if "url" in menu:
         return menu["url"]
     elif "model" in menu:
         app_label, model_name = menu["model"].split(".")
         return reverse("admin:{}_{}_changelist".format(app_label, model_name))
     elif "view" in menu:
         view_name = menu["view"]
         return reverse(view_name)
     else:
         return ""
 
+
 def _fix_menu_id(menu):
     if not "id" in menu:
         menu["id"] = "id" + hashlib.md5(menu["title"].encode("utf-8")).hexdigest()
     return menu["id"]
 
+
 def _fix_menu_url(menu):
     menu["url"] = get_menu_url(menu)
     return menu["url"]
 
+
 def _fix_menu_active(menu, request):
     active_patterns = menu.get("active_patterns")
     if not active_patterns:
         if "model" in menu:
             active_patterns = "^(" + menu["url"] + ".*)$"
         else:
             active_patterns = "^" + menu["url"] + "$"
@@ -50,33 +55,37 @@
     menu["active"] = False
     for active_pattern in active_patterns:
         if re.match(active_pattern, request.path):
             menu["active"] = True
             break
     return menu["active"]
 
+
 def get_user_menus(request):
     menus = []
 
     menus_settings = []
     if isinstance(DJANGO_ADMIN_GLOBAL_SIDEBAR_MENUS, str):
-        menus_loader = magic_import.import_from_string(DJANGO_ADMIN_GLOBAL_SIDEBAR_MENUS)
+        menus_loader = magic_import.import_from_string(
+            DJANGO_ADMIN_GLOBAL_SIDEBAR_MENUS
+        )
         if callable(menus_loader):
             menus_settings = menus_loader(request)
         else:
             menus_settings = menus_loader
     else:
         menus_settings = DJANGO_ADMIN_GLOBAL_SIDEBAR_MENUS
 
     menus_settings = copy.deepcopy(menus_settings)
     for menu1 in menus_settings:
         _fix_menu_id(menu1)
         _fix_menu_url(menu1)
         _fix_menu_active(menu1, request)
         if not "children" in menu1:
+            menu1["children"] = []
             if has_menu_permissions(request.user, menu1):
                 menus.append(menu1)
         else:
             children = []
             active_flag = False
             for menu2 in menu1["children"]:
                 if has_menu_permissions(request.user, menu2):
```

### Comparing `django-admin-global-sidebar-0.2.2/django_admin_global_sidebar.egg-info/PKG-INFO` & `django-admin-global-sidebar-0.2.3/django_admin_global_sidebar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-admin-global-sidebar
-Version: 0.2.2
+Version: 0.2.3
 Summary: Provides a configurable left navigation bar for Django's admin site.
+Home-page: UNKNOWN
 Author: Li HaoRan
-Author-email: lihaoran@zencore.cn
 Maintainer: Li HaoRan
-Maintainer-email: lihaoran@zencore.cn
 License: MIT
 Keywords: django admin extentions,django admin global admin
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -208,7 +208,13 @@
 ### v0.2.1
 
 - Fix sidebar height.
 
 ### v0.2.2
 
 - Doc update.
+
+### v0.2.3
+
+- 修正1级菜单children字段缺失导致的大量DEBUG异常输出问题。
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-admin-global-sidebar-0.2.2/django_admin_global_sidebar.egg-info/SOURCES.txt` & `django-admin-global-sidebar-0.2.3/django_admin_global_sidebar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-global-sidebar-0.2.2/setup.py` & `django-admin-global-sidebar-0.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,22 +10,20 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="django-admin-global-sidebar",
-    version="0.2.2",
+    version="0.2.3",
     description="Provides a configurable left navigation bar for Django's admin site.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Li HaoRan",
-    author_email="lihaoran@zencore.cn",
     maintainer="Li HaoRan",
-    maintainer_email="lihaoran@zencore.cn",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

