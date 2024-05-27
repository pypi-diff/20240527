# Comparing `tmp/imio.restapi-1.0rc1.tar.gz` & `tmp/imio.restapi-1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.restapi-1.0rc1.tar", last modified: Thu Mar 14 14:18:27 2024, max compression
+gzip compressed data, was "dist/imio.restapi-1.0rc2.tar", last modified: Mon May 27 10:28:00 2024, max compression
```

## Comparing `imio.restapi-1.0rc1.tar` & `imio.restapi-1.0rc2.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      657 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/LICENSE.rst
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio.restapi.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio.restapi.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      137 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio.restapi.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio.restapi.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio.restapi.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13254 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio.restapi.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3397 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio.restapi.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio.restapi.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      282 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio.restapi.egg-info/requires.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/settings/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      787 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/settings/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      612 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/settings/view.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2702 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/settings/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1663 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/settings/dataprovider.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/settings/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/form/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5984 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/form/tools.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7520 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/form/form.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      983 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/form/action.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      606 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/form/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4129 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/form/link.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/form/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      396 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/form/templates/action.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      119 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/form/templates/link.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      966 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/form/importer.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/form/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      589 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/setuphandlers.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/services/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1187 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/services/at.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2097 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/services/request_schema.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9809 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/services/add.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1399 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/services/transition.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4100 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/services/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2770 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/services/rest_link.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1696 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/services/uid.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2478 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/services/search.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2270 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/services/pod.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1115 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/services/update.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4569 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/services/infos.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/services/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1370 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      737 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/imio.history.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2345 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/imio.restapi.pot
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      535 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/update.sh
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2447 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/en/LC_MESSAGES/imio.restapi.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      682 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/en/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      611 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1320 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/update.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3229 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/fr/LC_MESSAGES/imio.restapi.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      689 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/fr/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/locales/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/vocabularies/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      781 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/vocabularies/applications.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      368 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/vocabularies/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4973 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/vocabularies/base.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/vocabularies/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      162 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/profiles/default/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      182 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      183 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/profiles/default/registry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      118 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/profiles/default/rolemap.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      105 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/profiles/default/catalog.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      483 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/profiles/default/controlpanel.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/profiles/uninstall/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      122 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2993 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1761 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4874 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/utils.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/serializer/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      414 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/serializer/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      875 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/serializer/rest_link.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3387 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/serializer/base.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/serializer/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5923 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/tests/test_service_transition.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3555 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/tests/test_service_infos.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      754 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/tests/test_utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3788 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/tests/test_service_pod.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1088 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/tests/test_service_search.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11979 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/tests/test_service_add.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2967 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/tests/test_service_update.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1917 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/tests/test_setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      181 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/upgrades.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1942 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/browser/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      901 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/browser/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1380 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/browser/viewlets.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/browser/templates/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      528 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/browser/templates/link-viewlet.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      473 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/browser/templates/action-viewlet.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      775 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/restapi/upgrades.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/src/imio/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       59 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/docs/index.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       39 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/requirements.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2278 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13254 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      127 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7267 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/CONTRIBUTORS.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2147 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      297 2024-03-14 14:18:27.000000 imio.restapi-1.0rc1/DEVELOP.rst
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      657 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/LICENSE.rst
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio.restapi.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio.restapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      137 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio.restapi.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio.restapi.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio.restapi.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13410 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio.restapi.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3397 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio.restapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio.restapi.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      282 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio.restapi.egg-info/requires.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/settings/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      787 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/settings/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      612 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/settings/view.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2702 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/settings/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1663 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/settings/dataprovider.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/settings/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/form/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5984 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/form/tools.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7520 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/form/form.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      983 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/form/action.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      606 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/form/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4129 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/form/link.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/form/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      396 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/form/templates/action.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      119 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/form/templates/link.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      966 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/form/importer.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/form/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      589 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/setuphandlers.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/services/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1187 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/services/at.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2097 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/services/request_schema.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9809 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/services/add.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1399 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/services/transition.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4100 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/services/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2770 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/services/rest_link.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1696 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/services/uid.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2478 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/services/search.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2270 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/services/pod.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1115 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/services/update.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4569 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/services/infos.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/services/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1370 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      737 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/imio.history.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2345 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/imio.restapi.pot
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      535 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/update.sh
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/en/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2447 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/en/LC_MESSAGES/imio.restapi.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      682 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/en/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      611 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1320 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/update.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3229 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/fr/LC_MESSAGES/imio.restapi.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      689 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/fr/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/locales/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/vocabularies/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      781 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/vocabularies/applications.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      368 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/vocabularies/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4973 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/vocabularies/base.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/vocabularies/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      162 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      182 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      183 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/profiles/default/registry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      118 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/profiles/default/rolemap.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      105 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/profiles/default/catalog.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      483 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/profiles/default/controlpanel.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/profiles/uninstall/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      122 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2993 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1761 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4874 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/utils.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/serializer/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      414 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/serializer/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      875 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/serializer/rest_link.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3387 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/serializer/base.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/serializer/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5923 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/tests/test_service_transition.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3555 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/tests/test_service_infos.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      754 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/tests/test_utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3788 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/tests/test_service_pod.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1088 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/tests/test_service_search.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11979 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/tests/test_service_add.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2967 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/tests/test_service_update.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1917 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/tests/test_setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      181 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/upgrades.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2000 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/browser/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      901 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/browser/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1380 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/browser/viewlets.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/browser/templates/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      528 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/browser/templates/link-viewlet.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      473 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/browser/templates/action-viewlet.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      775 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/restapi/upgrades.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/src/imio/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       59 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/docs/index.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       39 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/requirements.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2278 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13410 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      127 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7375 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       73 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/CONTRIBUTORS.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2147 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      297 2024-05-27 10:28:00.000000 imio.restapi-1.0rc2/DEVELOP.rst
```

### Comparing `imio.restapi-1.0rc1/LICENSE.rst` & `imio.restapi-1.0rc2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio.restapi.egg-info/PKG-INFO` & `imio.restapi-1.0rc2/src/imio.restapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.restapi
-Version: 1.0rc1
+Version: 1.0rc2
 Summary: Extended rest api service for IMIO usecases
 Home-page: https://pypi.python.org/pypi/imio.restapi
 Author: Martin Peeters
 Author-email: martin.peeters@affinitic.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -84,14 +84,20 @@
         - Martin Peeters [Affinitic], Original author
         
         
         Changelog
         =========
         
         
