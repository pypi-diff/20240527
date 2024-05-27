# Comparing `tmp/django-botmanager-0.2.17.tar.gz` & `tmp/django_botmanager-0.2.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-botmanager-0.2.17.tar", last modified: Tue Nov 21 10:30:03 2023, max compression
+gzip compressed data, was "django_botmanager-0.2.18.tar", last modified: Mon May 27 08:38:20 2024, max compression
```

## Comparing `django-botmanager-0.2.17.tar` & `django_botmanager-0.2.18.tar`

### file list

```diff
@@ -1,383 +1,43 @@
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.414893 django-botmanager-0.2.17/
--rw-rw-r--   0 titov     (1000) titov     (1000)     1479 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/LICENSE
--rw-r--r--   0 titov     (1000) titov     (1000)      320 2023-11-21 10:30:03.414893 django-botmanager-0.2.17/PKG-INFO
--rw-rw-r--   0 titov     (1000) titov     (1000)      562 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/README.md
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.358893 django-botmanager-0.2.17/botmanager/
--rw-rw-r--   0 titov     (1000) titov     (1000)       73 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/__init__.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     1542 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/admin.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      135 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/apps.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     7829 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/basetask.py
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.354893 django-botmanager-0.2.17/botmanager/locale/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.322892 django-botmanager-0.2.17/botmanager/locale/af/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.358893 django-botmanager-0.2.17/botmanager/locale/af/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2093 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/af/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2272 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/af/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.322892 django-botmanager-0.2.17/botmanager/locale/am/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.358893 django-botmanager-0.2.17/botmanager/locale/am/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2357 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/am/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2532 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/am/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.322892 django-botmanager-0.2.17/botmanager/locale/ar/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.362893 django-botmanager-0.2.17/botmanager/locale/ar/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2414 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ar/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2593 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ar/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.326892 django-botmanager-0.2.17/botmanager/locale/ar_DZ/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.362893 django-botmanager-0.2.17/botmanager/locale/ar_DZ/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2414 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ar_DZ/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2593 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ar_DZ/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.326892 django-botmanager-0.2.17/botmanager/locale/bg/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.362893 django-botmanager-0.2.17/botmanager/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2491 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/bg/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     3262 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/bg/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.326892 django-botmanager-0.2.17/botmanager/locale/bn/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.362893 django-botmanager-0.2.17/botmanager/locale/bn/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2740 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/bn/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2922 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/bn/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.326892 django-botmanager-0.2.17/botmanager/locale/bs/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.362893 django-botmanager-0.2.17/botmanager/locale/bs/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2203 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/bs/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2382 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/bs/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.326892 django-botmanager-0.2.17/botmanager/locale/ca/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.362893 django-botmanager-0.2.17/botmanager/locale/ca/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2137 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ca/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2316 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ca/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.326892 django-botmanager-0.2.17/botmanager/locale/cs/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.362893 django-botmanager-0.2.17/botmanager/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2216 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/cs/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2395 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/cs/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.326892 django-botmanager-0.2.17/botmanager/locale/cy/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.366893 django-botmanager-0.2.17/botmanager/locale/cy/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2139 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/cy/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2318 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/cy/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.326892 django-botmanager-0.2.17/botmanager/locale/da/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.366893 django-botmanager-0.2.17/botmanager/locale/da/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2102 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/da/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2281 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/da/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.326892 django-botmanager-0.2.17/botmanager/locale/de/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.366893 django-botmanager-0.2.17/botmanager/locale/de/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2167 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2346 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.326892 django-botmanager-0.2.17/botmanager/locale/el/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.366893 django-botmanager-0.2.17/botmanager/locale/el/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2586 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/el/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2765 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/el/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.326892 django-botmanager-0.2.17/botmanager/locale/en/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.366893 django-botmanager-0.2.17/botmanager/locale/en/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2062 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2241 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.326892 django-botmanager-0.2.17/botmanager/locale/en_AU/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.366893 django-botmanager-0.2.17/botmanager/locale/en_AU/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2062 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/en_AU/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2241 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/en_AU/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.330892 django-botmanager-0.2.17/botmanager/locale/en_GB/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.370893 django-botmanager-0.2.17/botmanager/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2062 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/en_GB/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2241 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/en_GB/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.330892 django-botmanager-0.2.17/botmanager/locale/eo/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.370893 django-botmanager-0.2.17/botmanager/locale/eo/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2084 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/eo/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2263 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/eo/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.330892 django-botmanager-0.2.17/botmanager/locale/es/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.370893 django-botmanager-0.2.17/botmanager/locale/es/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2151 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2333 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.330892 django-botmanager-0.2.17/botmanager/locale/es_AR/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.370893 django-botmanager-0.2.17/botmanager/locale/es_AR/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2151 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/es_AR/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2333 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/es_AR/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.330892 django-botmanager-0.2.17/botmanager/locale/es_CO/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.370893 django-botmanager-0.2.17/botmanager/locale/es_CO/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2151 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/es_CO/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2333 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/es_CO/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.330892 django-botmanager-0.2.17/botmanager/locale/es_MX/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.370893 django-botmanager-0.2.17/botmanager/locale/es_MX/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2151 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/es_MX/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2333 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/es_MX/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.330892 django-botmanager-0.2.17/botmanager/locale/et/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.370893 django-botmanager-0.2.17/botmanager/locale/et/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2119 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/et/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2298 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/et/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.330892 django-botmanager-0.2.17/botmanager/locale/eu/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.374893 django-botmanager-0.2.17/botmanager/locale/eu/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2103 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/eu/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2282 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/eu/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.330892 django-botmanager-0.2.17/botmanager/locale/fa/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.374893 django-botmanager-0.2.17/botmanager/locale/fa/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2332 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/fa/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2511 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/fa/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.330892 django-botmanager-0.2.17/botmanager/locale/fi/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.374893 django-botmanager-0.2.17/botmanager/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2140 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/fi/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2319 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.330892 django-botmanager-0.2.17/botmanager/locale/fr/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.374893 django-botmanager-0.2.17/botmanager/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2170 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2349 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.330892 django-botmanager-0.2.17/botmanager/locale/fy/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.374893 django-botmanager-0.2.17/botmanager/locale/fy/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2091 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/fy/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2270 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/fy/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.334892 django-botmanager-0.2.17/botmanager/locale/ga/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.374893 django-botmanager-0.2.17/botmanager/locale/ga/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2219 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ga/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2404 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ga/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.334892 django-botmanager-0.2.17/botmanager/locale/gd/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.378893 django-botmanager-0.2.17/botmanager/locale/gd/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2331 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/gd/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2516 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/gd/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.334892 django-botmanager-0.2.17/botmanager/locale/he/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.378893 django-botmanager-0.2.17/botmanager/locale/he/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2391 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/he/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2570 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/he/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.334892 django-botmanager-0.2.17/botmanager/locale/hi/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.378893 django-botmanager-0.2.17/botmanager/locale/hi/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2709 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/hi/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2888 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/hi/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.334892 django-botmanager-0.2.17/botmanager/locale/hr/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.378893 django-botmanager-0.2.17/botmanager/locale/hr/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2200 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/hr/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2379 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/hr/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.334892 django-botmanager-0.2.17/botmanager/locale/hu/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.378893 django-botmanager-0.2.17/botmanager/locale/hu/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2196 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/hu/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2375 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/hu/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.334892 django-botmanager-0.2.17/botmanager/locale/hy/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.378893 django-botmanager-0.2.17/botmanager/locale/hy/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2560 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/hy/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2739 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/hy/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.334892 django-botmanager-0.2.17/botmanager/locale/id/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.378893 django-botmanager-0.2.17/botmanager/locale/id/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2117 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/id/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2888 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.334892 django-botmanager-0.2.17/botmanager/locale/it/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.382893 django-botmanager-0.2.17/botmanager/locale/it/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2182 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2364 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.334892 django-botmanager-0.2.17/botmanager/locale/ja/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.382893 django-botmanager-0.2.17/botmanager/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2160 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ja/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2339 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ja/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.334892 django-botmanager-0.2.17/botmanager/locale/ka/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.382893 django-botmanager-0.2.17/botmanager/locale/ka/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2956 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ka/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     3138 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ka/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.334892 django-botmanager-0.2.17/botmanager/locale/kab/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.382893 django-botmanager-0.2.17/botmanager/locale/kab/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)      380 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/kab/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     1883 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/kab/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.338892 django-botmanager-0.2.17/botmanager/locale/kk/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.382893 django-botmanager-0.2.17/botmanager/locale/kk/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2462 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/kk/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2641 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/kk/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.338892 django-botmanager-0.2.17/botmanager/locale/km/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.382893 django-botmanager-0.2.17/botmanager/locale/km/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2932 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/km/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     3111 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/km/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.338892 django-botmanager-0.2.17/botmanager/locale/kn/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.386893 django-botmanager-0.2.17/botmanager/locale/kn/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2737 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/kn/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2916 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/kn/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.338892 django-botmanager-0.2.17/botmanager/locale/ko/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.386893 django-botmanager-0.2.17/botmanager/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2071 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ko/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2250 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ko/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.338892 django-botmanager-0.2.17/botmanager/locale/ky/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.386893 django-botmanager-0.2.17/botmanager/locale/ky/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2488 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ky/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2673 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ky/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.338892 django-botmanager-0.2.17/botmanager/locale/lb/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.386893 django-botmanager-0.2.17/botmanager/locale/lb/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2124 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/lb/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2303 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/lb/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.338892 django-botmanager-0.2.17/botmanager/locale/lt/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.386893 django-botmanager-0.2.17/botmanager/locale/lt/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2255 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/lt/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2434 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/lt/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.338892 django-botmanager-0.2.17/botmanager/locale/lv/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.386893 django-botmanager-0.2.17/botmanager/locale/lv/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2186 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/lv/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2365 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/lv/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.338892 django-botmanager-0.2.17/botmanager/locale/mk/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.386893 django-botmanager-0.2.17/botmanager/locale/mk/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2508 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/mk/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2687 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/mk/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.338892 django-botmanager-0.2.17/botmanager/locale/ml/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.386893 django-botmanager-0.2.17/botmanager/locale/ml/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2926 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ml/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     3105 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ml/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.342893 django-botmanager-0.2.17/botmanager/locale/mn/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.390893 django-botmanager-0.2.17/botmanager/locale/mn/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2542 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/mn/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2721 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/mn/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.342893 django-botmanager-0.2.17/botmanager/locale/mr/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.390893 django-botmanager-0.2.17/botmanager/locale/mr/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2722 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/mr/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2901 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/mr/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.342893 django-botmanager-0.2.17/botmanager/locale/ms/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.390893 django-botmanager-0.2.17/botmanager/locale/ms/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2122 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ms/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2304 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ms/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.342893 django-botmanager-0.2.17/botmanager/locale/my/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.390893 django-botmanager-0.2.17/botmanager/locale/my/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     3014 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/my/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     3196 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/my/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.342893 django-botmanager-0.2.17/botmanager/locale/nb/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.390893 django-botmanager-0.2.17/botmanager/locale/nb/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)      380 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/nb/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     1883 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/nb/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.342893 django-botmanager-0.2.17/botmanager/locale/ne/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.390893 django-botmanager-0.2.17/botmanager/locale/ne/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2747 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ne/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2926 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ne/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.342893 django-botmanager-0.2.17/botmanager/locale/nl/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.394893 django-botmanager-0.2.17/botmanager/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2115 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2294 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/nl/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.342893 django-botmanager-0.2.17/botmanager/locale/nn/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.394893 django-botmanager-0.2.17/botmanager/locale/nn/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)      380 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/nn/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     1883 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/nn/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.342893 django-botmanager-0.2.17/botmanager/locale/os/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.394893 django-botmanager-0.2.17/botmanager/locale/os/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)      380 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/os/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     1883 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/os/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.346892 django-botmanager-0.2.17/botmanager/locale/pa/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.394893 django-botmanager-0.2.17/botmanager/locale/pa/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2659 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/pa/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2838 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/pa/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.346892 django-botmanager-0.2.17/botmanager/locale/pl/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.394893 django-botmanager-0.2.17/botmanager/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2279 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2458 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.346892 django-botmanager-0.2.17/botmanager/locale/pt/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.394893 django-botmanager-0.2.17/botmanager/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2146 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2325 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/pt/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.346892 django-botmanager-0.2.17/botmanager/locale/pt_BR/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.394893 django-botmanager-0.2.17/botmanager/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2145 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2324 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.346892 django-botmanager-0.2.17/botmanager/locale/ro/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.394893 django-botmanager-0.2.17/botmanager/locale/ro/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2204 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ro/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2383 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ro/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.346892 django-botmanager-0.2.17/botmanager/locale/ru/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.398893 django-botmanager-0.2.17/botmanager/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2658 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2837 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.346892 django-botmanager-0.2.17/botmanager/locale/sk/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.398893 django-botmanager-0.2.17/botmanager/locale/sk/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2230 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/sk/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2409 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/sk/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.346892 django-botmanager-0.2.17/botmanager/locale/sl/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.398893 django-botmanager-0.2.17/botmanager/locale/sl/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2163 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/sl/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2342 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/sl/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.346892 django-botmanager-0.2.17/botmanager/locale/sq/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.398893 django-botmanager-0.2.17/botmanager/locale/sq/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2188 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/sq/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2370 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/sq/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.350892 django-botmanager-0.2.17/botmanager/locale/sr/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.398893 django-botmanager-0.2.17/botmanager/locale/sr/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2523 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/sr/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2702 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/sr/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.350892 django-botmanager-0.2.17/botmanager/locale/sr_Latn/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.398893 django-botmanager-0.2.17/botmanager/locale/sr_Latn/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2523 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/sr_Latn/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2702 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/sr_Latn/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.350892 django-botmanager-0.2.17/botmanager/locale/sv/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.398893 django-botmanager-0.2.17/botmanager/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2108 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/sv/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2287 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/sv/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.350892 django-botmanager-0.2.17/botmanager/locale/sw/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.402893 django-botmanager-0.2.17/botmanager/locale/sw/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2149 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/sw/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2334 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/sw/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.350892 django-botmanager-0.2.17/botmanager/locale/ta/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.402893 django-botmanager-0.2.17/botmanager/locale/ta/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2863 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ta/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     3045 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ta/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.350892 django-botmanager-0.2.17/botmanager/locale/te/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.402893 django-botmanager-0.2.17/botmanager/locale/te/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2703 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/te/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2882 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/te/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.350892 django-botmanager-0.2.17/botmanager/locale/tg/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.402893 django-botmanager-0.2.17/botmanager/locale/tg/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2460 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/tg/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2639 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/tg/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.350892 django-botmanager-0.2.17/botmanager/locale/th/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.402893 django-botmanager-0.2.17/botmanager/locale/th/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2818 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/th/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2997 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/th/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.350892 django-botmanager-0.2.17/botmanager/locale/tk/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.402893 django-botmanager-0.2.17/botmanager/locale/tk/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)      380 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/tk/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     1883 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/tk/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.350892 django-botmanager-0.2.17/botmanager/locale/tr/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.402893 django-botmanager-0.2.17/botmanager/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2140 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/tr/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2319 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/tr/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.350892 django-botmanager-0.2.17/botmanager/locale/tt/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.402893 django-botmanager-0.2.17/botmanager/locale/tt/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)      373 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/tt/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     1876 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/tt/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.354893 django-botmanager-0.2.17/botmanager/locale/udm/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.402893 django-botmanager-0.2.17/botmanager/locale/udm/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)      373 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/udm/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     1876 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/udm/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.354893 django-botmanager-0.2.17/botmanager/locale/ug/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.406893 django-botmanager-0.2.17/botmanager/locale/ug/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2481 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ug/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     3251 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ug/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.354893 django-botmanager-0.2.17/botmanager/locale/uk/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.406893 django-botmanager-0.2.17/botmanager/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2733 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2912 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.354893 django-botmanager-0.2.17/botmanager/locale/ur/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.406893 django-botmanager-0.2.17/botmanager/locale/ur/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2382 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ur/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2564 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/ur/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.354893 django-botmanager-0.2.17/botmanager/locale/uz/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.406893 django-botmanager-0.2.17/botmanager/locale/uz/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2162 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/uz/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2344 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/uz/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.354893 django-botmanager-0.2.17/botmanager/locale/vi/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.406893 django-botmanager-0.2.17/botmanager/locale/vi/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)     2227 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/vi/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     2406 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/vi/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.354893 django-botmanager-0.2.17/botmanager/locale/zh_Hans/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.410893 django-botmanager-0.2.17/botmanager/locale/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)      373 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     1876 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/zh_Hans/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.354893 django-botmanager-0.2.17/botmanager/locale/zh_Hant/
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.410893 django-botmanager-0.2.17/botmanager/locale/zh_Hant/LC_MESSAGES/
--rw-rw-r--   0 titov     (1000) titov     (1000)      373 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-rw-r--   0 titov     (1000) titov     (1000)     1876 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/locale/zh_Hant/LC_MESSAGES/django.po
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.410893 django-botmanager-0.2.17/botmanager/management/
--rw-rw-r--   0 titov     (1000) titov     (1000)        0 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/management/__init__.py
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.410893 django-botmanager-0.2.17/botmanager/management/commands/
--rw-rw-r--   0 titov     (1000) titov     (1000)      542 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/management/commands/__init__.py
--rw-rw-r--   0 titov     (1000) titov     (1000)    18210 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/management/commands/bot_manager.py
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.414893 django-botmanager-0.2.17/botmanager/migrations/
--rw-rw-r--   0 titov     (1000) titov     (1000)     3357 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/migrations/0001_initial.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      742 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/migrations/0002_auto_20161208_1406.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     1935 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/migrations/0003_auto_20161208_1529.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     2880 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/migrations/0004_auto_20161219_1931.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      712 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/migrations/0005_task_parent.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      448 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/migrations/0006_task_priority.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      667 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/migrations/0007_task_is_persistent.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      673 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/migrations/0008_auto_20170331_1752.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      489 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/migrations/0009_task_extra_params.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      653 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/migrations/0010_auto_20170531_1321.py
--rw-rw-r--   0 titov     (1000) titov     (1000)      706 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/migrations/0011_alter_task_create_dt_alter_task_id.py
--rw-rw-r--   0 titov     (1000) titov     (1000)        0 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/migrations/__init__.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     3674 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/models.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     3266 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/settings.py
--rw-rw-r--   0 titov     (1000) titov     (1000)     1105 2023-11-21 10:26:32.000000 django-botmanager-0.2.17/botmanager/utils.py
-drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2023-11-21 10:30:03.414893 django-botmanager-0.2.17/django_botmanager.egg-info/
--rw-r--r--   0 titov     (1000) titov     (1000)      320 2023-11-21 10:30:03.000000 django-botmanager-0.2.17/django_botmanager.egg-info/PKG-INFO
--rw-rw-r--   0 titov     (1000) titov     (1000)     8539 2023-11-21 10:30:03.000000 django-botmanager-0.2.17/django_botmanager.egg-info/SOURCES.txt
--rw-rw-r--   0 titov     (1000) titov     (1000)        1 2023-11-21 10:30:03.000000 django-botmanager-0.2.17/django_botmanager.egg-info/dependency_links.txt
--rw-rw-r--   0 titov     (1000) titov     (1000)       52 2023-11-21 10:30:03.000000 django-botmanager-0.2.17/django_botmanager.egg-info/requires.txt
--rw-rw-r--   0 titov     (1000) titov     (1000)       11 2023-11-21 10:30:03.000000 django-botmanager-0.2.17/django_botmanager.egg-info/top_level.txt
--rw-rw-r--   0 titov     (1000) titov     (1000)       38 2023-11-21 10:30:03.418893 django-botmanager-0.2.17/setup.cfg
--rw-rw-r--   0 titov     (1000) titov     (1000)      560 2023-11-21 10:27:34.000000 django-botmanager-0.2.17/setup.py
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-27 08:38:20.188832 django_botmanager-0.2.18/
+-rw-rw-r--   0 titov     (1000) titov     (1000)     1479 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/LICENSE
+-rw-rw-r--   0 titov     (1000) titov     (1000)       72 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/MANIFEST.in
+-rw-r--r--   0 titov     (1000) titov     (1000)      320 2024-05-27 08:38:20.188832 django_botmanager-0.2.18/PKG-INFO
+-rw-rw-r--   0 titov     (1000) titov     (1000)      562 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/README.md
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-27 08:38:20.184832 django_botmanager-0.2.18/botmanager/
+-rw-rw-r--   0 titov     (1000) titov     (1000)       73 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/__init__.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)     2881 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/admin.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      135 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/apps.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)     7829 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/basetask.py
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-27 08:38:20.184832 django_botmanager-0.2.18/botmanager/management/
+-rw-rw-r--   0 titov     (1000) titov     (1000)        0 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/management/__init__.py
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-27 08:38:20.184832 django_botmanager-0.2.18/botmanager/management/commands/
+-rw-rw-r--   0 titov     (1000) titov     (1000)      542 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/management/commands/__init__.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)    18210 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/management/commands/bot_manager.py
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-27 08:38:20.184832 django_botmanager-0.2.18/botmanager/migrations/
+-rw-rw-r--   0 titov     (1000) titov     (1000)     3357 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/migrations/0001_initial.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      742 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/migrations/0002_auto_20161208_1406.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)     1935 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/migrations/0003_auto_20161208_1529.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)     2880 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/migrations/0004_auto_20161219_1931.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      712 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/migrations/0005_task_parent.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      448 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/migrations/0006_task_priority.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      667 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/migrations/0007_task_is_persistent.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      673 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/migrations/0008_auto_20170331_1752.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      489 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/migrations/0009_task_extra_params.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      653 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/migrations/0010_auto_20170531_1321.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)      706 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/migrations/0011_alter_task_create_dt_alter_task_id.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)        0 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/migrations/__init__.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)     3674 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/models.py
+-rw-rw-r--   0 titov     (1000) titov     (1000)     3266 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/settings.py
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-27 08:38:20.180832 django_botmanager-0.2.18/botmanager/templates/
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-27 08:38:20.180832 django_botmanager-0.2.18/botmanager/templates/botmanager/
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-27 08:38:20.184832 django_botmanager-0.2.18/botmanager/templates/botmanager/task/
+-rw-rw-r--   0 titov     (1000) titov     (1000)      277 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/templates/botmanager/task/change_form.html
+-rw-rw-r--   0 titov     (1000) titov     (1000)     1105 2024-05-27 08:25:58.000000 django_botmanager-0.2.18/botmanager/utils.py
+drwxrwxr-x   0 titov     (1000) titov     (1000)        0 2024-05-27 08:38:20.188832 django_botmanager-0.2.18/django_botmanager.egg-info/
+-rw-r--r--   0 titov     (1000) titov     (1000)      320 2024-05-27 08:38:20.000000 django_botmanager-0.2.18/django_botmanager.egg-info/PKG-INFO
+-rw-rw-r--   0 titov     (1000) titov     (1000)     1133 2024-05-27 08:38:20.000000 django_botmanager-0.2.18/django_botmanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 titov     (1000) titov     (1000)        1 2024-05-27 08:38:20.000000 django_botmanager-0.2.18/django_botmanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 titov     (1000) titov     (1000)       52 2024-05-27 08:38:20.000000 django_botmanager-0.2.18/django_botmanager.egg-info/requires.txt
+-rw-rw-r--   0 titov     (1000) titov     (1000)       11 2024-05-27 08:38:20.000000 django_botmanager-0.2.18/django_botmanager.egg-info/top_level.txt
+-rw-rw-r--   0 titov     (1000) titov     (1000)       38 2024-05-27 08:38:20.188832 django_botmanager-0.2.18/setup.cfg
+-rw-rw-r--   0 titov     (1000) titov     (1000)      561 2024-05-27 08:35:52.000000 django_botmanager-0.2.18/setup.py
```

### Comparing `django-botmanager-0.2.17/LICENSE` & `django_botmanager-0.2.18/LICENSE`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/README.md` & `django_botmanager-0.2.18/README.md`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/basetask.py` & `django_botmanager-0.2.18/botmanager/basetask.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/management/commands/__init__.py` & `django_botmanager-0.2.18/botmanager/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/management/commands/bot_manager.py` & `django_botmanager-0.2.18/botmanager/management/commands/bot_manager.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/migrations/0001_initial.py` & `django_botmanager-0.2.18/botmanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/migrations/0002_auto_20161208_1406.py` & `django_botmanager-0.2.18/botmanager/migrations/0002_auto_20161208_1406.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/migrations/0003_auto_20161208_1529.py` & `django_botmanager-0.2.18/botmanager/migrations/0003_auto_20161208_1529.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/migrations/0004_auto_20161219_1931.py` & `django_botmanager-0.2.18/botmanager/migrations/0004_auto_20161219_1931.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/migrations/0005_task_parent.py` & `django_botmanager-0.2.18/botmanager/migrations/0005_task_parent.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/migrations/0007_task_is_persistent.py` & `django_botmanager-0.2.18/botmanager/migrations/0007_task_is_persistent.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/migrations/0008_auto_20170331_1752.py` & `django_botmanager-0.2.18/botmanager/migrations/0008_auto_20170331_1752.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/migrations/0010_auto_20170531_1321.py` & `django_botmanager-0.2.18/botmanager/migrations/0010_auto_20170531_1321.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/migrations/0011_alter_task_create_dt_alter_task_id.py` & `django_botmanager-0.2.18/botmanager/migrations/0011_alter_task_create_dt_alter_task_id.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/models.py` & `django_botmanager-0.2.18/botmanager/models.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/settings.py` & `django_botmanager-0.2.18/botmanager/settings.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/botmanager/utils.py` & `django_botmanager-0.2.18/botmanager/utils.py`

 * *Files identical despite different names*

### Comparing `django-botmanager-0.2.17/setup.py` & `django_botmanager-0.2.18/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 setup(
     name='django-botmanager',
-    version='0.2.17',
+    version='0.2.18',
     description='Async tasks for django',
     author='Dimoha',
     author_email='dimoha@controlstyle.ru',
     url='https://github.com/dimoha/django-botmanager',
     install_requires=[
         "setproctitle==1.1.10",
         "jsonfield==3.1.0",
         "psutil==5.8.0"
     ],
     packages=find_packages(),
     include_package_data=True,
     package_data={
         '': ['locale/*/LC_MESSAGES/*.mo', 'locale/*/LC_MESSAGES/*.po'],
     }
-)
+)
```

