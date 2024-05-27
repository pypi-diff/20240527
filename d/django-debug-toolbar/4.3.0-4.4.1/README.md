# Comparing `tmp/django_debug_toolbar-4.3.0.tar.gz` & `tmp/django_debug_toolbar-4.4.1.tar.gz`

## Comparing `django_debug_toolbar-4.3.0.tar` & `django_debug_toolbar-4.4.1.tar`

### file list

```diff
@@ -1,200 +1,205 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.editorconfig
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.eslintrc.js
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.readthedocs.yaml
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/Makefile
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/requirements_dev.txt
--rwxr-xr-x   0        0        0      546 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/setup.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tox.ini
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.tx/config
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/_stubs.py
--rw-r--r--   0        0        0     7467 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/apps.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/decorators.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/forms.py
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/middleware.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/settings.py
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/toolbar.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/urls.py
--rw-r--r--   0        0        0    12326 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/utils.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/views.py
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/ca/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18361 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14330 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16706 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16045 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/fi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18288 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14785 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/he/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/id/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15689 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/pt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    20656 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19081 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15128 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15296 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16981 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/management/commands/__init__.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/management/commands/debugsqlshell.py
--rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/__init__.py
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/cache.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/headers.py
--rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/profiling.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/redirects.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/request.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/settings.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/signals.py
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/staticfiles.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/timer.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/versions.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/history/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/history/forms.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/history/panel.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/history/views.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/__init__.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/forms.py
--rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/panel.py
--rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/tracking.py
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/utils.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/views.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/templates/__init__.py
--rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/templates/panel.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/panels/templates/views.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/css/print.css
--rw-r--r--   0        0        0    12621 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/css/toolbar.css
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/history.js
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/redirect.js
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/timer.js
--rw-r--r--   0        0        0    13578 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/toolbar.js
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/utils.js
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/base.html
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/redirect.html
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/includes/panel_button.html
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/includes/panel_content.html
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/cache.html
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/headers.html
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/history.html
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/history_tr.html
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/profiling.html
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/request.html
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/request_variables.html
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/settings.html
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/signals.html
--rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql.html
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql_select.html
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/template_source.html
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/templates.html
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/timer.html
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/versions.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/debug_toolbar/templatetags/__init__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/Makefile
--rw-r--r--   0        0        0    26588 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/changes.rst
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/checks.rst
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/commands.rst
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/conf.py
--rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/configuration.rst
--rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/contributing.rst
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/index.rst
--rw-r--r--   0        0        0     7726 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/installation.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/make.bat
--rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/panels.rst
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/docs/tips.rst
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/__init__.py
--rw-r--r--   0        0        0    84160 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/django-debug-toolbar.png
--rw-r--r--   0        0        0    55296 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/example.db
--rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/manage.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/screenshot.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/settings.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/urls.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/views.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/wsgi.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/static/test.css
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/templates/index.html
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/templates/htmx/boost.html
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/templates/jquery/index.html
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/templates/mootools/index.html
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/templates/prototype/index.html
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/example/templates/turbo/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/__init__.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/base.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/context_processors.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/forms.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/loaders.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/middleware.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/models.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/settings.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/sync.py
--rw-r--r--   0        0        0    10081 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/test_checks.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/test_decorators.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/test_forms.py
--rw-r--r--   0        0        0    31235 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/test_integration.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/test_utils.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/urls.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/urls_invalid.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/urls_use_package_urls.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/views.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/additional_static/base.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/commands/__init__.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/commands/test_debugsqlshell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/__init__.py
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_cache.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_custom.py
--rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_history.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_profiling.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_redirects.py
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_request.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_settings.py
--rw-r--r--   0        0        0    29916 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_sql.py
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_staticfiles.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_template.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/panels/test_versions.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/base.html
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/basic.html
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/ajax/ajax.html
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/jinja2/basic.jinja
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/registration/login.html
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/sql/flat.html
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/sql/included.html
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/tests/templates/sql/nested.html
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/LICENSE
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/README.rst
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/pyproject.toml
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 django_debug_toolbar-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.editorconfig
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/Makefile
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/eslint.config.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/requirements_dev.txt
+-rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/setup.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tox.ini
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.tx/config
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/_stubs.py
+-rw-r--r--   0        0        0     8887 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/apps.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/decorators.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/forms.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/middleware.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/settings.py
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/toolbar.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/urls.py
+-rw-r--r--   0        0        0    12326 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/utils.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/views.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18361 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17796 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14330 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18086 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6597 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16706 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16045 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/fi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18288 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14785 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15689 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/pt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9018 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20656 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19081 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15128 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15296 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16981 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/management/commands/__init__.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/management/commands/debugsqlshell.py
+-rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/__init__.py
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/cache.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/headers.py
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/profiling.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/redirects.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/request.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/settings.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/signals.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/staticfiles.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/timer.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/versions.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/history/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/history/forms.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/history/panel.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/history/views.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/__init__.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/forms.py
+-rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/panel.py
+-rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/tracking.py
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/utils.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/views.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/templates/__init__.py
+-rw-r--r--   0        0        0     8830 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/templates/panel.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/panels/templates/views.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/css/print.css
+-rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/css/toolbar.css
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/history.js
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/redirect.js
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/timer.js
+-rw-r--r--   0        0        0    14601 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/toolbar.js
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/utils.js
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/base.html
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/redirect.html
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/includes/panel_button.html
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/includes/panel_content.html
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/includes/theme_selector.html
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/cache.html
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/headers.html
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/history.html
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/history_tr.html
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/profiling.html
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/request.html
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/request_variables.html
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/settings.html
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/signals.html
+-rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql.html
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql_select.html
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/template_source.html
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/templates.html
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/timer.html
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/versions.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/debug_toolbar/templatetags/__init__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/Makefile
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/architecture.rst
+-rw-r--r--   0        0        0    28355 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/changes.rst
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/checks.rst
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/commands.rst
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/conf.py
+-rw-r--r--   0        0        0    11907 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/configuration.rst
+-rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/contributing.rst
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/index.rst
+-rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/installation.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/make.bat
+-rw-r--r--   0        0        0    11875 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/panels.rst
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/docs/tips.rst
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/__init__.py
+-rw-r--r--   0        0        0    84160 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/django-debug-toolbar.png
+-rw-r--r--   0        0        0    55296 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/example.db
+-rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/manage.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/screenshot.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/settings.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/test_views.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/urls.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/views.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/wsgi.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/static/test.css
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/templates/index.html
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/templates/htmx/boost.html
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/templates/jquery/index.html
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/templates/mootools/index.html
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/templates/prototype/index.html
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/example/templates/turbo/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/base.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/context_processors.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/forms.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/loaders.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/middleware.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/models.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/settings.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/sync.py
+-rw-r--r--   0        0        0    11589 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/test_checks.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/test_decorators.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/test_forms.py
+-rw-r--r--   0        0        0    33078 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/test_integration.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/test_utils.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/urls.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/urls_invalid.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/urls_use_package_urls.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/views.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/additional_static/base.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/commands/__init__.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/commands/test_debugsqlshell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/__init__.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_cache.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_custom.py
+-rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_history.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_profiling.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_redirects.py
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_request.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_settings.py
+-rw-r--r--   0        0        0    29916 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_sql.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_staticfiles.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_template.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/panels/test_versions.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/base.html
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/basic.html
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/ajax/ajax.html
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/jinja2/basic.jinja
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/registration/login.html
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/sql/flat.html
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/sql/included.html
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/tests/templates/sql/nested.html
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/LICENSE
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/README.rst
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 django_debug_toolbar-4.4.1/PKG-INFO
```

### Comparing `django_debug_toolbar-4.3.0/.pre-commit-config.yaml` & `django_debug_toolbar-4.4.1/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: check-toml
     -   id: check-yaml
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
     -   id: mixed-line-ending
     -   id: file-contents-sorter
         files: docs/spelling_wordlist.txt
 -   repo: https://github.com/pycqa/doc8
     rev: v1.1.1
     hooks:
     -   id: doc8
 -   repo: https://github.com/adamchainz/django-upgrade
-    rev: 1.15.0
+    rev: 1.16.0
     hooks:
     -   id: django-upgrade
-        args: [--target-version, "3.2"]
+        args: [--target-version, "4.2"]
 -   repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
     -   id: rst-backticks
     -   id: rst-directive-colons
 -   repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
     hooks:
     -   id: prettier
         entry: env PRETTIER_LEGACY_CLI=1 prettier
         types_or: [javascript, css]
         args:
         - --trailing-comma=es5
 -   repo: https://github.com/pre-commit/mirrors-eslint
-    rev: v8.56.0
+    rev: v9.0.0
     hooks:
     -   id: eslint
+        additional_dependencies:
+            - "eslint@v9.0.0-beta.1"
+            - "@eslint/js@v9.0.0-beta.1"
+            - "globals"
         files: \.js?$
         types: [file]
         args:
         - --fix
 -   repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.1.11'
+    rev: 'v0.3.7'
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
 -   repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 1.5.3
+    rev: 1.7.0
     hooks:
       - id: pyproject-fmt
 -   repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.15
+    rev: v0.16
     hooks:
       - id: validate-pyproject
```

### Comparing `django_debug_toolbar-4.3.0/CODE_OF_CONDUCT.md` & `django_debug_toolbar-4.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/Makefile` & `django_debug_toolbar-4.4.1/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 example:
 	python example/manage.py migrate --noinput
 	-DJANGO_SUPERUSER_PASSWORD=p python example/manage.py createsuperuser \
 		--noinput --username="$(USER)" --email="$(USER)@mailinator.com"
 	python example/manage.py runserver
 
+example_test:
+	python example/manage.py test example
+
 test:
 	DJANGO_SETTINGS_MODULE=tests.settings \
 		python -m django test $${TEST_ARGS:-tests}
 
 test_selenium:
 	DJANGO_SELENIUM_TESTS=true DJANGO_SETTINGS_MODULE=tests.settings \
 		python -m django test $${TEST_ARGS:-tests}
```

### Comparing `django_debug_toolbar-4.3.0/tox.ini` & `django_debug_toolbar-4.4.1/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 [tox]
 isolated_build = true
 envlist =
     docs
     packaging
-    py{38,39,310}-dj32-{sqlite,postgresql,postgis,mysql}
-    py{310,311}-dj41-{sqlite,postgresql,postgis,mysql}
+    py{38,39,310,311,312}-dj{42}-{sqlite,postgresql,postgis,mysql}
     py{310,311,312}-dj{42,50,main}-{sqlite,postgresql,psycopg3,postgis,mysql}
 
 [testenv]
 deps =
-    dj32: django~=3.2.9
-    dj41: django~=4.1.3
     dj42: django~=4.2.1
-    dj50: django~=5.0a1
+    dj50: django~=5.0.2
     djmain: https://github.com/django/django/archive/main.tar.gz
     postgresql: psycopg2-binary
     psycopg3: psycopg[binary]
     postgis: psycopg2-binary
     mysql: mysqlclient
     coverage[toml]
     Jinja2
@@ -29,52 +26,53 @@
     COVERAGE_ARGS
     DB_BACKEND
     DB_NAME
     DB_USER
     DB_PASSWORD
     DB_HOST
     DB_PORT
+    DISPLAY
+    DJANGO_SELENIUM_TESTS
     GITHUB_*
 setenv =
     PYTHONPATH = {toxinidir}
     PYTHONWARNINGS = d
