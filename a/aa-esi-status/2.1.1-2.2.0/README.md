# Comparing `tmp/aa_esi_status-2.1.1.tar.gz` & `tmp/aa_esi_status-2.2.0.tar.gz`

## Comparing `aa_esi_status-2.1.1.tar` & `aa_esi_status-2.2.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/__init__.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/apps.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/auth_hooks.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/constants.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/models.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/urls.py
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/.gitkeep
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/django.pot
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/pl_PL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/pl_PL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/migrations/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/static/esistatus/css/esistatus.css
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/static/esistatus/css/esistatus.min.css
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/static/esistatus/css/esistatus.min.css.map
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.js
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js.map
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/base.html
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/dashboard-widget.html
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/index.html
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/bundles/esistatus-dashboard-widget-js.html
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/partials/endpoints.html
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/partials/header/page-header.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templatetags/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templatetags/esistatus.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/tests/__init__.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/tests/test_access.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/tests/test_auth_hooks.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/tests/test_templatetags.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/tests/test_views.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/tests/utils.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/LICENSE
--rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/README.md
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    49019 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/__init__.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/apps.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/auth_hooks.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/constants.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/models.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/urls.py
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/.gitkeep
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/django.pot
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/migrations/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/static/esistatus/css/esistatus.css
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/static/esistatus/css/esistatus.min.css
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/static/esistatus/css/esistatus.min.css.map
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.js
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js.map
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/templates/esistatus/base.html
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/templates/esistatus/dashboard-widget.html
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/templates/esistatus/index.html
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/templates/esistatus/bundles/esistatus-dashboard-widget-js.html
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/templates/esistatus/partials/endpoints.html
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/templates/esistatus/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/templates/esistatus/partials/header/page-header.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/templatetags/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/templatetags/esistatus.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/tests/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/tests/test_access.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/tests/test_templatetags.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/tests/test_views.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/esistatus/tests/utils.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/LICENSE
+-rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/README.md
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    49017 2020-02-02 00:00:00.000000 aa_esi_status-2.2.0/PKG-INFO
```

### Comparing `aa_esi_status-2.1.1/esistatus/auth_hooks.py` & `aa_esi_status-2.2.0/esistatus/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/views.py` & `aa_esi_status-2.2.0/esistatus/views.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/locale/django.pot` & `aa_esi_status-2.2.0/esistatus/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,77 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
-#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-20 17:26+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
+"PO-Revision-Date: 2024-05-10 14:01+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-esi-status/it/>\n"
+"Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:5
 msgid "ESI Status"
 msgstr ""
 
 #: esistatus/apps.py:20
 #, python-brace-format
 msgid "ESI Status v{__version__}"
 msgstr ""
 
 #: esistatus/models.py:22
 msgid "Can access this app"
 msgstr ""
 
 #: esistatus/templates/esistatus/index.html:14
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:12
-msgid "Red Endpoints"
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:9
+msgid "Red endpoints"
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:17
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:15
-msgid "Yellow Endpoints"
+#: esistatus/templates/esistatus/index.html:15
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:10
+msgid ""
+"Red enpoints have a good chance of not responding at all or being completely "
+"unavailable."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:18
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:13
+msgid "Yellow endpoints"
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:19
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:14
+msgid "Yellow endpoints have a good chance of being slow or returning errors."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:22
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:17
+msgid "Green endpoints"
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:20
+#: esistatus/templates/esistatus/index.html:23
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
-msgid "Green Endpoints"
+msgid "Green endpoints are responding as expected."
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:25
+#: esistatus/templates/esistatus/index.html:28
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:24
 msgid "Detailed ESI status"
```

### Comparing `aa_esi_status-2.1.1/esistatus/locale/cs/LC_MESSAGES/django.mo` & `aa_esi_status-2.2.0/esistatus/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/locale/cs/LC_MESSAGES/django.po` & `aa_esi_status-2.2.0/esistatus/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,77 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-20 17:26+0100\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:01+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Czech <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-esi-status/cs/>\n"
-"Language: cs\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"Language-Team: Polish <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-esi-status/pl/>\n"
+"Language: pl_PL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
-"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2;\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:5
 msgid "ESI Status"
 msgstr ""
 
 #: esistatus/apps.py:20
 #, python-brace-format
 msgid "ESI Status v{__version__}"
 msgstr ""
 
 #: esistatus/models.py:22
 msgid "Can access this app"
 msgstr ""
 
 #: esistatus/templates/esistatus/index.html:14
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:12
-msgid "Red Endpoints"
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:9
+msgid "Red endpoints"
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:17
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:15
-msgid "Yellow Endpoints"
+#: esistatus/templates/esistatus/index.html:15
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:10
+msgid ""
+"Red enpoints have a good chance of not responding at all or being completely "
+"unavailable."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:18
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:13
+msgid "Yellow endpoints"
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:19
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:14
+msgid "Yellow endpoints have a good chance of being slow or returning errors."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:22
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:17
+msgid "Green endpoints"
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:20
+#: esistatus/templates/esistatus/index.html:23
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
-msgid "Green Endpoints"
+msgid "Green endpoints are responding as expected."
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:25
+#: esistatus/templates/esistatus/index.html:28
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:24
 msgid "Detailed ESI status"
@@ -66,11 +82,13 @@
 msgstr ""
 
 #: esistatus/templates/esistatus/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
+"Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
+"tłumaczenia?"
 
 #: esistatus/templates/esistatus/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr ""
+msgstr "Dołącz do naszego zespołu tłumaczy!"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aa_esi_status-2.1.1/esistatus/locale/de/LC_MESSAGES/django.mo` & `aa_esi_status-2.2.0/esistatus/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/locale/de/LC_MESSAGES/django.po` & `aa_esi_status-2.2.0/esistatus/locale/de/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -2,58 +2,81 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 19:54+0100\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:01+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: German <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-esi-status/de/>\n"
+"Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-esi-status/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:5
 msgid "ESI Status"
 msgstr "ESI Status"
 
 #: esistatus/apps.py:20
 #, python-brace-format
 msgid "ESI Status v{__version__}"
 msgstr "ESI Status v{__version__}"
 
 #: esistatus/models.py:22
 msgid "Can access this app"
 msgstr "Kann auf diese App zugreifen"
 
 #: esistatus/templates/esistatus/index.html:14
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:12
-msgid "Red Endpoints"
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:9
+#, fuzzy
+#| msgid "Red Endpoints"
+msgid "Red endpoints"
 msgstr "Rote Endpunkte"
 
-#: esistatus/templates/esistatus/index.html:17
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:15
-msgid "Yellow Endpoints"
+#: esistatus/templates/esistatus/index.html:15
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:10
+msgid ""
+"Red enpoints have a good chance of not responding at all or being completely "
+"unavailable."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:18
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:13
+#, fuzzy
+#| msgid "Yellow Endpoints"
+msgid "Yellow endpoints"
 msgstr "Gelbe Endpunkte"
 
-#: esistatus/templates/esistatus/index.html:20
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
-msgid "Green Endpoints"
+#: esistatus/templates/esistatus/index.html:19
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:14
+msgid "Yellow endpoints have a good chance of being slow or returning errors."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:22
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:17
+#, fuzzy
+#| msgid "Green Endpoints"
+msgid "Green endpoints"
 msgstr "Grüne Endpunkte"
 
-#: esistatus/templates/esistatus/index.html:25
+#: esistatus/templates/esistatus/index.html:23
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
+msgid "Green endpoints are responding as expected."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:28
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 "Der ESI-Status konnte nicht gelesen werden. Bitte versuche die Seite neu zu "
 "laden. Wenn das nicht hilft, ist es möglich, dass ESI vollständig "
 "unerreichbar ist."
```

### Comparing `aa_esi_status-2.1.1/esistatus/locale/es/LC_MESSAGES/django.mo` & `aa_esi_status-2.2.0/esistatus/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/locale/es/LC_MESSAGES/django.po` & `aa_esi_status-2.2.0/esistatus/locale/es/LC_MESSAGES/django.po`

 * *Files 15% similar despite different names*

```diff
@@ -3,59 +3,82 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023, 2024.
 # Geovanny David Morales De la cruz <moralesgeovanny1996@gmail.com>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 19:54+0100\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:01+0000\n"
