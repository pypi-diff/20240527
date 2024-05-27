# Comparing `tmp/django_import_export-4.0.3.tar.gz` & `tmp/django_import_export-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_import_export-4.0.3.tar", last modified: Thu May 16 13:47:07 2024, max compression
+gzip compressed data, was "django_import_export-4.0.5.tar", last modified: Thu May 23 18:32:40 2024, max compression
```

## Comparing `django_import_export-4.0.3.tar` & `django_import_export-4.0.5.tar`

### file list

```diff
@@ -1,344 +1,345 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.546338 django_import_export-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.506338 django_import_export-4.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.506338 django_import_export-4.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.506338 django_import_export-4.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-16 13:47:03.000000 django_import_export-4.0.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-16 13:47:03.000000 django_import_export-4.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-16 13:47:03.000000 django_import_export-4.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-16 13:47:03.000000 django_import_export-4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-16 13:47:03.000000 django_import_export-4.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-16 13:47:07.546338 django_import_export-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-16 13:47:03.000000 django_import_export-4.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-16 13:47:03.000000 django_import_export-4.0.3/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-16 13:47:03.000000 django_import_export-4.0.3/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.546338 django_import_export-4.0.3/django_import_export.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-16 13:47:07.000000 django_import_export-4.0.3/django_import_export.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-05-16 13:47:07.000000 django_import_export-4.0.3/django_import_export.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:47:07.000000 django_import_export-4.0.3/django_import_export.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 13:47:07.000000 django_import_export-4.0.3/django_import_export.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 13:47:07.000000 django_import_export-4.0.3/django_import_export.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.510338 django_import_export-4.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.494338 django_import_export-4.0.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.514338 django_import_export-4.0.3/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/change-form-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/custom-export-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/custom-import-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/date-widget-validation-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/django-import-export-change.png
--rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/django-import-export-export-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/django-import-export-import-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/django-import-export-import.png
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/export-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/export_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/import-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/import_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/non-field-specific-validation-error.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.518338 django_import_export-4.0.3/docs/_static/images/screenshots/
--rw-r--r--   0 runner    (1001) docker     (127)   445502 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/screenshots/confirm-import.png
--rw-r--r--   0 runner    (1001) docker     (127)   311653 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/screenshots/export-form.png
--rw-r--r--   0 runner    (1001) docker     (127)   469577 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/screenshots/export-selected-action.png
--rw-r--r--   0 runner    (1001) docker     (127)   447473 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/screenshots/import-complete.png
--rw-r--r--   0 runner    (1001) docker     (127)   308805 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/screenshots/import-form.png
--rw-r--r--   0 runner    (1001) docker     (127)   313540 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/screenshots/import-update-with-authors.png
--rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/select-for-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    22131 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/admin_integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    32484 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_admin.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_fields.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_forms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_instance_loaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_mixins.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_tmp_storages.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_widgets.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/bulk_import.rst
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/celery.rst
--rw-r--r--   0 runner    (1001) docker     (127)    59446 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/export_workflow.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    10518 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.518338 django_import_export-4.0.3/docs/image_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/image_src/export_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/image_src/import_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/import_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    15410 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/screenshots.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 13:47:07.000000 django_import_export-4.0.3/import_export/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    35711 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/formats/base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/instance_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.494338 django_import_export-4.0.3/import_export/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.494338 django_import_export-4.0.3/import_export/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/kz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/kz/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/kz/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/kz/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    51173 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/static/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/static/import_export/export.css
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/static/import_export/export_selectable_fields.js
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/static/import_export/guess_format.js
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/static/import_export/import.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.530338 django_import_export-4.0.3/import_export/templates/admin/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/change_list_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/change_list_export_item.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/change_list_import.html
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/change_list_import_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/change_list_import_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/export.html
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/import.html
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/resource_fields_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.530338 django_import_export-4.0.3/import_export/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templatetags/import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-16 13:47:03.000000 django_import_export-4.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.530338 django_import_export-4.0.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 13:47:03.000000 django_import_export-4.0.3/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 13:47:03.000000 django_import_export-4.0.3/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-16 13:47:03.000000 django_import_export-4.0.3/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-16 13:47:03.000000 django_import_export-4.0.3/runtests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-05-16 13:47:03.000000 django_import_export-4.0.3/runtests.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:47:07.546338 django_import_export-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:47:03.000000 django_import_export-4.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.530338 django_import_export-4.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/books-sample.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.530338 django_import_export-4.0.3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.534338 django_import_export-4.0.3/tests/core/exports/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/authors.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-ISO-8859-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-dos.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-empty-author-email.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-for-delete.csv
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-invalid-date.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-mac.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-mac.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-unicode.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-unicode.tsv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books.csv
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books.json
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books.xls
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/child.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.534338 django_import_export-4.0.3/tests/core/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/fixtures/author.json
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/fixtures/book.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/fixtures/category.json
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.538338 django_import_export-4.0.3/tests/core/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0002_book_published_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0003_withfloatfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0004_bookwithchapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0005_addparentchild.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0006_auto_20171130_0147.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0007_auto_20180628_0411.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0008_auto_20190409_0846.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0009_auto_20211111_0807.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0010_uuidbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0012_delete_legacybook.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0013_alter_author_birthday.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0014_bookwithchapternumbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0015_withpositiveintegerfields.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.502338 django_import_export-4.0.3/tests/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.538338 django_import_export-4.0.3/tests/core/templates/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.538338 django_import_export-4.0.3/tests/core/templates/core/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/templates/core/admin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/templates/core/category_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.538338 django_import_export-4.0.3/tests/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.542338 django_import_export-4.0.3/tests/core/tests/admin_integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/admin_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/admin_integration/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/admin_integration/test_action_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    20354 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/admin_integration/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    40988 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/admin_integration/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/admin_integration/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_instance_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_invalidrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14997 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_model_resource_fields_generate_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.542338 django_import_export-4.0.3/tests/core/tests/test_resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_bulk_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_diffs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16292 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_import_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.546338 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_data_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    13486 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_queryset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_natural_foreign_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)    26689 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.502338 django_import_export-4.0.3/tests/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.546338 django_import_export-4.0.3/tests/docker/db/
--rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/docker/db/init-mysql-db.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/docker/db/init-postgres-db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.546338 django_import_export-4.0.3/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/scripts/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.607267 django_import_export-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.559267 django_import_export-4.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.559267 django_import_export-4.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.559267 django_import_export-4.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-23 18:32:34.000000 django_import_export-4.0.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-23 18:32:34.000000 django_import_export-4.0.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-23 18:32:34.000000 django_import_export-4.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-23 18:32:34.000000 django_import_export-4.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-23 18:32:34.000000 django_import_export-4.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-23 18:32:34.000000 django_import_export-4.0.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11616 2024-05-23 18:32:40.607267 django_import_export-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-05-23 18:32:34.000000 django_import_export-4.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-23 18:32:34.000000 django_import_export-4.0.5/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-23 18:32:34.000000 django_import_export-4.0.5/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.607267 django_import_export-4.0.5/django_import_export.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11616 2024-05-23 18:32:40.000000 django_import_export-4.0.5/django_import_export.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-23 18:32:40.000000 django_import_export-4.0.5/django_import_export.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:32:40.000000 django_import_export-4.0.5/django_import_export.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-23 18:32:40.000000 django_import_export-4.0.5/django_import_export.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 18:32:40.000000 django_import_export-4.0.5/django_import_export.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.567267 django_import_export-4.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.547267 django_import_export-4.0.5/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.571267 django_import_export-4.0.5/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/change-form-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/custom-export-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/custom-import-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/date-widget-validation-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/django-import-export-change.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/django-import-export-export-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/django-import-export-import-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/django-import-export-import.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/export-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/export_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/import-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/import_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/non-field-specific-validation-error.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.575267 django_import_export-4.0.5/docs/_static/images/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (127)   445502 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/screenshots/confirm-import.png
+-rw-r--r--   0 runner    (1001) docker     (127)   311653 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/screenshots/export-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)   469577 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/screenshots/export-selected-action.png
+-rw-r--r--   0 runner    (1001) docker     (127)   447473 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/screenshots/import-complete.png
+-rw-r--r--   0 runner    (1001) docker     (127)   308805 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/screenshots/import-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)   313540 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/screenshots/import-update-with-authors.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/_static/images/select-for-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22131 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/admin_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    32484 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/api_admin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/api_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/api_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/api_forms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/api_instance_loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/api_mixins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/api_resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/api_results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/api_tmp_storages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/api_widgets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/bulk_import.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/celery.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    60192 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/export_workflow.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10518 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.575267 django_import_export-4.0.5/docs/image_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/image_src/export_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/image_src/import_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/import_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    15691 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/screenshots.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-23 18:32:34.000000 django_import_export-4.0.5/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.575267 django_import_export-4.0.5/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 18:32:40.000000 django_import_export-4.0.5/import_export/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35711 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.579267 django_import_export-4.0.5/import_export/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/formats/base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/instance_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.547267 django_import_export-4.0.5/import_export/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.579267 django_import_export-4.0.5/import_export/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.547267 django_import_export-4.0.5/import_export/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.579267 django_import_export-4.0.5/import_export/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.547267 django_import_export-4.0.5/import_export/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.579267 django_import_export-4.0.5/import_export/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.547267 django_import_export-4.0.5/import_export/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.579267 django_import_export-4.0.5/import_export/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.547267 django_import_export-4.0.5/import_export/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.579267 django_import_export-4.0.5/import_export/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.547267 django_import_export-4.0.5/import_export/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.579267 django_import_export-4.0.5/import_export/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.547267 django_import_export-4.0.5/import_export/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.579267 django_import_export-4.0.5/import_export/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.579267 django_import_export-4.0.5/import_export/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.579267 django_import_export-4.0.5/import_export/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.579267 django_import_export-4.0.5/import_export/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.579267 django_import_export-4.0.5/import_export/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.583267 django_import_export-4.0.5/import_export/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.583267 django_import_export-4.0.5/import_export/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/kz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.583267 django_import_export-4.0.5/import_export/locale/kz/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/kz/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/kz/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.583267 django_import_export-4.0.5/import_export/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.583267 django_import_export-4.0.5/import_export/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.583267 django_import_export-4.0.5/import_export/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.583267 django_import_export-4.0.5/import_export/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.583267 django_import_export-4.0.5/import_export/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.583267 django_import_export-4.0.5/import_export/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.583267 django_import_export-4.0.5/import_export/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51180 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.587267 django_import_export-4.0.5/import_export/static/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/static/import_export/export.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/static/import_export/export_selectable_fields.js
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/static/import_export/guess_format.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/static/import_export/import.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.551267 django_import_export-4.0.5/import_export/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.587267 django_import_export-4.0.5/import_export/templates/admin/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/templates/admin/import_export/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/templates/admin/import_export/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/templates/admin/import_export/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/templates/admin/import_export/change_list_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/templates/admin/import_export/change_list_export_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/templates/admin/import_export/change_list_import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/templates/admin/import_export/change_list_import_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/templates/admin/import_export/change_list_import_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/templates/admin/import_export/export.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/templates/admin/import_export/import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/templates/admin/import_export/resource_fields_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.587267 django_import_export-4.0.5/import_export/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/templatetags/import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21074 2024-05-23 18:32:34.000000 django_import_export-4.0.5/import_export/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-23 18:32:34.000000 django_import_export-4.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.587267 django_import_export-4.0.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 18:32:34.000000 django_import_export-4.0.5/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 18:32:34.000000 django_import_export-4.0.5/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-23 18:32:34.000000 django_import_export-4.0.5/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-23 18:32:34.000000 django_import_export-4.0.5/runtests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-05-23 18:32:34.000000 django_import_export-4.0.5/runtests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:32:40.607267 django_import_export-4.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:32:34.000000 django_import_export-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.587267 django_import_export-4.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/books-sample.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.591267 django_import_export-4.0.5/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.591267 django_import_export-4.0.5/tests/core/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/authors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/books-ISO-8859-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/books-dos.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/books-empty-author-email.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/books-for-delete.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/books-invalid-date.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/books-mac.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/books-mac.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/books-no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/books-unicode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/books-unicode.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/books.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/books.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/books.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/books.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/exports/child.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.591267 django_import_export-4.0.5/tests/core/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/fixtures/author.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/fixtures/book.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/fixtures/category.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.595267 django_import_export-4.0.5/tests/core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0002_book_published_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0003_withfloatfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0004_bookwithchapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0005_addparentchild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0006_auto_20171130_0147.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0007_auto_20180628_0411.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0008_auto_20190409_0846.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0009_auto_20211111_0807.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0010_uuidbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0012_delete_legacybook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0013_alter_author_birthday.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0014_bookwithchapternumbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0015_withpositiveintegerfields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/0016_alter_category_options_alter_uuidcategory_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.555267 django_import_export-4.0.5/tests/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.595267 django_import_export-4.0.5/tests/core/templates/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.595267 django_import_export-4.0.5/tests/core/templates/core/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/templates/core/admin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/templates/core/category_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.599267 django_import_export-4.0.5/tests/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.599267 django_import_export-4.0.5/tests/core/tests/admin_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/admin_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/admin_integration/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/admin_integration/test_action_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20354 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/admin_integration/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42497 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/admin_integration/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/admin_integration/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_instance_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_invalidrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14997 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_model_resource_fields_generate_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.603267 django_import_export-4.0.5/tests/core/tests/test_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_bulk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16292 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.607267 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13486 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_natural_foreign_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_resources/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26670 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/tests/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.555267 django_import_export-4.0.5/tests/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.607267 django_import_export-4.0.5/tests/docker/db/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/docker/db/init-mysql-db.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/docker/db/init-postgres-db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:40.607267 django_import_export-4.0.5/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/scripts/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-23 18:32:34.000000 django_import_export-4.0.5/tox.ini
```

### Comparing `django_import_export-4.0.3/.github/ISSUE_TEMPLATE/bug_report.md` & `django_import_export-4.0.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/.github/ISSUE_TEMPLATE/question.md` & `django_import_export-4.0.5/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/.github/stale.yml` & `django_import_export-4.0.5/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/.github/workflows/release.yml` & `django_import_export-4.0.5/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
           python -m
           pip install
           build
           --user
       - name: Build a binary wheel and a source tarball
         run: python -m build
       - name: Store the distribution packages
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: python-package-distributions
           path: dist/
 
   publish-to-pypi:
     name: >-
       Publish Python 🐍 distribution 📦 to PyPI
