# Comparing `tmp/django-mfa2-2.9.0.tar.gz` & `tmp/django-mfa2-2.9.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mfa2-2.9.0.tar", last modified: Mon May 27 05:53:37 2024, max compression
+gzip compressed data, was "dist/django-mfa2-2.9.0b1.tar", last modified: Thu Apr  4 13:44:54 2024, max compression
```

## Comparing `django-mfa2-2.9.0.tar` & `django-mfa2-2.9.0b1.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.931883 django-mfa2-2.9.0/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1075 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/LICENSE
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       64 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/MANIFEST.in
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)    11996 2024-05-27 05:53:37.931883 django-mfa2-2.9.0/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    10355 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/README.md
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.931883 django-mfa2-2.9.0/django_mfa2.egg-info/
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)    11996 2024-05-27 05:53:37.000000 django-mfa2-2.9.0/django_mfa2.egg-info/PKG-INFO
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)     2168 2024-05-27 05:53:37.000000 django-mfa2-2.9.0/django_mfa2.egg-info/SOURCES.txt
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)        1 2024-05-27 05:53:37.000000 django-mfa2-2.9.0/django_mfa2.egg-info/dependency_links.txt
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)        1 2019-01-18 07:28:18.000000 django-mfa2-2.9.0/django_mfa2.egg-info/not-zip-safe
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)       97 2024-05-27 05:53:37.000000 django-mfa2-2.9.0/django_mfa2.egg-info/requires.txt
--rwxrwxrwx   0 mohamed   (1000) mohamed   (1000)        4 2024-05-27 05:53:37.000000 django-mfa2-2.9.0/django_mfa2.egg-info/top_level.txt
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.927883 django-mfa2-2.9.0/mfa/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2021-11-16 08:30:56.000000 django-mfa2-2.9.0/mfa/ApproveLogin.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      804 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/Common.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3790 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/Email.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     9019 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/FIDO2.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5852 2024-05-27 05:49:21.000000 django-mfa2-2.9.0/mfa/TrustedDevice.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5455 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/U2F.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       22 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       63 2021-11-16 08:30:56.000000 django-mfa2-2.9.0/mfa/admin.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      127 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/apps.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1521 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/helpers.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      680 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/middleware.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.927883 django-mfa2-2.9.0/mfa/migrations/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      796 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/migrations/0001_initial.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      406 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/migrations/0002_user_keys_key_type.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      404 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/migrations/0003_auto_20181114_2159.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      401 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/migrations/0004_user_keys_enabled.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1081 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/migrations/0005_auto_20181115_2014.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1133 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/migrations/0006_trusted_devices.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      501 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/migrations/0007_auto_20181230_1549.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      427 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/migrations/0008_user_keys_last_used.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      756 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/migrations/0009_user_keys_owned_by_enterprise.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      411 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/migrations/0010_auto_20201110_0557.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      420 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/migrations/0011_auto_20210530_0622.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/migrations/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1716 2024-05-27 05:49:21.000000 django-mfa2-2.9.0/mfa/models.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5265 2024-05-27 05:49:21.000000 django-mfa2-2.9.0/mfa/recovery.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.927883 django-mfa2-2.9.0/mfa/static/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.927883 django-mfa2-2.9.0/mfa/static/mfa/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.927883 django-mfa2-2.9.0/mfa/static/mfa/css/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1590 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/static/mfa/css/bootstrap-toggle.min.css
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.931883 django-mfa2-2.9.0/mfa/static/mfa/js/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4129 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/static/mfa/js/bootstrap-toggle.min.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4106 2024-01-23 11:08:45.000000 django-mfa2-2.9.0/mfa/static/mfa/js/bootstrap-toggle.min.js.map
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    12175 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/static/mfa/js/cbor.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    17579 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/static/mfa/js/qrious.min.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)   114187 2024-01-23 11:08:45.000000 django-mfa2-2.9.0/mfa/static/mfa/js/qrious.min.js.map
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    21007 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/static/mfa/js/u2f-api.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    19071 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/static/mfa/js/ua-parser.min.js
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.931883 django-mfa2-2.9.0/mfa/templates/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.931883 django-mfa2-2.9.0/mfa/templates/ApproveLogin/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      123 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/templates/ApproveLogin/Add.html
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.931883 django-mfa2-2.9.0/mfa/templates/Email/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1714 2022-06-22 05:55:49.000000 django-mfa2-2.9.0/mfa/templates/Email/Add.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      235 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/templates/Email/Auth.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      108 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/templates/Email/mfa_email_token_template.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2554 2022-06-22 05:55:49.000000 django-mfa2-2.9.0/mfa/templates/Email/recheck.html
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.931883 django-mfa2-2.9.0/mfa/templates/FIDO2/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3164 2022-11-01 06:09:57.000000 django-mfa2-2.9.0/mfa/templates/FIDO2/Add.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      121 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/templates/FIDO2/Auth.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4726 2022-11-01 06:09:57.000000 django-mfa2-2.9.0/mfa/templates/FIDO2/recheck.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5593 2022-11-01 06:09:57.000000 django-mfa2-2.9.0/mfa/templates/MFA.html
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.931883 django-mfa2-2.9.0/mfa/templates/RECOVERY/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4795 2022-11-01 06:09:57.000000 django-mfa2-2.9.0/mfa/templates/RECOVERY/Add.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      240 2022-11-01 06:09:57.000000 django-mfa2-2.9.0/mfa/templates/RECOVERY/Auth.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3184 2022-11-01 06:09:57.000000 django-mfa2-2.9.0/mfa/templates/RECOVERY/recheck.html
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.931883 django-mfa2-2.9.0/mfa/templates/TOTP/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5300 2022-11-01 06:09:57.000000 django-mfa2-2.9.0/mfa/templates/TOTP/Add.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      236 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/templates/TOTP/Auth.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2581 2022-11-01 06:09:57.000000 django-mfa2-2.9.0/mfa/templates/TOTP/recheck.html
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.931883 django-mfa2-2.9.0/mfa/templates/TrustedDevices/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3961 2022-06-22 05:55:49.000000 django-mfa2-2.9.0/mfa/templates/TrustedDevices/Add.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      735 2022-06-22 05:55:49.000000 django-mfa2-2.9.0/mfa/templates/TrustedDevices/Done.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      278 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/templates/TrustedDevices/email.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4315 2022-12-19 11:23:22.000000 django-mfa2-2.9.0/mfa/templates/TrustedDevices/start.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      306 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/templates/TrustedDevices/user-agent.html
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-05-27 05:53:37.931883 django-mfa2-2.9.0/mfa/templates/U2F/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2690 2022-11-01 06:09:57.000000 django-mfa2-2.9.0/mfa/templates/U2F/Add.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      135 2021-11-16 07:57:44.000000 django-mfa2-2.9.0/mfa/templates/U2F/Auth.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3575 2022-11-01 06:09:57.000000 django-mfa2-2.9.0/mfa/templates/U2F/recheck.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      128 2021-11-16 08:31:00.000000 django-mfa2-2.9.0/mfa/templates/mfa_base.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1034 2022-06-22 05:55:49.000000 django-mfa2-2.9.0/mfa/templates/mfa_check.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      807 2022-06-22 05:55:49.000000 django-mfa2-2.9.0/mfa/templates/modal.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1419 2022-11-01 06:09:57.000000 django-mfa2-2.9.0/mfa/templates/select_mfa_method.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       60 2021-11-16 08:30:56.000000 django-mfa2-2.9.0/mfa/tests.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4338 2024-05-27 05:45:12.000000 django-mfa2-2.9.0/mfa/totp.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2759 2024-05-27 05:52:52.000000 django-mfa2-2.9.0/mfa/urls.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4075 2024-05-27 05:49:21.000000 django-mfa2-2.9.0/mfa/views.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       67 2024-05-27 05:53:37.931883 django-mfa2-2.9.0/setup.cfg
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1952 2024-05-27 05:49:21.000000 django-mfa2-2.9.0/setup.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1075 2019-01-18 07:17:11.000000 django-mfa2-2.9.0b1/LICENSE
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       64 2019-01-18 12:15:28.000000 django-mfa2-2.9.0b1/MANIFEST.in
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    11768 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    10355 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/README.md
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/django_mfa2.egg-info/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)    11768 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/django_mfa2.egg-info/PKG-INFO
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     2210 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/django_mfa2.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/django_mfa2.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2019-01-18 07:28:18.000000 django-mfa2-2.9.0b1/django_mfa2.egg-info/not-zip-safe
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       97 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/django_mfa2.egg-info/requires.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        4 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/django_mfa2.egg-info/top_level.txt
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/ApproveLogin.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      804 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/Common.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3790 2024-04-04 13:37:24.000000 django-mfa2-2.9.0b1/mfa/Email.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     9019 2024-04-04 13:31:55.000000 django-mfa2-2.9.0b1/mfa/FIDO2.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5851 2024-04-04 13:39:27.000000 django-mfa2-2.9.0b1/mfa/TrustedDevice.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5455 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/U2F.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       22 2024-04-04 13:15:05.000000 django-mfa2-2.9.0b1/mfa/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       63 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/admin.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      127 2024-04-04 13:15:05.000000 django-mfa2-2.9.0b1/mfa/apps.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1521 2024-04-04 13:32:57.000000 django-mfa2-2.9.0b1/mfa/helpers.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      680 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/middleware.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/migrations/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      796 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0001_initial.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      406 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0002_user_keys_key_type.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      404 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0003_auto_20181114_2159.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      401 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0004_user_keys_enabled.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1081 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0005_auto_20181115_2014.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1133 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0006_trusted_devices.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      501 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0007_auto_20181230_1549.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      427 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0008_user_keys_last_used.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      756 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0009_user_keys_owned_by_enterprise.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      411 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0010_auto_20201110_0557.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      420 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/migrations/0011_auto_20210530_0622.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      440 2022-09-02 07:52:00.000000 django-mfa2-2.9.0b1/mfa/migrations/0012_alter_user_keys_id.py
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        0 2019-01-18 07:17:42.000000 django-mfa2-2.9.0b1/mfa/migrations/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1717 2024-04-04 13:37:46.000000 django-mfa2-2.9.0b1/mfa/models.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5266 2024-04-04 13:38:22.000000 django-mfa2-2.9.0b1/mfa/recovery.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/static/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/static/mfa/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/static/mfa/css/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1590 2018-05-09 11:30:28.000000 django-mfa2-2.9.0b1/mfa/static/mfa/css/bootstrap-toggle.min.css
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     4129 2018-05-09 11:30:28.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/bootstrap-toggle.min.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4106 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/bootstrap-toggle.min.js.map
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    12175 2023-12-31 18:37:19.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/cbor.js
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)    17579 2019-01-02 14:37:10.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/qrious.min.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)   114187 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/qrious.min.js.map
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)    21007 2019-01-16 17:28:14.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/u2f-api.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    19071 2021-02-26 10:25:56.000000 django-mfa2-2.9.0b1/mfa/static/mfa/js/ua-parser.min.js
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/ApproveLogin/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      123 2019-01-18 07:17:42.000000 django-mfa2-2.9.0b1/mfa/templates/ApproveLogin/Add.html
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/Email/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1714 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/Email/Add.html
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      235 2019-01-21 15:33:45.000000 django-mfa2-2.9.0b1/mfa/templates/Email/Auth.html
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      108 2019-01-21 15:33:45.000000 django-mfa2-2.9.0b1/mfa/templates/Email/mfa_email_token_template.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2554 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/Email/recheck.html
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/FIDO2/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3164 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/FIDO2/Add.html
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      121 2019-06-20 17:36:18.000000 django-mfa2-2.9.0b1/mfa/templates/FIDO2/Auth.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4726 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/FIDO2/recheck.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5593 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/MFA.html
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/RECOVERY/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4795 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/RECOVERY/Add.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      240 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/RECOVERY/Auth.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3184 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/RECOVERY/recheck.html
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/TOTP/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5300 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/TOTP/Add.html
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      236 2019-01-18 12:39:43.000000 django-mfa2-2.9.0b1/mfa/templates/TOTP/Auth.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2581 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/TOTP/recheck.html
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3961 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/Add.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      735 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/Done.html
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      278 2019-01-18 07:17:42.000000 django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/email.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4315 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/start.html
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      306 2019-01-18 07:17:42.000000 django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/user-agent.html
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/mfa/templates/U2F/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2690 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/U2F/Add.html
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      135 2019-01-18 12:40:01.000000 django-mfa2-2.9.0b1/mfa/templates/U2F/Auth.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3575 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/U2F/recheck.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      128 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/mfa_base.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1034 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/mfa_check.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      807 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/modal.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1419 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/templates/select_mfa_method.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       60 2024-04-04 13:15:12.000000 django-mfa2-2.9.0b1/mfa/tests.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4338 2024-04-04 13:34:39.000000 django-mfa2-2.9.0b1/mfa/totp.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2740 2024-04-04 13:41:35.000000 django-mfa2-2.9.0b1/mfa/urls.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4076 2024-04-04 13:36:18.000000 django-mfa2-2.9.0b1/mfa/views.py
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       67 2024-04-04 13:44:54.000000 django-mfa2-2.9.0b1/setup.cfg
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1954 2024-04-04 13:43:31.000000 django-mfa2-2.9.0b1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `django-mfa2-2.9.0/LICENSE` & `django-mfa2-2.9.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/PKG-INFO` & `django-mfa2-2.9.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-mfa2
-Version: 2.9.0
+Version: 2.9.0b1
 Summary: Allows user to add 2FA to their accounts
 Home-page: https://github.com/mkalioby/django-mfa2/
 Download-URL: https://github.com/mkalioby/django-mfa2/
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
@@ -29,22 +29,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django>=2.0
-Requires-Dist: simplejson
-Requires-Dist: pyotp
-Requires-Dist: python-u2flib-server
-Requires-Dist: ua-parser
-Requires-Dist: user-agents
-Requires-Dist: python-jose
-Requires-Dist: fido2>=1.1.0
 
 # django-mfa2
 A Django app that handles MFA, it supports TOTP, U2F, FIDO2 U2F (Web Authn), Email Tokens , Trusted  Devices and backup codes.
 
 [![Works with PassKeys](https://github.com/mkalioby/django-mfa2/raw/master/img/Works%20with%20PassKeys-black.png)](https://fidoalliance.org/passkeys/)
 
 [![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `django-mfa2-2.9.0/README.md` & `django-mfa2-2.9.0b1/README.md`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/django_mfa2.egg-info/PKG-INFO` & `django-mfa2-2.9.0b1/django_mfa2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-mfa2
-Version: 2.9.0
+Version: 2.9.0b1
 Summary: Allows user to add 2FA to their accounts
 Home-page: https://github.com/mkalioby/django-mfa2/
 Download-URL: https://github.com/mkalioby/django-mfa2/
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
@@ -29,22 +29,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django>=2.0
-Requires-Dist: simplejson
-Requires-Dist: pyotp
-Requires-Dist: python-u2flib-server
-Requires-Dist: ua-parser
-Requires-Dist: user-agents
-Requires-Dist: python-jose
-Requires-Dist: fido2>=1.1.0
 
 # django-mfa2
 A Django app that handles MFA, it supports TOTP, U2F, FIDO2 U2F (Web Authn), Email Tokens , Trusted  Devices and backup codes.
 
 [![Works with PassKeys](https://github.com/mkalioby/django-mfa2/raw/master/img/Works%20with%20PassKeys-black.png)](https://fidoalliance.org/passkeys/)
 
 [![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `django-mfa2-2.9.0/django_mfa2.egg-info/SOURCES.txt` & `django-mfa2-2.9.0b1/django_mfa2.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 mfa/migrations/0005_auto_20181115_2014.py
 mfa/migrations/0006_trusted_devices.py
 mfa/migrations/0007_auto_20181230_1549.py
 mfa/migrations/0008_user_keys_last_used.py
 mfa/migrations/0009_user_keys_owned_by_enterprise.py
 mfa/migrations/0010_auto_20201110_0557.py
 mfa/migrations/0011_auto_20210530_0622.py
