# Comparing `tmp/django_debug_toolbar-4.4.1.tar.gz` & `tmp/django_debug_toolbar-4.4.2.tar.gz`

## Comparing `django_debug_toolbar-4.4.1.tar` & `django_debug_toolbar-4.4.2.tar`

### file list

```diff
@@ -1,205 +1,205 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.editorconfig
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.readthedocs.yaml
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/Makefile
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/eslint.config.js
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/requirements_dev.txt
--rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/setup.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tox.ini
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.tx/config
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/_stubs.py
--rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/apps.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/decorators.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/forms.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/middleware.py
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/settings.py
--rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/toolbar.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/urls.py
--rw-r--r--   0        0        0    12326 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/utils.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/views.py
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/ca/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18361 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14330 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16706 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16045 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/fi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18288 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14785 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/he/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/id/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15689 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/pt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    20656 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19081 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15128 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15296 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16981 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/management/commands/__init__.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/management/commands/debugsqlshell.py
--rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/__init__.py
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/cache.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/headers.py
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/profiling.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/redirects.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/request.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/settings.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/signals.py
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/staticfiles.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/timer.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/versions.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/history/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/history/forms.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/history/panel.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/history/views.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/__init__.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/forms.py
--rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/panel.py
--rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/tracking.py
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/utils.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/views.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/templates/__init__.py
--rw-r--r--   0        0        0     8830 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/templates/panel.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/templates/views.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/css/print.css
--rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/css/toolbar.css
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/history.js
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/redirect.js
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/timer.js
--rw-r--r--   0        0        0    14601 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/toolbar.js
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/utils.js
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/base.html
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/redirect.html
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/includes/panel_button.html
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/includes/panel_content.html
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/includes/theme_selector.html
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/cache.html
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/headers.html
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/history.html
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/history_tr.html
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/profiling.html
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/request.html
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/request_variables.html
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/settings.html
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/signals.html
--rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql.html
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql_select.html
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/template_source.html
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/templates.html
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/timer.html
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/versions.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templatetags/__init__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/Makefile
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/architecture.rst
--rw-r--r--   0        0        0    28355 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/changes.rst
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/checks.rst
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/commands.rst
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/conf.py
--rw-r--r--   0        0        0    11907 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/configuration.rst
--rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/contributing.rst
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/index.rst
--rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/installation.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/make.bat
--rw-r--r--   0        0        0    11875 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/panels.rst
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/tips.rst
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/__init__.py
--rw-r--r--   0        0        0    84160 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/django-debug-toolbar.png
--rw-r--r--   0        0        0    55296 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/example.db
--rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/manage.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/screenshot.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/settings.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/test_views.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/urls.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/views.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/wsgi.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/static/test.css
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/templates/index.html
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/templates/htmx/boost.html
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/templates/jquery/index.html
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/templates/mootools/index.html
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/templates/prototype/index.html
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/templates/turbo/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/__init__.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/base.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/context_processors.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/forms.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/loaders.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/middleware.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/models.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/settings.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/sync.py
--rw-r--r--   0        0        0    11589 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/test_checks.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/test_decorators.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/test_forms.py
--rw-r--r--   0        0        0    33078 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/test_integration.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/test_utils.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/urls.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/urls_invalid.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/urls_use_package_urls.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/views.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/additional_static/base.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/commands/__init__.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/commands/test_debugsqlshell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/__init__.py
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_cache.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_custom.py
--rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_history.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_profiling.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_redirects.py
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_request.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_settings.py
--rw-r--r--   0        0        0    29916 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_sql.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_staticfiles.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_template.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_versions.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/base.html
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/basic.html
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/ajax/ajax.html
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/jinja2/basic.jinja
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/registration/login.html
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/sql/flat.html
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/sql/included.html
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/sql/nested.html
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/LICENSE
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/README.rst
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/pyproject.toml
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/.editorconfig
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/Makefile
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/eslint.config.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/requirements_dev.txt
+-rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/setup.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tox.ini
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/.tx/config
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/_stubs.py
+-rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/apps.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/decorators.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/forms.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/middleware.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/settings.py
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/toolbar.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/urls.py
+-rw-r--r--   0        0        0    12326 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/utils.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/views.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18361 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14330 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16706 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16045 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/fi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18288 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14785 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15689 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/pt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20656 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19081 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15128 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15296 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16981 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/management/commands/__init__.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/management/commands/debugsqlshell.py
+-rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/__init__.py
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/cache.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/headers.py
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/profiling.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/redirects.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/request.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/settings.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/signals.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/staticfiles.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/timer.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/versions.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/history/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/history/forms.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/history/panel.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/history/views.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/sql/__init__.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/sql/forms.py
+-rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/sql/panel.py
+-rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/sql/tracking.py
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/sql/utils.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/sql/views.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/templates/__init__.py
+-rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/templates/panel.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/panels/templates/views.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/static/debug_toolbar/css/print.css
+-rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/static/debug_toolbar/css/toolbar.css
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/static/debug_toolbar/js/history.js
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/static/debug_toolbar/js/redirect.js
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/static/debug_toolbar/js/timer.js
+-rw-r--r--   0        0        0    14601 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/static/debug_toolbar/js/toolbar.js
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/static/debug_toolbar/js/utils.js
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/base.html
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/redirect.html
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/includes/panel_button.html
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/includes/panel_content.html
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/includes/theme_selector.html
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/cache.html
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/headers.html
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/history.html
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/history_tr.html
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/profiling.html
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/request.html
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/request_variables.html
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/settings.html
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/signals.html
+-rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/sql.html
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/sql_select.html
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/template_source.html
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/templates.html
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/timer.html
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/versions.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/debug_toolbar/templatetags/__init__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/docs/Makefile
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/docs/architecture.rst
+-rw-r--r--   0        0        0    28634 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/docs/changes.rst
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/docs/checks.rst
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/docs/commands.rst
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/docs/conf.py
+-rw-r--r--   0        0        0    11930 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/docs/configuration.rst
+-rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/docs/contributing.rst
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/docs/index.rst
+-rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/docs/installation.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/docs/make.bat
+-rw-r--r--   0        0        0    11875 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/docs/panels.rst
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/docs/tips.rst
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/__init__.py
+-rw-r--r--   0        0        0    84160 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/django-debug-toolbar.png
+-rw-r--r--   0        0        0    55296 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/example.db
+-rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/manage.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/screenshot.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/settings.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/test_views.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/urls.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/views.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/wsgi.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/static/test.css
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/templates/index.html
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/templates/htmx/boost.html
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/templates/jquery/index.html
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/templates/mootools/index.html
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/templates/prototype/index.html
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/example/templates/turbo/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/base.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/context_processors.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/forms.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/loaders.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/middleware.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/models.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/settings.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/sync.py
+-rw-r--r--   0        0        0    11589 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/test_checks.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/test_decorators.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/test_forms.py
+-rw-r--r--   0        0        0    33078 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/test_integration.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/test_utils.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/urls.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/urls_invalid.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/urls_use_package_urls.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/views.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/additional_static/base.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/commands/__init__.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/commands/test_debugsqlshell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/panels/__init__.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/panels/test_cache.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/panels/test_custom.py
+-rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/panels/test_history.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/panels/test_profiling.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/panels/test_redirects.py
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/panels/test_request.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/panels/test_settings.py
+-rw-r--r--   0        0        0    29900 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/panels/test_sql.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/panels/test_staticfiles.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/panels/test_template.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/panels/test_versions.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/templates/base.html
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/templates/basic.html
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/templates/ajax/ajax.html
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/templates/jinja2/basic.jinja
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/templates/registration/login.html
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/templates/sql/flat.html
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/templates/sql/included.html
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/tests/templates/sql/nested.html
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/LICENSE
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/README.rst
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.2/PKG-INFO
```