-    py39-dj32-postgresql: DJANGO_SELENIUM_TESTS = true
-    py311-dj42-postgresql: DJANGO_SELENIUM_TESTS = true
+    py311-dj42-postgresql: DJANGO_SELENIUM_TESTS = {env:DJANGO_SELENIUM_TESTS:true}
     DB_NAME = {env:DB_NAME:debug_toolbar}
     DB_USER = {env:DB_USER:debug_toolbar}
     DB_HOST = {env:DB_HOST:localhost}
     DB_PASSWORD =  {env:DB_PASSWORD:debug_toolbar}
     DJANGO_SETTINGS_MODULE = tests.settings
 allowlist_externals = make
 pip_pre = True
 commands = python -b -W always -m coverage run -m django test -v2 {posargs:tests}
 
 
-[testenv:py{38,39,310,311,312}-dj{32,41,42,50,main}-{postgresql,psycopg3}]
+[testenv:py{38,39,310,311,312}-dj{42,50,main}-{postgresql,psycopg3}]
 setenv =
     {[testenv]setenv}
     DB_BACKEND = postgresql
     DB_PORT = {env:DB_PORT:5432}
 
 
-[testenv:py{38,39,310,311,312}-dj{32,41,42,50,main}-postgis]
+[testenv:py{38,39,310,311,312}-dj{42,50,main}-postgis]
 setenv =
     {[testenv]setenv}
     DB_BACKEND = postgis
     DB_PORT = {env:DB_PORT:5432}
 
 
-[testenv:py{38,39,310,311,312}-dj{32,41,42,50,main}-mysql]
+[testenv:py{38,39,310,311,312}-dj{42,50,main}-mysql]
 setenv =
     {[testenv]setenv}
     DB_BACKEND = mysql
     DB_PORT = {env:DB_PORT:3306}
 
 
-[testenv:py{38,39,310,311,312}-dj{32,41,42,50,main}-sqlite]
+[testenv:py{38,39,310,311,312}-dj{42,50,main}-sqlite]
 setenv =
     {[testenv]setenv}
     DB_BACKEND = sqlite3
     DB_NAME = ":memory:"
 
 [testenv:docs]
 commands = make -C {toxinidir}/docs {posargs:spelling}
```

### Comparing `django_debug_toolbar-4.3.0/.github/workflows/release.yml` & `django_debug_toolbar-4.4.1/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.8
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U build hatchling twine
```

### Comparing `django_debug_toolbar-4.3.0/.github/workflows/test.yml` & `django_debug_toolbar-4.4.1/.github/workflows/test.yml`

 * *Files 22% similar despite different names*

```diff
@@ -29,26 +29,26 @@
         ports:
         - 3306:3306
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         allow-prereleases: true
 
     - name: Get pip cache dir
       id: pip-cache
       run: |
         echo "dir=$(pip cache dir)" >> $GITHUB_OUTPUT
 
     - name: Cache
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ${{ steps.pip-cache.outputs.dir }}
         key:
           ${{ matrix.python-version }}-v1-${{ hashFiles('**/pyproject.toml') }}-${{ hashFiles('**/tox.ini') }}
         restore-keys: |
           ${{ matrix.python-version }}-v1-
 
@@ -62,19 +62,14 @@
       env:
         DB_BACKEND: mysql
         DB_USER: root
         DB_PASSWORD: debug_toolbar
         DB_HOST: 127.0.0.1
         DB_PORT: 3306
 
-    - name: Upload coverage data
-      uses: actions/upload-artifact@v3
-      with:
-        name: coverage-data
-        path: ".coverage.*"
 
   postgres:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       max-parallel: 5
       matrix:
@@ -104,26 +99,26 @@
           --health-timeout 5s
           --health-retries 5
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         allow-prereleases: true
 
     - name: Get pip cache dir
       id: pip-cache
       run: |
         echo "dir=$(pip cache dir)" >> $GITHUB_OUTPUT
 
     - name: Cache
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ${{ steps.pip-cache.outputs.dir }}
         key:
           ${{ matrix.python-version }}-v1-${{ hashFiles('**/pyproject.toml') }}-${{ hashFiles('**/tox.ini') }}
         restore-keys: |
           ${{ matrix.python-version }}-v1-
 
@@ -140,44 +135,38 @@
     - name: Test with tox
       run: tox
       env:
         DB_BACKEND: ${{ matrix.database }}
         DB_HOST: localhost
         DB_PORT: 5432
 
-    - name: Upload coverage data
-      uses: actions/upload-artifact@v3
-      with:
-        name: coverage-data
-        path: ".coverage.*"
-
   sqlite:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       max-parallel: 5
       matrix:
         python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         allow-prereleases: true
 
     - name: Get pip cache dir
       id: pip-cache
       run: |
         echo "dir=$(pip cache dir)" >> $GITHUB_OUTPUT
 
     - name: Cache
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ${{ steps.pip-cache.outputs.dir }}
         key:
           ${{ matrix.python-version }}-v1-${{ hashFiles('**/pyproject.toml') }}-${{ hashFiles('**/tox.ini') }}
         restore-keys: |
           ${{ matrix.python-version }}-v1-
 
@@ -188,71 +177,34 @@
 
     - name: Test with tox
       run: tox
       env:
         DB_BACKEND: sqlite3
         DB_NAME: ":memory:"
 
-    - name: Upload coverage data
-      uses: actions/upload-artifact@v3
-      with:
-        name: coverage-data
-        path: ".coverage.*"
-
-  coverage:
-    name: Check coverage.
-    runs-on: "ubuntu-latest"
-    needs: [sqlite, mysql, postgres]
-    steps:
-      - uses: actions/checkout@v4
-      - uses: actions/setup-python@v4
-        with:
-          # Use latest, so it understands all syntax.
-          python-version: "3.11"
-
-      - run: python -m pip install --upgrade coverage[toml]
-
-      - name: Download coverage data.
-        uses: actions/download-artifact@v3
-        with:
-          name: coverage-data
-
-      - name: Combine coverage & check percentage
-        run: |
-          python -m coverage combine
-          python -m coverage html
-          python -m coverage report
-
-      - name: Upload HTML report if check failed.
-        uses: actions/upload-artifact@v3
-        with:
-          name: html-report
-          path: htmlcov
-        if: ${{ failure() }}
-
   lint:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: 3.8
 
     - name: Get pip cache dir
       id: pip-cache
       run: |
         echo "dir=$(pip cache dir)" >> $GITHUB_OUTPUT
 
     - name: Cache
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ${{ steps.pip-cache.outputs.dir }}
         key:
           ${{ matrix.python-version }}-v1-${{ hashFiles('**/pyproject.toml') }}-${{ hashFiles('**/tox.ini') }}
         restore-keys: |
           ${{ matrix.python-version }}-v1-
```

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/_stubs.py` & `django_debug_toolbar-4.4.1/debug_toolbar/_stubs.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/apps.py` & `django_debug_toolbar-4.4.1/debug_toolbar/apps.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 import mimetypes
 
 from django.apps import AppConfig
 from django.conf import settings
-from django.core.checks import Warning, register
+from django.core.checks import Error, Warning, register
 from django.middleware.gzip import GZipMiddleware
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext_lazy as _
 
 from debug_toolbar import settings as dt_settings
 
 
@@ -173,15 +173,15 @@
                 "settings.py.",
                 id="debug_toolbar.W005",
             )
         )
     return errors
 
 
-@register()
+@register
 def js_mimetype_check(app_configs, **kwargs):
     """
     Check that JavaScript files are resolving to the correct content type.
     """
     # Ideally application/javascript is returned, but text/javascript is
     # acceptable.
     javascript_types = {"application/javascript", "text/javascript"}
@@ -202,7 +202,44 @@
                 "\n"
                 "[HKEY_CLASSES_ROOT\\.js]\n"
                 '"Content Type"="application/javascript"',
                 id="debug_toolbar.W007",
             )
         ]
     return []
+
+
+@register
+def debug_toolbar_installed_when_running_tests_check(app_configs, **kwargs):
+    """
+    Check that the toolbar is not being used when tests are running
+    """
+    if not settings.DEBUG and dt_settings.get_config()["IS_RUNNING_TESTS"]:
+        return [
+            Error(
+                "The Django Debug Toolbar can't be used with tests",
+                hint="Django changes the DEBUG setting to False when running "
+                "tests. By default the Django Debug Toolbar is installed because "
+                "DEBUG is set to True. For most cases, you need to avoid installing "
+                "the toolbar when running tests. If you feel this check is in error, "
+                "you can set `DEBUG_TOOLBAR_CONFIG['IS_RUNNING_TESTS'] = False` to "
+                "bypass this check.",
+                id="debug_toolbar.E001",
+            )
+        ]
+    else:
+        return []
+
+
+@register
+def check_settings(app_configs, **kwargs):
+    errors = []
+    USER_CONFIG = getattr(settings, "DEBUG_TOOLBAR_CONFIG", {})
+    if "OBSERVE_REQUEST_CALLBACK" in USER_CONFIG:
+        errors.append(
+            Warning(
+                "The deprecated OBSERVE_REQUEST_CALLBACK setting is present in DEBUG_TOOLBAR_CONFIG.",
+                hint="Use the UPDATE_ON_FETCH and/or SHOW_TOOLBAR_CALLBACK settings instead.",
+                id="debug_toolbar.W008",
+            )
+        )
+    return errors
```

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/decorators.py` & `django_debug_toolbar-4.4.1/debug_toolbar/decorators.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/forms.py` & `django_debug_toolbar-4.4.1/debug_toolbar/forms.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/settings.py` & `django_debug_toolbar-4.4.1/debug_toolbar/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import warnings
 from functools import lru_cache
 
 from django.conf import settings
 from django.dispatch import receiver
 from django.test.signals import setting_changed
 
@@ -38,15 +39,17 @@
     "PROFILER_MAX_DEPTH": 10,
     "PROFILER_THRESHOLD_RATIO": 8,
     "SHOW_TEMPLATE_CONTEXT": True,
     "SKIP_TEMPLATE_PREFIXES": ("django/forms/widgets/", "admin/widgets/"),
     "SQL_WARNING_THRESHOLD": 500,  # milliseconds
     "OBSERVE_REQUEST_CALLBACK": "debug_toolbar.toolbar.observe_request",
     "TOOLBAR_LANGUAGE": None,
+    "IS_RUNNING_TESTS": "test" in sys.argv,
     "UPDATE_ON_FETCH": False,
+    "DEFAULT_THEME": "auto",
 }
 
 
 @lru_cache(maxsize=None)
 def get_config():
     USER_CONFIG = getattr(settings, "DEBUG_TOOLBAR_CONFIG", {})
     CONFIG = CONFIG_DEFAULTS.copy()
```

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/toolbar.py` & `django_debug_toolbar-4.4.1/debug_toolbar/toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,8 +181,8 @@
             return func_or_path
 
 
 def observe_request(request):
     """
     Determine whether to update the toolbar from a client side request.
     """
-    return not DebugToolbar.is_toolbar_request(request)
+    return True
```

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/utils.py` & `django_debug_toolbar-4.4.1/debug_toolbar/utils.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/views.py` & `django_debug_toolbar-4.4.1/debug_toolbar/views.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/ca/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/ca/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/cs/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/cs/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/de/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/de/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/en/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/es/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/es/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/fa/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/fa/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/fi/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/fi/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/fr/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/fr/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/he/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/he/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/id/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/id/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/it/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/it/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/ja/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/ja/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/nl/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/nl/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/pl/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/pl/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/pt/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/pt/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/ru/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/ru/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/sk/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/sk/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/sv_SE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/uk/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/uk/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po` & `django_debug_toolbar-4.4.1/debug_toolbar/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/management/commands/debugsqlshell.py` & `django_debug_toolbar-4.4.1/debug_toolbar/management/commands/debugsqlshell.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/__init__.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/__init__.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/cache.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/cache.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/headers.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/headers.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/profiling.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/profiling.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,20 +82,18 @@
                 file_path,
                 file_name,
                 line_num,
                 method,
             )
 
     def subfuncs(self):