+mfa/migrations/0012_alter_user_keys_id.py
 mfa/migrations/__init__.py
 mfa/static/mfa/css/bootstrap-toggle.min.css
 mfa/static/mfa/js/bootstrap-toggle.min.js
 mfa/static/mfa/js/bootstrap-toggle.min.js.map
 mfa/static/mfa/js/cbor.js
 mfa/static/mfa/js/qrious.min.js
 mfa/static/mfa/js/qrious.min.js.map
```

### Comparing `django-mfa2-2.9.0/mfa/Common.py` & `django-mfa2-2.9.0b1/mfa/Common.py`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/Email.py` & `django-mfa2-2.9.0b1/mfa/Email.py`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/FIDO2.py` & `django-mfa2-2.9.0b1/mfa/FIDO2.py`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/TrustedDevice.py` & `django-mfa2-2.9.0b1/mfa/TrustedDevice.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from django.template.context_processors import csrf
 import user_agents
 from django.utils import timezone
 from django.urls import reverse
 
 from .models import User_Keys
 
-
 def id_generator(size=6, chars=string.ascii_uppercase + string.digits):
     x = "".join(random.choice(chars) for _ in range(size))
     if not User_Keys.objects.filter(properties__icontains='"key": "%s"' % x).exists():
         return x
     return id_generator(size, chars)
```

