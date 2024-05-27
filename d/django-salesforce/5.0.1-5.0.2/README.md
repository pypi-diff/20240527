# Comparing `tmp/django-salesforce-5.0.1.tar.gz` & `tmp/django-salesforce-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-salesforce-5.0.1.tar", last modified: Mon Mar  4 18:44:03 2024, max compression
+gzip compressed data, was "django-salesforce-5.0.2.tar", last modified: Mon May 27 14:30:23 2024, max compression
```

## Comparing `django-salesforce-5.0.1.tar` & `django-salesforce-5.0.2.tar`

### file list

```diff
@@ -1,245 +1,246 @@
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.224871 django-salesforce-5.0.1/
--rw-r--r--   0 philchristensen   (502) staff       (20)      475 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/.coveragerc
--rw-r--r--   0 philchristensen   (502) staff       (20)      263 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/.editorconfig
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.173832 django-salesforce-5.0.1/.github/
--rw-r--r--   0 philchristensen   (502) staff       (20)       64 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/.github/FUNDING.yml
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.174208 django-salesforce-5.0.1/.github/workflows/
--rw-r--r--   0 philchristensen   (502) staff       (20)     1946 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/.github/workflows/main.yml
--rw-r--r--   0 philchristensen   (502) staff       (20)      604 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/AUTHORS.md
--rw-r--r--   0 philchristensen   (502) staff       (20)    15786 2024-03-04 18:43:04.000000 django-salesforce-5.0.1/CHANGELOG.rst
--rw-r--r--   0 philchristensen   (502) staff       (20)     3217 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 philchristensen   (502) staff       (20)     1572 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/CONTRIBUTING.md
--rwxr-xr-x   0 philchristensen   (502) staff       (20)     1392 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/LICENSE.md
--rw-r--r--   0 philchristensen   (502) staff       (20)       67 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/MANIFEST.in
--rw-r--r--   0 philchristensen   (502) staff       (20)    16608 2024-03-04 18:44:03.224629 django-salesforce-5.0.1/PKG-INFO
--rw-r--r--   0 philchristensen   (502) staff       (20)    16090 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/README.rst
--rwxr-xr-x   0 philchristensen   (502) staff       (20)     2313 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/coverage_run.sh
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.224257 django-salesforce-5.0.1/django_salesforce.egg-info/
--rw-r--r--   0 philchristensen   (502) staff       (20)    16608 2024-03-04 18:44:03.000000 django-salesforce-5.0.1/django_salesforce.egg-info/PKG-INFO
--rw-r--r--   0 philchristensen   (502) staff       (20)     6224 2024-03-04 18:44:03.000000 django-salesforce-5.0.1/django_salesforce.egg-info/SOURCES.txt
--rw-r--r--   0 philchristensen   (502) staff       (20)        1 2024-03-04 18:44:03.000000 django-salesforce-5.0.1/django_salesforce.egg-info/dependency_links.txt
--rw-r--r--   0 philchristensen   (502) staff       (20)        1 2020-05-08 14:00:41.000000 django-salesforce-5.0.1/django_salesforce.egg-info/not-zip-safe
--rw-r--r--   0 philchristensen   (502) staff       (20)       40 2024-03-04 18:44:03.000000 django-salesforce-5.0.1/django_salesforce.egg-info/requires.txt
--rw-r--r--   0 philchristensen   (502) staff       (20)       11 2024-03-04 18:44:03.000000 django-salesforce-5.0.1/django_salesforce.egg-info/top_level.txt
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.175642 django-salesforce-5.0.1/docs/
--rw-r--r--   0 philchristensen   (502) staff       (20)      956 2021-11-24 22:24:08.000000 django-salesforce-5.0.1/docs/details.rst
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      428 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/manage.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      281 2023-05-23 16:17:25.000000 django-salesforce-5.0.1/mypy.ini
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      148 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/pylint.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)    12617 2021-10-11 23:01:08.000000 django-salesforce-5.0.1/pylintrc
--rw-r--r--   0 philchristensen   (502) staff       (20)      133 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/requirements.txt
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.178351 django-salesforce-5.0.1/salesforce/
--rw-r--r--   0 philchristensen   (502) staff       (20)      662 2024-03-04 18:43:04.000000 django-salesforce-5.0.1/salesforce/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      304 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/admin.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      286 2020-05-08 13:55:20.000000 django-salesforce-5.0.1/salesforce/apps.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    26537 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/auth.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.183226 django-salesforce-5.0.1/salesforce/backend/
--rw-r--r--   0 philchristensen   (502) staff       (20)     2278 2023-12-07 15:16:54.000000 django-salesforce-5.0.1/salesforce/backend/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     4704 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/salesforce/backend/base.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      600 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/backend/client.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    25481 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/backend/compiler.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1417 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/backend/creation.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     3649 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/salesforce/backend/enterprise.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     3285 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/salesforce/backend/features.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2050 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/salesforce/backend/indep.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    22326 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/salesforce/backend/introspection.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2516 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/backend/manager.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2894 2023-05-23 16:17:25.000000 django-salesforce-5.0.1/salesforce/backend/models_lookups.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     6328 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/backend/models_sql_query.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     4187 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/salesforce/backend/operations.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     9862 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/backend/query.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1487 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/salesforce/backend/schema.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1043 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/backend/test_helpers.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    19041 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/salesforce/backend/utils.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     3406 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/backend/validation.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.185794 django-salesforce-5.0.1/salesforce/dbapi/
--rw-r--r--   0 philchristensen   (502) staff       (20)     4265 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/salesforce/dbapi/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2074 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/dbapi/common.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    41514 2023-12-07 15:16:54.000000 django-salesforce-5.0.1/salesforce/dbapi/driver.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     8012 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/dbapi/exceptions.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    14558 2023-05-23 16:17:25.000000 django-salesforce-5.0.1/salesforce/dbapi/subselect.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     5470 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/salesforce/dbapi/test_helpers.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     8104 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/salesforce/defaults.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    13057 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/salesforce/fields.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.186230 django-salesforce-5.0.1/salesforce/management/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/salesforce/management/__init__.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.186617 django-salesforce-5.0.1/salesforce/management/commands/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/salesforce/management/commands/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     7020 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/management/commands/inspectdb.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    11027 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     4823 2022-08-04 22:27:47.000000 django-salesforce-5.0.1/salesforce/models_extend.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2076 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/salesforce/models_template.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     4143 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/router.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.188447 django-salesforce-5.0.1/salesforce/testrunner/
--rw-r--r--   0 philchristensen   (502) staff       (20)       94 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/testrunner/__init__.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.191228 django-salesforce-5.0.1/salesforce/testrunner/example/
--rw-r--r--   0 philchristensen   (502) staff       (20)       94 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/testrunner/example/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      482 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/testrunner/example/admin.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      196 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/testrunner/example/forms.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    18862 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/salesforce/testrunner/example/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2049 2020-05-08 13:55:20.000000 django-salesforce-5.0.1/salesforce/testrunner/example/models_template.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.191925 django-salesforce-5.0.1/salesforce/testrunner/example/templates/
--rw-r--r--   0 philchristensen   (502) staff       (20)      444 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/salesforce/testrunner/example/templates/list-accounts.html
--rw-r--r--   0 philchristensen   (502) staff       (20)      717 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/salesforce/testrunner/example/templates/search-accounts.html
--rw-r--r--   0 philchristensen   (502) staff       (20)      314 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/testrunner/example/tests.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1268 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/salesforce/testrunner/example/universal_admin.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      290 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/testrunner/example/urls.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      971 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/testrunner/example/views.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      668 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/salesforce/testrunner/local_settings.py.sample
--rw-r--r--   0 philchristensen   (502) staff       (20)     6819 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/testrunner/settings.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      999 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/salesforce/testrunner/test_patch.diff
--rw-r--r--   0 philchristensen   (502) staff       (20)      279 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/salesforce/testrunner/urls.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.194962 django-salesforce-5.0.1/salesforce/tests/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/salesforce/tests/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1712 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/salesforce/tests/test_auth.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      817 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/salesforce/tests/test_basic.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1249 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/salesforce/tests/test_browser.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     8625 2021-11-24 22:24:08.000000 django-salesforce-5.0.1/salesforce/tests/test_bulk.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      331 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/salesforce/tests/test_doc_tests.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2432 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/salesforce/tests/test_indep.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    64017 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/salesforce/tests/test_integration.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    12583 2022-08-04 22:27:47.000000 django-salesforce-5.0.1/salesforce/tests/test_unit.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2731 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/salesforce/tests/test_utils.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.195598 django-salesforce-5.0.1/salesforce/tests/unit_tests/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/salesforce/tests/unit_tests/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     3042 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/salesforce/tests/unit_tests/test_qparser.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     4502 2022-08-04 22:27:47.000000 django-salesforce-5.0.1/salesforce/utils.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      261 2024-03-04 18:44:03.225128 django-salesforce-5.0.1/setup.cfg
--rw-r--r--   0 philchristensen   (502) staff       (20)     2336 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/setup.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.199151 django-salesforce-5.0.1/tests/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2139 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/clean_test_data.py
--rw-r--r--   0 philchristensen   (502) staff       (20)   303104 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/tests/db.sqlite3
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.201487 django-salesforce-5.0.1/tests/inspectdb/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/inspectdb/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      138 2020-05-08 13:55:20.000000 django-salesforce-5.0.1/tests/inspectdb/admin.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.202478 django-salesforce-5.0.1/tests/inspectdb/dependent_model/
--rw-r--r--   0 philchristensen   (502) staff       (20)      236 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/inspectdb/dependent_model/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      349 2020-05-08 13:55:20.000000 django-salesforce-5.0.1/tests/inspectdb/dependent_model/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      450 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/tests/inspectdb/dependent_model/settings.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      463 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/inspectdb/dependent_model/test.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      357 2020-05-08 13:55:20.000000 django-salesforce-5.0.1/tests/inspectdb/settings.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     5340 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/tests/inspectdb/slow_test.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)     1800 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/inspectdb/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     3913 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/inspectdb/tests.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      118 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/inspectdb/urls.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      636 2023-05-23 16:17:25.000000 django-salesforce-5.0.1/tests/mypy.sh
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.203625 django-salesforce-5.0.1/tests/no_django_dbapi/
--rw-r--r--   0 philchristensen   (502) staff       (20)       76 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/no_django_dbapi/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)       33 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/no_django_dbapi/settings.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     3124 2023-05-23 16:17:25.000000 django-salesforce-5.0.1/tests/no_django_dbapi/test.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      114 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/no_django_dbapi/test.sh
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.204620 django-salesforce-5.0.1/tests/no_salesforce/
--rw-r--r--   0 philchristensen   (502) staff       (20)       79 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/no_salesforce/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      586 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/no_salesforce/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      944 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/no_salesforce/settings.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      939 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/no_salesforce/tests.py
--rw-r--r--   0 philchristensen   (502) staff       (20)       48 2022-08-04 22:27:47.000000 django-salesforce-5.0.1/tests/no_urls.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.206565 django-salesforce-5.0.1/tests/t_debug_toolbar/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/t_debug_toolbar/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      158 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/tests/t_debug_toolbar/admin.py
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/t_debug_toolbar/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      426 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/tests/t_debug_toolbar/settings.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.207286 django-salesforce-5.0.1/tests/t_debug_toolbar/small_app/
--rw-r--r--   0 philchristensen   (502) staff       (20)      168 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/tests/t_debug_toolbar/small_app/admin.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      630 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/tests/t_debug_toolbar/small_app/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      271 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/tests/t_debug_toolbar/small_app/urls.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)       96 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/t_debug_toolbar/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     3223 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/tests/t_debug_toolbar/tests.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      332 2020-05-08 13:55:20.000000 django-salesforce-5.0.1/tests/t_debug_toolbar/urls.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      418 2020-05-08 13:55:20.000000 django-salesforce-5.0.1/tests/t_debug_toolbar/views.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.208189 django-salesforce-5.0.1/tests/test_app_label/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_app_label/__init__.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.208970 django-salesforce-5.0.1/tests/test_app_label/salesforce/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_app_label/salesforce/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      187 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_app_label/salesforce/apps.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      413 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_app_label/salesforce/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      303 2020-05-08 13:55:20.000000 django-salesforce-5.0.1/tests/test_app_label/salesforce/tests.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      450 2022-08-04 22:27:47.000000 django-salesforce-5.0.1/tests/test_app_label/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)       96 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_app_label/test.sh
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.209984 django-salesforce-5.0.1/tests/test_compatibility/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_compatibility/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1930 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_compatibility/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      343 2022-08-04 22:27:47.000000 django-salesforce-5.0.1/tests/test_compatibility/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      102 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_compatibility/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1872 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/tests/test_compatibility/tests.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.211087 django-salesforce-5.0.1/tests/test_default_db/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_default_db/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2091 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_default_db/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      381 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/tests/test_default_db/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      351 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_default_db/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     5346 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_default_db/tests.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.212051 django-salesforce-5.0.1/tests/test_dynamic_auth/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_dynamic_auth/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_dynamic_auth/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      524 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/tests/test_dynamic_auth/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      100 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_dynamic_auth/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1619 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/tests/test_dynamic_auth/tests.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.212907 django-salesforce-5.0.1/tests/test_general/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_general/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      126 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_general/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      108 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_general/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     4073 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_general/test_helpers.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.213982 django-salesforce-5.0.1/tests/test_lazy_connect/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_lazy_connect/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_lazy_connect/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      652 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/tests/test_lazy_connect/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      100 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_lazy_connect/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1039 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_lazy_connect/tests.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.215170 django-salesforce-5.0.1/tests/test_managers/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/tests/test_managers/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      850 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/tests/test_managers/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      447 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/tests/test_managers/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)       92 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/tests/test_managers/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1453 2023-05-23 16:17:25.000000 django-salesforce-5.0.1/tests/test_managers/tests.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.216210 django-salesforce-5.0.1/tests/test_migrate/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_migrate/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      881 2020-05-08 13:55:20.000000 django-salesforce-5.0.1/tests/test_migrate/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      558 2022-08-04 22:27:47.000000 django-salesforce-5.0.1/tests/test_migrate/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)     1116 2021-11-24 22:24:08.000000 django-salesforce-5.0.1/tests/test_migrate/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1182 2020-05-08 13:55:20.000000 django-salesforce-5.0.1/tests/test_migrate/tests.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.217197 django-salesforce-5.0.1/tests/test_mixin/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_mixin/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     2469 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_mixin/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      322 2022-08-04 22:27:47.000000 django-salesforce-5.0.1/tests/test_mixin/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)       86 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_mixin/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1651 2020-05-08 13:55:20.000000 django-salesforce-5.0.1/tests/test_mixin/tests.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.218320 django-salesforce-5.0.1/tests/test_mock/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/test_mock/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    18727 2022-08-04 22:27:47.000000 django-salesforce-5.0.1/tests/test_mock/mocksf.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      525 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_mock/settings.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     7670 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_mock/test_data.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     4641 2021-11-24 22:24:08.000000 django-salesforce-5.0.1/tests/test_mock/test_mocksf.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.219643 django-salesforce-5.0.1/tests/test_mock2/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_mock2/__init__.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.220105 django-salesforce-5.0.1/tests/test_mock2/migrations/
--rw-r--r--   0 philchristensen   (502) staff       (20)     4372 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_mock2/migrations/0001_initial.py
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_mock2/migrations/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     1694 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_mock2/models.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      177 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_mock2/mypy.ini
--rw-r--r--   0 philchristensen   (502) staff       (20)      826 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/tests/test_mock2/settings.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)       95 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_mock2/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     5589 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/test_mock2/test_rec.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      268 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/tests/tests.sh
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      175 2020-04-22 12:21:48.000000 django-salesforce-5.0.1/tests/tests_no_django.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1001 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/tests/to_mock.py
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.221538 django-salesforce-5.0.1/tests/tooling/
--rw-r--r--   0 philchristensen   (502) staff       (20)        0 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/tests/tooling/__init__.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      138 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/tests/tooling/admin.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      366 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/tooling/settings.py
--rw-r--r--   0 philchristensen   (502) staff       (20)    10445 2023-12-07 15:16:54.000000 django-salesforce-5.0.1/tests/tooling/slow_test.py
--rwxr-xr-x   0 philchristensen   (502) staff       (20)      605 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/tooling/test.sh
--rw-r--r--   0 philchristensen   (502) staff       (20)     1871 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/tests/tooling/tests.py
--rw-r--r--   0 philchristensen   (502) staff       (20)      140 2021-10-11 22:52:49.000000 django-salesforce-5.0.1/tests/tooling/urls.py
--rw-r--r--   0 philchristensen   (502) staff       (20)     4203 2024-03-04 18:40:06.000000 django-salesforce-5.0.1/tox.ini
-drwxr-xr-x   0 philchristensen   (502) staff       (20)        0 2024-03-04 18:44:03.223603 django-salesforce-5.0.1/wiki/
--rw-r--r--   0 philchristensen   (502) staff       (20)      548 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/wiki/Documents-and-Attachments.md
--rw-r--r--   0 philchristensen   (502) staff       (20)     3078 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/wiki/Empty-strings-in-filters.md
--rw-r--r--   0 philchristensen   (502) staff       (20)     4902 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/wiki/Error-messages.md
--rw-r--r--   0 philchristensen   (502) staff       (20)     6979 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/wiki/Experimental-Features.rest
--rw-r--r--   0 philchristensen   (502) staff       (20)     2939 2023-07-04 13:35:06.000000 django-salesforce-5.0.1/wiki/Foreign-Key-Support.rest
--rw-r--r--   0 philchristensen   (502) staff       (20)     2505 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/wiki/Home.md
--rw-r--r--   0 philchristensen   (502) staff       (20)     7981 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/wiki/Introspection-and-Special-Attributes-of-Fields.rest
--rw-r--r--   0 philchristensen   (502) staff       (20)     2120 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/wiki/Lead-Conversion.rest
--rw-r--r--   0 philchristensen   (502) staff       (20)     1528 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/wiki/Release-Process.md
--rw-r--r--   0 philchristensen   (502) staff       (20)     1977 2020-07-09 19:30:00.000000 django-salesforce-5.0.1/wiki/SalesforceModels-used-with-local-databases.md
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.673853 django-salesforce-5.0.2/
+-rw-r--r--   0 philchristensen   (501) staff       (20)      475 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/.coveragerc
+-rw-r--r--   0 philchristensen   (501) staff       (20)      263 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/.editorconfig
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.647203 django-salesforce-5.0.2/.github/
+-rw-r--r--   0 philchristensen   (501) staff       (20)       64 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/.github/FUNDING.yml
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.647344 django-salesforce-5.0.2/.github/workflows/
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1947 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/.github/workflows/main.yml
+-rw-r--r--   0 philchristensen   (501) staff       (20)      604 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/AUTHORS.md
+-rw-r--r--   0 philchristensen   (501) staff       (20)    17158 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/CHANGELOG.rst
+-rw-r--r--   0 philchristensen   (501) staff       (20)     3217 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1572 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/CONTRIBUTING.md
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)     1392 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/LICENSE.md
+-rw-r--r--   0 philchristensen   (501) staff       (20)       67 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/MANIFEST.in
+-rw-r--r--   0 philchristensen   (501) staff       (20)    16517 2024-05-27 14:30:23.673975 django-salesforce-5.0.2/PKG-INFO
+-rw-r--r--   0 philchristensen   (501) staff       (20)    16084 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/README.rst
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)     2324 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/coverage_run.sh
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.648106 django-salesforce-5.0.2/django_salesforce.egg-info/
+-rw-r--r--   0 philchristensen   (501) staff       (20)    16517 2024-05-27 14:30:23.000000 django-salesforce-5.0.2/django_salesforce.egg-info/PKG-INFO
+-rw-r--r--   0 philchristensen   (501) staff       (20)     6259 2024-05-27 14:30:23.000000 django-salesforce-5.0.2/django_salesforce.egg-info/SOURCES.txt
+-rw-r--r--   0 philchristensen   (501) staff       (20)        1 2024-05-27 14:30:23.000000 django-salesforce-5.0.2/django_salesforce.egg-info/dependency_links.txt
+-rw-r--r--   0 philchristensen   (501) staff       (20)        1 2024-05-27 14:30:23.000000 django-salesforce-5.0.2/django_salesforce.egg-info/not-zip-safe
+-rw-r--r--   0 philchristensen   (501) staff       (20)       41 2024-05-27 14:30:23.000000 django-salesforce-5.0.2/django_salesforce.egg-info/requires.txt
+-rw-r--r--   0 philchristensen   (501) staff       (20)       11 2024-05-27 14:30:23.000000 django-salesforce-5.0.2/django_salesforce.egg-info/top_level.txt
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.648218 django-salesforce-5.0.2/docs/
+-rw-r--r--   0 philchristensen   (501) staff       (20)      956 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/docs/details.rst
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)      428 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/manage.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      281 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/mypy.ini
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)      148 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/pylint.sh
+-rw-r--r--   0 philchristensen   (501) staff       (20)    12617 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/pylintrc
+-rw-r--r--   0 philchristensen   (501) staff       (20)      134 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/requirements.txt
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.649707 django-salesforce-5.0.2/salesforce/
+-rw-r--r--   0 philchristensen   (501) staff       (20)      699 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/salesforce/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      304 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/admin.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      286 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/apps.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)    26537 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/auth.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.652230 django-salesforce-5.0.2/salesforce/backend/
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2232 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/salesforce/backend/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     4704 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/backend/base.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      600 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/backend/client.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)    26012 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/salesforce/backend/compiler.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1417 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/backend/creation.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     3649 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/backend/enterprise.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     3285 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/backend/features.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2050 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/backend/indep.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)    22500 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/backend/introspection.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2516 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/backend/manager.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     3366 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/salesforce/backend/models_lookups.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     6328 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/backend/models_sql_query.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     8148 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/salesforce/backend/operations.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     9862 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/backend/query.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1487 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/backend/schema.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1043 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/backend/test_helpers.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)    19041 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/backend/utils.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     3406 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/backend/validation.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.653181 django-salesforce-5.0.2/salesforce/dbapi/
+-rw-r--r--   0 philchristensen   (501) staff       (20)     4265 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/dbapi/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2074 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/dbapi/common.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)    41514 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/dbapi/driver.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     8012 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/dbapi/exceptions.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)    14558 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/dbapi/subselect.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     5470 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/dbapi/test_helpers.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     8104 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/defaults.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)    13114 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/fields.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.653379 django-salesforce-5.0.2/salesforce/management/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/management/__init__.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.653581 django-salesforce-5.0.2/salesforce/management/commands/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/management/commands/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     7020 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/management/commands/inspectdb.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)    10988 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     4823 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/models_extend.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2076 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/models_template.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     4143 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/router.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.654366 django-salesforce-5.0.2/salesforce/testrunner/
+-rw-r--r--   0 philchristensen   (501) staff       (20)       94 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/testrunner/__init__.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.655491 django-salesforce-5.0.2/salesforce/testrunner/example/
+-rw-r--r--   0 philchristensen   (501) staff       (20)       94 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/testrunner/example/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      482 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/testrunner/example/admin.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      196 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/testrunner/example/forms.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)    22059 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/salesforce/testrunner/example/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2049 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/testrunner/example/models_template.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.655798 django-salesforce-5.0.2/salesforce/testrunner/example/templates/
+-rw-r--r--   0 philchristensen   (501) staff       (20)      444 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/testrunner/example/templates/list-accounts.html
+-rw-r--r--   0 philchristensen   (501) staff       (20)      717 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/testrunner/example/templates/search-accounts.html
+-rw-r--r--   0 philchristensen   (501) staff       (20)      314 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/testrunner/example/tests.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1268 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/testrunner/example/universal_admin.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      290 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/testrunner/example/urls.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      971 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/testrunner/example/views.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      668 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/testrunner/local_settings.py.sample
+-rw-r--r--   0 philchristensen   (501) staff       (20)     7252 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/salesforce/testrunner/settings.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      999 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/testrunner/test_patch.diff
+-rw-r--r--   0 philchristensen   (501) staff       (20)      279 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/testrunner/urls.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.657308 django-salesforce-5.0.2/salesforce/tests/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/tests/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1712 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/tests/test_auth.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      817 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/tests/test_basic.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1249 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/tests/test_browser.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     8625 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/tests/test_bulk.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      331 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/tests/test_doc_tests.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2368 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/salesforce/tests/test_documents.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2432 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/tests/test_indep.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)    64955 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/salesforce/tests/test_integration.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)    12968 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/tests/test_unit.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2731 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/tests/test_utils.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.657541 django-salesforce-5.0.2/salesforce/tests/unit_tests/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/tests/unit_tests/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     3042 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/tests/unit_tests/test_qparser.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     4502 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/salesforce/utils.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      261 2024-05-27 14:30:23.674233 django-salesforce-5.0.2/setup.cfg
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2336 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/setup.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.659706 django-salesforce-5.0.2/tests/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2286 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/tests/clean_test_data.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)   303104 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/db.sqlite3
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.660649 django-salesforce-5.0.2/tests/inspectdb/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/inspectdb/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      138 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/inspectdb/admin.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.661101 django-salesforce-5.0.2/tests/inspectdb/dependent_model/
+-rw-r--r--   0 philchristensen   (501) staff       (20)      236 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/inspectdb/dependent_model/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      349 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/inspectdb/dependent_model/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      450 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/inspectdb/dependent_model/settings.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      463 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/inspectdb/dependent_model/test.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      357 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/inspectdb/settings.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     5340 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/inspectdb/slow_test.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)     1800 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/inspectdb/test.sh
+-rw-r--r--   0 philchristensen   (501) staff       (20)     3913 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/inspectdb/tests.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      118 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/inspectdb/urls.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)      636 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/mypy.sh
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.661554 django-salesforce-5.0.2/tests/no_django_dbapi/
+-rw-r--r--   0 philchristensen   (501) staff       (20)       76 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/no_django_dbapi/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)       33 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/no_django_dbapi/settings.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     3124 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/no_django_dbapi/test.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)      114 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/no_django_dbapi/test.sh
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.662046 django-salesforce-5.0.2/tests/no_salesforce/
+-rw-r--r--   0 philchristensen   (501) staff       (20)       79 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/no_salesforce/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      586 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/no_salesforce/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      944 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/no_salesforce/settings.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      939 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/no_salesforce/tests.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)       48 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/no_urls.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.662944 django-salesforce-5.0.2/tests/t_debug_toolbar/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/t_debug_toolbar/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      158 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/t_debug_toolbar/admin.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/t_debug_toolbar/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      426 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/t_debug_toolbar/settings.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.663375 django-salesforce-5.0.2/tests/t_debug_toolbar/small_app/
+-rw-r--r--   0 philchristensen   (501) staff       (20)      168 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/t_debug_toolbar/small_app/admin.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      630 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/t_debug_toolbar/small_app/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      271 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/t_debug_toolbar/small_app/urls.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)       96 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/t_debug_toolbar/test.sh
+-rw-r--r--   0 philchristensen   (501) staff       (20)     3223 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/t_debug_toolbar/tests.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      332 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/t_debug_toolbar/urls.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      418 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/t_debug_toolbar/views.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.663731 django-salesforce-5.0.2/tests/test_app_label/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_app_label/__init__.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.664210 django-salesforce-5.0.2/tests/test_app_label/salesforce/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_app_label/salesforce/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      187 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_app_label/salesforce/apps.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      413 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_app_label/salesforce/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      303 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_app_label/salesforce/tests.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      450 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_app_label/settings.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)       96 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_app_label/test.sh
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.664789 django-salesforce-5.0.2/tests/test_compatibility/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_compatibility/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1930 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_compatibility/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      343 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_compatibility/settings.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)      102 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_compatibility/test.sh
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1872 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_compatibility/tests.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.665349 django-salesforce-5.0.2/tests/test_default_db/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_default_db/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2091 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_default_db/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      381 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_default_db/settings.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)      351 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_default_db/test.sh
+-rw-r--r--   0 philchristensen   (501) staff       (20)     5346 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_default_db/tests.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.665972 django-salesforce-5.0.2/tests/test_dynamic_auth/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_dynamic_auth/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_dynamic_auth/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      524 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_dynamic_auth/settings.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)      100 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_dynamic_auth/test.sh
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1619 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_dynamic_auth/tests.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.666433 django-salesforce-5.0.2/tests/test_general/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_general/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      126 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_general/settings.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)      108 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_general/test.sh
+-rw-r--r--   0 philchristensen   (501) staff       (20)     4073 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_general/test_helpers.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.666994 django-salesforce-5.0.2/tests/test_lazy_connect/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_lazy_connect/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_lazy_connect/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      652 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_lazy_connect/settings.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)      100 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_lazy_connect/test.sh
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1039 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_lazy_connect/tests.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.667562 django-salesforce-5.0.2/tests/test_managers/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_managers/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      850 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_managers/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      447 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_managers/settings.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)       92 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_managers/test.sh
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1453 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_managers/tests.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.668135 django-salesforce-5.0.2/tests/test_migrate/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_migrate/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      881 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_migrate/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      558 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_migrate/settings.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)     1116 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_migrate/test.sh
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1182 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_migrate/tests.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.668749 django-salesforce-5.0.2/tests/test_mixin/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mixin/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2469 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mixin/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      322 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mixin/settings.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)       86 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mixin/test.sh
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1651 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mixin/tests.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.669390 django-salesforce-5.0.2/tests/test_mock/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mock/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)    18727 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mock/mocksf.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      525 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mock/settings.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     7670 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mock/test_data.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     4641 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mock/test_mocksf.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.670263 django-salesforce-5.0.2/tests/test_mock2/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mock2/__init__.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.670695 django-salesforce-5.0.2/tests/test_mock2/migrations/
+-rw-r--r--   0 philchristensen   (501) staff       (20)     4372 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mock2/migrations/0001_initial.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mock2/migrations/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1694 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mock2/models.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      177 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mock2/mypy.ini
+-rw-r--r--   0 philchristensen   (501) staff       (20)      826 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mock2/settings.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)       95 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mock2/test.sh
+-rw-r--r--   0 philchristensen   (501) staff       (20)     5589 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/test_mock2/test_rec.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)      268 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/tests.sh
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)      175 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/tests_no_django.sh
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1001 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/to_mock.py
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.671619 django-salesforce-5.0.2/tests/tooling/
+-rw-r--r--   0 philchristensen   (501) staff       (20)        0 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/tooling/__init__.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      138 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/tooling/admin.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      366 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/tooling/settings.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)    10445 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/tooling/slow_test.py
+-rwxr-xr-x   0 philchristensen   (501) staff       (20)      605 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/tooling/test.sh
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1871 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/tooling/tests.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)      140 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/tests/tooling/urls.py
+-rw-r--r--   0 philchristensen   (501) staff       (20)     4220 2024-05-27 14:24:59.000000 django-salesforce-5.0.2/tox.ini
+drwxr-xr-x   0 philchristensen   (501) staff       (20)        0 2024-05-27 14:30:23.673696 django-salesforce-5.0.2/wiki/
+-rw-r--r--   0 philchristensen   (501) staff       (20)      548 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/wiki/Documents-and-Attachments.md
+-rw-r--r--   0 philchristensen   (501) staff       (20)     3078 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/wiki/Empty-strings-in-filters.md
+-rw-r--r--   0 philchristensen   (501) staff       (20)     4902 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/wiki/Error-messages.md
+-rw-r--r--   0 philchristensen   (501) staff       (20)     6979 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/wiki/Experimental-Features.rest
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2939 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/wiki/Foreign-Key-Support.rest
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2505 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/wiki/Home.md
+-rw-r--r--   0 philchristensen   (501) staff       (20)     7981 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/wiki/Introspection-and-Special-Attributes-of-Fields.rest
+-rw-r--r--   0 philchristensen   (501) staff       (20)     2120 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/wiki/Lead-Conversion.rest
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1528 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/wiki/Release-Process.md
+-rw-r--r--   0 philchristensen   (501) staff       (20)     1977 2024-05-22 15:47:51.000000 django-salesforce-5.0.2/wiki/SalesforceModels-used-with-local-databases.md
```

### Comparing `django-salesforce-5.0.1/.github/workflows/main.yml` & `django-salesforce-5.0.2/.github/workflows/main.yml`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       max-parallel: 1
       matrix:
-        python-version: [3.8, 3.11, "3.10", 3.7, 3.9]
+        python-version: [3.8, 3.12, 3.11, "3.10", 3.9]
     timeout-minutes: 20
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
@@ -37,19 +37,19 @@
         DJSF_LICENSE_KEY: ${{ secrets.DJSF_LICENSE_KEY }}
         SF_CONSUMER_KEY: ${{ secrets.SF_CONSUMER_KEY }}
         SF_CONSUMER_SECRET: ${{ secrets.SF_CONSUMER_SECRET }}
         SF_USER: ${{ secrets.SF_USER }}
         SF_PASSWORD: ${{ secrets.SF_PASSWORD }}
         SF_HOST: ${{ secrets.SF_HOST }}
 
-        TOXENV_38:  "docs_style,typing,clean,dj22-py38,dj32-py38"
-        TOXENV_311: "dj50-py311,dj42-py311"
+        TOXENV_38:  "docs_style,typing,clean,dj22-py38,dj21-py38"
+        TOXENV_312: "dj50-py312"
+        TOXENV_311: "dj42-py311"
         TOXENV_310: "dj40-py310"
-        TOXENV_37:  "dj20-py37,dj30-py37"
-        TOXENV_39:  "no_django-py39,debug_toolbar-dj42-py39"
+        TOXENV_39:  "no_django-py39,debug_toolbar-dj42-py39,dj32-py39,dj30-py39"
       run: |
         TOXENV_NAME=$(echo TOXENV_${{ matrix.python-version }} | sed 's/\.//')
         cat > salesforce/testrunner/local_settings.py <<'-- end local_settings --'
         SF_PK = 'Id'
         SF_LAZY_CONNECT = False
         -- end local_settings --
         echo "tox -e ${!TOXENV_NAME}"
```