@@ -42,15 +42,15 @@
     environment:
       name: pypi
       url: https://pypi.org/p/django-import-export
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Publish distribution 📦 to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
 
   publish-to-testpypi:
@@ -61,15 +61,15 @@
     environment:
       name: testpypi
       url: https://test.pypi.org/p/django-import-export
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Publish distribution 📦 to TestPyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         repository-url: https://test.pypi.org/legacy/
```

### Comparing `django_import_export-4.0.3/.github/workflows/test.yml` & `django_import_export-4.0.5/.github/workflows/test.yml`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 on:
   push:
     branches:
     - main
   pull_request:
     branches:
     - main
-    # temporary - remove after release 4
-    - release-4
 
 jobs:
   test:
     runs-on: ubuntu-latest
     env:
       DB_NAME: import_export
       IMPORT_EXPORT_POSTGRESQL_USER: postgres
```

### Comparing `django_import_export-4.0.3/AUTHORS` & `django_import_export-4.0.5/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -148,7 +148,8 @@
 * Glay00 (Gleb Gorelov)
 * PrashansaChaudhary (Prashansa Chaudhary)
 * Vedang Barhate (bvedang)
 * RobTilton (Robert Tilton)
 * ulliholtgrave
 * mishka251 (Mikhail Belov)
 * jhthompson (Jeremy Thompson)
+* thisisumurzakov (Akbarbek Umurzakov)
```

### Comparing `django_import_export-4.0.3/CODE_OF_CONDUCT.md` & `django_import_export-4.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/LICENSE` & `django_import_export-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/Makefile` & `django_import_export-4.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/PKG-INFO` & `django_import_export-4.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 4.0.3
+Version: 4.0.5
 Summary: Django application and library for importing and exporting data with included admin integration.
 Author-email: Bojan Mihelač <djangoimportexport@gmail.com>
 Maintainer-email: Matthew Hegarty <djangoimportexport@gmail.com>
 License: Copyright (c) Bojan Mihelac and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
