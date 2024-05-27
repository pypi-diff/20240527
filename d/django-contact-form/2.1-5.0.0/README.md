# Comparing `tmp/django-contact-form-2.1.tar.gz` & `tmp/django_contact_form-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-contact-form-2.1.tar", last modified: Wed Jul  5 06:29:24 2023, max compression
+gzip compressed data, was "django_contact_form-5.0.0.tar", last modified: Mon May 27 01:33:48 2024, max compression
```

## Comparing `django-contact-form-2.1.tar` & `django_contact_form-5.0.0.tar`

### file list

```diff
@@ -1,87 +1,89 @@
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.906338 django-contact-form-2.1/
--rw-r--r--   0 james      (503) staff       (20)      299 2023-07-04 01:51:37.000000 django-contact-form-2.1/.editorconfig
--rw-r--r--   0 james      (503) staff       (20)      107 2023-07-04 01:51:49.000000 django-contact-form-2.1/.flake8
--rw-r--r--   0 james      (503) staff       (20)     1041 2023-07-04 08:19:03.000000 django-contact-form-2.1/.pre-commit-config.yaml
--rw-r--r--   0 james      (503) staff       (20)      295 2023-07-04 01:59:19.000000 django-contact-form-2.1/.readthedocs.yaml
--rw-r--r--   0 james      (503) staff       (20)     1523 2022-05-30 06:56:29.000000 django-contact-form-2.1/LICENSE
--rw-r--r--   0 james      (503) staff       (20)      293 2023-07-04 08:10:13.000000 django-contact-form-2.1/MANIFEST.in
--rw-r--r--   0 james      (503) staff       (20)     1710 2023-07-05 06:29:24.906225 django-contact-form-2.1/PKG-INFO
--rw-r--r--   0 james      (503) staff       (20)      478 2020-12-12 09:41:33.000000 django-contact-form-2.1/README.rst
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.901949 django-contact-form-2.1/docs/
--rw-r--r--   0 james      (503) staff       (20)     5616 2015-12-01 10:34:46.000000 django-contact-form-2.1/docs/Makefile
--rw-r--r--   0 james      (503) staff       (20)     1720 2023-07-05 02:38:57.000000 django-contact-form-2.1/docs/conf.py
--rw-r--r--   0 james      (503) staff       (20)      106 2023-07-04 01:59:07.000000 django-contact-form-2.1/docs/docs_settings.py
--rw-r--r--   0 james      (503) staff       (20)     5794 2023-07-05 00:51:40.000000 django-contact-form-2.1/docs/faq.rst
--rw-r--r--   0 james      (503) staff       (20)      583 2023-07-05 00:25:12.000000 django-contact-form-2.1/docs/forms.rst
--rw-r--r--   0 james      (503) staff       (20)      868 2023-07-05 00:48:50.000000 django-contact-form-2.1/docs/index.rst
--rw-r--r--   0 james      (503) staff       (20)     3482 2023-07-05 00:50:19.000000 django-contact-form-2.1/docs/install.rst
--rw-r--r--   0 james      (503) staff       (20)     5122 2015-12-01 10:34:46.000000 django-contact-form-2.1/docs/make.bat
--rw-r--r--   0 james      (503) staff       (20)     6040 2023-07-05 00:41:36.000000 django-contact-form-2.1/docs/quickstart.rst
--rw-r--r--   0 james      (503) staff       (20)      107 2018-09-09 08:47:05.000000 django-contact-form-2.1/docs/spelling_wordlist.txt
--rw-r--r--   0 james      (503) staff       (20)     2352 2023-07-05 01:59:23.000000 django-contact-form-2.1/docs/upgrade.rst
--rw-r--r--   0 james      (503) staff       (20)      113 2023-07-05 00:36:23.000000 django-contact-form-2.1/docs/views.rst
--rw-r--r--   0 james      (503) staff       (20)    10866 2023-07-04 08:13:40.000000 django-contact-form-2.1/noxfile.py
--rw-r--r--   0 james      (503) staff       (20)     2205 2023-07-04 08:36:59.000000 django-contact-form-2.1/pyproject.toml
--rw-r--r--   0 james      (503) staff       (20)      364 2023-07-04 08:18:23.000000 django-contact-form-2.1/runtests.py
--rw-r--r--   0 james      (503) staff       (20)       38 2023-07-05 06:29:24.906374 django-contact-form-2.1/setup.cfg
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.897444 django-contact-form-2.1/src/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.902478 django-contact-form-2.1/src/django_contact_form/
--rw-r--r--   0 james      (503) staff       (20)       77 2023-07-05 06:24:43.000000 django-contact-form-2.1/src/django_contact_form/__init__.py
--rw-r--r--   0 james      (503) staff       (20)      708 2022-05-31 04:37:32.000000 django-contact-form-2.1/src/django_contact_form/akismet_urls.py
--rw-r--r--   0 james      (503) staff       (20)    12612 2023-07-05 00:25:05.000000 django-contact-form-2.1/src/django_contact_form/forms.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.898504 django-contact-form-2.1/src/django_contact_form/locale/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.897607 django-contact-form-2.1/src/django_contact_form/locale/da/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.903138 django-contact-form-2.1/src/django_contact_form/locale/da/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1019 2020-02-09 10:11:31.000000 django-contact-form-2.1/src/django_contact_form/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.897716 django-contact-form-2.1/src/django_contact_form/locale/de/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.903401 django-contact-form-2.1/src/django_contact_form/locale/de/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      532 2018-09-10 05:35:10.000000 django-contact-form-2.1/src/django_contact_form/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)      895 2019-12-15 18:19:12.000000 django-contact-form-2.1/src/django_contact_form/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.897836 django-contact-form-2.1/src/django_contact_form/locale/en/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.903651 django-contact-form-2.1/src/django_contact_form/locale/en/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      378 2018-09-10 05:35:10.000000 django-contact-form-2.1/src/django_contact_form/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)      796 2018-09-10 05:34:39.000000 django-contact-form-2.1/src/django_contact_form/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.897953 django-contact-form-2.1/src/django_contact_form/locale/es/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.903902 django-contact-form-2.1/src/django_contact_form/locale/es/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      560 2018-09-10 05:35:10.000000 django-contact-form-2.1/src/django_contact_form/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)      891 2018-09-10 05:34:39.000000 django-contact-form-2.1/src/django_contact_form/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.898068 django-contact-form-2.1/src/django_contact_form/locale/eu/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.904158 django-contact-form-2.1/src/django_contact_form/locale/eu/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      564 2018-09-10 05:35:10.000000 django-contact-form-2.1/src/django_contact_form/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)      895 2018-09-10 05:34:39.000000 django-contact-form-2.1/src/django_contact_form/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.898190 django-contact-form-2.1/src/django_contact_form/locale/fr/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.904389 django-contact-form-2.1/src/django_contact_form/locale/fr/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      530 2018-09-10 05:35:10.000000 django-contact-form-2.1/src/django_contact_form/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)      887 2019-12-15 18:19:12.000000 django-contact-form-2.1/src/django_contact_form/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.898307 django-contact-form-2.1/src/django_contact_form/locale/it/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.904501 django-contact-form-2.1/src/django_contact_form/locale/it/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      726 2018-09-18 14:46:02.000000 django-contact-form-2.1/src/django_contact_form/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.898429 django-contact-form-2.1/src/django_contact_form/locale/nl/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.904738 django-contact-form-2.1/src/django_contact_form/locale/nl/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      651 2020-09-21 07:57:57.000000 django-contact-form-2.1/src/django_contact_form/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     1025 2020-09-21 07:57:57.000000 django-contact-form-2.1/src/django_contact_form/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.898557 django-contact-form-2.1/src/django_contact_form/locale/uk/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.904963 django-contact-form-2.1/src/django_contact_form/locale/uk/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      684 2020-02-09 10:11:31.000000 django-contact-form-2.1/src/django_contact_form/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)      934 2020-02-09 10:11:31.000000 django-contact-form-2.1/src/django_contact_form/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0 james      (503) staff       (20)      601 2022-05-31 04:35:57.000000 django-contact-form-2.1/src/django_contact_form/urls.py
--rw-r--r--   0 james      (503) staff       (20)     4212 2023-07-05 00:36:19.000000 django-contact-form-2.1/src/django_contact_form/views.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.903030 django-contact-form-2.1/src/django_contact_form.egg-info/
--rw-r--r--   0 james      (503) staff       (20)     1710 2023-07-05 06:29:24.000000 django-contact-form-2.1/src/django_contact_form.egg-info/PKG-INFO
--rw-r--r--   0 james      (503) staff       (20)     2029 2023-07-05 06:29:24.000000 django-contact-form-2.1/src/django_contact_form.egg-info/SOURCES.txt
--rw-r--r--   0 james      (503) staff       (20)        1 2023-07-05 06:29:24.000000 django-contact-form-2.1/src/django_contact_form.egg-info/dependency_links.txt
--rw-r--r--   0 james      (503) staff       (20)      232 2023-07-05 06:29:24.000000 django-contact-form-2.1/src/django_contact_form.egg-info/requires.txt
--rw-r--r--   0 james      (503) staff       (20)       20 2023-07-05 06:29:24.000000 django-contact-form-2.1/src/django_contact_form.egg-info/top_level.txt
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.905501 django-contact-form-2.1/tests/
--rw-r--r--   0 james      (503) staff       (20)        0 2015-12-01 10:34:46.000000 django-contact-form-2.1/tests/__init__.py
--rw-r--r--   0 james      (503) staff       (20)     1399 2023-07-04 02:16:34.000000 django-contact-form-2.1/tests/settings.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.898749 django-contact-form-2.1/tests/templates/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.906066 django-contact-form-2.1/tests/templates/django_contact_form/
--rw-r--r--   0 james      (503) staff       (20)       11 2015-12-01 10:34:46.000000 django-contact-form-2.1/tests/templates/django_contact_form/contact_form.html
--rw-r--r--   0 james      (503) staff       (20)       10 2015-12-01 10:34:46.000000 django-contact-form-2.1/tests/templates/django_contact_form/contact_form.txt
--rw-r--r--   0 james      (503) staff       (20)       21 2015-12-01 10:34:46.000000 django-contact-form-2.1/tests/templates/django_contact_form/contact_form_sent.html
--rw-r--r--   0 james      (503) staff       (20)       20 2015-12-01 10:34:46.000000 django-contact-form-2.1/tests/templates/django_contact_form/contact_form_subject.txt
--rw-r--r--   0 james      (503) staff       (20)       29 2015-12-01 10:34:46.000000 django-contact-form-2.1/tests/templates/django_contact_form/test_callable_template_name.html
--rw-r--r--   0 james      (503) staff       (20)     7287 2023-07-04 08:15:11.000000 django-contact-form-2.1/tests/test_forms.py
--rw-r--r--   0 james      (503) staff       (20)      823 2022-05-31 04:36:06.000000 django-contact-form-2.1/tests/test_urls.py
--rw-r--r--   0 james      (503) staff       (20)     4576 2023-07-04 08:09:38.000000 django-contact-form-2.1/tests/test_views.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.094209 django_contact_form-5.0.0/
+-rw-r--r--   0 james      (503) staff       (20)      299 2023-07-04 01:51:37.000000 django_contact_form-5.0.0/.editorconfig
+-rw-r--r--   0 james      (503) staff       (20)      107 2023-07-04 01:51:49.000000 django_contact_form-5.0.0/.flake8
+-rw-r--r--   0 james      (503) staff       (20)     1042 2024-05-24 07:42:22.000000 django_contact_form-5.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 james      (503) staff       (20)      295 2023-07-04 01:59:19.000000 django_contact_form-5.0.0/.readthedocs.yaml
+-rw-r--r--   0 james      (503) staff       (20)     1531 2024-05-27 01:04:26.000000 django_contact_form-5.0.0/LICENSE
+-rw-r--r--   0 james      (503) staff       (20)      293 2023-07-04 08:10:13.000000 django_contact_form-5.0.0/MANIFEST.in
+-rw-r--r--   0 james      (503) staff       (20)     3195 2024-05-27 01:33:48.093985 django_contact_form-5.0.0/PKG-INFO
+-rw-r--r--   0 james      (503) staff       (20)     1417 2024-05-27 00:54:40.000000 django_contact_form-5.0.0/README.rst
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.087704 django_contact_form-5.0.0/docs/
+-rw-r--r--   0 james      (503) staff       (20)     5616 2015-12-01 10:34:46.000000 django_contact_form-5.0.0/docs/Makefile
+-rw-r--r--   0 james      (503) staff       (20)     6012 2024-05-25 08:45:00.000000 django_contact_form-5.0.0/docs/changelog.rst
+-rw-r--r--   0 james      (503) staff       (20)     1793 2024-05-25 01:43:29.000000 django_contact_form-5.0.0/docs/conf.py
+-rw-r--r--   0 james      (503) staff       (20)      106 2023-07-04 01:59:07.000000 django_contact_form-5.0.0/docs/docs_settings.py
+-rw-r--r--   0 james      (503) staff       (20)     3765 2024-05-25 08:42:02.000000 django_contact_form-5.0.0/docs/faq.rst
+-rw-r--r--   0 james      (503) staff       (20)      583 2024-05-26 08:01:11.000000 django_contact_form-5.0.0/docs/forms.rst
+-rw-r--r--   0 james      (503) staff       (20)     1349 2024-05-26 07:55:20.000000 django_contact_form-5.0.0/docs/index.rst
+-rw-r--r--   0 james      (503) staff       (20)     3072 2024-05-26 07:56:15.000000 django_contact_form-5.0.0/docs/install.rst
+-rw-r--r--   0 james      (503) staff       (20)     5122 2015-12-01 10:34:46.000000 django_contact_form-5.0.0/docs/make.bat
+-rw-r--r--   0 james      (503) staff       (20)      173 2024-05-25 08:44:42.000000 django_contact_form-5.0.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 james      (503) staff       (20)     6118 2024-05-26 07:58:07.000000 django_contact_form-5.0.0/docs/usage.rst
+-rw-r--r--   0 james      (503) staff       (20)      113 2023-07-05 00:36:23.000000 django_contact_form-5.0.0/docs/views.rst
+-rw-r--r--   0 james      (503) staff       (20)    10859 2024-05-25 08:01:20.000000 django_contact_form-5.0.0/noxfile.py
+-rw-r--r--   0 james      (503) staff       (20)     2136 2024-05-27 01:06:57.000000 django_contact_form-5.0.0/pyproject.toml
+-rw-r--r--   0 james      (503) staff       (20)      405 2024-05-27 01:29:59.000000 django_contact_form-5.0.0/runtests.py
+-rw-r--r--   0 james      (503) staff       (20)       38 2024-05-27 01:33:48.094312 django_contact_form-5.0.0/setup.cfg
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.083339 django_contact_form-5.0.0/src/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.088635 django_contact_form-5.0.0/src/django_contact_form/
+-rw-r--r--   0 james      (503) staff       (20)      120 2024-05-27 01:30:49.000000 django_contact_form-5.0.0/src/django_contact_form/__init__.py
+-rw-r--r--   0 james      (503) staff       (20)     2961 2024-05-27 01:07:46.000000 django_contact_form-5.0.0/src/django_contact_form/_akismet.py
+-rw-r--r--   0 james      (503) staff       (20)      749 2024-05-27 01:13:07.000000 django_contact_form-5.0.0/src/django_contact_form/akismet_urls.py
+-rw-r--r--   0 james      (503) staff       (20)    13274 2024-05-27 01:08:06.000000 django_contact_form-5.0.0/src/django_contact_form/forms.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.084434 django_contact_form-5.0.0/src/django_contact_form/locale/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.083521 django_contact_form-5.0.0/src/django_contact_form/locale/da/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.089426 django_contact_form-5.0.0/src/django_contact_form/locale/da/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1019 2024-05-27 01:12:53.000000 django_contact_form-5.0.0/src/django_contact_form/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.083641 django_contact_form-5.0.0/src/django_contact_form/locale/de/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.089681 django_contact_form-5.0.0/src/django_contact_form/locale/de/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      532 2018-09-10 05:35:10.000000 django_contact_form-5.0.0/src/django_contact_form/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)      895 2024-05-27 01:13:00.000000 django_contact_form-5.0.0/src/django_contact_form/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.083763 django_contact_form-5.0.0/src/django_contact_form/locale/en/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.089955 django_contact_form-5.0.0/src/django_contact_form/locale/en/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      378 2018-09-10 05:35:10.000000 django_contact_form-5.0.0/src/django_contact_form/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)      796 2024-05-27 01:13:01.000000 django_contact_form-5.0.0/src/django_contact_form/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.083884 django_contact_form-5.0.0/src/django_contact_form/locale/es/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.090248 django_contact_form-5.0.0/src/django_contact_form/locale/es/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      560 2018-09-10 05:35:10.000000 django_contact_form-5.0.0/src/django_contact_form/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)      891 2024-05-27 01:13:02.000000 django_contact_form-5.0.0/src/django_contact_form/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.084000 django_contact_form-5.0.0/src/django_contact_form/locale/eu/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.090534 django_contact_form-5.0.0/src/django_contact_form/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      564 2018-09-10 05:35:10.000000 django_contact_form-5.0.0/src/django_contact_form/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)      895 2024-05-27 01:13:03.000000 django_contact_form-5.0.0/src/django_contact_form/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.084121 django_contact_form-5.0.0/src/django_contact_form/locale/fr/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.090820 django_contact_form-5.0.0/src/django_contact_form/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      530 2018-09-10 05:35:10.000000 django_contact_form-5.0.0/src/django_contact_form/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)      887 2024-05-27 01:13:04.000000 django_contact_form-5.0.0/src/django_contact_form/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.084241 django_contact_form-5.0.0/src/django_contact_form/locale/it/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.090953 django_contact_form-5.0.0/src/django_contact_form/locale/it/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      726 2018-09-18 14:46:02.000000 django_contact_form-5.0.0/src/django_contact_form/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.084366 django_contact_form-5.0.0/src/django_contact_form/locale/nl/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.091233 django_contact_form-5.0.0/src/django_contact_form/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      651 2020-09-21 07:57:57.000000 django_contact_form-5.0.0/src/django_contact_form/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     1025 2020-09-21 07:57:57.000000 django_contact_form-5.0.0/src/django_contact_form/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.084482 django_contact_form-5.0.0/src/django_contact_form/locale/uk/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.091510 django_contact_form-5.0.0/src/django_contact_form/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      684 2020-02-09 10:11:31.000000 django_contact_form-5.0.0/src/django_contact_form/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)      934 2020-02-09 10:11:31.000000 django_contact_form-5.0.0/src/django_contact_form/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0 james      (503) staff       (20)      642 2024-05-27 01:08:12.000000 django_contact_form-5.0.0/src/django_contact_form/urls.py
+-rw-r--r--   0 james      (503) staff       (20)     4205 2024-05-27 01:08:24.000000 django_contact_form-5.0.0/src/django_contact_form/views.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.093280 django_contact_form-5.0.0/src/django_contact_form.egg-info/
+-rw-r--r--   0 james      (503) staff       (20)     3195 2024-05-27 01:33:48.000000 django_contact_form-5.0.0/src/django_contact_form.egg-info/PKG-INFO
+-rw-r--r--   0 james      (503) staff       (20)     2096 2024-05-27 01:33:48.000000 django_contact_form-5.0.0/src/django_contact_form.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (503) staff       (20)        1 2024-05-27 01:33:48.000000 django_contact_form-5.0.0/src/django_contact_form.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (503) staff       (20)      224 2024-05-27 01:33:48.000000 django_contact_form-5.0.0/src/django_contact_form.egg-info/requires.txt
+-rw-r--r--   0 james      (503) staff       (20)       20 2024-05-27 01:33:48.000000 django_contact_form-5.0.0/src/django_contact_form.egg-info/top_level.txt
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.092311 django_contact_form-5.0.0/tests/
+-rw-r--r--   0 james      (503) staff       (20)        0 2015-12-01 10:34:46.000000 django_contact_form-5.0.0/tests/__init__.py
+-rw-r--r--   0 james      (503) staff       (20)     1441 2024-05-27 01:13:20.000000 django_contact_form-5.0.0/tests/settings.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.084661 django_contact_form-5.0.0/tests/templates/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2024-05-27 01:33:48.093072 django_contact_form-5.0.0/tests/templates/django_contact_form/
+-rw-r--r--   0 james      (503) staff       (20)       11 2015-12-01 10:34:46.000000 django_contact_form-5.0.0/tests/templates/django_contact_form/contact_form.html
+-rw-r--r--   0 james      (503) staff       (20)       10 2015-12-01 10:34:46.000000 django_contact_form-5.0.0/tests/templates/django_contact_form/contact_form.txt
+-rw-r--r--   0 james      (503) staff       (20)       21 2015-12-01 10:34:46.000000 django_contact_form-5.0.0/tests/templates/django_contact_form/contact_form_sent.html
+-rw-r--r--   0 james      (503) staff       (20)       20 2015-12-01 10:34:46.000000 django_contact_form-5.0.0/tests/templates/django_contact_form/contact_form_subject.txt
+-rw-r--r--   0 james      (503) staff       (20)       29 2015-12-01 10:34:46.000000 django_contact_form-5.0.0/tests/templates/django_contact_form/test_callable_template_name.html
+-rw-r--r--   0 james      (503) staff       (20)     6154 2024-05-27 01:13:30.000000 django_contact_form-5.0.0/tests/test_akismet_integration.py
+-rw-r--r--   0 james      (503) staff       (20)     4923 2024-05-27 01:13:37.000000 django_contact_form-5.0.0/tests/test_forms.py
+-rw-r--r--   0 james      (503) staff       (20)      662 2024-05-27 01:13:44.000000 django_contact_form-5.0.0/tests/test_urls.py
+-rw-r--r--   0 james      (503) staff       (20)     3484 2024-05-27 01:13:50.000000 django_contact_form-5.0.0/tests/test_views.py
```

### Comparing `django-contact-form-2.1/.pre-commit-config.yaml` & `django_contact_form-5.0.0/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.4.0
+  rev: v4.6.0
   hooks:
     - id: check-added-large-files
     - id: check-ast
     - id: check-byte-order-marker
     - id: check-case-conflict
     - id: check-docstring-first
     - id: check-merge-conflict
     - id: check-toml
     - id: check-yaml
     - id: debug-statements
     - id: end-of-file-fixer
     - id: trailing-whitespace
 - repo: https://github.com/psf/black