-        i = 0
         h, s, v = self.hsv
         count = len(self.statobj.all_callees[self.func])
-        for func, stats in self.statobj.all_callees[self.func].items():
-            i += 1
-            h1 = h + (i / count) / (self.depth + 1)
+        for i, (func, stats) in enumerate(self.statobj.all_callees[self.func].items()):
+            h1 = h + ((i + 1) / count) / (self.depth + 1)
             s1 = 0 if stats[3] == 0 else s * (stats[3] / self.stats[3])
             yield FunctionCall(
                 self.statobj,
                 func,
                 self.depth + 1,
                 stats=stats,
                 id=str(self.id) + "_" + str(i),
```

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/redirects.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/redirects.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/request.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/request.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/settings.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/settings.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/signals.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/signals.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/staticfiles.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/staticfiles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import contextlib
 from contextvars import ContextVar
 from os.path import join, normpath
 
 from django.conf import settings
 from django.contrib.staticfiles import finders, storage
-from django.core.checks import Warning
 from django.utils.functional import LazyObject
 from django.utils.translation import gettext_lazy as _, ngettext
 
 from debug_toolbar import panels
 
 
 class StaticFile:
@@ -174,31 +173,7 @@
         apps = []
         for finder in finders.get_finders():
             if isinstance(finder, finders.AppDirectoriesFinder):
                 for app in finder.apps:
                     if app not in apps:
                         apps.append(app)
         return apps
-
-    @classmethod
-    def run_checks(cls):
-        """
-        Check that the integration is configured correctly for the panel.
-
-        Specifically look for static files that haven't been collected yet.
-
-        Return a list of :class: `django.core.checks.CheckMessage` instances.
-        """
-        errors = []
-        for finder in finders.get_finders():
-            try:
-                for path, finder_storage in finder.list([]):
-                    finder_storage.path(path)
-            except OSError:
-                errors.append(
-                    Warning(
-                        "debug_toolbar requires the STATICFILES_DIRS directories to exist.",
-                        hint="Running manage.py collectstatic may help uncover the issue.",
-                        id="debug_toolbar.staticfiles.W001",
-                    )
-                )
-        return errors
```

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/timer.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/timer.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/versions.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/versions.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/history/panel.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/history/panel.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/history/views.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/history/views.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/forms.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/forms.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/panel.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/panel.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/tracking.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/tracking.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/utils.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/utils.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/sql/views.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/sql/views.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/templates/panel.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/templates/panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,17 +150,17 @@
                     # Replace LANGUAGES, which is available in i18n context
                     # processor
                     elif key == "LANGUAGES" and isinstance(value, tuple):
                         temp_layer[key] = "<<languages>>"
                     # QuerySet would trigger the database: user can run the
                     # query from SQL Panel
                     elif isinstance(value, (QuerySet, RawQuerySet)):
-                        temp_layer[
-                            key
-                        ] = f"<<{value.__class__.__name__.lower()} of {value.model._meta.label}>>"
+                        temp_layer[key] = (
+                            f"<<{value.__class__.__name__.lower()} of {value.model._meta.label}>>"
+                        )
                     else:
                         token = allow_sql.set(False)  # noqa: FBT003
                         try:
                             saferepr(value)  # this MAY trigger a db query
                         except SQLQueryTriggered:
                             temp_layer[key] = "<<triggers database query>>"
                         except UnicodeEncodeError:
```

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/panels/templates/views.py` & `django_debug_toolbar-4.4.1/debug_toolbar/panels/templates/views.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/css/toolbar.css` & `django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/css/toolbar.css`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,92 @@
 /* Variable definitions */
-:root {
+:root,
+#djDebug[data-theme="light"] {
     /* Font families are the same as in Django admin/css/base.css */
     --djdt-font-family-primary: "Segoe UI", system-ui, Roboto, "Helvetica Neue",
         Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji",
         "Segoe UI Symbol", "Noto Color Emoji";
     --djdt-font-family-monospace: ui-monospace, Menlo, Monaco, "Cascadia Mono",
         "Segoe UI Mono", "Roboto Mono", "Oxygen Mono", "Ubuntu Monospace",
         "Source Code Pro", "Fira Mono", "Droid Sans Mono", "Courier New",
         monospace, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol",
         "Noto Color Emoji";
+
+    color-scheme: light;
+    --djdt-font-color: black;
+    --djdt-background-color: white;
+    --djdt-panel-content-background-color: #eee;
+    --djdt-panel-content-table-background-color: var(--djdt-background-color);
+    --djdt-panel-title-background-color: #ffc;
+    --djdt-djdt-panel-content-table-strip-background-color: #f5f5f5;
+    --djdt--highlighted-background-color: lightgrey;
+    --djdt-toggle-template-background-color: #bbb;
+
+    --djdt-sql-font-color: #333;
+    --djdt-pre-text-color: #555;
+    --djdt-path-and-locals: #777;
+    --djdt-stack-span-color: black;
+    --djdt-template-highlight-color: #333;
+
+    --djdt-table-border-color: #ccc;
+    --djdt-button-border-color: var(--djdt-table-border-color);
+    --djdt-pre-border-color: var(--djdt-table-border-color);
+    --djdt-raw-border-color: var(--djdt-table-border-color);
+}
+
+@media (prefers-color-scheme: dark) {
+    :root {
+        color-scheme: dark;
+        --djdt-font-color: #8393a7;
+        --djdt-background-color: #1e293bff;
+        --djdt-panel-content-background-color: #0f1729ff;
+        --djdt-panel-title-background-color: #242432;
+        --djdt-djdt-panel-content-table-strip-background-color: #324154ff;
+        --djdt--highlighted-background-color: #2c2a7dff;
+        --djdt-toggle-template-background-color: #282755;
+
+        --djdt-sql-font-color: var(--djdt-font-color);
+        --djdt-pre-text-color: var(--djdt-font-color);
+        --djdt-path-and-locals: #65758cff;
+        --djdt-stack-span-color: #7c8fa4;
+        --djdt-template-highlight-color: var(--djdt-stack-span-color);
+
+        --djdt-table-border-color: #324154ff;
+        --djdt-button-border-color: var(--djdt-table-border-color);
+        --djdt-pre-border-color: var(--djdt-table-border-color);
+        --djdt-raw-border-color: var(--djdt-table-border-color);
+    }
+}
+
+#djDebug[data-theme="dark"] {
+    color-scheme: dark;
+    --djdt-font-color: #8393a7;
+    --djdt-background-color: #1e293bff;
+    --djdt-panel-content-background-color: #0f1729ff;
+    --djdt-panel-title-background-color: #242432;
+    --djdt-djdt-panel-content-table-strip-background-color: #324154ff;
+    --djdt--highlighted-background-color: #2c2a7dff;
+    --djdt-toggle-template-background-color: #282755;
+
+    --djdt-sql-font-color: var(--djdt-font-color);
+    --djdt-pre-text-color: var(--djdt-font-color);
+    --djdt-path-and-locals: #65758cff;
+    --djdt-stack-span-color: #7c8fa4;
+    --djdt-template-highlight-color: var(--djdt-stack-span-color);
+
+    --djdt-table-border-color: #324154ff;
+    --djdt-button-border-color: var(--djdt-table-border-color);
+    --djdt-pre-border-color: var(--djdt-table-border-color);
+    --djdt-raw-border-color: var(--djdt-table-border-color);
 }
 
 /* Debug Toolbar CSS Reset, adapted from Eric Meyer's CSS Reset */
 #djDebug {
-    color: #000;
-    background: #fff;
+    color: var(--djdt-font-color);
+    background: var(--djdt-background-color);
 }
 #djDebug,
 #djDebug div,
 #djDebug span,
 #djDebug applet,
 #djDebug object,
 #djDebug iframe,
@@ -83,28 +151,28 @@
     padding: 0;
     min-width: 0;
     width: auto;
     border: 0;
     outline: 0;
     font-size: 12px;
     line-height: 1.5em;
-    color: #000;
+    color: var(--djdt-font-color);
     vertical-align: baseline;
     background-color: transparent;
     font-family: var(--djdt-font-family-primary);
     text-align: left;
     text-shadow: none;
     white-space: normal;
     transition: none;
 }
 
 #djDebug button {
     background-color: #eee;
     background-image: linear-gradient(to bottom, #eee, #cccccc);
-    border: 1px solid #ccc;
+    border: 1px solid var(--djdt-button-border-color);
     border-bottom: 1px solid #bbb;
     border-radius: 3px;
     color: #333;
     line-height: 1;
     padding: 0 8px;
     text-align: center;
     text-shadow: 0 1px 0 #eee;
@@ -264,41 +332,41 @@
 #djDebug code {
     font-size: 12px;
     white-space: pre;
 }
 
 #djDebug pre {
     white-space: pre-wrap;
-    color: #555;
-    border: 1px solid #ccc;
+    color: var(--djdt-pre-text-color);
+    border: 1px solid var(--djdt-pre-border-color);
     border-collapse: collapse;
-    background-color: #fff;
+    background-color: var(--djdt-background-color);
     padding: 2px 3px;
     margin-bottom: 3px;
 }
 
 #djDebug .djdt-panelContent {
     position: fixed;
     margin: 0;
     top: 0;
     right: 220px;
     bottom: 0;
     left: 0px;
-    background-color: #eee;
+    background-color: var(--djdt-panel-content-background-color);
     color: #666;
     z-index: 100000000;
 }
 
 #djDebug .djdt-panelContent > div {
     border-bottom: 1px solid #ddd;
 }
 
 #djDebug .djDebugPanelTitle {
     position: absolute;
-    background-color: #ffc;
+    background-color: var(--djdt-panel-title-background-color);
     color: #666;
     padding-left: 20px;
     top: 0;
     right: 0;
     left: 0;
     height: 50px;
 }
@@ -353,24 +421,24 @@
 #djDebug h4 {
     font-size: 20px;
     font-weight: bold;
     margin-top: 0.8em;
 }
 
 #djDebug .djdt-panelContent table {
-    border: 1px solid #ccc;
+    border: 1px solid var(--djdt-table-border-color);
     border-collapse: collapse;
     width: 100%;
-    background-color: #fff;
+    background-color: var(--djdt-panel-content-table-background-color);
     display: table;
     margin-top: 0.8em;
     overflow: auto;
 }
 #djDebug .djdt-panelContent tbody > tr:nth-child(odd):not(.djdt-highlighted) {
-    background-color: #f5f5f5;
+    background-color: var(--djdt-panel-content-table-strip-background-color);
 }
 #djDebug .djdt-panelContent tbody td,
 #djDebug .djdt-panelContent tbody th {
     vertical-align: top;
     padding: 2px 3px;
 }
 #djDebug .djdt-panelContent tbody td.djdt-time {
@@ -388,15 +456,15 @@
     width: 12em;
     text-align: right;
     color: #666;
     padding-right: 0.5em;
 }
 
 #djDebug .djTemplateContext {
-    background-color: #fff;
+    background-color: var(--djdt-background-color);
 }
 
 #djDebug .djdt-panelContent .djDebugClose {
     position: absolute;
     top: 4px;
     right: 15px;
     line-height: 16px;
@@ -429,31 +497,31 @@
 
 #djDebug .djdt-panelContent dd {
     margin-left: 10px;
 }
 
 #djDebug a.toggleTemplate {
     padding: 4px;
-    background-color: #bbb;
+    background-color: var(--djdt-toggle-template-background-color);
     border-radius: 3px;
 }
 
 #djDebug a.toggleTemplate:hover {
     padding: 4px;
     background-color: #444;
     color: #ffe761;
     border-radius: 3px;
 }
 
 #djDebug .djDebugCollapsed {
-    color: #333;
+    color: var(--djdt-sql-font-color);
 }
 
 #djDebug .djDebugUncollapsed {
