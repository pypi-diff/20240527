# Comparing `tmp/plonemeeting.restapi-2.5.tar.gz` & `tmp/plonemeeting.restapi-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plonemeeting.restapi-2.5.tar", last modified: Tue Mar 19 10:58:36 2024, max compression
+gzip compressed data, was "dist/plonemeeting.restapi-2.6.tar", last modified: Mon May 27 10:28:36 2024, max compression
```

## Comparing `plonemeeting.restapi-2.5.tar` & `plonemeeting.restapi-2.6.tar`

### file list

```diff
@@ -1,100 +1,101 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      657 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/LICENSE.rst
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      272 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/setuphandlers.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3300 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/get.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      725 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/users.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15615 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/add.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4315 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1667 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/meetingconfig.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6723 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/search.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1469 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/annex.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11176 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/attendees.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1421 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/infos.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1531 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/configure.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      475 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/imio.history.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/en/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/en/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      575 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/en/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      609 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/en/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      434 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/plone.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      609 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      667 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/imio.history.po
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      332 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/sync_pos.sh
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/profiles/testing/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/profiles/testing/metadata.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      176 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/profiles/default/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      181 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      240 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/profiles/default/rolemap.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      105 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/profiles/default/catalog.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1200 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/interfaces.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8670 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/utils.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9914 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/item.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2181 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5072 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/meetingconfig.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5028 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/user.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1366 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/held_position.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3579 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/dxfields.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25317 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/base.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1636 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/pod_template.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2522 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/atfields.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1847 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/summary.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2916 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/catalog.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3517 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/meeting.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2157 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/annex.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      741 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/converters.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      524 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      283 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/testing.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/deserializer/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      458 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/deserializer/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      952 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/deserializer/dxfields.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      879 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/deserializer/atfields.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/deserializer/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2354 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/deserializer/atcontent.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23606 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_attendees.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2746 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_infos.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1724 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/base.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5671 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_annexes.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24560 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_get.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8682 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13616 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_meetingconfig.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    45756 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_add.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7087 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_users.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    42090 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_search.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      330 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/overrides.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      183 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/restapi/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting.restapi.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting.restapi.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      145 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting.restapi.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting.restapi.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting.restapi.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24581 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting.restapi.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3536 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting.restapi.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting.restapi.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/src/plonemeeting.restapi.egg-info/requires.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      125 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/bootstrap.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       61 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/requirements.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1743 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24581 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      167 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18369 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1162 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      469 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/Makefile
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      199 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/README.md
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2024-03-19 10:58:36.000000 plonemeeting.restapi-2.5/setup.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      657 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/LICENSE.rst
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      272 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/setuphandlers.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3300 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/get.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      725 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/users.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    15615 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/add.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4315 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1667 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/meetingconfig.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6723 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/search.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1469 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/annex.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11176 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/attendees.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1421 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/infos.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1531 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/configure.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      475 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/imio.history.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/en/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      575 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/en/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      609 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/en/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      434 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/plone.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      609 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      672 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/imio.history.po
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      332 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/sync_pos.sh
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/profiles/testing/metadata.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      176 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      181 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      240 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/profiles/default/rolemap.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      105 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/profiles/default/catalog.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1200 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      256 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8670 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/utils.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9914 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/item.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2181 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5072 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/meetingconfig.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5028 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/user.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1366 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/held_position.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3579 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/dxfields.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25317 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/base.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1636 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/pod_template.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2522 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/atfields.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1847 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/summary.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2916 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/catalog.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3517 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/meeting.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2157 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/annex.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      741 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/converters.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      524 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      283 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/testing.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/deserializer/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      458 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/deserializer/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      952 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/deserializer/dxfields.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      879 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/deserializer/atfields.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/deserializer/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2354 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/deserializer/atcontent.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    23606 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_attendees.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2746 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_infos.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3937 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_delete.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1724 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/base.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5671 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_annexes.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    24560 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_get.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8682 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    13616 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_meetingconfig.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    46241 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_add.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7087 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_users.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    42090 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_search.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      330 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/overrides.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      183 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/restapi/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       80 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting.restapi.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting.restapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      145 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting.restapi.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting.restapi.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       13 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting.restapi.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25036 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting.restapi.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3591 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting.restapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting.restapi.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/src/plonemeeting.restapi.egg-info/requires.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      125 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/bootstrap.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       61 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/requirements.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1743 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    25036 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      167 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18736 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1162 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      469 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/Makefile
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      199 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/README.md
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      366 2024-05-27 10:28:36.000000 plonemeeting.restapi-2.6/setup.cfg
```

### Comparing `plonemeeting.restapi-2.5/LICENSE.rst` & `plonemeeting.restapi-2.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/get.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/get.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/users.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/users.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/add.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/add.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/configure.zcml` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/meetingconfig.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/meetingconfig.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/search.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/search.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/annex.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/annex.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/attendees.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/attendees.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/services/infos.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/services/infos.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/configure.zcml` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/en/LC_MESSAGES/plone.po` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/en/LC_MESSAGES/imio.history.po` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/en/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/plone.po` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/imio.history.po` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files 25% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: DOMAIN\n"
 
 #. Default: "This item has been created using the Webservice (rest)."
 msgid "create_element_using_ws_rest_comments"
