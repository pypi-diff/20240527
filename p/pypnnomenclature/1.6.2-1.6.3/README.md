# Comparing `tmp/pypnnomenclature-1.6.2.tar.gz` & `tmp/pypnnomenclature-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypnnomenclature-1.6.2.tar", last modified: Fri Apr 26 09:51:17 2024, max compression
+gzip compressed data, was "pypnnomenclature-1.6.3.tar", last modified: Mon May 27 13:36:48 2024, max compression
```

## Comparing `pypnnomenclature-1.6.2.tar` & `pypnnomenclature-1.6.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:17.040634 pypnnomenclature-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-26 09:51:17.040634 pypnnomenclature-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 09:51:17.040634 pypnnomenclature-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:17.032634 pypnnomenclature-1.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:17.032634 pypnnomenclature-1.6.2/src/pypnnomenclature/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:17.036634 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:17.036634 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13365 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/data/nomenclatures.sql
--rw-r--r--   0 runner    (1001) docker     (127)   199614 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/data/nomenclatures_inpn_data.sql
--rw-r--r--   0 runner    (1001) docker     (127)    15473 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/data/nomenclatures_taxonomie.sql
--rw-r--r--   0 runner    (1001) docker     (127)    67206 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/data/nomenclatures_taxonomie_data.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:17.040634 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/11e7741319fd_get_default_nomenclature_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/6015397d686a_nomenclatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/618542880d1f_fix_typo_nomenc_type_def.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/803524258bd3_add_group3_inpn_cor_taxref.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/96a713739fdd_nomenclatures_inpn_data.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/a763fb554ff2_nomenclatures_taxonomie_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/b820c66d8daa_get_nomenclature_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     9962 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/ee1146f6c0f4_add_uicn_rl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/f5436084bf17_nomenclatures_taxonomie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/f8c2c8482419_get_default_nomenclature_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:17.040634 pypnnomenclature-1.6.2/src/pypnnomenclature/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/tests/test_nomenclatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-26 09:51:13.000000 pypnnomenclature-1.6.2/src/pypnnomenclature/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:51:17.040634 pypnnomenclature-1.6.2/src/pypnnomenclature.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-26 09:51:17.000000 pypnnomenclature-1.6.2/src/pypnnomenclature.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-26 09:51:17.000000 pypnnomenclature-1.6.2/src/pypnnomenclature.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:51:17.000000 pypnnomenclature-1.6.2/src/pypnnomenclature.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-26 09:51:17.000000 pypnnomenclature-1.6.2/src/pypnnomenclature.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-26 09:51:17.000000 pypnnomenclature-1.6.2/src/pypnnomenclature.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 09:51:17.000000 pypnnomenclature-1.6.2/src/pypnnomenclature.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:48.717210 pypnnomenclature-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-27 13:36:48.717210 pypnnomenclature-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:36:48.717210 pypnnomenclature-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:48.709210 pypnnomenclature-1.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:48.713210 pypnnomenclature-1.6.3/src/pypnnomenclature/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:48.713210 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:48.713210 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13365 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/data/nomenclatures.sql
+-rw-r--r--   0 runner    (1001) docker     (127)   199614 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/data/nomenclatures_inpn_data.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    15473 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/data/nomenclatures_taxonomie.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    67206 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/data/nomenclatures_taxonomie_data.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:48.717210 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/11e7741319fd_get_default_nomenclature_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/6015397d686a_nomenclatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/618542880d1f_fix_typo_nomenc_type_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/803524258bd3_add_group3_inpn_cor_taxref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/96a713739fdd_nomenclatures_inpn_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/a763fb554ff2_nomenclatures_taxonomie_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/b820c66d8daa_get_nomenclature_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9962 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/ee1146f6c0f4_add_uicn_rl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/f5436084bf17_nomenclatures_taxonomie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/f8c2c8482419_get_default_nomenclature_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:48.717210 pypnnomenclature-1.6.3/src/pypnnomenclature/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/tests/test_nomenclatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-27 13:36:43.000000 pypnnomenclature-1.6.3/src/pypnnomenclature/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:48.717210 pypnnomenclature-1.6.3/src/pypnnomenclature.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-27 13:36:48.000000 pypnnomenclature-1.6.3/src/pypnnomenclature.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-27 13:36:48.000000 pypnnomenclature-1.6.3/src/pypnnomenclature.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:36:48.000000 pypnnomenclature-1.6.3/src/pypnnomenclature.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 13:36:48.000000 pypnnomenclature-1.6.3/src/pypnnomenclature.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-27 13:36:48.000000 pypnnomenclature-1.6.3/src/pypnnomenclature.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 13:36:48.000000 pypnnomenclature-1.6.3/src/pypnnomenclature.egg-info/top_level.txt
```

### Comparing `pypnnomenclature-1.6.2/LICENSE` & `pypnnomenclature-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/PKG-INFO` & `pypnnomenclature-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypnnomenclature
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python lib related to nomenclatures
 Home-page: https://github.com/PnX-SI/Nomenclature-api-module
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -21,16 +21,16 @@
 Requires-Dist: flask-sqlalchemy
 Requires-Dist: flask-migrate
 Requires-Dist: psycopg2
 Requires-Dist: flask-marshmallow
 Requires-Dist: marshmallow-sqlalchemy
 Requires-Dist: sqlalchemy
 Requires-Dist: utils-flask-sqlalchemy>=0.4.1
