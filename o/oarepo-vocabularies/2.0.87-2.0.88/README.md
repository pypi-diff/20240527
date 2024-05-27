# Comparing `tmp/oarepo_vocabularies-2.0.87.tar.gz` & `tmp/oarepo_vocabularies-2.0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo_vocabularies-2.0.87.tar", last modified: Mon Apr 29 13:35:28 2024, max compression
+gzip compressed data, was "oarepo_vocabularies-2.0.88.tar", last modified: Mon May 27 07:39:35 2024, max compression
```

## Comparing `oarepo_vocabularies-2.0.87.tar` & `oarepo_vocabularies-2.0.88.tar`

### file list

```diff
@@ -1,249 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.476331 oarepo_vocabularies-2.0.87/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-29 13:35:28.476331 oarepo_vocabularies-2.0.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.420331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.424331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/ext_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.424331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/hacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.424331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/models/ui.json
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.424331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.428331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.428331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/jsonschemas/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/systemfields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.428331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.428331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/records/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.428331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/vocabulary_type/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/vocabulary_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/vocabulary_type/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/vocabulary_type/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.432331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.432331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/components/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/components/scanning_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.432331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/custom_fields/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/type_ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/ui_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.432331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.436331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.436331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.436331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.436331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.436331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.408331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.436331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.440331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.440331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.440331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/components/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/components/deposit.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/components/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.440331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/vocabulary_type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/vocabulary_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/vocabulary_type/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.444331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/ITaxonomyArray.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/ITaxonomyItem.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/IVocabularyArray.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/IVocabularyItem.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/TaxonomyArray.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/VocabularyArray.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/VocabularyItem.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.412330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.448331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/SidebarLink.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesForm.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSearch.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/descendants.html
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.448331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.412330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.416330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.412330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.448331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.448331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.452331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.452331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.452331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.452331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.456331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.456331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.456331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.460331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.464331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.464331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.464331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.464331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.464331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/TreeSelectFieldModal.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/VocabularyTreeSelectField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/index.js
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.468331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.468331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.468331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.468331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/VocabularyButtonSidebar.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.468331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/translationKeys.js
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.412330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.468331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.472331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/tree-field.less
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.412330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.416330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.472331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/breadcrumb.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/grid.overrides
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.472331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/tree-field.variables
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/vocabulary_cf.variables
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.416330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.472331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.472331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.416330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.472331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.416330 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.472331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/webpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.476331 oarepo_vocabularies-2.0.87/oarepo_vocabularies/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/views/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies/views/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:35:28.476331 oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-29 13:35:28.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-04-29 13:35:28.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:35:28.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 13:35:28.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-29 13:35:28.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-29 13:35:28.000000 oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-29 13:35:28.476331 oarepo_vocabularies-2.0.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:26:44.000000 oarepo_vocabularies-2.0.87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.637565 oarepo_vocabularies-2.0.88/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-27 07:39:35.637565 oarepo_vocabularies-2.0.88/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.577565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.581565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/ext_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.581565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/resources/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/hacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.581565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/models/ui.json
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.585565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.585565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/records/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.585565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/records/jsonschemas/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/records/systemfields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.585565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.585565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/records/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.589565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/vocabulary_type/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/vocabulary_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/vocabulary_type/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/vocabulary_type/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.593565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.593565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/components/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/components/scanning_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.593565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/custom_fields/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/type_ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/ui_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.565565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.565565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.565565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.565565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.593565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.593565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.565565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.593565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.565565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.593565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.597565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.565565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.597565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.565565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.597565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.601565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.605565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.605565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/components/deposit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/components/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.605565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/vocabulary_type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/vocabulary_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/vocabulary_type/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.609565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/ITaxonomyArray.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/ITaxonomyItem.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/IVocabularyArray.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/IVocabularyItem.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/TaxonomyArray.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/VocabularyArray.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/VocabularyItem.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.569565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.609565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/SidebarLink.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesBreadcrumb.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesForm.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSearch.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/descendants.html
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.609565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.569565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.573565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.569565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.613565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.613565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.617565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.617565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.617565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.621565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.621565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.621565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.621565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.621565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.625565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.625565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.625565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.625565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.625565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/TreeSelectFieldModal.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/VocabularyTreeSelectField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.629565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.629565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.629565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.629565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/VocabularyButtonSidebar.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.629565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/translationKeys.js
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.573565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.629565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.633565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/tree-field.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.573565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.573565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.633565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/breadcrumb.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/grid.overrides
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.633565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/tree-field.variables
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/vocabulary_cf.variables
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.573565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.633565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.633565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.573565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.637565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.573565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.637565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/webpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.637565 oarepo_vocabularies-2.0.88/oarepo_vocabularies/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/views/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies/views/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:39:35.637565 oarepo_vocabularies-2.0.88/oarepo_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-27 07:39:35.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12775 2024-05-27 07:39:35.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:39:35.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-27 07:39:35.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 07:39:35.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 07:39:35.000000 oarepo_vocabularies-2.0.88/oarepo_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-27 07:39:35.637565 oarepo_vocabularies-2.0.88/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:31:04.000000 oarepo_vocabularies-2.0.88/setup.py
```

### Comparing `oarepo_vocabularies-2.0.87/LICENSE` & `oarepo_vocabularies-2.0.88/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/MANIFEST.in` & `oarepo_vocabularies-2.0.88/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/PKG-INFO` & `oarepo_vocabularies-2.0.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 2.0.87
+Version: 2.0.88
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: invenio-vocabularies
 Requires-Dist: oarepo-runtime>=1.4.44
 Requires-Dist: openpyxl
 Requires-Dist: oarepo-ui>=5.0.91