### Comparing `django-salesforce-5.0.1/AUTHORS.md` & `django-salesforce-5.0.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/CHANGELOG.rst` & `django-salesforce-5.0.2/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,40 @@
 some undocumented internal code that could yet have been used by
 someone. Not related e.g. to examples and tests,
 but a new feature can be referred by a test name if not documented yet.
 Some items here can be marked as "internal": not ready enough or
 experimental.
 
 
-[5.0.1] not released yet
+[5.0.2] not released yet
 ------------------------
+The main new features are in the improved query compiler
+
+* Remove: the old Python 3.7
+* Remove: the code for Django 2.0
+* Fix: many issues in the query compiler in edge cases:
+  - fix a query with offset, but without a limit (NotImplementedError)
+  - fix a '__range' lookup on a field of custom foreign key object (SalesforceError)
+  - fix a '=null' lookup.  It worked probably always correctly, but the old implementation was different from  standard lookups. It made it impossible to distinguish it from unsupported queries
+* Add: The query compiler is now much more precise. Most of unsupported queries will
+  write a warning before they are tried compiled. This is how users have
+  discovered some functional queries in the past.
+  No regression is known that a previously correct query would write a warning.
+* Add: Support for date and datetime lookup by year, quarter, month, day, week_day, hour
+  e.g. group this year by month:
+  .filter(date__year=2024).value('date__month').annotate(total=Sum('amount'))
+* Add: The method .sf(minimal_aliases=True) is not necessary
+  for ContentDocumentLink .filter(...); #259
+* Fix: Compile correctly: .filter(related_model__field__in=...) Fix #302
+* Fix: Prepare tests for Salesforce API 61.0 Summer '24
+* Add: Introspect Salesforce fields of type Formula to sf_formula="..." parameter
+
+
+[5.0.1] 2024-03-04
+------------------
 * Add: Support for ``db_default`` field option in Django 5.0. It allows a seamless
   support of the ``defaultedOnCreate`` counterpart in Salesforce.
 * Add: Support for Salesforce API 60.0 Spring '24.
 * Change: Values of ``FloatField`` are now really float, not Decimal as previously.
 * Fix: Compatibility with the current django-debug-toolbar #322
 * Fix: Introspection ``inspectdb`` of custom editable name fields #308
 * Add: FloatField is used by ``inspectdb`` for some metadata with negative decimal places