### Comparing `django_debug_toolbar-4.4.1/.pre-commit-config.yaml` & `django_debug_toolbar-4.4.2/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     -   id: file-contents-sorter
         files: docs/spelling_wordlist.txt
 -   repo: https://github.com/pycqa/doc8
     rev: v1.1.1
     hooks:
     -   id: doc8
 -   repo: https://github.com/adamchainz/django-upgrade
-    rev: 1.16.0
+    rev: 1.17.0
     hooks:
     -   id: django-upgrade
         args: [--target-version, "4.2"]
 -   repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
     -   id: rst-backticks
@@ -28,32 +28,32 @@
     hooks:
     -   id: prettier
         entry: env PRETTIER_LEGACY_CLI=1 prettier
         types_or: [javascript, css]
         args:
         - --trailing-comma=es5
 -   repo: https://github.com/pre-commit/mirrors-eslint
-    rev: v9.0.0
+    rev: v9.3.0
     hooks:
     -   id: eslint
         additional_dependencies:
             - "eslint@v9.0.0-beta.1"
             - "@eslint/js@v9.0.0-beta.1"
             - "globals"
         files: \.js?$
         types: [file]
         args:
         - --fix
 -   repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.3.7'
+    rev: 'v0.4.5'
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
 -   repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 1.7.0
