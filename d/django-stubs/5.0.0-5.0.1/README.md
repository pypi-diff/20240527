# Comparing `tmp/django_stubs-5.0.0.tar.gz` & `tmp/django_stubs-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_stubs-5.0.0.tar", last modified: Tue Apr 30 10:03:06 2024, max compression
+gzip compressed data, was "django_stubs-5.0.1.tar", last modified: Mon May 27 11:22:14 2024, max compression
```

## Comparing `django_stubs-5.0.0.tar` & `django_stubs-5.0.1.tar`

### file list

```diff
@@ -1,834 +1,835 @@
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.921465 django_stubs-5.0.0/
--rw-r--r--   0 marti     (1000) marti     (1000)     1075 2023-06-02 14:08:54.000000 django_stubs-5.0.0/LICENSE.md
--rw-r--r--   0 marti     (1000) marti     (1000)    16027 2024-04-30 10:03:06.921465 django_stubs-5.0.0/PKG-INFO
--rw-r--r--   0 marti     (1000) marti     (1000)    14648 2024-04-30 10:01:49.000000 django_stubs-5.0.0/README.md
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.851465 django_stubs-5.0.0/django-stubs/
--rw-r--r--   0 marti     (1000) marti     (1000)      224 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.851465 django_stubs-5.0.0/django-stubs/apps/
--rw-r--r--   0 marti     (1000) marti     (1000)       78 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/apps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1125 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/apps/config.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1970 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/apps/registry.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.851465 django_stubs-5.0.0/django-stubs/conf/
--rw-r--r--   0 marti     (1000) marti     (1000)     1545 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/conf/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)    17238 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/conf/global_settings.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.851465 django_stubs-5.0.0/django-stubs/conf/locale/
--rw-r--r--   0 marti     (1000) marti     (1000)       50 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/conf/locale/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.851465 django_stubs-5.0.0/django-stubs/conf/urls/
--rw-r--r--   0 marti     (1000) marti     (1000)     1073 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/conf/urls/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      231 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/conf/urls/i18n.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      193 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/conf/urls/static.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.851465 django_stubs-5.0.0/django-stubs/contrib/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.854799 django_stubs-5.0.0/django-stubs/contrib/admin/
--rw-r--r--   0 marti     (1000) marti     (1000)     1203 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      313 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/actions.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      136 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/apps.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1078 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/admin/checks.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2167 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/admin/decorators.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      251 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4313 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/filters.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      237 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/forms.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     5570 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/helpers.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.854799 django_stubs-5.0.0/django-stubs/contrib/admin/migrations/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1052 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/admin/models.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)    16634 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/options.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4347 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/sites.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.854799 django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1981 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/admin_list.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      690 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/admin_modify.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      503 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/admin_urls.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      605 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      441 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/log.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1629 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/tests.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4488 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.854799 django_stubs-5.0.0/django-stubs/contrib/admin/views/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/views/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      374 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/views/autocomplete.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      383 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admin/views/decorators.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3177 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/views/main.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     5651 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/admin/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.854799 django_stubs-5.0.0/django-stubs/contrib/admindocs/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admindocs/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      129 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admindocs/apps.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      478 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admindocs/middleware.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       60 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admindocs/urls.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      840 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admindocs/utils.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1018 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/admindocs/views.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/auth/
--rw-r--r--   0 marti     (1000) marti     (1000)     1735 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/auth/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      560 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/auth/admin.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       68 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/apps.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1891 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/backends.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1592 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/auth/base_user.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      398 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/checks.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      662 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      955 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/contrib/auth/decorators.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3962 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/auth/forms.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/auth/handlers/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/handlers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      198 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/handlers/modwsgi.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2614 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/auth/hashers.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/auth/management/
--rw-r--r--   0 marti     (1000) marti     (1000)      406 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/auth/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/auth/management/commands/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      125 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/management/commands/changepassword.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      194 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      818 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/auth/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/auth/migrations/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1228 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/mixins.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4693 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/auth/models.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2114 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/auth/password_validation.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      120 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/signals.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      735 2023-06-02 14:08:54.000000 django_stubs-5.0.0/django-stubs/contrib/auth/tokens.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       60 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/auth/urls.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      153 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/auth/validators.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2550 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/auth/views.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/contenttypes/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      655 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/admin.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       76 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/apps.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      414 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/checks.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3851 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/fields.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1421 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/forms.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/contenttypes/management/
--rw-r--r--   0 marti     (1000) marti     (1000)     1305 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/contenttypes/management/commands/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      363 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.858132 django_stubs-5.0.0/django-stubs/contrib/contenttypes/migrations/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1040 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/models.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      213 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/contenttypes/views.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/flatpages/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      259 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/admin.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      129 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/apps.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      136 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/forms.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      293 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/flatpages/migrations/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      402 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/models.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       81 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/sitemaps.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/flatpages/templatetags/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      484 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       60 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/urls.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      309 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/flatpages/views.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/gis/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/gis/admin/
--rw-r--r--   0 marti     (1000) marti     (1000)      724 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/admin/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      261 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/admin/options.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      272 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/admin/widgets.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       67 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/gis/db/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      200 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/adapter.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1443 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/features.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      836 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/models.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1408 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/operations.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.861465 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      251 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      867 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/features.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      333 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1268 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      699 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.864799 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      226 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      254 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      444 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/features.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      287 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      727 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/models.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1440 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      826 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.864799 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      399 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      351 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      189 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/const.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      407 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/features.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      360 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      765 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/models.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2320 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      247 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      340 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.864799 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      182 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      835 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      127 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      417 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      451 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      775 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1345 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1103 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      656 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.864799 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/
--rw-r--r--   0 marti     (1000) marti     (1000)      834 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      800 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/aggregates.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     6433 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/fields.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     6939 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/functions.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2955 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/lookups.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      345 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/proxy.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.864799 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/sql/
--rw-r--r--   0 marti     (1000) marti     (1000)      166 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/sql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      829 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/db/models/sql/conversion.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      866 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/feeds.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.868132 django_stubs-5.0.0/django-stubs/contrib/gis/forms/
--rw-r--r--   0 marti     (1000) marti     (1000)      642 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      808 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/gis/forms/fields.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      952 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/forms/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.868132 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/
--rw-r--r--   0 marti     (1000) marti     (1000)     1070 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      137 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      574 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/datasource.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      324 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/driver.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      688 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/envelope.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      200 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/error.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      947 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/feature.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1460 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/field.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4844 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/geometries.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      304 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/geomtype.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1741 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/layer.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      858 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/libgdal.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.868132 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1036 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      961 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1077 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      970 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1053 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      614 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.868132 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1565 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/band.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      225 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      252 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/const.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2395 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/source.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2193 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/contrib/gis/gdal/srs.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.868132 django_stubs-5.0.0/django-stubs/contrib/gis/geoip2/
--rw-r--r--   0 marti     (1000) marti     (1000)      106 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geoip2/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1202 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geoip2/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       99 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geoip2/resources.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       97 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geometry.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.871465 django_stubs-5.0.0/django-stubs/contrib/gis/geos/
--rw-r--r--   0 marti     (1000) marti     (1000)      883 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      185 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      604 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/collections.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1252 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/coordseq.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       36 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/error.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      310 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/factory.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     5385 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/geometry.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      453 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/io.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      896 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/libgeos.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      766 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/linestring.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1126 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/mutable_list.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      816 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/point.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      713 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/polygon.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      737 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prepared.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.871465 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/
--rw-r--r--   0 marti     (1000) marti     (1000)     4249 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      795 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      474 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      792 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/geom.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3014 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/io.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      232 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/misc.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      789 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      434 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      496 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      609 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/topology.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1343 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/contrib/gis/measure.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      252 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/ptr.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.871465 django_stubs-5.0.0/django-stubs/contrib/gis/serializers/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/serializers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      493 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/serializers/geojson.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      244 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.871465 django_stubs-5.0.0/django-stubs/contrib/gis/sitemaps/
--rw-r--r--   0 marti     (1000) marti     (1000)      138 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/sitemaps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      328 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/sitemaps/kml.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      352 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/sitemaps/views.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.871465 django_stubs-5.0.0/django-stubs/contrib/gis/utils/
--rw-r--r--   0 marti     (1000) marti     (1000)      436 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/utils/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2561 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/gis/utils/layermapping.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      129 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/gis/utils/ogrinfo.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      320 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/utils/ogrinspect.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      199 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/utils/srs.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      202 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/gis/views.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.874799 django_stubs-5.0.0/django-stubs/contrib/humanize/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/humanize/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      128 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/humanize/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.874799 django_stubs-5.0.0/django-stubs/contrib/humanize/templatetags/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/humanize/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      859 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/humanize/templatetags/humanize.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.874799 django_stubs-5.0.0/django-stubs/contrib/messages/
--rw-r--r--   0 marti     (1000) marti     (1000)      690 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/messages/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1294 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/api.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      193 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/messages/apps.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      120 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/constants.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      225 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      349 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.874799 django_stubs-5.0.0/django-stubs/contrib/messages/storage/
--rw-r--r--   0 marti     (1000) marti     (1000)      168 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/messages/storage/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      906 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/storage/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      463 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/storage/cookie.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      228 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/storage/fallback.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      468 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/storage/session.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       44 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/messages/utils.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      427 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/messages/views.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.874799 django_stubs-5.0.0/django-stubs/contrib/postgres/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.874799 django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/
--rw-r--r--   0 marti     (1000) marti     (1000)      864 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2208 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/general.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      822 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/mixins.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      910 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/statistics.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      270 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/apps.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1320 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/constraints.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      459 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/expressions.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/
--rw-r--r--   0 marti     (1000) marti     (1000)      759 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2399 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/array.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      385 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/citext.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1013 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/hstore.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       99 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/jsonb.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3182 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/ranges.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      106 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/fields/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/postgres/forms/
--rw-r--r--   0 marti     (1000) marti     (1000)      604 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2299 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/forms/array.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      478 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/forms/hstore.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1537 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/forms/ranges.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      223 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/functions.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4041 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/indexes.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      877 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/lookups.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2045 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/operations.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4829 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/search.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      152 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/serializers.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      383 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/signals.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      177 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/utils.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      707 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/postgres/validators.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/redirects/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/redirects/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      185 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/redirects/admin.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      129 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/redirects/apps.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      379 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/redirects/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/redirects/migrations/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/redirects/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      150 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/redirects/models.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/sessions/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      128 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/apps.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1892 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      280 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/cache.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      286 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/cached_db.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      549 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/db.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      239 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/file.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      100 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/backends/signed_cookies.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      677 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/base_session.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      210 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/exceptions.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/sessions/management/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.878132 django_stubs-5.0.0/django-stubs/contrib/sessions/management/commands/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      155 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      447 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/sessions/migrations/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      243 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/models.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      157 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/sessions/serializers.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/sitemaps/
--rw-r--r--   0 marti     (1000) marti     (1000)     1741 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/sitemaps/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      128 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sitemaps/apps.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      694 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/sitemaps/views.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/sites/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sites/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      138 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sites/admin.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       69 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sites/apps.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      247 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/sites/checks.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      289 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/sites/management.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      247 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sites/managers.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      209 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sites/middleware.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/sites/migrations/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sites/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      605 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/sites/models.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      375 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/sites/requests.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      221 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/sites/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/staticfiles/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      120 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/apps.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      391 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/checks.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2496 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/finders.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1815 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/handlers.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/commands/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1170 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      206 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      120 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2355 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/storage.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      100 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/testing.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      152 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/urls.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      345 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/utils.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      216 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/staticfiles/views.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.881465 django_stubs-5.0.0/django-stubs/contrib/syndication/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/syndication/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      131 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/contrib/syndication/apps.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1889 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/contrib/syndication/views.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.884799 django_stubs-5.0.0/django-stubs/core/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       98 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/asgi.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.884799 django_stubs-5.0.0/django-stubs/core/cache/
--rw-r--r--   0 marti     (1000) marti     (1000)      697 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/cache/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.884799 django_stubs-5.0.0/django-stubs/core/cache/backends/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4184 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      634 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/db.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      182 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      259 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/filebased.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      226 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/locmem.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      776 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/memcached.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2296 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/cache/backends/redis.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      198 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/cache/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.884799 django_stubs-5.0.0/django-stubs/core/checks/
--rw-r--r--   0 marti     (1000) marti     (1000)      652 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      265 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/async_checks.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      529 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/caches.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.884799 django_stubs-5.0.0/django-stubs/core/checks/compatibility/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/compatibility/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      256 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/core/checks/compatibility/django_4_0.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      229 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/database.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      268 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/core/checks/files.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1084 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/messages.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      389 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/model_checks.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1889 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/checks/registry.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.884799 django_stubs-5.0.0/django-stubs/core/checks/security/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/security/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2087 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/core/checks/security/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      514 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/core/checks/security/csrf.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      577 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/security/sessions.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      565 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/core/checks/templates.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      625 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/translation.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      706 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/checks/urls.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1968 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/core/exceptions.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.888132 django_stubs-5.0.0/django-stubs/core/files/
--rw-r--r--   0 marti     (1000) marti     (1000)       68 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/files/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1897 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/files/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      359 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/files/images.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      296 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/files/locks.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      130 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/files/move.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.888132 django_stubs-5.0.0/django-stubs/core/files/storage/
--rw-r--r--   0 marti     (1000) marti     (1000)      724 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/core/files/storage/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1073 2023-06-02 14:08:54.000000 django_stubs-5.0.0/django-stubs/core/files/storage/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      910 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/files/storage/filesystem.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      509 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/files/storage/handler.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      884 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/files/storage/memory.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      338 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/core/files/storage/mixins.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      100 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/files/temp.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1535 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/files/uploadedfile.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3017 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/files/uploadhandler.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      736 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/files/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.888132 django_stubs-5.0.0/django-stubs/core/handlers/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/handlers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2473 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/handlers/asgi.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1353 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/handlers/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      770 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/handlers/exception.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1265 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/handlers/wsgi.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.888132 django_stubs-5.0.0/django-stubs/core/mail/
--rw-r--r--   0 marti     (1000) marti     (1000)     1714 2023-06-02 14:08:54.000000 django_stubs-5.0.0/django-stubs/core/mail/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.888132 django_stubs-5.0.0/django-stubs/core/mail/backends/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/mail/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      670 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/core/mail/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      303 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/core/mail/backends/console.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      103 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/mail/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      128 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/mail/backends/filebased.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      103 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/mail/backends/locmem.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      454 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/mail/backends/smtp.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4034 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/mail/message.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       95 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/mail/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.891465 django_stubs-5.0.0/django-stubs/core/management/
--rw-r--r--   0 marti     (1000) marti     (1000)      945 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/management/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3804 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/management/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1178 2023-10-23 19:46:47.000000 django_stubs-5.0.0/django-stubs/core/management/color.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.891465 django_stubs-5.0.0/django-stubs/core/management/commands/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      179 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/check.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      503 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/compilemessages.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      284 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/createcachetable.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      155 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/dbshell.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      568 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/diffsettings.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      153 2023-10-23 19:46:47.000000 django_stubs-5.0.0/django-stubs/core/management/commands/dumpdata.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      220 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/flush.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      944 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/management/commands/inspectdb.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2347 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/loaddata.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2320 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/makemessages.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      847 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/core/management/commands/makemigrations.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      643 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/migrate.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       85 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/management/commands/optimizemigration.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      617 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/runserver.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      111 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/sendtestemail.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      319 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/shell.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      371 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/showmigrations.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      184 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/sqlflush.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      203 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/sqlmigrate.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       83 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/sqlsequencereset.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      405 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/squashmigrations.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      225 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/startapp.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      225 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/core/management/commands/startproject.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      232 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/test.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       85 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/commands/testserver.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      488 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/sql.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1033 2023-10-23 19:46:47.000000 django_stubs-5.0.0/django-stubs/core/management/templates.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      850 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/management/utils.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2516 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/paginator.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.894798 django_stubs-5.0.0/django-stubs/core/serializers/
--rw-r--r--   0 marti     (1000) marti     (1000)     1193 2023-10-23 19:46:47.000000 django_stubs-5.0.0/django-stubs/core/serializers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3195 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/serializers/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      577 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/serializers/json.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      398 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/serializers/jsonl.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      490 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/serializers/python.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      831 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/serializers/pyyaml.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2355 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/serializers/xml_serializer.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.894798 django_stubs-5.0.0/django-stubs/core/servers/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/servers/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1459 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/servers/basehttp.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      139 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/signals.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2656 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/signing.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4626 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/core/validators.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       98 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/core/wsgi.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.894798 django_stubs-5.0.0/django-stubs/db/
--rw-r--r--   0 marti     (1000) marti     (1000)     1047 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.894798 django_stubs-5.0.0/django-stubs/db/backends/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.894798 django_stubs-5.0.0/django-stubs/db/backends/base/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/base/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     5434 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/backends/base/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      555 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/base/client.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1301 2023-10-23 19:46:47.000000 django_stubs-5.0.0/django-stubs/db/backends/base/creation.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     5747 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/backends/base/features.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1870 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/base/introspection.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     7157 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/base/operations.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4499 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/backends/base/schema.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      389 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/base/validation.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3183 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/backends/ddl_references.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.894798 django_stubs-5.0.0/django-stubs/db/backends/dummy/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/dummy/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      924 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/dummy/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      176 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/dummy/features.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.894798 django_stubs-5.0.0/django-stubs/db/backends/mysql/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2491 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      473 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/client.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      734 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/compiler.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      255 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/creation.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3812 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/features.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      568 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2872 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/operations.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      902 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/schema.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      354 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/mysql/validation.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.898132 django_stubs-5.0.0/django-stubs/db/backends/oracle/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2718 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      546 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/client.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      373 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/creation.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1874 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/features.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      398 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/functions.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      351 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/introspection.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3990 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/operations.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      924 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/schema.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      511 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/utils.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      308 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/oracle/validation.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.898132 django_stubs-5.0.0/django-stubs/db/backends/postgresql/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1441 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      524 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/client.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      208 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/creation.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2256 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/features.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      304 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/introspection.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      529 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/operations.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      809 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/postgresql/schema.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       63 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/signals.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.898132 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1052 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      441 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/client.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      322 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/creation.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      205 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/features.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      432 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/introspection.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1014 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/operations.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      215 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/backends/sqlite3/schema.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2930 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/backends/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.901465 django_stubs-5.0.0/django-stubs/db/migrations/
--rw-r--r--   0 marti     (1000) marti     (1000)      265 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2830 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/autodetector.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      664 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1770 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/migrations/executor.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2404 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/migrations/graph.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1960 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/loader.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1161 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/db/migrations/migration.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.901465 django_stubs-5.0.0/django-stubs/db/migrations/operations/
--rw-r--r--   0 marti     (1000) marti     (1000)     1159 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/migrations/operations/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1522 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/migrations/operations/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1251 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/migrations/operations/fields.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     5188 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/db/migrations/operations/models.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1965 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/migrations/operations/special.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      974 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/migrations/operations/utils.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      290 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/optimizer.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1109 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/questioner.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      887 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/migrations/recorder.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1835 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/serializer.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4952 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/migrations/state.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      195 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/utils.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1235 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/migrations/writer.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.901465 django_stubs-5.0.0/django-stubs/db/models/
--rw-r--r--   0 marti     (1000) marti     (1000)     4647 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      821 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/aggregates.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4692 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       96 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/models/constants.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2994 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/constraints.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3733 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/deletion.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2021 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/enums.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)    10469 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/expressions.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.904798 django_stubs-5.0.0/django-stubs/db/models/fields/
--rw-r--r--   0 marti     (1000) marti     (1000)    22400 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/fields/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4525 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/fields/files.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1766 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/fields/generated.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3929 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/fields/json.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      515 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/models/fields/mixins.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      161 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/models/fields/proxy.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)    12081 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/fields/related.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     6978 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/fields/related_descriptors.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1393 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/models/fields/related_lookups.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4804 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/fields/reverse_related.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.904798 django_stubs-5.0.0/django-stubs/db/models/functions/
--rw-r--r--   0 marti     (1000) marti     (1000)     3407 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/functions/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      567 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/functions/comparison.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1393 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/functions/datetime.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1222 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/models/functions/math.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      100 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/models/functions/mixins.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4746 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/functions/text.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      988 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/functions/window.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2266 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/db/models/indexes.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     6017 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/lookups.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     8022 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/manager.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     5288 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/models/options.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)    11068 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/query.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3549 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/query_utils.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      908 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/db/models/signals.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.904798 django_stubs-5.0.0/django-stubs/db/models/sql/
--rw-r--r--   0 marti     (1000) marti     (1000)      284 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/models/sql/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     6753 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/sql/compiler.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      286 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/models/sql/constants.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1791 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/db/models/sql/datastructures.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     9563 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/sql/query.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1619 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/db/models/sql/subqueries.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2259 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/sql/where.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      551 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/db/models/utils.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2178 2023-06-02 14:08:54.000000 django_stubs-5.0.0/django-stubs/db/transaction.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2120 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/db/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.904798 django_stubs-5.0.0/django-stubs/dispatch/
--rw-r--r--   0 marti     (1000) marti     (1000)      116 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/dispatch/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1453 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/dispatch/dispatcher.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.904798 django_stubs-5.0.0/django-stubs/forms/
--rw-r--r--   0 marti     (1000) marti     (1000)     4083 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/forms/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2940 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/forms/boundfield.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)    20466 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/forms/fields.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3164 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/forms/forms.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3902 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/forms/formsets.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)    12164 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/forms/models.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1191 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/forms/renderers.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2479 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/forms/utils.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)    10519 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/forms/widgets.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.908132 django_stubs-5.0.0/django-stubs/http/
--rw-r--r--   0 marti     (1000) marti     (1000)     1332 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/http/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      108 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/http/cookie.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2007 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/http/multipartparser.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     8951 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/http/request.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     5834 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/http/response.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.908132 django_stubs-5.0.0/django-stubs/middleware/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/middleware/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1063 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/middleware/cache.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      387 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/middleware/clickjacking.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      968 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/middleware/common.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1794 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/middleware/csrf.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      339 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/middleware/gzip.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      369 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/middleware/http.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      417 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/middleware/locale.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      645 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/middleware/security.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1807 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/shortcuts.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.908132 django_stubs-5.0.0/django-stubs/template/
--rw-r--r--   0 marti     (1000) marti     (1000)      756 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/__init__.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.908132 django_stubs-5.0.0/django-stubs/template/backends/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/backends/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      974 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/template/backends/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1062 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/backends/django.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      402 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/template/backends/dummy.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      931 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/template/backends/jinja2.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      215 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/backends/utils.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     5561 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/template/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3368 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/template/context.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      631 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/context_processors.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3540 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/template/defaultfilters.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     6912 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/defaulttags.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2224 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/template/engine.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      511 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3244 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/library.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      670 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/template/loader.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2289 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/template/loader_tags.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.911465 django_stubs-5.0.0/django-stubs/template/loaders/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/loaders/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       88 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/loaders/app_directories.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      488 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/loaders/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      554 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/loaders/cached.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      518 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/loaders/filesystem.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      323 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/loaders/locmem.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2434 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/template/response.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1246 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/template/smartif.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      648 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/template/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.911465 django_stubs-5.0.0/django-stubs/templatetags/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/templatetags/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      629 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/templatetags/cache.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3492 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/templatetags/i18n.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      410 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/templatetags/l10n.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1123 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/templatetags/static.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1039 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/templatetags/tz.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.911465 django_stubs-5.0.0/django-stubs/test/
--rw-r--r--   0 marti     (1000) marti     (1000)      890 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/test/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)    13259 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/test/client.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1345 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/test/html.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     6645 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/test/runner.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      539 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/test/selenium.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1307 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/test/signals.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     9605 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/test/testcases.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     6346 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/test/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.911465 django_stubs-5.0.0/django-stubs/urls/
--rw-r--r--   0 marti     (1000) marti     (1000)     1578 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/urls/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      922 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/urls/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1851 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/urls/conf.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      996 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/urls/converters.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      102 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/urls/exceptions.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4668 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/urls/resolvers.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      157 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/urls/utils.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.914798 django_stubs-5.0.0/django-stubs/utils/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      286 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/_os.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1487 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/utils/archive.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      230 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/asyncio.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2872 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/autoreload.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1287 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/cache.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1101 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/choices.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1300 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/connection.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      570 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/crypto.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4759 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/datastructures.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2005 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/dateformat.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      505 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/dateparse.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      156 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/dates.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      640 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/deconstruct.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1155 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/decorators.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1829 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/deprecation.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      198 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/duration.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3195 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/utils/encoding.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2803 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/utils/feedgenerator.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1850 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/utils/formats.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4231 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/functional.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       66 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/hashable.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2510 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/html.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1307 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/http.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      483 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/inspect.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      175 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/ipv6.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)       61 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/itercompat.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      714 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/jslex.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1742 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/utils/log.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      242 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/lorem_ipsum.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      312 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/module_loading.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      319 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/numberformat.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      917 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/regex_helper.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      589 2023-06-29 17:05:25.000000 django_stubs-5.0.0/django-stubs/utils/safestring.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      627 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/termcolors.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2392 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/text.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      423 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/timesince.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1557 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/timezone.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.918132 django_stubs-5.0.0/django-stubs/utils/translation/
--rw-r--r--   0 marti     (1000) marti     (1000)     2033 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/translation/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      286 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/utils/translation/reloader.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      335 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/translation/template.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      801 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/translation/trans_null.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3000 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/utils/translation/trans_real.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      986 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/tree.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      518 2023-06-27 17:49:10.000000 django_stubs-5.0.0/django-stubs/utils/version.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      424 2023-12-05 19:01:16.000000 django_stubs-5.0.0/django-stubs/utils/xmlutils.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.918132 django_stubs-5.0.0/django-stubs/views/
--rw-r--r--   0 marti     (1000) marti     (1000)       39 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      323 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/views/csrf.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3125 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/views/debug.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.918132 django_stubs-5.0.0/django-stubs/views/decorators/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/decorators/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      347 2023-06-02 14:08:54.000000 django_stubs-5.0.0/django-stubs/views/decorators/cache.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      274 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/decorators/clickjacking.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      162 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/decorators/common.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      427 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/decorators/csrf.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      361 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/views/decorators/debug.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      146 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/decorators/gzip.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      718 2023-06-02 14:08:54.000000 django_stubs-5.0.0/django-stubs/views/decorators/http.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      218 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/decorators/vary.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      807 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/views/defaults.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.918132 django_stubs-5.0.0/django-stubs/views/generic/
--rw-r--r--   0 marti     (1000) marti     (1000)      797 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/generic/__init__.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     2428 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/views/generic/base.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     4561 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/views/generic/dates.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1109 2023-03-15 16:53:32.000000 django_stubs-5.0.0/django-stubs/views/generic/detail.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     3393 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/views/generic/edit.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1963 2023-10-18 16:41:31.000000 django_stubs-5.0.0/django-stubs/views/generic/list.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)     1091 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/views/i18n.pyi
--rw-r--r--   0 marti     (1000) marti     (1000)      502 2024-04-30 10:01:49.000000 django_stubs-5.0.0/django-stubs/views/static.pyi
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.921465 django_stubs-5.0.0/django_stubs.egg-info/
--rw-r--r--   0 marti     (1000) marti     (1000)    16027 2024-04-30 10:03:06.000000 django_stubs-5.0.0/django_stubs.egg-info/PKG-INFO
--rw-r--r--   0 marti     (1000) marti     (1000)    30353 2024-04-30 10:03:06.000000 django_stubs-5.0.0/django_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 marti     (1000) marti     (1000)        1 2024-04-30 10:03:06.000000 django_stubs-5.0.0/django_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 marti     (1000) marti     (1000)      151 2024-04-30 10:03:06.000000 django_stubs-5.0.0/django_stubs.egg-info/requires.txt
--rw-r--r--   0 marti     (1000) marti     (1000)       32 2024-04-30 10:03:06.000000 django_stubs-5.0.0/django_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.918132 django_stubs-5.0.0/mypy_django_plugin/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/mypy_django_plugin/__init__.py
--rw-r--r--   0 marti     (1000) marti     (1000)     4784 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/config.py
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.921465 django_stubs-5.0.0/mypy_django_plugin/django/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/mypy_django_plugin/django/__init__.py
--rw-r--r--   0 marti     (1000) marti     (1000)    22288 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/django/context.py
--rw-r--r--   0 marti     (1000) marti     (1000)      227 2023-03-15 16:53:32.000000 django_stubs-5.0.0/mypy_django_plugin/errorcodes.py
--rw-r--r--   0 marti     (1000) marti     (1000)       89 2023-06-27 17:49:10.000000 django_stubs-5.0.0/mypy_django_plugin/exceptions.py
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.921465 django_stubs-5.0.0/mypy_django_plugin/lib/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/mypy_django_plugin/lib/__init__.py
--rw-r--r--   0 marti     (1000) marti     (1000)     3087 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/lib/fullnames.py
--rw-r--r--   0 marti     (1000) marti     (1000)    17822 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/lib/helpers.py
--rw-r--r--   0 marti     (1000) marti     (1000)    15367 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/main.py
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/mypy_django_plugin/py.typed
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.921465 django_stubs-5.0.0/mypy_django_plugin/transformers/
--rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-03-15 16:53:32.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/__init__.py
--rw-r--r--   0 marti     (1000) marti     (1000)    11307 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/fields.py
--rw-r--r--   0 marti     (1000) marti     (1000)     1787 2023-06-27 17:49:10.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/forms.py
--rw-r--r--   0 marti     (1000) marti     (1000)     1313 2023-06-27 17:49:10.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/functional.py
--rw-r--r--   0 marti     (1000) marti     (1000)     3104 2023-03-15 16:53:32.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/init_create.py
--rw-r--r--   0 marti     (1000) marti     (1000)    25150 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/managers.py
--rw-r--r--   0 marti     (1000) marti     (1000)    10079 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/manytomany.py
--rw-r--r--   0 marti     (1000) marti     (1000)     1938 2023-06-27 17:49:10.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/meta.py
--rw-r--r--   0 marti     (1000) marti     (1000)    49032 2024-04-30 10:01:49.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/models.py
--rw-r--r--   0 marti     (1000) marti     (1000)     2821 2023-12-05 19:01:16.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/orm_lookups.py
--rw-r--r--   0 marti     (1000) marti     (1000)    13235 2023-10-23 19:46:47.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/querysets.py
--rw-r--r--   0 marti     (1000) marti     (1000)     2048 2023-06-27 17:49:10.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/request.py
--rw-r--r--   0 marti     (1000) marti     (1000)     2495 2023-06-27 17:49:10.000000 django_stubs-5.0.0/mypy_django_plugin/transformers/settings.py
--rw-r--r--   0 marti     (1000) marti     (1000)     1841 2024-04-30 10:01:49.000000 django_stubs-5.0.0/pyproject.toml
--rw-r--r--   0 marti     (1000) marti     (1000)       38 2024-04-30 10:03:06.921465 django_stubs-5.0.0/setup.cfg
--rw-r--r--   0 marti     (1000) marti     (1000)     2348 2024-04-30 10:01:49.000000 django_stubs-5.0.0/setup.py
-drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:03:06.921465 django_stubs-5.0.0/tests/
--rw-r--r--   0 marti     (1000) marti     (1000)     7607 2024-04-30 10:01:49.000000 django_stubs-5.0.0/tests/test_error_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.359205 django_stubs-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 11:22:12.000000 django_stubs-5.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15437 2024-05-27 11:22:14.359205 django_stubs-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-05-27 11:22:12.000000 django_stubs-5.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.231204 django_stubs-5.0.1/django-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.231204 django_stubs-5.0.1/django-stubs/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/apps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/apps/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/apps/registry.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.231204 django_stubs-5.0.1/django-stubs/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/conf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17238 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/conf/global_settings.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.231204 django_stubs-5.0.1/django-stubs/conf/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/conf/locale/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.231204 django_stubs-5.0.1/django-stubs/conf/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/conf/urls/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/conf/urls/i18n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/conf/urls/static.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.231204 django_stubs-5.0.1/django-stubs/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.235204 django_stubs-5.0.1/django-stubs/contrib/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/actions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/filters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/forms.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/helpers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.235204 django_stubs-5.0.1/django-stubs/contrib/admin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/sites.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.235204 django_stubs-5.0.1/django-stubs/contrib/admin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/templatetags/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/templatetags/admin_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/templatetags/admin_modify.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/templatetags/admin_urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/templatetags/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/templatetags/log.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/tests.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.235204 django_stubs-5.0.1/django-stubs/contrib/admin/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/views/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/views/autocomplete.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/views/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/views/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admin/widgets.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.239205 django_stubs-5.0.1/django-stubs/contrib/admindocs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admindocs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admindocs/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admindocs/middleware.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admindocs/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admindocs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/admindocs/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.243204 django_stubs-5.0.1/django-stubs/contrib/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/backends.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/base_user.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/context_processors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/forms.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.243204 django_stubs-5.0.1/django-stubs/contrib/auth/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/handlers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/handlers/modwsgi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/hashers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.243204 django_stubs-5.0.1/django-stubs/contrib/auth/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/management/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.243204 django_stubs-5.0.1/django-stubs/contrib/auth/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/management/commands/changepassword.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/management/commands/createsuperuser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.243204 django_stubs-5.0.1/django-stubs/contrib/auth/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/password_validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/tokens.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/validators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/auth/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.243204 django_stubs-5.0.1/django-stubs/contrib/contenttypes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/contenttypes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/contenttypes/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/contenttypes/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/contenttypes/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/contenttypes/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/contenttypes/forms.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.243204 django_stubs-5.0.1/django-stubs/contrib/contenttypes/management/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/contenttypes/management/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.243204 django_stubs-5.0.1/django-stubs/contrib/contenttypes/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/contenttypes/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.243204 django_stubs-5.0.1/django-stubs/contrib/contenttypes/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/contenttypes/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/contenttypes/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/contenttypes/prefetch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/contenttypes/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.247204 django_stubs-5.0.1/django-stubs/contrib/flatpages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/flatpages/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/flatpages/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/flatpages/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/flatpages/forms.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/flatpages/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.247204 django_stubs-5.0.1/django-stubs/contrib/flatpages/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/flatpages/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/flatpages/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/flatpages/sitemaps.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.247204 django_stubs-5.0.1/django-stubs/contrib/flatpages/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/flatpages/templatetags/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/flatpages/templatetags/flatpages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/flatpages/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/flatpages/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.247204 django_stubs-5.0.1/django-stubs/contrib/gis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.247204 django_stubs-5.0.1/django-stubs/contrib/gis/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/admin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/admin/options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/apps.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.247204 django_stubs-5.0.1/django-stubs/contrib/gis/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.251205 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.251205 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/base/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/base/adapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/base/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/base/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/base/operations.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.251205 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/mysql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/mysql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/mysql/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/mysql/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/mysql/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/mysql/schema.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.251205 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/oracle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/oracle/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/oracle/adapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/oracle/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/oracle/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/oracle/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/oracle/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/oracle/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/oracle/schema.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.255205 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/postgis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/postgis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/postgis/adapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/postgis/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/postgis/const.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/postgis/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/postgis/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/postgis/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/postgis/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/postgis/pgraster.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/postgis/schema.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.255205 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/spatialite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/spatialite/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/spatialite/adapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/spatialite/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/spatialite/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/spatialite/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/spatialite/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/spatialite/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.259204 django_stubs-5.0.1/django-stubs/contrib/gis/db/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/models/aggregates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/models/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/models/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/models/lookups.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/models/proxy.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.259204 django_stubs-5.0.1/django-stubs/contrib/gis/db/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/models/sql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/db/models/sql/conversion.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/feeds.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.259204 django_stubs-5.0.1/django-stubs/contrib/gis/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/forms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/forms/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/forms/widgets.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.259204 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/datasource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/driver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/envelope.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/feature.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/field.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/geometries.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/geomtype.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/layer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/libgdal.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.263205 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/prototypes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/prototypes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/prototypes/ds.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/prototypes/generation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/prototypes/geom.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/prototypes/raster.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/prototypes/srs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.263205 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/raster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/raster/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/raster/band.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/raster/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/raster/const.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/raster/source.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/gdal/srs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.263205 django_stubs-5.0.1/django-stubs/contrib/gis/geoip2/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geoip2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geoip2/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geoip2/resources.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geometry.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.267205 django_stubs-5.0.1/django-stubs/contrib/gis/geos/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/collections.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/coordseq.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/geometry.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/io.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/libgeos.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/linestring.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/mutable_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/point.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/polygon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/prepared.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.267205 django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/errcheck.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/geom.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/io.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/misc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/predicates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/prepared.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/threadsafe.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/topology.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/measure.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/ptr.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.267205 django_stubs-5.0.1/django-stubs/contrib/gis/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/serializers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/serializers/geojson.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/shortcuts.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.267205 django_stubs-5.0.1/django-stubs/contrib/gis/sitemaps/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/sitemaps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/sitemaps/kml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/sitemaps/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.271205 django_stubs-5.0.1/django-stubs/contrib/gis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/utils/layermapping.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/utils/ogrinfo.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/utils/ogrinspect.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/utils/srs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/gis/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.271205 django_stubs-5.0.1/django-stubs/contrib/humanize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/humanize/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/humanize/apps.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.271205 django_stubs-5.0.1/django-stubs/contrib/humanize/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/humanize/templatetags/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/humanize/templatetags/humanize.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.271205 django_stubs-5.0.1/django-stubs/contrib/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/messages/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/messages/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/messages/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/messages/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/messages/context_processors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/messages/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.271205 django_stubs-5.0.1/django-stubs/contrib/messages/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/messages/storage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/messages/storage/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/messages/storage/cookie.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/messages/storage/fallback.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/messages/storage/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/messages/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/messages/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/messages/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.275205 django_stubs-5.0.1/django-stubs/contrib/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.275205 django_stubs-5.0.1/django-stubs/contrib/postgres/aggregates/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/aggregates/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/aggregates/general.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/aggregates/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/aggregates/statistics.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/constraints.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/expressions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.279205 django_stubs-5.0.1/django-stubs/contrib/postgres/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/fields/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/fields/array.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/fields/citext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/fields/hstore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/fields/jsonb.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/fields/ranges.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/fields/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.279205 django_stubs-5.0.1/django-stubs/contrib/postgres/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/forms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/forms/array.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/forms/hstore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/forms/ranges.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/indexes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/lookups.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/serializers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/postgres/validators.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.279205 django_stubs-5.0.1/django-stubs/contrib/redirects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/redirects/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/redirects/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/redirects/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/redirects/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.279205 django_stubs-5.0.1/django-stubs/contrib/redirects/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/redirects/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/redirects/models.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.279205 django_stubs-5.0.1/django-stubs/contrib/sessions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/apps.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.283205 django_stubs-5.0.1/django-stubs/contrib/sessions/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/backends/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/backends/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/backends/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/backends/cached_db.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/backends/db.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/backends/file.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/backends/signed_cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/base_session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.283205 django_stubs-5.0.1/django-stubs/contrib/sessions/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/management/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.283205 django_stubs-5.0.1/django-stubs/contrib/sessions/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/management/commands/clearsessions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.283205 django_stubs-5.0.1/django-stubs/contrib/sessions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sessions/serializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.283205 django_stubs-5.0.1/django-stubs/contrib/sitemaps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sitemaps/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sitemaps/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sitemaps/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.283205 django_stubs-5.0.1/django-stubs/contrib/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sites/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sites/admin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sites/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sites/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sites/management.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sites/managers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sites/middleware.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.283205 django_stubs-5.0.1/django-stubs/contrib/sites/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sites/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sites/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sites/requests.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/sites/shortcuts.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.287205 django_stubs-5.0.1/django-stubs/contrib/staticfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/finders.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/handlers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.287205 django_stubs-5.0.1/django-stubs/contrib/staticfiles/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/management/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.287205 django_stubs-5.0.1/django-stubs/contrib/staticfiles/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/management/commands/findstatic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/management/commands/runserver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/storage.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/testing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/staticfiles/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.287205 django_stubs-5.0.1/django-stubs/contrib/syndication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/syndication/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/syndication/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/contrib/syndication/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.291205 django_stubs-5.0.1/django-stubs/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/asgi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.291205 django_stubs-5.0.1/django-stubs/core/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/cache/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.291205 django_stubs-5.0.1/django-stubs/core/cache/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/cache/backends/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/cache/backends/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/cache/backends/db.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/cache/backends/dummy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/cache/backends/filebased.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/cache/backends/locmem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/cache/backends/memcached.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/cache/backends/redis.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/cache/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.295205 django_stubs-5.0.1/django-stubs/core/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/async_checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/caches.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.295205 django_stubs-5.0.1/django-stubs/core/checks/compatibility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/compatibility/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/compatibility/django_4_0.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/database.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/files.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/messages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/model_checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/registry.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.295205 django_stubs-5.0.1/django-stubs/core/checks/security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/security/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/security/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/security/csrf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/security/sessions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/templates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/translation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/checks/urls.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.295205 django_stubs-5.0.1/django-stubs/core/files/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/images.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/locks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/move.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.295205 django_stubs-5.0.1/django-stubs/core/files/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/storage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/storage/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/storage/filesystem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/storage/handler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/storage/memory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/storage/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/temp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/uploadedfile.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/uploadhandler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/files/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.299205 django_stubs-5.0.1/django-stubs/core/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/handlers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/handlers/asgi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/handlers/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/handlers/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/handlers/wsgi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.299205 django_stubs-5.0.1/django-stubs/core/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/mail/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.299205 django_stubs-5.0.1/django-stubs/core/mail/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/mail/backends/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/mail/backends/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/mail/backends/console.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/mail/backends/dummy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/mail/backends/filebased.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/mail/backends/locmem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/mail/backends/smtp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/mail/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/mail/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.299205 django_stubs-5.0.1/django-stubs/core/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/color.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.307205 django_stubs-5.0.1/django-stubs/core/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/check.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/compilemessages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/createcachetable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/dbshell.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/diffsettings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/dumpdata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/flush.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/inspectdb.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/loaddata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/makemessages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/makemigrations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/migrate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/optimizemigration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/runserver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/sendtestemail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/shell.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/showmigrations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/sqlflush.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/sqlmigrate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/sqlsequencereset.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/squashmigrations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/startapp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/startproject.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/commands/testserver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/sql.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/templates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/management/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/paginator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.307205 django_stubs-5.0.1/django-stubs/core/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/serializers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/serializers/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/serializers/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/serializers/jsonl.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/serializers/python.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/serializers/pyyaml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/serializers/xml_serializer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.307205 django_stubs-5.0.1/django-stubs/core/servers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/servers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/servers/basehttp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/signing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/validators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/core/wsgi.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.307205 django_stubs-5.0.1/django-stubs/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.307205 django_stubs-5.0.1/django-stubs/db/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.311205 django_stubs-5.0.1/django-stubs/db/backends/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/base/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/base/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/base/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/base/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/base/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/base/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/base/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/base/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/base/validation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/ddl_references.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.311205 django_stubs-5.0.1/django-stubs/db/backends/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/dummy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/dummy/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/dummy/features.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.311205 django_stubs-5.0.1/django-stubs/db/backends/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/mysql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/mysql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/mysql/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/mysql/compiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/mysql/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/mysql/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/mysql/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/mysql/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/mysql/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/mysql/validation.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.315205 django_stubs-5.0.1/django-stubs/db/backends/oracle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/oracle/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/oracle/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/oracle/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/oracle/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/oracle/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/oracle/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/oracle/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/oracle/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/oracle/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/oracle/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/oracle/validation.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.315205 django_stubs-5.0.1/django-stubs/db/backends/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/postgresql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/postgresql/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/postgresql/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/postgresql/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/postgresql/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/postgresql/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/postgresql/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/postgresql/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/signals.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.319205 django_stubs-5.0.1/django-stubs/db/backends/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/sqlite3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/sqlite3/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/sqlite3/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/sqlite3/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/sqlite3/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/sqlite3/introspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/sqlite3/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/sqlite3/schema.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/backends/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.319205 django_stubs-5.0.1/django-stubs/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/autodetector.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/executor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/graph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/loader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/migration.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.319205 django_stubs-5.0.1/django-stubs/db/migrations/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/operations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/operations/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/operations/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/operations/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/operations/special.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/operations/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/optimizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/questioner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/recorder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/state.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/migrations/writer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.323205 django_stubs-5.0.1/django-stubs/db/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/aggregates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/constraints.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/deletion.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/expressions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.327205 django_stubs-5.0.1/django-stubs/db/models/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)    22430 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/fields/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/fields/files.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/fields/generated.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/fields/json.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/fields/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/fields/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/fields/related.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/fields/related_descriptors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/fields/related_lookups.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/fields/reverse_related.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.327205 django_stubs-5.0.1/django-stubs/db/models/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/functions/comparison.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/functions/datetime.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/functions/math.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/functions/mixins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/functions/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/functions/window.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/indexes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/lookups.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/options.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/query_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/signals.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.327205 django_stubs-5.0.1/django-stubs/db/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/sql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/sql/compiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/sql/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/sql/datastructures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9357 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/sql/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/sql/subqueries.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/sql/where.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/models/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/db/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.327205 django_stubs-5.0.1/django-stubs/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/dispatch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/dispatch/dispatcher.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.331205 django_stubs-5.0.1/django-stubs/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/forms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/forms/boundfield.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20507 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/forms/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/forms/forms.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/forms/formsets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12178 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/forms/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/forms/renderers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/forms/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/forms/widgets.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.331205 django_stubs-5.0.1/django-stubs/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/http/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/http/cookie.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/http/multipartparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/http/request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/http/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.331205 django_stubs-5.0.1/django-stubs/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/middleware/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/middleware/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/middleware/clickjacking.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/middleware/common.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/middleware/csrf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/middleware/gzip.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/middleware/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/middleware/locale.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/middleware/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/shortcuts.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.335205 django_stubs-5.0.1/django-stubs/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.335205 django_stubs-5.0.1/django-stubs/template/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/backends/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/backends/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/backends/django.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/backends/dummy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/backends/jinja2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/backends/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/context_processors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/defaultfilters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/defaulttags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/engine.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/library.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/loader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/loader_tags.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.339205 django_stubs-5.0.1/django-stubs/template/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/loaders/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/loaders/app_directories.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/loaders/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/loaders/cached.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/loaders/filesystem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/loaders/locmem.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/smartif.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/template/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.339205 django_stubs-5.0.1/django-stubs/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/templatetags/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/templatetags/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/templatetags/i18n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/templatetags/l10n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/templatetags/static.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/templatetags/tz.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.339205 django_stubs-5.0.1/django-stubs/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/test/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13259 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/test/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/test/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/test/runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/test/selenium.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/test/signals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/test/testcases.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/test/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.343205 django_stubs-5.0.1/django-stubs/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/urls/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/urls/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/urls/conf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/urls/converters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/urls/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/urls/resolvers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/urls/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.347205 django_stubs-5.0.1/django-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/_os.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/archive.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/asyncio.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/autoreload.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/choices.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/crypto.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/datastructures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/dateformat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/dateparse.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/dates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/deconstruct.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/deprecation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/duration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/encoding.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/feedgenerator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/formats.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/functional.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/hashable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/inspect.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/ipv6.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/itercompat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/jslex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/log.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/lorem_ipsum.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/module_loading.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/numberformat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/regex_helper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/safestring.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/termcolors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/timesince.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/timezone.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.351205 django_stubs-5.0.1/django-stubs/utils/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/translation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/translation/reloader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/translation/template.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/translation/trans_null.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/translation/trans_real.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/tree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/utils/xmlutils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.351205 django_stubs-5.0.1/django-stubs/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/csrf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/debug.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.351205 django_stubs-5.0.1/django-stubs/views/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/decorators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/decorators/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/decorators/clickjacking.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/decorators/common.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/decorators/csrf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/decorators/debug.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/decorators/gzip.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/decorators/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/decorators/vary.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/defaults.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.355205 django_stubs-5.0.1/django-stubs/views/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/generic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/generic/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/generic/dates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/generic/detail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/generic/edit.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/generic/list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/i18n.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-27 11:22:12.000000 django_stubs-5.0.1/django-stubs/views/static.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.359205 django_stubs-5.0.1/django_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15437 2024-05-27 11:22:14.000000 django_stubs-5.0.1/django_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30396 2024-05-27 11:22:14.000000 django_stubs-5.0.1/django_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:22:14.000000 django_stubs-5.0.1/django_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-27 11:22:14.000000 django_stubs-5.0.1/django_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 11:22:14.000000 django_stubs-5.0.1/django_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.355205 django_stubs-5.0.1/mypy_django_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.355205 django_stubs-5.0.1/mypy_django_plugin/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22288 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/django/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.355205 django_stubs-5.0.1/mypy_django_plugin/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/lib/fullnames.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17822 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/lib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15411 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.359205 django_stubs-5.0.1/mypy_django_plugin/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/transformers/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/transformers/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/transformers/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/transformers/init_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25137 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/transformers/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/transformers/manytomany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/transformers/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49280 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/transformers/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/transformers/orm_lookups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/transformers/querysets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/transformers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 11:22:12.000000 django_stubs-5.0.1/mypy_django_plugin/transformers/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-27 11:22:12.000000 django_stubs-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:22:14.359205 django_stubs-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-27 11:22:12.000000 django_stubs-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:22:14.359205 django_stubs-5.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-27 11:22:12.000000 django_stubs-5.0.1/tests/test_error_handling.py
```

### Comparing `django_stubs-5.0.0/LICENSE.md` & `django_stubs-5.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/PKG-INFO` & `django_stubs-5.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stubs
-Version: 5.0.0
+Version: 5.0.1
 Summary: Mypy stubs for Django
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
@@ -15,30 +15,31 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: django
 Requires-Dist: asgiref
 Requires-Dist: django-stubs-ext>=5.0.0
 Requires-Dist: tomli; python_version < "3.11"