@@ -98,59 +98,63 @@
 .. |downloads| image:: https://static.pepy.tech/personalized-badge/django-import-export?period=month&units=international_system&left_color=black&right_color=blue&left_text=Downloads/month
     :target: https://pepy.tech/project/django-import-export
 
 .. |xfollow| image:: https://img.shields.io/twitter/url/https/twitter.com/django_import.svg?style=social&label=Follow%20%40django_import
    :alt: Follow us on X
    :target: https://twitter.com/django_import
 
-.. |main_screenshot| image:: https://github.com/matthewhegarty/django-import-export/blob/doc-updates/docs/_static/images/screenshots/import-form.png
-   :width: 800
-   :alt: screenshot of the import form in django-import-export
+.. |discord|  image:: https://img.shields.io/discord/1240294048653119508?style=flat
+   :alt: Discord
 
-|build| |coveralls| |pypi| |docs| |pyver| |djangover| |downloads| |xfollow|
+|build| |coveralls| |pypi| |docs| |pyver| |djangover| |downloads| |xfollow| |discord|
 
 Introduction
 ============
 
 Straightforward, reliable and comprehensive file import / export for your Django application.
 
 *django-import-export* is an application and library which lets you manage import / export from / to a variety of sources (csv, xlsx, json etc).
 
 Can be run programmatically, or with optional integration with the Django Admin site:
 
-|main_screenshot|
+..
+  source of this video uploaded to this issue comment:
+  https://github.com/django-import-export/django-import-export/pull/1833#issuecomment-2118777440
 
-`More screenshots <https://django-import-export.readthedocs.io/en/latest/screenshots.html/>`_
+https://github.com/django-import-export/django-import-export/assets/6249838/ab56d8ba-c307-4bdf-8fa9-225669c72b37
+
+`Screenshots <https://django-import-export.readthedocs.io/en/latest/screenshots.html>`_
 
 Features
 ========
 
 * Import / export via `Admin UI Integration <https://django-import-export.readthedocs.io/en/latest/admin_integration.html>`_ or `programmatically <https://django-import-export.readthedocs.io/en/latest/getting_started.html#importing-data>`_
 * Import to and from a variety of file formats (csv, json, xlsx, pandas, HTML, YAML... and anything else that `tablib <https://github.com/jazzband/tablib>`_ supports)
 * `Preview <https://django-import-export.readthedocs.io/en/latest/screenshots.html/>`_ data before importing in Admin UI
 * Support for `bulk import <https://django-import-export.readthedocs.io/en/latest/bulk_import.html>`_
-* Handles `CRUD operations during import <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#create-or-update-model-instances>`_
+* Handles `CRUD (and 'skip') operations during import <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#create-or-update-model-instances>`_
 * Flexible handling of `foreign key <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#importing-model-relations>`_ relationships
 * `Many-to-many relationship <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#many-to-many-relations>`_ support
 * `Validation <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#validation-during-import>`_ of imported data
-* Define custom `Transformations <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#advanced-data-manipulation-on-export>`_ for exported data
+* Define custom `transformations <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#advanced-data-manipulation-on-export>`_ for exported data
 * Import / export the same model instance as `different views <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#customize-resource-options>`_
-* Export using `natural keys <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#django-natural-keys>`_ for portability between environments
+* Export using `natural keys <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#django-natural-keys>`__ for portability between environments
 * `Select items for export <https://django-import-export.readthedocs.io/en/latest/screenshots.html/>`_ via the Admin UI object list
 * `Select fields for export <https://django-import-export.readthedocs.io/en/latest/screenshots.html/>`_ via the export form
 * `Export single object instances <https://django-import-export.readthedocs.io/en/latest/admin_integration.html#export-from-model-instance-change-form>`_
 * Use `django permissions <https://django-import-export.readthedocs.io/en/latest/installation.html#import-export-import-permission-code>`_ to control import / export authorization
 * Internationalization support
-* Based on `tablib <https://github.com/jazzband/tablib>`_
+* Based on `tablib <https://github.com/jazzband/tablib>`__
 * Support for MySQL / PostgreSQL / SQLite
 * Extensible - `add custom logic to control import / export <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html>`_
 * Handle import from various character encodings
 * `Celery <https://django-import-export.readthedocs.io/en/latest/celery.html>`_ integration
 * Test locally with `Docker <https://django-import-export.readthedocs.io/en/latest/testing.html>`_
-* Comprehensive `documentation <https://django-import-export.readthedocs.io/en/latest/index.html>`_
+* Comprehensive `documentation <https://django-import-export.readthedocs.io/en/latest/index.html>`__
+* `Extensible API <https://django-import-export.readthedocs.io/en/latest/api_admin.html>`_
 * test coverage :100:
 * Supports dark mode :rocket:
 
 Example use-cases
 =================
 
 *django-import-export* is designed to be extensible and can be used to support a variety of operations.
@@ -164,26 +168,32 @@
 * Add `hooks <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#advanced-data-manipulation-on-export>`_ to anonymize data on export
 * `Modify import / export UI forms <https://django-import-export.readthedocs.io/en/latest/admin_integration.html#customize-admin-import-forms>`_ to add dynamic filtering on import / export.
 
 Getting started
 ===============
 
 * `Installation <https://django-import-export.readthedocs.io/en/latest/installation.html>`_
-* `Getting started <https://django-import-export.readthedocs.io/en/latest/getting_started.html>`_
+* `Getting started <https://django-import-export.readthedocs.io/en/latest/getting_started.html>`__
 * `Example application <https://django-import-export.readthedocs.io/en/latest/installation.html#exampleapp>`_
 
 Help and support
 ================
 
+* `Documentation <https://django-import-export.readthedocs.io/en/latest/>`_
 * `FAQ <https://django-import-export.readthedocs.io/en/latest/faq.html>`_
 * `Getting help <https://django-import-export.readthedocs.io/en/latest/faq.html#what-s-the-best-way-to-communicate-a-problem-question-or-suggestion>`_
 * `Contributing <https://django-import-export.readthedocs.io/en/latest/faq.html#how-can-i-help>`_
 * Become a `sponsor <https://github.com/sponsors/django-import-export>`_
 * `Raise a security issue <https://github.com/django-import-export/django-import-export/blob/main/SECURITY.md>`_
 * Join our `discord <https://discord.gg/aCcec52kY4>`_
 
+Commercial support
+==================
+
+Commercial support is provided by `Bellaport Systems Ltd <https://www.bellaport.co.uk>`_
+
 Releases
 ========
 
 * `Release notes <https://django-import-export.readthedocs.io/en/latest/release_notes.html>`_
 * `Changelog <https://django-import-export.readthedocs.io/en/latest/changelog.html>`_
```

### Comparing `django_import_export-4.0.3/README.rst` & `django_import_export-4.0.5/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -26,59 +26,63 @@
 .. |downloads| image:: https://static.pepy.tech/personalized-badge/django-import-export?period=month&units=international_system&left_color=black&right_color=blue&left_text=Downloads/month
     :target: https://pepy.tech/project/django-import-export
 
 .. |xfollow| image:: https://img.shields.io/twitter/url/https/twitter.com/django_import.svg?style=social&label=Follow%20%40django_import
    :alt: Follow us on X
    :target: https://twitter.com/django_import
 
-.. |main_screenshot| image:: https://github.com/matthewhegarty/django-import-export/blob/doc-updates/docs/_static/images/screenshots/import-form.png
-   :width: 800
-   :alt: screenshot of the import form in django-import-export
+.. |discord|  image:: https://img.shields.io/discord/1240294048653119508?style=flat
+   :alt: Discord
 
-|build| |coveralls| |pypi| |docs| |pyver| |djangover| |downloads| |xfollow|
+|build| |coveralls| |pypi| |docs| |pyver| |djangover| |downloads| |xfollow| |discord|
 
 Introduction
 ============
 
 Straightforward, reliable and comprehensive file import / export for your Django application.
 
 *django-import-export* is an application and library which lets you manage import / export from / to a variety of sources (csv, xlsx, json etc).
 
 Can be run programmatically, or with optional integration with the Django Admin site:
 