+    rev: 2.1.3
     hooks:
       - id: pyproject-fmt
 -   repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.16
+    rev: v0.18
     hooks:
       - id: validate-pyproject
```

### Comparing `django_debug_toolbar-4.4.1/CODE_OF_CONDUCT.md` & `django_debug_toolbar-4.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/Makefile` & `django_debug_toolbar-4.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/eslint.config.js` & `django_debug_toolbar-4.4.2/eslint.config.js`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tox.ini` & `django_debug_toolbar-4.4.2/tox.ini`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/.github/dependabot.yml` & `django_debug_toolbar-4.4.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/.github/workflows/coverage.yml` & `django_debug_toolbar-4.4.2/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/.github/workflows/release.yml` & `django_debug_toolbar-4.4.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/.github/workflows/test.yml` & `django_debug_toolbar-4.4.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/_stubs.py` & `django_debug_toolbar-4.4.2/debug_toolbar/_stubs.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/apps.py` & `django_debug_toolbar-4.4.2/debug_toolbar/apps.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/decorators.py` & `django_debug_toolbar-4.4.2/debug_toolbar/decorators.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/forms.py` & `django_debug_toolbar-4.4.2/debug_toolbar/forms.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/middleware.py` & `django_debug_toolbar-4.4.2/debug_toolbar/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 _HTML_TYPES = ("text/html", "application/xhtml+xml")
 
 
 def show_toolbar(request):
     """
     Default function to determine whether to show the toolbar on a given page.
     """
