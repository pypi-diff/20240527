# Comparing `tmp/moose-frank-9.3.0.tar.gz` & `tmp/moose-frank-9.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/moose-frank-9.3.0.tar", last modified: Mon Feb 19 12:45:37 2024, max compression
+gzip compressed data, was "moose-frank-9.3.1.tar", last modified: Mon May 27 04:26:55 2024, max compression
```

## Comparing `moose-frank-9.3.0.tar` & `moose-frank-9.3.1.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-02-19 12:45:30.000000 moose-frank-9.3.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-02-19 12:45:30.000000 moose-frank-9.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2477 2024-02-19 12:45:37.000000 moose-frank-9.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      817 2024-02-19 12:45:30.000000 moose-frank-9.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-02-19 12:45:36.000000 moose-frank-9.3.0/moose_frank/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/graphene/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/graphene/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/graphene/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/graphene/converter.py
--rw-rw-rw-   0 root         (0) root         (0)     6777 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/graphene/mutations.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/graphene/schema_mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     2316 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/graphene/types.py
--rw-rw-rw-   0 root         (0) root         (0)      452 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/graphene/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/js_routes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/js_routes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5123 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/js_routes/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/js_routes/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/js_routes/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/js_routes/utils/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1565 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     1877 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)     1613 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/management/commands/dump_routes_resolver.py
--rw-rw-rw-   0 root         (0) root         (0)     3086 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/management/commands/generate_urlpatterns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/storages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/storages/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2142 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/storages/gcloud.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/templates/js_routes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/templates/js_routes/_dump/
--rw-rw-rw-   0 root         (0) root         (0)     2258 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/templates/js_routes/_dump/resolver.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/templatetags/active.py
--rw-rw-rw-   0 root         (0) root         (0)     3622 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/templatetags/generic.py
--rw-rw-rw-   0 root         (0) root         (0)      937 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/templatetags/mathtags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25735 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/tests/django.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/tests/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/tests/pillow.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/tests/requests_mock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank/utils/
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/utils/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     1347 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/utils/dates.py
--rw-rw-rw-   0 root         (0) root         (0)     1247 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/utils/filters.py
--rw-rw-rw-   0 root         (0) root         (0)      769 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/utils/network.py
--rw-rw-rw-   0 root         (0) root         (0)     1198 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/utils/sanitizer.py
--rw-rw-rw-   0 root         (0) root         (0)      443 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/utils/text.py
--rw-rw-rw-   0 root         (0) root         (0)     3561 2024-02-19 12:45:30.000000 moose-frank-9.3.0/moose_frank/utils/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2477 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1499 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      130 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-02-19 12:45:37.000000 moose-frank-9.3.0/moose_frank.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-02-19 12:45:37.000000 moose-frank-9.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1740 2024-02-19 12:45:36.000000 moose-frank-9.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-05-27 04:26:44.000000 moose-frank-9.3.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-05-27 04:26:44.000000 moose-frank-9.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-05-27 04:26:55.000000 moose-frank-9.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      817 2024-05-27 04:26:44.000000 moose-frank-9.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-27 04:26:54.000000 moose-frank-9.3.1/moose_frank/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/graphene/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/graphene/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/graphene/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/graphene/converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6777 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/graphene/mutations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/graphene/schema_mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/graphene/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      452 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/graphene/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/js_routes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 04:26:45.000000 moose-frank-9.3.1/moose_frank/js_routes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5123 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/js_routes/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/js_routes/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 04:26:45.000000 moose-frank-9.3.1/moose_frank/js_routes/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/js_routes/utils/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1877 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/management/commands/dump_routes_resolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     3086 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/management/commands/generate_urlpatterns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/storages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 04:26:45.000000 moose-frank-9.3.1/moose_frank/storages/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2142 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/storages/gcloud.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/templates/js_routes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/templates/js_routes/_dump/
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/templates/js_routes/_dump/resolver.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 04:26:45.000000 moose-frank-9.3.1/moose_frank/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/templatetags/active.py
+-rw-rw-rw-   0 root         (0) root         (0)     3622 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/templatetags/generic.py
+-rw-rw-rw-   0 root         (0) root         (0)      937 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/templatetags/mathtags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 04:26:45.000000 moose-frank-9.3.1/moose_frank/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25735 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/tests/django.py
+-rw-rw-rw-   0 root         (0) root         (0)     1137 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/tests/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/tests/pillow.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/tests/requests_mock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/utils/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/utils/dates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/utils/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/utils/network.py
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/utils/sanitizer.py
+-rw-rw-rw-   0 root         (0) root         (0)      443 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/utils/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     3561 2024-05-27 04:26:44.000000 moose-frank-9.3.1/moose_frank/utils/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1514 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      130 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-27 04:26:55.000000 moose-frank-9.3.1/moose_frank.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-05-27 04:26:44.000000 moose-frank-9.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-27 04:26:55.000000 moose-frank-9.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1740 2024-05-27 04:26:54.000000 moose-frank-9.3.1/setup.py
```

### Comparing `moose-frank-9.3.0/LICENSE.txt` & `moose-frank-9.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/README.md` & `moose-frank-9.3.1/README.md`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/graphene/converter.py` & `moose-frank-9.3.1/moose_frank/graphene/converter.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/graphene/mutations.py` & `moose-frank-9.3.1/moose_frank/graphene/mutations.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/graphene/schema_mixins.py` & `moose-frank-9.3.1/moose_frank/graphene/schema_mixins.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/graphene/types.py` & `moose-frank-9.3.1/moose_frank/graphene/types.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/js_routes/serializers.py` & `moose-frank-9.3.1/moose_frank/js_routes/serializers.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/js_routes/utils/text.py` & `moose-frank-9.3.1/moose_frank/js_routes/utils/text.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/locale/nl/LC_MESSAGES/django.mo` & `moose-frank-9.3.1/moose_frank/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/locale/nl/LC_MESSAGES/django.po` & `moose-frank-9.3.1/moose_frank/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/management/commands/dump_routes_resolver.py` & `moose-frank-9.3.1/moose_frank/management/commands/dump_routes_resolver.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/management/commands/generate_urlpatterns.py` & `moose-frank-9.3.1/moose_frank/management/commands/generate_urlpatterns.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/storages/gcloud.py` & `moose-frank-9.3.1/moose_frank/storages/gcloud.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/templates/js_routes/_dump/resolver.ts` & `moose-frank-9.3.1/moose_frank/templates/js_routes/_dump/resolver.ts`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/templatetags/active.py` & `moose-frank-9.3.1/moose_frank/templatetags/active.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/templatetags/generic.py` & `moose-frank-9.3.1/moose_frank/templatetags/generic.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/templatetags/mathtags.py` & `moose-frank-9.3.1/moose_frank/templatetags/mathtags.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/tests/django.py` & `moose-frank-9.3.1/moose_frank/tests/django.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/tests/graphql.py` & `moose-frank-9.3.1/moose_frank/tests/graphql.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,17 +17,17 @@
         files: Optional[dict] = None,
         extra_token_data: Optional[dict] = None,
     ):
         headers = {}
         if as_user:
             if extra_token_data is None:
                 extra_token_data = {}
