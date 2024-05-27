# Comparing `tmp/aa_ledger-0.5.0a1.tar.gz` & `tmp/aa_ledger-0.5.0b1.tar.gz`

## Comparing `aa_ledger-0.5.0a1.tar` & `aa_ledger-0.5.0b1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/admin.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/app_settings.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/apps.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/auth_hooks.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/decorators.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/errors.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/hooks.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/providers.py
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/tasks.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/urls.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/api/__init__.py
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/api/helpers.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/api/schema.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/api/character/__init__.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/api/character/ledger.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/api/character/template.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/api/corporation/__init__.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/api/corporation/ledger.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/api/corporation/template.py
--rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/api/managers/billboard_manager.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/api/managers/core_manager.py
--rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/api/managers/ledger_manager.py
--rw-r--r--   0        0        0    14008 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/api/managers/template_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/locate/__init__.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/locate/de.po
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/managers/charaudit_manager.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/managers/corpaudit_manager.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/managers/general_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/migrations/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/models/__init__.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/models/characteraudit.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/models/corporationaudit.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/models/events.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/models/general.py
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/static/ledger/css/billboards_dark.css
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/static/ledger/css/cards.css
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/static/ledger/css/custom.css
--rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/static/ledger/guides/ledger-1.png
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/static/ledger/guides/ledger-2.png
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/static/ledger/guides/ledger-3.png
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/static/ledger/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/static/ledger/js/charledger.js
--rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/static/ledger/js/corpledger.js
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/static/ledger/js/img.js
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/task_helpers/__init__.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/task_helpers/char_helpers.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/task_helpers/core_helpers.py
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/task_helpers/corp_helpers.py
--rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/task_helpers/etag_helpers.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/base.html
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/error.html
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/index.html
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/menu.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/bundles/ledger-css.html
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/charledger/char_ledger.html
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/charledger/month.html
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/charledger/year.html
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/corpledger/corp_ledger.html
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/corpledger/month.html
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/corpledger/year.html
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/modals/modal-full.html
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/modals/modal-xl.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/modals/modal.html
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/modals/modal_dialog.html
--rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templates/ledger/modals/pve/view_character_content.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templatetags/__init__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/templatetags/ledger.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/view_helpers/__init__.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/view_helpers/core.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/views/__init__.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/views/pve.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/views/character/char_audit.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/views/corporation/corp_audit.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/views/corporation/corp_events.py
--rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/ledger/views/corporation/corp_tax.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/LICENSE
--rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/README.md
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/pyproject.toml
--rw-r--r--   0        0        0     8414 2020-02-02 00:00:00.000000 aa_ledger-0.5.0a1/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/admin.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/app_settings.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/apps.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/auth_hooks.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/decorators.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/errors.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/hooks.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/providers.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/tasks.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/urls.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/api/__init__.py
+-rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/api/helpers.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/api/schema.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/api/character/__init__.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/api/character/ledger.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/api/character/template.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/api/corporation/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/api/corporation/ledger.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/api/corporation/template.py
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/api/managers/billboard_manager.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/api/managers/core_manager.py
+-rw-r--r--   0        0        0     9598 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/api/managers/ledger_manager.py
+-rw-r--r--   0        0        0    13926 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/api/managers/template_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/locate/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/locate/de.po
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/managers/charaudit_manager.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/managers/corpaudit_manager.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/managers/general_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/migrations/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/models/__init__.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/models/characteraudit.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/models/corporationaudit.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/models/events.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/models/general.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/static/ledger/css/billboards_dark.css
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/static/ledger/css/cards.css
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/static/ledger/css/custom.css
+-rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/static/ledger/guides/ledger-1.png
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/static/ledger/guides/ledger-2.png
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/static/ledger/guides/ledger-3.png
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/static/ledger/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/static/ledger/js/charledger.js
+-rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/static/ledger/js/corpledger.js
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/static/ledger/js/img.js
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/task_helpers/__init__.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/task_helpers/char_helpers.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/task_helpers/core_helpers.py
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/task_helpers/corp_helpers.py
+-rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/task_helpers/etag_helpers.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/base.html
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/error.html
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/index.html
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/menu.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/bundles/ledger-css.html
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/charledger/char_ledger.html
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/charledger/month.html
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/charledger/year.html
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/corpledger/corp_ledger.html
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/corpledger/month.html
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/corpledger/year.html
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/modals/modal-full.html
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/modals/modal-xl.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/modals/modal.html
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/modals/modal_dialog.html
+-rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templates/ledger/modals/pve/view_character_content.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templatetags/__init__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/templatetags/ledger.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/view_helpers/__init__.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/view_helpers/core.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/views/__init__.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/views/pve.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/views/character/char_audit.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/views/corporation/corp_audit.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/views/corporation/corp_events.py
+-rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/ledger/views/corporation/corp_tax.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/LICENSE
+-rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/README.md
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/pyproject.toml
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 aa_ledger-0.5.0b1/PKG-INFO
```

### Comparing `aa_ledger-0.5.0a1/ledger/admin.py` & `aa_ledger-0.5.0b1/ledger/admin.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/app_settings.py` & `aa_ledger-0.5.0b1/ledger/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/auth_hooks.py` & `aa_ledger-0.5.0b1/ledger/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/decorators.py` & `aa_ledger-0.5.0b1/ledger/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/hooks.py` & `aa_ledger-0.5.0b1/ledger/hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/tasks.py` & `aa_ledger-0.5.0b1/ledger/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/urls.py` & `aa_ledger-0.5.0b1/ledger/urls.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/api/__init__.py` & `aa_ledger-0.5.0b1/ledger/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/api/helpers.py` & `aa_ledger-0.5.0b1/ledger/api/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/api/schema.py` & `aa_ledger-0.5.0b1/ledger/api/schema.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/api/character/ledger.py` & `aa_ledger-0.5.0b1/ledger/api/character/ledger.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/api/character/template.py` & `aa_ledger-0.5.0b1/ledger/api/character/template.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/api/corporation/ledger.py` & `aa_ledger-0.5.0b1/ledger/api/corporation/ledger.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/api/corporation/template.py` & `aa_ledger-0.5.0b1/ledger/api/corporation/template.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/api/managers/billboard_manager.py` & `aa_ledger-0.5.0b1/ledger/api/managers/billboard_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import math
+from dataclasses import dataclass, field
 from datetime import datetime
 from decimal import Decimal
 
 from ledger import app_settings