-msgstr "Ce point a été créé depuis un appel WebService (REST)."
+msgstr "Cet élément a été créé depuis un appel WebService (REST)."
```

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/testing.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/testing.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/utils.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/utils.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/item.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/item.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/configure.zcml` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/configure.zcml`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/meetingconfig.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/meetingconfig.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/user.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/user.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/held_position.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/held_position.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/dxfields.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/dxfields.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/base.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/base.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/pod_template.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/pod_template.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/atfields.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/atfields.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/summary.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/summary.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/catalog.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/catalog.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/meeting.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/meeting.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/annex.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/annex.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/serializer/converters.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/serializer/converters.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/config.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/config.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/deserializer/dxfields.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/deserializer/dxfields.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/deserializer/atfields.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/deserializer/atfields.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/deserializer/atcontent.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/deserializer/atcontent.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_attendees.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_attendees.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_infos.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_infos.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/base.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/base.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_annexes.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_annexes.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_get.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_get.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/config.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/config.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_meetingconfig.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_meetingconfig.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_add.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_add.py`

 * *Files 2% similar despite different names*

```diff
@@ -852,31 +852,42 @@
             "config_id": cfg.getId(),
             "proposingGroup": self.developers.getId(),
             "title": "My item",
             "__children__": [
                 {
                     "@type": "annex",
                     "title": "My annex 1",
-                    "content_category": "item-annex",
+                    "content_category": "preview-annex",
                     "file": {
                         "data": "123456",
                         "encoding": "ascii",
                         "filename": "file.txt",
                     },
                 },
                 {
                     "@type": "annex",
                     "title": "My annex 2",
-                    "content_category": "item-annex",
+                    "content_category": "preview-annex",
                     "file": {"data": base64_pdf_data, "filename": "file.pdf"},
                 },
             ],
         }
         response = self.api_session.post(endpoint_url, json=json)
         transaction.commit()
+        self.assertEqual(response.status_code, 400)
+        self.assertEqual(
+            response.json(),
+            {u'message': u"[{'message': 'You must select a PDF file!', "
+                         u"'error': 'ValidationError'}]",
+             u'type': u'BadRequest'}
+        )
+        # fix annex1 annex type
+        json['__children__'][0]["content_category"] = "item-annex"
+        response = self.api_session.post(endpoint_url, json=json)
+        transaction.commit()
         # this tries to manage randomly failing test
         try:
             self.assertEqual(response.status_code, 201, response.content)
         except Exception:
             response = self.api_session.post(endpoint_url, json=json)
             transaction.commit()
             self.assertEqual(response.status_code, 201, response.content)
```

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_users.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_users.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting/restapi/tests/test_services_search.py` & `plonemeeting.restapi-2.6/src/plonemeeting/restapi/tests/test_services_search.py`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting.restapi.egg-info/PKG-INFO` & `plonemeeting.restapi-2.6/src/plonemeeting.restapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plonemeeting.restapi
-Version: 2.5
+Version: 2.6
 Summary: Extended rest api service for Products.PloneMeeting usecases
 Home-page: https://pypi.python.org/pypi/plonemeeting.restapi
 Author: Gauthier Bastien
 Author-email: gauthier@imio.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -56,14 +56,25 @@
         
         Changelog
         =========
         
         Version 1.x is for PloneMeeting 4.1.x, version 2.x is for PloneMeeting 4.2.x+
         
         
+        2.6 (2024-05-27)
+        ----------------
+        
+        - Adapted `test_restapi_add_item_with_annexes_children` to show that annex
+          `content_category` `only_pdf` parameter is taken into account.
+          [gbastien]
+        - Added `testServiceDelete` to show that the `DELETE` method works as expected.
+          [gbastien]
+        - Fixed french translation for `create_element_using_ws_rest_comments`.
+          [gbastien]
+        
         2.5 (2024-03-19)
         ----------------
         
         - When using `fullobjects`, only serialize `next/previous` when specifically
           asked using `include_nextprev=true`.
           [gbastien]
```