-            headers[
-                "HTTP_AUTHORIZATION"
-            ] = f"JWT {get_token(as_user, **extra_token_data)}"
+            headers["HTTP_AUTHORIZATION"] = (
+                f"JWT {get_token(as_user, **extra_token_data)}"
+            )
 
         data = {
             "operations": json.dumps({"query": query, "variables": variables or {}})
         }
         if files:
             mapping = {i: [k] for i, k in enumerate(files.keys())}
             data["map"] = json.dumps(mapping)
```

### Comparing `moose-frank-9.3.0/moose_frank/utils/cache.py` & `moose-frank-9.3.1/moose_frank/utils/cache.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/utils/dates.py` & `moose-frank-9.3.1/moose_frank/utils/dates.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/utils/filters.py` & `moose-frank-9.3.1/moose_frank/utils/filters.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/utils/network.py` & `moose-frank-9.3.1/moose_frank/utils/network.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/utils/sanitizer.py` & `moose-frank-9.3.1/moose_frank/utils/sanitizer.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank/utils/validators.py` & `moose-frank-9.3.1/moose_frank/utils/validators.py`

 * *Files identical despite different names*

### Comparing `moose-frank-9.3.0/moose_frank.egg-info/SOURCES.txt` & `moose-frank-9.3.1/moose_frank.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 moose_frank/__init__.py
 moose_frank.egg-info/PKG-INFO
 moose_frank.egg-info/SOURCES.txt
 moose_frank.egg-info/dependency_links.txt
 moose_frank.egg-info/not-zip-safe
```

### Comparing `moose-frank-9.3.0/setup.py` & `moose-frank-9.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 
-version = "9.3.0"
+version = "9.3.1"
 
 setup(
     name="moose-frank",
     packages=find_packages(),
     version=version,
     description="A Python package packed with tools that are commonly used in "
     "Moose projects.",
@@ -16,15 +16,15 @@
     author="Sven Groot (Moose / Digital Agency)",
     author_email="sven@wearemoose.com",
     url="https://gitlab.com/mediamoose/moose-frank/tree/v{}".format(version),
     download_url="https://gitlab.com/mediamoose/moose-frank/repository/v{}/archive.tar.gz".format(
         version
     ),
     include_package_data=True,
-    install_requires=["django>=3.2.23"],
+    install_requires=["django>=3.2.25"],
     extras_require={
         "graphene": [
             "graphene-django>=3.0",
             "graphene-file-upload>=1.3",
             "graphene>=3.2",
         ],
         "gcloud": [
```