-|main_screenshot|
+..
+  source of this video uploaded to this issue comment:
+  https://github.com/django-import-export/django-import-export/pull/1833#issuecomment-2118777440
 
-`More screenshots <https://django-import-export.readthedocs.io/en/latest/screenshots.html/>`_
+https://github.com/django-import-export/django-import-export/assets/6249838/ab56d8ba-c307-4bdf-8fa9-225669c72b37
+
+`Screenshots <https://django-import-export.readthedocs.io/en/latest/screenshots.html>`_
 
 Features
 ========
 
 * Import / export via `Admin UI Integration <https://django-import-export.readthedocs.io/en/latest/admin_integration.html>`_ or `programmatically <https://django-import-export.readthedocs.io/en/latest/getting_started.html#importing-data>`_
 * Import to and from a variety of file formats (csv, json, xlsx, pandas, HTML, YAML... and anything else that `tablib <https://github.com/jazzband/tablib>`_ supports)
 * `Preview <https://django-import-export.readthedocs.io/en/latest/screenshots.html/>`_ data before importing in Admin UI
 * Support for `bulk import <https://django-import-export.readthedocs.io/en/latest/bulk_import.html>`_
-* Handles `CRUD operations during import <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#create-or-update-model-instances>`_
+* Handles `CRUD (and 'skip') operations during import <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#create-or-update-model-instances>`_
 * Flexible handling of `foreign key <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#importing-model-relations>`_ relationships
 * `Many-to-many relationship <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#many-to-many-relations>`_ support
 * `Validation <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#validation-during-import>`_ of imported data
-* Define custom `Transformations <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#advanced-data-manipulation-on-export>`_ for exported data
+* Define custom `transformations <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#advanced-data-manipulation-on-export>`_ for exported data
 * Import / export the same model instance as `different views <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#customize-resource-options>`_
-* Export using `natural keys <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#django-natural-keys>`_ for portability between environments
+* Export using `natural keys <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#django-natural-keys>`__ for portability between environments
 * `Select items for export <https://django-import-export.readthedocs.io/en/latest/screenshots.html/>`_ via the Admin UI object list
 * `Select fields for export <https://django-import-export.readthedocs.io/en/latest/screenshots.html/>`_ via the export form
 * `Export single object instances <https://django-import-export.readthedocs.io/en/latest/admin_integration.html#export-from-model-instance-change-form>`_
 * Use `django permissions <https://django-import-export.readthedocs.io/en/latest/installation.html#import-export-import-permission-code>`_ to control import / export authorization
 * Internationalization support
-* Based on `tablib <https://github.com/jazzband/tablib>`_
+* Based on `tablib <https://github.com/jazzband/tablib>`__
 * Support for MySQL / PostgreSQL / SQLite
 * Extensible - `add custom logic to control import / export <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html>`_
 * Handle import from various character encodings
 * `Celery <https://django-import-export.readthedocs.io/en/latest/celery.html>`_ integration
 * Test locally with `Docker <https://django-import-export.readthedocs.io/en/latest/testing.html>`_
-* Comprehensive `documentation <https://django-import-export.readthedocs.io/en/latest/index.html>`_
+* Comprehensive `documentation <https://django-import-export.readthedocs.io/en/latest/index.html>`__
+* `Extensible API <https://django-import-export.readthedocs.io/en/latest/api_admin.html>`_
 * test coverage :100:
 * Supports dark mode :rocket:
 
 Example use-cases
 =================
 
 *django-import-export* is designed to be extensible and can be used to support a variety of operations.
@@ -92,26 +96,32 @@
 * Add `hooks <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#advanced-data-manipulation-on-export>`_ to anonymize data on export
 * `Modify import / export UI forms <https://django-import-export.readthedocs.io/en/latest/admin_integration.html#customize-admin-import-forms>`_ to add dynamic filtering on import / export.
 
 Getting started
 ===============
 
 * `Installation <https://django-import-export.readthedocs.io/en/latest/installation.html>`_
-* `Getting started <https://django-import-export.readthedocs.io/en/latest/getting_started.html>`_
+* `Getting started <https://django-import-export.readthedocs.io/en/latest/getting_started.html>`__
 * `Example application <https://django-import-export.readthedocs.io/en/latest/installation.html#exampleapp>`_
 
 Help and support
 ================
 
+* `Documentation <https://django-import-export.readthedocs.io/en/latest/>`_
 * `FAQ <https://django-import-export.readthedocs.io/en/latest/faq.html>`_
 * `Getting help <https://django-import-export.readthedocs.io/en/latest/faq.html#what-s-the-best-way-to-communicate-a-problem-question-or-suggestion>`_
 * `Contributing <https://django-import-export.readthedocs.io/en/latest/faq.html#how-can-i-help>`_
 * Become a `sponsor <https://github.com/sponsors/django-import-export>`_
 * `Raise a security issue <https://github.com/django-import-export/django-import-export/blob/main/SECURITY.md>`_
 * Join our `discord <https://discord.gg/aCcec52kY4>`_
 
+Commercial support
+==================
+
+Commercial support is provided by `Bellaport Systems Ltd <https://www.bellaport.co.uk>`_
+
 Releases
 ========
 
 * `Release notes <https://django-import-export.readthedocs.io/en/latest/release_notes.html>`_
 * `Changelog <https://django-import-export.readthedocs.io/en/latest/changelog.html>`_