-    internal_ips = settings.INTERNAL_IPS.copy()
+    internal_ips = list(settings.INTERNAL_IPS)
 
     try:
         # This is a hack for docker installations. It attempts to look
         # up the IP address of the docker host.
         # This is not guaranteed to work.
         docker_ip = (
             # Convert the last segment of the IP address to be .1
```

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/settings.py` & `django_debug_toolbar-4.4.2/debug_toolbar/settings.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/toolbar.py` & `django_debug_toolbar-4.4.2/debug_toolbar/toolbar.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/utils.py` & `django_debug_toolbar-4.4.2/debug_toolbar/utils.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/views.py` & `django_debug_toolbar-4.4.2/debug_toolbar/views.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/ca/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/ca/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/cs/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/cs/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/de/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/de/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/en/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/es/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/es/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/fa/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/fa/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/fi/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/fi/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/fr/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/fr/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/he/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/he/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/id/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/id/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/it/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/it/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/ja/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/ja/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/nl/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/nl/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/pl/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/pl/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/pt/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/pt/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/ru/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/ru/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/sk/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/sk/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/uk/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/uk/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.2/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/management/commands/debugsqlshell.py` & `django_debug_toolbar-4.4.2/debug_toolbar/management/commands/debugsqlshell.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/__init__.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/__init__.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/cache.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/cache.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/headers.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/headers.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/profiling.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/profiling.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/redirects.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/redirects.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/request.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/request.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/settings.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/settings.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/signals.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/signals.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/staticfiles.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/staticfiles.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/timer.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/timer.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/versions.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/versions.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/history/panel.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/history/panel.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/history/views.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/history/views.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/forms.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/sql/forms.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/panel.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/sql/panel.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/tracking.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/sql/tracking.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/utils.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/sql/utils.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/views.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/sql/views.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/templates/panel.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/templates/panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                     # QuerySet would trigger the database: user can run the
                     # query from SQL Panel
                     elif isinstance(value, (QuerySet, RawQuerySet)):
                         temp_layer[key] = (
                             f"<<{value.__class__.__name__.lower()} of {value.model._meta.label}>>"
                         )
                     else:
-                        token = allow_sql.set(False)  # noqa: FBT003
+                        token = allow_sql.set(False)
                         try:
                             saferepr(value)  # this MAY trigger a db query
                         except SQLQueryTriggered:
                             temp_layer[key] = "<<triggers database query>>"
                         except UnicodeEncodeError:
                             temp_layer[key] = "<<Unicode encode error>>"
                         except Exception:
```

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/panels/templates/views.py` & `django_debug_toolbar-4.4.2/debug_toolbar/panels/templates/views.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/css/toolbar.css` & `django_debug_toolbar-4.4.2/debug_toolbar/static/debug_toolbar/css/toolbar.css`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
         "Segoe UI Symbol", "Noto Color Emoji";
     --djdt-font-family-monospace: ui-monospace, Menlo, Monaco, "Cascadia Mono",
         "Segoe UI Mono", "Roboto Mono", "Oxygen Mono", "Ubuntu Monospace",
         "Source Code Pro", "Fira Mono", "Droid Sans Mono", "Courier New",
         monospace, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol",
         "Noto Color Emoji";
 
-    color-scheme: light;
     --djdt-font-color: black;
     --djdt-background-color: white;
     --djdt-panel-content-background-color: #eee;
     --djdt-panel-content-table-background-color: var(--djdt-background-color);
     --djdt-panel-title-background-color: #ffc;
     --djdt-djdt-panel-content-table-strip-background-color: #f5f5f5;
     --djdt--highlighted-background-color: lightgrey;
@@ -31,15 +30,14 @@
     --djdt-button-border-color: var(--djdt-table-border-color);
     --djdt-pre-border-color: var(--djdt-table-border-color);
     --djdt-raw-border-color: var(--djdt-table-border-color);
 }
 
 @media (prefers-color-scheme: dark) {
     :root {
-        color-scheme: dark;
         --djdt-font-color: #8393a7;
         --djdt-background-color: #1e293bff;
         --djdt-panel-content-background-color: #0f1729ff;
         --djdt-panel-title-background-color: #242432;
         --djdt-djdt-panel-content-table-strip-background-color: #324154ff;
         --djdt--highlighted-background-color: #2c2a7dff;
         --djdt-toggle-template-background-color: #282755;
@@ -54,15 +52,14 @@
         --djdt-button-border-color: var(--djdt-table-border-color);
         --djdt-pre-border-color: var(--djdt-table-border-color);
         --djdt-raw-border-color: var(--djdt-table-border-color);
     }
 }
 
 #djDebug[data-theme="dark"] {
-    color-scheme: dark;
     --djdt-font-color: #8393a7;
     --djdt-background-color: #1e293bff;
     --djdt-panel-content-background-color: #0f1729ff;
     --djdt-panel-title-background-color: #242432;
     --djdt-djdt-panel-content-table-strip-background-color: #324154ff;
     --djdt--highlighted-background-color: #2c2a7dff;
     --djdt-toggle-template-background-color: #282755;
```

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/history.js` & `django_debug_toolbar-4.4.2/debug_toolbar/static/debug_toolbar/js/history.js`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/timer.js` & `django_debug_toolbar-4.4.2/debug_toolbar/static/debug_toolbar/js/timer.js`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/toolbar.js` & `django_debug_toolbar-4.4.2/debug_toolbar/static/debug_toolbar/js/toolbar.js`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/utils.js` & `django_debug_toolbar-4.4.2/debug_toolbar/static/debug_toolbar/js/utils.js`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/base.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/base.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/redirect.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/redirect.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/includes/panel_button.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/includes/panel_button.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/includes/panel_content.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/includes/panel_content.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/includes/theme_selector.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/includes/theme_selector.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/cache.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/cache.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/headers.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/headers.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/history.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/history.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/history_tr.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/history_tr.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/profiling.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/profiling.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/request.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/request.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/request_variables.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/request_variables.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/sql.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql_select.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/sql_select.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/templates.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/templates.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/timer.html` & `django_debug_toolbar-4.4.2/debug_toolbar/templates/debug_toolbar/panels/timer.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/docs/Makefile` & `django_debug_toolbar-4.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/docs/architecture.rst` & `django_debug_toolbar-4.4.2/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/docs/changes.rst` & `django_debug_toolbar-4.4.2/docs/changes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 Change log
 ==========
 
 Pending
 -------
 
+4.4.2 (2024-05-27)
+------------------
+
+* Removed some CSS which wasn't carefully limited to the toolbar's elements.
+* Stopped assuming that ``INTERNAL_IPS`` is a list.
+* Added a section to the installation docs about running tests in projects
+  where the toolbar is being used.
+
 
 4.4.1 (2024-05-26)
 ------------------
 
 * Pin metadata version to 2.2 to be compatible with Jazzband release
   process.
```

### Comparing `django_debug_toolbar-4.4.1/docs/checks.rst` & `django_debug_toolbar-4.4.2/docs/checks.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/docs/commands.rst` & `django_debug_toolbar-4.4.2/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/docs/conf.py` & `django_debug_toolbar-4.4.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "Django Debug Toolbar"
 copyright = "{}, Django Debug Toolbar developers and contributors"
 copyright = copyright.format(datetime.date.today().year)
 
 # The full version, including alpha/beta/rc tags
-release = "4.4.1"
+release = "4.4.2"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `django_debug_toolbar-4.4.1/docs/configuration.rst` & `django_debug_toolbar-4.4.2/docs/configuration.rst`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,16 @@
 * ``INSERT_BEFORE``
 
   Default: ``'</body>'``
 
   The toolbar searches for this string in the HTML and inserts itself just
   before.
 
+.. _IS_RUNNING_TESTS:
+
 * ``IS_RUNNING_TESTS``
 
   Default: ``"test" in sys.argv``
 
   This setting whether the application is running tests. If this resolves to
   ``True``, the toolbar will prevent you from running tests. This should only
   be changed if your test command doesn't include ``test`` or if you wish to
```

### Comparing `django_debug_toolbar-4.4.1/docs/contributing.rst` & `django_debug_toolbar-4.4.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/docs/installation.rst` & `django_debug_toolbar-4.4.2/docs/installation.rst`

 * *Files 5% similar despite different names*

```diff
@@ -152,14 +152,47 @@
 .. warning::
 
     If using Docker, the toolbar will attempt to look up your host name
     automatically and treat it as an allowable internal IP. If you're not
     able to get the toolbar to work with your docker installation, review
     the code in ``debug_toolbar.middleware.show_toolbar``.
 
+7. Disable the toolbar when running tests (optional)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+If you're running tests in your project you shouldn't activate the toolbar. You
+can do this by adding another setting:
+
+.. code-block:: python
+
+    TESTING = "test" in sys.argv
+
+    if not TESTING:
+        INSTALLED_APPS = [
+            *INSTALLED_APPS,
+            "debug_toolbar",
+        ]
+        MIDDLEWARE = [
+            "debug_toolbar.middleware.DebugToolbarMiddleware",
+            *MIDDLEWARE,
+        ]
+
+You should also modify your URLconf file:
+
+.. code-block:: python
+
+    if not settings.TESTING:
+        urlpatterns = [
+            *urlpatterns,
+            path("__debug__/", include("debug_toolbar.urls")),
+        ]
+
+Alternatively, you can check out the :ref:`IS_RUNNING_TESTS <IS_RUNNING_TESTS>`
+option.
+
 Troubleshooting
 ---------------
 
 On some platforms, the Django ``runserver`` command may use incorrect content
 types for static assets. To guess content types, Django relies on the
 :mod:`mimetypes` module from the Python standard library, which itself relies
 on the underlying platform's map files. If you find improper content types for
```

### Comparing `django_debug_toolbar-4.4.1/docs/make.bat` & `django_debug_toolbar-4.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/docs/panels.rst` & `django_debug_toolbar-4.4.2/docs/panels.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/docs/spelling_wordlist.txt` & `django_debug_toolbar-4.4.2/docs/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/docs/tips.rst` & `django_debug_toolbar-4.4.2/docs/tips.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/example/README.rst` & `django_debug_toolbar-4.4.2/example/README.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/example/django-debug-toolbar.png` & `django_debug_toolbar-4.4.2/example/django-debug-toolbar.png`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/example/example.db` & `django_debug_toolbar-4.4.2/example/example.db`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/example/screenshot.py` & `django_debug_toolbar-4.4.2/example/screenshot.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/example/settings.py` & `django_debug_toolbar-4.4.2/example/settings.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/example/urls.py` & `django_debug_toolbar-4.4.2/example/urls.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/example/templates/index.html` & `django_debug_toolbar-4.4.2/example/templates/index.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/example/templates/htmx/boost.html` & `django_debug_toolbar-4.4.2/example/templates/htmx/boost.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/example/templates/jquery/index.html` & `django_debug_toolbar-4.4.2/example/templates/jquery/index.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/example/templates/mootools/index.html` & `django_debug_toolbar-4.4.2/example/templates/mootools/index.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/example/templates/prototype/index.html` & `django_debug_toolbar-4.4.2/example/templates/prototype/index.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/example/templates/turbo/index.html` & `django_debug_toolbar-4.4.2/example/templates/turbo/index.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/base.py` & `django_debug_toolbar-4.4.2/tests/base.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/models.py` & `django_debug_toolbar-4.4.2/tests/models.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/settings.py` & `django_debug_toolbar-4.4.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/sync.py` & `django_debug_toolbar-4.4.2/tests/sync.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/test_checks.py` & `django_debug_toolbar-4.4.2/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/test_decorators.py` & `django_debug_toolbar-4.4.2/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/test_forms.py` & `django_debug_toolbar-4.4.2/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/test_integration.py` & `django_debug_toolbar-4.4.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/test_utils.py` & `django_debug_toolbar-4.4.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/urls.py` & `django_debug_toolbar-4.4.2/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/views.py` & `django_debug_toolbar-4.4.2/tests/views.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/commands/test_debugsqlshell.py` & `django_debug_toolbar-4.4.2/tests/commands/test_debugsqlshell.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/panels/test_cache.py` & `django_debug_toolbar-4.4.2/tests/panels/test_cache.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/panels/test_custom.py` & `django_debug_toolbar-4.4.2/tests/panels/test_custom.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/panels/test_history.py` & `django_debug_toolbar-4.4.2/tests/panels/test_history.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/panels/test_profiling.py` & `django_debug_toolbar-4.4.2/tests/panels/test_profiling.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/panels/test_redirects.py` & `django_debug_toolbar-4.4.2/tests/panels/test_redirects.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/panels/test_request.py` & `django_debug_toolbar-4.4.2/tests/panels/test_request.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/panels/test_settings.py` & `django_debug_toolbar-4.4.2/tests/panels/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/panels/test_sql.py` & `django_debug_toolbar-4.4.2/tests/panels/test_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         wraps=sql_tracking.patch_cursor_wrapper_with_mixin,
     )
     async def test_cursor_wrapper_asyncio_ctx(self, mock_patch_cursor_wrapper):
         self.assertTrue(sql_tracking.allow_sql.get())
         await sync_to_async(sql_call)()
 
         async def task():