-"Last-Translator: Geovanny David Morales De la cruz <moralesgeovanny1996@gmail"
-".com>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-esi-status/es/>\n"
+"Last-Translator: Geovanny David Morales De la cruz "
+"<moralesgeovanny1996@gmail.com>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-esi-status/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:5
 msgid "ESI Status"
 msgstr "Estado del ESI"
 
 #: esistatus/apps.py:20
 #, python-brace-format
 msgid "ESI Status v{__version__}"
 msgstr ""
 
 #: esistatus/models.py:22
 msgid "Can access this app"
 msgstr "Puede acceder esta aplicacion"
 
 #: esistatus/templates/esistatus/index.html:14
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:12
-msgid "Red Endpoints"
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:9
+#, fuzzy
+#| msgid "Red Endpoints"
+msgid "Red endpoints"
 msgstr "Endpoints en Rojo"
 
-#: esistatus/templates/esistatus/index.html:17
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:15
-msgid "Yellow Endpoints"
+#: esistatus/templates/esistatus/index.html:15
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:10
+msgid ""
+"Red enpoints have a good chance of not responding at all or being completely "
+"unavailable."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:18
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:13
+#, fuzzy
+#| msgid "Yellow Endpoints"
+msgid "Yellow endpoints"
 msgstr "Endpoints en Amarillo"
 
-#: esistatus/templates/esistatus/index.html:20
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
-msgid "Green Endpoints"
+#: esistatus/templates/esistatus/index.html:19
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:14
+msgid "Yellow endpoints have a good chance of being slow or returning errors."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:22
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:17
+#, fuzzy
+#| msgid "Green Endpoints"
+msgid "Green endpoints"
 msgstr "Endpoints en Verde"
 
-#: esistatus/templates/esistatus/index.html:25
+#: esistatus/templates/esistatus/index.html:23
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
+msgid "Green endpoints are responding as expected."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:28
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 "No se pudo leer el estado del ESI. Intenta recargar la página. Si esto no "
 "ayuda, es posible que el ESI se haya caído por completo."
```

### Comparing `aa_esi_status-2.1.1/esistatus/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_esi_status-2.2.0/esistatus/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/locale/fr_FR/LC_MESSAGES/django.po` & `aa_esi_status-2.2.0/esistatus/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 22% similar despite different names*

```diff
@@ -3,58 +3,81 @@
 # This file is distributed under the same license as the PACKAGE package.
 # erka Ekanon <M6musicT@hotmail.fr>, 2024.
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 19:54+0100\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:01+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-esi-status/fr/>\n"
+"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-esi-status/fr/>\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:5
 msgid "ESI Status"
 msgstr "Statut ESI"
 
 #: esistatus/apps.py:20
 #, python-brace-format
 msgid "ESI Status v{__version__}"
 msgstr "Statut ESI v{__version__}"
 
 #: esistatus/models.py:22
 msgid "Can access this app"
 msgstr "Peut accéder à cette application"
 
 #: esistatus/templates/esistatus/index.html:14
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:12
-msgid "Red Endpoints"
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:9
+#, fuzzy
+#| msgid "Red Endpoints"
+msgid "Red endpoints"
 msgstr "Points de terminaison rouges"
 
-#: esistatus/templates/esistatus/index.html:17
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:15
-msgid "Yellow Endpoints"
+#: esistatus/templates/esistatus/index.html:15
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:10
+msgid ""
+"Red enpoints have a good chance of not responding at all or being completely "
+"unavailable."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:18
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:13
+#, fuzzy
+#| msgid "Yellow Endpoints"
+msgid "Yellow endpoints"
 msgstr "Points de terminaison jaunes"
 
-#: esistatus/templates/esistatus/index.html:20
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
-msgid "Green Endpoints"
+#: esistatus/templates/esistatus/index.html:19
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:14
+msgid "Yellow endpoints have a good chance of being slow or returning errors."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:22
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:17
+#, fuzzy
+#| msgid "Green Endpoints"
+msgid "Green endpoints"
 msgstr "Points de terminaison verts"
 
-#: esistatus/templates/esistatus/index.html:25
+#: esistatus/templates/esistatus/index.html:23
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
+msgid "Green endpoints are responding as expected."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:28
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 "Impossible de lire le statut ESI. Veuillez essayer de recharger la page. Si "
 "cela ne résout pas le problème, il est possible que le statut ESI soit "
 "complètement en panne."
```

### Comparing `aa_esi_status-2.1.1/esistatus/locale/it_IT/LC_MESSAGES/django.po` & `aa_esi_status-2.2.0/esistatus/locale/nl/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -3,58 +3,75 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 19:54+0100\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:01+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-esi-status/it/>\n"
-"Language: it_IT\n"
+"Language-Team: Dutch <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-esi-status/nl/>\n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:5
 msgid "ESI Status"
 msgstr ""
 
 #: esistatus/apps.py:20
 #, python-brace-format
 msgid "ESI Status v{__version__}"
 msgstr ""
 
 #: esistatus/models.py:22
 msgid "Can access this app"
 msgstr ""
 
 #: esistatus/templates/esistatus/index.html:14
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:12
-msgid "Red Endpoints"
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:9
+msgid "Red endpoints"
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:17
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:15
-msgid "Yellow Endpoints"
+#: esistatus/templates/esistatus/index.html:15
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:10
+msgid ""
+"Red enpoints have a good chance of not responding at all or being completely "
+"unavailable."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:18
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:13
+msgid "Yellow endpoints"
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:19
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:14
+msgid "Yellow endpoints have a good chance of being slow or returning errors."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:22
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:17
+msgid "Green endpoints"
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:20
+#: esistatus/templates/esistatus/index.html:23
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
-msgid "Green Endpoints"
+msgid "Green endpoints are responding as expected."
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:25
+#: esistatus/templates/esistatus/index.html:28
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:24
 msgid "Detailed ESI status"
```

### Comparing `aa_esi_status-2.1.1/esistatus/locale/ja/LC_MESSAGES/django.po` & `aa_esi_status-2.2.0/esistatus/locale/sk/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -3,58 +3,76 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 19:54+0100\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:01+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-esi-status/ja/>\n"
-"Language: ja\n"
+"Language-Team: Slovak <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-esi-status/sk/>\n"
+"Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:5
 msgid "ESI Status"
 msgstr ""
 
 #: esistatus/apps.py:20
 #, python-brace-format
 msgid "ESI Status v{__version__}"
 msgstr ""
 
 #: esistatus/models.py:22
 msgid "Can access this app"
 msgstr ""
 
 #: esistatus/templates/esistatus/index.html:14
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:12
-msgid "Red Endpoints"
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:9
+msgid "Red endpoints"
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:17
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:15
-msgid "Yellow Endpoints"
+#: esistatus/templates/esistatus/index.html:15
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:10
+msgid ""
+"Red enpoints have a good chance of not responding at all or being completely "
+"unavailable."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:18
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:13
+msgid "Yellow endpoints"
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:19
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:14
+msgid "Yellow endpoints have a good chance of being slow or returning errors."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:22
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:17
+msgid "Green endpoints"
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:20
+#: esistatus/templates/esistatus/index.html:23
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
-msgid "Green Endpoints"
+msgid "Green endpoints are responding as expected."
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:25
+#: esistatus/templates/esistatus/index.html:28
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:24
 msgid "Detailed ESI status"
```

### Comparing `aa_esi_status-2.1.1/esistatus/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_esi_status-2.2.0/esistatus/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/locale/ko_KR/LC_MESSAGES/django.po` & `aa_esi_status-2.2.0/esistatus/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 22% similar despite different names*