```

### Comparing `django_import_export-4.0.3/RELEASE.md` & `django_import_export-4.0.5/RELEASE.md`

 * *Files 18% similar despite different names*

```diff
@@ -27,7 +27,23 @@
 
 This is implemented using a Webhook defined in the Github repo (Settings / Webhooks).
 
 readthedocs should be checked after each release to ensure that the docs have built correctly.
 Login to [readthedocs.org](https://readthedocs.org) to check that the build ran OK (click on 'Builds' tab).
 
 For pre-releases, the release version has to be activated via the readthedocs UI before it can be built.
+
+### Troubleshooting
+
+The build can fail on 'publish to PyPI' with errors such as:
+
+```
+`long_description` has syntax errors in markup and would not be rendered on PyPI.
+```
+
+This is because the README.rst contains syntax errors and cannot be rendered.  You can check this with:
+
+```
+pip install readme_renderer
+python setup.py check -r -s
+```
+If there are duplicate target names, you can correct this with [underscores](https://github.com/sphinx-doc/sphinx/issues/3921#issuecomment-315581557).
```

### Comparing `django_import_export-4.0.3/django_import_export.egg-info/PKG-INFO` & `django_import_export-4.0.5/django_import_export.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 4.0.3
+Version: 4.0.5
 Summary: Django application and library for importing and exporting data with included admin integration.
 Author-email: Bojan Mihelač <djangoimportexport@gmail.com>
 Maintainer-email: Matthew Hegarty <djangoimportexport@gmail.com>
 License: Copyright (c) Bojan Mihelac and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
@@ -98,59 +98,63 @@
 .. |downloads| image:: https://static.pepy.tech/personalized-badge/django-import-export?period=month&units=international_system&left_color=black&right_color=blue&left_text=Downloads/month
     :target: https://pepy.tech/project/django-import-export
 
 .. |xfollow| image:: https://img.shields.io/twitter/url/https/twitter.com/django_import.svg?style=social&label=Follow%20%40django_import
    :alt: Follow us on X
    :target: https://twitter.com/django_import
 
-.. |main_screenshot| image:: https://github.com/matthewhegarty/django-import-export/blob/doc-updates/docs/_static/images/screenshots/import-form.png
-   :width: 800
-   :alt: screenshot of the import form in django-import-export
+.. |discord|  image:: https://img.shields.io/discord/1240294048653119508?style=flat
+   :alt: Discord
 
-|build| |coveralls| |pypi| |docs| |pyver| |djangover| |downloads| |xfollow|
+|build| |coveralls| |pypi| |docs| |pyver| |djangover| |downloads| |xfollow| |discord|
 
 Introduction
 ============
 
 Straightforward, reliable and comprehensive file import / export for your Django application.
 
 *django-import-export* is an application and library which lets you manage import / export from / to a variety of sources (csv, xlsx, json etc).
 
 Can be run programmatically, or with optional integration with the Django Admin site:
 
-|main_screenshot|
+..
+  source of this video uploaded to this issue comment:
+  https://github.com/django-import-export/django-import-export/pull/1833#issuecomment-2118777440
 
-`More screenshots <https://django-import-export.readthedocs.io/en/latest/screenshots.html/>`_
+https://github.com/django-import-export/django-import-export/assets/6249838/ab56d8ba-c307-4bdf-8fa9-225669c72b37
+
+`Screenshots <https://django-import-export.readthedocs.io/en/latest/screenshots.html>`_
 
 Features
 ========
 
 * Import / export via `Admin UI Integration <https://django-import-export.readthedocs.io/en/latest/admin_integration.html>`_ or `programmatically <https://django-import-export.readthedocs.io/en/latest/getting_started.html#importing-data>`_
 * Import to and from a variety of file formats (csv, json, xlsx, pandas, HTML, YAML... and anything else that `tablib <https://github.com/jazzband/tablib>`_ supports)
 * `Preview <https://django-import-export.readthedocs.io/en/latest/screenshots.html/>`_ data before importing in Admin UI
 * Support for `bulk import <https://django-import-export.readthedocs.io/en/latest/bulk_import.html>`_
-* Handles `CRUD operations during import <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#create-or-update-model-instances>`_
+* Handles `CRUD (and 'skip') operations during import <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#create-or-update-model-instances>`_
 * Flexible handling of `foreign key <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#importing-model-relations>`_ relationships
 * `Many-to-many relationship <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#many-to-many-relations>`_ support
 * `Validation <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#validation-during-import>`_ of imported data
-* Define custom `Transformations <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#advanced-data-manipulation-on-export>`_ for exported data
+* Define custom `transformations <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#advanced-data-manipulation-on-export>`_ for exported data
 * Import / export the same model instance as `different views <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#customize-resource-options>`_
-* Export using `natural keys <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#django-natural-keys>`_ for portability between environments
+* Export using `natural keys <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#django-natural-keys>`__ for portability between environments
 * `Select items for export <https://django-import-export.readthedocs.io/en/latest/screenshots.html/>`_ via the Admin UI object list
 * `Select fields for export <https://django-import-export.readthedocs.io/en/latest/screenshots.html/>`_ via the export form
 * `Export single object instances <https://django-import-export.readthedocs.io/en/latest/admin_integration.html#export-from-model-instance-change-form>`_
 * Use `django permissions <https://django-import-export.readthedocs.io/en/latest/installation.html#import-export-import-permission-code>`_ to control import / export authorization
 * Internationalization support
-* Based on `tablib <https://github.com/jazzband/tablib>`_
+* Based on `tablib <https://github.com/jazzband/tablib>`__
 * Support for MySQL / PostgreSQL / SQLite
 * Extensible - `add custom logic to control import / export <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html>`_
 * Handle import from various character encodings
 * `Celery <https://django-import-export.readthedocs.io/en/latest/celery.html>`_ integration
 * Test locally with `Docker <https://django-import-export.readthedocs.io/en/latest/testing.html>`_
-* Comprehensive `documentation <https://django-import-export.readthedocs.io/en/latest/index.html>`_
+* Comprehensive `documentation <https://django-import-export.readthedocs.io/en/latest/index.html>`__
+* `Extensible API <https://django-import-export.readthedocs.io/en/latest/api_admin.html>`_
 * test coverage :100:
 * Supports dark mode :rocket:
 
 Example use-cases
 =================
 
 *django-import-export* is designed to be extensible and can be used to support a variety of operations.
@@ -164,26 +168,32 @@
 * Add `hooks <https://django-import-export.readthedocs.io/en/latest/advanced_usage.html#advanced-data-manipulation-on-export>`_ to anonymize data on export
 * `Modify import / export UI forms <https://django-import-export.readthedocs.io/en/latest/admin_integration.html#customize-admin-import-forms>`_ to add dynamic filtering on import / export.
 
 Getting started
 ===============
 
 * `Installation <https://django-import-export.readthedocs.io/en/latest/installation.html>`_
-* `Getting started <https://django-import-export.readthedocs.io/en/latest/getting_started.html>`_
+* `Getting started <https://django-import-export.readthedocs.io/en/latest/getting_started.html>`__
 * `Example application <https://django-import-export.readthedocs.io/en/latest/installation.html#exampleapp>`_
 
 Help and support
 ================
 
+* `Documentation <https://django-import-export.readthedocs.io/en/latest/>`_
 * `FAQ <https://django-import-export.readthedocs.io/en/latest/faq.html>`_
 * `Getting help <https://django-import-export.readthedocs.io/en/latest/faq.html#what-s-the-best-way-to-communicate-a-problem-question-or-suggestion>`_
 * `Contributing <https://django-import-export.readthedocs.io/en/latest/faq.html#how-can-i-help>`_
 * Become a `sponsor <https://github.com/sponsors/django-import-export>`_
 * `Raise a security issue <https://github.com/django-import-export/django-import-export/blob/main/SECURITY.md>`_
 * Join our `discord <https://discord.gg/aCcec52kY4>`_
 
+Commercial support
+==================
+
+Commercial support is provided by `Bellaport Systems Ltd <https://www.bellaport.co.uk>`_
+
 Releases
 ========
 
 * `Release notes <https://django-import-export.readthedocs.io/en/latest/release_notes.html>`_
 * `Changelog <https://django-import-export.readthedocs.io/en/latest/changelog.html>`_
```

### Comparing `django_import_export-4.0.3/django_import_export.egg-info/SOURCES.txt` & `django_import_export-4.0.5/django_import_export.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,15 @@
 tests/core/migrations/0009_auto_20211111_0807.py
 tests/core/migrations/0010_uuidbook.py
 tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
 tests/core/migrations/0012_delete_legacybook.py
 tests/core/migrations/0013_alter_author_birthday.py
 tests/core/migrations/0014_bookwithchapternumbers.py
 tests/core/migrations/0015_withpositiveintegerfields.py
+tests/core/migrations/0016_alter_category_options_alter_uuidcategory_options.py
 tests/core/migrations/__init__.py
 tests/core/templates/core/category_list.html
 tests/core/templates/core/admin/change_list.html
 tests/core/tests/__init__.py
 tests/core/tests/resources.py
 tests/core/tests/test_base_formats.py
 tests/core/tests/test_declarative.py
```

### Comparing `django_import_export-4.0.3/docs/Makefile` & `django_import_export-4.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/change-form-export.png` & `django_import_export-4.0.5/docs/_static/images/change-form-export.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/custom-export-form.png` & `django_import_export-4.0.5/docs/_static/images/custom-export-form.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/custom-import-form.png` & `django_import_export-4.0.5/docs/_static/images/custom-import-form.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/date-widget-validation-error.png` & `django_import_export-4.0.5/docs/_static/images/date-widget-validation-error.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/django-import-export-change.png` & `django_import_export-4.0.5/docs/_static/images/django-import-export-change.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/django-import-export-export-confirm.png` & `django_import_export-4.0.5/docs/_static/images/django-import-export-export-confirm.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/django-import-export-import-confirm.png` & `django_import_export-4.0.5/docs/_static/images/django-import-export-import-confirm.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/django-import-export-import.png` & `django_import_export-4.0.5/docs/_static/images/django-import-export-import.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/export-button.png` & `django_import_export-4.0.5/docs/_static/images/export-button.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/export_workflow.svg` & `django_import_export-4.0.5/docs/_static/images/export_workflow.svg`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/import-button.png` & `django_import_export-4.0.5/docs/_static/images/import-button.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/import_workflow.svg` & `django_import_export-4.0.5/docs/_static/images/import_workflow.svg`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/non-field-specific-validation-error.png` & `django_import_export-4.0.5/docs/_static/images/non-field-specific-validation-error.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/screenshots/confirm-import.png` & `django_import_export-4.0.5/docs/_static/images/screenshots/confirm-import.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/screenshots/export-form.png` & `django_import_export-4.0.5/docs/_static/images/screenshots/export-form.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/screenshots/export-selected-action.png` & `django_import_export-4.0.5/docs/_static/images/screenshots/export-selected-action.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/screenshots/import-complete.png` & `django_import_export-4.0.5/docs/_static/images/screenshots/import-complete.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/screenshots/import-form.png` & `django_import_export-4.0.5/docs/_static/images/screenshots/import-form.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/screenshots/import-update-with-authors.png` & `django_import_export-4.0.5/docs/_static/images/screenshots/import-update-with-authors.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/_static/images/select-for-export.png` & `django_import_export-4.0.5/docs/_static/images/select-for-export.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/admin_integration.rst` & `django_import_export-4.0.5/docs/admin_integration.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/advanced_usage.rst` & `django_import_export-4.0.5/docs/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/api_mixins.rst` & `django_import_export-4.0.5/docs/api_mixins.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/api_widgets.rst` & `django_import_export-4.0.5/docs/api_widgets.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/bulk_import.rst` & `django_import_export-4.0.5/docs/bulk_import.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/changelog.rst` & `django_import_export-4.0.5/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 Changelog
 =========
 
 .. warning::
 
     Version 4 introduces breaking changes.  Please refer to :doc:`release notes<release_notes>`.
 
+4.0.5 (2024-05-23)
+------------------
+
+- Fix for invalid build due to malformed README.rst (`1851 <https://github.com/django-import-export/django-import-export/pull/1851>`_)
+
+4.0.4 (2024-05-23)
+------------------
+
+- Refactored ``DateWidget`` & ``DateTimeWidget`` to remove code duplication (`1839 <https://github.com/django-import-export/django-import-export/pull/1839>`_)
+- Release note documentation updated (`1840 <https://github.com/django-import-export/django-import-export/pull/1840>`_)
+- Added missing migration to example app (`1843 <https://github.com/django-import-export/django-import-export/pull/1843>`_)
+- Fix admin UI display of field import order (`1849 <https://github.com/django-import-export/django-import-export/pull/1849>`_)
+
 4.0.3 (2024-05-16)
 ------------------
 
 - Support widgets with CSS and JS media in ImportForm (`1807 <https://github.com/django-import-export/django-import-export/pull/1807>`_)
 - Documentation updates (`1833 <https://github.com/django-import-export/django-import-export/pull/1833>`_)
 - Clarified documentation when importing with ``import_id_fields``  (`1836 <https://github.com/django-import-export/django-import-export/pull/1836>`_)
 - re-add ``resource_class`` deprecation warning (`1837 <https://github.com/django-import-export/django-import-export/pull/1837>`_)
```

### Comparing `django_import_export-4.0.3/docs/conf.py` & `django_import_export-4.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/contributing.rst` & `django_import_export-4.0.5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/export_workflow.rst` & `django_import_export-4.0.5/docs/export_workflow.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/faq.rst` & `django_import_export-4.0.5/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/getting_started.rst` & `django_import_export-4.0.5/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/image_src/export_workflow.txt` & `django_import_export-4.0.5/docs/image_src/export_workflow.txt`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/image_src/import_workflow.txt` & `django_import_export-4.0.5/docs/image_src/import_workflow.txt`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/import_workflow.rst` & `django_import_export-4.0.5/docs/import_workflow.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/index.rst` & `django_import_export-4.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/installation.rst` & `django_import_export-4.0.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/make.bat` & `django_import_export-4.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/release_notes.rst` & `django_import_export-4.0.5/docs/release_notes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,22 @@
   model instance.
   The call to :meth:`~import_export.widgets.Widget.render` from :meth:`~import_export.fields.Field.export` has been removed.
 
 * Use of ``ExportViewFormMixin`` is deprecated.  See `this issue <https://github.com/django-import-export/django-import-export/issues/1666>`_.
 
 * See :ref:`renamed_methods`.
 
+* In the Admin UI, the declaration of ``resource_class`` is replaced by ``resource_classes``::
+
+      class BookAdmin(ImportExportModelAdmin):
+        # remove this line
+        # resource_class = BookResource
+        # replace with this
+        resource_classes = [BookResource]
+
 Admin UI
 ========
 
 LogEntry
 --------
 
 ``LogEntry`` instances are created during import for creates, updates and deletes.
```

### Comparing `django_import_export-4.0.3/docs/screenshots.rst` & `django_import_export-4.0.5/docs/screenshots.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/docs/testing.rst` & `django_import_export-4.0.5/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/admin.py` & `django_import_export-4.0.5/import_export/admin.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/declarative.py` & `django_import_export-4.0.5/import_export/declarative.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/exceptions.py` & `django_import_export-4.0.5/import_export/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/fields.py` & `django_import_export-4.0.5/import_export/fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/formats/base_formats.py` & `django_import_export-4.0.5/import_export/formats/base_formats.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/forms.py` & `django_import_export-4.0.5/import_export/forms.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/instance_loaders.py` & `django_import_export-4.0.5/import_export/instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/ar/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/ar/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/bg/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/bg/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/ca/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/ca/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/cs/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/cs/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/de/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/de/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/es/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/es/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/es_AR/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/es_AR/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/fa/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/fa/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/fi/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/fi/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/fr/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/fr/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/it/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/it/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/ja/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/ja/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/ko/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/ko/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/kz/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/kz/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/kz/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/kz/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/nl/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/nl/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/pl/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/pl/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/pt_BR/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/pt_BR/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/ru/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/ru/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/sk/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/sk/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/tr/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/tr/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_import_export-4.0.5/import_export/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/locale/zh_Hans/LC_MESSAGES/django.po` & `django_import_export-4.0.5/import_export/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/mixins.py` & `django_import_export-4.0.5/import_export/mixins.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/options.py` & `django_import_export-4.0.5/import_export/options.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/resources.py` & `django_import_export-4.0.5/import_export/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1081,15 +1081,15 @@
                 for f in export_fields
                 if f.attribute in fields or f.column_name in fields
             ]
 
         return [force_str(field.column_name) for field in export_fields]
 
     def get_user_visible_fields(self):
-        return self.get_fields()
+        return self.get_import_fields()
 
     def iter_queryset(self, queryset):
         if not isinstance(queryset, QuerySet):
             yield from queryset
         elif queryset._prefetch_related_lookups:
             # Django's queryset.iterator ignores prefetch_related which might result
             # in an excessive amount of db calls. Therefore we use pagination
```

### Comparing `django_import_export-4.0.3/import_export/results.py` & `django_import_export-4.0.5/import_export/results.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/static/import_export/export_selectable_fields.js` & `django_import_export-4.0.5/import_export/static/import_export/export_selectable_fields.js`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/static/import_export/guess_format.js` & `django_import_export-4.0.5/import_export/static/import_export/guess_format.js`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/static/import_export/import.css` & `django_import_export-4.0.5/import_export/static/import_export/import.css`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/templates/admin/import_export/base.html` & `django_import_export-4.0.5/import_export/templates/admin/import_export/base.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/templates/admin/import_export/export.html` & `django_import_export-4.0.5/import_export/templates/admin/import_export/export.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/templates/admin/import_export/import.html` & `django_import_export-4.0.5/import_export/templates/admin/import_export/import.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/templates/admin/import_export/resource_fields_list.html` & `django_import_export-4.0.5/import_export/templates/admin/import_export/resource_fields_list.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/tmp_storages.py` & `django_import_export-4.0.5/import_export/tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/utils.py` & `django_import_export-4.0.5/import_export/utils.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/import_export/widgets.py` & `django_import_export-4.0.5/import_export/widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,48 @@
 def format_datetime(value, datetime_format):
     # handle correct formatting of dates
     # see https://code.djangoproject.com/ticket/32738
     format_ = django.utils.formats.sanitize_strftime_format(datetime_format)
     return value.strftime(format_)
 
 
+class _ParseDateTimeMixin(object):
+    """Internal Mixin for shared logic with date and datetime conversions."""
+
+    def __init__(
+        self,
+        format=None,
+        input_formats=None,
+        default_format="%Y-%m-%d",
+        coerce_to_string=True,
+    ):
+        super().__init__(coerce_to_string=coerce_to_string)
+        self.formats = (format,) if format else (input_formats or (default_format,))
+
+    def _parse_value(self, value, value_type):
+        """Attempt to parse the value using the provided formats.
+        Raise ValueError if parsing fails."""
+        if not value:
+            return None
+        if isinstance(value, value_type):
+            return value
+
+        for format_ in self.formats:
+            try:
+                parsed_date = datetime.strptime(value, format_)
+                if value_type is date:
+                    return parsed_date.date()
+                if value_type is time:
+                    return parsed_date.time()
+                return parsed_date
+            except (ValueError, TypeError) as e:
+                logger.debug(str(e))
+        raise ValueError("Value could not be parsed using defined formats.")
+
+
 class Widget:
     """
     A Widget handles converting between import and export representations.
     """
 
     def __init__(self, coerce_to_string=True):
         """
@@ -209,144 +243,101 @@
         if self.coerce_to_string is False:
             return value
         if value in self.NULL_VALUES or not type(value) is bool:
             return ""
         return self.TRUE_VALUES[0] if value else self.FALSE_VALUES[0]
 
 
-class DateWidget(Widget):
+class DateWidget(_ParseDateTimeMixin, Widget):
     """
-    Widget for converting date fields.
+    Widget for converting date fields to Python date instances.
 
     Takes optional ``format`` parameter. If none is set, either
     ``settings.DATE_INPUT_FORMATS`` or ``"%Y-%m-%d"`` is used.
     """
 
     def __init__(self, format=None, coerce_to_string=True):
-        super().__init__(coerce_to_string=coerce_to_string)
-        if format is None:
-            if not settings.DATE_INPUT_FORMATS:
-                formats = ("%Y-%m-%d",)
-            else:
-                formats = settings.DATE_INPUT_FORMATS
-        else:
-            formats = (format,)
-        self.formats = formats
+        super().__init__(
+            format, settings.DATE_INPUT_FORMATS, "%Y-%m-%d", coerce_to_string
+        )
 
     def clean(self, value, row=None, **kwargs):
         """
         :returns: A python date instance.
         :raises: ValueError if the value cannot be parsed using defined formats.
         """
-        if not value:
-            return None
-        if isinstance(value, date):
-            return value
-        for format in self.formats:
-            try:
-                return datetime.strptime(value, format).date()
-            except (ValueError, TypeError) as e:
-                logger.debug(str(e))
-        raise ValueError(_("Value could not be parsed using defined date formats."))
+        return self._parse_value(value, date)
 
     def render(self, value, obj=None):
         self._obj_deprecation_warning(obj)
         if self.coerce_to_string is False:
             return value
         if not value or not type(value) is date:
             return ""
         return format_datetime(value, self.formats[0])
 
 
-class DateTimeWidget(Widget):
+class DateTimeWidget(_ParseDateTimeMixin, Widget):
     """
-    Widget for converting date fields.
+    Widget for converting datetime fields to Python datetime instances.
 
     Takes optional ``format`` parameter. If none is set, either
     ``settings.DATETIME_INPUT_FORMATS`` or ``"%Y-%m-%d %H:%M:%S"`` is used.
     """
 
     def __init__(self, format=None, coerce_to_string=True):
-        super().__init__(coerce_to_string=coerce_to_string)
-        if format is None:
-            if not settings.DATETIME_INPUT_FORMATS:
-                formats = ("%Y-%m-%d %H:%M:%S",)
-            else:
-                formats = settings.DATETIME_INPUT_FORMATS
-        else:
-            formats = (format,)
-        self.formats = formats
+        super().__init__(
+            format,
+            settings.DATETIME_INPUT_FORMATS,
+            "%Y-%m-%d %H:%M:%S",
+            coerce_to_string,
+        )
 
     def clean(self, value, row=None, **kwargs):
         """
         :returns: A python datetime instance.
         :raises: ValueError if the value cannot be parsed using defined formats.
         """
-        dt = None
-        if not value:
+        dt = self._parse_value(value, datetime)
+        if dt is None:
             return None
-        if isinstance(value, datetime):
-            dt = value
-        else:
-            for format_ in self.formats:
-                try:
-                    dt = datetime.strptime(value, format_)
-                except (ValueError, TypeError) as e:
-                    logger.debug(str(e))
-        if dt:
-            if settings.USE_TZ and timezone.is_naive(dt):
-                dt = timezone.make_aware(dt)
-            return dt
-        raise ValueError(_("Value could not be parsed using defined datetime formats."))
+        if settings.USE_TZ and timezone.is_naive(dt):
+            return timezone.make_aware(dt)
+        return dt
 
     def render(self, value, obj=None):
         self._obj_deprecation_warning(obj)
         if self.coerce_to_string is False:
             return value
         if not value or not type(value) is datetime:
             return ""
         if settings.USE_TZ:
             value = timezone.localtime(value)
         return format_datetime(value, self.formats[0])
 
 
-class TimeWidget(Widget):
+class TimeWidget(_ParseDateTimeMixin, Widget):
     """
     Widget for converting time fields.
 
     Takes optional ``format`` parameter. If none is set, either
     ``settings.DATETIME_INPUT_FORMATS`` or ``"%H:%M:%S"`` is used.
     """
 
     def __init__(self, format=None, coerce_to_string=True):
-        super().__init__(coerce_to_string=coerce_to_string)
-        if format is None:
-            if not settings.TIME_INPUT_FORMATS:
-                formats = ("%H:%M:%S",)
-            else:
-                formats = settings.TIME_INPUT_FORMATS
-        else:
-            formats = (format,)
-        self.formats = formats
+        super().__init__(
+            format, settings.TIME_INPUT_FORMATS, "%H:%M:%S", coerce_to_string
+        )
 
     def clean(self, value, row=None, **kwargs):
         """
         :returns: A python time instance.
         :raises: ValueError if the value cannot be parsed using defined formats.
         """
-        if not value:
-            return None
-        if isinstance(value, time):
-            return value
-        for format in self.formats:
-            try:
-                return datetime.strptime(value, format).time()
-            except (ValueError, TypeError) as e:
-                logger.debug(str(e))
-        raise ValueError(_("Value could not be parsed using defined time formats."))
+        return self._parse_value(value, time)
 
     def render(self, value, obj=None):
         self._obj_deprecation_warning(obj)
         if self.coerce_to_string is False:
             return value
         if not value or not type(value) is time:
             return ""
```

### Comparing `django_import_export-4.0.3/pyproject.toml` & `django_import_export-4.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 maintainers = [
     {name = "Matthew Hegarty", email = "djangoimportexport@gmail.com"},
 ]
 description = "Django application and library for importing and exporting data with included admin integration."
 keywords = ["django", "import", "export"]
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
-dynamic = ["version", "readme"]
+readme = "README.rst"
+dynamic = ["version"]
 classifiers = [
     "Framework :: Django",
     "Framework :: Django :: 4.2",
     "Framework :: Django :: 5.0",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
@@ -56,16 +57,13 @@
 Repository = "https://github.com/django-import-export/django-import-export"
 Changelog = "https://github.com/django-import-export/django-import-export/blob/main/docs/changelog.rst"
 
 [tool.setuptools]
 platforms = ["OS Independent"]
 license-files = ["LICENSE", "AUTHORS"]
 
-[tool.setuptools.dynamic]
-readme = {file = ["README.rst"]}
-
 [tool.setuptools_scm]
 write_to = "import_export/_version.py"
 local_scheme = "no-local-version"
 
 [tool.isort]
 profile = "black"
```

### Comparing `django_import_export-4.0.3/runtests.py` & `django_import_export-4.0.5/runtests.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/runtests.sh` & `django_import_export-4.0.5/runtests.sh`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/admin.py` & `django_import_export-4.0.5/tests/core/admin.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/exports/books-empty-author-email.xlsx` & `django_import_export-4.0.5/tests/core/exports/books-empty-author-email.xlsx`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/exports/books.json` & `django_import_export-4.0.5/tests/core/exports/books.json`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/exports/books.xls` & `django_import_export-4.0.5/tests/core/exports/books.xls`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/exports/books.xlsx` & `django_import_export-4.0.5/tests/core/exports/books.xlsx`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/fixtures/book.json` & `django_import_export-4.0.5/tests/core/fixtures/book.json`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/forms.py` & `django_import_export-4.0.5/tests/core/forms.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/migrations/0001_initial.py` & `django_import_export-4.0.5/tests/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/migrations/0003_withfloatfield.py` & `django_import_export-4.0.5/tests/core/migrations/0003_withfloatfield.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/migrations/0004_bookwithchapters.py` & `django_import_export-4.0.5/tests/core/migrations/0004_bookwithchapters.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/migrations/0005_addparentchild.py` & `django_import_export-4.0.5/tests/core/migrations/0005_addparentchild.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/migrations/0007_auto_20180628_0411.py` & `django_import_export-4.0.5/tests/core/migrations/0007_auto_20180628_0411.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/migrations/0008_auto_20190409_0846.py` & `django_import_export-4.0.5/tests/core/migrations/0008_auto_20190409_0846.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/migrations/0009_auto_20211111_0807.py` & `django_import_export-4.0.5/tests/core/migrations/0009_auto_20211111_0807.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/migrations/0010_uuidbook.py` & `django_import_export-4.0.5/tests/core/migrations/0010_uuidbook.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py` & `django_import_export-4.0.5/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/migrations/0014_bookwithchapternumbers.py` & `django_import_export-4.0.5/tests/core/migrations/0014_bookwithchapternumbers.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/migrations/0015_withpositiveintegerfields.py` & `django_import_export-4.0.5/tests/core/migrations/0015_withpositiveintegerfields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/models.py` & `django_import_export-4.0.5/tests/core/models.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/admin_integration/mixins.py` & `django_import_export-4.0.5/tests/core/tests/admin_integration/mixins.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/admin_integration/test_action_export.py` & `django_import_export-4.0.5/tests/core/tests/admin_integration/test_action_export.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/admin_integration/test_export.py` & `django_import_export-4.0.5/tests/core/tests/admin_integration/test_export.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/admin_integration/test_import.py` & `django_import_export-4.0.5/tests/core/tests/admin_integration/test_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -829,15 +829,15 @@
         response = self._do_import_post(
             self.book_import_url, "books-invalid-date.csv", index
         )
         result = response.context["result"]
         # there should be a single invalid row
         self.assertEqual(1, len(result.invalid_rows))
         self.assertEqual(
-            "Value could not be parsed using defined date formats.",
+            "Value could not be parsed using defined formats.",
             result.invalid_rows[0].error.messages[0],
         )
         # no rows should be imported because we rollback on validation errors
         self.assertEqual(0, Book.objects.count())
 
     def test_import_action_error_on_save(self):
         with mock.patch("core.models.Book.save") as mock_save:
@@ -1003,7 +1003,49 @@
             r'<td><ins style="background:#e6ffe6;">1</ins></td>[\\n\s]+'
             r'<td><ins style="background:#e6ffe6;">test@example.com</ins></td>[\\n\s]+'
             r'<td><ins style="background:#e6ffe6;">Some book</ins></td>[\\n\s]+'
             r"<td><span>None</span></td>[\\n\s]+"
             "</tr>"
         )
         self.assertRegex(str(response.content), target_row_re)