```

### Comparing `django-salesforce-5.0.1/CODE_OF_CONDUCT.md` & `django-salesforce-5.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/CONTRIBUTING.md` & `django-salesforce-5.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/LICENSE.md` & `django-salesforce-5.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/PKG-INFO` & `django-salesforce-5.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 Metadata-Version: 2.1
 Name: django-salesforce
-Version: 5.0.1
+Version: 5.0.2
 Summary: a Salesforce backend for Django's ORM
 Home-page: https://github.com/django-salesforce/django-salesforce
 Author: Hynek Cernoch
 Author-email: hynek@sdb.cz
 Maintainer: Phil Christensen
 Maintainer-email: phil@bubblehouse.org
 License: AGPL
 Keywords: django salesforce orm backend
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 License-File: AUTHORS.md
-Requires-Dist: django>=2.0
-Requires-Dist: pytz>=2012c
-Requires-Dist: requests>=2.4.0
 
 django-salesforce
 =================
 
 .. image:: https://github.com/django-salesforce/django-salesforce/actions/workflows/main.yml/badge.svg
    :target: https://github.com/django-salesforce/django-salesforce/actions/workflows/main.yml
 
 .. image:: https://badge.fury.io/py/django-salesforce.svg
    :target: https://pypi.python.org/pypi/django-salesforce
 
-.. image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue
+.. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg
    :target: https://www.python.org/
 
-.. image:: https://img.shields.io/badge/Django-2.0%2C%202.1%2C%202.2%20%7C%203.0%2C%203.1%20%2C%203.2%20%7C%204.0%2C%204.1%2C%204.2%20%7C%205.0-blue.svg
+.. image:: https://img.shields.io/badge/Django-2.1%2C%202.2%20%7C%203.0%2C%203.1%20%2C%203.2%20%7C%204.0%2C%204.1%2C%204.2%20%7C%205.0-blue.svg
    :target: https://www.djangoproject.com/
 
 This library allows you to load, edit and query the objects in any Salesforce instance
 using Django models. The integration is fairly complete, and generally seamless
 for most uses. It works by integrating with the Django ORM, allowing access to
 the objects in your SFDC instance (Salesforce .com) as if they were in a
 traditional database.
 
-Python 3.7 to 3.12, Django 2.0 to 5.0. (Tested also with Python 3.13 alpha 2)
+Python 3.8 to 3.12, Django 2.1 to 5.0. (Tested also with Python 3.13b1)
 
 Use with Django 5.0 or 4.2(LTS) currently requires an enteprise license key DJSF_LICENSE_KEY
 until August 2024 unless you accept the AGPL license and install our otherwise identical
 package "django-salesforce-agpl" instead. The license keys are available to sponsors.
 Both versions will be unlocked automatically in Django-salesforce 5.1 when a key will be
 required for Django 5.1. Use with pre-release Django versions is free.
 
