# Comparing `tmp/django-crispy-formset-modal-0.7.tar.gz` & `tmp/django-crispy-formset-modal-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-crispy-formset-modal-0.7.tar", last modified: Mon Mar 25 14:51:31 2024, max compression
+gzip compressed data, was "django-crispy-formset-modal-0.8.tar", last modified: Mon Mar 25 19:32:34 2024, max compression
```

## Comparing `django-crispy-formset-modal-0.7.tar` & `django-crispy-formset-modal-0.8.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.285419 django-crispy-formset-modal-0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-03-25 14:51:31.285419 django-crispy-formset-modal-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.281419 django-crispy-formset-modal-0.7/crispy_formset_modal/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.277418 django-crispy-formset-modal-0.7/crispy_formset_modal/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.277418 django-crispy-formset-modal-0.7/crispy_formset_modal/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.281419 django-crispy-formset-modal-0.7/crispy_formset_modal/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.277418 django-crispy-formset-modal-0.7/crispy_formset_modal/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.277418 django-crispy-formset-modal-0.7/crispy_formset_modal/static/crispy_formset_modal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.281419 django-crispy-formset-modal-0.7/crispy_formset_modal/static/crispy_formset_modal/js/
--rw-r--r--   0 runner    (1001) docker     (127)    23875 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/static/crispy_formset_modal/js/crispy-formset-modal.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    69206 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/static/crispy_formset_modal/js/crispy-formset-modal.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.277418 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.277418 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.281419 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/edit_button.html
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/table.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.281419 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/edit_button.html
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/form.html
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/table.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.281419 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bulma/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bulma/edit_button.html
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bulma/form.html
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bulma/modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bulma/table.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.285419 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/tailwind/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/tailwind/edit_button.html
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/tailwind/form.html
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/tailwind/modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/tailwind/table.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.285419 django-crispy-formset-modal-0.7/crispy_formset_modal/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/crispy_formset_modal/templatetags/formset_modal_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:51:31.285419 django-crispy-formset-modal-0.7/django_crispy_formset_modal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-03-25 14:51:31.000000 django-crispy-formset-modal-0.7/django_crispy_formset_modal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-25 14:51:31.000000 django-crispy-formset-modal-0.7/django_crispy_formset_modal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 14:51:31.000000 django-crispy-formset-modal-0.7/django_crispy_formset_modal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-25 14:51:31.000000 django-crispy-formset-modal-0.7/django_crispy_formset_modal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-25 14:51:31.000000 django-crispy-formset-modal-0.7/django_crispy_formset_modal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-25 14:51:31.285419 django-crispy-formset-modal-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-25 14:51:22.000000 django-crispy-formset-modal-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.740083 django-crispy-formset-modal-0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-03-25 19:32:34.740083 django-crispy-formset-modal-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.736083 django-crispy-formset-modal-0.8/crispy_formset_modal/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.732083 django-crispy-formset-modal-0.8/crispy_formset_modal/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.732083 django-crispy-formset-modal-0.8/crispy_formset_modal/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.736083 django-crispy-formset-modal-0.8/crispy_formset_modal/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/locale/es/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.732083 django-crispy-formset-modal-0.8/crispy_formset_modal/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.732083 django-crispy-formset-modal-0.8/crispy_formset_modal/static/crispy_formset_modal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.736083 django-crispy-formset-modal-0.8/crispy_formset_modal/static/crispy_formset_modal/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    23875 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/static/crispy_formset_modal/js/crispy-formset-modal.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    69206 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/static/crispy_formset_modal/js/crispy-formset-modal.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.732083 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.732083 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.736083 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/edit_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/empty_state.html
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/table.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.740083 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/edit_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/empty_state.html
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/table.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.740083 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bulma/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bulma/edit_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bulma/empty_state.html
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bulma/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bulma/modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bulma/table.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.740083 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/tailwind/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/tailwind/edit_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/tailwind/empty_state.html
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/tailwind/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/tailwind/modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/tailwind/table.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.740083 django-crispy-formset-modal-0.8/crispy_formset_modal/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/crispy_formset_modal/templatetags/formset_modal_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:32:34.740083 django-crispy-formset-modal-0.8/django_crispy_formset_modal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-03-25 19:32:34.000000 django-crispy-formset-modal-0.8/django_crispy_formset_modal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-25 19:32:34.000000 django-crispy-formset-modal-0.8/django_crispy_formset_modal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 19:32:34.000000 django-crispy-formset-modal-0.8/django_crispy_formset_modal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-25 19:32:34.000000 django-crispy-formset-modal-0.8/django_crispy_formset_modal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-25 19:32:34.000000 django-crispy-formset-modal-0.8/django_crispy_formset_modal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-25 19:32:34.740083 django-crispy-formset-modal-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-25 19:32:25.000000 django-crispy-formset-modal-0.8/setup.py
```

### Comparing `django-crispy-formset-modal-0.7/LICENSE` & `django-crispy-formset-modal-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/PKG-INFO` & `django-crispy-formset-modal-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-crispy-formset-modal
-Version: 0.7
+Version: 0.8
 Summary: Django app that provides an easy way to manage and manipulate formsets using modals with Django Crispy Forms.
 Home-page: https://github.com/blasferna/django-crispy-formset-modal
 Author: Blas Fernandez
 Author-email: blasferna@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django-crispy-formset-modal-0.7/README.md` & `django-crispy-formset-modal-0.8/README.md`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/layout.py` & `django-crispy-formset-modal-0.8/crispy_formset_modal/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,17 @@
                 "has_footer": len(self.sum_columns) > 0,
                 "form_template_name": (
                     f"crispy_formset_modal/{template_pack}/form.html"
                 ),
                 "modal_template_name": (
                     f"crispy_formset_modal/{template_pack}/modal.html"
                 ),
+                "empty_state_template_name": (
+                    f"crispy_formset_modal/{template_pack}/empty_state.html"
+                ),
                 "template_pack": template_pack,
                 "modal_size": self.modal_size,
                 "modal_placement": self.modal_placement,
                 "edit_button_template_name": USER_CONFIG["edit_button_template_name"][
                     template_pack
                 ],
             }
```

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/locale/es/LC_MESSAGES/django.po` & `django-crispy-formset-modal-0.8/crispy_formset_modal/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/locale/es/LC_MESSAGES/djangojs.po` & `django-crispy-formset-modal-0.8/crispy_formset_modal/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/static/crispy_formset_modal/js/crispy-formset-modal.min.js` & `django-crispy-formset-modal-0.8/crispy_formset_modal/static/crispy_formset_modal/js/crispy-formset-modal.min.js`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/static/crispy_formset_modal/js/crispy-formset-modal.min.js.map` & `django-crispy-formset-modal-0.8/crispy_formset_modal/static/crispy_formset_modal/js/crispy-formset-modal.min.js.map`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/edit_button.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/edit_button.html`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/form.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/form.html`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/modal.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/modal.html`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/table.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/table.html`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 {% endfor %}
                 <th class="text-left" style="width: 4rem;"></th>
                 </tr>
             </thead>
             <tbody>  
                 <tr class="empty-table">
                     <td class="empty-table-content text-center" colspan={{ headers|length|add:3 }}>