### Comparing `plonemeeting.restapi-2.5/src/plonemeeting.restapi.egg-info/SOURCES.txt` & `plonemeeting.restapi-2.6/src/plonemeeting.restapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -71,12 +71,13 @@
 src/plonemeeting/restapi/services/users.py
 src/plonemeeting/restapi/tests/__init__.py
 src/plonemeeting/restapi/tests/base.py
 src/plonemeeting/restapi/tests/config.py
 src/plonemeeting/restapi/tests/test_services_add.py
 src/plonemeeting/restapi/tests/test_services_annexes.py
 src/plonemeeting/restapi/tests/test_services_attendees.py
+src/plonemeeting/restapi/tests/test_services_delete.py
 src/plonemeeting/restapi/tests/test_services_get.py
 src/plonemeeting/restapi/tests/test_services_infos.py
 src/plonemeeting/restapi/tests/test_services_meetingconfig.py
 src/plonemeeting/restapi/tests/test_services_search.py
 src/plonemeeting/restapi/tests/test_services_users.py
```

### Comparing `plonemeeting.restapi-2.5/setup.py` & `plonemeeting.restapi-2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 long_description = "\n\n".join(
     [open("README.rst").read(), open("CHANGES.rst").read(), ])
 
 
 setup(
     name="plonemeeting.restapi",
-    version="2.5",
+    version="2.6",
     description="Extended rest api service for Products.PloneMeeting usecases",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `plonemeeting.restapi-2.5/PKG-INFO` & `plonemeeting.restapi-2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plonemeeting.restapi
-Version: 2.5
+Version: 2.6
 Summary: Extended rest api service for Products.PloneMeeting usecases
 Home-page: https://pypi.python.org/pypi/plonemeeting.restapi
 Author: Gauthier Bastien
 Author-email: gauthier@imio.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -56,14 +56,25 @@
         
         Changelog
         =========
         
         Version 1.x is for PloneMeeting 4.1.x, version 2.x is for PloneMeeting 4.2.x+
         
         
+        2.6 (2024-05-27)
+        ----------------
+        
+        - Adapted `test_restapi_add_item_with_annexes_children` to show that annex
+          `content_category` `only_pdf` parameter is taken into account.
+          [gbastien]
+        - Added `testServiceDelete` to show that the `DELETE` method works as expected.
+          [gbastien]
+        - Fixed french translation for `create_element_using_ws_rest_comments`.
+          [gbastien]
+        
         2.5 (2024-03-19)
         ----------------
         
         - When using `fullobjects`, only serialize `next/previous` when specifically
           asked using `include_nextprev=true`.
           [gbastien]
```

### Comparing `plonemeeting.restapi-2.5/CHANGES.rst` & `plonemeeting.restapi-2.6/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 Changelog
 =========
 
 Version 1.x is for PloneMeeting 4.1.x, version 2.x is for PloneMeeting 4.2.x+
 
 
+2.6 (2024-05-27)
+----------------
+
+- Adapted `test_restapi_add_item_with_annexes_children` to show that annex
+  `content_category` `only_pdf` parameter is taken into account.
+  [gbastien]
+- Added `testServiceDelete` to show that the `DELETE` method works as expected.
+  [gbastien]
+- Fixed french translation for `create_element_using_ws_rest_comments`.
+  [gbastien]
+
 2.5 (2024-03-19)
 ----------------
 
 - When using `fullobjects`, only serialize `next/previous` when specifically
   asked using `include_nextprev=true`.
   [gbastien]
```

### Comparing `plonemeeting.restapi-2.5/README.rst` & `plonemeeting.restapi-2.6/README.rst`

 * *Files identical despite different names*

### Comparing `plonemeeting.restapi-2.5/LICENSE.GPL` & `plonemeeting.restapi-2.6/LICENSE.GPL`

 * *Files identical despite different names*