-    color: #333;
+    color: var(--djdt-sql-font-color);
 }
 
 #djDebug .djUnselected {
     display: none;
 }
 
 #djDebug tr.djSelected {
@@ -479,74 +547,74 @@
     z-index: 1000000001;
 }
 #djDebug span.djDebugLineChartWarning {
     background-color: #900;
 }
 
 #djDebug .highlight {
-    color: #000;
+    color: var(--djdt-font-color);
 }
 #djDebug .highlight .err {
-    color: #000;
+    color: var(--djdt-font-color);
 } /* Error */
 #djDebug .highlight .g {
-    color: #000;
+    color: var(--djdt-font-color);
 } /* Generic */
 #djDebug .highlight .k {
-    color: #000;
+    color: var(--djdt-font-color);
     font-weight: bold;
 } /* Keyword */
 #djDebug .highlight .o {
-    color: #000;
+    color: var(--djdt-font-color);
 } /* Operator */
 #djDebug .highlight .n {
-    color: #000;
+    color: var(--djdt-font-color);
 } /* Name */
 #djDebug .highlight .mi {
-    color: #000;
+    color: var(--djdt-font-color);
     font-weight: bold;
 } /* Literal.Number.Integer */
 #djDebug .highlight .l {
-    color: #000;
+    color: var(--djdt-font-color);
 } /* Literal */
 #djDebug .highlight .x {
-    color: #000;
+    color: var(--djdt-font-color);
 } /* Other */
 #djDebug .highlight .p {
-    color: #000;
+    color: var(--djdt-font-color);
 } /* Punctuation */
 #djDebug .highlight .m {
-    color: #000;
+    color: var(--djdt-font-color);
     font-weight: bold;
 } /* Literal.Number */
 #djDebug .highlight .s {
-    color: #333;
+    color: var(--djdt-template-highlight-color);
 } /* Literal.String */
 #djDebug .highlight .w {
     color: #888888;
 } /* Text.Whitespace */
 #djDebug .highlight .il {
-    color: #000;
+    color: var(--djdt-font-color);
     font-weight: bold;
 } /* Literal.Number.Integer.Long */
 #djDebug .highlight .na {
-    color: #333;
+    color: var(--djdt-template-highlight-color);
 } /* Name.Attribute */
 #djDebug .highlight .nt {
-    color: #000;
+    color: var(--djdt-font-color);
     font-weight: bold;
 } /* Name.Tag */
 #djDebug .highlight .nv {
-    color: #333;
+    color: var(--djdt-template-highlight-color);
 } /* Name.Variable */
 #djDebug .highlight .s2 {
-    color: #333;
+    color: var(--djdt-template-highlight-color);
 } /* Literal.String.Double */
 #djDebug .highlight .cp {
-    color: #333;
+    color: var(--djdt-template-highlight-color);
 } /* Comment.Preproc */
 
 #djDebug svg.djDebugLineChart {
     width: 100%;
     height: 1.5em;
 }
 
@@ -591,32 +659,32 @@
 }
 
 #djDebug .djSQLDetailsDiv {
     margin-top: 0.8em;
 }
 
 #djDebug .djdt-stack span {
-    color: #000;
+    color: var(--djdt-stack-span-color);
     font-weight: bold;
 }
 #djDebug .djdt-stack span.djdt-path,
 #djDebug .djdt-stack pre.djdt-locals,
 #djDebug .djdt-stack pre.djdt-locals span {
-    color: #777;
+    color: var(--djdt-path-and-locals);
     font-weight: normal;
 }
 #djDebug .djdt-stack span.djdt-code {
     font-weight: normal;
 }
 #djDebug .djdt-stack pre.djdt-locals {
     margin: 0 27px 27px 27px;
 }
 #djDebug .djdt-raw {
     background-color: #fff;
-    border: 1px solid #ccc;
+    border: 1px solid var(--djdt-raw-border-color);
     margin-top: 0.8em;
     padding: 5px;
     white-space: pre-wrap;
 }
 
 #djDebug .djdt-width-20 {
     width: 20%;
@@ -627,15 +695,15 @@
 #djDebug .djdt-width-60 {
     width: 60%;
 }
 #djDebug .djdt-max-height-100 {
     max-height: 100%;
 }
 #djDebug .djdt-highlighted {
-    background-color: lightgrey;
+    background-color: var(--djdt--highlighted-background-color);
 }
 #djDebug tr.djdt-highlighted.djdt-profile-row {
     background-color: #ffc;
 }
 #djDebug tr.djdt-highlighted.djdt-profile-row:nth-child(2n + 1) {
     background-color: #dd9;
 }
@@ -650,7 +718,21 @@
 #djDebug .flash-new {
     animation: djdt-flash-new 1s;
 }
 
 .djdt-hidden {
     display: none;
 }
+
+#djDebug #djDebugToolbar a#djToggleThemeButton {
+    display: flex;
+    align-items: center;
+    cursor: pointer;
+}
+#djToggleThemeButton > svg {
+    margin-left: auto;
+}
+#djDebug[data-theme="light"] #djToggleThemeButton svg.theme-light,
+#djDebug[data-theme="dark"] #djToggleThemeButton svg.theme-dark,
+#djDebug[data-theme="auto"] #djToggleThemeButton svg.theme-auto {
+    display: block;
+}
```

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/history.js` & `django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/history.js`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/timer.js` & `django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/timer.js`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/toolbar.js` & `django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/toolbar.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 import {
     $$,
     ajax,
-    replaceToolbarState,
-    debounce
+    debounce,
+    replaceToolbarState
 } from "./utils.js";
 
 function onKeyDown(event) {
     if (event.keyCode === 27) {
         djdt.hideOneLevel();
     }
 }
@@ -219,14 +219,38 @@
             djdt.showToolbar();
         } else {
             djdt.hideToolbar();
         }
         if (djDebug.dataset.sidebarUrl !== undefined) {
             djdt.updateOnAjax();
         }
+
+        // Updates the theme using user settings
+        const userTheme = localStorage.getItem("djdt.user-theme");
+        if (userTheme !== null) {
+            djDebug.setAttribute("data-theme", userTheme);
+        }
+        // Adds the listener to the Theme Toggle Button
+        $$.on(djDebug, "click", "#djToggleThemeButton", function() {
+            switch (djDebug.getAttribute("data-theme")) {
+                case "auto":
+                    djDebug.setAttribute("data-theme", "light");
+                    localStorage.setItem("djdt.user-theme", "light");
+                    break;
+                case "light":
+                    djDebug.setAttribute("data-theme", "dark");
+                    localStorage.setItem("djdt.user-theme", "dark");
+                    break;
+                default:
+                    /* dark is the default */
+                    djDebug.setAttribute("data-theme", "auto");
+                    localStorage.setItem("djdt.user-theme", "auto");
+                    break;
+            }
+        });
     },
     hidePanels() {
         const djDebug = getDebugElement();
         $$.hide(document.getElementById("djDebugWindow"));
         djDebug.querySelectorAll(".djdt-panelContent").forEach(function(e) {
             $$.hide(e);
         });
```

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/static/debug_toolbar/js/utils.js` & `django_debug_toolbar-4.4.1/debug_toolbar/static/debug_toolbar/js/utils.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -73,15 +73,19 @@
 function ajax(url, init) {
     init = Object.assign({
         credentials: "same-origin"
     }, init);
     return fetch(url, init)
         .then(function(response) {
             if (response.ok) {
-                return response.json();
+                return response.json().catch(function(error) {
+                    return Promise.reject(
+                        new Error("The response  is a invalid Json object : " + error)
+                    );
+                });
             }
             return Promise.reject(
                 new Error(response.status + ": " + response.statusText)
             );
         })
         .catch(function(error) {
             const win = document.getElementById("djDebugWindow");
```

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/base.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/base.html`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,24 @@
      data-render-panel-url="{% url 'djdt:render_panel' %}"
      {% endif %}
      {% url 'djdt:history_sidebar' as history_url %}
      {% if history_url %}
      data-sidebar-url="{{ history_url }}"
      {% endif %}
      data-default-show="{% if toolbar.config.SHOW_COLLAPSED %}false{% else %}true{% endif %}"
-     {{ toolbar.config.ROOT_TAG_EXTRA_ATTRS|safe }}  data-update-on-fetch="{{ toolbar.config.UPDATE_ON_FETCH }}">
+     {{ toolbar.config.ROOT_TAG_EXTRA_ATTRS|safe }}  data-update-on-fetch="{{ toolbar.config.UPDATE_ON_FETCH }}"
+     data-theme="{{ toolbar.config.DEFAULT_THEME }}">
   <div class="djdt-hidden" id="djDebugToolbar">
     <ul id="djDebugPanelList">
       <li><a id="djHideToolBarButton" href="#" title="{% trans 'Hide toolbar' %}">{% trans "Hide" %} »</a></li>
+      <li>
+        <a id="djToggleThemeButton" href="#" title="{% trans 'Toggle Theme' %}">
+          {% trans "Toggle Theme" %} {% include "debug_toolbar/includes/theme_selector.html" %}
+        </a>
+      </li>
       {% for panel in toolbar.panels %}
         {% include "debug_toolbar/includes/panel_button.html" %}
       {% endfor %}
     </ul>
   </div>
   <div class="djdt-hidden" id="djDebugToolbarHandle">
     <div title="{% trans 'Show toolbar' %}" id="djShowToolBarButton">
```

#### html2text {}

```diff
@@ -3,14 +3,17 @@
 {% endblock %}
 % if not toolbar.should_render_panels %} data-store-id="{{ toolbar.store_id }}"
 data-render-panel-url="{% url 'djdt:render_panel' %}" {% endif %} {% url 'djdt:
 history_sidebar' as history_url %} {% if history_url %} data-sidebar-url="{
 { history_url }}" {% endif %} data-default-show="{% if
 toolbar.config.SHOW_COLLAPSED %}false{% else %}true{% endif %}" {
 { toolbar.config.ROOT_TAG_EXTRA_ATTRS|safe }} data-update-on-fetch="{
-{ toolbar.config.UPDATE_ON_FETCH }}">
+{ toolbar.config.UPDATE_ON_FETCH }}" data-theme="{
+{ toolbar.config.DEFAULT_THEME }}">
     * _{_%_ _t_r_a_n_s_ _"_H_i_d_e_"_ _%_}_ _Â_»