-                       {% trans "No data" %}   
+                       {% include empty_state_template_name %}
                     </td>
                 </tr>
             </tbody>
             {% if has_footer %}
             <tfoot>
                 <tr>
                     <td>&nbsp;</td>
```

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/edit_button.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/edit_button.html`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/form.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/form.html`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/modal.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/modal.html`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/table.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/table.html`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 {% endfor %}
                 <th class="text-left" style="width: 4rem;"></th>
                 </tr>
             </thead>
             <tbody>  
                 <tr class="empty-table">
                     <td class="empty-table-content text-center" colspan={{ headers|length|add:3 }}>
-                       {% trans "No data" %}   
+                        {% include empty_state_template_name %}
                     </td>
                 </tr>
             </tbody>
             {% if has_footer %}
             <tfoot>
                 <tr>
                     <td>&nbsp;</td>
```

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bulma/edit_button.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bulma/edit_button.html`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bulma/form.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bulma/form.html`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bulma/modal.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bulma/modal.html`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/bulma/table.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/bulma/table.html`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 {% endfor %}
                 <th class="has-text-left" style="width: 4rem;"></th>
                 </tr>
             </thead>
             <tbody>  
                 <tr class="empty-table">
                     <td class="empty-table-content has-text-centered" colspan={{ headers|length|add:3 }}>