-from ledger.api.managers.core_manager import (
-    LedgerData,
-    LedgerDate,
-    LedgerModels,
-    LedgerSum,
-)
+from ledger.api.managers.core_manager import LedgerData, LedgerDate, LedgerModels
+
+
+@dataclass
+class LedgerSum:
+    sum_amount: list = field(default_factory=lambda: ["Ratting"])
+    sum_amount_ess: list = field(default_factory=lambda: ["ESS Payout"])
+    sum_amount_misc: list = field(default_factory=lambda: ["Miscellaneous"])
+    sum_amount_mining: list = field(default_factory=lambda: ["Mining"])
+    total_sum: int = None
 
 
 class BillboardLedger:
     def __init__(self, date_data: LedgerDate, models: LedgerModels, corp=False):
         self.is_corp = corp
         self.data = LedgerData()
         self.models = models
```

### Comparing `aa_ledger-0.5.0a1/ledger/api/managers/core_manager.py` & `aa_ledger-0.5.0b1/ledger/api/managers/core_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,111 +1,94 @@
+from dataclasses import asdict, dataclass, field
 from datetime import datetime
 
 from django.db.models import Q
 
 from ledger import app_settings
 
 
+@dataclass
 class LedgerDataCore:
-    """LedgerDataCore class to store the core data."""
-
-    def __init__(self):
-        self.total_bounty = 0
-        self.total_ess_payout = 0
-        self.total_mining = 0
-        self.total_miscellaneous = 0
-        self.total_isk = 0
+    total_bounty: int = 0
+    total_ess_payout: int = 0
+    total_mining: int = 0
+    total_miscellaneous: int = 0
+    total_isk: int = 0
 
 
+@dataclass
 class LedgerData(LedgerDataCore):