-  rev: 23.1.0
+  rev: 24.4.2
   hooks:
     - id: black
-      language_version: python3.7
+      language_version: python3.12
       name: black (Python formatter)
 - repo: https://github.com/pycqa/flake8
-  rev: 6.0.0
+  rev: 7.0.0
   hooks:
     - id: flake8
       name: flake8 (Python linter)
 - repo: https://github.com/econchick/interrogate
-  rev: 1.5.0
+  rev: 1.7.0
   hooks:
     - id: interrogate
       name: interrogate (Python docstring enforcer)
       args: [--quiet]
 - repo: https://github.com/pycqa/isort
-  rev: 5.12.0
+  rev: 5.13.2
   hooks:
     - id: isort
       name: isort (Python formatter)
```

### Comparing `django-contact-form-2.1/LICENSE` & `django_contact_form-5.0.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2007-2022, James Bennett
+Copyright (c) James Bennett, and contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
     * Redistributions of source code must retain the above copyright
```

### Comparing `django-contact-form-2.1/docs/Makefile` & `django_contact_form-5.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/docs/conf.py` & `django_contact_form-5.0.0/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Configuration file for the Sphinx documentation builder:
 
 https://www.sphinx-doc.org/
 
 """
+
 import os
 import sys
-
-import django_contact_form
+from importlib.metadata import version as get_version
 
 extensions = [
     "notfound.extension",
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
     "sphinxcontrib_django",
@@ -20,16 +20,16 @@
     "sphinx_inline_tabs",
 ]
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
 project = "django-contact-form"
 copyright = "2007, James Bennett"
-version = django_contact_form.__version__
-release = django_contact_form.__version__
+version = get_version("django-contact-form")
+release = version
 exclude_trees = ["_build"]
 pygments_style = "sphinx"
 htmlhelp_basename = "django-contact-formdoc"
 html_theme = "furo"
 latex_documents = [
     (
         "index",
@@ -37,14 +37,15 @@
         "django-contact-form Documentation",
         "James Bennett",
         "manual",
     )
 ]
 
 intersphinx_mapping = {
+    "akismet": ("https://akismet.readthedocs.io/en/latest", None),
     "django": (
         "https://docs.djangoproject.com/en/stable/",
         "https://docs.djangoproject.com/en/stable/_objects/",
     ),
     "python": ("https://docs.python.org/3", None),
 }
```

### Comparing `django-contact-form-2.1/docs/forms.rst` & `django_contact_form-5.0.0/docs/forms.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 
 The base contact form class
 ---------------------------
 
 .. autoclass:: ContactForm
 
 
-The spam filtering contact form class
+The spam-filtering contact form class
 -------------------------------------
 
 .. autoclass:: AkismetContactForm
```

### Comparing `django-contact-form-2.1/docs/install.rst` & `django_contact_form-5.0.0/docs/install.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 .. _install:
 
 
-Installation and recommended configuration
-==========================================
+Installation guide
+==================
 
-django-contact-form |release| supports Django 3.2, 4.1, and 4.2 on Python 3.8,
-3.9, 3.10, and 3.11 (Django 4.1 and 4.2 only). Note that Django 3.2's support
-for Python 3.10 was added in Django 3.2.9, so you may experience issues with
-Python 3.10 and earlier Django 3.2 versions.
+``django-contact-form`` |release| supports Django 4.2 and 5.0 on Python 3.8
+(Django 4.2 only), 3.9 (Django 4.2 only), 3.10, 3.11, and 3.12.
 
-.. note:: **Django 3.2 and supported Python versions**
+Django 4.2 only added Python 3.12 support in the 4.2.8 release, so for use with
+Python 3.12 it is suggested that you use at least Django 4.2.8 (and always
+recommended to use the latest bugfix release of whichever Django version you
+choose to use).
 
-   Django 3.2 was released before Python 3.10 had come out, and although it now
-   supports Python 3.10, it did not officially do so until the Django 3.2.9
-   release. You may encounter problems if you try to use Django 3.2.8 or
-   earlier with Python 3.10.
 
-   Also, although Django 3.2 continues to officially support Python 3.6 and
-   3.7, django-contact-form |release| does not, because the Python core team's
-   support windows for Python 3.6 and 3.7 have ended.
+Installing ``django-contact-form``
+----------------------------------
 
-
-Installing django-contact-form
-------------------------------
-
-To install django-contact-form, run the following command from a command
+To install ``django-contact-form``, run the following command from a command
 prompt/terminal:
 
 .. tab:: macOS/Linux/other Unix
 
    .. code-block:: shell
 
       python -m pip install django-contact-form
@@ -36,30 +28,31 @@
 .. tab:: Windows
 
    .. code-block:: shell
 
       py -m pip install django-contact-form
 
 If you plan to use the spam-filtering
-:class:`~django_contact_form.forms.AkismetContactForm`, you will also need the
-``akismet`` Python library. You can install this separately, or you can have it
-automatically installed for you alongside django-contact-form, by instead
-running:
+:class:`~django_contact_form.forms.AkismetContactForm`, you will also need `the
+Python akismet client <https://akismet.readthedocs.io/>`_. You can install this
+separately (in which case, be sure to install at least version 24.5.0 of
+``akismet``), or you can have it automatically installed for you alongside
+``django-contact-form``, by running:
 
 .. tab:: macOS/Linux/other Unix
 
    .. code-block:: shell
 
-      python -m pip install django-contact-form[akismet]
+      python -m pip install "django-contact-form[akismet]"
 
 .. tab:: Windows
 
    .. code-block:: shell
 
-      py -m pip install django-contact-form[akismet]
+      py -m pip install "django-contact-form[akismet]"
 
 This will use ``pip``, the standard Python package-installation tool. If you
 are using a supported version of Python, your installation of Python should
 have come with ``pip`` bundled. If ``pip`` does not appear to be present, you
 can try running the following from a command prompt/terminal:
 
 .. tab:: macOS/Linux/other Unix
@@ -74,32 +67,33 @@
 
       py -m ensurepip --upgrade
 
 Instructions are also available for `how to obtain and manually install or
 upgrade pip <https://pip.pypa.io/en/latest/installation/>`_.
 
 If you don't already have a supported version of Django installed, using
-``pip`` to install django-contact-form will also install the latest
+``pip`` to install ``django-contact-form`` will also install the latest
 supported version of Django.
 
 Installing from a source checkout
 ---------------------------------
 
-If you want to work on django-contact-form, you can obtain a source checkout.
+If you want to work on ``django-contact-form``, you can obtain a source
+checkout.
 
 The development repository for django-contact-form is at
 <https://github.com/ubernostrum/django-contact-form>. If you have git
 installed, you can obtain a copy of the repository by typing:
 
 .. code-block:: shell
 
    git clone https://github.com/ubernostrum/django-contact-form.git
 
 From there, you can use git commands to check out the specific revision you
-want, and perform an “editable” install (allowing you to change code as you
+want, and perform an "editable" install (allowing you to change code as you
 work on it) by typing:
 
 .. tab:: macOS/Linux/other Unix
 
    .. code-block:: shell
 
       python -m pip install -e .
@@ -109,10 +103,9 @@
    .. code-block:: shell
 
       py -m pip install -e .
 
 Next steps
 ----------
 
-To get up and running quickly, check out :ref:`the quick start guide
-<quickstart>`. For full documentation, see :ref:`the documentation
-index <index>`.
+To start using ``django-contact-form``, check out :ref:`the usage guide
+<usage>`.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-contact-form-2.1/docs/make.bat` & `django_contact_form-5.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/docs/quickstart.rst` & `django_contact_form-5.0.0/docs/usage.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-.. _quickstart:
+.. _usage:
 
-Quick start guide
-=================
+Usage guide
+===========
 
-First you'll need to have Django and django-contact-form installed; for details
+First you'll need to have Django and ``django-contact-form`` installed. For details
 on that, see :ref:`the installation guide <install>`.
 
 Once that's done, you can start setting up django-contact-form. Add
 ``"django_contact_form"`` to your :setting:`INSTALLED_APPS` setting. Then, you
 can begin configuring.
 
 
 URL configuration
 -----------------
 
-The quickest way to set up the views in django-contact-form is to use the
+The quickest way to set up the views in ``django-contact-form`` is to use the
 provided URLconf, found at ``django_contact_form.urls``. You can include it
-wherever you like in your site's URL configuration; for example, to have it
+wherever you like in your site's URL configuration. For example, to have it
 live at the URL ``/contact/``:
 
 .. code-block:: python
 
     from django.urls import include, path
 
 
     urlpatterns = [
         # ... other URL patterns for your site ...
         path("contact/", include("django_contact_form.urls")),
     ]
 
 If you'll be using a custom form class, you'll need to manually set up your
-URLs so you can tell django-contact-form about your form class. For example:
+URLs so you can tell ``django-contact-form`` about your form class. For example:
 
 
 .. code-block:: python
 
     from django.urls import include, path
     from django.views.generic import TemplateView
 
@@ -57,23 +57,26 @@
             name="django_contact_form_sent"),
     ]
 
 .. important:: **Where to put custom forms and views**
 
    When writing a custom form class (or custom
    :class:`~django_contact_form.views.ContactFormView` subclass), **don't** put
-   your custom code inside django-contact-form. Instead, put your custom code
-   in the appropriate place (a ``forms.py`` or ``views.py`` file) in an
-   application you've written.
+   your custom code inside ``django-contact-form``. Instead, put your custom
+   code in the appropriate place (a ``forms.py`` or ``views.py`` file) in a
+   Django application you've written.
 
 
+.. _default-templates:
+
 Required templates
 ------------------
 
-The two views above will need several templates to be created.
+In the default configuration, ``django-contact-form`` requires the following
+templates to exist:
 
 
 ``django_contact_form/contact_form.html``
 `````````````````````````````````````````
 
 This is used to display the contact form. It has a
 :class:`~django.template.RequestContext` (so any context processors will be
@@ -138,41 +141,41 @@
 
       In order to prevent `header injection attacks
       <https://en.wikipedia.org/wiki/Email_injection>`_, the subject *must* be
       only a single line of text, and Django's email framework will reject any
       attempt to send an email with a multi-line subject. So it's a good idea
       to ensure your ``contact_form_subject.txt`` template only produces a
       single line of output when rendered; as a precaution, however,
-      django-contact-form will, by default, condense the output of this
+      ``django-contact-form`` will, by default, condense the output of this
       template to a single line.
 
 
 Using a spam-filtering contact form
 -----------------------------------
 
 Spam filtering is a common desire for contact forms, due to the large amount of
 spam they can attract. There is a spam-filtering contact form class included in
-django-contact-form: :class:`~django_contact_form.forms.AkismetContactForm`,
-which uses `the Wordpress Akismet spam-detection service
-<https://akismet.com/>`_.
+``django-contact-form``:
+:class:`~django_contact_form.forms.AkismetContactForm`, which uses `the Akismet
+spam-detection service <https://akismet.com/>`_.
 
 To use this form, you will need to do the following things:
 
-1. Install the Python ``akismet`` module to allow django-contact-form to
-   communicate with the Akismet service. You can do this via ``pip install
-   akismet``, or as you install django-contact-form via ``pip install
-   django-contact-form[akismet]``.
+1. Install `the Python akismet client <https://akismet.readthedocs.io/>`_ to
+   allow ``django-contact-form`` to communicate with the Akismet service. You
+   can do this manually (in which case you must install at least version 24.5.0
+   of ``akismet``) or as you install ``django-contact-form`` by telling ``pip``
+   to install ``"django-contact-form[akismet]"``.
 
 2. Obtain an Akismet API key from <https://akismet.com/>, and associate it with
    the URL of your site.
 
-3. Supply the API key and URL for django-contact-form to use. You can either
-   place them in the Django settings :setting:`AKISMET_API_KEY` and
-   :setting:`AKISMET_BLOG_URL`, or in the environment variables
-   ``PYTHON_AKISMET_API_KEY`` and ``PYTHON_AKISMET_BLOG_URL``.
+3. Supply the API key and URL for ``django-contact-form`` to use, by placing
+   them in the environment variables ``PYTHON_AKISMET_API_KEY`` and
+   ``PYTHON_AKISMET_BLOG_URL``.
 
 Then you can replace the suggested URLconf above with the following:
 
 .. code-block:: python
 
     from django.urls import include, path
```

### Comparing `django-contact-form-2.1/noxfile.py` & `django_contact_form-5.0.0/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 suite.
 
 To see available tasks, run ``nox --list``. To run all available tasks -- which requires
 a functioning installation of at least one supported Python version -- run ``nox``. To
 run a single task, use ``nox -s`` with the name of that task.
 
 """