+    * _{_%_ _t_r_a_n_s_ _"_T_o_g_g_l_e_ _T_h_e_m_e_"_ _%_}_ _{_%_ _i_n_c_l_u_d_e_ _"_d_e_b_u_g___t_o_o_l_b_a_r_/_i_n_c_l_u_d_e_s_/
+      _t_h_e_m_e___s_e_l_e_c_t_o_r_._h_t_m_l_"_ _%_}
     * {% for panel in toolbar.panels %} {% include "debug_toolbar/includes/
       panel_button.html" %} {% endfor %}
 DJDT
 {% for panel in toolbar.panels %} {% include "debug_toolbar/includes/
 panel_content.html" %} {% endfor %}
```

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/redirect.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/redirect.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/includes/panel_button.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/includes/panel_button.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/includes/panel_content.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/includes/panel_content.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/cache.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/cache.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/headers.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/headers.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/history.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/history.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% load i18n %}{% load static %}
 <form method="get" action="{% url 'djdt:history_refresh' %}">
-    {{ refresh_form }}
+    {{ refresh_form.as_div }}
     <button class="refreshHistory">Refresh</button>
 </form>
 <table class="djdt-max-height-100">
     <thead>
         <tr>
             <th>{% trans "Time" %}</th>
             <th>{% trans "Method" %}</th>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 {% load i18n %}{% load static %}
-{{ refresh_form }} Refresh
+{{ refresh_form.as_div }} Refresh
 {{%% ttrraannss  {{%% ttrraannss    {{%% ttrraannss ""PPaatthh"" {{%% ttrraannss      {{%% ttrraannss    {{%% ttrraannss
 ""TTiimmee"" %%}} ""MMeetthhoodd"" %%}} %%}}              ""RReeqquueesstt      ""SSttaattuuss"" %%}} ""AAccttiioonn"" %%}}
                                       VVaarriiaabblleess"" %%}}
```

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/history_tr.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/history_tr.html`

 * *Files 4% similar despite different names*

```diff
@@ -39,12 +39,12 @@
         </div>
     </td>
     <td>
         <p>{{ store_context.toolbar.stats.HistoryPanel.status_code|escape }}</p>
     </td>
     <td class="djdt-actions">
         <form method="get" action="{% url 'djdt:history_sidebar' %}">
-            {{ store_context.form }}
+            {{ store_context.form.as_div }}
             <button data-store-id="{{ id }}" class="switchHistory">Switch</button>
         </form>
     </td>
 </tr>
```

#### html2text {}

```diff
@@ -4,8 +4,8 @@
 {{ store_context.toolbar.stats.HistoryPanel.request_url|truncatechars:
 100|escape }}
 +
 {{%% ttrraannss ""VVaarriiaabbllee"" %%}} {{%% ttrraannss ""VVaalluuee"" %%}}
 {{ key|pprint }}       {{ value|pprint }}
 No data
 {{ store_context.toolbar.stats.HistoryPanel.status_code|escape }}
-{{ store_context.form }} Switch
+{{ store_context.form.as_div }} Switch
```

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/profiling.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/profiling.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/request.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/request.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/request_variables.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/request_variables.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql.html`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
           <td class="djdt-time">
             {{ query.duration|floatformat:"2" }}
           </td>
           <td class="djdt-actions">
             {% if query.params %}
               {% if query.is_select %}
                 <form method="post">
-                  {{ query.form }}
+                  {{ query.form.as_div }}
                   <button formaction="{% url 'djdt:sql_select' %}" class="remoteCall">Sel</button>
                   <button formaction="{% url 'djdt:sql_explain' %}" class="remoteCall">Expl</button>
                   {% if query.vendor == 'mysql' %}
                     <button formaction="{% url 'djdt:sql_profile' %}" class="remoteCall">Prof</button>
                   {% endif %}
                 </form>
               {% endif %}
```

#### html2text {}

```diff
@@ -5,37 +5,37 @@
       endblocktrans %} {% if info.similar_count %} {% blocktrans with
       count=info.similar_count trimmed %} including {{ count }} similar {%
       endblocktrans %} {% if info.duplicate_count %} {% blocktrans with
       dupes=info.duplicate_count trimmed %} and {{ dupes }} duplicates {%
       endblocktrans %} {% endif %} {% endif %})
     * {% endfor %}
 {% if queries %}
- {{%% ttrraannss ""QQuueerryy"" %%}}           {{%% ttrraannss           {{%% ttrraannss ""TTiimmee ((mmss))"" %%}}     {{%% ttrraannss
-                               ""TTiimmeelliinnee"" %%}}                                  ""AAccttiioonn"" %%}}
+ {{%% ttrraannss ""QQuueerryy"" %%}}           {{%% ttrraannss           {{%% ttrraannss ""TTiimmee ((mmss))"" %%}}     {{%% ttrraannss ""AAccttiioonn""
+                               ""TTiimmeelliinnee"" %%}}                                  %%}}
    {{ query.sql|safe }}                                                       {% if
    {% if query.similar_count                                                  query.params %}
    %} {{%% bblloocckkttrraannss wwiitthh                                                      {% if
-   ccoouunntt==qquueerryy..ssiimmiillaarr__ccoouunntt   {% if                                          query.is_select
-   %%}}{{{{ ccoouunntt }}}} ssiimmiillaarr       query.starts_trans {                           %}
-   qquueerriieess..{{%% eennddbblloocckkttrraannss %%}} %} {% endif %} {%  {                           {{ query.form
- + {% endif %} {% if           if                 query.duration|floatformat: }} Sel Expl {%
-   query.duplicate_count %} {{%% query.ends_trans   "2" }}                      if query.vendor
-   bblloocckkttrraannss wwiitthh             %} {% endif %}                                 == 'mysql' %}
-   dduuppeess==qquueerryy..dduupplliiccaattee__ccoouunntt                                                Prof {% endif
-   %%}}DDuupplliiccaatteedd {{{{ dduuppeess }}}}                                                   %}
-   ttiimmeess..{{%% eennddbblloocckkttrraannss %%}}                                                  {% endif %} {%
-   {% endif %}                                                                endif %}
+   ccoouunntt==qquueerryy..ssiimmiillaarr__ccoouunntt                                                  query.is_select
+   %%}}{{{{ ccoouunntt }}}} ssiimmiillaarr       {% if                                          %}
+   qquueerriieess..{{%% eennddbblloocckkttrraannss %%}} query.starts_trans {                           {
+ + {% endif %} {% if           %} {% endif %} {%  {                           {
+   query.duplicate_count %} {{%% if                 query.duration|floatformat: query.form.as_div
+   bblloocckkttrraannss wwiitthh             query.ends_trans   "2" }}                      }} Sel Expl {% if
+   dduuppeess==qquueerryy..dduupplliiccaattee__ccoouunntt %} {% endif %}                                 query.vendor ==
+   %%}}DDuupplliiccaatteedd {{{{ dduuppeess }}}}                                                   'mysql' %} Prof
+   ttiimmeess..{{%% eennddbblloocckkttrraannss %%}}                                                  {% endif %}
+   {% endif %}                                                                {% endif %} {%
+                                                                              endif %}
    {{%% ttrraannss ""CCoonnnneeccttiioonn::"" %%}} {{ query.alias }}
    {% if query.iso_level %}
    {{%% ttrraannss ""IIssoollaattiioonn lleevveell::"" %%}} {{ query.iso_level }}
    {% endif %} {% if query.trans_status %}
    {{%% ttrraannss ""TTrraannssaaccttiioonn ssttaattuuss::"" %%}} {{ query.trans_status }}
    {% endif %} {% if query.stacktrace %}
    {{ query.stacktrace }}
    {% endif %} {% if query.template_info %}
-   {{ line.num }} % if line.highlight %}class="djdt-highlighted"{% endif %}>{{ line.content
-                  }}
+   {{ line.num }} % if line.highlight %}class="djdt-highlighted"{% endif %}>{{ line.content }}
    {{{{ qquueerryy..tteemmppllaattee__iinnffoo..nnaammee||ddeeffaauulltt::__((""((uunnkknnoowwnn))"")) }}}}
    {% endif %}
 {% else %}
 {% trans "No SQL queries were recorded during this request." %}
 {% endif %}
```

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql_explain.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql_profile.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/sql_select.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/sql_select.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/staticfiles.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/templates.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/templates.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/debug_toolbar/templates/debug_toolbar/panels/timer.html` & `django_debug_toolbar-4.4.1/debug_toolbar/templates/debug_toolbar/panels/timer.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/docs/Makefile` & `django_debug_toolbar-4.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/docs/changes.rst` & `django_debug_toolbar-4.4.1/docs/changes.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,55 @@
 Change log
 ==========
 
 Pending
 -------
 
+
+4.4.1 (2024-05-26)
+------------------
+
+* Pin metadata version to 2.2 to be compatible with Jazzband release
+  process.
+
+4.4.0 (2024-05-26)
+------------------
+
+* Raised the minimum Django version to 4.2.
+* Automatically support Docker rather than having the developer write a
+  workaround for ``INTERNAL_IPS``.
+* Display a better error message when the toolbar's requests
+  return invalid json.
+* Render forms with ``as_div`` to silence Django 5.0 deprecation warnings.
+* Stayed on top of pre-commit hook updates.
+* Added :doc:`architecture documentation <architecture>` to help
+  on-board new contributors.
+* Removed the static file path validation check in
+  :class:`StaticFilesPanel <debug_toolbar.panels.staticfiles.StaticFilesPanel>`
+  since that check is made redundant by a similar check in Django 4.0 and
+  later.
+* Deprecated the ``OBSERVE_REQUEST_CALLBACK`` setting and added check
+  ``debug_toolbar.W008`` to warn when it is present in
+  ``DEBUG_TOOLBAR_SETTINGS``.
+* Add a note on the profiling panel about using Python 3.12 and later
+  about needing ``--nothreading``
+* Added ``IS_RUNNING_TESTS`` setting to allow overriding the
+  ``debug_toolbar.E001`` check to avoid including the toolbar when running
+  tests.
+* Fixed the bug causing ``'djdt' is not a registered namespace`` and updated
+  docs to help in initial configuration while running tests.
+* Added a link in the installation docs to a more complete installation
+  example in the example app.
+* Added check to prevent the toolbar from being installed when tests
+  are running.
+* Added test to example app and command to run the example app's tests.
+* Implemented dark mode theme and button to toggle the theme,
+  introduced the ``DEFAULT_THEME`` setting which sets the default theme
+  to use.
+
 4.3.0 (2024-02-01)
 ------------------
 
 * Dropped support for Django 4.0.
 * Added Python 3.12 to test matrix.
 * Removed outdated third-party panels from the list.
 * Avoided the unnecessary work of recursively quoting SQL parameters.
```

### Comparing `django_debug_toolbar-4.3.0/docs/commands.rst` & `django_debug_toolbar-4.4.1/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/docs/conf.py` & `django_debug_toolbar-4.4.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "Django Debug Toolbar"
 copyright = "{}, Django Debug Toolbar developers and contributors"
 copyright = copyright.format(datetime.date.today().year)
 
 # The full version, including alpha/beta/rc tags
-release = "4.3.0"
+release = "4.4.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `django_debug_toolbar-4.3.0/docs/configuration.rst` & `django_debug_toolbar-4.4.1/docs/configuration.rst`

 * *Files 10% similar despite different names*

```diff
@@ -68,14 +68,25 @@
 * ``INSERT_BEFORE``
 
   Default: ``'</body>'``
 
   The toolbar searches for this string in the HTML and inserts itself just
   before.
 
+* ``IS_RUNNING_TESTS``
+
+  Default: ``"test" in sys.argv``
+
+  This setting whether the application is running tests. If this resolves to
+  ``True``, the toolbar will prevent you from running tests. This should only
+  be changed if your test command doesn't include ``test`` or if you wish to
+  test your application with the toolbar configured. If you do wish to test
+  your application with the toolbar configured, set this setting to
+  ``False``.
+
 .. _RENDER_PANELS:
 
 * ``RENDER_PANELS``
 
   Default: ``None``
 
   If set to ``False``, the debug toolbar will keep the contents of panels in
@@ -141,18 +152,22 @@
 
 .. _OBSERVE_REQUEST_CALLBACK:
 
 * ``OBSERVE_REQUEST_CALLBACK``
 
   Default: ``'debug_toolbar.toolbar.observe_request'``
 
+  .. note::
+
+     This setting is deprecated in favor of the ``UPDATE_ON_FETCH`` and
+     ``SHOW_TOOLBAR_CALLBACK`` settings.
+
   This is the dotted path to a function used for determining whether the
-  toolbar should update on AJAX requests or not. The default checks are that
-  the request doesn't originate from the toolbar itself, EG that
-  ``is_toolbar_request`` is false for a given request.
+  toolbar should update on AJAX requests or not. The default implementation
+  always returns ``True``.
 
 .. _TOOLBAR_LANGUAGE:
 
 * ``TOOLBAR_LANGUAGE``
 
   Default: ``None``
 
@@ -169,14 +184,22 @@
 
   Default: ``False``
 
   This controls whether the toolbar should update to the latest AJAX
   request when it occurs. This is especially useful when using htmx
   boosting or similar JavaScript techniques.
 
+.. _DEFAULT_THEME:
+
+* ``DEFAULT_THEME``
+
+  Default: ``"auto"``
+
+  This controls which theme will use the toolbar by default.
+
 Panel options
 ~~~~~~~~~~~~~
 
 * ``EXTRA_SIGNALS``
 
   Default: ``[]``
 
@@ -347,18 +370,18 @@
         'SHOW_COLLAPSED': True,
         # Panel options
         'SQL_WARNING_THRESHOLD': 100,   # milliseconds
     }
 
 Theming support
 ---------------
-The debug toolbar uses CSS variables to define fonts. This allows changing
-fonts without having to override many individual CSS rules. For example, if
-you preferred Roboto instead of the default list of fonts you could add a
-**debug_toolbar/base.html** template override to your project:
+The debug toolbar uses CSS variables to define fonts and colors. This allows
+changing fonts and colors without having to override many individual CSS rules.
+For example, if you preferred Roboto instead of the default list of fonts you
+could add a **debug_toolbar/base.html** template override to your project:
 
 .. code-block:: django
 
     {% extends 'debug_toolbar/base.html' %}
 
     {% block css %}{{ block.super }}
     <style>
```