+        1.0rc2 (2024-05-27)
+        -------------------
+        
+        - Do not fail to log restapi call when using DELETE.
+          [gbastien]
+        
         1.0rc1 (2024-03-14)
         -------------------
         
         - Moved unused `utils.listify` to `imio.pyutils.utils.listify`.
           [gbastien]
         - When using a `base_search_uid` take also `sort_on/sort_order`
           defined on the Collection.
```

### Comparing `imio.restapi-1.0rc1/src/imio.restapi.egg-info/SOURCES.txt` & `imio.restapi-1.0rc2/src/imio.restapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/settings/configure.zcml` & `imio.restapi-1.0rc2/src/imio/restapi/settings/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/settings/view.py` & `imio.restapi-1.0rc2/src/imio/restapi/settings/view.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/settings/interfaces.py` & `imio.restapi-1.0rc2/src/imio/restapi/settings/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/settings/dataprovider.py` & `imio.restapi-1.0rc2/src/imio/restapi/settings/dataprovider.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/form/tools.py` & `imio.restapi-1.0rc2/src/imio/restapi/form/tools.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/form/form.py` & `imio.restapi-1.0rc2/src/imio/restapi/form/form.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/form/action.py` & `imio.restapi-1.0rc2/src/imio/restapi/form/action.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/form/configure.zcml` & `imio.restapi-1.0rc2/src/imio/restapi/form/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/form/link.py` & `imio.restapi-1.0rc2/src/imio/restapi/form/link.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/form/importer.py` & `imio.restapi-1.0rc2/src/imio/restapi/form/importer.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/setuphandlers.py` & `imio.restapi-1.0rc2/src/imio/restapi/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/services/at.py` & `imio.restapi-1.0rc2/src/imio/restapi/services/at.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/services/request_schema.py` & `imio.restapi-1.0rc2/src/imio/restapi/services/request_schema.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/services/add.py` & `imio.restapi-1.0rc2/src/imio/restapi/services/add.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/services/transition.py` & `imio.restapi-1.0rc2/src/imio/restapi/services/transition.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/services/configure.zcml` & `imio.restapi-1.0rc2/src/imio/restapi/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/services/rest_link.py` & `imio.restapi-1.0rc2/src/imio/restapi/services/rest_link.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/services/uid.py` & `imio.restapi-1.0rc2/src/imio/restapi/services/uid.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/services/search.py` & `imio.restapi-1.0rc2/src/imio/restapi/services/search.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/services/pod.py` & `imio.restapi-1.0rc2/src/imio/restapi/services/pod.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/services/update.py` & `imio.restapi-1.0rc2/src/imio/restapi/services/update.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/services/infos.py` & `imio.restapi-1.0rc2/src/imio/restapi/services/infos.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/configure.zcml` & `imio.restapi-1.0rc2/src/imio/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/locales/imio.history.pot` & `imio.restapi-1.0rc2/src/imio/restapi/locales/imio.history.pot`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/locales/imio.restapi.pot` & `imio.restapi-1.0rc2/src/imio/restapi/locales/imio.restapi.pot`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/locales/update.sh` & `imio.restapi-1.0rc2/src/imio/restapi/locales/update.sh`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/locales/en/LC_MESSAGES/imio.restapi.po` & `imio.restapi-1.0rc2/src/imio/restapi/locales/en/LC_MESSAGES/imio.restapi.po`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/locales/en/LC_MESSAGES/imio.history.po` & `imio.restapi-1.0rc2/src/imio/restapi/locales/en/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/locales/README.rst` & `imio.restapi-1.0rc2/src/imio/restapi/locales/README.rst`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/locales/update.py` & `imio.restapi-1.0rc2/src/imio/restapi/locales/update.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/locales/fr/LC_MESSAGES/imio.restapi.po` & `imio.restapi-1.0rc2/src/imio/restapi/locales/fr/LC_MESSAGES/imio.restapi.po`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/locales/fr/LC_MESSAGES/imio.history.po` & `imio.restapi-1.0rc2/src/imio/restapi/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/vocabularies/applications.py` & `imio.restapi-1.0rc2/src/imio/restapi/vocabularies/applications.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/vocabularies/base.py` & `imio.restapi-1.0rc2/src/imio/restapi/vocabularies/base.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/testing.py` & `imio.restapi-1.0rc2/src/imio/restapi/testing.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/interfaces.py` & `imio.restapi-1.0rc2/src/imio/restapi/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/utils.py` & `imio.restapi-1.0rc2/src/imio/restapi/utils.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/serializer/rest_link.py` & `imio.restapi-1.0rc2/src/imio/restapi/serializer/rest_link.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/serializer/base.py` & `imio.restapi-1.0rc2/src/imio/restapi/serializer/base.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/tests/test_service_transition.py` & `imio.restapi-1.0rc2/src/imio/restapi/tests/test_service_transition.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/tests/test_service_infos.py` & `imio.restapi-1.0rc2/src/imio/restapi/tests/test_service_infos.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/tests/test_utils.py` & `imio.restapi-1.0rc2/src/imio/restapi/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/tests/test_service_pod.py` & `imio.restapi-1.0rc2/src/imio/restapi/tests/test_service_pod.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/tests/test_service_search.py` & `imio.restapi-1.0rc2/src/imio/restapi/tests/test_service_search.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/tests/test_service_add.py` & `imio.restapi-1.0rc2/src/imio/restapi/tests/test_service_add.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/tests/test_service_update.py` & `imio.restapi-1.0rc2/src/imio/restapi/tests/test_service_update.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/tests/test_setup.py` & `imio.restapi-1.0rc2/src/imio/restapi/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/__init__.py` & `imio.restapi-1.0rc2/src/imio/restapi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     # log the input when debug is enabled
     if debug:
         # with POST, data is in the body
         if self.request.get('method', 'GET') != 'GET':
             data = json_body(self.request)
             fplog("restapi_call_debug",
                   extras="INPUT: \n" + json.dumps(data, indent=4, sort_keys=True))