-Requires-Dist: typing-extensions
+Requires-Dist: typing-extensions>=4.11.0
 Requires-Dist: types-PyYAML
 Provides-Extra: compatible-mypy
 Requires-Dist: mypy~=1.10.0; extra == "compatible-mypy"
 Provides-Extra: redis
 Requires-Dist: redis; extra == "redis"
+Provides-Extra: oracle
+Requires-Dist: oracledb; extra == "oracle"
 
 <img src="https://raw.githubusercontent.com/typeddjango/django-stubs/master/logo.svg" alt="django-stubs">
 
 [![Build status](https://github.com/typeddjango/django-stubs/workflows/test/badge.svg?branch=master&event=push)](https://github.com/typeddjango/django-stubs/actions?query=workflow%3Atest)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Gitter](https://badges.gitter.im/mypy-django/Lobby.svg)](https://gitter.im/mypy-django/Lobby)
 [![StackOverflow](https://shields.io/badge/ask-stackoverflow-orange?logo=stackoverflow)](https://stackoverflow.com/questions/tagged/django-stubs)
@@ -83,14 +84,15 @@
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
+| 5.0.1          | 1.10.x       | 5.0            | 4.2                    | 3.8 - 3.12     |
 | 5.0.0          | 1.10.x       | 5.0            | 4.2, 4.1               | 3.8 - 3.12     |
 | 4.2.7          | 1.7.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.6          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.5          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.4          | 1.5.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.3          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
@@ -288,39 +290,14 @@
     return m.foo  # OK, since we said field "foo" was allowed
 
 
 func(MyModel.objects.annotate(foo=Value("")).get(id=1))  # OK
 func(MyModel.objects.annotate(bar=Value("")).get(id=1))  # Error
 ```
 
-### How do I check if something is an instance of QuerySet in runtime?
-
-A limitation of making `QuerySet` generic is that you can not use
-it for `isinstance` checks.
-
-```python
-from django.db.models.query import QuerySet
-
-def foo(obj: object) -> None:
-    if isinstance(obj, QuerySet): # Error: Parameterized generics cannot be used with class or instance checks
-        ...
-```
-
-To get around with this issue without making `QuerySet` non-generic,
-Django-stubs provides `django_stubs_ext.QuerySetAny`, a non-generic
-variant of `QuerySet` suitable for runtime type checking:
-
-```python
-from django_stubs_ext import QuerySetAny
-
-def foo(obj: object) -> None:
-    if isinstance(obj, QuerySetAny):  # OK
-        ...
-```
-
 ### Why am I getting incompatible argument type mentioning `_StrPromise`?
 
 The lazy translation functions of Django (such as `gettext_lazy`) return a `Promise` instead of `str`. These two types [cannot be used interchangeably](https://github.com/typeddjango/django-stubs/pull/1139#issuecomment-1232167698). The return type of these functions was therefore [changed](https://github.com/typeddjango/django-stubs/pull/689) to reflect that.
 
 If you encounter this error in your own code, you can either cast the `Promise` to `str` (causing the translation to be evaluated), or use the `StrPromise` or `StrOrPromise` types from `django-stubs-ext` in type hints. Which solution to choose depends depends on the particular case. See [working with lazy translation objects](https://docs.djangoproject.com/en/4.1/topics/i18n/translation/#working-with-lazy-translation-objects) in the Django documentation for more information.
 
 If this is reported on Django code, please report an issue or open a pull request to fix the type hints.
```

### Comparing `django_stubs-5.0.0/README.md` & `django_stubs-5.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
+| 5.0.1          | 1.10.x       | 5.0            | 4.2                    | 3.8 - 3.12     |
 | 5.0.0          | 1.10.x       | 5.0            | 4.2, 4.1               | 3.8 - 3.12     |
 | 4.2.7          | 1.7.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.6          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.5          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.4          | 1.5.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.3          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
@@ -250,39 +251,14 @@
     return m.foo  # OK, since we said field "foo" was allowed
 
 
 func(MyModel.objects.annotate(foo=Value("")).get(id=1))  # OK
 func(MyModel.objects.annotate(bar=Value("")).get(id=1))  # Error
 ```
 
-### How do I check if something is an instance of QuerySet in runtime?
-
-A limitation of making `QuerySet` generic is that you can not use
-it for `isinstance` checks.
-
-```python
-from django.db.models.query import QuerySet
-
-def foo(obj: object) -> None:
-    if isinstance(obj, QuerySet): # Error: Parameterized generics cannot be used with class or instance checks
-        ...
-```
-
-To get around with this issue without making `QuerySet` non-generic,
-Django-stubs provides `django_stubs_ext.QuerySetAny`, a non-generic
-variant of `QuerySet` suitable for runtime type checking:
-
-```python
-from django_stubs_ext import QuerySetAny
-
-def foo(obj: object) -> None:
-    if isinstance(obj, QuerySetAny):  # OK
-        ...
-```
-
 ### Why am I getting incompatible argument type mentioning `_StrPromise`?
 
 The lazy translation functions of Django (such as `gettext_lazy`) return a `Promise` instead of `str`. These two types [cannot be used interchangeably](https://github.com/typeddjango/django-stubs/pull/1139#issuecomment-1232167698). The return type of these functions was therefore [changed](https://github.com/typeddjango/django-stubs/pull/689) to reflect that.
 
 If you encounter this error in your own code, you can either cast the `Promise` to `str` (causing the translation to be evaluated), or use the `StrPromise` or `StrOrPromise` types from `django-stubs-ext` in type hints. Which solution to choose depends depends on the particular case. See [working with lazy translation objects](https://docs.djangoproject.com/en/4.1/topics/i18n/translation/#working-with-lazy-translation-objects) in the Django documentation for more information.
 
 If this is reported on Django code, please report an issue or open a pull request to fix the type hints.
```

### Comparing `django_stubs-5.0.0/django-stubs/apps/config.pyi` & `django_stubs-5.0.1/django-stubs/apps/config.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/apps/registry.pyi` & `django_stubs-5.0.1/django-stubs/apps/registry.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/conf/__init__.pyi` & `django_stubs-5.0.1/django-stubs/conf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/conf/global_settings.pyi` & `django_stubs-5.0.1/django-stubs/conf/global_settings.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/conf/urls/__init__.pyi` & `django_stubs-5.0.1/django-stubs/conf/urls/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 from typing_extensions import TypeAlias
 
 handler400: str | Callable[..., HttpResponse]
 handler403: str | Callable[..., HttpResponse]
 handler404: str | Callable[..., HttpResponse]
 handler500: str | Callable[..., HttpResponse]
 
-IncludedURLConf: TypeAlias = tuple[Sequence[URLResolver | URLPattern], str | None, str | None]
+_IncludedURLConf: TypeAlias = tuple[Sequence[URLResolver | URLPattern], str | None, str | None]
 
 # Deprecated
 @overload
 def url(
     regex: str, view: Callable[..., HttpResponseBase], kwargs: dict[str, Any] | None = ..., name: str | None = ...
 ) -> URLPattern: ...
 @overload
 def url(
-    regex: str, view: IncludedURLConf, kwargs: dict[str, Any] | None = ..., name: str | None = ...
+    regex: str, view: _IncludedURLConf, kwargs: dict[str, Any] | None = ..., name: str | None = ...
 ) -> URLResolver: ...
 @overload
 def url(
     regex: str,
     view: Sequence[URLResolver | str],
     kwargs: dict[str, Any] | None = ...,
     name: str | None = ...,
```

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/__init__.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/checks.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/checks.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/decorators.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/decorators.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/filters.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/filters.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/helpers.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/helpers.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/models.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/models.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/options.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/options.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/sites.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/sites.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/admin_list.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/templatetags/admin_list.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/admin_modify.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/templatetags/admin_modify.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/templatetags/base.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/templatetags/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/tests.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/tests.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/utils.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/utils.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/views/main.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/views/main.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from collections.abc import Callable, Iterable, Sequence
 from typing import Any, Literal
 
+from django import forms
 from django.contrib.admin.filters import ListFilter
 from django.contrib.admin.options import ModelAdmin, _DisplayT, _ListFilterT
 from django.db.models.base import Model
 from django.db.models.expressions import Expression
 from django.db.models.options import Options
 from django.db.models.query import QuerySet
 from django.forms.formsets import BaseFormSet
@@ -13,15 +14,18 @@
 ALL_VAR: str
 ORDER_VAR: str
 PAGE_VAR: str
 SEARCH_VAR: str
 ERROR_FLAG: str
 IGNORED_PARAMS: tuple[str, ...]
 
+class ChangeListSearchForm(forms.Form): ...
+
 class ChangeList:
+    search_form_class: type[forms.Form]
     model: type[Model]
     opts: Options
     lookup_opts: Options
     root_queryset: QuerySet
     list_display: _DisplayT
     list_display_links: _DisplayT
     list_filter: Sequence[_ListFilterT]
@@ -33,16 +37,21 @@
     list_max_show_all: int
     model_admin: ModelAdmin
     preserved_filters: str
     sortable_by: Sequence[str] | None
     page_num: int
     show_all: bool
     is_popup: bool
+    add_facets: bool
+    is_facets_optional: bool
     to_field: Any
     params: dict[str, Any]
+    filter_params: dict[str, list[str]]
+    remove_facet_link: str
+    add_facet_link: str
     list_editable: Sequence[str]
     query: str
     queryset: Any
     title: str
     pk_attname: str
     formset: BaseFormSet | None
     def __init__(
```

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admin/widgets.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admin/widgets.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,26 @@
         self,
         verbose_name: _StrOrPromise,
         is_stacked: bool,
         attrs: _OptAttrs | None = ...,
         choices: _Choices = ...,
     ) -> None: ...
 
-class AdminDateWidget(forms.DateInput):
+class BaseAdminDateWidget(forms.DateInput):
     def __init__(self, attrs: _OptAttrs | None = ..., format: str | None = ...) -> None: ...
 
-class AdminTimeWidget(forms.TimeInput):
+class AdminDateWidget(BaseAdminDateWidget):
+    template_name: str
+
+class BaseAdminTimeWidget(forms.TimeInput):
     def __init__(self, attrs: _OptAttrs | None = ..., format: str | None = ...) -> None: ...
 
+class AdminTimeWidget(BaseAdminTimeWidget):
+    template_name: str
+
 class AdminSplitDateTime(forms.SplitDateTimeWidget):
     template_name: str
     def __init__(self, attrs: _OptAttrs | None = ...) -> None: ...
     def get_context(self, name: str, value: Any, attrs: _OptAttrs | None) -> dict[str, Any]: ...
 
 class AdminRadioSelect(forms.RadioSelect): ...
 class AdminFileWidget(forms.ClearableFileInput): ...
@@ -66,15 +72,14 @@
     def url_parameters(self) -> dict[str, str]: ...
     def label_and_url_for_value(self, value: Any) -> tuple[str, str]: ...
     def format_value(self, value: Any) -> str | None: ...
     def value_from_datadict(self, data: Mapping[str, Any], files: Mapping[str, Iterable[File]], name: str) -> Any: ...
 
 class RelatedFieldWidgetWrapper(forms.Widget):
     template_name: str
-    choices: ModelChoiceIterator
     widget: forms.ChoiceWidget
     rel: ManyToOneRel
     can_add_related: bool
     can_change_related: bool
     can_delete_related: bool
     can_view_related: bool
     admin_site: AdminSite
@@ -86,14 +91,18 @@
         can_add_related: bool | None = ...,
         can_change_related: bool = ...,
         can_delete_related: bool = ...,
         can_view_related: bool = ...,
     ) -> None: ...
     @property
     def is_hidden(self) -> bool: ...
+    @property
+    def choices(self) -> ModelChoiceIterator: ...
+    @choices.setter
+    def choices(self, value: ModelChoiceIterator) -> None: ...
     def get_related_url(self, info: tuple[str, str], action: str, *args: Any) -> str: ...
     def get_context(self, name: str, value: Any, attrs: _OptAttrs | None) -> dict[str, Any]: ...
     def value_from_datadict(self, data: Mapping[str, Any], files: Mapping[str, Iterable[File]], name: str) -> Any: ...
     def value_omitted_from_data(
         self, data: Mapping[str, Any], files: Mapping[str, Iterable[File]], name: str
     ) -> bool: ...
     def id_for_label(self, id_: str) -> str: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admindocs/utils.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admindocs/utils.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/admindocs/views.pyi` & `django_stubs-5.0.1/django-stubs/contrib/admindocs/views.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/auth/__init__.pyi` & `django_stubs-5.0.1/django-stubs/contrib/auth/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-from django.contrib.auth.backends import ModelBackend
+from django.contrib.auth.backends import BaseBackend
 from django.contrib.auth.base_user import AbstractBaseUser
 from django.contrib.auth.models import AnonymousUser
 from django.db.models.options import Options
 from django.http.request import HttpRequest
 from django.test.client import Client
 
 from .signals import user_logged_in as user_logged_in
@@ -12,23 +12,23 @@
 from .signals import user_login_failed as user_login_failed
 
 SESSION_KEY: str
 BACKEND_SESSION_KEY: str
 HASH_SESSION_KEY: str
 REDIRECT_FIELD_NAME: str
 
-def load_backend(path: str) -> ModelBackend: ...
-def get_backends() -> list[ModelBackend]: ...
+def load_backend(path: str) -> BaseBackend: ...
+def get_backends() -> list[BaseBackend]: ...
 def authenticate(request: HttpRequest | None = ..., **credentials: Any) -> AbstractBaseUser | None: ...
 async def aauthenticate(request: HttpRequest | None = ..., **credentials: Any) -> AbstractBaseUser | None: ...
 def login(
-    request: HttpRequest, user: AbstractBaseUser | None, backend: type[ModelBackend] | str | None = ...
+    request: HttpRequest, user: AbstractBaseUser | None, backend: type[BaseBackend] | str | None = ...
 ) -> None: ...
 async def alogin(
-    request: HttpRequest, user: AbstractBaseUser | None, backend: type[ModelBackend] | str | None = ...
+    request: HttpRequest, user: AbstractBaseUser | None, backend: type[BaseBackend] | str | None = ...
 ) -> None: ...
 def logout(request: HttpRequest) -> None: ...
 async def alogout(request: HttpRequest) -> None: ...
 def get_user_model() -> type[AbstractBaseUser]: ...
 def get_user(request: HttpRequest | Client) -> AbstractBaseUser | AnonymousUser: ...
 async def aget_user(request: HttpRequest | Client) -> AbstractBaseUser | AnonymousUser: ...
 def get_permission_codename(action: str, opts: Options) -> str: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/contrib/auth/admin.pyi` & `django_stubs-5.0.1/django-stubs/contrib/auth/admin.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import Any
+from typing import Any, TypeVar
 
 from django.contrib import admin
-from django.contrib.auth.models import Group, User
+from django.contrib.auth.models import AbstractUser, Group
 from django.http.request import HttpRequest
 from django.http.response import HttpResponse
 
+_AbstractUserT = TypeVar("_AbstractUserT", bound=AbstractUser)
+
 csrf_protect_m: Any
 sensitive_post_parameters_m: Any
 
 class GroupAdmin(admin.ModelAdmin[Group]): ...
 
-class UserAdmin(admin.ModelAdmin[User]):
+class UserAdmin(admin.ModelAdmin[_AbstractUserT]):
     change_user_password_template: Any
     add_fieldsets: Any
     add_form: Any
     change_password_form: Any
     def user_change_password(self, request: HttpRequest, id: str, form_url: str = ...) -> HttpResponse: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/contrib/auth/backends.pyi` & `django_stubs-5.0.1/django-stubs/contrib/auth/backends.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 _AnyUser: TypeAlias = AbstractBaseUser | AnonymousUser
 
 UserModel: Any
 
 class BaseBackend:
     def authenticate(self, request: HttpRequest | None, **kwargs: Any) -> AbstractBaseUser | None: ...
-    def get_user(self, user_id: int) -> AbstractBaseUser | None: ...
+    def get_user(self, user_id: Any) -> AbstractBaseUser | None: ...
     def get_user_permissions(self, user_obj: _AnyUser, obj: Model | None = ...) -> set[str]: ...
     def get_group_permissions(self, user_obj: _AnyUser, obj: Model | None = ...) -> set[str]: ...
     def get_all_permissions(self, user_obj: _AnyUser, obj: Model | None = ...) -> set[str]: ...
     def has_perm(self, user_obj: _AnyUser, perm: str, obj: Model | None = ...) -> bool: ...
 
 class ModelBackend(BaseBackend):
     def authenticate(
@@ -36,10 +36,10 @@
 class AllowAllUsersModelBackend(ModelBackend): ...
 
 _U = TypeVar("_U", bound=AbstractBaseUser)
 
 class RemoteUserBackend(ModelBackend):
     create_unknown_user: bool
     def clean_username(self, username: str) -> str: ...
-    def configure_user(self, request: HttpRequest, user: _U) -> _U: ...
+    def configure_user(self, request: HttpRequest, user: _U, created: bool = ...) -> _U: ...
 
 class AllowAllUsersRemoteUserBackend(RemoteUserBackend): ...
```

### Comparing `django_stubs-5.0.0/django-stubs/contrib/auth/base_user.pyi` & `django_stubs-5.0.1/django-stubs/contrib/auth/base_user.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     def is_authenticated(self) -> Literal[True]: ...
     def set_password(self, raw_password: str | None) -> None: ...
     def check_password(self, raw_password: str) -> bool: ...
     async def acheck_password(self, raw_password: str) -> bool: ...
     def set_unusable_password(self) -> None: ...
     def has_usable_password(self) -> bool: ...
     def get_session_auth_hash(self) -> str: ...
+    def get_session_auth_fallback_hash(self) -> str: ...
     @classmethod
     def get_email_field_name(cls) -> str: ...
     @classmethod
     @overload
     def normalize_username(cls, username: str) -> str: ...
     @classmethod
     @overload
```

### Comparing `django_stubs-5.0.0/django-stubs/contrib/auth/context_processors.pyi` & `django_stubs-5.0.1/django-stubs/contrib/auth/context_processors.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/auth/decorators.pyi` & `django_stubs-5.0.1/django-stubs/contrib/auth/decorators.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/auth/forms.pyi` & `django_stubs-5.0.1/django-stubs/contrib/auth/forms.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/auth/hashers.pyi` & `django_stubs-5.0.1/django-stubs/contrib/auth/hashers.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/auth/middleware.pyi` & `django_stubs-5.0.1/django-stubs/contrib/auth/middleware.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/auth/mixins.pyi` & `django_stubs-5.0.1/django-stubs/contrib/auth/mixins.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/auth/models.pyi` & `django_stubs-5.0.1/django-stubs/contrib/auth/models.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/auth/password_validation.pyi` & `django_stubs-5.0.1/django-stubs/contrib/auth/password_validation.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/auth/tokens.pyi` & `django_stubs-5.0.1/django-stubs/contrib/auth/tokens.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/auth/views.pyi` & `django_stubs-5.0.1/django-stubs/contrib/auth/views.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/contenttypes/admin.pyi` & `django_stubs-5.0.1/django-stubs/contrib/contenttypes/admin.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/contenttypes/fields.pyi` & `django_stubs-5.0.1/django-stubs/contrib/contenttypes/fields.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -40,19 +40,22 @@
     model: Any
     def contribute_to_class(self, cls: type[Model], name: str, **kwargs: Any) -> None: ...
     def get_filter_kwargs_for_object(self, obj: Model) -> dict[str, ContentType | None]: ...
     def get_forward_related_filter(self, obj: Model) -> dict[str, int]: ...
     def check(self, **kwargs: Any) -> list[CheckMessage]: ...
     def get_cache_name(self) -> str: ...
     def get_content_type(
-        self, obj: Model | None = ..., id: int | None = ..., using: str | None = ...
+        self, obj: Model | None = ..., id: int | None = ..., using: str | None = ..., model: type[Model] | None = ...
     ) -> ContentType: ...
     def get_prefetch_queryset(
         self, instances: list[Model] | QuerySet, queryset: QuerySet | None = ...
     ) -> tuple[list[Model], Callable, Callable, bool, str, bool]: ...
+    def get_prefetch_querysets(
+        self, instances: list[Model] | QuerySet, querysets: list[QuerySet] | None = ...
+    ) -> tuple[list[Model], Callable, Callable, bool, str, bool]: ...
     def __get__(self, instance: Model | None, cls: type[Model] | None = ...) -> Any | None: ...
     def __set__(self, instance: Model, value: Any | None) -> None: ...
 
 class GenericRel(ForeignObjectRel):
     field: GenericRelation
     def __init__(
         self,
```

### Comparing `django_stubs-5.0.0/django-stubs/contrib/contenttypes/forms.pyi` & `django_stubs-5.0.1/django-stubs/contrib/contenttypes/forms.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/contenttypes/management/__init__.pyi` & `django_stubs-5.0.1/django-stubs/contrib/contenttypes/management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/contenttypes/models.pyi` & `django_stubs-5.0.1/django-stubs/contrib/contenttypes/models.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/features.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/base/features.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/models.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/base/models.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/base/operations.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/base/operations.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/features.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/mysql/features.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/mysql/operations.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/mysql/operations.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/models.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/oracle/models.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/operations.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/oracle/operations.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/oracle/schema.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/mysql/schema.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+from logging import Logger
 from typing import Any
 
-from django.db.backends.oracle.schema import DatabaseSchemaEditor
+from django.db.backends.mysql.schema import DatabaseSchemaEditor
+from django.db.models.base import Model
+from django.db.models.fields import Field
 
-class OracleGISSchemaEditor(DatabaseSchemaEditor):
-    sql_add_geometry_metadata: str
+logger: Logger
+
+class MySQLGISSchemaEditor(DatabaseSchemaEditor):
     sql_add_spatial_index: str
     sql_drop_spatial_index: str
-    sql_clear_geometry_table_metadata: str
-    sql_clear_geometry_field_metadata: str
     geometry_sql: Any
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
-    def geo_quote_name(self, name: Any) -> Any: ...
-    def column_sql(self, model: Any, field: Any, include_default: bool = ...) -> Any: ...
-    def create_model(self, model: Any) -> None: ...
-    def delete_model(self, model: Any) -> None: ...
-    def add_field(self, model: Any, field: Any) -> None: ...
-    def remove_field(self, model: Any, field: Any) -> None: ...
-    def run_geometry_sql(self) -> None: ...
+    def skip_default(self, field: Field) -> bool: ...
+    def column_sql(
+        self, model: type[Model], field: Field, include_default: bool = ...
+    ) -> tuple[None, None] | tuple[str, list[Any]]: ...
+    def create_model(self, model: type[Model]) -> None: ...
+    def add_field(self, model: type[Model], field: Field) -> None: ...
+    def remove_field(self, model: type[Model], field: Field) -> None: ...
+    def create_spatial_indexes(self) -> None: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/models.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/postgis/models.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/postgis/operations.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/postgis/operations.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-from typing import Any, Literal
+from typing import Any, Literal, MutableMapping
 
 from django.contrib.gis.db.backends.base.operations import BaseSpatialOperations
 from django.contrib.gis.db.backends.utils import SpatialOperator
 from django.contrib.gis.db.models.fields import GeometryField
+from django.contrib.gis.db.models.lookups import GISLookup
 from django.db.backends.postgresql.operations import DatabaseOperations
 from django.db.models import Func
 from django.utils.functional import cached_property
 
 BILATERAL: Literal["bilateral"]
 
 class PostGISOperator(SpatialOperator):
     geography: Any
     raster: bool | Literal["bilateral"]
     def __init__(self, geography: bool = ..., raster: bool | Literal["bilateral"] = ..., **kwargs: Any) -> None: ...
     def check_raster(self, lookup: Any, template_params: Any) -> Any: ...
+    def check_geography(
+        self,
+        lookup: GISLookup,
+        template_params: MutableMapping[str, Any],
+    ) -> MutableMapping[str, Any]: ...
 
 class ST_Polygon(Func):
     function: str
     def __init__(self, expr: Any) -> None: ...
     @cached_property
     def output_field(self) -> GeometryField: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/base.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/spatialite/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/models.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/spatialite/models.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/spatialite/operations.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/spatialite/schema.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/postgresql/schema.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from typing import Any
 
-from django.db.backends.sqlite3.schema import DatabaseSchemaEditor
+from django.db.backends.base.schema import BaseDatabaseSchemaEditor
+from django.db.backends.postgresql.base import DatabaseWrapper
+from django.db.models.base import Model
+from django.db.models.indexes import Index
 
-class SpatialiteSchemaEditor(DatabaseSchemaEditor):
-    sql_add_geometry_column: str
-    sql_add_spatial_index: str
-    sql_drop_spatial_index: str
-    sql_recover_geometry_metadata: str
-    sql_remove_geometry_metadata: str
-    sql_discard_geometry_columns: str
-    sql_update_geometry_columns: str
-    geometry_tables: Any
-    geometry_sql: Any
-    def __init__(self, *args: Any, **kwargs: Any) -> None: ...
-    def geo_quote_name(self, name: Any) -> Any: ...
-    def column_sql(self, model: Any, field: Any, include_default: bool = ...) -> Any: ...
-    def remove_geometry_metadata(self, model: Any, field: Any) -> None: ...
-    def create_model(self, model: Any) -> None: ...
-    def delete_model(self, model: Any, **kwargs: Any) -> None: ...
-    def add_field(self, model: Any, field: Any) -> None: ...
-    def remove_field(self, model: Any, field: Any) -> None: ...
-    def alter_db_table(
-        self, model: Any, old_db_table: Any, new_db_table: Any, disable_constraints: bool = ...
-    ) -> None: ...
+class DatabaseSchemaEditor(BaseDatabaseSchemaEditor):
+    connection: DatabaseWrapper
+    sql_create_sequence: str
+    sql_delete_sequence: str
+    sql_set_sequence_max: str
+    sql_set_sequence_owner: str
+    sql_create_index: str
+    sql_create_index_concurrently: str
+    sql_delete_index: str
+    sql_delete_index_concurrently: str
+    sql_create_column_inline_fk: str
+    sql_delete_fk: str
+    sql_delete_procedure: str
+    def quote_value(self, value: Any) -> str: ...
+    def add_index(self, model: type[Model], index: Index, concurrently: bool = ...) -> None: ...
+    def remove_index(self, model: type[Model], index: Index, concurrently: bool = ...) -> None: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/backends/utils.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/backends/utils.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from collections.abc import Mapping, Sequence
-from typing import Any
+from collections.abc import Sequence
+from typing import Any, MutableMapping
 
 from django.contrib.gis.db.models.lookups import GISLookup
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.sql.compiler import _AsSqlType
 
 class SpatialOperator:
     sql_template: Any
@@ -12,10 +12,10 @@
     def __init__(self, op: Any | None = ..., func: Any | None = ...) -> None: ...
     @property
     def default_template(self) -> Any: ...
     def as_sql(
         self,
         connection: BaseDatabaseWrapper,
         lookup: GISLookup,
-        template_params: Mapping[str, Any],
+        template_params: MutableMapping[str, Any],
         sql_params: Sequence[Any],
     ) -> _AsSqlType: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/models/__init__.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/models/aggregates.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/models/aggregates.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/models/fields.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/models/fields.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/models/functions.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/models/functions.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/models/lookups.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/models/lookups.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/db/models/sql/conversion.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/db/models/sql/conversion.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/feeds.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/feeds.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/forms/__init__.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/forms/fields.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/forms/fields.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/forms/widgets.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/forms/widgets.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/__init__.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/datasource.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/datasource.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/envelope.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/envelope.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/feature.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/feature.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/field.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/field.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/geometries.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/geometries.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/layer.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/layer.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/libgdal.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/libgdal.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/ds.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/prototypes/ds.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/prototypes/errcheck.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/generation.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/prototypes/generation.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/geom.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/prototypes/geom.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/raster.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/prototypes/raster.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/prototypes/srs.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/prototypes/srs.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/band.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/raster/band.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/raster/source.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/raster/source.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/gdal/srs.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/gdal/srs.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geoip2/base.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geoip2/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/__init__.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/collections.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/collections.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/coordseq.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/coordseq.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/geometry.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/geometry.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/libgeos.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/libgeos.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/linestring.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/linestring.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/mutable_list.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/mutable_list.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/point.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/point.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/polygon.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/polygon.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/prepared.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/prepared.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/__init__.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/coordseq.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/geom.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/geom.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/io.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/io.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/predicates.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/predicates.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/geos/prototypes/topology.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/geos/prototypes/topology.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/measure.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/measure.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/gis/utils/layermapping.pyi` & `django_stubs-5.0.1/django-stubs/contrib/gis/utils/layermapping.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/humanize/templatetags/humanize.pyi` & `django_stubs-5.0.1/django-stubs/contrib/humanize/templatetags/humanize.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/messages/__init__.pyi` & `django_stubs-5.0.1/django-stubs/contrib/messages/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/messages/api.pyi` & `django_stubs-5.0.1/django-stubs/contrib/messages/api.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/messages/storage/base.pyi` & `django_stubs-5.0.1/django-stubs/contrib/messages/storage/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/__init__.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/aggregates/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/general.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/aggregates/general.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/mixins.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/aggregates/mixins.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/aggregates/statistics.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/aggregates/statistics.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/constraints.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/constraints.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/fields/__init__.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/fields/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/fields/array.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/fields/array.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/fields/hstore.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/fields/hstore.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/fields/ranges.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/fields/ranges.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/forms/__init__.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/forms/array.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/forms/array.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/forms/ranges.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/forms/ranges.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/indexes.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/indexes.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/lookups.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/lookups.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/operations.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/operations.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/search.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/search.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/postgres/validators.pyi` & `django_stubs-5.0.1/django-stubs/contrib/postgres/validators.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/sessions/backends/base.pyi` & `django_stubs-5.0.1/django-stubs/contrib/sessions/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/sessions/backends/db.pyi` & `django_stubs-5.0.1/django-stubs/contrib/sessions/backends/db.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/sessions/base_session.pyi` & `django_stubs-5.0.1/django-stubs/contrib/sessions/base_session.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from datetime import datetime
-from typing import Any, TypeVar
+from typing import Any, ClassVar, TypeVar
 
 from django.contrib.sessions.backends.base import SessionBase
 from django.db import models
+from typing_extensions import Self
 
 _T = TypeVar("_T", bound=AbstractBaseSession)
 
 class BaseSessionManager(models.Manager[_T]):
     def encode(self, session_dict: dict[str, Any]) -> str: ...
     def save(self, session_key: str, session_dict: dict[str, Any], expire_date: datetime) -> _T: ...
 
 class AbstractBaseSession(models.Model):
-    expire_date: datetime
-    session_data: str
-    session_key: str
-    objects: Any
+    session_key = models.CharField(primary_key=True)
+    session_data = models.TextField()
+    expire_date = models.DateTimeField()
+    objects: ClassVar[BaseSessionManager[Self]]
 
     @classmethod
     def get_session_store_class(cls) -> type[SessionBase] | None: ...
     def get_decoded(self) -> dict[str, Any]: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/contrib/sitemaps/__init__.pyi` & `django_stubs-5.0.1/django-stubs/contrib/sitemaps/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/sitemaps/views.pyi` & `django_stubs-5.0.1/django-stubs/contrib/sitemaps/views.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/sites/models.pyi` & `django_stubs-5.0.1/django-stubs/contrib/sites/models.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/staticfiles/finders.pyi` & `django_stubs-5.0.1/django-stubs/contrib/staticfiles/finders.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/staticfiles/handlers.pyi` & `django_stubs-5.0.1/django-stubs/contrib/staticfiles/handlers.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi` & `django_stubs-5.0.1/django-stubs/contrib/staticfiles/management/commands/collectstatic.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/staticfiles/storage.pyi` & `django_stubs-5.0.1/django-stubs/contrib/staticfiles/storage.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/contrib/syndication/views.pyi` & `django_stubs-5.0.1/django-stubs/contrib/syndication/views.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/cache/__init__.pyi` & `django_stubs-5.0.1/django-stubs/core/cache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/cache/backends/base.pyi` & `django_stubs-5.0.1/django-stubs/core/cache/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/cache/backends/db.pyi` & `django_stubs-5.0.1/django-stubs/core/cache/backends/db.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/cache/backends/memcached.pyi` & `django_stubs-5.0.1/django-stubs/core/cache/backends/memcached.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/cache/backends/redis.pyi` & `django_stubs-5.0.1/django-stubs/core/cache/backends/redis.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/checks/__init__.pyi` & `django_stubs-5.0.1/django-stubs/core/checks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/checks/caches.pyi` & `django_stubs-5.0.1/django-stubs/core/checks/caches.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/checks/messages.pyi` & `django_stubs-5.0.1/django-stubs/core/checks/messages.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/checks/registry.pyi` & `django_stubs-5.0.1/django-stubs/core/checks/registry.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/checks/security/base.pyi` & `django_stubs-5.0.1/django-stubs/core/checks/security/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/checks/security/csrf.pyi` & `django_stubs-5.0.1/django-stubs/core/checks/security/csrf.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/checks/security/sessions.pyi` & `django_stubs-5.0.1/django-stubs/core/checks/security/sessions.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/checks/templates.pyi` & `django_stubs-5.0.1/django-stubs/core/checks/templates.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/checks/translation.pyi` & `django_stubs-5.0.1/django-stubs/core/checks/translation.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/checks/urls.pyi` & `django_stubs-5.0.1/django-stubs/core/checks/urls.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/exceptions.pyi` & `django_stubs-5.0.1/django-stubs/core/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/files/base.pyi` & `django_stubs-5.0.1/django-stubs/core/files/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/files/storage/__init__.pyi` & `django_stubs-5.0.1/django-stubs/core/files/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/files/storage/base.pyi` & `django_stubs-5.0.1/django-stubs/core/files/storage/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/files/storage/filesystem.pyi` & `django_stubs-5.0.1/django-stubs/core/files/storage/filesystem.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/files/storage/memory.pyi` & `django_stubs-5.0.1/django-stubs/core/files/storage/memory.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/files/uploadedfile.pyi` & `django_stubs-5.0.1/django-stubs/core/files/uploadedfile.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/files/uploadhandler.pyi` & `django_stubs-5.0.1/django-stubs/core/files/uploadhandler.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/files/utils.pyi` & `django_stubs-5.0.1/django-stubs/core/files/utils.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/handlers/asgi.pyi` & `django_stubs-5.0.1/django-stubs/core/handlers/asgi.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/handlers/base.pyi` & `django_stubs-5.0.1/django-stubs/core/handlers/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/handlers/exception.pyi` & `django_stubs-5.0.1/django-stubs/core/handlers/exception.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/handlers/wsgi.pyi` & `django_stubs-5.0.1/django-stubs/core/handlers/wsgi.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/mail/__init__.pyi` & `django_stubs-5.0.1/django-stubs/core/mail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/mail/backends/base.pyi` & `django_stubs-5.0.1/django-stubs/core/mail/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/mail/message.pyi` & `django_stubs-5.0.1/django-stubs/core/mail/message.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/management/__init__.pyi` & `django_stubs-5.0.1/django-stubs/core/management/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/management/base.pyi` & `django_stubs-5.0.1/django-stubs/core/management/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/management/color.pyi` & `django_stubs-5.0.1/django-stubs/core/management/color.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/management/commands/diffsettings.pyi` & `django_stubs-5.0.1/django-stubs/core/management/commands/diffsettings.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/management/commands/inspectdb.pyi` & `django_stubs-5.0.1/django-stubs/core/management/commands/inspectdb.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/management/commands/loaddata.pyi` & `django_stubs-5.0.1/django-stubs/core/management/commands/loaddata.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/management/commands/makemessages.pyi` & `django_stubs-5.0.1/django-stubs/core/management/commands/makemessages.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/management/commands/makemigrations.pyi` & `django_stubs-5.0.1/django-stubs/core/management/commands/makemigrations.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/management/commands/migrate.pyi` & `django_stubs-5.0.1/django-stubs/core/management/commands/migrate.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/management/commands/runserver.pyi` & `django_stubs-5.0.1/django-stubs/core/management/commands/runserver.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/management/templates.pyi` & `django_stubs-5.0.1/django-stubs/core/management/templates.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/management/utils.pyi` & `django_stubs-5.0.1/django-stubs/core/management/utils.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/paginator.pyi` & `django_stubs-5.0.1/django-stubs/core/paginator.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/serializers/__init__.pyi` & `django_stubs-5.0.1/django-stubs/core/serializers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/serializers/base.pyi` & `django_stubs-5.0.1/django-stubs/core/serializers/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/serializers/json.pyi` & `django_stubs-5.0.1/django-stubs/core/serializers/json.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/serializers/pyyaml.pyi` & `django_stubs-5.0.1/django-stubs/core/serializers/pyyaml.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/serializers/xml_serializer.pyi` & `django_stubs-5.0.1/django-stubs/core/serializers/xml_serializer.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/servers/basehttp.pyi` & `django_stubs-5.0.1/django-stubs/core/servers/basehttp.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/signing.pyi` & `django_stubs-5.0.1/django-stubs/core/signing.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/core/validators.pyi` & `django_stubs-5.0.1/django-stubs/core/validators.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/__init__.pyi` & `django_stubs-5.0.1/django-stubs/db/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/base/base.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/base/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/base/client.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/base/client.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/base/creation.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/base/creation.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/base/features.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/base/features.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     minimum_database_version: tuple[int, ...] | None
     gis_enabled: bool
     allows_group_by_lob: bool
     allows_group_by_selected_pks: bool
     allows_group_by_select_index: bool
     empty_fetchmany_value: Sequence[Any]
     update_can_self_select: bool
+    delete_can_self_reference_subquery: bool
     interprets_empty_strings_as_nulls: bool
     supports_nullable_unique_constraints: bool
     supports_partially_nullable_unique_constraints: bool
     supports_deferrable_unique_constraints: bool
     can_use_chunked_reads: bool
     can_return_columns_from_insert: bool
     can_return_rows_from_bulk_insert: bool
@@ -60,25 +61,27 @@
     introspected_field_types: dict[str, str]
     supports_index_column_ordering: bool
     can_introspect_materialized_views: bool
     can_distinct_on_fields: bool
     atomic_transactions: bool
     can_rollback_ddl: bool
     schema_editor_uses_clientside_param_binding: bool
-    supports_atomic_references_rename: bool
     supports_combined_alters: bool
     supports_foreign_keys: bool
     can_create_inline_fk: bool
     can_rename_index: bool
     indexes_foreign_keys: bool
     supports_column_check_constraints: bool
     supports_table_check_constraints: bool
     can_introspect_check_constraints: bool
     supports_paramstyle_pyformat: bool
     requires_literal_defaults: bool
+    supports_expression_defaults: bool
+    supports_default_keyword_in_insert: bool
+    supports_default_keyword_in_bulk_insert: bool
     connection_persists_old_columns: bool
     closed_cursor_error_class: type[DatabaseError]
     has_case_insensitive_like: bool
     bare_select_suffix: str
     implied_column_null: bool
     supports_select_for_update_with_limit: bool
     greatest_least_ignores_nulls: bool
@@ -86,14 +89,15 @@
     ignores_table_name_case: bool
     for_update_after_from: bool
     supports_select_union: bool
     supports_select_intersection: bool
     supports_select_difference: bool
     supports_slicing_ordering_in_compound: bool
     supports_parentheses_in_compound: bool
+    supports_nulls_distinct_unique_constraints: bool
     requires_compound_order_by_subquery: bool
     supports_aggregate_filter_clause: bool
     supports_index_on_text_field: bool
     supports_over_clause: bool
     supports_frame_range_fixed_distance: bool
     only_supports_unbounded_with_preceding_and_following: bool
     supports_cast_with_precision: bool
@@ -124,19 +128,22 @@
     json_key_contains_list_matching_requires_list: bool
     has_json_object_function: bool
     supports_collation_on_charfield: bool
     supports_collation_on_textfield: bool
     supports_non_deterministic_collations: bool
     supports_comments: bool
     supports_comments_inline: bool
+    supports_stored_generated_columns: bool
+    supports_virtual_generated_columns: bool
     supports_logical_xor: bool
     prohibits_null_characters_in_text_exception: tuple[ValueError | DataError] | None
     supports_unlimited_charfield: bool
     test_collations: dict[str, str | None]
     test_now_utc_template: str | None
+    insert_test_table_with_defaults: str | None
     django_test_expected_failures: set[str]
     django_test_skips: dict[str, set[str]]
     connection: BaseDatabaseWrapper
     def __init__(self, connection: BaseDatabaseWrapper) -> None: ...
     @cached_property
     def supports_explaining_query_execution(self) -> bool: ...
     @cached_property
```

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/base/introspection.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/base/introspection.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/base/operations.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/base/operations.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any
 
 from django.core.management.color import Style
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.backends.utils import CursorWrapper
 from django.db.models.base import Model
 from django.db.models.constants import OnConflict
-from django.db.models.expressions import Case, Expression
+from django.db.models.expressions import Case, Col, Expression
 from django.db.models.fields import Field
 from django.db.models.sql.compiler import SQLCompiler
 
 class BaseDatabaseOperations:
     compiler_module: str
     integer_field_ranges: dict[str, tuple[int, int]]
     set_operators: dict[str, str]
@@ -107,7 +107,10 @@
     def window_frame_range_start_end(self, start: int | None = ..., end: int | None = ...) -> tuple[str, str]: ...
     def explain_query_prefix(self, format: str | None = ..., **options: Any) -> str: ...
     def insert_statement(self, on_conflict: OnConflict | None = ...) -> str: ...
     def on_conflict_suffix_sql(
         self, fields: Any, on_conflict: Any, update_fields: Any, unique_fields: Any
     ) -> str | Any: ...
     def format_for_duration_arithmetic(self, sql: str) -> str: ...
+    def prepare_join_on_clause(
+        self, lhs_table: str, lhs_field: Field, rhs_table: str, rhs_field: Field
+    ) -> tuple[Col, Col]: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/base/schema.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/base/schema.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -70,16 +70,16 @@
     ) -> None: ...
     def execute(self, sql: Statement | str, params: Sequence[Any] | None = ...) -> None: ...
     def quote_name(self, name: str) -> str: ...
     def table_sql(self, model: type[Model]) -> tuple[str, list[Any]]: ...
     def column_sql(
         self, model: type[Model], field: Field, include_default: bool = ...
     ) -> tuple[None, None] | tuple[str, list[Any]]: ...
-    def skip_default(self, field: Any) -> bool: ...
-    def skip_default_on_alter(self, field: Any) -> bool: ...
+    def skip_default(self, field: Field) -> bool: ...
+    def skip_default_on_alter(self, field: Field) -> bool: ...
     def prepare_default(self, value: Any) -> Any: ...
     def db_default_sql(self, field: Field) -> _AsSqlType: ...
     def effective_default(self, field: Field) -> int | str: ...
     def quote_value(self, value: Any) -> str: ...
     def create_model(self, model: type[Model]) -> None: ...
     def delete_model(self, model: type[Model]) -> None: ...
     def add_index(self, model: type[Model], index: Index) -> None: ...
@@ -97,14 +97,14 @@
         self,
         model: type[Model],
         old_index_together: Sequence[Sequence[str]],
         new_index_together: Sequence[Sequence[str]],
     ) -> None: ...
     def alter_db_table(self, model: type[Model], old_db_table: str, new_db_table: str) -> None: ...
     def alter_db_table_comment(
-        self, model: type[Model], old_db_table_comment: str | None, new_db_table_comment: str
+        self, model: type[Model], old_db_table_comment: str, new_db_table_comment: str
     ) -> None: ...
-    def alter_db_tablespace(self, model: Any, old_db_tablespace: Any, new_db_tablespace: Any) -> None: ...
-    def add_field(self, model: Any, field: Any) -> None: ...
-    def remove_field(self, model: Any, field: Any) -> None: ...
+    def alter_db_tablespace(self, model: type[Model], old_db_tablespace: str, new_db_tablespace: str) -> None: ...
+    def add_field(self, model: type[Model], field: Field) -> None: ...
+    def remove_field(self, model: type[Model], field: Field) -> None: ...
     def alter_field(self, model: type[Model], old_field: Field, new_field: Field, strict: bool = ...) -> None: ...
     def remove_procedure(self, procedure_name: Any, param_types: Any = ...) -> None: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/ddl_references.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/ddl_references.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/dummy/base.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/dummy/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/mysql/base.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/mysql/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/mysql/compiler.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/mysql/compiler.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/mysql/features.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/mysql/features.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/mysql/introspection.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/mysql/introspection.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/mysql/operations.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/mysql/operations.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/mysql/schema.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/mysql/schema.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Any
 
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django.db.backends.mysql.base import DatabaseWrapper
+from django.db.models.base import Model
+from django.db.models.fields import Field
 
 class DatabaseSchemaEditor(BaseDatabaseSchemaEditor):
     connection: DatabaseWrapper
     sql_rename_table: str
     sql_alter_column_null: str
     sql_alter_column_not_null: str
     sql_alter_column_type: str
@@ -18,9 +20,9 @@
     sql_delete_pk: str
     sql_create_index: str
     @property
     def sql_delete_check(self) -> str: ...  # type: ignore[override]
     @property
     def sql_rename_column(self) -> str: ...  # type: ignore[override]
     def quote_value(self, value: Any) -> str: ...
-    def skip_default(self, field: Any) -> bool: ...
-    def add_field(self, model: Any, field: Any) -> None: ...
+    def skip_default(self, field: Field) -> bool: ...
+    def add_field(self, model: type[Model], field: Field) -> None: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/oracle/base.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/oracle/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/oracle/client.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/oracle/client.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/oracle/features.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/oracle/features.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/oracle/operations.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/oracle/operations.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/oracle/schema.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/oracle/schema.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from typing import Any
 
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django.db.backends.oracle.base import DatabaseWrapper
+from django.db.models.base import Model
+from django.db.models.fields import Field
 
 class DatabaseSchemaEditor(BaseDatabaseSchemaEditor):
     connection: DatabaseWrapper
     sql_create_column: str
     sql_alter_column_type: str
     sql_alter_column_null: str
     sql_alter_column_not_null: str
     sql_alter_column_default: str
     sql_alter_column_no_default: str
     sql_delete_column: str
     sql_create_column_inline_fk: str
     sql_delete_table: str
     sql_create_index: str
     def quote_value(self, value: Any) -> str: ...
-    def remove_field(self, model: Any, field: Any) -> None: ...
-    def delete_model(self, model: Any) -> None: ...
-    def alter_field(self, model: Any, old_field: Any, new_field: Any, strict: bool = ...) -> None: ...
+    def remove_field(self, model: type[Model], field: Field) -> None: ...
+    def delete_model(self, model: type[Model]) -> None: ...
+    def alter_field(self, model: type[Model], old_field: Field, new_field: Field, strict: bool = ...) -> None: ...
     def normalize_name(self, name: Any) -> str: ...
     def prepare_default(self, value: Any) -> Any: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/postgresql/base.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/postgresql/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/postgresql/client.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/postgresql/client.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/postgresql/features.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/postgresql/features.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/postgresql/operations.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/postgresql/operations.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/sqlite3/base.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/sqlite3/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/sqlite3/operations.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/sqlite3/operations.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/backends/utils.pyi` & `django_stubs-5.0.1/django-stubs/db/backends/utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 _ExecuteParameters: TypeAlias = Sequence[_SQLType] | Mapping[str, _SQLType] | None
 
 class CursorWrapper:
     cursor: Any
     db: Any
     def __init__(self, cursor: Any, db: Any) -> None: ...
     WRAP_ERROR_ATTRS: Any
+    APPS_NOT_READY_WARNING_MSG: str
+
     def __getattr__(self, attr: str) -> Any: ...
     def __iter__(self) -> Iterator[tuple[Any, ...]]: ...
     def __enter__(self) -> Self: ...
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
```

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/autodetector.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/autodetector.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -39,25 +39,32 @@
     renamed_models: Any
     renamed_models_rel: Any
     def generate_renamed_models(self) -> None: ...
     def generate_created_models(self) -> None: ...
     def generate_created_proxies(self) -> None: ...
     def generate_deleted_models(self) -> None: ...
     def generate_deleted_proxies(self) -> None: ...
+    def create_renamed_fields(self) -> None: ...
     renamed_fields: Any
     def generate_renamed_fields(self) -> None: ...
     def generate_added_fields(self) -> None: ...
     def generate_removed_fields(self) -> None: ...
     def generate_altered_fields(self) -> None: ...
     def create_altered_indexes(self) -> None: ...
+    def generate_renamed_indexes(self) -> None: ...
+    def create_altered_constraints(self) -> None: ...
+    def generate_added_constraints(self) -> None: ...
+    def generate_removed_constraints(self) -> None: ...
     def generate_added_indexes(self) -> None: ...
     def generate_removed_indexes(self) -> None: ...
+    def generate_removed_altered_unique_together(self) -> None: ...
     def generate_altered_unique_together(self) -> None: ...
     def generate_altered_index_together(self) -> None: ...
     def generate_altered_db_table(self) -> None: ...
+    def generate_altered_db_table_comment(self) -> None: ...
     def generate_altered_options(self) -> None: ...
     def generate_altered_order_with_respect_to(self) -> None: ...
     def generate_altered_managers(self) -> None: ...
     def arrange_for_graph(
         self, changes: dict[str, list[Migration]], graph: MigrationGraph, migration_name: str | None = ...
     ) -> dict[str, list[Migration]]: ...
     @classmethod
```

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/exceptions.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/executor.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/executor.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/graph.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/graph.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/loader.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/loader.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/migration.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/migration.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/operations/__init__.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/operations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/operations/base.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/operations/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/operations/fields.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/operations/fields.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/operations/models.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/operations/models.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/operations/special.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/operations/special.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/operations/utils.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/operations/utils.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/questioner.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/questioner.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/recorder.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/recorder.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/serializer.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/serializer.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,40 +3,41 @@
 
 class BaseSerializer:
     value: Any
     def __init__(self, value: Any) -> None: ...
     def serialize(self) -> tuple[str, set[str]]: ...
 
 class BaseSequenceSerializer(BaseSerializer): ...
+class BaseUnorderedSequenceSerializer(BaseSequenceSerializer): ...
 class BaseSimpleSerializer(BaseSerializer): ...
 class DateTimeSerializer(BaseSerializer): ...
 class DatetimeDatetimeSerializer(BaseSerializer): ...
 class DecimalSerializer(BaseSerializer): ...
 
 class DeconstructableSerializer(BaseSerializer):
     @staticmethod
     def serialize_deconstructed(
         path: str, args: list[Any], kwargs: dict[str, Callable | int | str]
     ) -> tuple[str, set[str]]: ...
 
 class DictionarySerializer(BaseSerializer): ...
 class EnumSerializer(BaseSerializer): ...
 class FloatSerializer(BaseSimpleSerializer): ...
-class FrozensetSerializer(BaseSequenceSerializer): ...
+class FrozensetSerializer(BaseUnorderedSequenceSerializer): ...
 class FunctionTypeSerializer(BaseSerializer): ...
 class FunctoolsPartialSerializer(BaseSerializer): ...
 class IterableSerializer(BaseSerializer): ...
 class ModelFieldSerializer(DeconstructableSerializer): ...
 class ModelManagerSerializer(DeconstructableSerializer): ...
 class OperationSerializer(BaseSerializer): ...
 class PathLikeSerializer(BaseSerializer): ...
 class PathSerializer(BaseSerializer): ...
 class RegexSerializer(BaseSerializer): ...
 class SequenceSerializer(BaseSequenceSerializer): ...
-class SetSerializer(BaseSequenceSerializer): ...
+class SetSerializer(BaseUnorderedSequenceSerializer): ...
 class SettingsReferenceSerializer(BaseSerializer): ...
 class TupleSerializer(BaseSequenceSerializer): ...
 class TypeSerializer(BaseSerializer): ...
 class UUIDSerializer(BaseSerializer): ...
 
 def serializer_factory(value: Any) -> BaseSerializer: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/state.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/state.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/migrations/writer.pyi` & `django_stubs-5.0.1/django-stubs/db/migrations/writer.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/__init__.pyi` & `django_stubs-5.0.1/django-stubs/db/models/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -87,10 +87,11 @@
 from .fields.related import OneToOneRel as OneToOneRel
 from .indexes import Index as Index
 from .lookups import Lookup as Lookup
 from .lookups import Transform as Transform
 from .manager import Manager as Manager
 from .query import Prefetch as Prefetch
 from .query import QuerySet as QuerySet
+from .query import aprefetch_related_objects as aprefetch_related_objects
 from .query import prefetch_related_objects as prefetch_related_objects
 from .query_utils import FilteredRelation as FilteredRelation
 from .query_utils import Q as Q
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/aggregates.pyi` & `django_stubs-5.0.1/django-stubs/db/models/aggregates.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/base.pyi` & `django_stubs-5.0.1/django-stubs/db/models/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/constraints.pyi` & `django_stubs-5.0.1/django-stubs/db/models/constraints.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         name: str | None = ...,
         violation_error_code: str | None = ...,
         violation_error_message: _StrOrPromise | None = ...,
     ) -> None: ...
     def constraint_sql(self, model: type[Model] | None, schema_editor: BaseDatabaseSchemaEditor | None) -> str: ...
     def create_sql(self, model: type[Model] | None, schema_editor: BaseDatabaseSchemaEditor | None) -> str: ...
     def remove_sql(self, model: type[Model] | None, schema_editor: BaseDatabaseSchemaEditor | None) -> str: ...
+    def get_violation_error_message(self) -> str: ...
     def deconstruct(self) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
     def clone(self) -> Self: ...
 
 class CheckConstraint(BaseConstraint):
     check: Q | BaseExpression
     def __init__(
         self,
@@ -49,25 +50,27 @@
     ) -> None: ...
 
 class UniqueConstraint(BaseConstraint):
     expressions: Sequence[BaseExpression | Combinable]
     fields: Sequence[str]
     condition: Q | None
     deferrable: Deferrable | None
+    nulls_distinct: bool | None
 
     @overload
     def __init__(
         self,
         *expressions: str | BaseExpression | Combinable,
         fields: None = ...,
         name: str | None = ...,
         condition: Q | None = ...,
         deferrable: Deferrable | None = ...,
         include: Sequence[str] | None = ...,
         opclasses: Sequence[Any] = ...,
+        nulls_distinct: bool | None = ...,
         violation_error_code: str | None = ...,
         violation_error_message: _StrOrPromise | None = ...,
     ) -> None: ...
     @overload
     def __init__(
         self,
         *,
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/deletion.pyi` & `django_stubs-5.0.1/django-stubs/db/models/deletion.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/enums.pyi` & `django_stubs-5.0.1/django-stubs/db/models/enums.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 import enum
 import sys
-from typing import Any, TypeVar, type_check_only
+from typing import Any, TypeVar, overload, type_check_only
 
-from typing_extensions import Self, TypeAlias
+from _typeshed import ConvertibleToInt
+from django.utils.functional import _StrOrPromise
+from typing_extensions import TypeAlias
 
 _Self = TypeVar("_Self")
 
 if sys.version_info >= (3, 11):
     _enum_property = enum.property
+    EnumType = enum.EnumType
+    IntEnum = enum.IntEnum
+    StrEnum = enum.StrEnum
 else:
     _enum_property = property
+    EnumType = enum.EnumMeta
 
-class ChoicesMeta(enum.EnumMeta):
+    class ReprEnum(enum.Enum): ...
+    class IntEnum(int, ReprEnum): ...
+    class StrEnum(str, ReprEnum): ...
+
+class ChoicesMeta(EnumType):
     # There's a contradiction between mypy and PYI019 regarding metaclasses. Where mypy
     # disallows 'typing_extensions.Self' on metaclasses, while PYI019 try to enforce
     # 'typing_extensions.Self' for '__new__' methods.. We've chosen to ignore the
     # linter and trust mypy.
     def __new__(
         metacls: type[_Self], classname: str, bases: tuple[type, ...], classdict: enum._EnumDict, **kwds: Any
     ) -> _Self: ...  # noqa: PYI019
@@ -27,40 +37,49 @@
     @property
     def labels(self) -> list[str]: ...
     @property
     def values(self) -> list[Any]: ...
 
 ChoicesType: TypeAlias = ChoicesMeta
 
-class Choices(enum.Enum, metaclass=ChoicesMeta):
+class Choices(enum.Enum, metaclass=ChoicesType):
     @property
     def label(self) -> str: ...
     @_enum_property
     def value(self) -> Any: ...
     @property
     def do_not_call_in_templates(self) -> bool: ...
 
 # fake, to keep simulate class properties
 @type_check_only
-class _IntegerChoicesMeta(ChoicesMeta):
+class _IntegerChoicesMeta(ChoicesType):
     @property
     def choices(self) -> list[tuple[int, str]]: ...
     @property
     def values(self) -> list[int]: ...
 
-class IntegerChoices(int, Choices, metaclass=_IntegerChoicesMeta):
-    def __new__(cls, value: int) -> Self: ...
+# In reality, the `__init__` overloads provided below should also support
+# all the arguments of `int.__new__`/`str.__new__` (e.g. `base`, `encoding`).
+# They are omitted on purpose to avoid having convoluted stubs for these enums:
+class IntegerChoices(Choices, IntEnum, metaclass=_IntegerChoicesMeta):
+    @overload
+    def __init__(self, x: ConvertibleToInt) -> None: ...
+    @overload
+    def __init__(self, x: ConvertibleToInt, label: _StrOrPromise) -> None: ...
     @_enum_property
     def value(self) -> int: ...
 
 # fake, to keep simulate class properties
 @type_check_only
-class _TextChoicesMeta(ChoicesMeta):
+class _TextChoicesMeta(ChoicesType):
     @property
     def choices(self) -> list[tuple[str, str]]: ...
     @property
     def values(self) -> list[str]: ...
 
-class TextChoices(str, Choices, metaclass=_TextChoicesMeta):
-    def __new__(cls, value: str) -> Self: ...
+class TextChoices(Choices, StrEnum, metaclass=_TextChoicesMeta):
+    @overload
+    def __init__(self, object: str) -> None: ...
+    @overload
+    def __init__(self, object: str, label: _StrOrPromise) -> None: ...
     @_enum_property
     def value(self) -> str: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/expressions.pyi` & `django_stubs-5.0.1/django-stubs/db/models/expressions.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     def __rxor__(self, other: Any) -> Combinable: ...
     def __invert__(self) -> NegatedExpression[Combinable]: ...
 
 class BaseExpression:
     is_summary: bool
     filterable: bool
     window_compatible: bool
+    allowed_default: bool
     def __init__(self, output_field: Field | None = ...) -> None: ...
     def get_db_converters(self, connection: BaseDatabaseWrapper) -> list[Callable]: ...
     def get_source_expressions(self) -> list[Any]: ...
     def set_source_expressions(self, exprs: Sequence[Combinable]) -> None: ...
     @cached_property
     def contains_aggregate(self) -> bool: ...
     @cached_property
@@ -125,14 +126,15 @@
 
 class TemporalSubtraction(CombinedExpression):
     output_field: ClassVar[fields.DurationField]
     def __init__(self, lhs: Combinable, rhs: Combinable) -> None: ...
 
 class F(_Deconstructible, Combinable):
     name: str
+    allowed_default: ClassVar[bool]
     def __init__(self, name: str) -> None: ...
     def resolve_expression(
         self,
         query: Any = ...,
         allow_joins: bool = ...,
         reuse: set[str] | None = ...,
         summarize: bool = ...,
@@ -189,14 +191,15 @@
 
 class RawSQL(Expression):
     params: list[Any]
     sql: str
     def __init__(self, sql: str, params: Sequence[Any], output_field: Field | None = ...) -> None: ...
 
 class Star(Expression): ...
+class DatabaseDefault(Expression): ...
 
 class Col(Expression):
     target: Field
     alias: str
     contains_column_references: Literal[True]
     possibly_multivalued: Literal[False]
     def __init__(self, alias: str, target: Field, output_field: Field | None = ...) -> None: ...
@@ -233,14 +236,15 @@
     extra: Any
     def __init__(
         self, *cases: Any, default: Any | None = ..., output_field: Field | None = ..., **extra: Any
     ) -> None: ...
 
 class Subquery(BaseExpression, Combinable):
     template: str
+    subquery: bool
     query: Query
     extra: dict[Any, Any]
     def __init__(self, queryset: Query | QuerySet, output_field: Field | None = ..., **extra: Any) -> None: ...
 
 class Exists(Subquery):
     output_field: ClassVar[fields.BooleanField]
     def __init__(self, queryset: Query | QuerySet, **kwargs: Any) -> None: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/fields/__init__.pyi` & `django_stubs-5.0.1/django-stubs/db/models/fields/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     help_text: _StrOrPromise
     attname: str
     auto_created: bool
     primary_key: bool
     remote_field: ForeignObjectRel | None
     is_relation: bool
     related_model: type[Model] | Literal["self"] | None
+    generated: ClassVar[bool]
     one_to_many: bool | None
     one_to_one: bool | None
     many_to_many: bool | None
     many_to_one: bool | None
     max_length: int | None
     model: type[Model]
     name: str
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/fields/files.pyi` & `django_stubs-5.0.1/django-stubs/db/models/fields/files.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/fields/generated.pyi` & `django_stubs-5.0.1/django-stubs/db/models/fields/generated.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Any, Iterable, Literal
+from typing import Any, ClassVar, Iterable, Literal
 
 from django.core.validators import _ValidatorCallable
 from django.db import models
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.expressions import Expression
 from django.db.models.fields import _ErrorMessagesMapping
 from django.db.models.sql import Query
 from django.utils.choices import _Choices
 from django.utils.datastructures import DictWrapper
 from django.utils.functional import _StrOrPromise
 
 class GeneratedField(models.Field):
-    generated: Literal[True]
+    generated: ClassVar[Literal[True]]
     db_returning: Literal[True]
     _query: Query | None
     output_field: models.Field | None
 
     def __init__(
         self,
         *,
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/fields/json.pyi` & `django_stubs-5.0.1/django-stubs/db/models/fields/json.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/fields/mixins.pyi` & `django_stubs-5.0.1/django-stubs/db/models/fields/mixins.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/fields/related.pyi` & `django_stubs-5.0.1/django-stubs/db/models/fields/related.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -138,14 +138,16 @@
     def related_fields(self) -> list[tuple[Field, Field]]: ...
     @cached_property
     def reverse_related_fields(self) -> list[tuple[Field, Field]]: ...
     @cached_property
     def local_related_fields(self) -> tuple[Field, ...]: ...
     @cached_property
     def foreign_related_fields(self) -> tuple[Field, ...]: ...
+    def get_joining_fields(self, reverse_join: bool = False) -> tuple[tuple[Field, Field], ...]: ...
+    def get_reverse_joining_fields(self) -> tuple[tuple[Field, Field], ...]: ...
 
 class ForeignKey(ForeignObject[_ST, _GT]):
     _pyi_private_set_type: Any | Combinable
     _pyi_private_get_type: Any
 
     remote_field: ManyToOneRel
     rel_class: type[ManyToOneRel]
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/fields/related_descriptors.pyi` & `django_stubs-5.0.1/django-stubs/db/models/fields/related_descriptors.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -23,24 +23,27 @@
 
 class ForwardManyToOneDescriptor(Generic[_F]):
     field: _F
     def __init__(self, field_with_rel: _F) -> None: ...
     @cached_property
     def RelatedObjectDoesNotExist(self) -> type[ObjectDoesNotExist]: ...
     def is_cached(self, instance: Model) -> bool: ...
-    def get_queryset(self, **hints: Any) -> QuerySet: ...
+    def get_queryset(self, **hints: Any) -> QuerySet[Any]: ...
     def get_prefetch_queryset(
-        self, instances: list[Model], queryset: QuerySet | None = ...
-    ) -> tuple[QuerySet, Callable, Callable, bool, str, bool]: ...
+        self, instances: list[Model], queryset: QuerySet[Any] | None = ...
+    ) -> tuple[QuerySet[Any], Callable[..., Any], Callable[..., Any], bool, str, bool]: ...
+    def get_prefetch_querysets(
+        self, instances: list[Model], querysets: list[QuerySet[Any]] | None = ...
+    ) -> tuple[QuerySet[Any], Callable[..., Any], Callable[..., Any], bool, str, bool]: ...
     def get_object(self, instance: Model) -> Model: ...
     def __get__(
         self, instance: Model | None, cls: type[Model] | None = ...
     ) -> Model | ForwardManyToOneDescriptor | None: ...
     def __set__(self, instance: Model, value: Model | None) -> None: ...
-    def __reduce__(self) -> tuple[Callable, tuple[type[Model], str]]: ...
+    def __reduce__(self) -> tuple[Callable[..., Any], tuple[type[Model], str]]: ...
 
 class ForwardOneToOneDescriptor(ForwardManyToOneDescriptor[_F]):
     def get_object(self, instance: Model) -> Model: ...
 
 class ReverseOneToOneDescriptor(Generic[_From, _To]):
     """
     In the example::
@@ -56,14 +59,17 @@
     @cached_property
     def RelatedObjectDoesNotExist(self) -> type[ObjectDoesNotExist]: ...
     def is_cached(self, instance: _From) -> bool: ...
     def get_queryset(self, **hints: Any) -> QuerySet[_To]: ...
     def get_prefetch_queryset(
         self, instances: list[_From], queryset: QuerySet[_To] | None = ...
     ) -> tuple[QuerySet[_To], Callable[..., Any], Callable[..., Any], bool, str, bool]: ...
+    def get_prefetch_querysets(
+        self, instances: list[_From], querysets: list[QuerySet[_To]] | None = ...
+    ) -> tuple[QuerySet[_To], Callable[..., Any], Callable[..., Any], bool, str, bool]: ...
     @overload
     def __get__(self, instance: None, cls: Any = ...) -> ReverseOneToOneDescriptor[_From, _To]: ...
     @overload
     def __get__(self, instance: _From, cls: Any = ...) -> _To: ...
     def __set__(self, instance: _From, value: _To | None) -> None: ...
     def __reduce__(self) -> tuple[Callable[..., Any], tuple[type[_To], str]]: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/fields/related_lookups.pyi` & `django_stubs-5.0.1/django-stubs/db/models/fields/related_lookups.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/fields/reverse_related.pyi` & `django_stubs-5.0.1/django-stubs/db/models/fields/reverse_related.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections.abc import Callable, Sequence
 from typing import Any, Literal
 
 from django.db.models.base import Model
 from django.db.models.fields import AutoField, Field, _AllLimitChoicesTo, _ChoicesList, _LimitChoicesTo
 from django.db.models.fields.related import ForeignKey, ForeignObject, ManyToManyField, OneToOneField
-from django.db.models.lookups import Lookup, StartsWith
+from django.db.models.lookups import Lookup, StartsWith, Transform
 from django.db.models.query_utils import FilteredRelation, PathInfo
 from django.db.models.sql.where import WhereNode
 from django.utils.functional import cached_property
 
 from .mixins import FieldCacheMixin
 
 # Common note: `model` and `through` can be of type `str` when passed to `__init__`.
@@ -58,28 +58,31 @@
     @cached_property
     def many_to_one(self) -> bool: ...
     @cached_property
     def one_to_many(self) -> bool: ...
     @cached_property
     def one_to_one(self) -> bool: ...
     def get_lookup(self, lookup_name: str) -> type[Lookup] | None: ...
+    def get_lookups(self) -> dict[str, Any]: ...
+    def get_transform(self, name: str) -> type[Transform] | None: ...
     def get_internal_type(self) -> str: ...
     @property
     def db_type(self) -> Any: ...
     # Yes, seems that `get_choices` will fail if `limit_choices_to=None`
     # and `self.limit_choices_to` is callable.
     def get_choices(
         self,
         include_blank: bool = ...,
         blank_choice: _ChoicesList = ...,
         limit_choices_to: _LimitChoicesTo | None = ...,
         ordering: Sequence[str] = ...,
     ) -> _ChoicesList: ...
     def is_hidden(self) -> bool: ...
     def get_joining_columns(self) -> tuple: ...
+    def get_joining_fields(self) -> tuple[tuple[Field, Field], ...]: ...
     def get_extra_restriction(
         self, where_class: type[WhereNode], alias: str, related_alias: str
     ) -> StartsWith | WhereNode | None: ...
     def set_field_name(self) -> None: ...
     def get_accessor_name(self, model: type[Model] | None = ...) -> str | None: ...
     def get_path_info(self, filtered_relation: FilteredRelation | None = ...) -> list[PathInfo]: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/functions/__init__.pyi` & `django_stubs-5.0.1/django-stubs/db/models/functions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/functions/comparison.pyi` & `django_stubs-5.0.1/django-stubs/db/models/functions/comparison.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/functions/math.pyi` & `django_stubs-5.0.1/django-stubs/db/models/functions/math.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/functions/text.pyi` & `django_stubs-5.0.1/django-stubs/db/models/functions/text.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/functions/window.pyi` & `django_stubs-5.0.1/django-stubs/db/models/functions/window.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/indexes.pyi` & `django_stubs-5.0.1/django-stubs/db/models/indexes.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/lookups.pyi` & `django_stubs-5.0.1/django-stubs/db/models/lookups.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from collections.abc import Iterable, Mapping
 from typing import Any, Generic, Literal, TypeVar
 
+from django.core.exceptions import EmptyResultSet
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models.expressions import Expression, Func
 from django.db.models.fields import BooleanField
 from django.db.models.query_utils import RegisterLookupMixin
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType, _ParamT
 from django.utils.datastructures import OrderedSet
 from django.utils.functional import cached_property
@@ -78,20 +79,28 @@
 class Exact(FieldGetDbPrepValueMixin, BuiltinLookup[_T]): ...
 class IExact(BuiltinLookup[_T]): ...
 class GreaterThan(FieldGetDbPrepValueMixin, BuiltinLookup[_T]): ...
 class GreaterThanOrEqual(FieldGetDbPrepValueMixin, BuiltinLookup[_T]): ...
 class LessThan(FieldGetDbPrepValueMixin, BuiltinLookup[_T]): ...
 class LessThanOrEqual(FieldGetDbPrepValueMixin, BuiltinLookup[_T]): ...
 
+class IntegerFieldOverflow:
+    underflow_exception: type[EmptyResultSet]
+    overflow_exception: type[EmptyResultSet]
+    def process_rhs(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
+
 class IntegerFieldFloatRounding:
     rhs: Any
     def get_prep_lookup(self) -> Any: ...
 
-class IntegerGreaterThanOrEqual(IntegerFieldFloatRounding, GreaterThanOrEqual[int | float]): ...
-class IntegerLessThan(IntegerFieldFloatRounding, LessThan[int | float]): ...
+class IntegerFieldExact(IntegerFieldOverflow, Exact[int | float]): ...
+class IntegerGreaterThan(IntegerFieldOverflow, GreaterThan[int | float]): ...
+class IntegerGreaterThanOrEqual(IntegerFieldOverflow, IntegerFieldFloatRounding, GreaterThanOrEqual[int | float]): ...
+class IntegerLessThan(IntegerFieldOverflow, IntegerFieldFloatRounding, LessThan[int | float]): ...
+class IntegerLessThanOrEqual(IntegerFieldOverflow, LessThanOrEqual[int | float]): ...
 
 class In(FieldGetDbPrepValueIterableMixin, BuiltinLookup):
     def split_parameter_list_as_sql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> Any: ...
 
 class PatternLookup(BuiltinLookup[str]):
     param_pattern: str
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/manager.pyi` & `django_stubs-5.0.1/django-stubs/db/models/manager.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from typing import Any, Generic, NoReturn, TypeVar, overload
 
 from django.db.models.base import Model
 from django.db.models.expressions import Combinable, OrderBy
 from django.db.models.query import QuerySet, RawQuerySet
 from typing_extensions import Self
 
-from django_stubs_ext import ValuesQuerySet
-
 _T = TypeVar("_T", bound=Model, covariant=True)
 
 class BaseManager(Generic[_T]):
     cache: Callable[[], Self]  # django-cacheops
     creation_counter: int
     auto_created: bool
     use_in_migrations: bool
@@ -103,23 +101,21 @@
         self,
         raw_query: str,
         params: Any = ...,
         translations: dict[str, str] | None = ...,
         using: str | None = ...,
     ) -> RawQuerySet: ...
     # The type of values may be overridden to be more specific in the mypy plugin, depending on the fields param
-    def values(self, *fields: str | Combinable, **expressions: Any) -> ValuesQuerySet[_T, dict[str, Any]]: ...
+    def values(self, *fields: str | Combinable, **expressions: Any) -> QuerySet[_T, dict[str, Any]]: ...
     # The type of values_list may be overridden to be more specific in the mypy plugin, depending on the fields param
-    def values_list(
-        self, *fields: str | Combinable, flat: bool = ..., named: bool = ...
-    ) -> ValuesQuerySet[_T, Any]: ...
-    def dates(self, field_name: str, kind: str, order: str = ...) -> ValuesQuerySet[_T, datetime.date]: ...
+    def values_list(self, *fields: str | Combinable, flat: bool = ..., named: bool = ...) -> QuerySet[_T, Any]: ...
+    def dates(self, field_name: str, kind: str, order: str = ...) -> QuerySet[_T, datetime.date]: ...
     def datetimes(
         self, field_name: str, kind: str, order: str = ..., tzinfo: datetime.tzinfo | None = ...
-    ) -> ValuesQuerySet[_T, datetime.datetime]: ...
+    ) -> QuerySet[_T, datetime.datetime]: ...
     def none(self) -> QuerySet[_T]: ...
     def all(self) -> QuerySet[_T]: ...
     def filter(self, *args: Any, **kwargs: Any) -> QuerySet[_T]: ...
     def exclude(self, *args: Any, **kwargs: Any) -> QuerySet[_T]: ...
     def complex_filter(self, filter_obj: Any) -> QuerySet[_T]: ...
     def count(self) -> int: ...
     async def acount(self) -> int: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/options.pyi` & `django_stubs-5.0.1/django-stubs/db/models/options.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/query.pyi` & `django_stubs-5.0.1/django-stubs/db/models/query.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,129 +1,132 @@
 import datetime
 from collections.abc import AsyncIterator, Collection, Iterable, Iterator, MutableMapping, Sequence, Sized
-from typing import Any, Generic, NamedTuple, TypeVar, overload
+from typing import Any, Generic, NamedTuple, overload
 
 from django.db.backends.utils import _ExecuteQuery
 from django.db.models import Manager
 from django.db.models.base import Model
 from django.db.models.expressions import Combinable, OrderBy
 from django.db.models.sql.query import Query, RawQuery
 from django.utils.functional import cached_property
-from typing_extensions import Self, TypeAlias
+from typing_extensions import Self, TypeAlias, TypeVar
 
-_T = TypeVar("_T", bound=Model, covariant=True)
-_Row = TypeVar("_Row", covariant=True)
+_T = TypeVar("_T", covariant=True)
+_Model = TypeVar("_Model", bound=Model, covariant=True)
+_Row = TypeVar("_Row", covariant=True, default=_Model)  # ONLY use together with _Model
 _QS = TypeVar("_QS", bound=_QuerySet)
 _TupleT = TypeVar("_TupleT", bound=tuple[Any, ...], covariant=True)
 
 MAX_GET_RESULTS: int
 REPR_OUTPUT_SIZE: int
 
-class BaseIterable(Generic[_Row]):
+class BaseIterable(Generic[_T]):
     queryset: QuerySet[Model]
     chunked_fetch: bool
     chunk_size: int
     def __init__(self, queryset: QuerySet[Model], chunked_fetch: bool = ..., chunk_size: int = ...) -> None: ...
-    def __aiter__(self) -> AsyncIterator[_Row]: ...
+    def __aiter__(self) -> AsyncIterator[_T]: ...
 
-class ModelIterable(Generic[_T], BaseIterable[_T]):
-    def __iter__(self) -> Iterator[_T]: ...
+class ModelIterable(Generic[_Model], BaseIterable[_Model]):
+    def __iter__(self) -> Iterator[_Model]: ...
 
 class RawModelIterable(BaseIterable[dict[str, Any]]):
     def __iter__(self) -> Iterator[dict[str, Any]]: ...
 
 class ValuesIterable(BaseIterable[dict[str, Any]]):
     def __iter__(self) -> Iterator[dict[str, Any]]: ...
 
 class ValuesListIterable(BaseIterable[_TupleT]):
     def __iter__(self) -> Iterator[_TupleT]: ...
 
 class NamedValuesListIterable(ValuesListIterable[NamedTuple]):
     def __iter__(self) -> Iterator[NamedTuple]: ...
 
-class FlatValuesListIterable(BaseIterable[_Row]):
-    def __iter__(self) -> Iterator[_Row]: ...
+class FlatValuesListIterable(BaseIterable[_T]):
+    def __iter__(self) -> Iterator[_T]: ...
 
-class _QuerySet(Generic[_T, _Row], Iterable[_Row], Sized):
-    model: type[_T]
+class QuerySet(Generic[_Model, _Row], Iterable[_Row], Sized):
+    model: type[_Model]
     query: Query
     _iterable_class: type[BaseIterable]
     _result_cache: list[_Row] | None
     def __init__(
         self,
         model: type[Model] | None = ...,
         query: Query | None = ...,
         using: str | None = ...,
         hints: dict[str, Model] | None = ...,
     ) -> None: ...
     @classmethod
-    def as_manager(cls) -> Manager[_T]: ...
+    def as_manager(cls) -> Manager[_Model]: ...
     def __len__(self) -> int: ...
     def __bool__(self) -> bool: ...
-    def __class_getitem__(cls: type[_QS], item: type[_T]) -> type[_QS]: ...
+    def __class_getitem__(cls: type[_QS], item: type[_Model]) -> type[_QS]: ...
     def __getstate__(self) -> dict[str, Any]: ...
     # Technically, the other QuerySet must be of the same type _T, but _T is covariant
-    def __and__(self, other: _QuerySet[_T, _Row]) -> Self: ...
-    def __or__(self, other: _QuerySet[_T, _Row]) -> Self: ...
+    def __and__(self, other: QuerySet[_Model, _Row]) -> Self: ...
+    def __or__(self, other: QuerySet[_Model, _Row]) -> Self: ...
     # IMPORTANT: When updating any of the following methods' signatures, please ALSO modify
     # the corresponding method in BaseManager.
     def iterator(self, chunk_size: int | None = ...) -> Iterator[_Row]: ...
     def aiterator(self, chunk_size: int = ...) -> AsyncIterator[_Row]: ...
     def aggregate(self, *args: Any, **kwargs: Any) -> dict[str, Any]: ...
     async def aaggregate(self, *args: Any, **kwargs: Any) -> dict[str, Any]: ...
     def get(self, *args: Any, **kwargs: Any) -> _Row: ...
     async def aget(self, *args: Any, **kwargs: Any) -> _Row: ...
-    def create(self, **kwargs: Any) -> _T: ...
-    async def acreate(self, **kwargs: Any) -> _T: ...
+    def create(self, **kwargs: Any) -> _Model: ...
+    async def acreate(self, **kwargs: Any) -> _Model: ...
     def bulk_create(
         self,
-        objs: Iterable[_T],
+        objs: Iterable[_Model],
         batch_size: int | None = ...,
         ignore_conflicts: bool = ...,
         update_conflicts: bool = ...,
         update_fields: Collection[str] | None = ...,
         unique_fields: Collection[str] | None = ...,
-    ) -> list[_T]: ...
+    ) -> list[_Model]: ...
     async def abulk_create(
         self,
-        objs: Iterable[_T],
+        objs: Iterable[_Model],
         batch_size: int | None = ...,
         ignore_conflicts: bool = ...,
         update_conflicts: bool = ...,
         update_fields: Collection[str] | None = ...,
         unique_fields: Collection[str] | None = ...,
-    ) -> list[_T]: ...
-    def bulk_update(self, objs: Iterable[_T], fields: Iterable[str], batch_size: int | None = ...) -> int: ...
-    async def abulk_update(self, objs: Iterable[_T], fields: Iterable[str], batch_size: int | None = ...) -> int: ...
-    def get_or_create(self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any) -> tuple[_T, bool]: ...
+    ) -> list[_Model]: ...
+    def bulk_update(self, objs: Iterable[_Model], fields: Iterable[str], batch_size: int | None = ...) -> int: ...
+    async def abulk_update(
+        self, objs: Iterable[_Model], fields: Iterable[str], batch_size: int | None = ...
+    ) -> int: ...
+    def get_or_create(self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any) -> tuple[_Model, bool]: ...
     async def aget_or_create(
         self, defaults: MutableMapping[str, Any] | None = ..., **kwargs: Any
-    ) -> tuple[_T, bool]: ...
+    ) -> tuple[_Model, bool]: ...
     def update_or_create(
         self,
         defaults: MutableMapping[str, Any] | None = ...,
         create_defaults: MutableMapping[str, Any] | None = ...,
         **kwargs: Any,
-    ) -> tuple[_T, bool]: ...
+    ) -> tuple[_Model, bool]: ...
     async def aupdate_or_create(
         self,
         defaults: MutableMapping[str, Any] | None = ...,
         create_defaults: MutableMapping[str, Any] | None = ...,
         **kwargs: Any,
-    ) -> tuple[_T, bool]: ...
+    ) -> tuple[_Model, bool]: ...
     def earliest(self, *fields: str | OrderBy) -> _Row: ...
     async def aearliest(self, *fields: str | OrderBy) -> _Row: ...
     def latest(self, *fields: str | OrderBy) -> _Row: ...
     async def alatest(self, *fields: str | OrderBy) -> _Row: ...
     def first(self) -> _Row | None: ...
     async def afirst(self) -> _Row | None: ...
     def last(self) -> _Row | None: ...
     async def alast(self) -> _Row | None: ...
-    def in_bulk(self, id_list: Iterable[Any] | None = ..., *, field_name: str = ...) -> dict[Any, _T]: ...
-    async def ain_bulk(self, id_list: Iterable[Any] | None = ..., *, field_name: str = ...) -> dict[Any, _T]: ...
+    def in_bulk(self, id_list: Iterable[Any] | None = ..., *, field_name: str = ...) -> dict[Any, _Model]: ...
+    async def ain_bulk(self, id_list: Iterable[Any] | None = ..., *, field_name: str = ...) -> dict[Any, _Model]: ...
     def delete(self) -> tuple[int, dict[str, int]]: ...
     async def adelete(self) -> tuple[int, dict[str, int]]: ...
     def update(self, **kwargs: Any) -> int: ...
     async def aupdate(self, **kwargs: Any) -> int: ...
     def exists(self) -> bool: ...
     async def aexists(self) -> bool: ...
     def explain(self, *, format: Any | None = ..., **options: Any) -> str: ...
@@ -134,21 +137,21 @@
         self,
         raw_query: _ExecuteQuery,
         params: Any = ...,
         translations: dict[str, str] | None = ...,
         using: str | None = ...,
     ) -> RawQuerySet: ...
     # The type of values may be overridden to be more specific in the mypy plugin, depending on the fields param
-    def values(self, *fields: str | Combinable, **expressions: Any) -> _QuerySet[_T, dict[str, Any]]: ...
+    def values(self, *fields: str | Combinable, **expressions: Any) -> QuerySet[_Model, dict[str, Any]]: ...
     # The type of values_list may be overridden to be more specific in the mypy plugin, depending on the fields param
-    def values_list(self, *fields: str | Combinable, flat: bool = ..., named: bool = ...) -> _QuerySet[_T, Any]: ...
-    def dates(self, field_name: str, kind: str, order: str = ...) -> _QuerySet[_T, datetime.date]: ...
+    def values_list(self, *fields: str | Combinable, flat: bool = ..., named: bool = ...) -> QuerySet[_Model, Any]: ...
+    def dates(self, field_name: str, kind: str, order: str = ...) -> QuerySet[_Model, datetime.date]: ...
     def datetimes(
         self, field_name: str, kind: str, order: str = ..., tzinfo: datetime.tzinfo | None = ...
-    ) -> _QuerySet[_T, datetime.datetime]: ...
+    ) -> QuerySet[_Model, datetime.datetime]: ...
     def none(self) -> Self: ...
     def all(self) -> Self: ...
     def filter(self, *args: Any, **kwargs: Any) -> Self: ...
     def exclude(self, *args: Any, **kwargs: Any) -> Self: ...
     def complex_filter(self, filter_obj: Any) -> Self: ...
     def count(self) -> int: ...
     async def acount(self) -> int: ...
@@ -169,15 +172,15 @@
         self,
         select: dict[str, Any] | None = ...,
         where: Sequence[str] | None = ...,
         params: Sequence[Any] | None = ...,
         tables: Sequence[str] | None = ...,
         order_by: Sequence[str] | None = ...,
         select_params: Sequence[Any] | None = ...,
-    ) -> _QuerySet[Any, Any]: ...
+    ) -> QuerySet[Any, Any]: ...
     def reverse(self) -> Self: ...
     def defer(self, *fields: Any) -> Self: ...
     def only(self, *fields: Any) -> Self: ...
     def using(self, alias: str | None) -> Self: ...
     @property
     def ordered(self) -> bool: ...
     @property
@@ -188,61 +191,61 @@
     def __aiter__(self) -> AsyncIterator[_Row]: ...
     @overload
     def __getitem__(self, i: int) -> _Row: ...
     @overload
     def __getitem__(self, s: slice) -> Self: ...
     def __reversed__(self) -> Iterator[_Row]: ...
 
-class RawQuerySet(Iterable[_T], Sized):
+class RawQuerySet(Iterable[_Model], Sized):
     query: RawQuery
     def __init__(
         self,
         raw_query: RawQuery | str,
         model: type[Model] | None = ...,
         query: Query | None = ...,
         params: tuple[Any] = ...,
         translations: dict[str, str] | None = ...,
         using: str = ...,
         hints: dict[str, Model] | None = ...,
     ) -> None: ...
     def __len__(self) -> int: ...
-    def __iter__(self) -> Iterator[_T]: ...
+    def __iter__(self) -> Iterator[_Model]: ...
     def __bool__(self) -> bool: ...
     @overload
-    def __getitem__(self, k: int) -> _T: ...
+    def __getitem__(self, k: int) -> _Model: ...
     @overload
     def __getitem__(self, k: str) -> Any: ...
     @overload
-    def __getitem__(self, k: slice) -> RawQuerySet[_T]: ...
+    def __getitem__(self, k: slice) -> RawQuerySet[_Model]: ...
     @cached_property
     def columns(self) -> list[str]: ...
     @property
     def db(self) -> str: ...
-    def iterator(self) -> Iterator[_T]: ...
+    def iterator(self) -> Iterator[_Model]: ...
     @cached_property
     def model_fields(self) -> dict[str, str]: ...
-    def prefetch_related(self, *lookups: Any) -> RawQuerySet[_T]: ...
+    def prefetch_related(self, *lookups: Any) -> RawQuerySet[_Model]: ...
     def resolve_model_init_order(self) -> tuple[list[str], list[int], list[tuple[str, int]]]: ...
-    def using(self, alias: str | None) -> RawQuerySet[_T]: ...
-
-_QuerySetAny: TypeAlias = _QuerySet  # noqa: PYI047
+    def using(self, alias: str | None) -> RawQuerySet[_Model]: ...
 
-QuerySet: TypeAlias = _QuerySet[_T, _T]
+# Deprecated alias of QuerySet, for compatibility only.
+_QuerySet: TypeAlias = QuerySet
 
 class Prefetch:
     prefetch_through: str
     prefetch_to: str
     queryset: QuerySet | None
     to_attr: str | None
     def __init__(self, lookup: str, queryset: QuerySet | None = ..., to_attr: str | None = ...) -> None: ...
     def __getstate__(self) -> dict[str, Any]: ...
     def add_prefix(self, prefix: str) -> None: ...
     def get_current_prefetch_to(self, level: int) -> str: ...
     def get_current_to_attr(self, level: int) -> tuple[str, str]: ...
     def get_current_queryset(self, level: int) -> QuerySet | None: ...
+    def get_current_querysets(self, level: int) -> list[QuerySet] | None: ...
 
-def prefetch_related_objects(model_instances: Iterable[_T], *related_lookups: str | Prefetch) -> None: ...
-async def aprefetch_related_objects(model_instances: Iterable[_T], *related_lookups: str | Prefetch) -> None: ...
+def prefetch_related_objects(model_instances: Iterable[_Model], *related_lookups: str | Prefetch) -> None: ...
+async def aprefetch_related_objects(model_instances: Iterable[_Model], *related_lookups: str | Prefetch) -> None: ...
 def get_prefetcher(instance: Model, through_attr: str, to_attr: str) -> tuple[Any, Any, bool, bool]: ...
 
 class InstanceCheckMeta(type): ...
 class EmptyQuerySet(metaclass=InstanceCheckMeta): ...
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/query_utils.pyi` & `django_stubs-5.0.1/django-stubs/db/models/query_utils.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from django.db.models.fields import Field
 from django.db.models.fields.mixins import FieldCacheMixin
 from django.db.models.lookups import Lookup, Transform
 from django.db.models.sql.compiler import SQLCompiler, _AsSqlType
 from django.db.models.sql.query import Query
 from django.db.models.sql.where import WhereNode
 from django.utils import tree
+from django.utils.functional import cached_property
 
 PathInfo = namedtuple(
     "PathInfo", ["from_opts", "to_opts", "target_fields", "join_field", "m2m", "direct", "filtered_relation"]
 )
 
 class InvalidQuery(Exception): ...
 
@@ -40,14 +41,16 @@
         reuse: set[str] | None = ...,
         summarize: bool = ...,
         for_save: bool = ...,
     ) -> WhereNode: ...
     def flatten(self) -> Iterator[Incomplete]: ...
     def check(self, against: dict[str, Any], using: str = ...) -> bool: ...
     def deconstruct(self) -> tuple[str, Sequence[Any], dict[str, Any]]: ...
+    @cached_property
+    def referenced_base_fields(self) -> set[str]: ...
 
 class DeferredAttribute:
     field: Field
     def __init__(self, field: Field) -> None: ...
     def __get__(self, instance: Model | None, cls: type[Model] | None = None) -> Any: ...
 
 _R = TypeVar("_R", bound=type)
@@ -81,12 +84,12 @@
 ) -> tuple[Literal[False] | _E, Sequence[str]]: ...
 def check_rel_lookup_compatibility(model: type[Model], target_opts: Any, field: FieldCacheMixin) -> bool: ...
 
 class FilteredRelation:
     relation_name: str
     alias: str | None
     condition: Q
-    path: list[str]
     def __init__(self, relation_name: str, *, condition: Q = ...) -> None: ...
     def clone(self) -> FilteredRelation: ...
-    def resolve_expression(self, *args: Any, **kwargs: Any) -> None: ...
+    def relabeled_clone(self, change_map: dict[str, str]) -> FilteredRelation: ...
+    def resolve_expression(self, query: Query, reuse: set[str], *args: Any, **kwargs: Any) -> FilteredRelation: ...
     def as_sql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/signals.pyi` & `django_stubs-5.0.1/django-stubs/db/models/signals.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/sql/compiler.pyi` & `django_stubs-5.0.1/django-stubs/db/models/sql/compiler.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 from decimal import Decimal
 from typing import Any, Literal, overload
 from uuid import UUID
 
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.backends.utils import CursorWrapper
 from django.db.models.base import Model
-from django.db.models.expressions import BaseExpression, Expression
+from django.db.models.expressions import BaseExpression, Expression, Ref
 from django.db.models.sql.query import Query
 from django.db.models.sql.subqueries import AggregateQuery, DeleteQuery, InsertQuery, UpdateQuery
 from django.utils.functional import cached_property
 from typing_extensions import TypeAlias
 
 _ParamT: TypeAlias = str | int
 
 _ParamsT: TypeAlias = list[_ParamT]
 _AsSqlType: TypeAlias = tuple[str, _ParamsT]
 
+class PositionRef(Ref):
+    def __init__(self, ordinal: str, refs: str, source: Expression) -> None: ...
+
 class SQLCompiler:
     query: Query
     connection: BaseDatabaseWrapper
     using: str | None
     quote_cache: Any
     select: Any
     annotation_col_map: Any
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/sql/datastructures.pyi` & `django_stubs-5.0.1/django-stubs/db/models/sql/datastructures.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -29,21 +29,19 @@
         join_type: str,
         join_field: FieldCacheMixin,
         nullable: bool,
         filtered_relation: FilteredRelation | None = ...,
     ) -> None: ...
     def as_sql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
     def relabeled_clone(self, change_map: dict[str | None, str]) -> Join: ...
-    def equals(self, other: BaseTable | Join, with_filtered_relation: bool) -> bool: ...
     def demote(self) -> Join: ...
     def promote(self) -> Join: ...
 
 class BaseTable:
     join_type: Any
     parent_alias: Any
     filtered_relation: Any
     table_name: str
     table_alias: str | None
     def __init__(self, table_name: str, alias: str | None) -> None: ...
     def as_sql(self, compiler: SQLCompiler, connection: BaseDatabaseWrapper) -> _AsSqlType: ...
     def relabeled_clone(self, change_map: dict[str | None, str]) -> BaseTable: ...
-    def equals(self, other: Join, with_filtered_relation: bool) -> bool: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/sql/query.pyi` & `django_stubs-5.0.1/django-stubs/db/models/sql/query.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -107,42 +107,40 @@
     def demote_joins(self, aliases: Iterable[str]) -> None: ...
     def reset_refcounts(self, to_counts: dict[str, int]) -> None: ...
     def change_aliases(self, change_map: dict[str | None, str]) -> None: ...
     def bump_prefix(self, outer_query: Query) -> None: ...
     def get_initial_alias(self) -> str: ...
     def count_active_tables(self) -> int: ...
     def resolve_expression(self, query: Query, *args: Any, **kwargs: Any) -> Query: ...  # type: ignore[override]
-    def resolve_lookup_value(self, value: Any, can_reuse: set[str] | None, allow_joins: bool) -> Any: ...
+    def resolve_lookup_value(
+        self, value: Any, can_reuse: set[str] | None, allow_joins: bool, summarize: bool = False
+    ) -> Any: ...
     def solve_lookup_type(self, lookup: str) -> tuple[Sequence[str], Sequence[str], Expression | Literal[False]]: ...
     def build_filter(
         self,
         filter_expr: Q | Expression | dict[str, str] | tuple[str, Any],
         branch_negated: bool = ...,
         current_negated: bool = ...,
         can_reuse: set[str] | None = ...,
         allow_joins: bool = ...,
         split_subq: bool = ...,
-        reuse_with_filtered_relation: bool = ...,
         check_filterable: bool = ...,
+        update_join_types: bool = ...,
     ) -> tuple[WhereNode, Iterable[str]]: ...
     def add_filter(self, filter_clause: tuple[str, Any]) -> None: ...
     def add_q(self, q_object: Q) -> None: ...
     def build_where(self, filter_expr: Q | Expression | dict[str, str] | tuple[str, Any]) -> WhereNode: ...
-    def build_filtered_relation_q(
-        self, q_object: Q, reuse: set[str], branch_negated: bool = ..., current_negated: bool = ...
-    ) -> WhereNode: ...
     def add_filtered_relation(self, filtered_relation: FilteredRelation, alias: str) -> None: ...
     def setup_joins(
         self,
         names: Sequence[str],
         opts: Any,
         alias: str,
         can_reuse: set[str] | None = ...,
         allow_many: bool = ...,
-        reuse_with_filtered_relation: bool = ...,
     ) -> JoinInfo: ...
     def trim_joins(
         self, targets: tuple[Field, ...], joins: list[str], path: list[PathInfo]
     ) -> tuple[tuple[Field, ...], str, list[str]]: ...
     def resolve_ref(
         self, name: str, allow_joins: bool = ..., reuse: set[str] | None = ..., summarize: bool = ...
     ) -> Expression: ...
@@ -195,15 +193,17 @@
     def extra_select(self) -> dict[str, Any]: ...
     def trim_start(self, names_with_path: list[tuple[str, list[PathInfo]]]) -> tuple[str, bool]: ...
     def is_nullable(self, field: Field) -> bool: ...
     def check_filterable(self, expression: Any) -> None: ...
     def build_lookup(self, lookups: Sequence[str], lhs: Expression | Query, rhs: Any) -> Lookup: ...
     def try_transform(self, lhs: Expression | Query, name: str) -> Transform: ...
     def join(
-        self, join: BaseTable | Join, reuse: str | None = ..., reuse_with_filtered_relation: bool = ...
+        self,
+        join: BaseTable | Join,
+        reuse: str | None = ...,
     ) -> str: ...
 
 class JoinPromoter:
     connector: str
     negated: bool
     effective_connector: str
     num_children: int
```

### Comparing `django_stubs-5.0.0/django-stubs/db/models/sql/subqueries.pyi` & `django_stubs-5.0.1/django-stubs/db/models/sql/subqueries.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/sql/where.pyi` & `django_stubs-5.0.1/django-stubs/db/models/sql/where.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/models/utils.pyi` & `django_stubs-5.0.1/django-stubs/db/models/utils.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/transaction.pyi` & `django_stubs-5.0.1/django-stubs/db/transaction.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/db/utils.pyi` & `django_stubs-5.0.1/django-stubs/db/utils.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/dispatch/dispatcher.pyi` & `django_stubs-5.0.1/django-stubs/dispatch/dispatcher.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/forms/__init__.pyi` & `django_stubs-5.0.1/django-stubs/forms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/forms/boundfield.pyi` & `django_stubs-5.0.1/django-stubs/forms/boundfield.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 from collections.abc import Iterable, Iterator
 from typing import Any, overload
 
 from django.forms.fields import Field
 from django.forms.forms import BaseForm
 from django.forms.renderers import BaseRenderer
-from django.forms.utils import ErrorList
+from django.forms.utils import ErrorList, RenderableFieldMixin
 from django.forms.widgets import Widget
 from django.utils.functional import _StrOrPromise, cached_property
 from django.utils.safestring import SafeString
 from typing_extensions import TypeAlias
 
 _AttrsT: TypeAlias = dict[str, str | bool]
 
-class BoundField:
+class BoundField(RenderableFieldMixin):
     form: BaseForm
     field: Field
     name: str
     html_name: str
     html_initial_name: str
     html_initial_id: str
     label: _StrOrPromise
     help_text: _StrOrPromise
+    renderer: BaseRenderer
     def __init__(self, form: BaseForm, field: Field, name: str) -> None: ...
     @cached_property
     def subwidgets(self) -> list[BoundWidget]: ...
     def __bool__(self) -> bool: ...
     def __iter__(self) -> Iterator[BoundWidget]: ...
     def __len__(self) -> int: ...
     @overload
     def __getitem__(self, idx: int | str) -> BoundWidget: ...
     @overload
     def __getitem__(self, idx: slice) -> list[BoundWidget]: ...
     @property
     def errors(self) -> ErrorList: ...
+    @property
+    def template_name(self) -> str: ...
     def as_widget(
         self, widget: Widget | None = ..., attrs: _AttrsT | None = ..., only_initial: bool = ...
     ) -> SafeString: ...
     def as_text(self, attrs: _AttrsT | None = ..., **kwargs: Any) -> SafeString: ...
     def __html__(self) -> SafeString: ...
     def as_textarea(self, attrs: _AttrsT | None = ..., **kwargs: Any) -> SafeString: ...
     def as_hidden(self, attrs: _AttrsT | None = ..., **kwargs: Any) -> SafeString: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/forms/fields.pyi` & `django_stubs-5.0.1/django-stubs/forms/fields.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         help_text: _StrOrPromise = ...,
         error_messages: _ErrorMessagesMapping | None = ...,
         show_hidden_initial: bool = ...,
         validators: Sequence[_ValidatorCallable] = ...,
         localize: bool = ...,
         disabled: bool = ...,
         label_suffix: str | None = ...,
+        template_name: str | None = ...,
     ) -> None: ...
     def prepare_value(self, value: Any) -> Any: ...
     def to_python(self, value: Any | None) -> Any | None: ...
     def validate(self, value: Any) -> None: ...
     def run_validators(self, value: Any) -> None: ...
     def clean(self, value: Any) -> Any: ...
     def bound_data(self, data: Any, initial: Any) -> Any: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/forms/forms.pyi` & `django_stubs-5.0.1/django-stubs/forms/forms.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from django.core.exceptions import ValidationError
 from django.forms.boundfield import BoundField
 from django.forms.fields import Field
 from django.forms.renderers import BaseRenderer
 from django.forms.utils import ErrorDict, ErrorList, RenderableFormMixin, _DataT, _FilesT
 from django.forms.widgets import Media, MediaDefiningClass
 from django.utils.functional import _StrOrPromise, cached_property
-from django.utils.safestring import SafeString
 
 class DeclarativeFieldsMetaclass(MediaDefiningClass): ...
 
 class BaseForm(RenderableFormMixin):
     default_renderer: BaseRenderer | type[BaseRenderer] | None
     field_order: Iterable[str] | None
     use_required_attribute: bool
@@ -67,19 +66,11 @@
     def changed_data(self) -> list[str]: ...
     @property
     def media(self) -> Media: ...
     def is_multipart(self) -> bool: ...
     def hidden_fields(self) -> list[BoundField]: ...
     def visible_fields(self) -> list[BoundField]: ...
     def get_initial_for_field(self, field: Field, field_name: str) -> Any: ...
-    def _html_output(
-        self,
-        normal_row: str,
-        error_row: str,
-        row_ender: str,
-        help_text_html: str,
-        errors_on_separate_row: bool,
-    ) -> SafeString: ...
 
-class Form(BaseForm):
+class Form(BaseForm, metaclass=DeclarativeFieldsMetaclass):
     base_fields: ClassVar[dict[str, Field]]
     declared_fields: ClassVar[dict[str, Field]]
```

### Comparing `django_stubs-5.0.0/django-stubs/forms/formsets.pyi` & `django_stubs-5.0.1/django-stubs/forms/formsets.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections.abc import Iterator, Mapping, Sequence, Sized
 from typing import Any, Generic, TypeVar
 
 from django.db.models.fields import _ErrorMessagesDict
 from django.forms.forms import BaseForm, Form
+from django.forms.renderers import BaseRenderer
 from django.forms.utils import ErrorList, RenderableFormMixin, _DataT, _FilesT
-from django.forms.widgets import Media, Widget
+from django.forms.widgets import Media, MediaDefiningClass, Widget
 from django.utils.functional import cached_property
 
 TOTAL_FORM_COUNT: str
 INITIAL_FORM_COUNT: str
 MIN_NUM_FORM_COUNT: str
 MAX_NUM_FORM_COUNT: str
 ORDERING_FIELD_NAME: str
@@ -40,16 +41,16 @@
     prefix: str | None
     auto_id: str
     data: _DataT
     files: _FilesT
     initial: Sequence[Mapping[str, Any]] | None
     form_kwargs: dict[str, Any]
     error_class: type[ErrorList]
-    deletion_widget: type[Widget]
-    ordering_widget: type[Widget]
+    deletion_widget: MediaDefiningClass
+    ordering_widget: MediaDefiningClass
     default_error_messages: _ErrorMessagesDict
     template_name_div: str
     template_name_p: str
     template_name_table: str
     template_name_ul: str
     def __init__(
         self,
@@ -57,14 +58,16 @@
         files: _FilesT | None = ...,
         auto_id: str = ...,
         prefix: str | None = ...,
         initial: Sequence[Mapping[str, Any]] | None = ...,
         error_class: type[ErrorList] = ...,
         form_kwargs: dict[str, Any] | None = ...,
         error_messages: Mapping[str, str] | None = ...,
+        form_renderer: BaseRenderer = ...,
+        renderer: BaseRenderer = ...,
     ) -> None: ...
     def __iter__(self) -> Iterator[_F]: ...
     def __getitem__(self, index: int) -> _F: ...
     def __len__(self) -> int: ...
     def __bool__(self) -> bool: ...
     @cached_property
     def management_form(self) -> ManagementForm: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/forms/models.pyi` & `django_stubs-5.0.1/django-stubs/forms/models.pyi`

 * *Files identical despite different names*

```diff
@@ -11,15 +11,15 @@
 from django.forms.fields import ChoiceField, Field, _ClassLevelWidgetT
 from django.forms.forms import BaseForm, DeclarativeFieldsMetaclass
 from django.forms.formsets import BaseFormSet
 from django.forms.renderers import BaseRenderer
 from django.forms.utils import ErrorList, _DataT, _FilesT
 from django.forms.widgets import Widget
 from django.utils.choices import BaseChoiceIterator, CallableChoiceIterator, _Choices, _ChoicesCallable
-from django.utils.datastructures import _IndexableCollection, _PropertyDescriptor
+from django.utils.datastructures import _PropertyDescriptor
 from django.utils.functional import _StrOrPromise
 from typing_extensions import TypeAlias
 
 ALL_FIELDS: Literal["__all__"]
 
 _Fields: TypeAlias = Collection[str] | Literal["__all__"]
 _Widgets: TypeAlias = dict[str, type[Widget] | Widget]
@@ -46,14 +46,15 @@
     localized_fields: _Fields | None = ...,
     labels: _Labels | None = ...,
     help_texts: _HelpTexts | None = ...,
     error_messages: _ErrorMessages | None = ...,
     field_classes: Mapping[str, type[Field]] | None = ...,
     *,
     apply_limit_choices_to: bool = ...,
+    form_declared_fields: _Fields | None = ...,
 ) -> dict[str, Any]: ...
 
 class ModelFormOptions(Generic[_M]):
     model: type[_M]
     fields: _Fields | None
     exclude: _Fields | None
     widgets: _Widgets | None
@@ -121,15 +122,15 @@
         prefix: str | None = ...,
         queryset: QuerySet[_M] | None = ...,
         *,
         initial: Sequence[dict[str, Any]] | None = ...,
         **kwargs: Any,
     ) -> None: ...
     def initial_form_count(self) -> int: ...
-    def get_queryset(self) -> _IndexableCollection[_M]: ...
+    def get_queryset(self) -> QuerySet[_M]: ...
     def save_new(self, form: _ModelFormT, commit: bool = ...) -> _M: ...
     def save_existing(self, form: _ModelFormT, obj: _M, commit: bool = ...) -> _M: ...
     def delete_existing(self, obj: _M, commit: bool = ...) -> None: ...
     saved_forms: list[_ModelFormT]
     def save_m2m(self) -> None: ...
     def save(self, commit: bool = ...) -> list[_M]: ...
     def clean(self) -> None: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/forms/renderers.pyi` & `django_stubs-5.0.1/django-stubs/forms/renderers.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from django.utils.functional import cached_property
 
 def get_default_renderer() -> BaseRenderer: ...
 
 class BaseRenderer:
     form_template_name: str
     formset_template_name: str
+    field_template_name: str
     def get_template(self, template_name: str) -> Any: ...
     def render(self, template_name: str, context: dict[str, Any], request: HttpRequest | None = ...) -> str: ...
 
 class EngineMixin:
     def get_template(self, template_name: str) -> Any: ...
     @cached_property
     def engine(self) -> BaseEngine: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/forms/utils.pyi` & `django_stubs-5.0.1/django-stubs/forms/utils.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -22,16 +22,23 @@
     def get_context(self) -> dict[str, Any]: ...
     def render(
         self,
         template_name: str | None = ...,
         context: dict[str, Any] | None = ...,
         renderer: BaseRenderer | type[BaseRenderer] | None = ...,
     ) -> SafeString: ...
-    __str__ = render
-    __html__ = render
+    # This is a lie, but this is how it is supposed to be used,
+    # in reallity it is `__str__ = __html__ = render`:
+    def __str__(self) -> SafeString: ...
+    def __html__(self) -> SafeString: ...
+
+class RenderableFieldMixin(RenderableMixin):
+    def as_field_group(self) -> SafeString: ...
+    def as_hidden(self) -> SafeString: ...
+    def as_widget(self) -> SafeString: ...
 
 class RenderableFormMixin(RenderableMixin):
     def as_p(self) -> SafeString: ...
     def as_table(self) -> SafeString: ...
     def as_ul(self) -> SafeString: ...
     def as_div(self) -> SafeString: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/forms/widgets.pyi` & `django_stubs-5.0.1/django-stubs/forms/widgets.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     input_type: str
     template_name: str
 
 class MultipleHiddenInput(HiddenInput):
     template_name: str
 
 class FileInput(Input):
+    allow_multiple_selected: bool
     input_type: str
     template_name: str
     needs_multipart_form: bool
     def format_value(self, value: Any) -> None: ...
     def value_from_datadict(self, data: _DataT, files: _FilesT, name: str) -> Any: ...
     def value_omitted_from_data(self, data: _DataT, files: _FilesT, name: str) -> bool: ...
     def use_required_attribute(self, initial: Any) -> bool: ...
@@ -104,14 +105,15 @@
 FILE_INPUT_CONTRADICTION: object
 
 class ClearableFileInput(FileInput):
     clear_checkbox_label: str
     initial_text: str
     input_text: str
     template_name: str
+    checked: bool
     def clear_checkbox_name(self, name: str) -> str: ...
     def clear_checkbox_id(self, name: str) -> str: ...
     def is_initial(self, value: File | str | None) -> bool: ...
     def get_context(self, name: str, value: Any, attrs: _OptAttrs | None) -> dict[str, Any]: ...
     def value_from_datadict(self, data: _DataT, files: _FilesT, name: str) -> Any: ...
     def value_omitted_from_data(self, data: _DataT, files: _FilesT, name: str) -> bool: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/http/__init__.pyi` & `django_stubs-5.0.1/django-stubs/http/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/http/multipartparser.pyi` & `django_stubs-5.0.1/django-stubs/http/multipartparser.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/http/request.pyi` & `django_stubs-5.0.1/django-stubs/http/request.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 from collections.abc import Iterable, Mapping
 from io import BytesIO
 from re import Pattern
-from typing import Any, BinaryIO, Callable, Literal, NoReturn, TypeVar, overload, type_check_only
+from typing import Any, Awaitable, BinaryIO, Callable, Literal, NoReturn, TypeVar, overload, type_check_only
 
 from django.contrib.auth.base_user import AbstractBaseUser
 from django.contrib.auth.models import AnonymousUser
 from django.contrib.sessions.backends.base import SessionBase
 from django.contrib.sites.models import Site
 from django.core.files import uploadedfile, uploadhandler
 from django.urls import ResolverMatch
@@ -53,15 +53,15 @@
     _stream: BinaryIO
     # Attributes added by optional parts of Django
     # django.contrib.admin views:
     current_app: str
     # django.contrib.auth.middleware.AuthenticationMiddleware:
     user: AbstractBaseUser | AnonymousUser
     # django.contrib.auth.middleware.AuthenticationMiddleware:
-    auser: Callable[[], AbstractBaseUser | AnonymousUser]
+    auser: Callable[[], Awaitable[AbstractBaseUser | AnonymousUser]]
     # django.middleware.locale.LocaleMiddleware:
     LANGUAGE_CODE: str
     # django.contrib.sites.middleware.CurrentSiteMiddleware
     site: Site
     # django.contrib.sessions.middleware.SessionMiddleware
     session: SessionBase
     # The magic. If we instantiate HttpRequest directly somewhere, it has
```

### Comparing `django_stubs-5.0.0/django-stubs/http/response.pyi` & `django_stubs-5.0.1/django-stubs/http/response.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/middleware/cache.pyi` & `django_stubs-5.0.1/django-stubs/middleware/cache.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/middleware/common.pyi` & `django_stubs-5.0.1/django-stubs/middleware/common.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/middleware/csrf.pyi` & `django_stubs-5.0.1/django-stubs/middleware/csrf.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/middleware/security.pyi` & `django_stubs-5.0.1/django-stubs/middleware/security.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/shortcuts.pyi` & `django_stubs-5.0.1/django-stubs/shortcuts.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/__init__.pyi` & `django_stubs-5.0.1/django-stubs/template/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/backends/base.pyi` & `django_stubs-5.0.1/django-stubs/template/backends/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/backends/django.pyi` & `django_stubs-5.0.1/django-stubs/template/backends/django.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/backends/jinja2.pyi` & `django_stubs-5.0.1/django-stubs/template/backends/jinja2.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/base.pyi` & `django_stubs-5.0.1/django-stubs/template/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/context.pyi` & `django_stubs-5.0.1/django-stubs/template/context.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/context_processors.pyi` & `django_stubs-5.0.1/django-stubs/template/context_processors.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/defaultfilters.pyi` & `django_stubs-5.0.1/django-stubs/template/defaultfilters.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/defaulttags.pyi` & `django_stubs-5.0.1/django-stubs/template/defaulttags.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/engine.pyi` & `django_stubs-5.0.1/django-stubs/template/engine.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/library.pyi` & `django_stubs-5.0.1/django-stubs/template/library.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/loader.pyi` & `django_stubs-5.0.1/django-stubs/template/loader.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/loader_tags.pyi` & `django_stubs-5.0.1/django-stubs/template/loader_tags.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/loaders/cached.pyi` & `django_stubs-5.0.1/django-stubs/template/loaders/cached.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/loaders/filesystem.pyi` & `django_stubs-5.0.1/django-stubs/template/loaders/filesystem.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/response.pyi` & `django_stubs-5.0.1/django-stubs/template/response.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/smartif.pyi` & `django_stubs-5.0.1/django-stubs/template/smartif.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/template/utils.pyi` & `django_stubs-5.0.1/django-stubs/template/utils.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/templatetags/cache.pyi` & `django_stubs-5.0.1/django-stubs/templatetags/cache.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/templatetags/i18n.pyi` & `django_stubs-5.0.1/django-stubs/templatetags/i18n.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/templatetags/static.pyi` & `django_stubs-5.0.1/django-stubs/templatetags/static.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/templatetags/tz.pyi` & `django_stubs-5.0.1/django-stubs/templatetags/tz.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/test/__init__.pyi` & `django_stubs-5.0.1/django-stubs/test/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/test/client.pyi` & `django_stubs-5.0.1/django-stubs/test/client.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/test/html.pyi` & `django_stubs-5.0.1/django-stubs/test/html.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/test/runner.pyi` & `django_stubs-5.0.1/django-stubs/test/runner.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/test/selenium.pyi` & `django_stubs-5.0.1/django-stubs/test/selenium.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/test/signals.pyi` & `django_stubs-5.0.1/django-stubs/test/signals.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/test/testcases.pyi` & `django_stubs-5.0.1/django-stubs/test/testcases.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/test/utils.pyi` & `django_stubs-5.0.1/django-stubs/test/utils.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/urls/__init__.pyi` & `django_stubs-5.0.1/django-stubs/urls/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/urls/base.pyi` & `django_stubs-5.0.1/django-stubs/urls/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/urls/conf.pyi` & `django_stubs-5.0.1/django-stubs/urls/conf.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 from types import ModuleType
 from typing import Any, Coroutine, overload
 
 from django.urls import URLPattern, URLResolver, _AnyURL
 from django.utils.functional import _StrOrPromise
 from typing_extensions import TypeAlias
 
-from ..conf.urls import IncludedURLConf
+from ..conf.urls import _IncludedURLConf
 from ..http.response import HttpResponseBase
 
 _URLConf: TypeAlias = str | ModuleType | Sequence[_AnyURL]
 
-def include(
-    arg: _URLConf | tuple[_URLConf, str], namespace: str | None = ...
-) -> tuple[Sequence[URLResolver | URLPattern], str | None, str | None]: ...
+def include(arg: _URLConf | tuple[_URLConf, str], namespace: str | None = ...) -> _IncludedURLConf: ...
 
 # path()
 @overload
 def path(
     route: _StrOrPromise, view: Callable[..., HttpResponseBase], kwargs: dict[str, Any] = ..., name: str = ...
 ) -> URLPattern: ...
 @overload
 def path(
     route: _StrOrPromise,
     view: Callable[..., Coroutine[Any, Any, HttpResponseBase]],
     kwargs: dict[str, Any] = ...,
     name: str = ...,
 ) -> URLPattern: ...
 @overload
-def path(route: _StrOrPromise, view: IncludedURLConf, kwargs: dict[str, Any] = ..., name: str = ...) -> URLResolver: ...
+def path(
+    route: _StrOrPromise, view: _IncludedURLConf, kwargs: dict[str, Any] = ..., name: str = ...
+) -> URLResolver: ...
 @overload
 def path(
     route: _StrOrPromise, view: Sequence[URLResolver | str], kwargs: dict[str, Any] = ..., name: str = ...
 ) -> URLResolver: ...
 
 # re_path()
 @overload
@@ -44,13 +44,13 @@
     route: _StrOrPromise,
     view: Callable[..., Coroutine[Any, Any, HttpResponseBase]],
     kwargs: dict[str, Any] = ...,
     name: str = ...,
 ) -> URLPattern: ...
 @overload
 def re_path(
-    route: _StrOrPromise, view: IncludedURLConf, kwargs: dict[str, Any] = ..., name: str = ...
+    route: _StrOrPromise, view: _IncludedURLConf, kwargs: dict[str, Any] = ..., name: str = ...
 ) -> URLResolver: ...
 @overload
 def re_path(
     route: _StrOrPromise, view: Sequence[URLResolver | str], kwargs: dict[str, Any] = ..., name: str = ...
 ) -> URLResolver: ...
```

### Comparing `django_stubs-5.0.0/django-stubs/urls/converters.pyi` & `django_stubs-5.0.1/django-stubs/urls/converters.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/urls/resolvers.pyi` & `django_stubs-5.0.1/django-stubs/urls/resolvers.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/archive.pyi` & `django_stubs-5.0.1/django-stubs/utils/archive.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/autoreload.pyi` & `django_stubs-5.0.1/django-stubs/utils/autoreload.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/cache.pyi` & `django_stubs-5.0.1/django-stubs/utils/cache.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/choices.pyi` & `django_stubs-5.0.1/django-stubs/utils/choices.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/connection.pyi` & `django_stubs-5.0.1/django-stubs/utils/connection.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/crypto.pyi` & `django_stubs-5.0.1/django-stubs/utils/crypto.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/datastructures.pyi` & `django_stubs-5.0.1/django-stubs/utils/datastructures.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/dateformat.pyi` & `django_stubs-5.0.1/django-stubs/utils/dateformat.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/deconstruct.pyi` & `django_stubs-5.0.1/django-stubs/utils/deconstruct.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/decorators.pyi` & `django_stubs-5.0.1/django-stubs/utils/decorators.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/deprecation.pyi` & `django_stubs-5.0.1/django-stubs/utils/deprecation.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/encoding.pyi` & `django_stubs-5.0.1/django-stubs/utils/encoding.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/feedgenerator.pyi` & `django_stubs-5.0.1/django-stubs/utils/feedgenerator.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/formats.pyi` & `django_stubs-5.0.1/django-stubs/utils/formats.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/functional.pyi` & `django_stubs-5.0.1/django-stubs/utils/functional.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/html.pyi` & `django_stubs-5.0.1/django-stubs/utils/html.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/http.pyi` & `django_stubs-5.0.1/django-stubs/utils/http.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/jslex.pyi` & `django_stubs-5.0.1/django-stubs/utils/jslex.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/log.pyi` & `django_stubs-5.0.1/django-stubs/utils/log.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/regex_helper.pyi` & `django_stubs-5.0.1/django-stubs/utils/regex_helper.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/safestring.pyi` & `django_stubs-5.0.1/django-stubs/utils/safestring.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/termcolors.pyi` & `django_stubs-5.0.1/django-stubs/utils/termcolors.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/text.pyi` & `django_stubs-5.0.1/django-stubs/utils/text.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/timezone.pyi` & `django_stubs-5.0.1/django-stubs/utils/timezone.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/translation/__init__.pyi` & `django_stubs-5.0.1/django-stubs/utils/translation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/translation/trans_null.pyi` & `django_stubs-5.0.1/django-stubs/utils/translation/trans_null.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/translation/trans_real.pyi` & `django_stubs-5.0.1/django-stubs/utils/translation/trans_real.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/tree.pyi` & `django_stubs-5.0.1/django-stubs/utils/tree.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/utils/version.pyi` & `django_stubs-5.0.1/django-stubs/utils/version.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/views/debug.pyi` & `django_stubs-5.0.1/django-stubs/views/debug.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/views/decorators/http.pyi` & `django_stubs-5.0.1/django-stubs/views/decorators/http.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/views/defaults.pyi` & `django_stubs-5.0.1/django-stubs/views/defaults.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/views/generic/__init__.pyi` & `django_stubs-5.0.1/django-stubs/views/generic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/views/generic/base.pyi` & `django_stubs-5.0.1/django-stubs/views/generic/base.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/views/generic/dates.pyi` & `django_stubs-5.0.1/django-stubs/views/generic/dates.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/views/generic/detail.pyi` & `django_stubs-5.0.1/django-stubs/views/generic/detail.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/views/generic/edit.pyi` & `django_stubs-5.0.1/django-stubs/views/generic/edit.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/views/generic/list.pyi` & `django_stubs-5.0.1/django-stubs/views/generic/list.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django-stubs/views/i18n.pyi` & `django_stubs-5.0.1/django-stubs/views/i18n.pyi`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/django_stubs.egg-info/PKG-INFO` & `django_stubs-5.0.1/django_stubs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-stubs
-Version: 5.0.0
+Version: 5.0.1
 Summary: Mypy stubs for Django
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
@@ -15,30 +15,31 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: django
 Requires-Dist: asgiref
 Requires-Dist: django-stubs-ext>=5.0.0
 Requires-Dist: tomli; python_version < "3.11"
-Requires-Dist: typing-extensions
+Requires-Dist: typing-extensions>=4.11.0
 Requires-Dist: types-PyYAML
 Provides-Extra: compatible-mypy
 Requires-Dist: mypy~=1.10.0; extra == "compatible-mypy"
 Provides-Extra: redis
 Requires-Dist: redis; extra == "redis"
+Provides-Extra: oracle
+Requires-Dist: oracledb; extra == "oracle"
 
 <img src="https://raw.githubusercontent.com/typeddjango/django-stubs/master/logo.svg" alt="django-stubs">
 
 [![Build status](https://github.com/typeddjango/django-stubs/workflows/test/badge.svg?branch=master&event=push)](https://github.com/typeddjango/django-stubs/actions?query=workflow%3Atest)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Gitter](https://badges.gitter.im/mypy-django/Lobby.svg)](https://gitter.im/mypy-django/Lobby)
 [![StackOverflow](https://shields.io/badge/ask-stackoverflow-orange?logo=stackoverflow)](https://stackoverflow.com/questions/tagged/django-stubs)
@@ -83,14 +84,15 @@
 
 ## Version compatibility
 
 We rely on different `django` and `mypy` versions:
 
 | django-stubs   | Mypy version | Django version | Django partial support | Python version |
 |----------------|--------------|----------------|------------------------|----------------|
+| 5.0.1          | 1.10.x       | 5.0            | 4.2                    | 3.8 - 3.12     |
 | 5.0.0          | 1.10.x       | 5.0            | 4.2, 4.1               | 3.8 - 3.12     |
 | 4.2.7          | 1.7.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.6          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.5          | 1.6.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.12     |
 | 4.2.4          | 1.5.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.3          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
 | 4.2.2          | 1.4.x        | 4.2            | 4.1, 3.2               | 3.8 - 3.11     |
@@ -288,39 +290,14 @@
     return m.foo  # OK, since we said field "foo" was allowed
 
 
 func(MyModel.objects.annotate(foo=Value("")).get(id=1))  # OK
 func(MyModel.objects.annotate(bar=Value("")).get(id=1))  # Error
 ```
 
-### How do I check if something is an instance of QuerySet in runtime?
-
-A limitation of making `QuerySet` generic is that you can not use
-it for `isinstance` checks.
-
-```python
-from django.db.models.query import QuerySet
-
-def foo(obj: object) -> None:
-    if isinstance(obj, QuerySet): # Error: Parameterized generics cannot be used with class or instance checks
-        ...
-```
-
-To get around with this issue without making `QuerySet` non-generic,
-Django-stubs provides `django_stubs_ext.QuerySetAny`, a non-generic
-variant of `QuerySet` suitable for runtime type checking:
-
-```python
-from django_stubs_ext import QuerySetAny
-
-def foo(obj: object) -> None:
-    if isinstance(obj, QuerySetAny):  # OK
-        ...
-```
-
 ### Why am I getting incompatible argument type mentioning `_StrPromise`?
 
 The lazy translation functions of Django (such as `gettext_lazy`) return a `Promise` instead of `str`. These two types [cannot be used interchangeably](https://github.com/typeddjango/django-stubs/pull/1139#issuecomment-1232167698). The return type of these functions was therefore [changed](https://github.com/typeddjango/django-stubs/pull/689) to reflect that.
 
 If you encounter this error in your own code, you can either cast the `Promise` to `str` (causing the translation to be evaluated), or use the `StrPromise` or `StrOrPromise` types from `django-stubs-ext` in type hints. Which solution to choose depends depends on the particular case. See [working with lazy translation objects](https://docs.djangoproject.com/en/4.1/topics/i18n/translation/#working-with-lazy-translation-objects) in the Django documentation for more information.
 
 If this is reported on Django code, please report an issue or open a pull request to fix the type hints.
```

### Comparing `django_stubs-5.0.0/django_stubs.egg-info/SOURCES.txt` & `django_stubs-5.0.1/django_stubs.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 django-stubs/contrib/contenttypes/__init__.pyi
 django-stubs/contrib/contenttypes/admin.pyi
 django-stubs/contrib/contenttypes/apps.pyi
 django-stubs/contrib/contenttypes/checks.pyi
 django-stubs/contrib/contenttypes/fields.pyi
 django-stubs/contrib/contenttypes/forms.pyi
 django-stubs/contrib/contenttypes/models.pyi
+django-stubs/contrib/contenttypes/prefetch.pyi
 django-stubs/contrib/contenttypes/views.pyi
 django-stubs/contrib/contenttypes/management/__init__.pyi
 django-stubs/contrib/contenttypes/management/commands/__init__.pyi
 django-stubs/contrib/contenttypes/management/commands/remove_stale_contenttypes.pyi
 django-stubs/contrib/contenttypes/migrations/__init__.pyi
 django-stubs/contrib/flatpages/__init__.pyi
 django-stubs/contrib/flatpages/admin.pyi
@@ -102,15 +103,14 @@
 django-stubs/contrib/gis/geometry.pyi
 django-stubs/contrib/gis/measure.pyi
 django-stubs/contrib/gis/ptr.pyi
 django-stubs/contrib/gis/shortcuts.pyi
 django-stubs/contrib/gis/views.pyi
 django-stubs/contrib/gis/admin/__init__.pyi
 django-stubs/contrib/gis/admin/options.pyi
-django-stubs/contrib/gis/admin/widgets.pyi
 django-stubs/contrib/gis/db/__init__.pyi
 django-stubs/contrib/gis/db/backends/__init__.pyi
 django-stubs/contrib/gis/db/backends/utils.pyi
 django-stubs/contrib/gis/db/backends/base/__init__.pyi
 django-stubs/contrib/gis/db/backends/base/adapter.pyi
 django-stubs/contrib/gis/db/backends/base/features.pyi
 django-stubs/contrib/gis/db/backends/base/models.pyi
@@ -227,14 +227,15 @@
 django-stubs/contrib/humanize/templatetags/humanize.pyi
 django-stubs/contrib/messages/__init__.pyi
 django-stubs/contrib/messages/api.pyi
 django-stubs/contrib/messages/apps.pyi
 django-stubs/contrib/messages/constants.pyi
 django-stubs/contrib/messages/context_processors.pyi
 django-stubs/contrib/messages/middleware.pyi
+django-stubs/contrib/messages/test.pyi
 django-stubs/contrib/messages/utils.pyi
 django-stubs/contrib/messages/views.pyi
 django-stubs/contrib/messages/storage/__init__.pyi
 django-stubs/contrib/messages/storage/base.pyi
 django-stubs/contrib/messages/storage/cookie.pyi
 django-stubs/contrib/messages/storage/fallback.pyi
 django-stubs/contrib/messages/storage/session.pyi
```

### Comparing `django_stubs-5.0.0/mypy_django_plugin/config.py` & `django_stubs-5.0.1/mypy_django_plugin/config.py`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/mypy_django_plugin/django/context.py` & `django_stubs-5.0.1/mypy_django_plugin/django/context.py`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/mypy_django_plugin/lib/fullnames.py` & `django_stubs-5.0.1/mypy_django_plugin/lib/fullnames.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 FOREIGN_OBJECT_FULLNAME = "django.db.models.fields.related.ForeignObject"
 FOREIGN_KEY_FULLNAME = "django.db.models.fields.related.ForeignKey"
 ONETOONE_FIELD_FULLNAME = "django.db.models.fields.related.OneToOneField"
 MANYTOMANY_FIELD_FULLNAME = "django.db.models.fields.related.ManyToManyField"
 DUMMY_SETTINGS_BASE_CLASS = "django.conf._DjangoConfLazyObject"
 AUTH_USER_MODEL_FULLNAME = "django.conf.settings.AUTH_USER_MODEL"
 
-QUERYSET_CLASS_FULLNAME = "django.db.models.query._QuerySet"
+QUERYSET_CLASS_FULLNAME = "django.db.models.query.QuerySet"
 BASE_MANAGER_CLASS_FULLNAME = "django.db.models.manager.BaseManager"
 MANAGER_CLASS_FULLNAME = "django.db.models.manager.Manager"
 RELATED_MANAGER_CLASS = "django.db.models.fields.related_descriptors.RelatedManager"
 
 WITH_ANNOTATIONS_FULLNAME = "django_stubs_ext.WithAnnotations"
 ANNOTATIONS_FULLNAME = "django_stubs_ext.annotations.Annotations"
```

### Comparing `django_stubs-5.0.0/mypy_django_plugin/lib/helpers.py` & `django_stubs-5.0.1/mypy_django_plugin/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/mypy_django_plugin/main.py` & `django_stubs-5.0.1/mypy_django_plugin/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import itertools
 import sys
 from functools import partial
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type
 
-from mypy.build import PRI_MYPY
+from mypy.build import PRI_MED, PRI_MYPY
 from mypy.modulefinder import mypy_path
 from mypy.nodes import MypyFile, TypeInfo
 from mypy.options import Options
 from mypy.plugin import (
     AnalyzeTypeContext,
     AttributeContext,
     ClassDefContext,
@@ -95,22 +95,22 @@
 
     def _get_typeinfo_or_none(self, class_name: str) -> Optional[TypeInfo]:
         sym = self.lookup_fully_qualified(class_name)
         if sym is not None and isinstance(sym.node, TypeInfo):
             return sym.node
         return None
 
-    def _new_dependency(self, module: str) -> Tuple[int, str, int]:
+    def _new_dependency(self, module: str, priority: int = PRI_MYPY) -> Tuple[int, str, int]:
         fake_lineno = -1
-        return (PRI_MYPY, module, fake_lineno)
+        return (priority, module, fake_lineno)
 
     def get_additional_deps(self, file: MypyFile) -> List[Tuple[int, str, int]]:
         # for settings
         if file.fullname == "django.conf" and self.django_context.django_settings_module:
-            return [self._new_dependency(self.django_context.django_settings_module)]
+            return [self._new_dependency(self.django_context.django_settings_module, PRI_MED)]
 
         # for values / values_list
         if file.fullname == "django.db.models":
             return [self._new_dependency("typing"), self._new_dependency("django_stubs_ext")]
 
         # for `get_user_model()`
         if self.django_context.settings:
```

### Comparing `django_stubs-5.0.0/mypy_django_plugin/transformers/fields.py` & `django_stubs-5.0.1/mypy_django_plugin/transformers/fields.py`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/mypy_django_plugin/transformers/forms.py` & `django_stubs-5.0.1/mypy_django_plugin/transformers/forms.py`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/mypy_django_plugin/transformers/functional.py` & `django_stubs-5.0.1/mypy_django_plugin/transformers/functional.py`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/mypy_django_plugin/transformers/init_create.py` & `django_stubs-5.0.1/mypy_django_plugin/transformers/init_create.py`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/mypy_django_plugin/transformers/managers.py` & `django_stubs-5.0.1/mypy_django_plugin/transformers/managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         if (
             typed_var
             and isinstance(typed_var[0], Instance)
             and typed_var[0].type.has_base(fullnames.MODEL_CLASS_FULLNAME)
         ):
             ret_type = _replace_type_var(ret_type, base_that_has_method.defn.type_vars[0].fullname, typed_var[0])
             args_types = [
-                _replace_type_var(arg_type, base_that_has_method.defn.type_vars[0].fullname, manager_instance.args[0])
+                _replace_type_var(arg_type, base_that_has_method.defn.type_vars[0].fullname, typed_var[0])
                 for arg_type in args_types
             ]
     if base_that_has_method.self_type:
         # Manages -> Self returns
         ret_type = _replace_type_var(ret_type, base_that_has_method.self_type.fullname, queryset_instance)
 
     # Drop any 'self' argument as our manager is already initialized
@@ -212,15 +212,15 @@
             return False
         type_var = unic_args[0]
     if not type_var:
         # No type var found in the bases.
         return False
 
     if type_info.has_base(fullnames.QUERYSET_CLASS_FULLNAME):
-        # If it is a subclass of _QuerySet, it is compatible.
+        # If it is a subclass of QuerySet, it is compatible.
         return True
     # check that at least one base is a subclass of queryset with Generic type vars
     return any(_has_compatible_type_vars(sub_base.type) for sub_base in type_info.bases)
 
 
 def _replace_type_var(ret_type: MypyType, to_replace: str, replace_by: MypyType) -> MypyType:
     """
```

### Comparing `django_stubs-5.0.0/mypy_django_plugin/transformers/manytomany.py` & `django_stubs-5.0.1/mypy_django_plugin/transformers/manytomany.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import NamedTuple, Optional, Tuple, Union
 
 from mypy.checker import TypeChecker
-from mypy.nodes import AssignmentStmt, Expression, MemberExpr, NameExpr, StrExpr, TypeInfo
+from mypy.nodes import AssignmentStmt, Expression, MemberExpr, NameExpr, RefExpr, StrExpr, TypeInfo
 from mypy.plugin import FunctionContext, MethodContext
 from mypy.semanal import SemanticAnalyzer
 from mypy.types import Instance, ProperType, TypeVarType, UninhabitedType
 from mypy.types import Type as MypyType
 
 from mypy_django_plugin.django.context import DjangoContext
 from mypy_django_plugin.lib import fullnames, helpers
@@ -125,15 +125,15 @@
     api: Union[TypeChecker, SemanticAnalyzer],
     django_context: DjangoContext,
 ) -> Optional[ProperType]:
     """
     Attempts to resolve an expression to a 'TypeInfo' instance. Any lazy reference
     argument(e.g. "<app_label>.<object_name>") to a Django model is also attempted.
     """
-    if isinstance(expr, NameExpr) and isinstance(expr.node, TypeInfo):
+    if isinstance(expr, RefExpr) and isinstance(expr.node, TypeInfo):
         if helpers.is_model_type(expr.node):
             return Instance(expr.node, [])
 
     lazy_reference = None
     if isinstance(expr, StrExpr):
         lazy_reference = expr.value
     elif (
```

### Comparing `django_stubs-5.0.0/mypy_django_plugin/transformers/meta.py` & `django_stubs-5.0.1/mypy_django_plugin/transformers/meta.py`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/mypy_django_plugin/transformers/models.py` & `django_stubs-5.0.1/mypy_django_plugin/transformers/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     ARG_STAR2,
     MDEF,
     Argument,
     AssignmentStmt,
     CallExpr,
     Context,
     Expression,
+    FakeInfo,
     NameExpr,
     RefExpr,
     Statement,
     StrExpr,
     SymbolTableNode,
     TypeInfo,
     Var,
@@ -636,14 +637,18 @@
         # Produce all statements from current class
         model_bases = deque([self.model_classdef])
         # Do a breadth first search over the current model and its bases, to find all
         # abstract parent models that have not been "interrupted" by any concrete model.
         while model_bases:
             model = model_bases.popleft()
             yield from model.defs.body
+            if isinstance(model.info, FakeInfo):
+                # While loading from cache ClassDef infos are faked and 'FakeInfo' doesn't have
+                # all attributes of a 'TypeInfo' set. See #2184
+                continue
             for base in model.info.bases:
                 # Only produce any additional statements from abstract model bases, as they
                 # simulate regular python inheritance. Avoid concrete models, and any of their
                 # parents, as they're handled differently by Django.
                 if helpers.is_abstract_model(base.type) and base.type.fullname not in processed_models:
                     model_bases.append(base.type.defn)
                     processed_models.add(base.type.fullname)
```

### Comparing `django_stubs-5.0.0/mypy_django_plugin/transformers/orm_lookups.py` & `django_stubs-5.0.1/mypy_django_plugin/transformers/orm_lookups.py`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/mypy_django_plugin/transformers/querysets.py` & `django_stubs-5.0.1/mypy_django_plugin/transformers/querysets.py`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/mypy_django_plugin/transformers/request.py` & `django_stubs-5.0.1/mypy_django_plugin/transformers/request.py`

 * *Files identical despite different names*

### Comparing `django_stubs-5.0.0/mypy_django_plugin/transformers/settings.py` & `django_stubs-5.0.1/mypy_django_plugin/transformers/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,18 +34,16 @@
     settings_module = typechecker_api.modules.get(django_context.django_settings_module)
     global_settings_module = typechecker_api.modules.get("django.conf.global_settings")
     for module in [settings_module, global_settings_module]:
         if module is not None:
             sym = module.names.get(setting_name)
             if sym is not None:
                 if sym.type is None:
-                    ctx.api.fail(
-                        f"Import cycle from Django settings module prevents type inference for {setting_name!r}",
-                        ctx.context,
-                    )
+                    # When analysing a function, mypy will defer analysis to a later pass
+                    typechecker_api.handle_cannot_determine_type(setting_name, ctx.context)
                     return ctx.default_attr_type
                 return sym.type
 
     # Now, we want to check if this setting really exist in runtime.
     # If it does, we just return `Any`, not to raise any false-positives.
     # But, we cannot reconstruct the exact runtime type.
     # See https://github.com/typeddjango/django-stubs/pull/1163
```

### Comparing `django_stubs-5.0.0/pyproject.toml` & `django_stubs-5.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,36 +2,14 @@
 target-version = ['py38']
 line-length = 120
 include = '\.pyi?$'
 
 [tool.codespell]
 ignore-words-list = "aadd,acount,nam,asend"
 
-[tool.pyright]
-include = [
-    "django-stubs",
-    "ext/django_stubs_ext",
-    "mypy_django_plugin",
-    "scripts",
-    "tests",
-]
-exclude = [
-    ".github",
-    ".mypy_cache",
-    "build",
-]
-reportMissingTypeArgument = "warning"
-reportPrivateUsage = "none"
-stubPath = "."
-typeCheckingMode = "strict"
-
-pythonVersion = "3.8"
-pythonPlatform = "All"
-
-
 [tool.ruff]
 # Adds to default excludes: https://ruff.rs/docs/settings/#exclude
 extend-exclude = [
     ".*/",
     "django-source",
     "stubgen",
     "out",
@@ -64,15 +42,15 @@
     "E741",
     "E743",
     "F403", # Use wildcard import
     "F405",
     "F822",
     "F821",
 ]
-"tests/*.py" = ["INP001"]
+"tests/*.py" = ["INP001", "PGH003"]
 "ext/tests/*.py" = ["INP001"]
 "setup.py" = ["INP001"]
 
 [tool.ruff.lint.flake8-tidy-imports.banned-api]
 "_typeshed.Self".msg = "Use typing_extensions.Self (PEP 673) instead."
 
 [tool.ruff.lint.isort]
```

### Comparing `django_stubs-5.0.0/setup.py` & `django_stubs-5.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,27 +22,28 @@
 
 dependencies = [
     "django",
     "asgiref",
     "django-stubs-ext>=5.0.0",
     "tomli; python_version < '3.11'",
     # Types:
-    "typing-extensions",
+    "typing-extensions>=4.11.0",
     "types-PyYAML",
 ]
 
 # Keep compatible-mypy major.minor version pinned to what we use in CI (requirements.txt)
 extras_require = {
     "compatible-mypy": ["mypy~=1.10.0"],
     "redis": ["redis"],
+    "oracle": ["oracledb"],
 }
 
 setup(
     name="django-stubs",
-    version="5.0.0",
+    version="5.0.1",
     description="Mypy stubs for Django",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     license_files=["LICENSE.md"],
     url="https://github.com/typeddjango/django-stubs",
     author="Maksim Kurnikov",
@@ -64,15 +65,14 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Typing :: Typed",
         "Framework :: Django",
-        "Framework :: Django :: 4.1",
         "Framework :: Django :: 4.2",
         "Framework :: Django :: 5.0",
     ],
     project_urls={
         "Funding": "https://github.com/sponsors/typeddjango",
         "Release notes": "https://github.com/typeddjango/django-stubs/releases",
     },
```

### Comparing `django_stubs-5.0.0/tests/test_error_handling.py` & `django_stubs-5.0.1/tests/test_error_handling.py`

 * *Files identical despite different names*