-Requires-Dist: taxhub>=1.14.0
-Requires-Dist: pypnusershub>=2.1.4
+Requires-Dist: taxhub>=1.14.1
+Requires-Dist: pypnusershub>=2.1.5
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-flask; extra == "tests"
 
 # Nomenclature-api-module
 
 [![pytest](https://github.com/PnX-SI/Nomenclature-api-module/actions/workflows/pytest.yml/badge.svg)](https://github.com/PnX-SI/Nomenclature-api-module/actions/workflows/pytest.yml)
```

### Comparing `pypnnomenclature-1.6.2/README.md` & `pypnnomenclature-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/setup.py` & `pypnnomenclature-1.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/__init__.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/__init__.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/admin.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/admin.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/env.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/env.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/data/nomenclatures.sql` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/data/nomenclatures.sql`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/data/nomenclatures_inpn_data.sql` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/data/nomenclatures_inpn_data.sql`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/data/nomenclatures_taxonomie.sql` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/data/nomenclatures_taxonomie.sql`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/data/nomenclatures_taxonomie_data.sql` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/data/nomenclatures_taxonomie_data.sql`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/env.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/env.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/11e7741319fd_get_default_nomenclature_value.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/11e7741319fd_get_default_nomenclature_value.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/6015397d686a_nomenclatures.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/6015397d686a_nomenclatures.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/618542880d1f_fix_typo_nomenc_type_def.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/618542880d1f_fix_typo_nomenc_type_def.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/803524258bd3_add_group3_inpn_cor_taxref.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/803524258bd3_add_group3_inpn_cor_taxref.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/96a713739fdd_nomenclatures_inpn_data.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/96a713739fdd_nomenclatures_inpn_data.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/a763fb554ff2_nomenclatures_taxonomie_data.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/a763fb554ff2_nomenclatures_taxonomie_data.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/b820c66d8daa_get_nomenclature_label.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/b820c66d8daa_get_nomenclature_label.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/ee1146f6c0f4_add_uicn_rl.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/ee1146f6c0f4_add_uicn_rl.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/f5436084bf17_nomenclatures_taxonomie.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/f5436084bf17_nomenclatures_taxonomie.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/migrations/versions/f8c2c8482419_get_default_nomenclature_value.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/migrations/versions/f8c2c8482419_get_default_nomenclature_value.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/models.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/models.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/repository.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/repository.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/routes.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/routes.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/tests/test_nomenclatures.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/tests/test_nomenclatures.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature/utils.py` & `pypnnomenclature-1.6.3/src/pypnnomenclature/utils.py`

 * *Files identical despite different names*

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature.egg-info/PKG-INFO` & `pypnnomenclature-1.6.3/src/pypnnomenclature.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypnnomenclature
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python lib related to nomenclatures
 Home-page: https://github.com/PnX-SI/Nomenclature-api-module
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -21,16 +21,16 @@
 Requires-Dist: flask-sqlalchemy
 Requires-Dist: flask-migrate
 Requires-Dist: psycopg2
 Requires-Dist: flask-marshmallow
 Requires-Dist: marshmallow-sqlalchemy
 Requires-Dist: sqlalchemy
 Requires-Dist: utils-flask-sqlalchemy>=0.4.1
-Requires-Dist: taxhub>=1.14.0
-Requires-Dist: pypnusershub>=2.1.4
+Requires-Dist: taxhub>=1.14.1
+Requires-Dist: pypnusershub>=2.1.5
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-flask; extra == "tests"
 
 # Nomenclature-api-module
 
 [![pytest](https://github.com/PnX-SI/Nomenclature-api-module/actions/workflows/pytest.yml/badge.svg)](https://github.com/PnX-SI/Nomenclature-api-module/actions/workflows/pytest.yml)
```

### Comparing `pypnnomenclature-1.6.2/src/pypnnomenclature.egg-info/SOURCES.txt` & `pypnnomenclature-1.6.3/src/pypnnomenclature.egg-info/SOURCES.txt`

 * *Files identical despite different names*