-    """LedgerData class to store the data."""
-
-    def __init__(self):
-        super().__init__()
-        self.total_cost = 0
-        self.total_production_cost = 0
-        self.total_market = 0
+    total_cost: int = 0
+    total_production_cost: int = 0
+    total_market: int = 0
 
 
 class LedgerModels:
     """LedgerModels class to store the models."""
 
     def __init__(
         self, character_journal=None, corporation_journal=None, mining_journal=None
     ):
         self.char_journal = character_journal
         self.corp_journal = corporation_journal
         self.mining_journal = mining_journal
 
 
+@dataclass
 class LedgerDate:
-    """LedgerDate class to store the date data."""
+    year: int
+    month: int
+    monthly: bool = field(init=False)
+    current_date: datetime = field(default_factory=datetime.now, init=False)
+    range_data: int = field(init=False)
+    day_checks: list = field(init=False)
 
-    def __init__(self, year, month):
-        self.year = year
-        self.month = month
-        self.monthly = month == 0
-        self.current_date = datetime.now()
+    def __post_init__(self):
+        self.monthly = self.month == 0
         self.range_data = 12 if self.monthly else 31
         self.day_checks = list(range(1, self.range_data + 1))
 
 
-class LedgerSum:
-    """LedgerSum class to store the sum amounts."""
-
-    def __init__(self):
-        self.sum_amount = ["Ratting"]
-        self.sum_amount_ess = ["ESS Payout"]
-        self.sum_amount_misc = ["Miscellaneous"]
-        self.sum_amount_mining = ["Mining"]
-        self.total_sum = None
-
-
+@dataclass
 class LedgerTotal:
-    """LedgerTotal class to store the total amounts."""
-
-    def __init__(self):
-        self.total_amount = 0
-        self.total_amount_ess = 0
-        self.total_amount_all = 0
-        self.total_amount_mining = 0
-        self.total_amount_others = 0
+    total_amount: int = 0
+    total_amount_ess: int = 0
+    total_amount_all: int = 0
+    total_amount_mining: int = 0
+    total_amount_others: int = 0
 
     def to_dict(self):
-        """Return the SummaryTotal as a dictionary."""
-        return {
-            "total_amount": self.total_amount,
-            "total_amount_ess": self.total_amount_ess,
-            "total_amount_all": self.total_amount_all,
-            "total_amount_mining": self.total_amount_mining,
-            "total_amount_others": self.total_amount_others,
-        }
+        return asdict(self)
 
 
+@dataclass
 class LedgerFilterCore:
-    """LedgerFilter class to store the filter data."""
+    char_id: list
 
-    def __init__(self, char_id: list):
-        self.char_id = char_id
+    filter_first_party: Q = field(init=False)
+    filter_second_party: Q = field(init=False)
+    filter_partys: Q = field(init=False)
+    filter_bounty: Q = field(init=False)
+    filter_ess: Q = field(init=False)
+    filter_mining: Q = field(init=False)
 
-        # Party Filters
+    def __post_init__(self):
         self.filter_first_party = Q(first_party_id__in=self.char_id)
         self.filter_second_party = Q(second_party_id__in=self.char_id)
         self.filter_partys = self.filter_first_party | self.filter_second_party
-
-        # Main Filters
         self.filter_bounty = self.filter_second_party & Q(ref_type="bounty_prizes")
         self.filter_ess = self.filter_second_party & Q(ref_type="ess_escrow_transfer")
         self.filter_mining = (
             Q(character__eve_character__character_id__in=self.char_id)
             if app_settings.LEDGER_MEMBERAUDIT_USE
             else Q(character__character__character_id__in=self.char_id)
         )
 
 
+@dataclass
 class LedgerFilterCost(LedgerFilterCore):
     """LedgerFilter class to store the filter data."""
 
     def __init__(self, char_id):
         super().__init__(char_id)
         self.my_filter_market_cost = self.filter_partys & Q(
             ref_type__in=[
@@ -115,31 +98,34 @@
             ]
         )
         self.filter_production = self.filter_partys & Q(
             ref_type__in=["industry_job_tax", "manufacturing"]
         )
 
 