### Comparing `django_debug_toolbar-4.3.0/docs/contributing.rst` & `django_debug_toolbar-4.4.1/docs/contributing.rst`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,20 @@
 For convenience, there's an alias for the second command::
 
     $ make example
 
 Look at ``example/settings.py`` for running the example with another database
 than SQLite.
 
+Architecture
+------------
+
+There is high-level information on how the Django Debug Toolbar is structured
+in the :doc:`architecture documentation <architecture>`.
+
 Tests
 -----
 
 Once you've set up a development environment as explained above, you can run
 the test suite for the versions of Django and Python installed in that
 environment using the SQLite database::
 
@@ -75,14 +81,20 @@
 
 or by setting the ``DJANGO_SELENIUM_TESTS`` environment variable::
 
     $ DJANGO_SELENIUM_TESTS=true make test
     $ DJANGO_SELENIUM_TESTS=true make coverage
     $ DJANGO_SELENIUM_TESTS=true tox
 
+Note that by default, ``tox`` enables the Selenium tests for a single test
+environment.  To run the entire ``tox`` test suite with all Selenium tests
+disabled, run the following::
+
+    $ DJANGO_SELENIUM_TESTS= tox
+
 To test via ``tox`` against other databases, you'll need to create the user,
 database and assign the proper permissions. For PostgreSQL in a ``psql``
 shell (note this allows the debug_toolbar user the permission to create
 databases)::
 
     psql> CREATE USER debug_toolbar WITH PASSWORD 'debug_toolbar';
     psql> ALTER USER debug_toolbar CREATEDB;
```

### Comparing `django_debug_toolbar-4.3.0/docs/installation.rst` & `django_debug_toolbar-4.4.1/docs/installation.rst`

 * *Files 5% similar despite different names*

```diff
@@ -77,14 +77,19 @@
 .. code-block:: python
 
     INSTALLED_APPS = [
         # ...
         "debug_toolbar",
         # ...
     ]
+.. note:: Check  out the configuration example in the
+   `example app
+   <https://github.com/jazzband/django-debug-toolbar/tree/main/example>`_
+   to learn how to set up the toolbar to function smoothly while running
+   your tests.
 
 4. Add the URLs
 ^^^^^^^^^^^^^^^
 
 Add django-debug-toolbar's URLs to your project's URLconf:
 
 .. code-block:: python
@@ -95,14 +100,15 @@
         # ...
         path("__debug__/", include("debug_toolbar.urls")),
     ]
 
 This example uses the ``__debug__`` prefix, but you can use any prefix that
 doesn't clash with your application's URLs.
 
+
 5. Add the Middleware
 ^^^^^^^^^^^^^^^^^^^^^
 
 The Debug Toolbar is mostly implemented in a middleware. Add it to your
 ``MIDDLEWARE`` setting:
 
 .. code-block:: python
@@ -141,20 +147,18 @@
 
 You can change the logic of determining whether or not the Debug Toolbar
 should be shown with the :ref:`SHOW_TOOLBAR_CALLBACK <SHOW_TOOLBAR_CALLBACK>`
 option.
 
 .. warning::
 
-    If using Docker the following will set your ``INTERNAL_IPS`` correctly in Debug mode::
-
-        if DEBUG:
-            import socket  # only if you haven't already imported this
-            hostname, _, ips = socket.gethostbyname_ex(socket.gethostname())
-            INTERNAL_IPS = [ip[: ip.rfind(".")] + ".1" for ip in ips] + ["127.0.0.1", "10.0.2.2"]
+    If using Docker, the toolbar will attempt to look up your host name
+    automatically and treat it as an allowable internal IP. If you're not
+    able to get the toolbar to work with your docker installation, review
+    the code in ``debug_toolbar.middleware.show_toolbar``.
 
 Troubleshooting
 ---------------
 
 On some platforms, the Django ``runserver`` command may use incorrect content
 types for static assets. To guess content types, Django relies on the
 :mod:`mimetypes` module from the Python standard library, which itself relies
```

### Comparing `django_debug_toolbar-4.3.0/docs/make.bat` & `django_debug_toolbar-4.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/docs/panels.rst` & `django_debug_toolbar-4.4.1/docs/panels.rst`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,18 @@
 .. class:: debug_toolbar.panels.profiling.ProfilingPanel
 
 Profiling information for the processing of the request.
 
 This panel is included but inactive by default. You can activate it by default
 with the ``DISABLE_PANELS`` configuration option.
 
+For version of Python 3.12 and later you need to use
+``python -m manage runserver --nothreading``
+Concurrent requests don't work with the profiling panel.
+
 The panel will include all function calls made by your project if you're using
 the setting ``settings.BASE_DIR`` to point to your project's root directory.
 If a function is in a file within that directory and does not include
 ``"/site-packages/"`` or ``"/dist-packages/"`` in the path, it will be
 included.
 
 Third-party panels
```

### Comparing `django_debug_toolbar-4.3.0/docs/tips.rst` & `django_debug_toolbar-4.4.1/docs/tips.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/example/README.rst` & `django_debug_toolbar-4.4.1/example/README.rst`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/example/django-debug-toolbar.png` & `django_debug_toolbar-4.4.1/example/django-debug-toolbar.png`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/example/example.db` & `django_debug_toolbar-4.4.1/example/example.db`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/example/screenshot.py` & `django_debug_toolbar-4.4.1/example/screenshot.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/example/settings.py` & `django_debug_toolbar-4.4.1/example/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Django settings for example project."""
 
 import os
+import sys
 
 BASE_DIR = os.path.dirname(os.path.dirname(__file__))
 
 
 # Quick-start development settings - unsuitable for production
 
+
 SECRET_KEY = "ABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890"
 
 DEBUG = True
 
 INTERNAL_IPS = ["127.0.0.1", "::1"]
 
 # Application definition
@@ -18,19 +20,17 @@
 INSTALLED_APPS = [
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.staticfiles",
-    "debug_toolbar",
 ]
 
 MIDDLEWARE = [
-    "debug_toolbar.middleware.DebugToolbarMiddleware",
     "django.middleware.security.SecurityMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.middleware.clickjacking.XFrameOptionsMiddleware",
@@ -57,15 +57,14 @@
     }
 ]
 
 USE_TZ = True
 
 WSGI_APPLICATION = "example.wsgi.application"
 
-DEBUG_TOOLBAR_CONFIG = {"ROOT_TAG_EXTRA_ATTRS": "data-turbo-permanent hx-preserve"}
 
 # Cache and database
 
 CACHES = {"default": {"BACKEND": "django.core.cache.backends.dummy.DummyCache"}}
 
 DATABASES = {
     "default": {
@@ -93,7 +92,22 @@
             "NAME": "debug_toolbar",
             "USER": "debug_toolbar",
             "PASSWORD": "debug_toolbar",
         }
     }
 
 STATICFILES_DIRS = [os.path.join(BASE_DIR, "example", "static")]
+
+
+# Only enable the toolbar when we're in debug mode and we're
+# not running tests. Django will change DEBUG to be False for
+# tests, so we can't rely on DEBUG alone.
+ENABLE_DEBUG_TOOLBAR = DEBUG and "test" not in sys.argv
+if ENABLE_DEBUG_TOOLBAR:
+    INSTALLED_APPS += [
+        "debug_toolbar",
+    ]
+    MIDDLEWARE += [
+        "debug_toolbar.middleware.DebugToolbarMiddleware",
+    ]
+    # Customize the config to support turbo and htmx boosting.
+    DEBUG_TOOLBAR_CONFIG = {"ROOT_TAG_EXTRA_ATTRS": "data-turbo-permanent hx-preserve"}
```

### Comparing `django_debug_toolbar-4.3.0/example/urls.py` & `django_debug_toolbar-4.4.1/example/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from django.conf import settings
 from django.contrib import admin
 from django.urls import include, path
 from django.views.generic import TemplateView
 
 from example.views import increment
 
 urlpatterns = [
@@ -29,9 +30,13 @@
         TemplateView.as_view(
             template_name="turbo/index.html", extra_context={"page_num": "2"}
         ),
         name="turbo2",
     ),
     path("admin/", admin.site.urls),
     path("ajax/increment", increment, name="ajax_increment"),
-    path("__debug__/", include("debug_toolbar.urls")),
 ]
+
+if settings.ENABLE_DEBUG_TOOLBAR:
+    urlpatterns += [
+        path("__debug__/", include("debug_toolbar.urls")),
+    ]
```

### Comparing `django_debug_toolbar-4.3.0/example/templates/index.html` & `django_debug_toolbar-4.4.1/example/templates/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,16 @@
   <body>
     <h1>Index of Tests</h1>
     {% cache 10 index_cache %}
       <ul>
         <li><a href="/jquery/">jQuery 3.3.1</a></li>
         <li><a href="/mootools/">MooTools 1.6.0</a></li>
         <li><a href="/prototype/">Prototype 1.7.3.0</a></li>
-        <li><a href="/turbo/">Hotwire Turbo</a></li>
-        <li><a href="/htmx/">htmx</a></li>
+        <li><a href="{% url 'turbo' %}">Hotwire Turbo</a></li>
+        <li><a href="{% url 'htmx' %}">htmx</a></li>
       </ul>
       <p><a href="/admin/">Django Admin</a></p>
     {% endcache %}
     <p>
       <span>Value </span>
       <span id="session-value">{{ request.session.value|default:0 }}</span>
       <button id="incrementFetch" data-url="{% url 'ajax_increment' %}" type="button">Increment via fetch</button>
```

### Comparing `django_debug_toolbar-4.3.0/example/templates/htmx/boost.html` & `django_debug_toolbar-4.4.1/example/templates/htmx/boost.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/example/templates/jquery/index.html` & `django_debug_toolbar-4.4.1/example/templates/jquery/index.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/example/templates/mootools/index.html` & `django_debug_toolbar-4.4.1/example/templates/mootools/index.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/example/templates/prototype/index.html` & `django_debug_toolbar-4.4.1/example/templates/prototype/index.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/example/templates/turbo/index.html` & `django_debug_toolbar-4.4.1/example/templates/turbo/index.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/base.py` & `django_debug_toolbar-4.4.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/models.py` & `django_debug_toolbar-4.4.1/tests/models.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/settings.py` & `django_debug_toolbar-4.4.1/tests/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,9 +122,11 @@
 
 DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
 
 # Debug Toolbar configuration
 
 DEBUG_TOOLBAR_CONFIG = {
     # Django's test client sets wsgi.multiprocess to True inappropriately
-    "RENDER_PANELS": False
+    "RENDER_PANELS": False,
+    # IS_RUNNING_TESTS must be False even though we're running tests because we're running the toolbar's own tests.
+    "IS_RUNNING_TESTS": False,
 }