-                       {% trans "No data" %}   
+                        {% include empty_state_template_name %}
                     </td>
                 </tr>
             </tbody>
             {% if has_footer %}
             <tfoot>
                 <tr>
                     <td>&nbsp;</td>
```

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/tailwind/form.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/tailwind/form.html`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/tailwind/modal.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/tailwind/modal.html`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templates/crispy_formset_modal/tailwind/table.html` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templates/crispy_formset_modal/tailwind/table.html`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/crispy_formset_modal/templatetags/formset_modal_tags.py` & `django-crispy-formset-modal-0.8/crispy_formset_modal/templatetags/formset_modal_tags.py`

 * *Files identical despite different names*

### Comparing `django-crispy-formset-modal-0.7/django_crispy_formset_modal.egg-info/PKG-INFO` & `django-crispy-formset-modal-0.8/django_crispy_formset_modal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-crispy-formset-modal
-Version: 0.7
+Version: 0.8
 Summary: Django app that provides an easy way to manage and manipulate formsets using modals with Django Crispy Forms.
 Home-page: https://github.com/blasferna/django-crispy-formset-modal
 Author: Blas Fernandez
 Author-email: blasferna@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django-crispy-formset-modal-0.7/django_crispy_formset_modal.egg-info/SOURCES.txt` & `django-crispy-formset-modal-0.8/django_crispy_formset_modal.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,30 @@
 crispy_formset_modal/helper.py
 crispy_formset_modal/layout.py
 crispy_formset_modal/locale/es/LC_MESSAGES/django.po
 crispy_formset_modal/locale/es/LC_MESSAGES/djangojs.po
 crispy_formset_modal/static/crispy_formset_modal/js/crispy-formset-modal.min.js
 crispy_formset_modal/static/crispy_formset_modal/js/crispy-formset-modal.min.js.map
 crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/edit_button.html
+crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/empty_state.html
 crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/form.html
 crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/modal.html
 crispy_formset_modal/templates/crispy_formset_modal/bootstrap4/table.html
 crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/edit_button.html
+crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/empty_state.html
 crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/form.html
 crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/modal.html
 crispy_formset_modal/templates/crispy_formset_modal/bootstrap5/table.html
 crispy_formset_modal/templates/crispy_formset_modal/bulma/edit_button.html
+crispy_formset_modal/templates/crispy_formset_modal/bulma/empty_state.html
 crispy_formset_modal/templates/crispy_formset_modal/bulma/form.html
 crispy_formset_modal/templates/crispy_formset_modal/bulma/modal.html
 crispy_formset_modal/templates/crispy_formset_modal/bulma/table.html
 crispy_formset_modal/templates/crispy_formset_modal/tailwind/edit_button.html
+crispy_formset_modal/templates/crispy_formset_modal/tailwind/empty_state.html
 crispy_formset_modal/templates/crispy_formset_modal/tailwind/form.html
 crispy_formset_modal/templates/crispy_formset_modal/tailwind/modal.html
 crispy_formset_modal/templates/crispy_formset_modal/tailwind/table.html
 crispy_formset_modal/templatetags/formset_modal_tags.py
 django_crispy_formset_modal.egg-info/PKG-INFO
 django_crispy_formset_modal.egg-info/SOURCES.txt
 django_crispy_formset_modal.egg-info/dependency_links.txt
```

### Comparing `django-crispy-formset-modal-0.7/setup.py` & `django-crispy-formset-modal-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="django-crispy-formset-modal",
     packages=["crispy_formset_modal"],
     include_package_data=True,
-    version="0.7",
+    version="0.8",
     description="Django app that provides an easy way to manage and manipulate formsets using modals with Django Crispy Forms.",
     long_description=open("README.md").read(),
 	long_description_content_type="text/markdown",
     author="Blas Fernandez",
     author_email="blasferna@gmail.com",
     url="https://github.com/blasferna/django-crispy-formset-modal",
     classifiers=[
```