-            sql_tracking.allow_sql.set(False)  # noqa: FBT003
+            sql_tracking.allow_sql.set(False)
             # By disabling sql_tracking.allow_sql, we are indicating that any
             # future SQL queries should be stopped. If SQL query occurs,
             # it raises an exception.
             with self.assertRaises(sql_tracking.SQLQueryTriggered):
                 await sync_to_async(sql_call)()
 
         # Ensure this is called in another context
```

### Comparing `django_debug_toolbar-4.4.1/tests/panels/test_staticfiles.py` & `django_debug_toolbar-4.4.2/tests/panels/test_staticfiles.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/panels/test_template.py` & `django_debug_toolbar-4.4.2/tests/panels/test_template.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/panels/test_versions.py` & `django_debug_toolbar-4.4.2/tests/panels/test_versions.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/tests/templates/ajax/ajax.html` & `django_debug_toolbar-4.4.2/tests/templates/ajax/ajax.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/LICENSE` & `django_debug_toolbar-4.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.4.1/README.rst` & `django_debug_toolbar-4.4.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 .. image:: https://raw.github.com/jazzband/django-debug-toolbar/main/example/django-debug-toolbar.png
    :alt: Django Debug Toolbar screenshot
 
 In addition to the built-in panels, a number of third-party panels are
 contributed by the community.
 