+
+
+class DefaultFieldsImportOrderTest(AdminTestMixin, TestCase):
+    """
+    Display correct import order based on default 'fields' declaration (issue 1845).
+    Ensure that the prompt text on the import page renders the
+    fields in the correct order.
+    """
+
+    def test_import_preview_order(self):
+        response = self.client.get(self.ebook_import_url)
+        # test display rendered in correct order
+        target_re = (
+            r"This importer will import the following fields:[\\n\s]+"
+            r"<code>id, author_email, name, published_date</code>[\\n\s]+"
+        )
+        self.assertRegex(str(response.content), target_re)
+
+
+class DeclaredImportOrderTest(AdminTestMixin, TestCase):
+    """
+    Display correct import order when 'import_order' is declared (issue 1845).
+    Ensure that the prompt text on the import page renders the
+    fields in the correct order.
+    """
+
+    def setUp(self):
+        super().setUp()
+        EBookResource._meta.import_order = ("id", "name", "published", "author_email")
+
+    def tearDown(self):
+        super().tearDown()
+        EBookResource._meta.import_order = ()
+
+    def test_import_preview_order(self):
+        response = self.client.get(self.ebook_import_url)
+        # test display rendered in correct order
+        target_re = (
+            r"This importer will import the following fields:[\\n\s]+"
+            r"<code>id, name, published_date, author_email</code>[\\n\s]+"
+        )
+        self.assertRegex(str(response.content), target_re)
```

### Comparing `django_import_export-4.0.3/tests/core/tests/admin_integration/test_views.py` & `django_import_export-4.0.5/tests/core/tests/admin_integration/test_views.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/resources.py` & `django_import_export-4.0.5/tests/core/tests/resources.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_base_formats.py` & `django_import_export-4.0.5/tests/core/tests/test_base_formats.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_declarative.py` & `django_import_export-4.0.5/tests/core/tests/test_declarative.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_fields.py` & `django_import_export-4.0.5/tests/core/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_forms.py` & `django_import_export-4.0.5/tests/core/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_instance_loaders.py` & `django_import_export-4.0.5/tests/core/tests/test_instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_invalidrow.py` & `django_import_export-4.0.5/tests/core/tests/test_invalidrow.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_mixins.py` & `django_import_export-4.0.5/tests/core/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_model_resource_fields_generate_widgets.py` & `django_import_export-4.0.5/tests/core/tests/test_model_resource_fields_generate_widgets.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_permissions.py` & `django_import_export-4.0.5/tests/core/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_bulk_operations.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_bulk_operations.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_diffs.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_diffs.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_import_export.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_import_export.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_misc.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_misc.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_data_handling.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_data_handling.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_data_import.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_data_import.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_error_handling.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_export.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_export.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_fields.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_m2m.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_m2m.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_queryset.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_queryset.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_relationship.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_relationship.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_resource.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_widget.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_modelresource/test_widget.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_natural_foreign_key.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_natural_foreign_key.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_resources/test_relationships.py` & `django_import_export-4.0.5/tests/core/tests/test_resources/test_relationships.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_results.py` & `django_import_export-4.0.5/tests/core/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_tmp_storages.py` & `django_import_export-4.0.5/tests/core/tests/test_tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/core/tests/test_widgets.py` & `django_import_export-4.0.5/tests/core/tests/test_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     def test_clean_returns_date_when_date_passed(self):
         self.assertEqual(self.date, self.widget.clean(self.date))
 
     @patch("import_export.widgets.logger")
     def test_clean_raises_ValueError(self, mock_logger):
         self.widget = widgets.DateWidget("x")
         with self.assertRaisesRegex(
-            ValueError, "Value could not be parsed using defined date formats."
+            ValueError, "Value could not be parsed using defined formats."
         ):
             self.widget.clean("2021-05-01")
         mock_logger.debug.assert_called_with(
             "time data '2021-05-01' does not match format 'x'"
         )
 
     @override_settings(USE_TZ=True)