@@ -317,14 +314,14 @@
    UNION, EXCEPT, INTERSECT and DISTINCT.
 
 Backwards-incompatible changes
 ------------------------------
 
 The last most important:
 
+-  v5.0.2: Removed support for Python 3.7 and Django 2.0
+
 -  v4.2: Some new features or versions implemented after June 2023 can require a license key
    (sponsorship) or to accept the AGPL license. (AGPL is fine for exclusive open source
    contribution or for education, but impossible if you do not share all your
    source codes.)
    Removed support for Python 3.6
-
--  v4.0: Removed support for Python 3.5
```

### Comparing `django-salesforce-5.0.1/README.rst` & `django-salesforce-5.0.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 
 .. image:: https://github.com/django-salesforce/django-salesforce/actions/workflows/main.yml/badge.svg
    :target: https://github.com/django-salesforce/django-salesforce/actions/workflows/main.yml
 
 .. image:: https://badge.fury.io/py/django-salesforce.svg
    :target: https://pypi.python.org/pypi/django-salesforce
 
-.. image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue
+.. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg
    :target: https://www.python.org/
 
-.. image:: https://img.shields.io/badge/Django-2.0%2C%202.1%2C%202.2%20%7C%203.0%2C%203.1%20%2C%203.2%20%7C%204.0%2C%204.1%2C%204.2%20%7C%205.0-blue.svg
+.. image:: https://img.shields.io/badge/Django-2.1%2C%202.2%20%7C%203.0%2C%203.1%20%2C%203.2%20%7C%204.0%2C%204.1%2C%204.2%20%7C%205.0-blue.svg
    :target: https://www.djangoproject.com/
 
 This library allows you to load, edit and query the objects in any Salesforce instance
 using Django models. The integration is fairly complete, and generally seamless
 for most uses. It works by integrating with the Django ORM, allowing access to
 the objects in your SFDC instance (Salesforce .com) as if they were in a
 traditional database.
 
-Python 3.7 to 3.12, Django 2.0 to 5.0. (Tested also with Python 3.13 alpha 2)
+Python 3.8 to 3.12, Django 2.1 to 5.0. (Tested also with Python 3.13b1)
 
 Use with Django 5.0 or 4.2(LTS) currently requires an enteprise license key DJSF_LICENSE_KEY
 until August 2024 unless you accept the AGPL license and install our otherwise identical
 package "django-salesforce-agpl" instead. The license keys are available to sponsors.
 Both versions will be unlocked automatically in Django-salesforce 5.1 when a key will be
 required for Django 5.1. Use with pre-release Django versions is free.
 
@@ -299,14 +299,14 @@
    UNION, EXCEPT, INTERSECT and DISTINCT.
 
 Backwards-incompatible changes
 ------------------------------
 
 The last most important:
 
+-  v5.0.2: Removed support for Python 3.7 and Django 2.0
+
 -  v4.2: Some new features or versions implemented after June 2023 can require a license key
    (sponsorship) or to accept the AGPL license. (AGPL is fine for exclusive open source
    contribution or for education, but impossible if you do not share all your
    source codes.)
    Removed support for Python 3.6
-
--  v4.0: Removed support for Python 3.5
```

### Comparing `django-salesforce-5.0.1/coverage_run.sh` & `django-salesforce-5.0.2/coverage_run.sh`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 $COVERAGE run -a $SOURCE manage.py inspectdb --database=salesforce Account >/dev/null
 $COVERAGE run -a $SOURCE manage.py inspectdb --database=salesforce --table-filter=Account >/dev/null
 $COVERAGE run -a $SOURCE manage.py inspectdb --database=salesforce --tooling-api >/dev/null
 $COVERAGE run -a $SOURCE manage.py makemigrations
 $COVERAGE run -a $SOURCE manage.py migrate --database=default
 $COVERAGE run -a $SOURCE manage.py check --settings=tests.tooling.settings
 
-for x in dj20-py37 dj22-py38 dj31-py39 dj40-py310; do
+for x in dj21-py38 dj22-py38 dj31-py39 dj40-py310 dj50-py312; do
     echo "*** $x ***"
     .tox/${x}/bin/coverage run -a $SOURCE manage.py inspectdb --database=salesforce >/dev/null
     .tox/${x}/bin/coverage run -a $SOURCE manage.py test salesforce
 done
 for DIR in tests/test_* tests/no_salesforce tests/t_debug_toolbar tests/no_django_dbapi; do
     x=${DIR//\//.}
     TESTS=$(find $DIR -name \*test\*.py)
```

### Comparing `django-salesforce-5.0.1/django_salesforce.egg-info/PKG-INFO` & `django-salesforce-5.0.2/django_salesforce.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 Metadata-Version: 2.1
 Name: django-salesforce
-Version: 5.0.1
+Version: 5.0.2
 Summary: a Salesforce backend for Django's ORM
 Home-page: https://github.com/django-salesforce/django-salesforce
 Author: Hynek Cernoch
 Author-email: hynek@sdb.cz
 Maintainer: Phil Christensen
 Maintainer-email: phil@bubblehouse.org
 License: AGPL
 Keywords: django salesforce orm backend
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 License-File: AUTHORS.md
-Requires-Dist: django>=2.0
-Requires-Dist: pytz>=2012c
-Requires-Dist: requests>=2.4.0
 
 django-salesforce
 =================
 
 .. image:: https://github.com/django-salesforce/django-salesforce/actions/workflows/main.yml/badge.svg
    :target: https://github.com/django-salesforce/django-salesforce/actions/workflows/main.yml
 
 .. image:: https://badge.fury.io/py/django-salesforce.svg
    :target: https://pypi.python.org/pypi/django-salesforce
 
-.. image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue
+.. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue.svg
    :target: https://www.python.org/
 
-.. image:: https://img.shields.io/badge/Django-2.0%2C%202.1%2C%202.2%20%7C%203.0%2C%203.1%20%2C%203.2%20%7C%204.0%2C%204.1%2C%204.2%20%7C%205.0-blue.svg
+.. image:: https://img.shields.io/badge/Django-2.1%2C%202.2%20%7C%203.0%2C%203.1%20%2C%203.2%20%7C%204.0%2C%204.1%2C%204.2%20%7C%205.0-blue.svg
    :target: https://www.djangoproject.com/
 
 This library allows you to load, edit and query the objects in any Salesforce instance
 using Django models. The integration is fairly complete, and generally seamless
 for most uses. It works by integrating with the Django ORM, allowing access to
 the objects in your SFDC instance (Salesforce .com) as if they were in a
 traditional database.
 
-Python 3.7 to 3.12, Django 2.0 to 5.0. (Tested also with Python 3.13 alpha 2)
+Python 3.8 to 3.12, Django 2.1 to 5.0. (Tested also with Python 3.13b1)
 
 Use with Django 5.0 or 4.2(LTS) currently requires an enteprise license key DJSF_LICENSE_KEY
 until August 2024 unless you accept the AGPL license and install our otherwise identical
 package "django-salesforce-agpl" instead. The license keys are available to sponsors.
 Both versions will be unlocked automatically in Django-salesforce 5.1 when a key will be
 required for Django 5.1. Use with pre-release Django versions is free.
 
@@ -317,14 +314,14 @@
    UNION, EXCEPT, INTERSECT and DISTINCT.
 
 Backwards-incompatible changes
 ------------------------------
 
 The last most important:
 
+-  v5.0.2: Removed support for Python 3.7 and Django 2.0
+
 -  v4.2: Some new features or versions implemented after June 2023 can require a license key
    (sponsorship) or to accept the AGPL license. (AGPL is fine for exclusive open source
    contribution or for education, but impossible if you do not share all your
    source codes.)
    Removed support for Python 3.6
-
--  v4.0: Removed support for Python 3.5
```

### Comparing `django-salesforce-5.0.1/django_salesforce.egg-info/SOURCES.txt` & `django-salesforce-5.0.2/django_salesforce.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 salesforce/testrunner/example/templates/search-accounts.html
 salesforce/tests/__init__.py
 salesforce/tests/test_auth.py
 salesforce/tests/test_basic.py
 salesforce/tests/test_browser.py
 salesforce/tests/test_bulk.py
 salesforce/tests/test_doc_tests.py
+salesforce/tests/test_documents.py
 salesforce/tests/test_indep.py
 salesforce/tests/test_integration.py
 salesforce/tests/test_unit.py
 salesforce/tests/test_utils.py
 salesforce/tests/unit_tests/__init__.py
 salesforce/tests/unit_tests/test_qparser.py
 tests/__init__.py
```

### Comparing `django-salesforce-5.0.1/docs/details.rst` & `django-salesforce-5.0.2/docs/details.rst`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/pylintrc` & `django-salesforce-5.0.2/pylintrc`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/auth.py` & `django-salesforce-5.0.2/salesforce/auth.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/backend/__init__.py` & `django-salesforce-5.0.2/salesforce/backend/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,27 +28,26 @@
 """
 
 import logging
 import re
 
 import django
 
-DJANGO_21_PLUS = django.VERSION[:2] >= (2, 1)
 DJANGO_22_PLUS = django.VERSION[:2] >= (2, 2)
 DJANGO_30_PLUS = django.VERSION[:2] >= (3, 0)
 DJANGO_31_PLUS = django.VERSION[:2] >= (3, 1)
 DJANGO_32_PLUS = django.VERSION[:2] >= (3, 2)
 DJANGO_40_PLUS = django.VERSION[:2] >= (4, 0)
 DJANGO_41_PLUS = django.VERSION[:2] >= (4, 1)
 DJANGO_42_PLUS = django.VERSION[:2] >= (4, 2)
 DJANGO_50_PLUS = django.VERSION[:2] >= (5, 0)
 max_django = (5, 0)
 is_dev_version = django.VERSION[3:] and re.match('(alpha|beta|rc)', django.VERSION[3])
-if django.VERSION[:2] < (2, 0) or django.VERSION[:2] > max_django and not is_dev_version:
-    raise ImportError("Django version between 2.0 and 5.0 is required "
+if django.VERSION[:2] < (2, 1) or django.VERSION[:2] > max_django and not is_dev_version:
+    raise ImportError("Django version between 2.1 and 5.0 is required "
                       "for this django-salesforce.")
     # Usually three or more blocking issues can be expected by every
     # new major Django version. Strict check before support is better.
 
     # New Django development versions are enabled without any restriction, but
     # new stable Django versions must be verified before they are enabled here.
```

### Comparing `django-salesforce-5.0.1/salesforce/backend/base.py` & `django-salesforce-5.0.2/salesforce/backend/base.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/backend/client.py` & `django-salesforce-5.0.2/salesforce/backend/client.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/backend/compiler.py` & `django-salesforce-5.0.2/salesforce/backend/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,34 +5,39 @@
 #
 
 """
 Generate queries using the SOQL dialect.  (like django.db.models.sql.compiler and  django.db.models.sql.where)
 """
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Tuple
 import re
+import warnings
 from django.core.exceptions import EmptyResultSet
 from django.db import NotSupportedError
 from django.db.models.sql import compiler as sql_compiler, where as sql_where, constants, datastructures
 from django.db.models.sql.where import AND
 from django.db.transaction import TransactionManagementError
 
 import salesforce.backend.models_lookups   # noqa pylint:disable=unused-import # required for activation of lookups
-from salesforce.backend import DJANGO_21_PLUS, DJANGO_30_PLUS, DJANGO_31_PLUS, DJANGO_40_PLUS, DJANGO_42_PLUS
+from salesforce.backend import DJANGO_30_PLUS, DJANGO_31_PLUS, DJANGO_40_PLUS, DJANGO_42_PLUS
 from salesforce.backend.utils import FullResultSet
 from salesforce.dbapi import DatabaseError
-from salesforce.dbapi.subselect import AGGREGATION_WORDS
+from salesforce.dbapi.exceptions import SalesforceWarning
 # pylint:disable=no-else-return,too-many-branches,too-many-locals
 
 AliasMapItems = List[Tuple[
     Optional[str],
     str,
     Optional[Tuple[Tuple[str, str], ...]],
     str
 ]]
 
+objects_needing_minimal_aliases = [
+    'ContentDocumentLink', 'ContentFolderItem', 'ContentFolderMember', 'IdeaComment', 'Vote'
+]
+
 
 class SfParams:  # like an immutable DataClass: clone when updating
     def __init__(self):
         self.query_all = False
         self.all_or_none = None  # type: Optional[bool]
         self.edge_updates = False
         self.minimal_aliases = False
@@ -79,43 +84,53 @@
         """
         r = self.connection.ops.quote_name(name)
         self.quote_cache[name] = r
         return r
 
     def sf_fix_field(self, sql_field: str, debug_: int = 0) -> str:
         """Translate the field name from sql join "alias.name" to SOQL tree "object_1.object_2...name"."""
-        # debug_: 1 = print what is not recompiled, 2 = print everything
+        # debug_: 1 = print what is recompiled
         soql_trans = self.query_topology()