+@dataclass
 class LedgerFilterTrading(LedgerFilterCost):
     """LedgerFilter class to store the filter data."""
 
-    # pylint: disable=duplicate-code
     def __init__(self, char_id):
         super().__init__(char_id)
         self.filter_market = self.filter_partys & Q(ref_type="market_transaction")
         self.filter_contract = self.filter_partys & Q(
             ref_type__in=[
                 "contract_price_payment_corp",
                 "contract_reward",
                 "contract_price",
             ],
             amount__gt=0,
         )
-        self.filter_donation = self.filter_partys & Q(ref_type="player_donation")
+        self.filter_donation = self.filter_partys & Q(
+            ref_type="player_donation", amount__gt=0
+        )
 
 
+@dataclass
 class LedgerFilter(LedgerFilterTrading):
     """LedgerFilterAll class to store all filter data."""
 
     def __init__(self, char_id):
-        super().__init__(char_id)  # Call the __init__ method of the base class
+        super().__init__(char_id)
         self.char_id = char_id
```

### Comparing `aa_ledger-0.5.0a1/ledger/api/managers/ledger_manager.py` & `aa_ledger-0.5.0b1/ledger/api/managers/ledger_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,20 @@
 
             # Convert the ESS Payout for Character
             amounts["ess"] = convert_ess_payout(amounts["ess"])
 
             total_amount_others = (
                 amounts["contracts"] + amounts["transactions"] + amounts["donations"]
             )
