# Comparing `tmp/django-admin-console-0.1.2.tar.gz` & `tmp/django-admin-console-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-console-0.1.2.tar", last modified: Sat May 25 11:12:07 2024, max compression
+gzip compressed data, was "django-admin-console-0.1.3.tar", last modified: Mon May 27 03:39:04 2024, max compression
```

## Comparing `django-admin-console-0.1.2.tar` & `django-admin-console-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-25 11:12:07.136965 django-admin-console-0.1.2/
--rw-r--r--   0 peter      (501) staff       (20)    26526 2024-05-25 11:04:04.000000 django-admin-console-0.1.2/LICENSE
--rw-r--r--   0 peter      (501) staff       (20)      273 2024-05-25 11:04:04.000000 django-admin-console-0.1.2/MANIFEST.in
--rw-r--r--   0 peter      (501) staff       (20)      391 2024-05-25 11:12:07.136752 django-admin-console-0.1.2/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)       34 2024-05-25 11:04:04.000000 django-admin-console-0.1.2/README.md
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-25 11:12:07.122163 django-admin-console-0.1.2/django_admin_console.egg-info/
--rw-r--r--   0 peter      (501) staff       (20)      391 2024-05-25 11:12:07.000000 django-admin-console-0.1.2/django_admin_console.egg-info/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)     1134 2024-05-25 11:12:07.000000 django-admin-console-0.1.2/django_admin_console.egg-info/SOURCES.txt
--rw-r--r--   0 peter      (501) staff       (20)        1 2024-05-25 11:12:07.000000 django-admin-console-0.1.2/django_admin_console.egg-info/dependency_links.txt
--rw-r--r--   0 peter      (501) staff       (20)       12 2024-05-25 11:12:07.000000 django-admin-console-0.1.2/django_admin_console.egg-info/requires.txt
--rw-r--r--   0 peter      (501) staff       (20)       12 2024-05-25 11:12:07.000000 django-admin-console-0.1.2/django_admin_console.egg-info/top_level.txt
--rw-r--r--   0 peter      (501) staff       (20)       38 2024-05-25 11:12:07.137021 django-admin-console-0.1.2/setup.cfg
--rw-r--r--   0 peter      (501) staff       (20)      715 2024-05-25 11:11:56.000000 django-admin-console-0.1.2/setup.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-25 11:12:07.124370 django-admin-console-0.1.2/web_console/
--rw-r--r--   0 peter      (501) staff       (20)        0 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)       63 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/admin.py
--rw-r--r--   0 peter      (501) staff       (20)      153 2024-05-25 10:53:51.000000 django-admin-console-0.1.2/web_console/apps.py
--rw-r--r--   0 peter      (501) staff       (20)       57 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/models.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-25 11:12:07.119237 django-admin-console-0.1.2/web_console/static/
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-25 11:12:07.119460 django-admin-console-0.1.2/web_console/static/console/
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-25 11:12:07.125218 django-admin-console-0.1.2/web_console/static/console/css/
--rw-r--r--   0 peter      (501) staff       (20)      179 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/static/console/css/console.css
--rw-r--r--   0 peter      (501) staff       (20)    19098 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/static/console/css/miniAdmin.css
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-25 11:12:07.125971 django-admin-console-0.1.2/web_console/static/console/img/
--rw-r--r--   0 peter      (501) staff       (20)    76190 2023-07-03 13:36:04.000000 django-admin-console-0.1.2/web_console/static/console/img/logo.png
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-25 11:12:07.127361 django-admin-console-0.1.2/web_console/static/console/js/
--rw-r--r--   0 peter      (501) staff       (20)      835 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/static/console/js/console.js
--rw-r--r--   0 peter      (501) staff       (20)    39769 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/static/console/js/miniAdmin.js
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-25 11:12:07.127606 django-admin-console-0.1.2/web_console/static/console/layui/
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-25 11:12:07.129830 django-admin-console-0.1.2/web_console/static/console/layui/css/
--rw-r--r--   0 peter      (501) staff       (20)   124905 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/static/console/layui/css/layui.css
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-25 11:12:07.132151 django-admin-console-0.1.2/web_console/static/console/layui/font/
--rw-r--r--   0 peter      (501) staff       (20)    54172 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/static/console/layui/font/iconfont.eot
--rw-r--r--   0 peter      (501) staff       (20)   330645 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/static/console/layui/font/iconfont.svg
--rw-r--r--   0 peter      (501) staff       (20)    53996 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/static/console/layui/font/iconfont.ttf
--rw-r--r--   0 peter      (501) staff       (20)    34624 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/static/console/layui/font/iconfont.woff
--rw-r--r--   0 peter      (501) staff       (20)    29736 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/static/console/layui/font/iconfont.woff2
--rw-r--r--   0 peter      (501) staff       (20)   360497 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/static/console/layui/layui.js
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-25 11:12:07.119702 django-admin-console-0.1.2/web_console/templates/
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-25 11:12:07.136226 django-admin-console-0.1.2/web_console/templates/console/
--rw-r--r--   0 peter      (501) staff       (20)      989 2024-05-24 15:14:01.000000 django-admin-console-0.1.2/web_console/templates/console/frame_base.html
--rw-r--r--   0 peter      (501) staff       (20)     2735 2024-05-24 15:17:34.000000 django-admin-console-0.1.2/web_console/templates/console/home.html
--rw-r--r--   0 peter      (501) staff       (20)     8160 2024-05-24 15:07:12.000000 django-admin-console-0.1.2/web_console/templates/console/layout.html
--rw-r--r--   0 peter      (501) staff       (20)     5022 2024-05-24 15:27:27.000000 django-admin-console-0.1.2/web_console/templates/console/login.html
--rw-r--r--   0 peter      (501) staff       (20)       60 2024-05-24 14:54:01.000000 django-admin-console-0.1.2/web_console/tests.py
--rw-r--r--   0 peter      (501) staff       (20)      399 2024-05-24 15:27:28.000000 django-admin-console-0.1.2/web_console/urls.py
--rw-r--r--   0 peter      (501) staff       (20)     1426 2024-05-24 15:37:13.000000 django-admin-console-0.1.2/web_console/views.py
+drwxr-xr-x   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:39:04.260000 django-admin-console-0.1.3/
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)     1108 2024-05-27 03:24:51.000000 django-admin-console-0.1.3/LICENSE.txt
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)      279 2024-05-27 03:24:51.000000 django-admin-console-0.1.3/MANIFEST.in
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)      395 2024-05-27 03:39:04.259586 django-admin-console-0.1.3/PKG-INFO
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)       59 2024-05-27 03:38:46.000000 django-admin-console-0.1.3/README.md
+drwxr-xr-x   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:39:04.231726 django-admin-console-0.1.3/admin_console/
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:14:04.000000 django-admin-console-0.1.3/admin_console/__init__.py
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)       63 2024-05-27 03:14:04.000000 django-admin-console-0.1.3/admin_console/admin.py
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)      157 2024-05-27 03:14:05.000000 django-admin-console-0.1.3/admin_console/apps.py
+drwxr-xr-x   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:39:04.232839 django-admin-console-0.1.3/admin_console/migrations/
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:14:04.000000 django-admin-console-0.1.3/admin_console/migrations/__init__.py
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)       57 2024-05-27 03:14:04.000000 django-admin-console-0.1.3/admin_console/models.py
+drwxr-xr-x   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:39:04.219626 django-admin-console-0.1.3/admin_console/static/
+drwxr-xr-x   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:39:04.221114 django-admin-console-0.1.3/admin_console/static/console/
+drwxr-xr-x   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:39:04.234457 django-admin-console-0.1.3/admin_console/static/console/css/
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)      179 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/static/console/css/console.css
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)    19098 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/static/console/css/miniAdmin.css
+drwxr-xr-x   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:39:04.235730 django-admin-console-0.1.3/admin_console/static/console/img/
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)    76190 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/static/console/img/logo.png
+drwxr-xr-x   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:39:04.237718 django-admin-console-0.1.3/admin_console/static/console/js/
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)      835 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/static/console/js/console.js
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)    39769 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/static/console/js/miniAdmin.js
+drwxr-xr-x   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:39:04.238940 django-admin-console-0.1.3/admin_console/static/console/layui/
+drwxr-xr-x   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:39:04.241938 django-admin-console-0.1.3/admin_console/static/console/layui/css/
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)   124905 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/static/console/layui/css/layui.css
+drwxr-xr-x   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:39:04.250517 django-admin-console-0.1.3/admin_console/static/console/layui/font/
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)    54172 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/static/console/layui/font/iconfont.eot
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)   330645 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/static/console/layui/font/iconfont.svg
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)    53996 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/static/console/layui/font/iconfont.ttf
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)    34624 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/static/console/layui/font/iconfont.woff
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)    29736 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/static/console/layui/font/iconfont.woff2
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)   360497 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/static/console/layui/layui.js
+drwxr-xr-x   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:39:04.222331 django-admin-console-0.1.3/admin_console/templates/
+drwxr-xr-x   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:39:04.254613 django-admin-console-0.1.3/admin_console/templates/console/
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)      989 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/templates/console/frame_base.html
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)     2735 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/templates/console/home.html
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)     8160 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/templates/console/layout.html
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)     5022 2024-05-27 01:37:09.000000 django-admin-console-0.1.3/admin_console/templates/console/login.html
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)       60 2024-05-27 03:14:04.000000 django-admin-console-0.1.3/admin_console/tests.py
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)      399 2024-05-27 03:29:28.000000 django-admin-console-0.1.3/admin_console/urls.py
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)     1426 2024-05-27 03:29:28.000000 django-admin-console-0.1.3/admin_console/views.py
+drwxr-xr-x   0 yuhua.yang   (510) staff       (20)        0 2024-05-27 03:39:04.258471 django-admin-console-0.1.3/django_admin_console.egg-info/
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)      395 2024-05-27 03:39:04.000000 django-admin-console-0.1.3/django_admin_console.egg-info/PKG-INFO
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)     1221 2024-05-27 03:39:04.000000 django-admin-console-0.1.3/django_admin_console.egg-info/SOURCES.txt
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)        1 2024-05-27 03:39:04.000000 django-admin-console-0.1.3/django_admin_console.egg-info/dependency_links.txt
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)       12 2024-05-27 03:39:04.000000 django-admin-console-0.1.3/django_admin_console.egg-info/requires.txt
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)       14 2024-05-27 03:39:04.000000 django-admin-console-0.1.3/django_admin_console.egg-info/top_level.txt
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)       38 2024-05-27 03:39:04.260181 django-admin-console-0.1.3/setup.cfg
+-rw-r--r--   0 yuhua.yang   (510) staff       (20)      719 2024-05-27 03:24:51.000000 django-admin-console-0.1.3/setup.py
```

### Comparing `django-admin-console-0.1.2/django_admin_console.egg-info/SOURCES.txt` & `django-admin-console-0.1.3/django_admin_console.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-LICENSE
+LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
+admin_console/__init__.py
+admin_console/admin.py
+admin_console/apps.py
+admin_console/models.py
+admin_console/tests.py
+admin_console/urls.py
+admin_console/views.py
+admin_console/migrations/__init__.py
+admin_console/static/console/css/console.css
+admin_console/static/console/css/miniAdmin.css
+admin_console/static/console/img/logo.png
+admin_console/static/console/js/console.js
+admin_console/static/console/js/miniAdmin.js
+admin_console/static/console/layui/layui.js
+admin_console/static/console/layui/css/layui.css
+admin_console/static/console/layui/font/iconfont.eot
+admin_console/static/console/layui/font/iconfont.svg
+admin_console/static/console/layui/font/iconfont.ttf
+admin_console/static/console/layui/font/iconfont.woff
+admin_console/static/console/layui/font/iconfont.woff2
+admin_console/templates/console/frame_base.html
+admin_console/templates/console/home.html
+admin_console/templates/console/layout.html
+admin_console/templates/console/login.html
 django_admin_console.egg-info/PKG-INFO
 django_admin_console.egg-info/SOURCES.txt
 django_admin_console.egg-info/dependency_links.txt
 django_admin_console.egg-info/requires.txt