+
 import os
 import pathlib
 import shutil
 import typing
 
 import nox
 
@@ -50,46 +51,43 @@
 # -----------------------------------------------------------------------------------
 
 
 @nox.session(tags=["tests"])
 @nox.parametrize(
     "python,django",
     [
-        # Python/Django testing matrix. Tests Django 3.2, 4.1, 4.2, on Python 3.8
+        # Python/Django testing matrix. Tests Django 4.2, and 5.0, on Python 3.8
         # through 3.11, skipping unsupported combinations.
         (python, django)
-        for python in ["3.8", "3.9", "3.10", "3.11"]
-        for django in ["3.2", "4.1", "4.2"]
-        if (python, django)
-        not in [
-            ("3.11", "3.2"),
-        ]
+        for python in ["3.8", "3.9", "3.10", "3.11", "3.12"]
+        for django in ["4.2", "5.0"]
+        if (python, django) not in [("3.8", "5.0"), ("3.9", "5.0")]
     ],
 )
 def tests_with_coverage(session: nox.Session, django: str) -> None:
     """
     Run the package's unit tests, with coverage report.
 
     """
-    session.install(f"Django~={django}.0", ".[tests]")
+    session.install(f"Django~={django}.0", ".[akismet,tests]")
     python_version = session.run(
         f"{session.bin}/python{session.python}", "--version", silent=True
     ).strip()
     django_version = session.run(
         f"{session.bin}/python{session.python}",
         "-Im",
         "django",
         "--version",
         silent=True,
     ).strip()
     session.log(f"Running tests with {python_version}/Django {django_version}")
     session.run(f"{session.bin}/python{session.python}", "-Im", "coverage", "--version")
     session.run(
         f"{session.bin}/python{session.python}",
-        "-Wonce::DeprecationWarning",
+        "-Wmodule::DeprecationWarning",
         "-Im",
         "coverage",
         "run",
         "--source",
         PACKAGE_NAME,
         "runtests.py",
         env={"DJANGO_SETTINGS_MODULE": "tests.settings"},
@@ -104,15 +102,15 @@
     clean()
 
 
 # Tasks which test the package's documentation.
 # -----------------------------------------------------------------------------------
 
 
-@nox.session(python=["3.11"], tags=["docs"])
+@nox.session(python=["3.12"], tags=["docs"])
 def docs_build(session: nox.Session) -> None:
     """
     Build the package's documentation as HTML.
 
     """
     session.install(".[docs]")
     session.chdir("docs")
@@ -126,15 +124,15 @@
         f"{session.bin}/../tmp/doctrees",
         ".",
         f"{session.bin}/../tmp/html",
     )
     clean()
 
 