```

### Comparing `django_debug_toolbar-4.3.0/tests/sync.py` & `django_debug_toolbar-4.4.1/tests/sync.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Taken from channels.db
 """
+
 from asgiref.sync import SyncToAsync
 from django.db import close_old_connections
 
 
 class DatabaseSyncToAsync(SyncToAsync):
     """
     SyncToAsync version that cleans up old database connections when it exits.
```

### Comparing `django_debug_toolbar-4.3.0/tests/test_checks.py` & `django_debug_toolbar-4.4.1/tests/test_checks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-import os
-import unittest
 from unittest.mock import patch
 
-import django
-from django.conf import settings
-from django.core.checks import Warning, run_checks
+from django.core.checks import Error, Warning, run_checks
 from django.test import SimpleTestCase, override_settings
 
-PATH_DOES_NOT_EXIST = os.path.join(settings.BASE_DIR, "tests", "invalid_static")
+from debug_toolbar import settings as dt_settings
+from debug_toolbar.apps import debug_toolbar_installed_when_running_tests_check
 
 
 class ChecksTestCase(SimpleTestCase):
     @override_settings(
         MIDDLEWARE=[
             "django.contrib.messages.middleware.MessageMiddleware",
             "django.contrib.sessions.middleware.SessionMiddleware",
@@ -88,43 +85,26 @@
                 "debug_toolbar is incompatible with MIDDLEWARE_CLASSES setting.",
                 hint="Use MIDDLEWARE instead of MIDDLEWARE_CLASSES",
                 id="debug_toolbar.W004",
             ),
             messages,
         )
 
-    @unittest.skipIf(django.VERSION >= (4,), "Django>=4 handles missing dirs itself.")
-    @override_settings(
-        STATICFILES_DIRS=[PATH_DOES_NOT_EXIST],
-    )
-    def test_panel_check_errors(self):
-        messages = run_checks()
-        self.assertEqual(
-            messages,
-            [
-                Warning(
-                    "debug_toolbar requires the STATICFILES_DIRS directories to exist.",
-                    hint="Running manage.py collectstatic may help uncover the issue.",
-                    id="debug_toolbar.staticfiles.W001",
-                )
-            ],
-        )
-
     @override_settings(DEBUG_TOOLBAR_PANELS=[])
     def test_panels_is_empty(self):
         errors = run_checks()
         self.assertEqual(
             errors,
             [
                 Warning(
                     "Setting DEBUG_TOOLBAR_PANELS is empty.",
                     hint="Set DEBUG_TOOLBAR_PANELS to a non-empty list in your "
                     "settings.py.",
                     id="debug_toolbar.W005",
-                )
+                ),
             ],
         )
 
     @override_settings(
         TEMPLATES=[
             {
                 "BACKEND": "django.template.backends.django.DjangoTemplates",
@@ -254,7 +234,52 @@
                     "\n"
                     "[HKEY_CLASSES_ROOT\\.js]\n"
                     '"Content Type"="application/javascript"',
                     id="debug_toolbar.W007",
                 )
             ],
         )
+
+    def test_debug_toolbar_installed_when_running_tests(self):
+        with self.settings(DEBUG=True):
+            # Update the config options because self.settings()
+            # would require redefining DEBUG_TOOLBAR_CONFIG entirely.
+            dt_settings.get_config()["IS_RUNNING_TESTS"] = True
+            errors = debug_toolbar_installed_when_running_tests_check(None)
+            self.assertEqual(len(errors), 0)
+
+            dt_settings.get_config()["IS_RUNNING_TESTS"] = False
+            errors = debug_toolbar_installed_when_running_tests_check(None)
+            self.assertEqual(len(errors), 0)
+        with self.settings(DEBUG=False):
+            dt_settings.get_config()["IS_RUNNING_TESTS"] = False
+            errors = debug_toolbar_installed_when_running_tests_check(None)
+            self.assertEqual(len(errors), 0)
+
+            dt_settings.get_config()["IS_RUNNING_TESTS"] = True
+            errors = debug_toolbar_installed_when_running_tests_check(None)
+            self.assertEqual(
+                errors,
+                [
+                    Error(
+                        "The Django Debug Toolbar can't be used with tests",
+                        hint="Django changes the DEBUG setting to False when running "
+                        "tests. By default the Django Debug Toolbar is installed because "
+                        "DEBUG is set to True. For most cases, you need to avoid installing "
+                        "the toolbar when running tests. If you feel this check is in error, "
+                        "you can set `DEBUG_TOOLBAR_CONFIG['IS_RUNNING_TESTS'] = False` to "
+                        "bypass this check.",
+                        id="debug_toolbar.E001",
+                    )
+                ],
+            )
+
+    @override_settings(
+        DEBUG_TOOLBAR_CONFIG={
+            "OBSERVE_REQUEST_CALLBACK": lambda request: False,
+            "IS_RUNNING_TESTS": False,
+        }
+    )
+    def test_observe_request_callback_specified(self):
+        errors = run_checks()
+        self.assertEqual(len(errors), 1)
+        self.assertEqual(errors[0].id, "debug_toolbar.W008")
```

### Comparing `django_debug_toolbar-4.3.0/tests/test_decorators.py` & `django_debug_toolbar-4.4.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/test_forms.py` & `django_debug_toolbar-4.4.1/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/test_integration.py` & `django_debug_toolbar-4.4.1/tests/test_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import re
 import time
 import unittest
+from unittest.mock import patch
 
 import html5lib
 from django.contrib.staticfiles.testing import StaticLiveServerTestCase
 from django.core import signing
 from django.core.cache import cache
 from django.db import connection
 from django.http import HttpResponse
@@ -62,14 +63,22 @@
         with self.settings(DEBUG=False):
             self.assertFalse(show_toolbar(self.request))
 
     def test_show_toolbar_INTERNAL_IPS(self):
         with self.settings(INTERNAL_IPS=[]):
             self.assertFalse(show_toolbar(self.request))
 
+    @patch("socket.gethostbyname", return_value="127.0.0.255")
+    def test_show_toolbar_docker(self, mocked_gethostbyname):
+        with self.settings(INTERNAL_IPS=[]):
+            # Is true because REMOTE_ADDR is 127.0.0.1 and the 255
+            # is shifted to be 1.
+            self.assertTrue(show_toolbar(self.request))
+        mocked_gethostbyname.assert_called_once_with("host.docker.internal")
+
     def test_should_render_panels_RENDER_PANELS(self):
         """
         The toolbar should force rendering panels on each request
         based on the RENDER_PANELS setting.
         """
         toolbar = DebugToolbar(self.request, self.get_response)
         self.assertFalse(toolbar.should_render_panels())
@@ -253,21 +262,23 @@
 
     def test_render_panel_checks_show_toolbar(self):
         url = "/__debug__/render_panel/"
         data = {"store_id": toolbar_store_id(), "panel_id": "VersionsPanel"}
 
         response = self.client.get(url, data)
         self.assertEqual(response.status_code, 200)
-        response = self.client.get(url, data, HTTP_X_REQUESTED_WITH="XMLHttpRequest")
+        response = self.client.get(
+            url, data, headers={"x-requested-with": "XMLHttpRequest"}
+        )
         self.assertEqual(response.status_code, 200)
         with self.settings(INTERNAL_IPS=[]):
             response = self.client.get(url, data)
             self.assertEqual(response.status_code, 404)
             response = self.client.get(
-                url, data, HTTP_X_REQUESTED_WITH="XMLHttpRequest"
+                url, data, headers={"x-requested-with": "XMLHttpRequest"}
             )
             self.assertEqual(response.status_code, 404)
 
     def test_middleware_render_toolbar_json(self):
         """Verify the toolbar is rendered and data is stored for a json request."""
         self.assertEqual(len(DebugToolbar._store), 0)
 
@@ -289,21 +300,23 @@
         data = {
             "template": template.template.name,
             "template_origin": signing.dumps(template.template.origin.name),
         }
 
         response = self.client.get(url, data)
         self.assertEqual(response.status_code, 200)
-        response = self.client.get(url, data, HTTP_X_REQUESTED_WITH="XMLHttpRequest")
+        response = self.client.get(
+            url, data, headers={"x-requested-with": "XMLHttpRequest"}
+        )
         self.assertEqual(response.status_code, 200)
         with self.settings(INTERNAL_IPS=[]):
             response = self.client.get(url, data)
             self.assertEqual(response.status_code, 404)
             response = self.client.get(
-                url, data, HTTP_X_REQUESTED_WITH="XMLHttpRequest"
+                url, data, headers={"x-requested-with": "XMLHttpRequest"}
             )
             self.assertEqual(response.status_code, 404)
 
     def test_template_source_errors(self):
         url = "/__debug__/template_source/"
 
         response = self.client.get(url, {})
@@ -335,21 +348,23 @@
                     "duration": "0",
                 }
             )
         }
 
         response = self.client.post(url, data)
         self.assertEqual(response.status_code, 200)
-        response = self.client.post(url, data, HTTP_X_REQUESTED_WITH="XMLHttpRequest")
+        response = self.client.post(
+            url, data, headers={"x-requested-with": "XMLHttpRequest"}
+        )
         self.assertEqual(response.status_code, 200)
         with self.settings(INTERNAL_IPS=[]):
             response = self.client.post(url, data)
             self.assertEqual(response.status_code, 404)
             response = self.client.post(
-                url, data, HTTP_X_REQUESTED_WITH="XMLHttpRequest"
+                url, data, headers={"x-requested-with": "XMLHttpRequest"}
             )
             self.assertEqual(response.status_code, 404)
 
     def test_sql_explain_checks_show_toolbar(self):
         url = "/__debug__/sql_explain/"
         data = {
             "signed": SignedDataForm.sign(
@@ -361,21 +376,23 @@
                     "duration": "0",
                 }
             )
         }
 
         response = self.client.post(url, data)
         self.assertEqual(response.status_code, 200)
-        response = self.client.post(url, data, HTTP_X_REQUESTED_WITH="XMLHttpRequest")
+        response = self.client.post(
+            url, data, headers={"x-requested-with": "XMLHttpRequest"}
+        )
         self.assertEqual(response.status_code, 200)
         with self.settings(INTERNAL_IPS=[]):
             response = self.client.post(url, data)
             self.assertEqual(response.status_code, 404)
             response = self.client.post(
-                url, data, HTTP_X_REQUESTED_WITH="XMLHttpRequest"
+                url, data, headers={"x-requested-with": "XMLHttpRequest"}
             )
             self.assertEqual(response.status_code, 404)
 
     @unittest.skipUnless(
         connection.vendor == "postgresql", "Test valid only on PostgreSQL"
     )
     def test_sql_explain_postgres_json_field(self):
@@ -393,21 +410,23 @@
                     "alias": "default",
                     "duration": "0",
                 }
             )
         }
         response = self.client.post(url, data)
         self.assertEqual(response.status_code, 200)
-        response = self.client.post(url, data, HTTP_X_REQUESTED_WITH="XMLHttpRequest")
+        response = self.client.post(
+            url, data, headers={"x-requested-with": "XMLHttpRequest"}
+        )
         self.assertEqual(response.status_code, 200)
         with self.settings(INTERNAL_IPS=[]):
             response = self.client.post(url, data)
             self.assertEqual(response.status_code, 404)
             response = self.client.post(
-                url, data, HTTP_X_REQUESTED_WITH="XMLHttpRequest"
+                url, data, headers={"x-requested-with": "XMLHttpRequest"}
             )
             self.assertEqual(response.status_code, 404)
 
     def test_sql_profile_checks_show_toolbar(self):
         url = "/__debug__/sql_profile/"
         data = {
             "signed": SignedDataForm.sign(
@@ -419,21 +438,23 @@
                     "duration": "0",
                 }
             )
         }
 
         response = self.client.post(url, data)
         self.assertEqual(response.status_code, 200)