-django_admin_console.egg-info/top_level.txt
-web_console/__init__.py
-web_console/admin.py
-web_console/apps.py
-web_console/models.py
-web_console/tests.py
-web_console/urls.py
-web_console/views.py
-web_console/static/console/css/console.css
-web_console/static/console/css/miniAdmin.css
-web_console/static/console/img/logo.png
-web_console/static/console/js/console.js
-web_console/static/console/js/miniAdmin.js
-web_console/static/console/layui/layui.js
-web_console/static/console/layui/css/layui.css
-web_console/static/console/layui/font/iconfont.eot
-web_console/static/console/layui/font/iconfont.svg
-web_console/static/console/layui/font/iconfont.ttf
-web_console/static/console/layui/font/iconfont.woff
-web_console/static/console/layui/font/iconfont.woff2
-web_console/templates/console/frame_base.html
-web_console/templates/console/home.html
-web_console/templates/console/layout.html
-web_console/templates/console/login.html
+django_admin_console.egg-info/top_level.txt
```

### Comparing `django-admin-console-0.1.2/web_console/static/console/css/miniAdmin.css` & `django-admin-console-0.1.3/admin_console/static/console/css/miniAdmin.css`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/static/console/img/logo.png` & `django-admin-console-0.1.3/admin_console/static/console/img/logo.png`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/static/console/js/console.js` & `django-admin-console-0.1.3/admin_console/static/console/js/console.js`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/static/console/js/miniAdmin.js` & `django-admin-console-0.1.3/admin_console/static/console/js/miniAdmin.js`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/static/console/layui/css/layui.css` & `django-admin-console-0.1.3/admin_console/static/console/layui/css/layui.css`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/static/console/layui/font/iconfont.eot` & `django-admin-console-0.1.3/admin_console/static/console/layui/font/iconfont.eot`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/static/console/layui/font/iconfont.svg` & `django-admin-console-0.1.3/admin_console/static/console/layui/font/iconfont.svg`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/static/console/layui/font/iconfont.ttf` & `django-admin-console-0.1.3/admin_console/static/console/layui/font/iconfont.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/static/console/layui/font/iconfont.woff` & `django-admin-console-0.1.3/admin_console/static/console/layui/font/iconfont.woff`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/static/console/layui/font/iconfont.woff2` & `django-admin-console-0.1.3/admin_console/static/console/layui/font/iconfont.woff2`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/static/console/layui/layui.js` & `django-admin-console-0.1.3/admin_console/static/console/layui/layui.js`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/templates/console/frame_base.html` & `django-admin-console-0.1.3/admin_console/templates/console/frame_base.html`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/templates/console/home.html` & `django-admin-console-0.1.3/admin_console/templates/console/home.html`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/templates/console/layout.html` & `django-admin-console-0.1.3/admin_console/templates/console/layout.html`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/templates/console/login.html` & `django-admin-console-0.1.3/admin_console/templates/console/login.html`

 * *Files identical despite different names*

### Comparing `django-admin-console-0.1.2/web_console/views.py` & `django-admin-console-0.1.3/admin_console/views.py`

 * *Files identical despite different names*