-@nox.session(python=["3.11"], tags=["docs"])
+@nox.session(python=["3.12"], tags=["docs"])
 def docs_docstrings(session: nox.Session) -> None:
     """
     Enforce the presence of docstrings on all modules, classes, functions, and
     methods.
 
     """
     session.install("interrogate")
@@ -149,15 +147,15 @@
         "src/",
         "tests/",
         "noxfile.py",
     )
     clean()
 
 
-@nox.session(python=["3.11"], tags=["docs"])
+@nox.session(python=["3.12"], tags=["docs"])
 def docs_spellcheck(session: nox.Session) -> None:
     """
     Spell-check the package's documentation.
 
     """
     session.install("pyenchant", "sphinxcontrib-spelling", ".[docs]")
     build_dir = session.create_tmp()
@@ -184,15 +182,15 @@
 # Code formatting checks.
 #
 # These checks do *not* reformat code -- that happens in pre-commit hooks -- but will
 # fail a CI build if they find any code that needs reformatting.
 # -----------------------------------------------------------------------------------
 
 
-@nox.session(python=["3.11"], tags=["formatters"])
+@nox.session(python=["3.12"], tags=["formatters"])
 def format_black(session: nox.Session) -> None:
     """
     Check code formatting with Black.
 
     """
     session.install("black")
     session.run(f"{session.bin}/python{session.python}", "-Im", "black", "--version")