```diff
@@ -4,64 +4,87 @@
 # Author50CO <tkddlschry@gmail.com>, 2023, 2024.
 # Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 # Mind of the Raven <okanieva@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 19:54+0100\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:01+0000\n"
 "Last-Translator: Mind of the Raven <okanieva@gmail.com>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-esi-status/ko/>\n"
+"Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-esi-status/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:5
 msgid "ESI Status"
 msgstr "ESI 상태"
 
 #: esistatus/apps.py:20
 #, python-brace-format
 msgid "ESI Status v{__version__}"
 msgstr "ESI 상태 v{__version__}"
 
 #: esistatus/models.py:22
 msgid "Can access this app"
 msgstr "서비스에 접근할 수 있습니다"
 
 #: esistatus/templates/esistatus/index.html:14
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:12
-msgid "Red Endpoints"
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:9
+#, fuzzy
+#| msgid "Red Endpoints"
+msgid "Red endpoints"
 msgstr "적색 엔드포인트"
 
-#: esistatus/templates/esistatus/index.html:17
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:15
-msgid "Yellow Endpoints"
+#: esistatus/templates/esistatus/index.html:15
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:10
+msgid ""
+"Red enpoints have a good chance of not responding at all or being completely "
+"unavailable."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:18
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:13
+#, fuzzy
+#| msgid "Yellow Endpoints"
+msgid "Yellow endpoints"
 msgstr "황색 엔드포인트"
 
-#: esistatus/templates/esistatus/index.html:20
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
-msgid "Green Endpoints"
+#: esistatus/templates/esistatus/index.html:19
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:14
+msgid "Yellow endpoints have a good chance of being slow or returning errors."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:22
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:17
+#, fuzzy
+#| msgid "Green Endpoints"
+msgid "Green endpoints"
 msgstr "청색 엔드포인트"
 
-#: esistatus/templates/esistatus/index.html:25
+#: esistatus/templates/esistatus/index.html:23
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
+msgid "Green endpoints are responding as expected."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:28
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
-"ESI 상태를 읽을 수 없습니다. 페이지를 새로고침 해 보세요. 그래도 읽어올 수 "
-"없는 경우, ESI가 완전히 다운됐을 수도 있습니다."
+"ESI 상태를 읽을 수 없습니다. 페이지를 새로고침 해 보세요. 그래도 읽어올 수 없"
+"는 경우, ESI가 완전히 다운됐을 수도 있습니다."
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:24
 msgid "Detailed ESI status"
 msgstr "ESI 상태"
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:26
 msgid "EVE Online status"
```

### Comparing `aa_esi_status-2.1.1/esistatus/locale/nl/LC_MESSAGES/django.po` & `aa_esi_status-2.2.0/esistatus/locale/cs/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -3,58 +3,76 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-20 17:26+0100\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:01+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Dutch <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-esi-status/nl/>\n"
-"Language: nl\n"
+"Language-Team: Czech <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-esi-status/cs/>\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:5
 msgid "ESI Status"
 msgstr ""
 
 #: esistatus/apps.py:20
 #, python-brace-format
 msgid "ESI Status v{__version__}"
 msgstr ""
 
 #: esistatus/models.py:22
 msgid "Can access this app"
 msgstr ""
 
 #: esistatus/templates/esistatus/index.html:14
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:12
-msgid "Red Endpoints"
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:9
+msgid "Red endpoints"
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:17
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:15
-msgid "Yellow Endpoints"
+#: esistatus/templates/esistatus/index.html:15
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:10
+msgid ""
+"Red enpoints have a good chance of not responding at all or being completely "
+"unavailable."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:18
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:13
+msgid "Yellow endpoints"
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:19
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:14
+msgid "Yellow endpoints have a good chance of being slow or returning errors."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:22
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:17
+msgid "Green endpoints"
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:20
+#: esistatus/templates/esistatus/index.html:23
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
-msgid "Green Endpoints"
+msgid "Green endpoints are responding as expected."
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:25
+#: esistatus/templates/esistatus/index.html:28
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:24
 msgid "Detailed ESI status"
```

### Comparing `aa_esi_status-2.1.1/esistatus/locale/pl_PL/LC_MESSAGES/django.mo` & `aa_esi_status-2.2.0/esistatus/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/locale/pl_PL/LC_MESSAGES/django.po` & `aa_esi_status-2.2.0/esistatus/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,101 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
+# Faer Yili <yilifaer@gmail.com>, 2024.
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
+# Dehao Wu <wudehao2000@163.com>, 2024.
+# SAM_FPS <sam_fps@163.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-20 17:26+0100\n"
-"PO-Revision-Date: 2024-05-10 14:01+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Polish <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-esi-status/pl/>\n"
-"Language: pl_PL\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
+"PO-Revision-Date: 2024-05-15 09:21+0000\n"
+"Last-Translator: SAM_FPS <sam_fps@163.com>\n"
+"Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-esi-status/zh_Hans/>\n"
+"Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
-"|| n%100>=20) ? 1 : 2;\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:5
 msgid "ESI Status"
-msgstr ""
+msgstr "esi状态"
 
 #: esistatus/apps.py:20
 #, python-brace-format
 msgid "ESI Status v{__version__}"
-msgstr ""
+msgstr "esi 状态 {__version__}"
 
 #: esistatus/models.py:22
 msgid "Can access this app"
-msgstr ""
+msgstr "能够访问此应用程序"
 
 #: esistatus/templates/esistatus/index.html:14
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:12
-msgid "Red Endpoints"
-msgstr ""
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:9
+#, fuzzy
+#| msgid "Red Endpoints"
+msgid "Red endpoints"
+msgstr "红色终端"
 
-#: esistatus/templates/esistatus/index.html:17
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:15
-msgid "Yellow Endpoints"
+#: esistatus/templates/esistatus/index.html:15
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:10
+msgid ""
+"Red enpoints have a good chance of not responding at all or being completely "
+"unavailable."
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:20
+#: esistatus/templates/esistatus/index.html:18
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:13
+#, fuzzy
+#| msgid "Yellow Endpoints"
+msgid "Yellow endpoints"
+msgstr "黄色终端"
+
+#: esistatus/templates/esistatus/index.html:19
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:14
+msgid "Yellow endpoints have a good chance of being slow or returning errors."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:22
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:17
+#, fuzzy
+#| msgid "Green Endpoints"
+msgid "Green endpoints"
+msgstr "绿色终端"
+
+#: esistatus/templates/esistatus/index.html:23
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
-msgid "Green Endpoints"
+msgid "Green endpoints are responding as expected."
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:25
+#: esistatus/templates/esistatus/index.html:28
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
+"无法读取 ESI 状态。 请尝试重新加载页面。 如果这没有解决，ESI 可能完全失效了。"
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:24
 msgid "Detailed ESI status"
-msgstr ""
+msgstr "ESI详细状态"
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:26
 msgid "EVE Online status"
-msgstr ""
+msgstr "EVE Online状态"
 
 #: esistatus/templates/esistatus/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr ""
-"Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
-"tłumaczenia?"
+msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
 
 #: esistatus/templates/esistatus/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "Dołącz do naszego zespołu tłumaczy!"
+msgstr "加入我们的翻译团队吧！"
```

### Comparing `aa_esi_status-2.1.1/esistatus/locale/ru/LC_MESSAGES/django.mo` & `aa_esi_status-2.2.0/esistatus/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/locale/sk/LC_MESSAGES/django.mo` & `aa_esi_status-2.2.0/esistatus/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/locale/sk/LC_MESSAGES/django.po` & `aa_esi_status-2.2.0/esistatus/locale/django.pot`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,75 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-20 17:26+0100\n"
-"PO-Revision-Date: 2024-05-10 14:01+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Slovak <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-esi-status/sk/>\n"
-"Language: sk\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
-">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
-"X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:5
 msgid "ESI Status"
 msgstr ""
 
 #: esistatus/apps.py:20
 #, python-brace-format
 msgid "ESI Status v{__version__}"
 msgstr ""
 
 #: esistatus/models.py:22
 msgid "Can access this app"
 msgstr ""
 
 #: esistatus/templates/esistatus/index.html:14
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:12
-msgid "Red Endpoints"
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:9
+msgid "Red endpoints"
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:17
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:15
-msgid "Yellow Endpoints"
+#: esistatus/templates/esistatus/index.html:15
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:10
+msgid ""
+"Red enpoints have a good chance of not responding at all or being completely "
+"unavailable."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:18
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:13
+msgid "Yellow endpoints"
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:19
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:14
+msgid "Yellow endpoints have a good chance of being slow or returning errors."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:22
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:17
+msgid "Green endpoints"
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:20
+#: esistatus/templates/esistatus/index.html:23
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
-msgid "Green Endpoints"
+msgid "Green endpoints are responding as expected."
 msgstr ""
 
-#: esistatus/templates/esistatus/index.html:25
+#: esistatus/templates/esistatus/index.html:28
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:24
 msgid "Detailed ESI status"
```

### Comparing `aa_esi_status-2.1.1/esistatus/locale/uk/LC_MESSAGES/django.mo` & `aa_esi_status-2.2.0/esistatus/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/locale/uk/LC_MESSAGES/django.po` & `aa_esi_status-2.2.0/esistatus/locale/uk/LC_MESSAGES/django.po`

 * *Files 13% similar despite different names*