```

### Comparing `oarepo_vocabularies-2.0.87/README.md` & `oarepo_vocabularies-2.0.88/README.md`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/components.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 class AuthorityComponent(ServiceComponent):
     def create(self, identity, data=None, record=None, errors=None, **kwargs):
         self.lookup_and_store_authority_records(record)
 
     def update(self, identity, data=None, record=None, **kwargs):
         self.lookup_and_store_authority_records(record)
 
+    def update_draft(self, identity, data=None, record=None, **kwargs):
+        self.lookup_and_store_authority_records(record)
+
     def lookup_and_store_authority_records(self, record):
         for found_vocabulary in find_vocabulary_relations(record):
             try:
                 found_vocabulary.field.validate(raise_first_exception=False)
             except MultipleInvalidRelationErrors as e:
                 authority_service = authorities.get_authority_api(
                     found_vocabulary.vocabulary_type
```

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/ext.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/resources/resource.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/resources/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/authorities/service.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/authorities/service.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/config.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ext.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/fixtures.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/fixtures.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/hacks.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/hacks.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/models/ui.json` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/models/ui.json`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/proxies.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/proxies.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/api.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/records/api.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/records/systemfields.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/records/systemfields.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/config.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/records/ui.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/ui.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/vocabulary_type/config.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/vocabulary_type/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/resources/vocabulary_type/resource.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/resources/vocabulary_type/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/cache.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/cache.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/components/hierarchy.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/components/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/config.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/custom_fields/hierarchy.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/custom_fields/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/facets.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/facets.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/permissions.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/schema.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/schema.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/search.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/search.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/service.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/service.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/services/ui_schema.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/services/ui_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/translations/messages.pot` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/config.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/ext.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/components/deposit.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/components/deposit.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/config.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/resource.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/vocabulary_type/config.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/vocabulary_type/config.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/ITaxonomyItem.jinja` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/ITaxonomyItem.jinja`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/IVocabularyItem.jinja` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/IVocabularyItem.jinja`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/VocabularyItem.jinja` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/VocabularyItem.jinja`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,24 @@
 {%- block head_links %}
 {{ super() }}
 {{ webpack['oarepo_vocabularies_ui_components.css'] }}
 {%- endblock %}
 
 {% block record_main_content %}
 <oarepo_vocabularies_ui.VocabulariesMain metadata={metadata} ui={ui} url_prefix={url_prefix} record={record} extra_context={extra_context} d={d}></oarepo_vocabularies_ui.VocabulariesMain>
+{% block vocabulary_descendants %}
+{% set search_app_config = extra_context["search_app_config"] %}
+  {%- include "oarepo_vocabularies_ui/descendants.html" -%}
+{% endblock vocabulary_descendants %}
 {% endblock record_main_content %}
 
 {% block record_sidebar %}
 <oarepo_vocabularies_ui.VocabulariesSidebar metadata={metadata} ui={ui} url_prefix={url_prefix} record={record} extra_context={extra_context}></oarepo_vocabularies_ui.VocabulariesSidebar>
 {% endblock record_sidebar %}
 
-{% block page_body %}
-  {{ super() }}
-  <div class="ui center aligned container rel-mb-2">
-    {% block vocabulary_descendants %}
-      {% set search_app_config = extra_context["search_app_config"] %}
-        {%- include "oarepo_vocabularies_ui/descendants.html" -%}
-    {% endblock vocabulary_descendants %}
-  </div>
-{% endblock page_body %}
+
 
 {%- block javascript %}
 {{super()}}
 {{webpack["oarepo_vocabularies_detail.js"] }}
 {{webpack['oarepo_vocabularies_ui_components.js']}}
 {%- endblock%}
```

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-{#def metadata, ui, record, d #}
+{#def metadata, ui, record, d, extra_context #}
 
 <div class="vocabularies-main">
+  <VocabulariesBreadcrumb extra_context={extra_context} metadata={metadata} />
   <div class="flex align-items-center rel-mt-1">
     {% if record.icon %}
       <img class="ui image rel-mr-1" src={{record.icon}}>
     {% endif %}
     <h1 class="ui header display-inline mt-0" >{{metadata.title.capitalize() if metadata.title else _("Missing title")}}</h1>
   </div>
   <dl class="ui very basic table">
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
-{#def metadata, ui, record, d #}
+{#def metadata, ui, record, d, extra_context #}
 {% if record.icon %} [{{record.icon}}]{% endif %}
 ************ {{{{mmeettaaddaattaa..ttiittllee..ccaappiittaalliizzee(()) iiff mmeettaaddaattaa..ttiittllee eellssee __((""MMiissssiinngg
 ttiittllee""))}}}} ************
 {% set custom_field_name="VOCABULARIES_CF_UI." + record.type %}
```

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import React, { useMemo } from "react";
 import PropTypes from "prop-types";
 import { OverridableContext } from "react-overridable";
-import { Container, Grid, Label } from "semantic-ui-react";
+import { Container, Grid, Header } from "semantic-ui-react";
 import {
   EmptyResults,
   Error,
   ReactSearchKit,
   ResultsLoader,
   withState,
   InvenioSearchApi,
@@ -15,17 +15,17 @@
 import { i18next } from "@translations/oarepo_vocabularies_ui/i18next";
 import { SearchConfigurationContext } from "@js/invenio_search_ui/components";
 
 const OnResults = withState(Results);
 
 const CountElement = ({ totalResults }) => {
   return (
-    <Label size="large">
+    <Header as="h3">
       {i18next.t("totalDescendants", { count: totalResults })}
-    </Label>
+    </Header>
   );
 };
 
 CountElement.propTypes = {
   totalResults: PropTypes.number.isRequired,
 };
```

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/TreeSelectFieldModal.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/TreeSelectFieldModal.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/VocabularyTreeSelectField.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyTreeSelectField/VocabularyTreeSelectField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/tree-field.less` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/tree-field.less`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/theme/webpack.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/theme/webpack.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/utils.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/ui/views.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/ui/views.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/views/api.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/views/api.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies/views/app.py` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies/views/app.py`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/PKG-INFO` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 2.0.87
+Version: 2.0.88
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: invenio-vocabularies
 Requires-Dist: oarepo-runtime>=1.4.44
 Requires-Dist: openpyxl
 Requires-Dist: oarepo-ui>=5.0.91
```

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/SOURCES.txt` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 oarepo_vocabularies/ui/templates/IVocabularyArray.jinja
 oarepo_vocabularies/ui/templates/IVocabularyItem.jinja
 oarepo_vocabularies/ui/templates/TaxonomyArray.jinja
 oarepo_vocabularies/ui/templates/TaxonomyItem.jinja
 oarepo_vocabularies/ui/templates/VocabularyArray.jinja
 oarepo_vocabularies/ui/templates/VocabularyItem.jinja
 oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/SidebarLink.jinja
+oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesBreadcrumb.jinja
 oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja
 oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesForm.jinja
 oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja
 oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja
 oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSearch.jinja
 oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja
 oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/descendants.html
```

### Comparing `oarepo_vocabularies-2.0.87/oarepo_vocabularies.egg-info/entry_points.txt` & `oarepo_vocabularies-2.0.88/oarepo_vocabularies.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo_vocabularies-2.0.87/setup.cfg` & `oarepo_vocabularies-2.0.88/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-vocabularies
-version = 2.0.87
+version = 2.0.88
 description = Support for custom fields and hierarchy on Invenio vocabularies
 authors = Mirek Simek <miroslav.simek@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