@@ -206,15 +204,15 @@
         "tests/",
         "docs/",
         "noxfile.py",
     )
     clean()
 
 
-@nox.session(python=["3.11"], tags=["formatters"])
+@nox.session(python=["3.12"], tags=["formatters"])
 def format_isort(session: nox.Session) -> None:
     """
     Check code formating with Black.
 
     """
     session.install("isort")
     session.run(f"{session.bin}/python{session.python}", "-Im", "isort", "--version")
@@ -232,15 +230,15 @@
     clean()
 
 
 # Linters.
 # -----------------------------------------------------------------------------------
 
 
-@nox.session(python=["3.11"], tags=["linters", "security"])
+@nox.session(python=["3.12"], tags=["linters", "security"])
 def lint_bandit(session: nox.Session) -> None:
     """
     Lint code with the Bandit security analyzer.
 
     """
     session.install("bandit[toml]")
     session.run(f"{session.bin}/python{session.python}", "-Im", "bandit", "--version")
@@ -253,15 +251,15 @@
         "-r",
         "src/",
         "tests/",
     )
     clean()
 
 
-@nox.session(python=["3.11"], tags=["linters"])
+@nox.session(python=["3.12"], tags=["linters"])
 def lint_flake8(session: nox.Session) -> None:
     """
     Lint code with flake8.
 
     """
     session.install("flake8", "flake8-bugbear")
     session.run(f"{session.bin}/python{session.python}", "-Im", "flake8", "--version")
@@ -273,45 +271,45 @@
         "tests/",
         "docs/",
         "noxfile.py",
     )
     clean()
 
 
-@nox.session(python=["3.11"], tags=["linters"])
+@nox.session(python=["3.12"], tags=["linters"])
 def lint_pylint(session: nox.Session) -> None:
     """
     Lint code with Pyling.
 
     """
     # Pylint requires that all dependencies be importable during the run, so unlike
     # other lint tasks we just install the package.
-    session.install(".", "akismet")
+    session.install(".[akismet]")
     session.install("pylint", "pylint-django")
     session.run(f"python{session.python}", "-Im", "pylint", "--version")
     session.run(f"python{session.python}", "-Im", "pylint", "src/", "tests/")
 
 
 # Packaging checks.
 # -----------------------------------------------------------------------------------
 
 
-@nox.session(python=["3.11"], tags=["packaging"])
+@nox.session(python=["3.12"], tags=["packaging"])
 def package_build(session: nox.Session) -> None:
     """
     Check that the package builds.
 
     """
     clean()
     session.install("build")
     session.run(f"{session.bin}/python{session.python}", "-Im", "build", "--version")
     session.run(f"{session.bin}/python{session.python}", "-Im", "build")
 
 
-@nox.session(python=["3.11"], tags=["packaging"])
+@nox.session(python=["3.12"], tags=["packaging"])
 def package_description(session: nox.Session) -> None:
     """
     Check that the package description will render on the Python Package Index.
 
     """
     package_dir = session.create_tmp()
     session.install("build", "twine")
@@ -331,15 +329,15 @@
         "twine",
         "check",
         f"{package_dir}/build/*",
     )
     clean()
 
 
-@nox.session(python=["3.11"], tags=["packaging"])
+@nox.session(python=["3.12"], tags=["packaging"])
 def package_manifest(session: nox.Session) -> None:
     """
     Check that the set of files in the package matches the set under version control.
 
     """
     session.install("check-manifest")
     session.run(
@@ -347,15 +345,15 @@
     )
     session.run(
         f"{session.bin}/python{session.python}", "-Im", "check_manifest", "--verbose"
     )
     clean()
 
 
-@nox.session(python=["3.11"], tags=["packaging"])
+@nox.session(python=["3.12"], tags=["packaging"])
 def package_pyroma(session: nox.Session) -> None:
     """
     Check package quality with pyroma.
 
     """
     session.install("pyroma")
     session.run(
@@ -363,15 +361,15 @@
         "-c",
         'from importlib.metadata import version; print(version("pyroma"))',
     )
     session.run(f"{session.bin}/python{session.python}", "-Im", "pyroma", ".")
     clean()
 
 
-@nox.session(python=["3.11"], tags=["packaging"])
+@nox.session(python=["3.12"], tags=["packaging"])
 def package_wheel(session: nox.Session) -> None:
     """
     Check the built wheel package for common errors.
 
     """
     package_dir = session.create_tmp()
     session.install("build", "check-wheel-contents")
```

### Comparing `django-contact-form-2.1/pyproject.toml` & `django_contact_form-5.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,80 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 authors = [
-  {name = "James Bennett", email = "james@b-list.org"}
+  {name = "James Bennett"}
+]
+maintainers = [
+  {name = "James Bennett"}
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Web Environment",
   "Framework :: Django",
-  "Framework :: Django :: 3.2",
-  "Framework :: Django :: 4.1",
   "Framework :: Django :: 4.2",
+  "Framework :: Django :: 5.0",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Utilities",
 ]
 name = "django-contact-form"
-description = "A generic contact-form application for Django"
+description = "A generic contact-form application for Django."
 dependencies = [
-  "Django>=3.2,!=4.0.*",
+  "Django>=4.2",
 ]
 dynamic = ["version"]
 keywords = ["django", "email", "contact-form"]
 license = {text = "BSD-3-Clause"}
 readme = "README.rst"
 requires-python = ">=3.8"
 
 [project.urls]
 documentation = "https://django-contact-form.readthedocs.io/"
 homepage = "https://github.com/ubernostrum/django-contact-form"
 
 [project.optional-dependencies]
 akismet = [
-  "akismet",
+  "akismet>=24.5.0",
 ]
 docs = [
   "furo",
   "sphinx",
   "sphinx-copybutton",
   "sphinx-inline-tabs",
   "sphinx-notfound-page",
   "sphinxcontrib-django",
   "sphinxext-opengraph",
 ]
 tests = [
-  "akismet",
   "coverage",
   "tomli; python_full_version < '3.11.0a7'",
 ]
 
 [tool.bandit]
 skips = ["B101"]
 
 [tool.black]