-        if '(' in sql_field:
-            match = re.match(r'^([A-Z_]+\()(\w+\.\w+)(\) (?:\w+|[!<>=]+ %s|LIKE %s))$', sql_field)
-            if not match or match.group(1)[:-1] not in AGGREGATION_WORDS:
-                if debug_:
-                    print("** sf_fix_field: Can not recompile sql: {!r}".format(sql_field))
-                return sql_field
-            pre, field, post = match.groups()
+        if sql_field.startswith('('):
+            return sql_field  # compiled and fixed yet
+        if re.match(r'[\w.]+$', sql_field) and len(sql_field.split('.')) == 2:
+            pre, field, post = '', sql_field, ''  # very easy fix for a simple 'select' field
+        elif sql_field.startswith('COUNT(Id)') and re.match(r'^COUNT\(Id\)(?: \w+)?$', sql_field, re.ASCII):
+            return sql_field  # not necessary to fix
         else:
-            if len(sql_field.split('.')) != 2:
-                if debug_:
-                    print("** sf_fix_field: Can not recompile sql: {!r}".format(sql_field))
+            match = re.match(r'^((?:\w+\()*)'     # optional some nested functions with one parameter
+                             r'((?:\w+\.)*\w+)'   # table.field
+                             r'('
+                             r'\)*'               # optional closing parentheses of functions
+                             # alias or operator with a placeholder %s of a parameter or 'IN (...'
+                             r'(?: (?:\w+|[!<>=]+ %s|LIKE %s|!?= null|(?:NOT )?IN \(.*))?)$',
+                             sql_field, re.ASCII)
+            if match:
+                pre, field, post = match.groups()
+                ok = len(field.rstrip('.Type').split('.')) == 2
+            if not match or not ok:
+                warnings.warn("sf_fix_field: Can not recompile unexpected sql: {!r}".format(sql_field),
+                              SalesforceWarning)
                 return sql_field
-            pre, field, post = '', sql_field, ''
-        tab_name, field_name = field.split('.')
-        if self.sf_params.minimal_aliases:
+        # fix the field
+        tab_name, field_name = field.split('.', 1)
+        if self.sf_params.minimal_aliases or tab_name in objects_needing_minimal_aliases:
             assert len(self.root_aliases) == 1
             if tab_name == self.root_aliases[0]:
                 trans_tab_name = ''
             else:
                 trans_root = soql_trans[self.root_aliases[0]]
                 assert soql_trans[tab_name].startswith(trans_root + '.')
                 trans_tab_name = soql_trans[tab_name].replace(trans_root + '.', '', 1)
         else:
             trans_tab_name = soql_trans[tab_name]
         dot = '.' if trans_tab_name else ''
         ret = "%s%s%s%s%s" % (pre, trans_tab_name, dot, field_name, post)