@@ -184,15 +184,15 @@
     def test_clean(self):
         self.assertEqual(self.widget.clean("13.08.2012 18:00:00"), self.datetime)
 
     @patch("import_export.widgets.logger")
     def test_clean_raises_ValueError(self, mock_logger):
         self.widget = widgets.DateTimeWidget("x")
         with self.assertRaisesRegex(
-            ValueError, "Value could not be parsed using defined datetime formats."
+            ValueError, "Value could not be parsed using defined formats."
         ):
             self.widget.clean("2021-05-01")
         mock_logger.debug.assert_called_with(
             "time data '2021-05-01' does not match format 'x'"
         )
 
     @ignore_utcnow_deprecation_warning
@@ -293,15 +293,15 @@
         self.widget = widgets.TimeWidget()
         self.assertEqual(("%H:%M:%S",), self.widget.formats)
 
     @patch("import_export.widgets.logger")
     def test_clean_raises_ValueError(self, mock_logger):
         self.widget = widgets.TimeWidget("x")
         with self.assertRaisesRegex(
-            ValueError, "Value could not be parsed using defined time formats."
+            ValueError, "Value could not be parsed using defined formats."
         ):
             self.widget.clean("20:15:00")
         mock_logger.debug.assert_called_with(
             "time data '20:15:00' does not match format 'x'"
         )
 
     def test_clean_returns_time_when_time_passed(self):
```

### Comparing `django_import_export-4.0.3/tests/docker-compose.yml` & `django_import_export-4.0.5/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/scripts/bulk_import.py` & `django_import_export-4.0.5/tests/scripts/bulk_import.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tests/settings.py` & `django_import_export-4.0.5/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.3/tox.ini` & `django_import_export-4.0.5/tox.ini`

 * *Files identical despite different names*