-target-version = ["py38"]
+target-version = ["py38", "py39", "py310", "py311", "py312"]
 
 [tool.check-manifest]
 ignore-bad-ideas = ["*.mo"]
 
-[tool.check-wheel-contents]
-ignore = ["W004"]
+#[tool.check-wheel-contents]
+#ignore = ["W004"]
 
 [tool.coverage.report]
 exclude_lines = [
   "pragma: no cover",
   "def __str__",
   "raise NotImplementedError",
 ]
@@ -84,17 +86,11 @@
 ignore-init-module = true
 ignore-magic = true
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint]
-disable = [
-  "duplicate-code",
-  "logging-fstring-interpolation",
-  "missing-class-docstring",
-  "missing-module-docstring",
-  "too-many-ancestors",
-]
+disable = ["duplicate-code"]
 
 [tool.setuptools.dynamic]
 version = {attr = "django_contact_form.__version__"}
```

### Comparing `django-contact-form-2.1/src/django_contact_form/akismet_urls.py` & `django_contact_form-5.0.0/src/django_contact_form/akismet_urls.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 If all you want is the basic contact-form plus spam filtering,
 include this URLConf somewhere in your URL hierarchy (for example, at
 ``/contact/``).
 
 """
 
+# SPDX-License-Identifier: BSD-3-Clause
+
 from django.urls import path
 from django.views.generic import TemplateView
 
 from .forms import AkismetContactForm
 from .views import ContactFormView
 
 urlpatterns = [
```

### Comparing `django-contact-form-2.1/src/django_contact_form/forms.py` & `django_contact_form-5.0.0/src/django_contact_form/forms.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
-A base contact form for allowing users to send email messages through
-a web interface.
+A base contact form for allowing users to send email messages through a web
+interface.
 
 """
 
+# SPDX-License-Identifier: BSD-3-Clause
+
 from django import forms
 from django.conf import settings
 from django.contrib.sites.shortcuts import get_current_site
 from django.core.mail import send_mail
 from django.template import loader
 from django.utils.translation import gettext_lazy as _
 
@@ -93,17 +95,17 @@
     doing so may interfere with functionality, may not accomplish what you want, and
     generally any desired customization can be accomplished in a more straightforward
     way through overriding one of the attributes/methods listed above.
 
     .. attribute:: request
 
        The :class:`~django.http.HttpRequest` object representing the current
-       request. This is set automatically in `__init__()`, and is used both to generate
-       a :class:`~django.template.RequestContext` for the templates and to allow
-       subclasses to engage in request-specific behavior.
+       request. This is set automatically in ``__init__()``, and is used both to
+       generate a :class:`~django.template.RequestContext` for the templates and to
+       allow subclasses to engage in request-specific behavior.
 
     .. automethod:: save
 
     Note that subclasses which override ``__init__`` or :meth:`save` need to accept
     ``*args`` and ``**kwargs``, and pass them via :func:`super`, in order to preserve
     behavior (each of those methods accepts at least one additional argument, and this
     application expects and requires them to do so).
@@ -126,34 +128,32 @@
         self, *args, data=None, files=None, request=None, recipient_list=None, **kwargs
     ):
         if request is None:
             raise TypeError("Keyword argument 'request' must be supplied")
         self.request = request
         if recipient_list is not None:
             self.recipient_list = recipient_list
-        super().__init__(data=data, files=files, *args, **kwargs)
+        super().__init__(data=data, files=files, *args, **kwargs)  # noqa: B026
 
-    def message(self):
+    def message(self) -> str:
         """
         Return the body of the message to send. By default, this is accomplished by
         rendering the template name specified in :attr:`template_name`.
 
-        :rtype: str
-
         """
         template_name = (
             self.template_name()  # pylint: disable=not-callable
             if callable(self.template_name)
             else self.template_name
         )
         return loader.render_to_string(
             template_name, self.get_message_context(), request=self.request
         )
 
-    def subject(self):
+    def subject(self) -> str:
         """
         Return the subject line of the message to send. By default, this is
         accomplished by rendering the template name specified in
         :attr:`subject_template_name`.
 
         .. warning:: **Subject must be a single line**
 
@@ -162,70 +162,58 @@
            can cause it to be interpreted as multiple headers; this is the `header
            injection attack <https://en.wikipedia.org/wiki/Email_injection>`_. To
            prevent this, :meth:`subject` will always force the subject to a single line
            of text, stripping all newline characters. If you override :meth:`subject`,
            be sure to either do this manually, or use :class:`super` to call the parent
            implementation.
 
-        :rtype: str
-
         """
         template_name = (
             self.subject_template_name()  # pylint: disable=not-callable
             if callable(self.subject_template_name)
             else self.subject_template_name
         )
         subject = loader.render_to_string(
             template_name, self.get_message_context(), request=self.request
         )
         return "".join(subject.splitlines())
 
-    def get_message_context(self):
+    def get_message_context(self) -> dict:
         """
         Return the context used to render the templates for the email
         subject and body.
 
-        .. warning:: **Renamed method**
-
-           Prior to django-contact-form 2.x, this method was named ``get_context()``. It
-           was renamed to ``get_message_context()`` in django-contact-form 2.0. See
-           :ref:`the upgrade guide <renamed-get-context>` for details.
-
         The default context will be a :class:`~django.template.RequestContext` (using
         the current HTTP request, so user information is available), plus the contents
         of the form's :attr:`~django.forms.Form.cleaned_data` dictionary, and one
         additional variable:
 
         ``site``
-          If `django.contrib.sites` is installed, the currently-active
+          If ``django.contrib.sites`` is installed, the currently-active
           :class:`~django.contrib.sites.models.Site` object. Otherwise, a
           :class:`~django.contrib.sites.requests.RequestSite` object generated from the
           request.
 
-        :rtype: dict
-
         """
         if not self.is_valid():
             raise ValueError("Cannot generate Context from invalid contact form")
         return dict(self.cleaned_data, site=get_current_site(self.request))
 
-    def get_message_dict(self):
+    def get_message_dict(self) -> dict:
         """
         Generate the parts of the message and return them in a dictionary suitable
         for passing as keyword arguments to Django's
         :func:`~django.core.mail.send_mail`.
 
-        By default, method will collect and return :attr:`from_email`,
+        By default, this method will collect and return :attr:`from_email`,
         :attr:`recipient_list`, :meth:`message` and :meth:`subject`. Overriding this
         allows essentially unlimited customization of how the message is generated. Note
         that for compatibility, implementations which override this should support
         callables for the values of :attr:`from_email` and :attr:`recipient_list`.
 
-        :rtype: dict
-
         """
         if not self.is_valid():
             raise ValueError("Message cannot be sent from invalid contact form")
         message_dict = {}
         for message_part in ("from_email", "message", "recipient_list", "subject"):
             attr = getattr(self, message_part)
             message_dict[message_part] = attr() if callable(attr) else attr
@@ -241,59 +229,86 @@
 
         """
         send_mail(fail_silently=fail_silently, **self.get_message_dict())
 
 
 class AkismetContactForm(ContactForm):
     """
-    A subclass of :class:`ContactForm` which adds spam filtering, via `the Wordpress
-    Akismet spam-detection service <https://akismet.com/>`_.
+    A subclass of :class:`ContactForm` which adds spam filtering, via `the Akismet
+    spam-detection service <https://akismet.com/>`_.
 
-    Use of this class requires you to provide configuration for the Akismet web service;
-    you'll need to obtain an Akismet API key, and you'll need to associate it with the
+    Use of this class requires you to provide configuration for the Akismet web service.
+    You'll need to obtain an Akismet API key, and you'll need to associate it with the
     site you'll use the contact form on. You can do this at <https://akismet.com/>. Once
-    you have, you can configure in either of two ways:
-
-    1. Put your Akismet API key in the Django setting :setting:`AKISMET_API_KEY`, and
-       the URL it's associated with in the setting :setting:`AKISMET_BLOG_URL`, or
-
-    2. Put your Akismet API key in the environment variable ``PYTHON_AKISMET_API_KEY``,
-       and the URL it's associated with in the environment variable
-       ``PYTHON_AKISMET_BLOG_URL``.
+    you have, put your Akismet API key in the environment variable
+    ``PYTHON_AKISMET_API_KEY``, and the URL it's associated with in the environment
+    variable ``PYTHON_AKISMET_BLOG_URL``.
 
     You will also need `the Python Akismet module <http://akismet.readthedocs.io/>`_ to
-    communicate with the Akismet web service. You can install it by running ``pip
-    install akismet``, or django-contact-form can install it automatically for you if
-    you run ``pip install django-contact-form[akismet]``.
+    communicate with the Akismet web service. You can install it manually (if you do,
+    install at least version 24.5.0), or ``django-contact-form`` can install it
+    automatically for you if you tell ``pip`` to install
+    ``"django-contact-form[akismet]"``.
 
     Once you have an Akismet API key and URL configured, and the ``akismet`` module
     installed, you can drop in :class:`AkismetContactForm` anywhere you would have used