```diff
@@ -2,59 +2,82 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 19:54+0100\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
 "PO-Revision-Date: 2024-05-10 14:01+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-esi-status/uk/>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-esi-status/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:5
 msgid "ESI Status"
 msgstr "Статус ESI"
 
 #: esistatus/apps.py:20
 #, python-brace-format
 msgid "ESI Status v{__version__}"
 msgstr ""
 
 #: esistatus/models.py:22
 msgid "Can access this app"
 msgstr ""
 
 #: esistatus/templates/esistatus/index.html:14
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:12
-msgid "Red Endpoints"
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:9
+#, fuzzy
+#| msgid "Red Endpoints"
+msgid "Red endpoints"
 msgstr "Червоні кінцеві точки"
 
-#: esistatus/templates/esistatus/index.html:17
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:15
-msgid "Yellow Endpoints"
+#: esistatus/templates/esistatus/index.html:15
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:10
+msgid ""
+"Red enpoints have a good chance of not responding at all or being completely "
+"unavailable."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:18
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:13
+#, fuzzy
+#| msgid "Yellow Endpoints"
+msgid "Yellow endpoints"
 msgstr "Жовті кінцеві точки"
 
-#: esistatus/templates/esistatus/index.html:20
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
-msgid "Green Endpoints"
+#: esistatus/templates/esistatus/index.html:19
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:14
+msgid "Yellow endpoints have a good chance of being slow or returning errors."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:22
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:17
+#, fuzzy
+#| msgid "Green Endpoints"
+msgid "Green endpoints"
 msgstr "Зелені кінцеві точки"
 
-#: esistatus/templates/esistatus/index.html:25
+#: esistatus/templates/esistatus/index.html:23
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
+msgid "Green endpoints are responding as expected."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:28
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 "Не вдалося прочитати статус ESI. Будь ласка, спробуйте перезавантажити "
 "сторінку. Якщо це не допомогло, цілком можливо, що ESI може повністю вийти з "
 "ладу."
```

### Comparing `aa_esi_status-2.1.1/esistatus/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_esi_status-2.2.0/esistatus/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_esi_status-2.2.0/esistatus/locale/ru/LC_MESSAGES/django.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,105 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Faer Yili <yilifaer@gmail.com>, 2024.
-# Peter Pfeufer <info@ppfeufer.de>, 2024.
-# Dehao Wu <wudehao2000@163.com>, 2024.
-# SAM_FPS <sam_fps@163.com>, 2024.
+# Nikolay <nick.postnikov@gmail.com>, 2023, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-15 19:54+0100\n"
-"PO-Revision-Date: 2024-05-15 09:21+0000\n"
-"Last-Translator: SAM_FPS <sam_fps@163.com>\n"
-"Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-esi-status/zh_Hans/>\n"
-"Language: zh_Hans\n"
+"POT-Creation-Date: 2024-05-27 07:15+0200\n"
+"PO-Revision-Date: 2024-05-10 14:01+0000\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-esi-status/ru/>\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
+"n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:5
 msgid "ESI Status"
-msgstr "esi状态"
+msgstr "Статус ESI"
 
 #: esistatus/apps.py:20
 #, python-brace-format
 msgid "ESI Status v{__version__}"
-msgstr "esi 状态 {__version__}"
+msgstr "Статус ESI v{__version__}"
 
 #: esistatus/models.py:22
 msgid "Can access this app"
-msgstr "能够访问此应用程序"
+msgstr "Имеет доступ к приложению"
 
 #: esistatus/templates/esistatus/index.html:14
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:12
-msgid "Red Endpoints"
-msgstr "红色终端"
-
-#: esistatus/templates/esistatus/index.html:17
-#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:15
-msgid "Yellow Endpoints"
-msgstr "黄色终端"
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:9
+#, fuzzy
+#| msgid "Red Endpoints"
+msgid "Red endpoints"
+msgstr "Красные конечные точки"
 
-#: esistatus/templates/esistatus/index.html:20
+#: esistatus/templates/esistatus/index.html:15
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:10
+msgid ""
+"Red enpoints have a good chance of not responding at all or being completely "
+"unavailable."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:18
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:13
+#, fuzzy
+#| msgid "Yellow Endpoints"
+msgid "Yellow endpoints"
+msgstr "Желтые конечные точки"
+
+#: esistatus/templates/esistatus/index.html:19
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:14
+msgid "Yellow endpoints have a good chance of being slow or returning errors."
+msgstr ""
+
+#: esistatus/templates/esistatus/index.html:22
+#: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:17
+#, fuzzy
+#| msgid "Green Endpoints"
+msgid "Green endpoints"
+msgstr "Зеленые конечные точки"
+
+#: esistatus/templates/esistatus/index.html:23
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
-msgid "Green Endpoints"
-msgstr "绿色终端"
+msgid "Green endpoints are responding as expected."
+msgstr ""
 
-#: esistatus/templates/esistatus/index.html:25
+#: esistatus/templates/esistatus/index.html:28
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
-msgstr "无法读取 ESI 状态。 请尝试重新加载页面。 如果这没有解决，ESI 可能完全失效了。"
+msgstr ""
+"Невозможно прочитать статус ESI. Пожалуйста, перегрузите страницу. Если "
+"проблема сохраниться, возможно ESI полностью неработоспособна."
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:24
+#, fuzzy
+#| msgid "ESI Status"
 msgid "Detailed ESI status"
-msgstr "ESI详细状态"
+msgstr "Статус ESI"
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:26
 msgid "EVE Online status"
-msgstr "EVE Online状态"
+msgstr ""
 
 #: esistatus/templates/esistatus/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
+msgstr ""
+"Вы хотите помочь перевести это приложение на ваш язык или улучшить текущий "
+"перевод?"
 
 #: esistatus/templates/esistatus/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "加入我们的翻译团队吧！"
+msgstr "Присоединяйтесь к нашей команде переводчиков!"
```

### Comparing `aa_esi_status-2.1.1/esistatus/migrations/0001_initial.py` & `aa_esi_status-2.2.0/esistatus/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.js` & `aa_esi_status-2.2.0/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -28,14 +28,20 @@
                 elementEsiStatusDashboardWidget.innerHTML = responseText;
 
                 if (!elementEsiStatusDashboardWidget.classList.contains('show')) {
                     const bsCollapse = new bootstrap.Collapse(elementEsiStatusDashboardWidget, { // eslint-disable-line no-unused-vars
                         show: true
                     });
                 }
+
+                // Initialize Bootstrap tooltips
+                [].slice.call(document.querySelectorAll('[data-bs-tooltip="aa-esi-status"]'))
+                    .map((tooltipTriggerEl) => {
+                        return new bootstrap.Tooltip(tooltipTriggerEl);
+                    });
             }
         })
         .catch((error) => {
             console.log(error);
         });
 };