### Comparing `django-mfa2-2.9.0/mfa/U2F.py` & `django-mfa2-2.9.0b1/mfa/U2F.py`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/helpers.py` & `django-mfa2-2.9.0b1/mfa/helpers.py`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/middleware.py` & `django-mfa2-2.9.0b1/mfa/middleware.py`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/migrations/0001_initial.py` & `django-mfa2-2.9.0b1/mfa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/migrations/0005_auto_20181115_2014.py` & `django-mfa2-2.9.0b1/mfa/migrations/0005_auto_20181115_2014.py`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/migrations/0006_trusted_devices.py` & `django-mfa2-2.9.0b1/mfa/migrations/0006_trusted_devices.py`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/migrations/0009_user_keys_owned_by_enterprise.py` & `django-mfa2-2.9.0b1/mfa/migrations/0009_user_keys_owned_by_enterprise.py`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/models.py` & `django-mfa2-2.9.0b1/mfa/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         from jsonfield import JSONField  # pyre-ignore[21]
     except ModuleNotFoundError as exc:
         raise ModuleNotFoundError(
             "Can't find a JSONField implementation, please install jsonfield if django < 4.0"
         )
 
 
+
 class User_Keys(models.Model):
     username = models.CharField(max_length=50)
     properties = JSONField(null=True)
     added_on = models.DateTimeField(auto_now_add=True)
     key_type = models.CharField(max_length=25, default="TOTP")
     enabled = models.BooleanField(default=True)
     expires = models.DateTimeField(null=True, default=None, blank=True)