-        if debug_ >= 2:
+
+        if debug_:
             print('** sf_fix_field: {!r} -> {!r}'.format(sql_field, ret))
         return ret
 
     # patched and simplified the parend method  # pylint:disable=no-else-return
     def execute_sql(self,
                     result_type: str = constants.MULTI,
                     chunked_fetch: bool = False,
@@ -150,16 +165,16 @@
         if not result_type or result_type == 'cursor':
             return cursor
 
         if result_type == constants.SINGLE:
             return cursor.fetchone()
 
         # The MULTI case.
-        result = iter(lambda: cursor.fetchmany(chunk_size),
-                      self.connection.features.empty_fetchmany_value)  # type: Iterable[Any]
+        result: Iterable[Any] = iter(lambda: cursor.fetchmany(chunk_size),
+                                     self.connection.features.empty_fetchmany_value)
         if not chunked_fetch and not self.connection.features.can_use_chunked_reads:
             # If we are using non-chunked reads, we return the same data
             # structure as normally, but ensure it is all read into memory
             # before going any further. Use chunked_fetch if requested.
             return list(result)
         return result
         # pylint:enable=no-else-return
@@ -182,18 +197,15 @@
         # as the pre_sql_setup will modify query state in a way that forbids
         # another run of it.
         refcounts_before = self.query.alias_refcount.copy()
         try:
             extra_select, order_by, group_by = self.pre_sql_setup()
             if with_limits and self.query.low_mark == self.query.high_mark:
                 return '', ()
-            if DJANGO_21_PLUS:
-                distinct_fields, distinct_params = self.get_distinct()
-            else:
-                distinct_fields = self.get_distinct()  # type: ignore[assignment] # noqa
+            distinct_fields, distinct_params = self.get_distinct()
 
             # This must come after 'select', 'ordering', and 'distinct' -- see
             # docstring of get_from_clause() for details.
             from_, f_params = self.get_from_clause()
 
             try:
                 where, w_params = self.compile(self.where) if self.where is not None else ("", [])
@@ -203,34 +215,31 @@
                 having, h_params = self.compile(self.having) if self.having is not None else ("", [])
             except FullResultSet:
                 having, h_params = "", []
             params = []
             result = ['SELECT']
 
             if self.query.distinct:
-                if DJANGO_21_PLUS:
-                    distinct_result, distinct_params = self.connection.ops.distinct_sql(
-                        distinct_fields,
-                        distinct_params,
-                    )
-                    result += distinct_result
-                    params += distinct_params
-                else:
-                    result.append(self.connection.ops.distinct_sql(distinct_fields))
+                distinct_result, distinct_params = self.connection.ops.distinct_sql(
+                    distinct_fields,
+                    distinct_params,
+                )
+                result += distinct_result
+                params += distinct_params
 
             out_cols = []
             col_idx = 1
             for _, (s_sql, s_params), alias in self.select + extra_select:
+                s_sql = self.sf_fix_field(s_sql)
                 if alias:
                     # fixed by removing 'AS'
                     s_sql = '%s %s' % (s_sql, self.connection.ops.quote_name(alias))
                 elif with_col_aliases:
                     s_sql = '%s AS %s' % (s_sql, 'Col%d' % col_idx)
                     col_idx += 1
-                s_sql = self.sf_fix_field(s_sql)
                 params.extend(s_params)
                 out_cols.append(s_sql)
 
             result.append(', '.join(out_cols))
 
             result.append('FROM')
             result.extend(from_)
@@ -259,15 +268,15 @@
 
             if DJANGO_40_PLUS:
                 if self.query.explain_info:                # type: ignore[attr-defined]
                     result.insert(0, self.connection.ops.explain_query_prefix(
                         self.query.explain_info.format,    # type: ignore[attr-defined]
                         **self.query.explain_info.options  # type: ignore[attr-defined]
                     ))
-            elif DJANGO_21_PLUS:
+            else:
                 if self.query.explain_query:
                     result.insert(0, self.connection.ops.explain_query_prefix(
                         self.query.explain_format,
                         **self.query.explain_options
                     ))
 
             if order_by:
@@ -387,15 +396,15 @@
         assert len(soql_trans) == len(alias_map_items)
         self.soql_trans = soql_trans
         return self.soql_trans
 
 
 class SalesforceWhereNode(sql_where.WhereNode):
 
-    # patched "django.db.models.sql.where.WhereNode.as_sql" from Django 2.0, 2.1
+    # patched "django.db.models.sql.where.WhereNode.as_sql" from Django 2.1
     # pylint:disable=no-else-return,no-else-raise,too-many-branches,too-many-locals,unused-argument
     def as_salesforce(self, compiler: sql_compiler.SQLCompiler, connection) -> Tuple[str, List[Any]]:
         """
         Return the SQL version of the where clause and the value to be
         substituted in. Return '', [] if this node matches everything,
         None, [] if this node is empty, and raise EmptyResultSet if this
         node can't match anything.
```

### Comparing `django-salesforce-5.0.1/salesforce/backend/creation.py` & `django-salesforce-5.0.2/salesforce/backend/creation.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/backend/enterprise.py` & `django-salesforce-5.0.2/salesforce/backend/enterprise.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/backend/features.py` & `django-salesforce-5.0.2/salesforce/backend/features.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/backend/indep.py` & `django-salesforce-5.0.2/salesforce/backend/indep.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/backend/introspection.py` & `django-salesforce-5.0.2/salesforce/backend/introspection.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     'AsyncOperationEvent',  # new in API 46.0 Summer '19
     'AsyncOperationStatus',  # new in API 46.0 Summer '19
     'FlowExecutionErrorEvent',  # new in API 47.0 Winter '20 - missing 'Id'
     'FlowOrchestrationEvent',  # new in API 53.0 Winter '22
     'DataObjectDataChgEvent',  # new in API 55.0 Summer '22 (no 'Id' field)
     'OrgSharingEvent', 'StatsInvalidationEvent',  # new in API 59.0 Summer '24 (no 'Id' field)
     'EmailBounceEvent',  # new in API 60.0 Spring '24 (no 'Id' field)
+    'MLEngagementEvent',  # new in API 61.0 Summer '24 (no 'Id' field)
 ]
 
 # this global variable is for `salesforce.management.commands.inspectdb`
 last_introspection = None
 
 
 class LastIntrospection:
@@ -221,14 +222,16 @@
         else:
             default = None
         if default is not None:
             params['default'] = default
         elif field['defaultedOnCreate'] and field['createable'] and DJANGO_50_PLUS:
             params['db_default'] = SymbolicModelsName('DEFAULTED_ON_CREATE')
             params['blank'] = True
+        elif field['calculatedFormula']:
+            params['sf_formula'] = field['calculatedFormula']
 
         if field['inlineHelpText']:
             params['help_text'] = field['inlineHelpText']
         if field['picklistValues']:
             params['choices'] = [(x['value'], x['label']) for x in field['picklistValues'] if x['active']]
             max_inspectdb_picklist_picklist_length = getattr(settings, 'SF_MAX_INSPECTDB_PICKLIST_LENGTH', 4000)
             if len(repr(params['choices'])) < max_inspectdb_picklist_picklist_length:
```

### Comparing `django-salesforce-5.0.1/salesforce/backend/manager.py` & `django-salesforce-5.0.2/salesforce/backend/manager.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/backend/models_lookups.py` & `django-salesforce-5.0.2/salesforce/backend/models_lookups.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 """
 Lookups  (like django.db.models.lookups, django.db.models.aggregates.Count)
+
+Every overridden class here must be registered either:
+- registered by '@Field.register_lookup' if the parent class is registered
+or must be
+- setattr(parent_class, 'as_salesforce', overridden_class)  if the parent class is not registered
 """
 from django.db import models
 from django.db.models.fields import Field
 from django.db.models import lookups
 
 
 class IsNull(models.lookups.IsNull):  # pylint:disable=abstract-method
     def override_as_sql(self, compiler, connection):  # pylint:disable=unused-argument
-        # it must be relabeled if used for a children rows set
-        if compiler.soql_trans is None:
-            compiler.get_from_clause()
-        sql, params = compiler.compile(self.lhs.relabeled_clone(compiler.soql_trans))
-        return ('%s %s null' % (sql, ('=' if self.rhs else '!='))), params
+        # it will be relabeled later by sf_fix_field() to prevent a problematic double relabel
+        lhs, params = self.process_lhs(compiler, connection)
+        operator = '=' if self.rhs else '!='
+        return f"{lhs} {operator} null", params
 
     setattr(models.lookups.IsNull, 'as_salesforce', override_as_sql)
 
 
 class Range(models.lookups.Range):  # pylint:disable=abstract-method
     def override_as_sql(self, compiler, connection):
         lhs, lhs_params = self.process_lhs(compiler, connection)
         rhs, rhs_params = self.process_rhs(compiler, connection)
         assert rhs == ('%s', '%s')
         assert len(rhs_params) == 2
         params = lhs_params + [rhs_params[0]] + lhs_params + [rhs_params[1]]
-        # The symbolic parameters %s are again substituted by %s. The real
-        # parameters will be passed finally directly to CursorWrapper.execute
-        return '(%s >= %s AND %s <= %s)' % (lhs, rhs[0], lhs, rhs[1]), params
+        lhs = compiler.sf_fix_field(lhs)
+        return f'({lhs} >= %s AND {lhs} <= %s)', params
 
     setattr(models.lookups.Range, 'as_salesforce', override_as_sql)
 
 
 class Count(models.aggregates.Count):
     # pylint:disable=abstract-method,too-many-ancestors  # undefined __and__, __or__, __rand__, __ror__
 
@@ -63,7 +66,19 @@
 
 @Field.register_lookup
 class NotEqual(lookups.Exact):  # pylint:disable=abstract-method
     lookup_name = 'not_eq'
 
     def get_rhs_op(self, connection, rhs):
         return '!= %s' % rhs
+
+
+class YearLookup(lookups.YearLookup):
+    def override_as_sql(self, compiler, connection):
+        sql, params = self.as_sql(compiler, connection)
+        lhs, *rest = sql.split(' ', 1)
+        if rest == ["BETWEEN %s AND %s"]:
+            lhs = compiler.sf_fix_field(lhs)
+            sql = f"({lhs} >= %s AND {lhs} <= %s)"
+        return sql, params
+
+    setattr(lookups.YearLookup, 'as_salesforce', override_as_sql)
```

### Comparing `django-salesforce-5.0.1/salesforce/backend/models_sql_query.py` & `django-salesforce-5.0.2/salesforce/backend/models_sql_query.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/backend/query.py` & `django-salesforce-5.0.2/salesforce/backend/query.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/backend/schema.py` & `django-salesforce-5.0.2/salesforce/backend/schema.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/backend/test_helpers.py` & `django-salesforce-5.0.2/salesforce/backend/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/backend/utils.py` & `django-salesforce-5.0.2/salesforce/backend/utils.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/backend/validation.py` & `django-salesforce-5.0.2/salesforce/backend/validation.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/dbapi/__init__.py` & `django-salesforce-5.0.2/salesforce/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/dbapi/common.py` & `django-salesforce-5.0.2/salesforce/dbapi/common.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/dbapi/driver.py` & `django-salesforce-5.0.2/salesforce/dbapi/driver.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/dbapi/exceptions.py` & `django-salesforce-5.0.2/salesforce/dbapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/dbapi/subselect.py` & `django-salesforce-5.0.2/salesforce/dbapi/subselect.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/dbapi/test_helpers.py` & `django-salesforce-5.0.2/salesforce/dbapi/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/defaults.py` & `django-salesforce-5.0.2/salesforce/defaults.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/fields.py` & `django-salesforce-5.0.2/salesforce/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 
         custom=True : Add '__c' to the column name if no db_column is defined.
     """
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         self.sf_read_only = kwargs.pop('sf_read_only', 0)
         self.sf_custom = kwargs.pop('custom', None)
         self.sf_namespace = ''
+        self.sf_formula = kwargs.pop('sf_formula', None)
         if kwargs.get('default') is DEFAULTED_ON_CREATE:
             kwargs['default'] = DefaultedOnCreate(internal_type=self.get_internal_type())
         if 'db_default' in kwargs and not DJANGO_50_PLUS:
             del kwargs['db_default']
         super().__init__(*args, **kwargs)
 
     def get_attname_column(self) -> Tuple[str, str]:
```

### Comparing `django-salesforce-5.0.1/salesforce/management/commands/inspectdb.py` & `django-salesforce-5.0.2/salesforce/management/commands/inspectdb.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/models.py` & `django-salesforce-5.0.2/salesforce/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from django.db import models
 from django.db.models.base import ModelBase
 # Only these two `on_delete` options are currently supported
 from django.db.models import PROTECT, DO_NOTHING  # NOQA pylint:disable=unused-wildcard-import,wildcard-import
 # from django.db.models import CASCADE, PROTECT, SET_NULL, SET, DO_NOTHING
 
 from salesforce.defaults import DefaultedOnCreate, DEFAULTED_ON_CREATE
-from salesforce.fields import (  # pylint:disable=useless-import-alias
+from salesforce.fields import (
     SalesforceAutoField as SalesforceAutoField, SF_PK, SfField, ForeignKey as ForeignKey)
 from salesforce.fields import NOT_UPDATEABLE, NOT_CREATEABLE, READ_ONLY
 from salesforce.fields import (  # noqa pylint:disable=useless-import-alias  # for other modules, but unused here
     AutoField as AutoField, BigIntegerField as BigIntegerField, BooleanField as BooleanField,
     CharField as CharField, DateField as DateField, DateTimeField as DateTimeField,
     DecimalField as DecimalField, EmailField as EmailField, FloatField as FloatField,
     IntegerField as IntegerField, OneToOneField as OneToOneField, SmallIntegerField as SmallIntegerField,
```

### Comparing `django-salesforce-5.0.1/salesforce/models_extend.py` & `django-salesforce-5.0.2/salesforce/models_extend.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/models_template.py` & `django-salesforce-5.0.2/salesforce/models_template.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/router.py` & `django-salesforce-5.0.2/salesforce/router.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/testrunner/example/models.py` & `django-salesforce-5.0.2/salesforce/testrunner/example/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -433,18 +433,63 @@
     email = models.CharField(unique=True, max_length=255, verbose_name='email', blank=True)
 
 
 class Campaign(SalesforceModel):
     name = models.CharField(max_length=80)
     number_sent = models.DecimalField(max_digits=18, decimal_places=0, verbose_name='Num Sent', blank=True, null=True)
     parent = models.ForeignKey('Campaign', on_delete=models.DO_NOTHING, blank=True, null=True)
+    start_date = models.DateField(blank=True, null=True)
+    created_date = models.DateTimeField(sf_read_only=models.READ_ONLY, auto_now_add=True)
 
 
 class CampaignMember(SalesforceModel):
     campaign = models.ForeignKey(Campaign, on_delete=models.DO_NOTHING)
     contact = models.ForeignKey(Contact, on_delete=models.DO_NOTHING)
     status = models.CharField(max_length=40)
 
 
 # this model will be removed to test removing in migrations
 class DeletedObject(SalesforceModel):
     pass
+
+
+# models for work with file attachments of objects
+
+class ContentDocument(models.Model):
+    owner_id = models.CharField(max_length=18, sf_read_only=models.NOT_CREATEABLE)
+    title = models.CharField(max_length=255, sf_read_only=models.NOT_CREATEABLE)
+    latest_published_version = models.ForeignKey('ContentVersion', models.DO_NOTHING, sf_read_only=models.READ_ONLY,
+                                                 blank=True, null=True)
+    description = models.TextField(sf_read_only=models.NOT_CREATEABLE, blank=True, null=True)
+    content_size = models.IntegerField(sf_read_only=models.READ_ONLY, blank=True, null=True)
+    file_type = models.CharField(max_length=20, sf_read_only=models.READ_ONLY, blank=True, null=True)
+    file_extension = models.CharField(max_length=40, sf_read_only=models.READ_ONLY, blank=True, null=True)
+
+
+class ContentDocumentLink(models.Model):
+    linked_entity_id = models.CharField(max_length=18, sf_read_only=models.NOT_UPDATEABLE)
+    content_document = models.ForeignKey(ContentDocument, models.DO_NOTHING, sf_read_only=models.NOT_UPDATEABLE)
+    share_type = models.CharField(max_length=40, blank=True, null=True,
+                                  choices=[('V', 'Viewer'), ('C', 'Collaborator'), ('I', 'Inferred')])
+    visibility = models.CharField(max_length=40, blank=True, null=True,
+                                  choices=[('AllUsers', 'All Users'), ('InternalUsers', 'Standard Users'),
+                                           ('SharedUsers', 'Shared Users')])
+
+
+class ContentVersion(models.Model):
+    content_document = models.ForeignKey(ContentDocument, models.DO_NOTHING, sf_read_only=models.NOT_UPDATEABLE)
+    content_url = models.URLField(blank=True, null=True)
+    version_number = models.CharField(max_length=20, sf_read_only=models.READ_ONLY, blank=True, null=True)
+    title = models.CharField(max_length=255)
+    description = models.TextField(blank=True, null=True)
+    path_on_client = models.CharField(max_length=500, sf_read_only=models.NOT_UPDATEABLE, blank=True, null=True)
+    owner = models.ForeignKey(User, models.DO_NOTHING, db_default=models.DEFAULTED_ON_CREATE, blank=True)
+    file_type = models.CharField(max_length=20, sf_read_only=models.READ_ONLY)
+    version_data = models.TextField(blank=True, null=True)
+    content_size = models.IntegerField(sf_read_only=models.READ_ONLY, blank=True, null=True)
+    file_extension = models.CharField(max_length=40, sf_read_only=models.READ_ONLY, blank=True, null=True)
+    origin = models.CharField(max_length=40, sf_read_only=models.NOT_UPDATEABLE, default='C',
+                              choices=[('C', 'Content'), ('H', 'Chatter')])
+    content_location = models.CharField(max_length=40, sf_read_only=models.NOT_UPDATEABLE, default='S',
+                                        choices=[('S', 'Salesforce'), ('E', 'External'),
+                                                 ('L', 'Social Customer Service')])
+    version_data_url = models.CharField(max_length=255, sf_read_only=models.READ_ONLY, blank=True, null=True)
```

### Comparing `django-salesforce-5.0.1/salesforce/testrunner/example/models_template.py` & `django-salesforce-5.0.2/salesforce/testrunner/example/models_template.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/testrunner/example/templates/search-accounts.html` & `django-salesforce-5.0.2/salesforce/testrunner/example/templates/search-accounts.html`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/testrunner/example/universal_admin.py` & `django-salesforce-5.0.2/salesforce/testrunner/example/universal_admin.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/testrunner/example/views.py` & `django-salesforce-5.0.2/salesforce/testrunner/example/views.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/testrunner/local_settings.py.sample` & `django-salesforce-5.0.2/salesforce/testrunner/local_settings.py.sample`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/testrunner/settings.py` & `django-salesforce-5.0.2/salesforce/testrunner/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -189,12 +189,20 @@
 # Name of primary key - by default 'id'. The value 'Id' was the default for
 # version "django-salesforce < 0.5".
 # The value SF_PK can not be changed after any migration for Salesforce has been created
 # SF_PK = 'Id'
 
 DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'  # not important for Salesforce, but for Django warnings
 
+# Django Debug Toolbar >= 4.4.0
+# Django changes the DEBUG setting to False when running tests.
+# By default the Django Debug Toolbar is installed because DEBUG is set to True.
+# For most cases, you need to avoid installing the toolbar when running tests.
+# If you feel this check is in error, you can set
+# `DEBUG_TOOLBAR_CONFIG['IS_RUNNING_TESTS'] = False` to bypass this check.
+DEBUG_TOOLBAR_CONFIG = {'IS_RUNNING_TESTS': False}
+
 DJSF_LICENSE_KEY = os.environ.get('DJSF_LICENSE_KEY', '')  # configure for enterprise features
 try:
     from salesforce.testrunner.local_settings import *  # noqa pylint:disable=unused-wildcard-import,wildcard-import
 except ImportError:
     pass
```

### Comparing `django-salesforce-5.0.1/salesforce/testrunner/test_patch.diff` & `django-salesforce-5.0.2/salesforce/testrunner/test_patch.diff`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/tests/test_auth.py` & `django-salesforce-5.0.2/salesforce/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/tests/test_basic.py` & `django-salesforce-5.0.2/salesforce/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/tests/test_browser.py` & `django-salesforce-5.0.2/salesforce/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/tests/test_bulk.py` & `django-salesforce-5.0.2/salesforce/tests/test_bulk.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/tests/test_indep.py` & `django-salesforce-5.0.2/salesforce/tests/test_indep.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/tests/test_integration.py` & `django-salesforce-5.0.2/salesforce/tests/test_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 import os
 import warnings
 from typing import Any, cast, List, TypeVar
 
 import pytz
 from django.conf import settings
 from django.db import connections
-from django.db.models import Q, Avg, Count, Sum, Min, Max, Model, query as models_query
+from django.db.models import Q, Avg, Count, Sum, Min, Max, Model, query as models_query, functions
 from django.test import TestCase, override_settings
 from django.utils import timezone
 from django.utils.crypto import get_random_string
 
 import salesforce
 from salesforce import router
-from salesforce.backend import DJANGO_21_PLUS, DJANGO_22_PLUS, DJANGO_50_PLUS
+from salesforce.backend import DJANGO_22_PLUS, DJANGO_50_PLUS
 from salesforce.backend.test_helpers import (  # noqa pylint:disable=unused-import
     expectedFailure, expectedFailureIf, skip, skipUnless, strtobool)
 from salesforce.backend.test_helpers import (
     current_user, default_is_sf, sf_alias, uid_version as uid,
     QuietSalesforceErrors, LazyTestMixin)
 from salesforce.dbapi.driver import ApiUsage
 from salesforce.dbapi.exceptions import SalesforceWarning
@@ -54,18 +54,17 @@
 def sf_tables() -> List[str]:
     if not _sf_tables and default_is_sf:
         for x in connections[sf_alias].introspection.table_list_cache['sobjects']:
             _sf_tables.append(x['name'])
     return _sf_tables
 
 
-# The field name 'id' or 'Id' must be never used in Python code in tests that
-# should work with both variants of SF_PK. The universale name 'pk' should be
-# used insted.
-# The name 'Id' should be used in SQL code, but the name 'id' would work just as well.
+# The field name 'id' or 'Id' in these universal tests that should work with
+# both variants of SF_PK. The name 'pk' is prefered here.
+# The name 'Id' is used in SQL code, but the name 'id' would work just as well.
 
 def refresh(obj: _M) -> _M:
     """Get the same object refreshed from the same db.
     """
     db = obj._state.db
     qs: models_query.QuerySet[_M] = type(obj).objects.using(db)
     return qs.get(pk=obj.pk)
@@ -108,15 +107,15 @@
             '%s' % contacts[0].__dict__  # Check that all fields are accessible
         self.lazy_check()
 
     @skipUnless(default_is_sf, "Default database should be any Salesforce.")
     def test_raw_translations(self) -> None:
         """Read a Contact raw and translate it to Lead fields."""
         contact = Contact.objects.all()[0]
-        # `translation` dictionary keys must be lowercase now
+        # `translation` dictionary key is lowercase
         false_lead_raw = list(Lead.objects.raw(
             "SELECT Id, LastName FROM Contact WHERE Id=%s", params=[contact.pk],
             translations={'lastname': 'Company'}))
         self.assertEqual(len(false_lead_raw), 1)
         self.assertEqual(false_lead_raw[0].Company, contact.last_name)
 
     @skipUnless(default_is_sf, "Default database should be any Salesforce.")
@@ -266,15 +265,15 @@
             # test 1b is unique value
             duplicate = ApexEmailNotification(user=current_sf_user)
             # the method self.assertRaise was too verbose about exception
             try:
                 with QuietSalesforceErrors(sf_alias):
                     duplicate.save()
             except salesforce.backend.base.SalesforceError as exc:
-                # TODO uncovered line, baybe bug
+                # TODO uncovered line, maybe bug
                 self.assertEqual(exc.data[0]['errorCode'], 'DUPLICATE_VALUE')  # type: ignore
             else:
                 self.assertRaises(salesforce.backend.base.SalesforceError, duplicate.save)
 
             # test 2: the reverse relation is a value, not a set
             users = User.objects.exclude(apex_email_notification__user=None)
             self.assertIn(current_user, [x.Username for x in users])
@@ -286,19 +285,14 @@
             # probably caused by .mypy_cache  # TODO report it if reproduced with a new django-stubs version
             self.assertEqual(result[0].user_id, notifier_u.user_id)
         finally:
             if new_u:
                 new_u.delete()
             if new_e:
                 new_e.delete()
-
-        # this had fail, therefore moved at the end and itemized for debugging
-        # qs = User.objects.exclude(apex_email_notification=None)
-        # print(qs.query.get_compiler('salesforce').as_sql())
-        # list(qs)
         list(User.objects.exclude(apex_email_notification=None))
 
     def test_update_date(self) -> None:
         """Test updating a date.
         """
         # removed microseconds only for easy compare in the test, no problem
         now = timezone.now().replace(microsecond=0)
@@ -505,16 +499,16 @@
     def test_datetime_miliseconds(self) -> None:
         """Verify that a field with milisecond resolution is readable.
         """
         triggers = CronTrigger.objects.all()
         if not triggers:
             self.skipTest("No object with milisecond resolution found.")
         self.assertTrue(isinstance(triggers[0].PreviousFireTime, datetime.datetime))
-        # The reliability of this is only 99.9%, therefore it is commented out.
-        # self.assertNotEqual(trigger.PreviousFireTime.microsecond, 0)
+        if all(trigger.PreviousFireTime.microsecond == 0 for trigger in triggers):
+            self.skipTest("Miliseconds == 0; That is possible with probability 0.1%, not error")
 
     @skipUnless(default_is_sf, "Default database should be any Salesforce.")
     def test_time_field(self) -> None:
         """Test a TimeField (read, modify, verify).
         """
         obj_orig = BusinessHours.objects.all()[0]
         obj = refresh(obj_orig)
@@ -799,15 +793,14 @@
                      len(leads_list))
             self.skipTest("Not enough Leads found for big query test")
 
     @skipUnless(default_is_sf, "Default database should be any Salesforce.")
     def test_cursor_execute_fetch(self) -> None:
         """Get results by cursor.execute(...); fetchone(), fetchmany(), fetchall()
         """
-        # TODO hy: fix for concurrency
         sql = "SELECT Id, LastName, FirstName, OwnerId FROM Contact LIMIT 2"
         cursor = connections[sf_alias].cursor()
         cursor.execute(sql)
         contacts = cursor.fetchall()
         self.assertEqual(len(contacts), 2)
         self.assertTrue(contacts[0][3].startswith('005'), "OwnerId must be an User.")
         cursor.execute(sql)
@@ -966,16 +959,15 @@
         self.assertEqual(len(values[0]), 3)
         if default_is_sf:
             self.assertRegex(cast(str, values[0]['pk']), '^003')
 
         values_list = Contact.objects.values_list('pk', 'first_name', 'last_name')[:2]
         self.assertEqual(len(values_list), 2)
         v0 = values[0]
-        # it is a list in Django 2.1, but a tuple in Django 2.0
-        self.assertEqual(list(values_list[0]), [v0['pk'], v0['first_name'], v0['last_name']])
+        self.assertEqual(values_list[0], (v0['pk'], v0['first_name'], v0['last_name']))
 
     @skipUnless(default_is_sf, "Default database should be any Salesforce.")
     def test_double_delete(self) -> None:
         """Test that repeated delete of the same object is ignored
 
         the same way like "DELETE FROM Contact WHERE Id='deleted yet'" would do.
         """
@@ -1049,19 +1041,14 @@
                 salesforce.auth.oauth_data[db]['access_token'] += 'simulated invalid/expired'
             for x in objects:
                 self.assertTrue(refresh(x))
         finally:
             for x in objects:
                 x.delete()
 
-    # This should not be implemented due to Django conventions.
-    # def test_raw_aggregate(self):
-    #    # raises "TypeError: list indices must be integers, not str"
-    #    list(Contact.objects.raw("select Count() from Contact"))
-
     @skipUnless(default_is_sf, "Default database should be any Salesforce.")
     def test_only_fields(self) -> None:
         """Verify that access to "only" fields doesn't require a request, but others do.
         """
         # print([(x.pk, x.last_name) for x in Contact.objects.only('last_name').order_by('pk')[:2]])
         with self.lazy_assert_n_requests(0):
             sql = User.objects.only('Username').query.get_compiler('salesforce').as_sql()[0]
@@ -1113,17 +1100,15 @@
         with self.lazy_assert_n_requests(1):
             _ = contact.email
         self.lazy_check()
         _  # noqa
 
     def test_incomplete_raw(self) -> None:
         """Test that omitted model fields can be queried by dot."""
-        # with self.lazy_assert_n_requests(2):  # problem - Why too much requests?
-        # raw query must contain the primary key (with the right capitalization, currently)
-        with self.lazy_assert_n_requests(1):  # TODO why two requests?
+        with self.lazy_assert_n_requests(1):
             ret = list(Contact.objects.raw("select Id from Contact where FirstName != '' limit 2000"))
         with self.lazy_assert_n_requests(1):
             last_name = ret[0].last_name
         self.assertTrue(last_name and 'last' not in last_name.lower())
         with self.lazy_assert_n_requests(1):
             first_name = ret[0].first_name
         with self.lazy_assert_n_requests(0):
@@ -1139,22 +1124,18 @@
         """
         test_lead = Lead(Company='sf_test lead', LastName='name')
         test_lead.save()
         try:
             qs = Lead.objects.filter(pk=test_lead.pk,
                                      owner__Username=current_user,
                                      last_modified_by__Username=current_user)
-            # Verify that a coplicated analysis is not performed on old Django
-            # so that the query can be at least somehow simply compiled to SOQL
-            # without exceptions, in order to prevent regressions.
             sql, params = qs.query.get_compiler('salesforce').as_sql()
-            # Verify expected filters in SOQL compiled by new Django
-            self.assertIn('Lead.Owner.Username = %s', sql)
-            self.assertIn('Lead.LastModifiedBy.Username = %s', sql)
-            # verify validity for SFDC, verify results
+            sql_parts = set(sql.split(' WHERE (')[1].rstrip(')').split(' AND '))
+            self.assertEqual(sql_parts,
+                             {'Lead.Id = %s', 'Lead.Owner.Username = %s', 'Lead.LastModifiedBy.Username = %s'})
             refreshed_lead = qs.get()
             self.assertEqual(refreshed_lead.pk, test_lead.pk)
         finally:
             test_lead.delete()
 
     @skipUnless(default_is_sf, "Default database should be any Salesforce.")
     def test_filter_by_more_fk_to_the_same_model_subquery(self) -> None:
@@ -1219,15 +1200,14 @@
         oc = OpportunityContactRole(opportunity=oppo, contact=contact, role='sponsor')
         oc.save()
         oc2 = OpportunityContactRole(opportunity=oppo, contact=contact, role='evaluator')
         oc2.save()
         try:
             qs = Contact.objects.filter(opportunity_roles__opportunity__name='test op')
             self.assertEqual(list(qs), 2 * [contact])
-            # self.assertEqual([x.pk for x in qs], 2 * [oppo.pk])
         finally:
             oc2.delete()
             oc.delete()
             oppo.delete()
 
     def test_filter_custom(self) -> None:
         """Verify that relations between custom and builtin objects
@@ -1240,19 +1220,28 @@
         # "SELECT Attachment.Id FROM Attachment WHERE Attachment.Parent.Name = 'abc'"
         list(qs)
         qs2 = Test.objects.filter(contact__last_name='Johnson')
         # "SELECT ... FROM django_Test__c WHERE django_Test__c.Contact__r.LastName = 'Johnson'")
         list(qs2)
         qs = Attachment.objects.filter(parent__in=Test.objects.filter(contact__last_name='Johnson'))
         list(qs)
+        # test the '__range' lookup
+        qs = Test.objects.filter(contact__name__range=('a', 'b')).values('pk').sf(minimal_aliases=True)
+        expect_sql = "SELECT Id FROM django_Test__c WHERE (Contact__r.Name >= 'a' AND Contact__r.Name <= 'b')"
+        list(qs)
+        self.assertEqual(str(qs.query), expect_sql)
 
     def test_using_none(self) -> None:
         alias = getattr(settings, 'SALESFORCE_DB_ALIAS', 'salesforce')
         self.assertEqual(Contact.objects.using(None)._db, alias)
 
+    def test_with_offst(self) -> None:
+        list(Contact.objects.all()[1:2])
+        list(Contact.objects.all()[2000:])
+
     @skipUnless(default_is_sf, "depends on Salesforce database.")
     def test_dynamic_fields(self) -> None:
         """Test that fields can be copied dynamically from other model"""
         self.assertTrue(models_template)
         self.assertIn('@', Organization.objects.get().created_by.Username)
 
     @skipUnless(default_is_sf, "depends on Salesforce database.")
@@ -1269,27 +1258,52 @@
         processed_soql = connections[sf_alias].connection.debug_info['soql'][2]
         self.assertGreater(len(processed_soql), 90000)
 
     def test_empty_slice(self) -> None:
         """Test queryset with empty slice - if high/low limits equals"""
         self.assertEqual(len(Contact.objects.all()[1:1]), 0)
 
-    @skipUnless(DJANGO_21_PLUS, "Method .explain() is only in Django >= 2.1")
     @skipUnless(default_is_sf, "depends on Salesforce database.")
     def test_select_explan(self) -> None:
         """Test EXPLAIN SELECT ..."""
         qs = Contact.objects.all()[:2]
         self.assertRegex(qs.explain(), r"^{'plans': \[{")
 
     def test_api_usage(self) -> None:
         """Test that API usage is updated by executing requests"""
         api_usage: ApiUsage = connections[sf_alias].connection.api_usage
         self.assertGreater(api_usage.api_usage, 0)
         self.assertGreater(api_usage.api_limit, 5000)
 
+    def test_extract_date(self) -> None:
+        campaign = Campaign.objects.create(name='test something', number_sent=3)
+        try:
+            # group datetime by year
+            list(Campaign.objects.values('created_date__year').annotate(total=Sum('number_sent')))
+            # filter datetime last year
+            list(Campaign.objects.filter(created_date__year=2023, number_sent__gte=100))
+            # filter date last year and group by month
+            list(Campaign.objects.filter(start_date__year=2023).values('start_date__month').annotate(cnt=Count('pk')))
+            # filter datetatetime by month
+            list(Campaign.objects.filter(created_date__month=1))
+            # filter datetatetime by quarter
+            list(Campaign.objects.filter(created_date__quarter=1))
+            # group by date from a DateTime field
+            list(Campaign.objects.values(c_date=functions.TruncDate('created_date')).annotate(cnt=Count('start_date')))
+            # example group by all possible type of datetime lookup expressions
+            list(Campaign.objects.values('start_date__year', 'start_date__month', 'start_date__day',
+                                         'start_date__week', 'start_date__week_day',
+                                         'start_date__quarter').annotate(total=Count('pk')))
+            list(Campaign.objects.values('created_date__year', 'created_date__month', 'created_date__day',
+                                         'created_date__week', 'created_date__week_day',
+                                         'created_date__hour', 'created_date__quarter').annotate(total=Count('pk')))
+        finally:
+            campaign.delete()
+
+
 # ============= Tests that need setUp Lead ==================
 
 
 class BasicLeadSOQLTest(TestCase):
     """Tests that use a test Lead"""
     databases = '__all__'
```

### Comparing `django-salesforce-5.0.1/salesforce/tests/test_unit.py` & `django-salesforce-5.0.2/salesforce/tests/test_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Type
 from django.apps.registry import Apps
 from django.test import TestCase
 from django.db.models import DO_NOTHING, Subquery
 from salesforce import fields, models
 from salesforce.dbapi import driver
 from salesforce.testrunner.example.models import (
-        Contact, Opportunity, OpportunityContactRole, ChargentOrder)
+        Contact, Opportunity, OpportunityContactRole, ChargentOrder, Test as TestModel)
 from salesforce.backend.test_helpers import default_is_sf, LazyTestMixin, skipUnless
 from salesforce.backend.utils import sobj_id
 
 
 class EasyCharField(models.CharField):
     def __init__(self, max_length=255, null=True, default='', **kwargs):
         super().__init__(max_length=max_length, null=null, default=default, **kwargs)
@@ -184,14 +184,22 @@
         alias_map_items = [
             (None, 'A', None, 'A'),
             ('A', 'C', (('Id', 'AId'),), 'C'),
             ('C', 'B', (('BId', 'Id'),), 'B')]
         self.assertTopo(alias_map_items, {'C': 'C', 'A': 'C.A', 'B': 'C.B'})
 
 
+class QueryTest(TestCase):
+    def test_where_related_in(self):
+        qs = TestModel.objects.filter(contact__name__in=('a', 'b')).values('pk')
+        soql = qs.query.get_compiler('salesforce').as_sql()[0]
+        expected = "SELECT django_Test__c.Id FROM django_Test__c WHERE django_Test__c.Contact__r.Name IN (%s, %s)"
+        self.assertEqual(soql, expected)
+
+
 class SfParamsTest(TestCase):
     # type checking of this test case is currently not possible
     databases = '__all__'
 
     def test_params_handover_and_isolation(self):
         """Test that sp_params are propagated to the rest of the queryset chain
         but isolated from the previous part.
```

### Comparing `django-salesforce-5.0.1/salesforce/tests/test_utils.py` & `django-salesforce-5.0.2/salesforce/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/tests/unit_tests/test_qparser.py` & `django-salesforce-5.0.2/salesforce/tests/unit_tests/test_qparser.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/salesforce/utils.py` & `django-salesforce-5.0.2/salesforce/utils.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/setup.py` & `django-salesforce-5.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         include_package_data=True,
         zip_safe=False,
         packages=find_packages(exclude=['tests', 'tests.*']),
 
         # setuptools won't auto-detect Git managed files without this
         setup_requires=[] if not with_git else ["setuptools_git >= 0.4.2"],
 
-        install_requires=['django>=2.0'] + requirements_txt,
+        install_requires=['django>=2.1'] + requirements_txt,
 
         # metadata for upload to PyPI
         author="Hynek Cernoch",
         author_email="hynek@sdb.cz",
         maintainer="Phil Christensen",
         maintainer_email="phil@bubblehouse.org",
         description="a Salesforce backend for Django's ORM",
```

### Comparing `django-salesforce-5.0.1/tests/clean_test_data.py` & `django-salesforce-5.0.2/tests/clean_test_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 but a test interrupted by debugger or Ctrl-C could do it.
 """
 from typing import List
 from unittest import TestCase
 from django.db.models import Q
 from salesforce.backend.operations import BULK_BATCH_SIZE
 from salesforce.backend.query import SalesforceQuerySet
-from salesforce.testrunner.example.models import Account, Campaign, Contact, Lead, Opportunity, Product, Test
+from salesforce.testrunner.example.models import (Account, Campaign, Contact, Lead, Opportunity, Product, Test,
+                                                  ContentDocument)
 from salesforce.tests.test_integration import sf_tables
 
 
 def qs_delete(qs: SalesforceQuerySet) -> List[int]:
     """Delete all items of queryset"""
     ret = list(qs)
     s = 0
@@ -33,14 +34,15 @@
             )),
             qs_delete(Campaign.objects.filter(name__startswith='test ')),
             qs_delete(Contact.objects.filter(Q(first_name__startswith='sf_test') | Q(last_name__startswith='sf_test') |
                                              Q(name='Joe Freelancer'))),
             qs_delete(Lead.objects.filter(LastName__startswith='UnitTest')),
             qs_delete(Opportunity.objects.filter(name__in=('test op', 'Example Opportunity'))),
             qs_delete(Product.objects.filter(Name__startswith='test ')),