-The current stable version of the Debug Toolbar is 4.4.1. It works on
+The current stable version of the Debug Toolbar is 4.4.2. It works on
 Django ≥ 4.2.0.
 
 The Debug Toolbar does not currently support `Django's asynchronous views
 <https://docs.djangoproject.com/en/dev/topics/async/>`_.
 
 Documentation, including installation and configuration instructions, is
 available at https://django-debug-toolbar.readthedocs.io/.
```

### Comparing `django_debug_toolbar-4.4.1/pyproject.toml` & `django_debug_toolbar-4.4.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   "hatchling",
 ]
 
 [project]
 name = "django-debug-toolbar"
 description = "A configurable set of panels that display various debug information about the current request/response."
 readme = "README.rst"
-license = {text = "BSD-3-Clause"}
+license = { text = "BSD-3-Clause" }
 authors = [
-    { name = "Rob Hudson" },
+  { name = "Rob Hudson" },
 ]
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Web Environment",
   "Framework :: Django",
   "Framework :: Django :: 4.2",
@@ -31,40 +31,40 @@
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "Django>=4.2.9",
+  "django>=4.2.9",
   "sqlparse>=0.2",
 ]
-[project.urls]
-Download = "https://pypi.org/project/django-debug-toolbar/"
-Homepage = "https://github.com/jazzband/django-debug-toolbar"
+urls.Download = "https://pypi.org/project/django-debug-toolbar/"
+urls.Homepage = "https://github.com/jazzband/django-debug-toolbar"
 
 [tool.hatch.build.targets.sdist]
 # Jazzband's release process is limited to 2.2 metadata
 core-metadata-version = "2.2"
 
 [tool.hatch.build.targets.wheel]