-    :class:`ContactForm`. A URLconf is provided in django-contact-form, at
-    ``django_contact_form.akismet_urls``, which will correctly configure
-    :class:`AkismetContactForm` for you.
+    :class:`ContactForm`. A URLconf is also provided in django-contact-form, at
+    ``django_contact_form.akismet_urls``, which will set up :class:`AkismetContactForm`
+    for you in place of the base contact form class.
+
+    If you want to customize the spam-filtering behavior, there are two methods you can
+    override:
+
+    .. automethod:: get_akismet_check_arguments
+    .. automethod:: get_akismet_client
 
     """
 
     SPAM_MESSAGE = _("Your message was classified as spam.")
 
-    def clean_body(self):
+    def get_akismet_check_arguments(self) -> dict:
         """
-        Apply Akismet spam filtering to the submission.
+        Return the arguments which will be passed to the Akismet spam check.
 
-        """
-        from akismet import Akismet  # pylint: disable=import-outside-toplevel
+        If your form contains additional fields which need to have their contents passed
+        to Akismet, override this to ensure those arguments are correctly set.
 
-        akismet_api = Akismet(
-            key=getattr(settings, "AKISMET_API_KEY", None),
-            blog_url=getattr(settings, "AKISMET_BLOG_URL", None),
-        )
-        akismet_kwargs = {
+        """
+        return {
             "user_ip": self.request.META["REMOTE_ADDR"],
             "user_agent": self.request.META.get("HTTP_USER_AGENT"),
             "comment_author": self.cleaned_data.get("name"),
             "comment_author_email": self.cleaned_data.get("email"),
             "comment_content": self.cleaned_data["body"],
             "comment_type": "contact-form",
         }
-        if akismet_api.comment_check(**akismet_kwargs):
+
+    def get_akismet_client(self) -> "akismet.SyncClient":  # noqa: F821
+        """
+        Obtain and return an Akismet API client.
+
+        By default, this will create a single API client instance and keep it resident
+        in memory for the life of the Python process.
+
+        If you need to customize the Akismet client creation (for example, to pass
+        custom arguments to the Akismet API client), override this method.
+
+        *Note:* Only synchronous Akismet clients (:class:`akismet.SyncClient`) are
+        supported here; async clients (:class:`akismet.AsyncClient`) are not.
+
+        """
+        from ._akismet import (  # pylint: disable=import-outside-toplevel
+            _try_get_akismet_client,
+        )
+
+        return _try_get_akismet_client()
+
+    def clean_body(self):
+        """
+        Apply Akismet spam filtering to the submission.
+
+        """
+        akismet_client = self.get_akismet_client()
+
+        if akismet_client.comment_check(**self.get_akismet_check_arguments()):
             raise forms.ValidationError(self.SPAM_MESSAGE)
         return self.cleaned_data["body"]
```

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/da/LC_MESSAGES/django.po` & `django_contact_form-5.0.0/src/django_contact_form/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/de/LC_MESSAGES/django.mo` & `django_contact_form-5.0.0/src/django_contact_form/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/de/LC_MESSAGES/django.po` & `django_contact_form-5.0.0/src/django_contact_form/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/en/LC_MESSAGES/django.po` & `django_contact_form-5.0.0/src/django_contact_form/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/es/LC_MESSAGES/django.mo` & `django_contact_form-5.0.0/src/django_contact_form/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/es/LC_MESSAGES/django.po` & `django_contact_form-5.0.0/src/django_contact_form/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/eu/LC_MESSAGES/django.mo` & `django_contact_form-5.0.0/src/django_contact_form/locale/eu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/eu/LC_MESSAGES/django.po` & `django_contact_form-5.0.0/src/django_contact_form/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/fr/LC_MESSAGES/django.mo` & `django_contact_form-5.0.0/src/django_contact_form/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/fr/LC_MESSAGES/django.po` & `django_contact_form-5.0.0/src/django_contact_form/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/it/LC_MESSAGES/django.po` & `django_contact_form-5.0.0/src/django_contact_form/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/nl/LC_MESSAGES/django.mo` & `django_contact_form-5.0.0/src/django_contact_form/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/nl/LC_MESSAGES/django.po` & `django_contact_form-5.0.0/src/django_contact_form/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/uk/LC_MESSAGES/django.mo` & `django_contact_form-5.0.0/src/django_contact_form/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/locale/uk/LC_MESSAGES/django.po` & `django_contact_form-5.0.0/src/django_contact_form/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.1/src/django_contact_form/urls.py` & `django_contact_form-5.0.0/src/django_contact_form/urls.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 If all you want is the basic ContactForm with default behavior,
 include this URLConf somewhere in your URL hierarchy (for example, at
 ``/contact/``)
 
 """
 
+# SPDX-License-Identifier: BSD-3-Clause
+
 from django.urls import path
 from django.views.generic import TemplateView
 
 from django_contact_form.views import ContactFormView
 
 urlpatterns = [
     path("", ContactFormView.as_view(), name="django_contact_form"),
```

### Comparing `django-contact-form-2.1/src/django_contact_form/views.py` & `django_contact_form-5.0.0/src/django_contact_form/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 View which can render and send email from a contact form.
 
 """
 
+# SPDX-License-Identifier: BSD-3-Clause
+
 from django.urls import reverse_lazy
 from django.views.generic.edit import FormView
 
 from .forms import ContactForm
 
 
 class ContactFormView(FormView):
     """
     The base view class from which most custom contact-form views should inherit. If
     you don't need any custom functionality, and are content with the default
     :class:`~django_contact_form.forms.ContactForm` class, you can also use it as-is
-    (and the provided URLConf, `django_contact_form.urls`, does exactly this).
+    (and the provided URLConf, ``django_contact_form.urls``, does exactly this).
 
     This is a subclass of Django's :class:`~django.views.generic.edit.FormView`, so
     refer to the Django documentation for a list of attributes/methods which can be
     overridden to customize behavior.
 
     One non-standard attribute is defined here:
 
@@ -40,46 +42,28 @@
 
        The form class to use. By default, will be
        :class:`~django_contact_form.forms.ContactForm`.
 
     .. attribute:: template_name
 
        A :class:`str`, the template to use when rendering the form. By default, will be
-       `django_contact_form/contact_form.html`.
+       ``django_contact_form/contact_form.html``.
 
     .. attribute:: success_url
 
        The URL to redirect to after successful form submission. Can be a hard-coded
        string, the string resulting from calling Django's :func:`~django.urls.reverse`
        helper, or the lazy object produced by Django's :func:`~django.urls.reverse_lazy`
        helper. Default value is the result of calling :func:`~django.urls.reverse_lazy`
-       with the URL name ``django_contact_form_sent``.
-
-       :rtype: str
-
-    .. method:: get_form_kwargs
-
-       Return additional keyword arguments (as a dictionary) to pass to the form class
-       on initialization.
+       with the URL name ``"django_contact_form_sent"``.
 
-       By default, this will return a dictionary containing the current
-       :class:`~django.http.HttpRequest` (as the key `request`) and, if
-       :attr:`~ContactFormView.recipient_list` was defined, its value (as the key
-       ``recipient_list``).
+    You can also override the following method for full customization of the form
+    instance construction:
 
-       .. warning:: **Request is a required argument**
-
-          If you override :meth:`get_form_kwargs`, you **must** ensure that, at the very
-          least, the keyword argument ``request`` is still provided, or
-          :class:`~django_contact_form.forms.ContactForm` initialization will raise
-          :exc:`TypeError`. The easiest approach is to use :class:`super` to call the
-          base implementation in :class:`ContactFormView`, and modify the dictionary it
-          returns.
-
-       :rtype: dict
+    .. automethod:: get_form_kwargs
 
     """
 
     form_class = ContactForm
     recipient_list = None
     success_url = reverse_lazy("django_contact_form_sent")
     template_name = "django_contact_form/contact_form.html"
@@ -88,18 +72,32 @@
         """
         Handle a valid form by sending the email.
 
         """
         form.save()
         return super().form_valid(form)
 
-    def get_form_kwargs(self):
+    def get_form_kwargs(self) -> dict:
         """