+            qs_delete(ContentDocument.objects.filter(title='some file.txt')),
         ]
         if 'django_Test__c' in sf_tables():
             ret.append(qs_delete(Test.objects.all()))
         print("Deleted objects={}".format(sum(x[0] for x in ret)))
 
     def test_clean_all_test_data(self):
         """It is cleaninng all known test data that can be necessary sometimes after interrupted tests
```

### Comparing `django-salesforce-5.0.1/tests/db.sqlite3` & `django-salesforce-5.0.2/tests/db.sqlite3`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/inspectdb/slow_test.py` & `django-salesforce-5.0.2/tests/inspectdb/slow_test.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/inspectdb/test.sh` & `django-salesforce-5.0.2/tests/inspectdb/test.sh`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/inspectdb/tests.py` & `django-salesforce-5.0.2/tests/inspectdb/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/mypy.sh` & `django-salesforce-5.0.2/tests/mypy.sh`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/no_django_dbapi/test.py` & `django-salesforce-5.0.2/tests/no_django_dbapi/test.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/no_salesforce/models.py` & `django-salesforce-5.0.2/tests/no_salesforce/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/no_salesforce/settings.py` & `django-salesforce-5.0.2/tests/no_salesforce/settings.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/no_salesforce/tests.py` & `django-salesforce-5.0.2/tests/no_salesforce/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/t_debug_toolbar/small_app/models.py` & `django-salesforce-5.0.2/tests/t_debug_toolbar/small_app/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/t_debug_toolbar/tests.py` & `django-salesforce-5.0.2/tests/t_debug_toolbar/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_compatibility/models.py` & `django-salesforce-5.0.2/tests/test_compatibility/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_compatibility/tests.py` & `django-salesforce-5.0.2/tests/test_compatibility/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_default_db/models.py` & `django-salesforce-5.0.2/tests/test_default_db/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_default_db/tests.py` & `django-salesforce-5.0.2/tests/test_default_db/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_dynamic_auth/settings.py` & `django-salesforce-5.0.2/tests/test_dynamic_auth/settings.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_dynamic_auth/tests.py` & `django-salesforce-5.0.2/tests/test_dynamic_auth/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_general/test_helpers.py` & `django-salesforce-5.0.2/tests/test_general/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_lazy_connect/settings.py` & `django-salesforce-5.0.2/tests/test_lazy_connect/settings.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_lazy_connect/tests.py` & `django-salesforce-5.0.2/tests/test_lazy_connect/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_managers/models.py` & `django-salesforce-5.0.2/tests/test_managers/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_managers/tests.py` & `django-salesforce-5.0.2/tests/test_managers/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_migrate/models.py` & `django-salesforce-5.0.2/tests/test_migrate/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_migrate/settings.py` & `django-salesforce-5.0.2/tests/test_migrate/settings.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_migrate/test.sh` & `django-salesforce-5.0.2/tests/test_migrate/test.sh`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_migrate/tests.py` & `django-salesforce-5.0.2/tests/test_migrate/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_mixin/models.py` & `django-salesforce-5.0.2/tests/test_mixin/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_mixin/tests.py` & `django-salesforce-5.0.2/tests/test_mixin/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_mock/mocksf.py` & `django-salesforce-5.0.2/tests/test_mock/mocksf.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_mock/settings.py` & `django-salesforce-5.0.2/tests/test_mock/settings.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_mock/test_data.py` & `django-salesforce-5.0.2/tests/test_mock/test_data.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_mock/test_mocksf.py` & `django-salesforce-5.0.2/tests/test_mock/test_mocksf.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_mock2/migrations/0001_initial.py` & `django-salesforce-5.0.2/tests/test_mock2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_mock2/models.py` & `django-salesforce-5.0.2/tests/test_mock2/models.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_mock2/settings.py` & `django-salesforce-5.0.2/tests/test_mock2/settings.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/test_mock2/test_rec.py` & `django-salesforce-5.0.2/tests/test_mock2/test_rec.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/to_mock.py` & `django-salesforce-5.0.2/tests/to_mock.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/tooling/slow_test.py` & `django-salesforce-5.0.2/tests/tooling/slow_test.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/tooling/test.sh` & `django-salesforce-5.0.2/tests/tooling/test.sh`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tests/tooling/tests.py` & `django-salesforce-5.0.2/tests/tooling/tests.py`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/tox.ini` & `django-salesforce-5.0.2/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -4,43 +4,42 @@
 
 [tox]
 # test the highest version, the lowest, Django 2.2 and some versions complementary to Github Actions
 # version Django 2.2 is special - some code in salesforce.backend.query is used only with this version.
 envlist =
     docs_style
     typing
-    dj50-py313
+    # dj50-py313
+    dj50-py312
     dj42-py312
     dj41-py311
     dj40-py310
     dj32-py39
     dj30-py38
-    dj22-py37
-    dj20-py37
-    # djdev-py312
+    dj22-py38
+    dj21-py38
+    # djdev-py313
     no_django-py311
     debug_toolbar-dj50-py312
     # pylint-dj42-py310`
 
-# Python versions used for Github Actions with the latest Ubuntu 22 Jammy Jellyfish are 3.8, 3.11, "3.10", 3.7, 3.9
+# Python versions used for Github Actions with the latest Ubuntu 22 Jammy Jellyfish are 3.8, 3.11, "3.10", 3.9
 
 [testenv]
 basepython =
-    py37: python3.7
     py38: python3.8
     py39: python3.9
     py310: python3.10
     py311: python3.11
     py312: python3.12
     py313: python3.13
     pypy: pypy
     pypy3: pypy3
 deps =
-    # minimal required versions for all supported Python versions
-    dj20: Django~=2.0.0   # py34-37
+    # listed also a range of Python versions officially supported by Django
     dj21: Django~=2.1.0   # py35-37
     dj22: Django~=2.2.17  # py35-37
     dj30: Django~=3.0.11  # py36-39
     dj31: Django~=3.1.3   # py36-39
     dj32: Django~=3.2.0   # py36-39
     dj40: Django~=4.0.0   # py38-310
     dj41: Django~=4.1.0   # py38-310
@@ -82,20 +81,20 @@
 basepython = python3
 commands =
     {envpython} manage.py test tests.clean_test_data
 
 [testenv:debug_toolbar-dj{32-py39,42-py39,50-py312}]
 commands = {envpython} manage.py test tests.t_debug_toolbar --settings=tests.t_debug_toolbar.settings
 
-[testenv:pylint-dj{20-py37,22-py37,30-py39,32-py39,40-py310,41-py310,42-py310}]
-# Python 3.11 will require "wrapt>=1.14.1" and therefore Python between 3.7 and 3.10 is used with pylint
+[testenv:pylint-dj{21-py38,22-py38,30-py39,32-py39,40-py310,41-py310,42-py310}]
+# Python 3.11 will require "wrapt>=1.14.1" and therefore Python between 3.8 and 3.10 is used with pylint
 setenv = DJANGO_SETTINGS_MODULE=salesforce.testrunner.settings
 commands = pylint --reports=no salesforce
 
-[testenv:no_django-py{37,39,311}]
+[testenv:no_django-py{38,39,311}]
 usedevelop=True
 allowlist_externals =
     rm
     {toxinidir}/tests/tests_no_django.sh
 commands =
     # remove Django because it has been installed by setup.py now if not by tox
     rm -rf {envsitepackagesdir}/django
@@ -110,15 +109,15 @@
     flake8<6.0
     rstcheck
 commands =
     flake8
     rstcheck --recursive README.rst CHANGELOG.rst docs
 
 [testenv:typing]
-# any python >= 3.5.3, < 3.9
+# currently only python3.8 is supported for typing with django-salesforce-stubs
 basepython = python3.8
 deps =
     mypy==0.770
     git+https://github.com/hynekcer/django-salesforce-stubs.git@v1.5.0.3#django-stubs
 allowlist_externals =
     bash
     touch
```

### Comparing `django-salesforce-5.0.1/wiki/Documents-and-Attachments.md` & `django-salesforce-5.0.2/wiki/Documents-and-Attachments.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/wiki/Empty-strings-in-filters.md` & `django-salesforce-5.0.2/wiki/Empty-strings-in-filters.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/wiki/Error-messages.md` & `django-salesforce-5.0.2/wiki/Error-messages.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/wiki/Experimental-Features.rest` & `django-salesforce-5.0.2/wiki/Experimental-Features.rest`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/wiki/Foreign-Key-Support.rest` & `django-salesforce-5.0.2/wiki/Foreign-Key-Support.rest`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/wiki/Home.md` & `django-salesforce-5.0.2/wiki/Home.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/wiki/Introspection-and-Special-Attributes-of-Fields.rest` & `django-salesforce-5.0.2/wiki/Introspection-and-Special-Attributes-of-Fields.rest`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/wiki/Lead-Conversion.rest` & `django-salesforce-5.0.2/wiki/Lead-Conversion.rest`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/wiki/Release-Process.md` & `django-salesforce-5.0.2/wiki/Release-Process.md`

 * *Files identical despite different names*

### Comparing `django-salesforce-5.0.1/wiki/SalesforceModels-used-with-local-databases.md` & `django-salesforce-5.0.2/wiki/SalesforceModels-used-with-local-databases.md`

 * *Files identical despite different names*