-            combined_amount = amounts["bounty"] + amounts["ess"] + total_amount_others
+            combined_amount = (
+                amounts["bounty"]
+                + amounts["ess"]
+                + amounts["mining"]["total_amount"]
+                + total_amount_others
+            )
 
             if amounts["bounty"] > 0 or total_amount_others > 0:
                 self.character_dict[char_id] = {
                     "main_id": char_id,
                     "main_name": char_name,
                     "total_amount": amounts["bounty"],
                     "total_amount_ess": amounts["ess"],
```

### Comparing `aa_ledger-0.5.0a1/ledger/api/managers/template_manager.py` & `aa_ledger-0.5.0b1/ledger/api/managers/template_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from dataclasses import dataclass
 from datetime import datetime
 
 from django.db.models import DecimalField, F, Q, Sum
 from django.db.models.functions import Coalesce
 
 from ledger.api.helpers import (
     convert_ess_payout,
@@ -16,69 +17,75 @@
 from ledger.view_helpers.core import calculate_days_year, events_filter
 
 CharacterMiningLedger, CharacterWalletJournalEntry = get_models_and_string()
 
 logger = get_extension_logger(__name__)
 
 
+@dataclass
 class TemplateData:
     """TemplateData class to store the data."""
 
-    def __init__(self, request, request_id, year, month):
-        self.request = request
-        self.request_id = request_id
-        self.year = year
-        self.month = month
-        self.current_date = datetime.now()
+    request: any
+    request_id: int
+    year: int
+    month: int
+    current_date: datetime = datetime.now()
+
+    def __post_init__(self):
         self.current_date = self.current_date.replace(year=self.year)
-        if not self.month == 0:
+        if self.month != 0:
             self.current_date = self.current_date.replace(month=self.month)
 
 
+@dataclass
 class TemplateTotalCore:
-    def __init__(self):
-        self.ess = 0
-        self.mining = 0
-        self.contract = 0
-        self.transaction = 0
-        self.donation = 0
-        self.production_cost = 0
-        self.market_cost = 0
+    """TemplateTotalCore class to store the core data."""
+
+    bounty: int = 0
+    ess: int = 0
+    mining: int = 0
+    contract: int = 0
+    transaction: int = 0
+    donation: int = 0
+    production_cost: int = 0
+    market_cost: int = 0
 
 
+@dataclass
 class TemplateTotalDay:
-    def __init__(self):
-        self.ess_day = 0
-        self.mining_day = 0
-        self.contract_day = 0
-        self.transaction_day = 0
-        self.donation_day = 0
-        self.production_cost_day = 0
-        self.market_cost_day = 0
+    """TemplateTotalDay class to store the daily data."""
 
+    bounty_day: int = 0
+    ess_day: int = 0
+    mining_day: int = 0
+    contract_day: int = 0
+    transaction_day: int = 0
+    donation_day: int = 0
+    production_cost_day: int = 0
+    market_cost_day: int = 0
 
+
+@dataclass
 class TemplateTotalHour:
-    def __init__(self):
-        self.ess_hour = 0
-        self.mining_hour = 0
-        self.contract_hour = 0
-        self.transaction_hour = 0
-        self.donation_hour = 0
-        self.production_cost_hour = 0
-        self.market_cost_hour = 0
+    """TemplateTotalHour class to store the hourly data."""
+
+    bounty_hour: int = 0
+    ess_hour: int = 0
+    mining_hour: int = 0
+    contract_hour: int = 0
+    transaction_hour: int = 0
+    donation_hour: int = 0
+    production_cost_hour: int = 0
+    market_cost_hour: int = 0
 
 
+@dataclass
 class TemplateTotal(TemplateTotalCore, TemplateTotalDay, TemplateTotalHour):
-    def __init__(self):
-        self.bounty = 0
-        self.bounty_day = 0
-        self.bounty_hour = 0
-        TemplateTotalCore.__init__(self)
-        TemplateTotalDay.__init__(self)
-        TemplateTotalHour.__init__(self)
+    """TemplateTotal class to store the data."""
 
     def to_dict(self):
         return {
             "bounty": {
                 "total_amount": self.bounty,
                 "total_amount_day": self.bounty_day,
                 "total_amount_hour": self.bounty_hour,
```

### Comparing `aa_ledger-0.5.0a1/ledger/locate/de.po` & `aa_ledger-0.5.0b1/ledger/locate/de.po`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/managers/charaudit_manager.py` & `aa_ledger-0.5.0b1/ledger/managers/charaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/managers/corpaudit_manager.py` & `aa_ledger-0.5.0b1/ledger/managers/corpaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/managers/general_manager.py` & `aa_ledger-0.5.0b1/ledger/managers/general_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/models/characteraudit.py` & `aa_ledger-0.5.0b1/ledger/models/characteraudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/models/corporationaudit.py` & `aa_ledger-0.5.0b1/ledger/models/corporationaudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/models/events.py` & `aa_ledger-0.5.0b1/ledger/models/events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/models/general.py` & `aa_ledger-0.5.0b1/ledger/models/general.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/static/ledger/css/billboards_dark.css` & `aa_ledger-0.5.0b1/ledger/static/ledger/css/billboards_dark.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/static/ledger/css/cards.css` & `aa_ledger-0.5.0b1/ledger/static/ledger/css/cards.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/static/ledger/css/custom.css` & `aa_ledger-0.5.0b1/ledger/static/ledger/css/custom.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/static/ledger/guides/ledger-1.png` & `aa_ledger-0.5.0b1/ledger/static/ledger/guides/ledger-1.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/static/ledger/guides/ledger-2.png` & `aa_ledger-0.5.0b1/ledger/static/ledger/guides/ledger-2.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/static/ledger/guides/ledger-3.png` & `aa_ledger-0.5.0b1/ledger/static/ledger/guides/ledger-3.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/static/ledger/images/Spinner-1s-64px-dark.gif` & `aa_ledger-0.5.0b1/ledger/static/ledger/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/static/ledger/images/Spinner-1s-64px-light.gif` & `aa_ledger-0.5.0b1/ledger/static/ledger/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/static/ledger/js/charledger.js` & `aa_ledger-0.5.0b1/ledger/static/ledger/js/charledger.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/static/ledger/js/corpledger.js` & `aa_ledger-0.5.0b1/ledger/static/ledger/js/corpledger.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/static/ledger/js/img.js` & `aa_ledger-0.5.0b1/ledger/static/ledger/js/img.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/task_helpers/char_helpers.py` & `aa_ledger-0.5.0b1/ledger/task_helpers/char_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/task_helpers/core_helpers.py` & `aa_ledger-0.5.0b1/ledger/task_helpers/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/task_helpers/corp_helpers.py` & `aa_ledger-0.5.0b1/ledger/task_helpers/corp_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/task_helpers/etag_helpers.py` & `aa_ledger-0.5.0b1/ledger/task_helpers/etag_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/base.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/base.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/error.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/error.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/index.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 {% extends 'ledger/base.html' %}
     {% load i18n %}
     {% load humanize %}
 
 {% block vow_block %}
-{{ memberaudit }}
     <div class="panel panel-primary">
         <div class="container-fluid">
             <div id="container">
                 <br>
                 <div class="line-container">
                     <div class="line-text"><h4>Ledger Guide</h4></div>
                     <hr class="custom-line">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% extends 'ledger/base.html' %} {% load i18n %} {% load humanize %} {% block
-vow_block %} {{ memberaudit }}
+vow_block %}
 
 ****** LLeeddggeerr GGuuiiddee ******
 ===============================================================================
 Character Ledger shows all Ratting / ESS Payout / Mining entrys per Month / Day
 
 You can switch between Months to show what you have already done and how much
 it was.
```

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/menu.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/menu.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/charledger/char_ledger.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/charledger/char_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/charledger/month.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/charledger/month.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/charledger/year.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/charledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/corpledger/corp_ledger.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/corpledger/corp_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/corpledger/month.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/corpledger/month.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/corpledger/year.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/corpledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/modals/modal-full.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/modals/modal-full.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/modals/modal-xl.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/modals/modal-xl.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/modals/modal.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/modals/modal.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/modals/modal_dialog.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/modals/modal_dialog.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/templates/ledger/modals/pve/view_character_content.html` & `aa_ledger-0.5.0b1/ledger/templates/ledger/modals/pve/view_character_content.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/view_helpers/core.py` & `aa_ledger-0.5.0b1/ledger/view_helpers/core.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/views/pve.py` & `aa_ledger-0.5.0b1/ledger/views/pve.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/views/character/char_audit.py` & `aa_ledger-0.5.0b1/ledger/views/character/char_audit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/views/corporation/corp_audit.py` & `aa_ledger-0.5.0b1/ledger/views/corporation/corp_audit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/views/corporation/corp_events.py` & `aa_ledger-0.5.0b1/ledger/views/corporation/corp_events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/ledger/views/corporation/corp_tax.py` & `aa_ledger-0.5.0b1/ledger/views/corporation/corp_tax.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/LICENSE` & `aa_ledger-0.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/README.md` & `aa_ledger-0.5.0b1/README.md`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.5.0a1/pyproject.toml` & `aa_ledger-0.5.0b1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     { name = "Geuthur", email = "devgeuthur@gmail.com" },
 ]
 requires-python = ">=3.8"
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -30,17 +31,16 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dynamic = [
     "version",
 ]
 dependencies = [
-    "allianceauth<5,>=4",
+    "allianceauth>=4",
     "allianceauth-app-utils>=1.19",
-    "dacite",
     "django-eveuniverse>=1.3",
     "django-ninja",
 ]
 optional-dependencies.tests-allianceauth-latest = [
     "coverage",
     "django-webtest",
 ]
```

### Comparing `aa_ledger-0.5.0a1/PKG-INFO` & `aa_ledger-0.5.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-ledger
-Version: 0.5.0a1
+Version: 0.5.0b1
 Summary: Character/Corporation Ledger
 Project-URL: Changelog, https://github.com/Geuthur/aa-ledger/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/Geuthur/aa-ledger
 Project-URL: Source, https://github.com/Geuthur/aa-ledger
 Project-URL: Tracker, https://github.com/Geuthur/aa-ledger/issues
 Author-email: Geuthur <devgeuthur@gmail.com>
 License: MIT License
@@ -28,30 +28,30 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Requires-Dist: allianceauth-app-utils>=1.19
-Requires-Dist: allianceauth<5,>=4
-Requires-Dist: dacite
+Requires-Dist: allianceauth>=4
 Requires-Dist: django-eveuniverse>=1.3
 Requires-Dist: django-ninja
 Provides-Extra: tests-allianceauth-latest
 Requires-Dist: coverage; extra == 'tests-allianceauth-latest'
 Requires-Dist: django-webtest; extra == 'tests-allianceauth-latest'
 Description-Content-Type: text/markdown
```