-    res = self.__old_pm_render()
+    # res can be None when using DELETE for example
+    res = self.__old_pm_render() or ""
     # log the output when debug is enabled
     if debug:
         fplog("restapi_call_debug", extras="OUTPUT: \n" + res)
     return res
 
 
 Service.render = render
```

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/browser/configure.zcml` & `imio.restapi-1.0rc2/src/imio/restapi/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/browser/viewlets.py` & `imio.restapi-1.0rc2/src/imio/restapi/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/browser/templates/link-viewlet.pt` & `imio.restapi-1.0rc2/src/imio/restapi/browser/templates/link-viewlet.pt`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/src/imio/restapi/upgrades.zcml` & `imio.restapi-1.0rc2/src/imio/restapi/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/setup.py` & `imio.restapi-1.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.restapi",
-    version="1.0rc1",
+    version="1.0rc2",
     description="Extended rest api service for IMIO usecases",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 6 - Mature",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `imio.restapi-1.0rc1/PKG-INFO` & `imio.restapi-1.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.restapi
-Version: 1.0rc1
+Version: 1.0rc2
 Summary: Extended rest api service for IMIO usecases
 Home-page: https://pypi.python.org/pypi/imio.restapi
 Author: Martin Peeters
 Author-email: martin.peeters@affinitic.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -84,14 +84,20 @@
         - Martin Peeters [Affinitic], Original author
         
         
         Changelog
         =========
         
         
+        1.0rc2 (2024-05-27)
+        -------------------
+        
+        - Do not fail to log restapi call when using DELETE.
+          [gbastien]
+        
         1.0rc1 (2024-03-14)
         -------------------
         
         - Moved unused `utils.listify` to `imio.pyutils.utils.listify`.
           [gbastien]
         - When using a `base_search_uid` take also `sort_on/sort_order`
           defined on the Collection.
```

### Comparing `imio.restapi-1.0rc1/CHANGES.rst` & `imio.restapi-1.0rc2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog
 =========
 
 
+1.0rc2 (2024-05-27)
+-------------------
+
+- Do not fail to log restapi call when using DELETE.
+  [gbastien]
+
 1.0rc1 (2024-03-14)
 -------------------
 
 - Moved unused `utils.listify` to `imio.pyutils.utils.listify`.
   [gbastien]
 - When using a `base_search_uid` take also `sort_on/sort_order`
   defined on the Collection.
```

### Comparing `imio.restapi-1.0rc1/README.rst` & `imio.restapi-1.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `imio.restapi-1.0rc1/LICENSE.GPL` & `imio.restapi-1.0rc2/LICENSE.GPL`

 * *Files identical despite different names*