-packages = ["debug_toolbar"]
+packages = [
+  "debug_toolbar",
+]
 # Jazzband's release process is limited to 2.2 metadata
 core-metadata-version = "2.2"
 
 [tool.hatch.version]
 path = "debug_toolbar/__init__.py"
 
 [tool.ruff]
-fix = true
-show-fixes = true
 target-version = "py38"
 
-[tool.ruff.lint]
-extend-select = [
+fix = true
+show-fixes = true
+lint.extend-select = [
   "ASYNC",  # flake8-async
   "B",      # flake8-bugbear
   "C4",     # flake8-comprehensions
   "C90",    # McCabe cyclomatic complexity
   "DJ",     # flake8-django
   "E",      # pycodestyle errors
   "F",      # Pyflakes
@@ -75,41 +75,41 @@
   "PIE",    # flake8-pie
   "RUF100", # Unused noqa directive
   "SIM",    # flake8-simplify
   "SLOT",   # flake8-slots
   "UP",     # pyupgrade
   "W",      # pycodestyle warnings
 ]
-extend-ignore = [
+lint.extend-ignore = [
   "B905",   # Allow zip() without strict=
   "E501",   # Ignore line length violations
   "SIM108", # Use ternary operator instead of if-else-block
+  "UP031",  # It's not always wrong to use percent-formatting
 ]
-
-[tool.ruff.lint.isort]
-combine-as-imports = true
-
-[tool.ruff.lint.mccabe]
-max-complexity = 16
-
-[tool.ruff.lint.per-file-ignores]
-"*/migrat*/*" = [
-  "N806",  # Allow using PascalCase model names in migrations
-  "N999",  # Ignore the fact that migration files are invalid module names
+lint.per-file-ignores."*/migrat*/*" = [
+  "N806", # Allow using PascalCase model names in migrations
+  "N999", # Ignore the fact that migration files are invalid module names
 ]
+lint.isort.combine-as-imports = true
+lint.mccabe.max-complexity = 16
 
 [tool.coverage.html]
 skip_covered = true
 skip_empty = true
 
 [tool.coverage.run]
 branch = true
 parallel = true
-source = ["debug_toolbar"]
+source = [
+  "debug_toolbar",
+]
 
 [tool.coverage.paths]
-source = ["src", ".tox/*/site-packages"]
+source = [
+  "src",
+  ".tox/*/site-packages",
+]
 
 [tool.coverage.report]
 # Update coverage badge link in README.rst when fail_under changes
 fail_under = 94
 show_missing = true
```

### Comparing `django_debug_toolbar-4.4.1/PKG-INFO` & `django_debug_toolbar-4.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.2
 Name: django-debug-toolbar
-Version: 4.4.1
+Version: 4.4.2
 Summary: A configurable set of panels that display various debug information about the current request/response.
 Project-URL: Download, https://pypi.org/project/django-debug-toolbar/
 Project-URL: Homepage, https://github.com/jazzband/django-debug-toolbar
 Author: Rob Hudson
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -70,15 +70,15 @@
 
 .. image:: https://raw.github.com/jazzband/django-debug-toolbar/main/example/django-debug-toolbar.png
    :alt: Django Debug Toolbar screenshot
 
 In addition to the built-in panels, a number of third-party panels are
 contributed by the community.
 
-The current stable version of the Debug Toolbar is 4.4.1. It works on
+The current stable version of the Debug Toolbar is 4.4.2. It works on
 Django ≥ 4.2.0.
 
 The Debug Toolbar does not currently support `Django's asynchronous views
 <https://docs.djangoproject.com/en/dev/topics/async/>`_.
 
 Documentation, including installation and configuration instructions, is
 available at https://django-debug-toolbar.readthedocs.io/.
```

