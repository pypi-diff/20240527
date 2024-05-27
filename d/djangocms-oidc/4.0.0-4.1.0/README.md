# Comparing `tmp/djangocms-oidc-4.0.0.tar.gz` & `tmp/djangocms_oidc-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-oidc-4.0.0.tar", last modified: Tue Sep 26 14:30:19 2023, max compression
+gzip compressed data, was "djangocms_oidc-4.1.0.tar", last modified: Mon May 27 12:55:53 2024, max compression
```

## Comparing `djangocms-oidc-4.0.0.tar` & `djangocms_oidc-4.1.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-09-26 14:30:19.567317 djangocms-oidc-4.0.0/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    35147 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/LICENSE
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      151 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/MANIFEST.in
--rw-r--r--   0 zbohm     (1000) zbohm     (1000)     7342 2023-09-26 14:30:19.567317 djangocms-oidc-4.0.0/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5913 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/README.rst
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-09-26 14:30:19.563316 djangocms-oidc-4.0.0/djangocms_oidc/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/__init__.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-09-26 14:30:19.563316 djangocms-oidc-4.0.0/djangocms_oidc/admin/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      373 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/admin/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      638 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/admin/forms.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      413 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/admin/options.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    13210 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/auth.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4530 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/cms_plugins.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      114 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/constants.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      441 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/forms.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2637 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/helpers.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-09-26 14:30:19.563316 djangocms-oidc-4.0.0/djangocms_oidc/locale/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-09-26 14:30:19.563316 djangocms-oidc-4.0.0/djangocms_oidc/locale/cs/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-09-26 14:30:19.563316 djangocms-oidc-4.0.0/djangocms_oidc/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11763 2023-09-26 13:50:18.000000 djangocms-oidc-4.0.0/djangocms_oidc/locale/cs/LC_MESSAGES/django.mo
--rw-------   0 zbohm     (1000) zbohm     (1000)    12113 2023-09-26 13:49:16.000000 djangocms-oidc-4.0.0/djangocms_oidc/locale/cs/LC_MESSAGES/django.po
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3511 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/middleware.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-09-26 14:30:19.563316 djangocms-oidc-4.0.0/djangocms_oidc/migrations/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     9263 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/migrations/0001_initial.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2225 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/migrations/0002_30274_button_label.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/migrations/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    12157 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/models.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-09-26 14:30:19.563316 djangocms-oidc-4.0.0/djangocms_oidc/templates/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-09-26 14:30:19.567317 djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-09-26 14:30:19.567317 djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/change_form/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2437 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/change_form/consumer.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      290 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/change_form/display_dedicated_content.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      386 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/change_form/list_identifiers.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      274 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/display_dedicated_content.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3515 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/handover_data.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      985 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/list_identifiers.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5291 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/login.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      128 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/show_attribute.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      236 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/show_attribute_country.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-09-26 14:30:19.567317 djangocms-oidc-4.0.0/djangocms_oidc/tests/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/tests/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2455 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/tests/settings.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2072 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/tests/test_admin_forms.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      538 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/tests/test_admin_options.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    27955 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/tests/test_auth.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    32505 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/tests/test_cms_plugins.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      878 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/tests/test_forms.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5665 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/tests/test_helpers.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    18721 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/tests/test_middleware.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11065 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/tests/test_models.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3726 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/tests/test_utils.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    20601 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/tests/test_views.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      698 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/tests/urls.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      432 2023-09-21 10:48:41.000000 djangocms-oidc-4.0.0/djangocms_oidc/tests/views.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1250 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/urls.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1525 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/utils.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8560 2023-09-26 14:06:01.000000 djangocms-oidc-4.0.0/djangocms_oidc/views.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-09-26 14:30:19.563316 djangocms-oidc-4.0.0/djangocms_oidc.egg-info/
--rw-r--r--   0 zbohm     (1000) zbohm     (1000)     7342 2023-09-26 14:30:19.000000 djangocms-oidc-4.0.0/djangocms_oidc.egg-info/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1976 2023-09-26 14:30:19.000000 djangocms-oidc-4.0.0/djangocms_oidc.egg-info/SOURCES.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-09-26 14:30:19.000000 djangocms-oidc-4.0.0/djangocms_oidc.egg-info/dependency_links.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-09-21 11:06:46.000000 djangocms-oidc-4.0.0/djangocms_oidc.egg-info/not-zip-safe
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      144 2023-09-26 14:30:19.000000 djangocms-oidc-4.0.0/djangocms_oidc.egg-info/requires.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       15 2023-09-26 14:30:19.000000 djangocms-oidc-4.0.0/djangocms_oidc.egg-info/top_level.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      380 2023-09-26 14:30:19.567317 djangocms-oidc-4.0.0/setup.cfg
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1791 2023-09-26 14:29:43.000000 djangocms-oidc-4.0.0/setup.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.487322 djangocms_oidc-4.1.0/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    35147 2020-09-17 12:54:57.000000 djangocms_oidc-4.1.0/LICENSE
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      151 2020-09-17 12:54:57.000000 djangocms_oidc-4.1.0/MANIFEST.in
+-rw-r--r--   0 zbohm     (1000) zbohm     (1000)     7342 2024-05-27 12:55:53.487322 djangocms_oidc-4.1.0/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5913 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/README.rst
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.479323 djangocms_oidc-4.1.0/djangocms_oidc/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/__init__.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.483322 djangocms_oidc-4.1.0/djangocms_oidc/admin/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      373 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/admin/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      638 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/admin/forms.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      413 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/admin/options.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    13210 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/auth.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4584 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.0/djangocms_oidc/cms_plugins.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      114 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/constants.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      701 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.0/djangocms_oidc/forms.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2637 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/helpers.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.479323 djangocms_oidc-4.1.0/djangocms_oidc/locale/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.479323 djangocms_oidc-4.1.0/djangocms_oidc/locale/cs/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.483322 djangocms_oidc-4.1.0/djangocms_oidc/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    12113 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/locale/cs/LC_MESSAGES/django.po
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3511 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/middleware.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.483322 djangocms_oidc-4.1.0/djangocms_oidc/migrations/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     9263 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/migrations/0001_initial.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2225 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/migrations/0002_30274_button_label.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/migrations/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    12191 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.0/djangocms_oidc/models.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.479323 djangocms_oidc-4.1.0/djangocms_oidc/templates/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.483322 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.483322 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/change_form/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3006 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/change_form/consumer.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      290 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/change_form/display_dedicated_content.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      386 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/change_form/list_identifiers.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      274 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/display_dedicated_content.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3515 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/handover_data.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      985 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/list_identifiers.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5291 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/login.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      128 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/show_attribute.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      236 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/show_attribute_country.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.483322 djangocms_oidc-4.1.0/djangocms_oidc/tests/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2455 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/settings.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2072 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_admin_forms.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      538 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_admin_options.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    27955 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_auth.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    32505 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_cms_plugins.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      878 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_forms.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5665 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_helpers.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    18721 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_middleware.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11065 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_models.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3726 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_utils.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    20601 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_views.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1126 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/test_widgets.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      698 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/urls.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      432 2022-02-14 12:58:55.000000 djangocms_oidc-4.1.0/djangocms_oidc/tests/views.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1250 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/urls.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1525 2024-04-23 07:16:24.000000 djangocms_oidc-4.1.0/djangocms_oidc/utils.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8560 2024-04-24 10:59:39.000000 djangocms_oidc-4.1.0/djangocms_oidc/views.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      482 2024-05-27 12:52:20.000000 djangocms_oidc-4.1.0/djangocms_oidc/widgets.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2024-05-27 12:55:53.483322 djangocms_oidc-4.1.0/djangocms_oidc.egg-info/
+-rw-r--r--   0 zbohm     (1000) zbohm     (1000)     7342 2024-05-27 12:55:53.000000 djangocms_oidc-4.1.0/djangocms_oidc.egg-info/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1992 2024-05-27 12:55:53.000000 djangocms_oidc-4.1.0/djangocms_oidc.egg-info/SOURCES.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2024-05-27 12:55:53.000000 djangocms_oidc-4.1.0/djangocms_oidc.egg-info/dependency_links.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2022-02-14 14:49:42.000000 djangocms_oidc-4.1.0/djangocms_oidc.egg-info/not-zip-safe
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      144 2024-05-27 12:55:53.000000 djangocms_oidc-4.1.0/djangocms_oidc.egg-info/requires.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       15 2024-05-27 12:55:53.000000 djangocms_oidc-4.1.0/djangocms_oidc.egg-info/top_level.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      380 2024-05-27 12:55:53.487322 djangocms_oidc-4.1.0/setup.cfg
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1791 2024-05-27 12:55:31.000000 djangocms_oidc-4.1.0/setup.py
```

### Comparing `djangocms-oidc-4.0.0/LICENSE` & `djangocms_oidc-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/PKG-INFO` & `djangocms_oidc-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-oidc
-Version: 4.0.0
+Version: 4.1.0
 Summary: Plugin OIDC (OpenID Connect) into Django CMS.
 Home-page: https://github.com/CZ-NIC/djangocms-oidc
 Author: Zdeněk Böhm
 Author-email: zdenek.bohm@nic.cz
 License: GPL GNU License
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `djangocms-oidc-4.0.0/README.rst` & `djangocms_oidc-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/admin/forms.py` & `djangocms_oidc-4.1.0/djangocms_oidc/admin/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/auth.py` & `djangocms_oidc-4.1.0/djangocms_oidc/auth.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/cms_plugins.py` & `djangocms_oidc-4.1.0/djangocms_oidc/cms_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from cms.plugin_base import CMSPluginBase
 from cms.plugin_pool import plugin_pool
 from django.utils.translation import gettext_lazy as _
 
 from .constants import DJANGOCMS_USER_SESSION_KEY
-from .forms import OIDCDataForm
+from .forms import OIDCDataForm, OIDCHandoverDataForm
 from .helpers import check_required_handovered, get_user_identifiers_formset, get_verified_as
 from .models import (
     OIDCDisplayDedicatedContent,
     OIDCHandoverData,
     OIDCIdentifier,
     OIDCLogin,
     OIDCShowAttribute,
@@ -40,14 +40,15 @@
         return context
 
 
 @plugin_pool.register_plugin
 class OIDCHandoverDataPlugin(OIDCConsumerBase):
     name = _('OIDC Handover data')
     model = OIDCHandoverData
+    form = OIDCHandoverDataForm
     render_template = "djangocms_oidc/handover_data.html"
 
 
 @plugin_pool.register_plugin
 class OIDCLoginPlugin(OIDCConsumerBase):
     name = _('OIDC Login')
     model = OIDCLogin
```

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/helpers.py` & `djangocms_oidc-4.1.0/djangocms_oidc/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/locale/cs/LC_MESSAGES/django.po` & `djangocms_oidc-4.1.0/djangocms_oidc/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/middleware.py` & `djangocms_oidc-4.1.0/djangocms_oidc/middleware.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/migrations/0001_initial.py` & `djangocms_oidc-4.1.0/djangocms_oidc/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/migrations/0002_30274_button_label.py` & `djangocms_oidc-4.1.0/djangocms_oidc/migrations/0002_30274_button_label.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/models.py` & `djangocms_oidc-4.1.0/djangocms_oidc/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,16 @@
     )
 
     provider = models.ForeignKey(OIDCProvider, on_delete=models.CASCADE)
     button_label = models.CharField(
         verbose_name=_('Button label'), max_length=80, null=True, blank=True,
         help_text=_("Button text for unlogged in user."))
     claims = models.JSONField(
-        verbose_name=_("Claims"), validators=[validate_claims], help_text=_("Claims attributes for data handover."))
+        verbose_name=_("Claims"), validators=[validate_claims], help_text=_("Claims attributes for data handover."),
+        default={"userinfo": {}})
     insist_on_required_claims = models.BooleanField(
         verbose_name=_("Insist on required claims"), default=False,
         help_text=_("Consider the data invalid if not all the required data has been handovered."))
     verified_by = models.CharField(
         verbose_name=_('Verified by names'), max_length=255, null=True, blank=True,
         help_text=_("Verified by names (separated by space)."))
     redirect_page = PageField(verbose_name=_('CMS Page'), blank=True, null=True, on_delete=models.SET_NULL,
```

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/change_form/consumer.html` & `djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/change_form/consumer.html`

 * *Files 14% similar despite different names*

```diff
@@ -119,35 +119,70 @@
 00000760: 655f 6e75 6d62 6572 223a 207b 2265 7373  e_number": {"ess
 00000770: 656e 7469 616c 223a 2074 7275 657d 2c0a  ential": true},.
 00000780: 2020 2020 2020 2020 2270 686f 6e65 5f6e          "phone_n
 00000790: 756d 6265 725f 7665 7269 6669 6564 223a  umber_verified":
 000007a0: 207b 2265 7373 656e 7469 616c 223a 2074   {"essential": t
 000007b0: 7275 657d 2c0a 2020 2020 2020 2020 2277  rue},.        "w
 000007c0: 6562 7369 7465 223a 207b 2265 7373 656e  ebsite": {"essen
-000007d0: 7469 616c 223a 2066 616c 7365 7d0a 2020  tial": false}.  
-000007e0: 2020 7d0a 7d0a 2020 2020 3c2f 7072 653e    }.}.    </pre>
-000007f0: 0a0a 2020 2020 3c68 343e 7b25 2074 7261  ..    <h4>{% tra
-00000800: 6e73 6c61 7465 2022 5665 7269 6669 6564  nslate "Verified
-00000810: 2062 7920 6e61 6d65 733a 2220 257d 3c2f   by names:" %}</
-00000820: 6834 3e0a 2020 2020 3c70 7265 3e6e 616d  h4>.    <pre>nam
-00000830: 6520 6769 7665 6e5f 6e61 6d65 2b66 616d  e given_name+fam
-00000840: 696c 795f 6e61 6d65 2070 7265 6665 7272  ily_name preferr
-00000850: 6564 5f75 7365 726e 616d 6520 6e69 636b  ed_username nick
-00000860: 6e61 6d65 2065 6d61 696c 206f 7065 6e69  name email openi
-00000870: 6432 5f69 643c 2f70 7265 3e0a 2020 2020  d2_id</pre>.    
-00000880: 3c70 3e0a 2020 2020 2020 2020 7b25 2062  <p>.        {% b
-00000890: 6c6f 636b 7472 616e 736c 6174 6520 7472  locktranslate tr
-000008a0: 696d 6d65 6420 257d 0a20 2020 2020 2020  immed %}.       
-000008b0: 2020 2020 2054 6865 206c 6973 7420 6f66       The list of
-000008c0: 206e 616d 6573 2069 7320 7363 726f 6c6c   names is scroll
-000008d0: 6564 2069 6e20 7468 6520 7370 6563 6966  ed in the specif
-000008e0: 6965 6420 6f72 6465 7220 756e 7469 6c20  ied order until 
-000008f0: 7468 6520 7661 6c75 6520 6973 2066 6f75  the value is fou
-00000900: 6e64 2e0a 2020 2020 2020 2020 2020 2020  nd..            
-00000910: 466f 7220 6e61 6d65 7320 636f 6d70 6f73  For names compos
-00000920: 6564 206f 6620 6120 706c 7573 2073 6967  ed of a plus sig
-00000930: 6e2c 2074 6865 2076 616c 7565 2063 6f6e  n, the value con
-00000940: 7369 7374 206f 6620 7468 656d 2e0a 2020  sist of them..  
-00000950: 2020 2020 2020 7b25 2065 6e64 626c 6f63        {% endbloc
-00000960: 6b74 7261 6e73 6c61 7465 2025 7d0a 2020  ktranslate %}.  
-00000970: 2020 3c2f 703e 0a7b 2520 656e 6462 6c6f    </p>.{% endblo
-00000980: 636b 2025 7d                             ck %}
+000007d0: 7469 616c 223a 2066 616c 7365 7d2c 0a0a  tial": false},..
+000007e0: 2020 2020 2020 2020 226d 6f6a 6569 645f          "mojeid_
+000007f0: 7661 6c69 6422 3a20 7b22 6573 7365 6e74  valid": {"essent
+00000800: 6961 6c22 3a20 7472 7565 7d2c 0a20 2020  ial": true},.   
+00000810: 207d 2c0a 2020 2020 2264 6562 7567 5f72   },.    "debug_r
+00000820: 6573 706f 6e73 6522 3a20 7472 7565 0a7d  esponse": true.}
+00000830: 0a20 2020 203c 2f70 7265 3e0a 2020 2020  .    </pre>.    
+00000840: 3c70 3e0a 2020 2020 2020 2020 4174 7465  <p>.        Atte
+00000850: 6e74 696f 6e21 2054 6865 203c 636f 6465  ntion! The <code
+00000860: 3e6d 6f6a 6569 645f 7661 6c69 643c 2f63  >mojeid_valid</c
+00000870: 6f64 653e 2061 7474 7269 6275 7465 2069  ode> attribute i
+00000880: 7320 6f6e 6c79 2070 6173 7365 6420 746f  s only passed to
+00000890: 2061 2063 6f6e 7375 6d65 7220 7769 7468   a consumer with
+000008a0: 0a20 2020 2020 2020 203c 6120 6872 6566  .        <a href
+000008b0: 3d22 6874 7470 733a 2f2f 7777 772e 6d6f  ="https://www.mo
+000008c0: 6a65 6964 2e63 7a2f 646f 6375 6d65 6e74  jeid.cz/document
+000008d0: 6174 696f 6e2f 7369 6e67 6c65 6874 6d6c  ation/singlehtml
+000008e0: 2f69 6e64 6578 2e68 746d 6c23 7465 726d  /index.html#term
+000008f0: 2d46 756c 6c2d 6163 6365 7373 2220 7461  -Full-access" ta
+00000900: 7267 6574 3d22 5f62 6c61 6e6b 223e 6675  rget="_blank">fu
+00000910: 6c6c 2061 6363 6573 733c 2f61 3e0a 2020  ll access</a>.  
+00000920: 2020 2020 2020 2873 6565 203c 693e 466c        (see <i>Fl
+00000930: 6167 20e2 8093 2076 616c 6964 6174 696f  ag ... validatio
+00000940: 6e3c 2f69 3e20 696e 203c 7374 726f 6e67  n</i> in <strong
+00000950: 3e4f 7468 6572 2064 6174 613c 2f73 7472  >Other data</str
+00000960: 6f6e 673e 2069 6e0a 2020 2020 2020 2020  ong> in.        
+00000970: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000980: 2f77 7777 2e6d 6f6a 6569 642e 637a 2f64  /www.mojeid.cz/d
+00000990: 6f63 756d 656e 7461 7469 6f6e 2f73 696e  ocumentation/sin
+000009a0: 676c 6568 746d 6c2f 696e 6465 782e 6874  glehtml/index.ht
+000009b0: 6d6c 2361 7070 656e 6469 782d 312d 6c69  ml#appendix-1-li
+000009c0: 7374 2d6f 662d 6461 7461 2d74 6f2d 6265  st-of-data-to-be
+000009d0: 2d68 616e 6465 642d 6f76 6572 2d6f 7065  -handed-over-ope
+000009e0: 6e69 642d 636f 6e6e 6563 7422 2074 6172  nid-connect" tar
+000009f0: 6765 743d 225f 626c 616e 6b22 3e4c 6973  get="_blank">Lis
+00000a00: 7420 6f66 2044 6174 6120 746f 2062 6520  t of Data to be 
+00000a10: 4861 6e64 6564 204f 7665 723c 2f61 3e29  Handed Over</a>)
+00000a20: 2e0a 2020 2020 3c2f 703e 0a20 2020 203c  ..    </p>.    <
+00000a30: 6834 3e7b 2520 7472 616e 736c 6174 6520  h4>{% translate 
+00000a40: 2256 6572 6966 6965 6420 6279 206e 616d  "Verified by nam
+00000a50: 6573 3a22 2025 7d3c 2f68 343e 0a20 2020  es:" %}</h4>.   
+00000a60: 203c 7072 653e 6e61 6d65 2067 6976 656e   <pre>name given
+00000a70: 5f6e 616d 652b 6661 6d69 6c79 5f6e 616d  _name+family_nam
+00000a80: 6520 7072 6566 6572 7265 645f 7573 6572  e preferred_user
+00000a90: 6e61 6d65 206e 6963 6b6e 616d 6520 656d  name nickname em
+00000aa0: 6169 6c20 6f70 656e 6964 325f 6964 3c2f  ail openid2_id</
+00000ab0: 7072 653e 0a20 2020 203c 703e 0a20 2020  pre>.    <p>.   
+00000ac0: 2020 2020 207b 2520 626c 6f63 6b74 7261       {% blocktra
+00000ad0: 6e73 6c61 7465 2074 7269 6d6d 6564 2025  nslate trimmed %
+00000ae0: 7d0a 2020 2020 2020 2020 2020 2020 5468  }.            Th
+00000af0: 6520 6c69 7374 206f 6620 6e61 6d65 7320  e list of names 
+00000b00: 6973 2073 6372 6f6c 6c65 6420 696e 2074  is scrolled in t
+00000b10: 6865 2073 7065 6369 6669 6564 206f 7264  he specified ord
+00000b20: 6572 2075 6e74 696c 2074 6865 2076 616c  er until the val
+00000b30: 7565 2069 7320 666f 756e 642e 0a20 2020  ue is found..   
+00000b40: 2020 2020 2020 2020 2046 6f72 206e 616d           For nam
+00000b50: 6573 2063 6f6d 706f 7365 6420 6f66 2061  es composed of a
+00000b60: 2070 6c75 7320 7369 676e 2c20 7468 6520   plus sign, the 
+00000b70: 7661 6c75 6520 636f 6e73 6973 7420 6f66  value consist of
+00000b80: 2074 6865 6d2e 0a20 2020 2020 2020 207b   them..        {
+00000b90: 2520 656e 6462 6c6f 636b 7472 616e 736c  % endblocktransl
+00000ba0: 6174 6520 257d 0a20 2020 203c 2f70 3e0a  ate %}.    </p>.
+00000bb0: 7b25 2065 6e64 626c 6f63 6b20 257d       {% endblock %}
```

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/handover_data.html` & `djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/handover_data.html`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/list_identifiers.html` & `djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/list_identifiers.html`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/templates/djangocms_oidc/login.html` & `djangocms_oidc-4.1.0/djangocms_oidc/templates/djangocms_oidc/login.html`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/tests/settings.py` & `djangocms_oidc-4.1.0/djangocms_oidc/tests/settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/tests/test_admin_forms.py` & `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_admin_forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/tests/test_admin_options.py` & `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_admin_options.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/tests/test_auth.py` & `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/tests/test_cms_plugins.py` & `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/tests/test_forms.py` & `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/tests/test_helpers.py` & `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/tests/test_middleware.py` & `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/tests/test_models.py` & `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/tests/test_utils.py` & `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/tests/test_views.py` & `djangocms_oidc-4.1.0/djangocms_oidc/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/tests/urls.py` & `djangocms_oidc-4.1.0/djangocms_oidc/tests/urls.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/urls.py` & `djangocms_oidc-4.1.0/djangocms_oidc/urls.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/utils.py` & `djangocms_oidc-4.1.0/djangocms_oidc/utils.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc/views.py` & `djangocms_oidc-4.1.0/djangocms_oidc/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc.egg-info/PKG-INFO` & `djangocms_oidc-4.1.0/djangocms_oidc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-oidc
-Version: 4.0.0
+Version: 4.1.0
 Summary: Plugin OIDC (OpenID Connect) into Django CMS.
 Home-page: https://github.com/CZ-NIC/djangocms-oidc
 Author: Zdeněk Böhm
 Author-email: zdenek.bohm@nic.cz
 License: GPL GNU License
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `djangocms-oidc-4.0.0/djangocms_oidc.egg-info/SOURCES.txt` & `djangocms_oidc-4.1.0/djangocms_oidc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 djangocms_oidc/forms.py
 djangocms_oidc/helpers.py
 djangocms_oidc/middleware.py
 djangocms_oidc/models.py
 djangocms_oidc/urls.py
 djangocms_oidc/utils.py
 djangocms_oidc/views.py
+djangocms_oidc/widgets.py
 djangocms_oidc.egg-info/PKG-INFO
 djangocms_oidc.egg-info/SOURCES.txt
 djangocms_oidc.egg-info/dependency_links.txt
 djangocms_oidc.egg-info/not-zip-safe
 djangocms_oidc.egg-info/requires.txt
 djangocms_oidc.egg-info/top_level.txt
 djangocms_oidc/admin/__init__.py
 djangocms_oidc/admin/forms.py
 djangocms_oidc/admin/options.py
-djangocms_oidc/locale/cs/LC_MESSAGES/django.mo
 djangocms_oidc/locale/cs/LC_MESSAGES/django.po
 djangocms_oidc/migrations/0001_initial.py
 djangocms_oidc/migrations/0002_30274_button_label.py
 djangocms_oidc/migrations/__init__.py
 djangocms_oidc/templates/djangocms_oidc/display_dedicated_content.html
 djangocms_oidc/templates/djangocms_oidc/handover_data.html
 djangocms_oidc/templates/djangocms_oidc/list_identifiers.html
@@ -45,9 +45,10 @@
 djangocms_oidc/tests/test_cms_plugins.py
 djangocms_oidc/tests/test_forms.py
 djangocms_oidc/tests/test_helpers.py
 djangocms_oidc/tests/test_middleware.py
 djangocms_oidc/tests/test_models.py
 djangocms_oidc/tests/test_utils.py
 djangocms_oidc/tests/test_views.py
+djangocms_oidc/tests/test_widgets.py
 djangocms_oidc/tests/urls.py
 djangocms_oidc/tests/views.py
```

### Comparing `djangocms-oidc-4.0.0/setup.py` & `djangocms_oidc-4.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     sub_commands = [("compile_catalog", lambda x: True)] + build.sub_commands
 
 
 setup(
     author='Zdeněk Böhm',
     author_email='zdenek.bohm@nic.cz',
     name='djangocms-oidc',
-    version='4.0.0',
+    version='4.1.0',
     description='Plugin OIDC (OpenID Connect) into Django CMS.',
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     url='https://github.com/CZ-NIC/djangocms-oidc',
     license='GPL GNU License',
     platforms=['OS Independent'],
     classifiers=(
```