```

### Comparing `aa_esi_status-2.1.1/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js` & `aa_esi_status-2.2.0/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,20 @@
 const elementEsiStatusDashboardWidget = document.getElementById("esi-status-dashboard-panel"),
     esiStatusDashboardWidget = () => {
         "use strict";
         fetch(esistatusSettings.dashboardWidget.ajaxUrl).then(t => {
             if (t.ok) return t.text();
             throw new Error("Something went wrong")
         }).then(t => {
-            if ("" !== t && (console.log("ESI Status Dashboard Widget: Updating widget content"), elementEsiStatusDashboardWidget.innerHTML = t, !elementEsiStatusDashboardWidget.classList.contains("show"))) new bootstrap.Collapse(elementEsiStatusDashboardWidget, {
-                show: !0
-            })
+            if ("" !== t) {
+                if (console.log("ESI Status Dashboard Widget: Updating widget content"), elementEsiStatusDashboardWidget.innerHTML = t, !elementEsiStatusDashboardWidget.classList.contains("show")) new bootstrap.Collapse(elementEsiStatusDashboardWidget, {
+                    show: !0
+                });
+                [].slice.call(document.querySelectorAll('[data-bs-tooltip="aa-esi-status"]')).map(t => new bootstrap.Tooltip(t))
+            }
         }).catch(t => {
             console.log(t)
         })
     };
 let esiStatusDashboardWidgetInterval;
 const activateEsiStatusDashboardWidget = () => {
         "use strict";
```

### Comparing `aa_esi_status-2.1.1/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js.map` & `aa_esi_status-2.2.0/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js.map`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8552631578947368%*

 * *Differences: {"'mappings'": "'AAQA,MAAMA,gCAAkCC,SAASC,eAAe,4BAA4B,EAKtFC,yBAA2B,KAC7B,aAEAC,MAAMC,kBAAkBC,gBAAgBC,OAAO,EAC1CC,KAAK,IACF,GAAIC,EAASC,GACT,OAAOD,EAASE,KAAK,EAEzB,MAAM,IAAIC,MAAM,sBAAsB,CAC1C,CAAC,EACAJ,KAAK,IACF,GAAqB,KAAjBK,EAAqB,CAKrB,GAJAC,QAAQC,IAAI,sDAAsD,EAElEf,gCAAgCgB,UAAYH,EAExC,CAACb,gCAAgCiB,UAAUC,SAAS,MAAM,EACvC,IAAIC,UAAUC,SAASpB,gCAAiC,CACvEqB,KAAM,CAAA,CACV,CAAC,EAIL,GAAGC,MAAMC,KAAKtB,SAASuB,iBAAiB,mCAAmC,CAAC,EACvEC,IAAI,GACM,IAAIN,UAAUO,QAAQC,CAAgB,CAChD,CACT,CACJ,CAAC,EACAC,MAAM,IACHd,Q […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "mappings": "AAQA,MAAMA,gCAAkCC,SAASC,eAAe,4BAA4B,EAKtFC,yBAA2B,KAC7B,aAEAC,MAAMC,kBAAkBC,gBAAgBC,OAAO,EAC1CC,KAAK,IACF,GAAIC,EAASC,GACT,OAAOD,EAASE,KAAK,EAEzB,MAAM,IAAIC,MAAM,sBAAsB,CAC1C,CAAC,EACAJ,KAAK,IACF,GAAqB,KAAjBK,IACAC,QAAQC,IAAI,sDAAsD,EAElEf,gCAAgCgB,UAAYH,EAExC,CAACb,gCAAgCiB,UAAUC,SAAS,MAAM,GACvC,IAAIC,UAAUC,SAASpB,gCAAiC,CACvEqB,KAAM,CAAA,CACV,CAAC,CAGb,CAAC,EACAC,MAAM,IACHR,QAAQC,IAAIQ,CAAK,CACrB,CAAC,CACT,EAEAC,IAAIC,iCAKJ,MAAMC,iCAAmC,KACrC,aAEAvB,yBAAyB,EAEzBW,QAAQC,IAAI,2DAA2D,EAEvEU,iCAAmCE,YAC/BxB,yBAA0B,GAC9B,CACJ,EAKMyB,mCAAqC,KACvC,aAEgD,KAAA,IAArCH,mCACPX,QAAQC,IAAI,6DAA6D,EAEzEc,cAAcJ,gCAAgC,EAEtD,EAKAK,OAAOC,iBAAiB,QAAS,KAC7B,aAEAL,iCAAiC,CACrC,CAAC,EAKDI,OAAOC,iBAAiB,OAAQ,KAC5B,aAEAH,mCAAmC,CACvC,CAAC,EAKDF,iCAAiC",
+    "mappings": "AAQA,MAAMA,gCAAkCC,SAASC,eAAe,4BAA4B,EAKtFC,yBAA2B,KAC7B,aAEAC,MAAMC,kBAAkBC,gBAAgBC,OAAO,EAC1CC,KAAK,IACF,GAAIC,EAASC,GACT,OAAOD,EAASE,KAAK,EAEzB,MAAM,IAAIC,MAAM,sBAAsB,CAC1C,CAAC,EACAJ,KAAK,IACF,GAAqB,KAAjBK,EAAqB,CAKrB,GAJAC,QAAQC,IAAI,sDAAsD,EAElEf,gCAAgCgB,UAAYH,EAExC,CAACb,gCAAgCiB,UAAUC,SAAS,MAAM,EACvC,IAAIC,UAAUC,SAASpB,gCAAiC,CACvEqB,KAAM,CAAA,CACV,CAAC,EAIL,GAAGC,MAAMC,KAAKtB,SAASuB,iBAAiB,mCAAmC,CAAC,EACvEC,IAAI,GACM,IAAIN,UAAUO,QAAQC,CAAgB,CAChD,CACT,CACJ,CAAC,EACAC,MAAM,IACHd,QAAQC,IAAIc,CAAK,CACrB,CAAC,CACT,EAEAC,IAAIC,iCAKJ,MAAMC,iCAAmC,KACrC,aAEA7B,yBAAyB,EAEzBW,QAAQC,IAAI,2DAA2D,EAEvEgB,iCAAmCE,YAC/B9B,yBAA0B,GAC9B,CACJ,EAKM+B,mCAAqC,KACvC,aAEgD,KAAA,IAArCH,mCACPjB,QAAQC,IAAI,6DAA6D,EAEzEoB,cAAcJ,gCAAgC,EAEtD,EAKAK,OAAOC,iBAAiB,QAAS,KAC7B,aAEAL,iCAAiC,CACrC,CAAC,EAKDI,OAAOC,iBAAiB,OAAQ,KAC5B,aAEAH,mCAAmC,CACvC,CAAC,EAKDF,iCAAiC",
     "names": [
         "elementEsiStatusDashboardWidget",
         "document",
         "getElementById",
         "esiStatusDashboardWidget",
         "fetch",
         "esistatusSettings",
@@ -19,14 +19,20 @@
         "log",
         "innerHTML",
         "classList",
         "contains",
         "bootstrap",
         "Collapse",
         "show",
+        "slice",
+        "call",
+        "querySelectorAll",
+        "map",
+        "Tooltip",
+        "tooltipTriggerEl",
         "catch",
         "error",
         "let",
         "esiStatusDashboardWidgetInterval",
         "activateEsiStatusDashboardWidget",
         "setInterval",
         "deactivateEsiStatusDashboardWidget",
```

### Comparing `aa_esi_status-2.1.1/esistatus/templates/esistatus/base.html` & `aa_esi_status-2.2.0/esistatus/templates/esistatus/base.html`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/templates/esistatus/index.html` & `aa_esi_status-2.2.0/esistatus/templates/esistatus/index.html`

 * *Files 21% similar despite different names*

```diff
@@ -18,78 +18,138 @@
 00000110: 7d0a 0a7b 2520 626c 6f63 6b20 6161 5f65  }..{% block aa_e
 00000120: 7369 7374 6174 7573 5f62 6f64 7920 257d  sistatus_body %}
 00000130: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
 00000140: 2272 6f77 223e 0a20 2020 2020 2020 207b  "row">.        {
 00000150: 2520 6966 2068 6173 5f73 7461 7475 735f  % if has_status_
 00000160: 7265 7375 6c74 2025 7d0a 2020 2020 2020  result %}.      
 00000170: 2020 2020 2020 7b25 2074 7261 6e73 6c61        {% transla
-00000180: 7465 2022 5265 6420 456e 6470 6f69 6e74  te "Red Endpoint
+00000180: 7465 2022 5265 6420 656e 6470 6f69 6e74  te "Red endpoint
 00000190: 7322 2061 7320 7472 616e 736c 6174 6564  s" as translated
 000001a0: 5f68 6561 6465 725f 7265 6420 257d 0a20  _header_red %}. 
-000001b0: 2020 2020 2020 2020 2020 207b 2520 696e             {% in
-000001c0: 636c 7564 6520 2765 7369 7374 6174 7573  clude 'esistatus
-000001d0: 2f70 6172 7469 616c 732f 656e 6470 6f69  /partials/endpoi
-000001e0: 6e74 732e 6874 6d6c 2720 7769 7468 2074  nts.html' with t
-000001f0: 6974 6c65 3d74 7261 6e73 6c61 7465 645f  itle=translated_
-00000200: 6865 6164 6572 5f72 6564 2073 7461 7475  header_red statu
-00000210: 733d 2272 6564 2220 6461 7461 3d65 7369  s="red" data=esi
-00000220: 5f65 6e64 706f 696e 745f 7374 6174 7573  _endpoint_status
-00000230: 2e72 6564 2025 7d0a 0a20 2020 2020 2020  .red %}..       
-00000240: 2020 2020 207b 2520 7472 616e 736c 6174       {% translat
-00000250: 6520 2259 656c 6c6f 7720 456e 6470 6f69  e "Yellow Endpoi
-00000260: 6e74 7322 2061 7320 7472 616e 736c 6174  nts" as translat
-00000270: 6564 5f68 6561 6465 725f 7965 6c6c 6f77  ed_header_yellow
-00000280: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00000290: 7b25 2069 6e63 6c75 6465 2027 6573 6973  {% include 'esis
-000002a0: 7461 7475 732f 7061 7274 6961 6c73 2f65  tatus/partials/e
-000002b0: 6e64 706f 696e 7473 2e68 746d 6c27 2077  ndpoints.html' w
-000002c0: 6974 6820 7469 746c 653d 7472 616e 736c  ith title=transl
-000002d0: 6174 6564 5f68 6561 6465 725f 7965 6c6c  ated_header_yell
-000002e0: 6f77 2073 7461 7475 733d 2279 656c 6c6f  ow status="yello
-000002f0: 7722 2064 6174 613d 6573 695f 656e 6470  w" data=esi_endp
-00000300: 6f69 6e74 5f73 7461 7475 732e 7965 6c6c  oint_status.yell
-00000310: 6f77 2025 7d0a 0a20 2020 2020 2020 2020  ow %}..         
-00000320: 2020 207b 2520 7472 616e 736c 6174 6520     {% translate 
-00000330: 2247 7265 656e 2045 6e64 706f 696e 7473  "Green Endpoints
+000001b0: 2020 2020 2020 2020 2020 207b 2520 7472             {% tr
+000001c0: 616e 736c 6174 6520 2252 6564 2065 6e70  anslate "Red enp
+000001d0: 6f69 6e74 7320 6861 7665 2061 2067 6f6f  oints have a goo
+000001e0: 6420 6368 616e 6365 206f 6620 6e6f 7420  d chance of not 
+000001f0: 7265 7370 6f6e 6469 6e67 2061 7420 616c  responding at al
+00000200: 6c20 6f72 2062 6569 6e67 2063 6f6d 706c  l or being compl
+00000210: 6574 656c 7920 756e 6176 6169 6c61 626c  etely unavailabl
+00000220: 652e 2220 6173 2074 7261 6e73 6c61 7465  e." as translate
+00000230: 645f 6865 6164 6572 5f72 6564 5f65 7870  d_header_red_exp
+00000240: 6c61 6e61 7469 6f6e 2025 7d0a 2020 2020  lanation %}.    
+00000250: 2020 2020 2020 2020 7b25 2069 6e63 6c75          {% inclu
+00000260: 6465 2027 6573 6973 7461 7475 732f 7061  de 'esistatus/pa
+00000270: 7274 6961 6c73 2f65 6e64 706f 696e 7473  rtials/endpoints
+00000280: 2e68 746d 6c27 2077 6974 6820 7469 746c  .html' with titl
+00000290: 653d 7472 616e 736c 6174 6564 5f68 6561  e=translated_hea
+000002a0: 6465 725f 7265 6420 7374 6174 7573 3d22  der_red status="
+000002b0: 7265 6422 2065 7870 6c61 6e61 7469 6f6e  red" explanation
+000002c0: 3d74 7261 6e73 6c61 7465 645f 6865 6164  =translated_head
+000002d0: 6572 5f72 6564 5f65 7870 6c61 6e61 7469  er_red_explanati
+000002e0: 6f6e 2064 6174 613d 6573 695f 656e 6470  on data=esi_endp
+000002f0: 6f69 6e74 5f73 7461 7475 732e 7265 6420  oint_status.red 
+00000300: 7769 7468 5f64 6574 6169 6c73 3d54 7275  with_details=Tru
+00000310: 6520 257d 0a0a 2020 2020 2020 2020 2020  e %}..          
+00000320: 2020 7b25 2074 7261 6e73 6c61 7465 2022    {% translate "
+00000330: 5965 6c6c 6f77 2065 6e64 706f 696e 7473  Yellow endpoints
 00000340: 2220 6173 2074 7261 6e73 6c61 7465 645f  " as translated_
-00000350: 6865 6164 6572 5f67 7265 656e 2025 7d0a  header_green %}.
-00000360: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-00000370: 6e63 6c75 6465 2027 6573 6973 7461 7475  nclude 'esistatu
-00000380: 732f 7061 7274 6961 6c73 2f65 6e64 706f  s/partials/endpo
-00000390: 696e 7473 2e68 746d 6c27 2077 6974 6820  ints.html' with 
-000003a0: 7469 746c 653d 7472 616e 736c 6174 6564  title=translated
-000003b0: 5f68 6561 6465 725f 6772 6565 6e20 7374  _header_green st
-000003c0: 6174 7573 3d22 6772 6565 6e22 2064 6174  atus="green" dat
-000003d0: 613d 6573 695f 656e 6470 6f69 6e74 5f73  a=esi_endpoint_s
-000003e0: 7461 7475 732e 6772 6565 6e20 257d 0a20  tatus.green %}. 
-000003f0: 2020 2020 2020 207b 2520 656c 7365 2025         {% else %
-00000400: 7d0a 2020 2020 2020 2020 2020 2020 3c64  }.            <d
-00000410: 6976 2063 6c61 7373 3d22 636f 6c2d 3132  iv class="col-12
-00000420: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00000430: 2020 203c 7020 636c 6173 733d 2261 6c65     <p class="ale
-00000440: 7274 2061 6c65 7274 2d77 6172 6e69 6e67  rt alert-warning
-00000450: 2074 6578 742d 6365 6e74 6572 223e 0a20   text-center">. 
-00000460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000470: 2020 207b 2520 7472 616e 736c 6174 6520     {% translate 
-00000480: 2243 6f75 6c64 6e27 7420 7265 6164 2074  "Couldn't read t
-00000490: 6865 2045 5349 2073 7461 7475 732e 2050  he ESI status. P
-000004a0: 6c65 6173 6520 7472 7920 616e 6420 7265  lease try and re
-000004b0: 6c6f 6164 2074 6865 2070 6167 652e 2049  load the page. I
-000004c0: 6620 7468 6174 2064 6f65 736e 2774 2068  f that doesn't h
-000004d0: 656c 702c 2069 7420 6973 2070 6f73 7369  elp, it is possi
-000004e0: 626c 6520 7468 6174 2045 5349 206d 6967  ble that ESI mig
-000004f0: 6874 2062 6520 646f 776e 2065 6e74 6972  ht be down entir
-00000500: 656c 792e 2220 257d 0a20 2020 2020 2020  ely." %}.       
-00000510: 2020 2020 2020 2020 203c 2f70 3e0a 2020           </p>.  
-00000520: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00000530: 0a20 2020 2020 2020 207b 2520 656e 6469  .        {% endi
-00000540: 6620 257d 0a20 2020 203c 2f64 6976 3e0a  f %}.    </div>.
-00000550: 7b25 2065 6e64 626c 6f63 6b20 257d 0a0a  {% endblock %}..
-00000560: 7b25 2062 6c6f 636b 2065 7874 7261 5f63  {% block extra_c
-00000570: 7373 2025 7d0a 2020 2020 3c6c 696e 6b20  ss %}.    <link 
-00000580: 7265 6c3d 2273 7479 6c65 7368 6565 7422  rel="stylesheet"
-00000590: 2068 7265 663d 227b 2520 6573 6973 7461   href="{% esista
-000005a0: 7475 735f 7374 6174 6963 2027 6573 6973  tus_static 'esis
-000005b0: 7461 7475 732f 6373 732f 6573 6973 7461  tatus/css/esista
-000005c0: 7475 732e 6d69 6e2e 6373 7327 2025 7d22  tus.min.css' %}"
-000005d0: 3e0a 7b25 2065 6e64 626c 6f63 6b20 257d  >.{% endblock %}
-000005e0: 0a                                       .
+00000350: 6865 6164 6572 5f79 656c 6c6f 7720 257d  header_yellow %}
+00000360: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
+00000370: 7472 616e 736c 6174 6520 2259 656c 6c6f  translate "Yello
+00000380: 7720 656e 6470 6f69 6e74 7320 6861 7665  w endpoints have
+00000390: 2061 2067 6f6f 6420 6368 616e 6365 206f   a good chance o
+000003a0: 6620 6265 696e 6720 736c 6f77 206f 7220  f being slow or 
+000003b0: 7265 7475 726e 696e 6720 6572 726f 7273  returning errors
+000003c0: 2e22 2061 7320 7472 616e 736c 6174 6564  ." as translated
+000003d0: 5f68 6561 6465 725f 7965 6c6c 6f77 5f65  _header_yellow_e
+000003e0: 7870 6c61 6e61 7469 6f6e 2025 7d0a 2020  xplanation %}.  
+000003f0: 2020 2020 2020 2020 2020 7b25 2069 6e63            {% inc
+00000400: 6c75 6465 2027 6573 6973 7461 7475 732f  lude 'esistatus/
+00000410: 7061 7274 6961 6c73 2f65 6e64 706f 696e  partials/endpoin
+00000420: 7473 2e68 746d 6c27 2077 6974 6820 7469  ts.html' with ti
+00000430: 746c 653d 7472 616e 736c 6174 6564 5f68  tle=translated_h
+00000440: 6561 6465 725f 7965 6c6c 6f77 2073 7461  eader_yellow sta
+00000450: 7475 733d 2279 656c 6c6f 7722 2065 7870  tus="yellow" exp
+00000460: 6c61 6e61 7469 6f6e 3d74 7261 6e73 6c61  lanation=transla
+00000470: 7465 645f 6865 6164 6572 5f79 656c 6c6f  ted_header_yello
+00000480: 775f 6578 706c 616e 6174 696f 6e20 6461  w_explanation da
+00000490: 7461 3d65 7369 5f65 6e64 706f 696e 745f  ta=esi_endpoint_
+000004a0: 7374 6174 7573 2e79 656c 6c6f 7720 7769  status.yellow wi
+000004b0: 7468 5f64 6574 6169 6c73 3d54 7275 6520  th_details=True 
+000004c0: 257d 0a0a 2020 2020 2020 2020 2020 2020  %}..            
+000004d0: 7b25 2074 7261 6e73 6c61 7465 2022 4772  {% translate "Gr
+000004e0: 6565 6e20 656e 6470 6f69 6e74 7322 2061  een endpoints" a
+000004f0: 7320 7472 616e 736c 6174 6564 5f68 6561  s translated_hea
+00000500: 6465 725f 6772 6565 6e20 257d 0a20 2020  der_green %}.   
+00000510: 2020 2020 2020 2020 207b 2520 7472 616e           {% tran
+00000520: 736c 6174 6520 2247 7265 656e 2065 6e64  slate "Green end
+00000530: 706f 696e 7473 2061 7265 2072 6573 706f  points are respo
+00000540: 6e64 696e 6720 6173 2065 7870 6563 7465  nding as expecte
+00000550: 642e 2220 6173 2074 7261 6e73 6c61 7465  d." as translate
+00000560: 645f 6865 6164 6572 5f67 7265 656e 5f65  d_header_green_e
+00000570: 7870 6c61 6e61 7469 6f6e 2025 7d0a 2020  xplanation %}.  
+00000580: 2020 2020 2020 2020 2020 7b25 2069 6e63            {% inc
+00000590: 6c75 6465 2027 6573 6973 7461 7475 732f  lude 'esistatus/
+000005a0: 7061 7274 6961 6c73 2f65 6e64 706f 696e  partials/endpoin
+000005b0: 7473 2e68 746d 6c27 2077 6974 6820 7469  ts.html' with ti
+000005c0: 746c 653d 7472 616e 736c 6174 6564 5f68  tle=translated_h
+000005d0: 6561 6465 725f 6772 6565 6e20 7374 6174  eader_green stat
+000005e0: 7573 3d22 6772 6565 6e22 2065 7870 6c61  us="green" expla
+000005f0: 6e61 7469 6f6e 3d74 7261 6e73 6c61 7465  nation=translate
+00000600: 645f 6865 6164 6572 5f67 7265 656e 5f65  d_header_green_e
+00000610: 7870 6c61 6e61 7469 6f6e 2064 6174 613d  xplanation data=
+00000620: 6573 695f 656e 6470 6f69 6e74 5f73 7461  esi_endpoint_sta
+00000630: 7475 732e 6772 6565 6e20 7769 7468 5f64  tus.green with_d
+00000640: 6574 6169 6c73 3d54 7275 6520 257d 0a20  etails=True %}. 
+00000650: 2020 2020 2020 207b 2520 656c 7365 2025         {% else %
+00000660: 7d0a 2020 2020 2020 2020 2020 2020 3c64  }.            <d
+00000670: 6976 2063 6c61 7373 3d22 636f 6c2d 3132  iv class="col-12
+00000680: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00000690: 2020 203c 7020 636c 6173 733d 2261 6c65     <p class="ale
+000006a0: 7274 2061 6c65 7274 2d77 6172 6e69 6e67  rt alert-warning
+000006b0: 2074 6578 742d 6365 6e74 6572 223e 0a20   text-center">. 
+000006c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006d0: 2020 207b 2520 7472 616e 736c 6174 6520     {% translate 
+000006e0: 2243 6f75 6c64 6e27 7420 7265 6164 2074  "Couldn't read t
+000006f0: 6865 2045 5349 2073 7461 7475 732e 2050  he ESI status. P
+00000700: 6c65 6173 6520 7472 7920 616e 6420 7265  lease try and re
+00000710: 6c6f 6164 2074 6865 2070 6167 652e 2049  load the page. I
+00000720: 6620 7468 6174 2064 6f65 736e 2774 2068  f that doesn't h
+00000730: 656c 702c 2069 7420 6973 2070 6f73 7369  elp, it is possi
+00000740: 626c 6520 7468 6174 2045 5349 206d 6967  ble that ESI mig
+00000750: 6874 2062 6520 646f 776e 2065 6e74 6972  ht be down entir
+00000760: 656c 792e 2220 257d 0a20 2020 2020 2020  ely." %}.       
+00000770: 2020 2020 2020 2020 203c 2f70 3e0a 2020           </p>.  
+00000780: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00000790: 0a20 2020 2020 2020 207b 2520 656e 6469  .        {% endi
+000007a0: 6620 257d 0a20 2020 203c 2f64 6976 3e0a  f %}.    </div>.
+000007b0: 7b25 2065 6e64 626c 6f63 6b20 257d 0a0a  {% endblock %}..
+000007c0: 7b25 2062 6c6f 636b 2065 7874 7261 5f63  {% block extra_c
+000007d0: 7373 2025 7d0a 2020 2020 3c6c 696e 6b20  ss %}.    <link 
+000007e0: 7265 6c3d 2273 7479 6c65 7368 6565 7422  rel="stylesheet"
+000007f0: 2068 7265 663d 227b 2520 6573 6973 7461   href="{% esista
+00000800: 7475 735f 7374 6174 6963 2027 6573 6973  tus_static 'esis
+00000810: 7461 7475 732f 6373 732f 6573 6973 7461  tatus/css/esista
+00000820: 7475 732e 6d69 6e2e 6373 7327 2025 7d22  tus.min.css' %}"
+00000830: 3e0a 7b25 2065 6e64 626c 6f63 6b20 257d  >.{% endblock %}
+00000840: 0a0a 7b25 2062 6c6f 636b 2065 7874 7261  ..{% block extra
+00000850: 5f6a 6176 6173 6372 6970 7420 257d 0a20  _javascript %}. 
+00000860: 2020 203c 7363 7269 7074 3e0a 2020 2020     <script>.    
+00000870: 2428 646f 6375 6d65 6e74 292e 7265 6164  $(document).read
+00000880: 7928 2829 203d 3e20 7b0a 2020 2020 2020  y(() => {.      
+00000890: 2020 2f2f 2049 6e69 7469 616c 697a 6520    // Initialize 
+000008a0: 426f 6f74 7374 7261 7020 746f 6f6c 7469  Bootstrap toolti
+000008b0: 7073 0a20 2020 2020 2020 205b 5d2e 736c  ps.        [].sl
+000008c0: 6963 652e 6361 6c6c 2864 6f63 756d 656e  ice.call(documen
+000008d0: 742e 7175 6572 7953 656c 6563 746f 7241  t.querySelectorA
+000008e0: 6c6c 2827 5b64 6174 612d 6273 2d74 6f6f  ll('[data-bs-too
+000008f0: 6c74 6970 3d22 6161 2d65 7369 2d73 7461  ltip="aa-esi-sta
+00000900: 7475 7322 5d27 2929 0a20 2020 2020 2020  tus"]')).       
+00000910: 2020 2020 202e 6d61 7028 2874 6f6f 6c74       .map((toolt
+00000920: 6970 5472 6967 6765 7245 6c29 203d 3e20  ipTriggerEl) => 
+00000930: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000940: 2020 7265 7475 726e 206e 6577 2062 6f6f    return new boo
+00000950: 7473 7472 6170 2e54 6f6f 6c74 6970 2874  tstrap.Tooltip(t
+00000960: 6f6f 6c74 6970 5472 6967 6765 7245 6c29  ooltipTriggerEl)
+00000970: 3b0a 2020 2020 2020 2020 2020 2020 7d29  ;.            })
+00000980: 3b0a 2020 2020 7d29 3b0a 2020 2020 3c2f  ;.    });.    </
+00000990: 7363 7269 7074 3e0a 7b25 2065 6e64 626c  script>.{% endbl
+000009a0: 6f63 6b20 257d 0a                        ock %}.
```

### Comparing `aa_esi_status-2.1.1/esistatus/templates/esistatus/partials/endpoints.html` & `aa_esi_status-2.2.0/esistatus/templates/esistatus/partials/endpoints.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 <div class="col-md-4 mb-3 mb-md-0">
     <div class="card card-{{ status }}-esi-endpoints">
         <div class="card-header bg-{% if status == 'red' %}danger{% elif status == 'yellow' %}warning{% else %}success{% endif %}">
             <div class="card-title text-white text-center mb-0">
-                {{ title }}
+                {{ title|title }}
+                <i
+                    class="fa-solid fa-info-circle cursor-pointer"
+                    data-bs-tooltip="aa-esi-status"
+                    title="{{ explanation }}"
+                ></i>
             </div>
         </div>
 
         <div class="card-body text-center">
             <b class="fs-4">{{ data.count }}</b><br>
             <span>
                 {{ data.percentage }}
```

### Comparing `aa_esi_status-2.1.1/esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html` & `aa_esi_status-2.2.0/esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 {% load i18n %}
 
 <div class="card">
-    <div class="card-header">
-        <div class="card-title text-center mb-0">
-            {% translate "ESI Status" %}
-        </div>
-    </div>
-
     <div class="card-body">
+        {% translate "ESI Status" as widget_title %}
+        {% include "framework/dashboard/widget-title.html" with title=widget_title %}
+
         <div class="row mb-3">
-            {% translate "Red Endpoints" as translated_header_red %}
-            {% include 'esistatus/partials/endpoints.html' with title=translated_header_red status="red" data=esi_endpoint_status.red with_details=False %}
+            {% translate "Red endpoints" as translated_header_red %}
+            {% translate "Red enpoints have a good chance of not responding at all or being completely unavailable." as translated_header_red_explanation %}
+            {% include 'esistatus/partials/endpoints.html' with title=translated_header_red status="red" explanation=translated_header_red_explanation data=esi_endpoint_status.red with_details=False %}
 
-            {% translate "Yellow Endpoints" as translated_header_yellow %}
-            {% include 'esistatus/partials/endpoints.html' with title=translated_header_yellow status="yellow" data=esi_endpoint_status.yellow with_details=False %}
+            {% translate "Yellow endpoints" as translated_header_yellow %}
+            {% translate "Yellow endpoints have a good chance of being slow or returning errors." as translated_header_yellow_explanation %}
+            {% include 'esistatus/partials/endpoints.html' with title=translated_header_yellow status="yellow" explanation=translated_header_yellow_explanation data=esi_endpoint_status.yellow with_details=False %}
 
-            {% translate "Green Endpoints" as translated_header_green %}
-            {% include 'esistatus/partials/endpoints.html' with title=translated_header_green status="green" data=esi_endpoint_status.green with_details=False %}
+            {% translate "Green endpoints" as translated_header_green %}
+            {% translate "Green endpoints are responding as expected." as translated_header_green_explanation %}
+            {% include 'esistatus/partials/endpoints.html' with title=translated_header_green status="green" explanation=translated_header_green_explanation data=esi_endpoint_status.green with_details=False %}
         </div>
 
         <div class="text-end">
             <p class="small mb-0">
                 <a href="{% url 'esistatus:index' %}">{% translate "Detailed ESI status" %}</a>
                 |
                 <a href="https://status.eveonline.com/" target="_blank" rel="noopener noreferer">{% translate "EVE Online status" %}</a>
```

#### html2text {}

```diff
@@ -1,12 +1,21 @@
 {% load i18n %}
-{% translate "ESI Status" %}
-{% translate "Red Endpoints" as translated_header_red %} {% include 'esistatus/
+{% translate "ESI Status" as widget_title %} {% include "framework/dashboard/
+widget-title.html" with title=widget_title %}
+{% translate "Red endpoints" as translated_header_red %} {% translate "Red
+enpoints have a good chance of not responding at all or being completely
+unavailable." as translated_header_red_explanation %} {% include 'esistatus/
 partials/endpoints.html' with title=translated_header_red status="red"
-data=esi_endpoint_status.red with_details=False %} {% translate "Yellow
-Endpoints" as translated_header_yellow %} {% include 'esistatus/partials/
-endpoints.html' with title=translated_header_yellow status="yellow"
+explanation=translated_header_red_explanation data=esi_endpoint_status.red
+with_details=False %} {% translate "Yellow endpoints" as
+translated_header_yellow %} {% translate "Yellow endpoints have a good chance
+of being slow or returning errors." as translated_header_yellow_explanation %}
+{% include 'esistatus/partials/endpoints.html' with
+title=translated_header_yellow status="yellow"
+explanation=translated_header_yellow_explanation
 data=esi_endpoint_status.yellow with_details=False %} {% translate "Green
-Endpoints" as translated_header_green %} {% include 'esistatus/partials/
-endpoints.html' with title=translated_header_green status="green"
+endpoints" as translated_header_green %} {% translate "Green endpoints are
+responding as expected." as translated_header_green_explanation %} {% include
+'esistatus/partials/endpoints.html' with title=translated_header_green
+status="green" explanation=translated_header_green_explanation
 data=esi_endpoint_status.green with_details=False %}
 _{_%_ _t_r_a_n_s_l_a_t_e_ _"_D_e_t_a_i_l_e_d_ _E_S_I_ _s_t_a_t_u_s_"_ _%_} | _{_%_ _t_r_a_n_s_l_a_t_e_ _"_E_V_E_ _O_n_l_i_n_e_ _s_t_a_t_u_s_"_ _%_}
```

### Comparing `aa_esi_status-2.1.1/esistatus/templatetags/esistatus.py` & `aa_esi_status-2.2.0/esistatus/templatetags/esistatus.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/tests/test_access.py` & `aa_esi_status-2.2.0/esistatus/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/tests/test_auth_hooks.py` & `aa_esi_status-2.2.0/esistatus/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/tests/test_templatetags.py` & `aa_esi_status-2.2.0/esistatus/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/tests/test_views.py` & `aa_esi_status-2.2.0/esistatus/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/esistatus/tests/utils.py` & `aa_esi_status-2.2.0/esistatus/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/LICENSE` & `aa_esi_status-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.1/README.md` & `aa_esi_status-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 ![AA ESI Status Dashboard Widget](https://raw.githubusercontent.com/ppfeufer/aa-esi-status/master/docs/images/dashboard-widget.jpg "AA ESI Status Dashboard Widget")
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA ESI Status >= 2.0.0 needs at least Alliance Auth v4.0.0!**
+> **AA ESI Status >= 2.0.0 needs at least Alliance Auth v4!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
 >
 > The last version of AA ESI Status that supports Alliance Auth v3 is `1.14.2`.
```

### Comparing `aa_esi_status-2.1.1/pyproject.toml` & `aa_esi_status-2.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dynamic = [
     "version",
 ]
 dependencies = [
-    "allianceauth<5.0.0,>=4",
+    "allianceauth<5.0.0,>=4.1",
     "allianceauth-app-utils>=1.12",
 ]
 [project.optional-dependencies]
 tests-allianceauth-latest = [
     "coverage",
     "django-webtest",
 ]
```

### Comparing `aa_esi_status-2.1.1/PKG-INFO` & `aa_esi_status-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-esi-status
-Version: 2.1.1
+Version: 2.2.0
 Summary: A simple status monitor for ESI
 Project-URL: Changelog, https://github.com/ppfeufer/aa-esi-status/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-esi-status/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-esi-status
 Project-URL: Source, https://github.com/ppfeufer/aa-esi-status.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-esi-status/issues
@@ -698,15 +698,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Requires-Dist: allianceauth-app-utils>=1.12
-Requires-Dist: allianceauth<5.0.0,>=4
+Requires-Dist: allianceauth<5.0.0,>=4.1
 Provides-Extra: tests-allianceauth-latest
 Requires-Dist: coverage; extra == 'tests-allianceauth-latest'
 Requires-Dist: django-webtest; extra == 'tests-allianceauth-latest'
 Description-Content-Type: text/markdown
 
 # AA ESI Status<a name="aa-esi-status"></a>
 
@@ -762,15 +762,15 @@
 
 ![AA ESI Status Dashboard Widget](https://raw.githubusercontent.com/ppfeufer/aa-esi-status/master/docs/images/dashboard-widget.jpg "AA ESI Status Dashboard Widget")
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA ESI Status >= 2.0.0 needs at least Alliance Auth v4.0.0!**
+> **AA ESI Status >= 2.0.0 needs at least Alliance Auth v4!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
 >
 > The last version of AA ESI Status that supports Alliance Auth v3 is `1.14.2`.
```