```

### Comparing `django-mfa2-2.9.0/mfa/recovery.py` & `django-mfa2-2.9.0b1/mfa/recovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 def recheck(request):
     context = csrf(request)
     context["mode"] = "recheck"
     if request.method == "POST":
         if verify_login(request, request.user.username, token=request.POST["recovery"])[
             0
         ]:
+
             request.session["mfa"]["rechecked_at"] = time.time()
             return HttpResponse(
                 simplejson.dumps({"recheck": True}), content_type="application/json"
             )
         else:
             return HttpResponse(
                 simplejson.dumps({"recheck": False}), content_type="application/json"
```

### Comparing `django-mfa2-2.9.0/mfa/static/mfa/css/bootstrap-toggle.min.css` & `django-mfa2-2.9.0b1/mfa/static/mfa/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/static/mfa/js/bootstrap-toggle.min.js` & `django-mfa2-2.9.0b1/mfa/static/mfa/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/static/mfa/js/bootstrap-toggle.min.js.map` & `django-mfa2-2.9.0b1/mfa/static/mfa/js/bootstrap-toggle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/static/mfa/js/cbor.js` & `django-mfa2-2.9.0b1/mfa/static/mfa/js/cbor.js`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/static/mfa/js/qrious.min.js` & `django-mfa2-2.9.0b1/mfa/static/mfa/js/qrious.min.js`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/static/mfa/js/qrious.min.js.map` & `django-mfa2-2.9.0b1/mfa/static/mfa/js/qrious.min.js.map`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/static/mfa/js/u2f-api.js` & `django-mfa2-2.9.0b1/mfa/static/mfa/js/u2f-api.js`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/static/mfa/js/ua-parser.min.js` & `django-mfa2-2.9.0b1/mfa/static/mfa/js/ua-parser.min.js`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/Email/Add.html` & `django-mfa2-2.9.0b1/mfa/templates/Email/Add.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/Email/recheck.html` & `django-mfa2-2.9.0b1/mfa/templates/Email/recheck.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/FIDO2/Add.html` & `django-mfa2-2.9.0b1/mfa/templates/FIDO2/Add.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/FIDO2/recheck.html` & `django-mfa2-2.9.0b1/mfa/templates/FIDO2/recheck.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/MFA.html` & `django-mfa2-2.9.0b1/mfa/templates/MFA.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/RECOVERY/Add.html` & `django-mfa2-2.9.0b1/mfa/templates/RECOVERY/Add.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/RECOVERY/recheck.html` & `django-mfa2-2.9.0b1/mfa/templates/RECOVERY/recheck.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/TOTP/Add.html` & `django-mfa2-2.9.0b1/mfa/templates/TOTP/Add.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/TOTP/recheck.html` & `django-mfa2-2.9.0b1/mfa/templates/TOTP/recheck.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/TrustedDevices/Add.html` & `django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/Add.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/TrustedDevices/Done.html` & `django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/Done.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/TrustedDevices/start.html` & `django-mfa2-2.9.0b1/mfa/templates/TrustedDevices/start.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/U2F/Add.html` & `django-mfa2-2.9.0b1/mfa/templates/U2F/Add.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/U2F/recheck.html` & `django-mfa2-2.9.0b1/mfa/templates/U2F/recheck.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/mfa_check.html` & `django-mfa2-2.9.0b1/mfa/templates/mfa_check.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/modal.html` & `django-mfa2-2.9.0b1/mfa/templates/modal.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/templates/select_mfa_method.html` & `django-mfa2-2.9.0b1/mfa/templates/select_mfa_method.html`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/totp.py` & `django-mfa2-2.9.0b1/mfa/totp.py`

 * *Files identical despite different names*

### Comparing `django-mfa2-2.9.0/mfa/urls.py` & `django-mfa2-2.9.0b1/mfa/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from . import views, totp, U2F, TrustedDevice, helpers, FIDO2, Email, recovery
 
 # app_name='mfa'
 
 try:
     from django.urls import re_path as url
 except ImportError:
-    from django.conf.urls import url  # pyre-ignore[21]
+    from django.conf.urls import url
 
 
 urlpatterns = [
     url(r"totp/start/", totp.start, name="start_new_otop"),
     url(r"totp/getToken", totp.getToken, name="get_new_otop"),
     url(r"totp/verify", totp.verify, name="verify_otop"),
     url(r"totp/auth", totp.auth, name="totp_auth"),
```

### Comparing `django-mfa2-2.9.0/mfa/views.py` & `django-mfa2-2.9.0b1/mfa/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         key.delete()
         return HttpResponse("Deleted Successfully")
     else:
         return HttpResponse("Error: You own this token so you can't delete it")
 
 
 def __get_callable_function__(func_path):
+
     if not "." in func_path:
         raise Exception("class Name should include modulename.classname")
 
     parsed_str = func_path.split(".")
     module_name, func_name = ".".join(parsed_str[:-1]), parsed_str[-1]
     imported_module = importlib.import_module(module_name)
     callable_func = getattr(imported_module, func_name)
```

### Comparing `django-mfa2-2.9.0/setup.py` & `django-mfa2-2.9.0b1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
-    name="django-mfa2",
-    version="2.9.0",
-    description="Allows user to add 2FA to their accounts",
+    name='django-mfa2',
+    version='2.9.0b1',
+    description='Allows user to add 2FA to their accounts',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    author="Mohamed El-Kalioby",
-    author_email="mkalioby@mkalioby.com",
-    url="https://github.com/mkalioby/django-mfa2/",
-    download_url="https://github.com/mkalioby/django-mfa2/",
-    license="MIT",
+
+    author='Mohamed El-Kalioby',
+    author_email = 'mkalioby@mkalioby.com',
+    url = 'https://github.com/mkalioby/django-mfa2/',
+    download_url='https://github.com/mkalioby/django-mfa2/',
+    license='MIT',
     packages=find_packages(),
     install_requires=[
-        "django >= 2.0",
-        "simplejson",
-        "pyotp",
-        "python-u2flib-server",
-        "ua-parser",
-        "user-agents",
-        "python-jose",
-        "fido2 >= 1.1.0",
-    ],
+        'django >= 2.0',
+        'simplejson',
+        'pyotp',
+        'python-u2flib-server',
+        'ua-parser',
+        'user-agents',
+        'python-jose',
+        'fido2 >= 1.1.0',
+      ],
     python_requires=">=3.5",
     include_package_data=True,
-    zip_safe=False,  # because we're including static files
+    zip_safe=False, # because we're including static files
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        # "Development Status :: 4 - Beta",
+        #"Development Status :: 5 - Production/Stable",
+        "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 2.0",
         "Framework :: Django :: 2.1",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
@@ -48,9 +49,9 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
-    ],
+]
 )
```