-        Override of base method in order to pass the HTTP request as a form keyword
-        argument, and also the optional recipient_list (if set).
+        Return additional keyword arguments (as a dictionary) to pass to the form class
+        on initialization.
+
+        By default, this will return a dictionary containing the current
+        :class:`~django.http.HttpRequest` (as the key ``request``) and, if
+        :attr:`~ContactFormView.recipient_list` was defined, its value (as the key
+        ``recipient_list``).
+
+        .. warning:: **Request is a required argument**
+
+           If you override :meth:`get_form_kwargs`, you **must** ensure that, at the very
+           least, the keyword argument ``request`` is still provided, or
+           :class:`~django_contact_form.forms.ContactForm` initialization will raise
+           :exc:`TypeError`. The easiest approach is to use :class:`super` to call the
+           base implementation in :class:`ContactFormView`, and modify the dictionary it
+           returns.
 
         """
         # ContactForm instances require instantiation with an
         # HttpRequest.
         kwargs = super().get_form_kwargs()
         kwargs.update({"request": self.request})
```

### Comparing `django-contact-form-2.1/src/django_contact_form.egg-info/SOURCES.txt` & `django_contact_form-5.0.0/src/django_contact_form.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 LICENSE
 MANIFEST.in
 README.rst
 noxfile.py
 pyproject.toml
 runtests.py
 docs/Makefile
+docs/changelog.rst
 docs/conf.py
 docs/docs_settings.py
 docs/faq.rst
 docs/forms.rst
 docs/index.rst
 docs/install.rst
 docs/make.bat
-docs/quickstart.rst
 docs/spelling_wordlist.txt
-docs/upgrade.rst
+docs/usage.rst
 docs/views.rst
 src/django_contact_form/__init__.py
+src/django_contact_form/_akismet.py
 src/django_contact_form/akismet_urls.py
 src/django_contact_form/forms.py
 src/django_contact_form/urls.py
 src/django_contact_form/views.py
 src/django_contact_form.egg-info/PKG-INFO
 src/django_contact_form.egg-info/SOURCES.txt
 src/django_contact_form.egg-info/dependency_links.txt
@@ -44,14 +45,15 @@
 src/django_contact_form/locale/it/LC_MESSAGES/django.po
 src/django_contact_form/locale/nl/LC_MESSAGES/django.mo
 src/django_contact_form/locale/nl/LC_MESSAGES/django.po
 src/django_contact_form/locale/uk/LC_MESSAGES/django.mo
 src/django_contact_form/locale/uk/LC_MESSAGES/django.po
 tests/__init__.py
 tests/settings.py
+tests/test_akismet_integration.py
 tests/test_forms.py
 tests/test_urls.py
 tests/test_views.py
 tests/templates/django_contact_form/contact_form.html
 tests/templates/django_contact_form/contact_form.txt
 tests/templates/django_contact_form/contact_form_sent.html
 tests/templates/django_contact_form/contact_form_subject.txt
```

### Comparing `django-contact-form-2.1/tests/settings.py` & `django_contact_form-5.0.0/tests/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """
 Minimal Django settings file for test runs.
 
 """
+
+# SPDX-License-Identifier: BSD-3-Clause
+
 import pathlib
 
 from django.utils.crypto import get_random_string
 
 APP_DIR = pathlib.Path(__file__).parents[0]
 
 DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
```

### Comparing `django-contact-form-2.1/tests/test_urls.py` & `django_contact_form-5.0.0/tests/test_urls.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 URLConf for testing django-contact-form.
 
 """
 
+# SPDX-License-Identifier: BSD-3-Clause
+
 from django.urls import path
 from django.views.generic import TemplateView
 
-from django_contact_form.forms import AkismetContactForm
 from django_contact_form.views import ContactFormView
 
 urlpatterns = [
     path("", ContactFormView.as_view(), name="django_contact_form"),
     path(
         "sent/",
         TemplateView.as_view(
@@ -19,13 +20,8 @@
         name="django_contact_form_sent",
     ),
     path(
         "test_recipient_list/",
         ContactFormView.as_view(recipient_list=["recipient_list@example.com"]),
         name="test_recipient_list",
     ),
-    path(
-        "test_akismet_form/",
-        ContactFormView.as_view(form_class=AkismetContactForm),
-        name="test_akismet_form",
-    ),
 ]
```

### Comparing `django-contact-form-2.1/tests/test_views.py` & `django_contact_form-5.0.0/tests/test_views.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Tests for the built-in views.
 
 """
 
-import os
-import unittest
-from unittest import mock
+# SPDX-License-Identifier: BSD-3-Clause
 
+from http import HTTPStatus
+
+import django
 from django.conf import settings
 from django.core import mail
 from django.test import RequestFactory, TestCase
 from django.test.utils import override_settings
 from django.urls import reverse
 
-from django_contact_form.forms import ContactForm
+from django_contact_form.forms import AkismetContactForm, ContactForm
 
 
 @override_settings(ROOT_URLCONF="tests.test_urls")
 class ContactFormViewTests(TestCase):
     """
     Tests for the built-in ContactFormView.
 
@@ -27,110 +28,80 @@
         """
         HTTP GET on the form view just shows the form.
 
         """
         contact_url = reverse("django_contact_form")
 
         response = self.client.get(contact_url)
-        self.assertEqual(200, response.status_code)
+        assert HTTPStatus.OK == response.status_code
         self.assertTemplateUsed(response, "django_contact_form/contact_form.html")
 
     def test_send(self):
         """
         Valid data through the view results in a successful send.
 
         """
         contact_url = reverse("django_contact_form")
         data = {"name": "Test", "email": "test@example.com", "body": "Test message"}
 
         response = self.client.post(contact_url, data=data)
 
         self.assertRedirects(response, reverse("django_contact_form_sent"))
 
-        self.assertEqual(1, len(mail.outbox))
+        assert 1 == len(mail.outbox)
 
         message = mail.outbox[0]
-        self.assertTrue(data["body"] in message.body)
-        self.assertEqual(settings.DEFAULT_FROM_EMAIL, message.from_email)
+        assert data["body"] in message.body
+        assert settings.DEFAULT_FROM_EMAIL == message.from_email
+
         form = ContactForm(request=RequestFactory().request)
-        self.assertEqual(form.recipient_list, message.recipients())
+        assert form.recipient_list == message.recipients()
 
     def test_invalid(self):
         """
         Invalid data doesn't work.
 
         """
         contact_url = reverse("django_contact_form")
         data = {"name": "Test", "body": "Test message"}
 
         response = self.client.post(contact_url, data=data)
 
-        self.assertEqual(200, response.status_code)
-        self.assertFormError(response, "form", "email", "This field is required.")
+        assert HTTPStatus.OK == response.status_code
+        # The argument signature of assertFormError() changed beginning in Django 4.1 --
+        # prior to that the first argument was a response object, and after the
+        # deprecation cycle completed in 5.0 the first argument is now the form
+        # instance.
+        if django.get_version() < "4.2":
+            self.assertFormError(response, "form", "email", "This field is required.")
+        else:
+            self.assertFormError(
+                response.context["form"], "email", "This field is required."
+            )
         self.assertEqual(0, len(mail.outbox))
 
     def test_recipient_list(self):
         """
         Passing recipient_list when instantiating ContactFormView
         properly overrides the list of recipients.
 
         """
         contact_url = reverse("test_recipient_list")
         data = {"name": "Test", "email": "test@example.com", "body": "Test message"}
 
         response = self.client.post(contact_url, data=data)
         self.assertRedirects(response, reverse("django_contact_form_sent"))
-        self.assertEqual(1, len(mail.outbox))
+        assert 1 == len(mail.outbox)
 
         message = mail.outbox[0]
-        self.assertEqual(["recipient_list@example.com"], message.recipients())
-
-
-@unittest.skipUnless(
-    getattr(settings, "AKISMET_API_KEY", os.getenv("PYTHON_AKISMET_API_KEY"))
-    is not None,
-    "AkismetContactForm requires Akismet configuration",
-)
-@override_settings(ROOT_URLCONF="django_contact_form.akismet_urls")
-class AkismetContactFormViewTests(TestCase):
-    """
-    Tests the views with the Akismet contact form.
-
-    """
+        assert ["recipient_list@example.com"] == message.recipients()
 
-    def test_akismet_view_spam(self):
+    @override_settings(ROOT_URLCONF="django_contact_form.akismet_urls")
+    def test_akismet_view(self):
         """
-        The Akismet contact form errors on spam.
+        The Akismet contact form URL uses a spam-filtering AkismetContactForm
+        instance.
 
         """
-        contact_url = reverse("django_contact_form")
-        data = {
-            "name": "viagra-test-123",
-            "email": "email@example.com",
-            "body": "This is spam.",
-        }
-        with mock.patch("akismet.Akismet", autospec=True) as akismet_mock:
-            instance = akismet_mock.return_value
-            instance.verify_key.return_value = True
-            instance.comment_check.return_value = True
-            response = self.client.post(contact_url, data=data)
-            self.assertEqual(200, response.status_code)
-            self.assertFalse(response.context["form"].is_valid())
-            self.assertTrue(response.context["form"].has_error("body"))
-
-    def test_akismet_view_ham(self):
-        """
-        The Akismet contact form does not error on non-spam.
-
-        """
-        contact_url = reverse("django_contact_form")
-        data = {"name": "Test", "email": "email@example.com", "body": "Test message."}
-        with mock.patch("akismet.Akismet", autospec=True) as akismet_mock:
-            instance = akismet_mock.return_value
-            instance.verify_key.return_value = True
-            instance.comment_check.return_value = False
-            response = self.client.post(contact_url, data=data)
-            self.assertRedirects(response, reverse("django_contact_form_sent"))
-            self.assertEqual(1, len(mail.outbox))
-
-            message = mail.outbox[0]
-            self.assertEqual(["noreply@example.com"], message.recipients())
+        response = self.client.get(reverse("django_contact_form"))
+        assert response.status_code == HTTPStatus.OK
+        assert isinstance(response.context["form"], AkismetContactForm)
```