-        response = self.client.post(url, data, HTTP_X_REQUESTED_WITH="XMLHttpRequest")
+        response = self.client.post(
+            url, data, headers={"x-requested-with": "XMLHttpRequest"}
+        )
         self.assertEqual(response.status_code, 200)
         with self.settings(INTERNAL_IPS=[]):
             response = self.client.post(url, data)
             self.assertEqual(response.status_code, 404)
             response = self.client.post(
-                url, data, HTTP_X_REQUESTED_WITH="XMLHttpRequest"
+                url, data, headers={"x-requested-with": "XMLHttpRequest"}
             )
             self.assertEqual(response.status_code, 404)
 
     @override_settings(DEBUG_TOOLBAR_CONFIG={"RENDER_PANELS": True})
     def test_render_panels_in_request(self):
         """
         Test that panels are are rendered during the request with
@@ -522,15 +543,15 @@
         # The key None (without quotes) exists in the list of template
         # variables.
         self.assertIn("None: &#x27;&#x27;", response.json()["content"])
 
 
 @unittest.skipIf(webdriver is None, "selenium isn't installed")
 @unittest.skipUnless(
-    "DJANGO_SELENIUM_TESTS" in os.environ, "selenium tests not requested"
+    os.environ.get("DJANGO_SELENIUM_TESTS"), "selenium tests not requested"
 )
 @override_settings(DEBUG=True)
 class DebugToolbarLiveTestCase(StaticLiveServerTestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         options = Options()
@@ -767,7 +788,35 @@
         # Need to wait until the ajax request is over and json_view is displayed on the toolbar
         time.sleep(2)
         history_panel = self.wait.until(
             lambda selenium: self.selenium.find_element(By.ID, "djdt-HistoryPanel")
         )
         self.assertNotIn("/ajax/", history_panel.text)
         self.assertIn("/json_view/", history_panel.text)
+
+    def test_theme_toggle(self):
+        self.get("/regular/basic/")
+
+        toolbar = self.selenium.find_element(By.ID, "djDebug")
+
+        # Check that the default theme is auto
+        self.assertEqual(toolbar.get_attribute("data-theme"), "auto")
+
+        # The theme toggle button is shown on the toolbar
+        toggle_button = self.selenium.find_element(By.ID, "djToggleThemeButton")
+        self.assertTrue(toggle_button.is_displayed())
+
+        # The theme changes when user clicks the button
+        toggle_button.click()
+        self.assertEqual(toolbar.get_attribute("data-theme"), "light")
+        toggle_button.click()
+        self.assertEqual(toolbar.get_attribute("data-theme"), "dark")
+        toggle_button.click()
+        self.assertEqual(toolbar.get_attribute("data-theme"), "auto")
+        # Switch back to light.
+        toggle_button.click()
+        self.assertEqual(toolbar.get_attribute("data-theme"), "light")
+
+        # Enter the page again to check that user settings is saved
+        self.get("/regular/basic/")
+        toolbar = self.selenium.find_element(By.ID, "djDebug")
+        self.assertEqual(toolbar.get_attribute("data-theme"), "light")
```

### Comparing `django_debug_toolbar-4.3.0/tests/test_utils.py` & `django_debug_toolbar-4.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/urls.py` & `django_debug_toolbar-4.4.1/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/views.py` & `django_debug_toolbar-4.4.1/tests/views.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/commands/test_debugsqlshell.py` & `django_debug_toolbar-4.4.1/tests/commands/test_debugsqlshell.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/panels/test_cache.py` & `django_debug_toolbar-4.4.1/tests/panels/test_cache.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/panels/test_custom.py` & `django_debug_toolbar-4.4.1/tests/panels/test_custom.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/panels/test_history.py` & `django_debug_toolbar-4.4.1/tests/panels/test_history.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/panels/test_profiling.py` & `django_debug_toolbar-4.4.1/tests/panels/test_profiling.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/panels/test_redirects.py` & `django_debug_toolbar-4.4.1/tests/panels/test_redirects.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/panels/test_request.py` & `django_debug_toolbar-4.4.1/tests/panels/test_request.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/panels/test_settings.py` & `django_debug_toolbar-4.4.1/tests/panels/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/panels/test_sql.py` & `django_debug_toolbar-4.4.1/tests/panels/test_sql.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/panels/test_staticfiles.py` & `django_debug_toolbar-4.4.1/tests/panels/test_staticfiles.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,12 @@
-import os
-import unittest
-
-import django
 from django.conf import settings
 from django.contrib.staticfiles import finders
-from django.test.utils import override_settings
 
 from ..base import BaseTestCase
 
-PATH_DOES_NOT_EXIST = os.path.join(settings.BASE_DIR, "tests", "invalid_static")
-
 
 class StaticFilesPanelTestCase(BaseTestCase):
     panel_id = "StaticFilesPanel"
 
     def test_default_case(self):
         response = self.panel.process_request(self.request)
         self.panel.generate_stats(self.request, response)
@@ -48,37 +41,7 @@
         self.panel.generate_stats(self.request, response)
         # ensure the panel renders correctly.
         content = self.panel.content
         self.assertIn(
             "django.contrib.staticfiles.finders.AppDirectoriesFinder", content
         )
         self.assertValidHTML(content)
-
-    @unittest.skipIf(django.VERSION >= (4,), "Django>=4 handles missing dirs itself.")
-    @override_settings(
-        STATICFILES_DIRS=[PATH_DOES_NOT_EXIST] + settings.STATICFILES_DIRS,
-        STATIC_ROOT=PATH_DOES_NOT_EXIST,
-    )
-    def test_finder_directory_does_not_exist(self):
-        """Misconfigure the static files settings and verify the toolbar runs.
-
-        The test case is that the STATIC_ROOT is in STATICFILES_DIRS and that
-        the directory of STATIC_ROOT does not exist.
-        """
-        response = self.panel.process_request(self.request)
-        self.panel.generate_stats(self.request, response)
-        content = self.panel.content
-        self.assertIn(
-            "django.contrib.staticfiles.finders.AppDirectoriesFinder", content
-        )
-        self.assertNotIn(
-            "django.contrib.staticfiles.finders.FileSystemFinder (2 files)", content
-        )
-        self.assertEqual(self.panel.num_used, 0)
-        self.assertNotEqual(self.panel.num_found, 0)
-        expected_apps = ["django.contrib.admin", "debug_toolbar"]
-        if settings.USE_GIS:
-            expected_apps = ["django.contrib.gis"] + expected_apps
-        self.assertEqual(self.panel.get_staticfiles_apps(), expected_apps)
-        self.assertEqual(
-            self.panel.get_staticfiles_dirs(), finders.FileSystemFinder().locations
-        )
```

### Comparing `django_debug_toolbar-4.3.0/tests/panels/test_template.py` & `django_debug_toolbar-4.4.1/tests/panels/test_template.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/panels/test_versions.py` & `django_debug_toolbar-4.4.1/tests/panels/test_versions.py`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/tests/templates/ajax/ajax.html` & `django_debug_toolbar-4.4.1/tests/templates/ajax/ajax.html`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/LICENSE` & `django_debug_toolbar-4.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_debug_toolbar-4.3.0/README.rst` & `django_debug_toolbar-4.4.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
 .. image:: https://raw.github.com/jazzband/django-debug-toolbar/main/example/django-debug-toolbar.png
    :alt: Django Debug Toolbar screenshot
 
 In addition to the built-in panels, a number of third-party panels are
 contributed by the community.
 
-The current stable version of the Debug Toolbar is 4.1.0. It works on
-Django ≥ 3.2.4.
+The current stable version of the Debug Toolbar is 4.4.1. It works on
+Django ≥ 4.2.0.
 
 The Debug Toolbar does not currently support `Django's asynchronous views
 <https://docs.djangoproject.com/en/dev/topics/async/>`_.
 
 Documentation, including installation and configuration instructions, is
 available at https://django-debug-toolbar.readthedocs.io/.
```

### Comparing `django_debug_toolbar-4.3.0/pyproject.toml` & `django_debug_toolbar-4.4.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -13,16 +13,14 @@
     { name = "Rob Hudson" },
 ]
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Web Environment",
   "Framework :: Django",
-  "Framework :: Django :: 3.2",
-  "Framework :: Django :: 4.1",
   "Framework :: Django :: 4.2",
   "Framework :: Django :: 5.0",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
@@ -33,28 +31,39 @@
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "Django>=3.2.4",
+  "Django>=4.2.9",
   "sqlparse>=0.2",
 ]
 [project.urls]
 Download = "https://pypi.org/project/django-debug-toolbar/"
 Homepage = "https://github.com/jazzband/django-debug-toolbar"
 
+[tool.hatch.build.targets.sdist]
+# Jazzband's release process is limited to 2.2 metadata
+core-metadata-version = "2.2"
+
 [tool.hatch.build.targets.wheel]
 packages = ["debug_toolbar"]
+# Jazzband's release process is limited to 2.2 metadata
+core-metadata-version = "2.2"
 
 [tool.hatch.version]
 path = "debug_toolbar/__init__.py"
 
 [tool.ruff]
+fix = true
+show-fixes = true
+target-version = "py38"
+
+[tool.ruff.lint]
 extend-select = [
   "ASYNC",  # flake8-async
   "B",      # flake8-bugbear
   "C4",     # flake8-comprehensions
   "C90",    # McCabe cyclomatic complexity
   "DJ",     # flake8-django
   "E",      # pycodestyle errors
@@ -71,25 +80,22 @@
   "W",      # pycodestyle warnings
 ]
 extend-ignore = [
   "B905",   # Allow zip() without strict=
   "E501",   # Ignore line length violations
   "SIM108", # Use ternary operator instead of if-else-block
 ]
-fix = true
-show-fixes = true
-target-version = "py38"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 combine-as-imports = true
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 16
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "*/migrat*/*" = [
   "N806",  # Allow using PascalCase model names in migrations
   "N999",  # Ignore the fact that migration files are invalid module names
 ]
 
 [tool.coverage.html]
 skip_covered = true
```

### Comparing `django_debug_toolbar-4.3.0/PKG-INFO` & `django_debug_toolbar-4.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.2
 Name: django-debug-toolbar
-Version: 4.3.0
+Version: 4.4.1
 Summary: A configurable set of panels that display various debug information about the current request/response.
 Project-URL: Download, https://pypi.org/project/django-debug-toolbar/
 Project-URL: Homepage, https://github.com/jazzband/django-debug-toolbar
 Author: Rob Hudson
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Requires-Dist: django>=3.2.4
+Requires-Dist: django>=4.2.9
 Requires-Dist: sqlparse>=0.2
 Description-Content-Type: text/x-rst
 
 =====================================
 Django Debug Toolbar |latest-version|
 =====================================
 
@@ -72,16 +70,16 @@
 
 .. image:: https://raw.github.com/jazzband/django-debug-toolbar/main/example/django-debug-toolbar.png
    :alt: Django Debug Toolbar screenshot
 
 In addition to the built-in panels, a number of third-party panels are
 contributed by the community.
 
-The current stable version of the Debug Toolbar is 4.1.0. It works on
-Django ≥ 3.2.4.
+The current stable version of the Debug Toolbar is 4.4.1. It works on
+Django ≥ 4.2.0.
 
 The Debug Toolbar does not currently support `Django's asynchronous views
 <https://docs.djangoproject.com/en/dev/topics/async/>`_.
 
 Documentation, including installation and configuration instructions, is
 available at https://django-debug-toolbar.readthedocs.io/.
```

