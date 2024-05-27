# Comparing `tmp/allianceauth-4.0.2.tar.gz` & `tmp/allianceauth-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-4.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "allianceauth-4.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `allianceauth-4.0.2.tar` & `allianceauth-4.1.0.tar`

### file list

```diff
@@ -1,846 +1,847 @@
--rw-r--r--   0        0        0    18026 2024-05-12 10:07:44.141393 allianceauth-4.0.2/LICENSE
--rw-r--r--   0        0        0     4980 2024-05-12 10:07:44.141393 allianceauth-4.0.2/README.md
--rw-r--r--   0        0        0      352 2024-05-12 10:07:44.141393 allianceauth-4.0.2/allianceauth/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.285393 allianceauth-4.0.2/allianceauth/analytics/__init__.py
--rw-r--r--   0        0        0      401 2024-05-12 10:07:44.141393 allianceauth-4.0.2/allianceauth/analytics/admin.py
--rw-r--r--   0        0        0      130 2024-05-12 10:07:44.141393 allianceauth-4.0.2/allianceauth/analytics/apps.py
--rw-r--r--   0        0        0      456 2024-05-12 10:07:44.141393 allianceauth-4.0.2/allianceauth/analytics/fixtures/disable_analytics.json
--rw-r--r--   0        0        0     1664 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0001_initial.py
--rw-r--r--   0        0        0     1072 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py
--rw-r--r--   0        0        0      907 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0003_Generate_Identifier.py
--rw-r--r--   0        0        0     1650 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0004_auto_20211015_0502.py
--rw-r--r--   0        0        0      495 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0005_alter_analyticspath_ignore_path.py
--rw-r--r--   0        0        0     1413 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0006_more_ignore_paths.py
--rw-r--r--   0        0        0      407 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0007_analyticstokens_secret.py
--rw-r--r--   0        0        0     2451 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0008_add_AA_GA-4_Team_Token .py
--rw-r--r--   0        0        0      672 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/migrations/0009_remove_analyticstokens_ignore_paths_and_more.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/analytics/migrations/__init__.py
--rw-r--r--   0        0        0     1173 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/models.py
--rw-r--r--   0        0        0     5449 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/tasks.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/analytics/tests/__init__.py
--rw-r--r--   0        0        0      951 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/tests/test_models.py
--rw-r--r--   0        0        0     2007 2024-05-12 10:07:44.142393 allianceauth-4.0.2/allianceauth/analytics/tests/test_tasks.py
--rw-r--r--   0        0        0     1535 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/analytics/tests/test_utils.py
--rw-r--r--   0        0        0      777 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/analytics/utils.py
--rw-r--r--   0        0        0     1178 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/apps.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/authentication/__init__.py
--rw-r--r--   0        0        0    21182 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/admin.py
--rw-r--r--   0        0        0     1345 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/app_settings.py
--rw-r--r--   0        0        0      514 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/apps.py
--rw-r--r--   0        0        0     1243 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/auth_hooks.py
--rw-r--r--   0        0        0     5150 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/backends.py
--rw-r--r--   0        0        0      434 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/checks.py
--rw-r--r--   0        0        0      641 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/constants.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/authentication/core/__init__.py
--rw-r--r--   0        0        0     1307 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/core/celery_workers.py
--rw-r--r--   0        0        0     3063 2024-05-12 10:07:44.143393 allianceauth-4.0.2/allianceauth/authentication/decorators.py
--rw-r--r--   0        0        0     2480 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/forms.py
--rw-r--r--   0        0        0      776 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/hmac_urls.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/authentication/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/authentication/management/commands/__init__.py
--rw-r--r--   0        0        0     1026 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/management/commands/checkmains.py
--rw-r--r--   0        0        0     2709 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/managers.py
--rw-r--r--   0        0        0     2422 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/middleware.py
--rw-r--r--   0        0        0     3147 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/migrations/0001_initial.py
--rw-r--r--   0        0        0      474 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/migrations/0002_auto_20160907_1914.py
--rw-r--r--   0        0        0      509 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/migrations/0003_authservicesinfo_state.py
--rw-r--r--   0        0        0     2543 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/migrations/0004_create_permissions.py
--rw-r--r--   0        0        0     1144 2024-05-12 10:07:44.144393 allianceauth-4.0.2/allianceauth/authentication/migrations/0005_delete_perms.py
--rw-r--r--   0        0        0     1324 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0006_auto_20160910_0542.py
--rw-r--r--   0        0        0      347 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0007_remove_authservicesinfo_is_blue.py
--rw-r--r--   0        0        0      319 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0008_set_state.py
--rw-r--r--   0        0        0      532 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0009_auto_20161021_0228.py
--rw-r--r--   0        0        0     1235 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py
--rw-r--r--   0        0        0      538 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py
--rw-r--r--   0        0        0     1567 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py
--rw-r--r--   0        0        0     1914 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0013_service_modules.py
--rw-r--r--   0        0        0      660 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0014_fleetup_permission.py
--rw-r--r--   0        0        0    13077 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0015_user_profiles.py
--rw-r--r--   0        0        0     1637 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0016_ownershiprecord.py
--rw-r--r--   0        0        0      612 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py
--rw-r--r--   0        0        0      410 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0018_alter_state_name_length.py
--rw-r--r--   0        0        0      545 2024-05-12 10:07:44.145393 allianceauth-4.0.2/allianceauth/authentication/migrations/0018_state_member_factions.py
--rw-r--r--   0        0        0      295 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/migrations/0019_merge_20211026_0919.py
--rw-r--r--   0        0        0      841 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py
--rw-r--r--   0        0        0     1004 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/migrations/0021_alter_userprofile_language.py
--rw-r--r--   0        0        0      529 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/migrations/0022_userprofile_theme.py
--rw-r--r--   0        0        0      683 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/migrations/0023_alter_userprofile_language.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/authentication/migrations/__init__.py
--rw-r--r--   0        0        0     6050 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/models.py
--rw-r--r--   0        0        0     7806 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/signals.py
--rw-r--r--   0        0        0      506 2024-05-12 10:07:44.146393 allianceauth-4.0.2/allianceauth/authentication/static/allianceauth/authentication/css/admin.css
--rw-r--r--   0        0        0   161344 2024-05-12 10:07:44.147393 allianceauth-4.0.2/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg
--rw-r--r--   0        0        0     2308 2024-05-12 10:07:44.147393 allianceauth-4.0.2/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png
--rw-r--r--   0        0        0     2248 2024-05-12 10:07:44.147393 allianceauth-4.0.2/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/__init__.py
--rw-r--r--   0        0        0     1536 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/counters.py
--rw-r--r--   0        0        0     3257 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/event_series.py
--rw-r--r--   0        0        0     1174 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/helpers.py
--rw-r--r--   0        0        0     1217 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/signals.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.296393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/__init__.py
--rw-r--r--   0        0        0     1704 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_counters.py
--rw-r--r--   0        0        0     5137 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_event_series.py
--rw-r--r--   0        0        0     1009 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_helpers.py
--rw-r--r--   0        0        0     2719 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_signals.py
--rw-r--r--   0        0        0     1661 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/tasks.py
--rw-r--r--   0        0        0      423 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/templates/authentication/dashboard.html
--rw-r--r--   0        0        0      188 2024-05-12 10:07:44.148393 allianceauth-4.0.2/allianceauth/authentication/templates/authentication/dashboard_bs3.html
--rw-r--r--   0        0        0     2476 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/authentication/dashboard_characters.html
--rw-r--r--   0        0        0      838 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/authentication/dashboard_groups.html
--rw-r--r--   0        0        0     3043 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/authentication/tokens.html
--rw-r--r--   0        0        0     2001 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/public/base.html
--rw-r--r--   0        0        0      674 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/public/lang_select.html
--rw-r--r--   0        0        0      493 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/public/login.html
--rw-r--r--   0        0        0     1604 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/public/middle_box.html
--rw-r--r--   0        0        0      956 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/public/register.html
--rw-r--r--   0        0        0      199 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/registration/activate.html
--rw-r--r--   0        0        0      346 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/registration/activation_email.txt
--rw-r--r--   0        0        0      446 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/registration/activation_email_html.txt
--rw-r--r--   0        0        0       49 2024-05-12 10:07:44.149393 allianceauth-4.0.2/allianceauth/authentication/templates/registration/activation_email_subject.txt
--rw-r--r--   0        0        0      833 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/authentication/tests/core/__init__.py
--rw-r--r--   0        0        0     2685 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/core/test_celery_workers.py
--rw-r--r--   0        0        0    29475 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_admin.py
--rw-r--r--   0        0        0     3456 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_app_settings.py
--rw-r--r--   0        0        0     7427 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_backend.py
--rw-r--r--   0        0        0     1517 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_commands.py
--rw-r--r--   0        0        0     3538 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_decorators.py
--rw-r--r--   0        0        0     6316 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_middleware.py
--rw-r--r--   0        0        0    11478 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_models.py
--rw-r--r--   0        0        0     3154 2024-05-12 10:07:44.150393 allianceauth-4.0.2/allianceauth/authentication/tests/test_signals.py
--rw-r--r--   0        0        0    10730 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/authentication/tests/test_templatetags.py
--rw-r--r--   0        0        0     5865 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/authentication/tests/test_views.py
--rw-r--r--   0        0        0     1170 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/authentication/urls.py
--rw-r--r--   0        0        0    14250 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/authentication/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/bin/__init__.py
--rw-r--r--   0        0        0     3680 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/bin/allianceauth.py
--rw-r--r--   0        0        0      274 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/context_processors.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/corputils/__init__.py
--rw-r--r--   0        0        0      140 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/corputils/admin.py
--rw-r--r--   0        0        0      130 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/corputils/apps.py
--rw-r--r--   0        0        0     1043 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/corputils/auth_hooks.py
--rw-r--r--   0        0        0     1970 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/corputils/managers.py
--rw-r--r--   0        0        0     1417 2024-05-12 10:07:44.151393 allianceauth-4.0.2/allianceauth/corputils/migrations/0001_initial.py
--rw-r--r--   0        0        0     5358 2024-05-12 10:07:44.152393 allianceauth-4.0.2/allianceauth/corputils/migrations/0002_migrate_permissions.py
--rw-r--r--   0        0        0      844 2024-05-12 10:07:44.152393 allianceauth-4.0.2/allianceauth/corputils/migrations/0003_granular_permissions.py
--rw-r--r--   0        0        0     2029 2024-05-12 10:07:44.152393 allianceauth-4.0.2/allianceauth/corputils/migrations/0004_member_models.py
--rw-r--r--   0        0        0     1516 2024-05-12 10:07:44.152393 allianceauth-4.0.2/allianceauth/corputils/migrations/0005_cleanup_permissions.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/corputils/migrations/__init__.py
--rw-r--r--   0        0        0     7223 2024-05-12 10:07:44.152393 allianceauth-4.0.2/allianceauth/corputils/models.py
--rw-r--r--   0        0        0   947431 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/swagger.json
--rw-r--r--   0        0        0      298 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/tasks.py
--rw-r--r--   0        0        0     1991 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/templates/corputils/base.html
--rw-r--r--   0        0        0    14560 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/templates/corputils/corpstats.html
--rw-r--r--   0        0        0     2268 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/templates/corputils/search.html
--rw-r--r--   0        0        0    16016 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/tests.py
--rw-r--r--   0        0        0      393 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/urls.py
--rw-r--r--   0        0        0     6999 2024-05-12 10:07:44.155393 allianceauth-4.0.2/allianceauth/corputils/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/eveonline/__init__.py
--rw-r--r--   0        0        0     7277 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/admin.py
--rw-r--r--   0        0        0      130 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/apps.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/__init__.py
--rw-r--r--   0        0        0     1320 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/admin.py
--rw-r--r--   0        0        0      229 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/apps.py
--rw-r--r--   0        0        0     4024 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/migrations/__init__.py
--rw-r--r--   0        0        0    10691 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/models.py
--rw-r--r--   0        0        0     2625 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/signals.py
--rw-r--r--   0        0        0     1403 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/__init__.py
--rw-r--r--   0        0        0     3221 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/test_managers.py
--rw-r--r--   0        0        0    12334 2024-05-12 10:07:44.156393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/test_models.py
--rw-r--r--   0        0        0     7961 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/test_signals.py
--rw-r--r--   0        0        0      646 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/__init__.py
--rw-r--r--   0        0        0     1496 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/dotlan.py
--rw-r--r--   0        0        0     3730 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/eveimageserver.py
--rw-r--r--   0        0        0     1229 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/evewho.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/tests/__init__.py
--rw-r--r--   0        0        0     7329 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/tests/test_evelinks.py
--rw-r--r--   0        0        0    11505 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/tests/test_templatetags.py
--rw-r--r--   0        0        0     1700 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/evelinks/zkillboard.py
--rw-r--r--   0        0        0     3350 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/managers.py
--rw-r--r--   0        0        0     3133 2024-05-12 10:07:44.157393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0001_initial.py
--rw-r--r--   0        0        0      332 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0002_remove_eveapikeypair_error_count.py
--rw-r--r--   0        0        0      797 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py
--rw-r--r--   0        0        0      403 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0004_eveapikeypair_sso_verified.py
--rw-r--r--   0        0        0      354 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0005_remove_eveallianceinfo_member_count.py
--rw-r--r--   0        0        0      655 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py
--rw-r--r--   0        0        0     4599 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0007_unique_id_name.py
--rw-r--r--   0        0        0      854 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0008_remove_apikeys.py
--rw-r--r--   0        0        0      519 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0009_on_delete.py
--rw-r--r--   0        0        0      596 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0010_alliance_ticker.py
--rw-r--r--   0        0        0     1297 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0011_ids_to_integers.py
--rw-r--r--   0        0        0     1121 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0012_index_additions.py
--rw-r--r--   0        0        0      428 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0013_evecorporationinfo_ceo_id.py
--rw-r--r--   0        0        0      416 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0014_auto_20210105_1413.py
--rw-r--r--   0        0        0     1201 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0015_factions.py
--rw-r--r--   0        0        0      409 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0016_character_names_are_not_unique.py
--rw-r--r--   0        0        0      623 2024-05-12 10:07:44.158393 allianceauth-4.0.2/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/eveonline/migrations/__init__.py
--rw-r--r--   0        0        0    14052 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/models.py
--rw-r--r--   0        0        0     9958 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/providers.py
--rw-r--r--   0        0        0    41989 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/swagger.json
--rw-r--r--   0        0        0     3808 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/tasks.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/eveonline/templatetags/__init__.py
--rw-r--r--   0        0        0     8354 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/templatetags/evelinks.py
--rw-r--r--   0        0        0     4194 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/templatetags/examples.html
--rw-r--r--   0        0        0      739 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/tests/__init__.py
--rw-r--r--   0        0        0     6043 2024-05-12 10:07:44.159393 allianceauth-4.0.2/allianceauth/eveonline/tests/esi_client_stub.py
--rw-r--r--   0        0        0   297070 2024-05-12 10:07:44.160393 allianceauth-4.0.2/allianceauth/eveonline/tests/swagger_old.json
--rw-r--r--   0        0        0    10079 2024-05-12 10:07:44.160393 allianceauth-4.0.2/allianceauth/eveonline/tests/test_managers.py
--rw-r--r--   0        0        0    23361 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/eveonline/tests/test_models.py
--rw-r--r--   0        0        0    23834 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/eveonline/tests/test_providers.py
--rw-r--r--   0        0        0    10117 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/eveonline/tests/test_tasks.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.303393 allianceauth-4.0.2/allianceauth/eveonline/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.304393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/__init__.py
--rw-r--r--   0        0        0      156 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/admin.py
--rw-r--r--   0        0        0      148 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/apps.py
--rw-r--r--   0        0        0      494 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/auth_hooks.py
--rw-r--r--   0        0        0      360 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/forms.py
--rw-r--r--   0        0        0     2291 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0001_initial.py
--rw-r--r--   0        0        0      489 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0002_auto_20160905_2220.py
--rw-r--r--   0        0        0      460 2024-05-12 10:07:44.161393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0003_auto_20160906_2354.py
--rw-r--r--   0        0        0      414 2024-05-12 10:07:44.162393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0004_make_strings_more_stringy.py
--rw-r--r--   0        0        0      510 2024-05-12 10:07:44.162393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0005_remove_fat_name.py
--rw-r--r--   0        0        0      397 2024-05-12 10:07:44.162393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0006_auto_20180803_0430.py
--rw-r--r--   0        0        0      606 2024-05-12 10:07:44.162393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0007_sentinel_user.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.311393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/__init__.py
--rw-r--r--   0        0        0     1122 2024-05-12 10:07:44.162393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/models.py
--rw-r--r--   0        0        0   947431 2024-05-12 10:07:44.164393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/swagger.json
--rw-r--r--   0        0        0     1851 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html
--rw-r--r--   0        0        0     1880 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkcreate.html
--rw-r--r--   0        0        0     2811 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html
--rw-r--r--   0        0        0     4516 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html
--rw-r--r--   0        0        0     1725 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html
--rw-r--r--   0        0        0     2730 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html
--rw-r--r--   0        0        0     3011 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html
--rw-r--r--   0        0        0     5912 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html
--rw-r--r--   0        0        0     1386 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/urls.py
--rw-r--r--   0        0        0    16656 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/fleetactivitytracking/views.py
--rw-r--r--   0        0        0       32 2024-05-12 10:07:44.165393 allianceauth-4.0.2/allianceauth/framework/__init__.py
--rw-r--r--   0        0        0     1421 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/framework/api/evecharacter.py
--rw-r--r--   0        0        0     1723 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/framework/api/user.py
--rw-r--r--   0        0        0      202 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/framework/apps.py
--rw-r--r--   0        0        0     3174 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/framework/static/allianceauth/framework/css/auth-framework.css
--rw-r--r--   0        0        0      336 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/framework/templates/framework/header/page-header.html
--rw-r--r--   0        0        0       31 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/framework/tests/__init__.py
--rw-r--r--   0        0        0     4468 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/framework/tests/test_api_user.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.311393 allianceauth-4.0.2/allianceauth/groupmanagement/__init__.py
--rw-r--r--   0        0        0     8978 2024-05-12 10:07:44.166393 allianceauth-4.0.2/allianceauth/groupmanagement/admin.py
--rw-r--r--   0        0        0      252 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/apps.py
--rw-r--r--   0        0        0     2336 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/auth_hooks.py
--rw-r--r--   0        0        0     2466 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/forms.py
--rw-r--r--   0        0        0     4341 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/managers.py
--rw-r--r--   0        0        0     2243 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0001_initial.py
--rw-r--r--   0        0        0      685 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py
--rw-r--r--   0        0        0      261 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0003_default_groups.py
--rw-r--r--   0        0        0     4322 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0004_authgroup.py
--rw-r--r--   0        0        0      631 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0005_authgroup_public.py
--rw-r--r--   0        0        0      607 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py
--rw-r--r--   0        0        0      877 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0007_on_delete.py
--rw-r--r--   0        0        0     1430 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py
--rw-r--r--   0        0        0     1100 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0009_requestlog.py
--rw-r--r--   0        0        0      614 2024-05-12 10:07:44.167393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0010_authgroup_states.py
--rw-r--r--   0        0        0      456 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0011_requestlog_date.py
--rw-r--r--   0        0        0      672 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0012_group_leads.py
--rw-r--r--   0        0        0      397 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0013_fix_requestlog_date_field.py
--rw-r--r--   0        0        0      410 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0014_auto_20200918_1412.py
--rw-r--r--   0        0        0      567 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py
--rw-r--r--   0        0        0      353 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0016_remove_grouprequest_status_field.py
--rw-r--r--   0        0        0     2296 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py
--rw-r--r--   0        0        0     1082 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py
--rw-r--r--   0        0        0      520 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.311393 allianceauth-4.0.2/allianceauth/groupmanagement/migrations/__init__.py
--rw-r--r--   0        0        0     8132 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/models.py
--rw-r--r--   0        0        0     1465 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/signals.py
--rw-r--r--   0        0        0      333 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/tasks.py
--rw-r--r--   0        0        0     4516 2024-05-12 10:07:44.168393 allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/audit.html
--rw-r--r--   0        0        0     4003 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html
--rw-r--r--   0        0        0     3764 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html
--rw-r--r--   0        0        0     4854 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/groups.html
--rw-r--r--   0        0        0     8485 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/index.html
--rw-r--r--   0        0        0      445 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/menu.html
--rw-r--r--   0        0        0      254 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/tests/__init__.py
--rw-r--r--   0        0        0    27572 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_admin.py
--rw-r--r--   0        0        0    17375 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_managers.py
--rw-r--r--   0        0        0    11668 2024-05-12 10:07:44.169393 allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_models.py
--rw-r--r--   0        0        0     4950 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_signals.py
--rw-r--r--   0        0        0     3999 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_views.py
--rw-r--r--   0        0        0     1651 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/groupmanagement/urls.py
--rw-r--r--   0        0        0    20437 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/groupmanagement/views.py
--rw-r--r--   0        0        0     4570 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/hooks.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.319393 allianceauth-4.0.2/allianceauth/hrapplications/__init__.py
--rw-r--r--   0        0        0      693 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/hrapplications/admin.py
--rw-r--r--   0        0        0      145 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/hrapplications/apps.py
--rw-r--r--   0        0        0     1023 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/hrapplications/auth_hooks.py
--rw-r--r--   0        0        0      353 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/hrapplications/forms.py
--rw-r--r--   0        0        0      900 2024-05-12 10:07:44.170393 allianceauth-4.0.2/allianceauth/hrapplications/managers.py
--rw-r--r--   0        0        0     6662 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/0001_initial.py
--rw-r--r--   0        0        0     1036 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/0002_choices_for_questions.py
--rw-r--r--   0        0        0      415 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/0003_applicationquestion_multi_select.py
--rw-r--r--   0        0        0     1461 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py
--rw-r--r--   0        0        0      558 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/0005_sorted_questions.py
--rw-r--r--   0        0        0     1946 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py
--rw-r--r--   0        0        0      427 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/0007_auto_20200918_1412.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.319393 allianceauth-4.0.2/allianceauth/hrapplications/migrations/__init__.py
--rw-r--r--   0        0        0     3237 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/models.py
--rw-r--r--   0        0        0     1411 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/corpchoice.html
--rw-r--r--   0        0        0     2946 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/create.html
--rw-r--r--   0        0        0    12438 2024-05-12 10:07:44.171393 allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/management.html
--rw-r--r--   0        0        0     1308 2024-05-12 10:07:44.172393 allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/partials/modals/search.html
--rw-r--r--   0        0        0     2772 2024-05-12 10:07:44.172393 allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/searchview.html
--rw-r--r--   0        0        0     8251 2024-05-12 10:07:44.172393 allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/view.html
--rw-r--r--   0        0        0     4165 2024-05-12 10:07:44.172393 allianceauth-4.0.2/allianceauth/hrapplications/tests.py
--rw-r--r--   0        0        0     1113 2024-05-12 10:07:44.172393 allianceauth-4.0.2/allianceauth/hrapplications/urls.py
--rw-r--r--   0        0        0    12011 2024-05-12 10:07:44.172393 allianceauth-4.0.2/allianceauth/hrapplications/views.py
--rw-r--r--   0        0        0     7262 2024-05-12 10:07:44.172393 allianceauth-4.0.2/allianceauth/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    85931 2024-05-12 10:07:44.173393 allianceauth-4.0.2/allianceauth/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    45125 2024-05-12 10:07:44.174393 allianceauth-4.0.2/allianceauth/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   100544 2024-05-12 10:07:44.174393 allianceauth-4.0.2/allianceauth/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2024-05-12 10:07:44.174393 allianceauth-4.0.2/allianceauth/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    83238 2024-05-12 10:07:44.175393 allianceauth-4.0.2/allianceauth/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    35108 2024-05-12 10:07:44.175393 allianceauth-4.0.2/allianceauth/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    96583 2024-05-12 10:07:44.175393 allianceauth-4.0.2/allianceauth/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    46059 2024-05-12 10:07:44.176393 allianceauth-4.0.2/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   101728 2024-05-12 10:07:44.176393 allianceauth-4.0.2/allianceauth/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    44568 2024-05-12 10:07:44.177393 allianceauth-4.0.2/allianceauth/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   100475 2024-05-12 10:07:44.177393 allianceauth-4.0.2/allianceauth/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    49616 2024-05-12 10:07:44.177393 allianceauth-4.0.2/allianceauth/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   104822 2024-05-12 10:07:44.178393 allianceauth-4.0.2/allianceauth/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    46390 2024-05-12 10:07:44.178393 allianceauth-4.0.2/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   101738 2024-05-12 10:07:44.178393 allianceauth-4.0.2/allianceauth/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    17293 2024-05-12 10:07:44.179393 allianceauth-4.0.2/allianceauth/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    88812 2024-05-12 10:07:44.179393 allianceauth-4.0.2/allianceauth/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    45885 2024-05-12 10:07:44.179393 allianceauth-4.0.2/allianceauth/locale/pl_PL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   101247 2024-05-12 10:07:44.179393 allianceauth-4.0.2/allianceauth/locale/pl_PL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    45746 2024-05-12 10:07:44.180393 allianceauth-4.0.2/allianceauth/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   106362 2024-05-12 10:07:44.180393 allianceauth-4.0.2/allianceauth/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    57333 2024-05-12 10:07:44.181393 allianceauth-4.0.2/allianceauth/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   112781 2024-05-12 10:07:44.181393 allianceauth-4.0.2/allianceauth/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    26591 2024-05-12 10:07:44.181393 allianceauth-4.0.2/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    92036 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.319393 allianceauth-4.0.2/allianceauth/menu/__init__.py
--rw-r--r--   0        0        0     3721 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/admin.py
--rw-r--r--   0        0        0      459 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/apps.py
--rw-r--r--   0        0        0      485 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/constants.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.319393 allianceauth-4.0.2/allianceauth/menu/core/__init__.py
--rw-r--r--   0        0        0     1363 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/core/menu_item_hooks.py
--rw-r--r--   0        0        0      892 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/core/smart_sync.py
--rw-r--r--   0        0        0      688 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/filters.py
--rw-r--r--   0        0        0     1397 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/forms.py
--rw-r--r--   0        0        0     1932 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/hooks.py
--rw-r--r--   0        0        0     2288 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/managers.py
--rw-r--r--   0        0        0     3143 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.320393 allianceauth-4.0.2/allianceauth/menu/migrations/__init__.py
--rw-r--r--   0        0        0     4094 2024-05-12 10:07:44.182393 allianceauth-4.0.2/allianceauth/menu/models.py
--rw-r--r--   0        0        0      289 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templates/admin/menu/menuitem/change_list.html
--rw-r--r--   0        0        0       62 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-block.html
--rw-r--r--   0        0        0     2009 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-item-bs5.html
--rw-r--r--   0        0        0      101 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-logo.html
--rw-r--r--   0        0        0      535 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-notification-block.html
--rw-r--r--   0        0        0     5068 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-user.html
--rw-r--r--   0        0        0     1308 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templates/menu/sortable-side-menu.html
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.320393 allianceauth-4.0.2/allianceauth/menu/templatetags/__init__.py
--rw-r--r--   0        0        0      893 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templatetags/menu_items.py
--rw-r--r--   0        0        0     5996 2024-05-12 10:07:44.183393 allianceauth-4.0.2/allianceauth/menu/templatetags/menu_menu_items.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.320393 allianceauth-4.0.2/allianceauth/menu/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.320393 allianceauth-4.0.2/allianceauth/menu/tests/core/__init__.py
--rw-r--r--   0        0        0     1799 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/core/test_menu_item_hooks.py
--rw-r--r--   0        0        0     1153 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/core/test_smart_sync.py
--rw-r--r--   0        0        0     2763 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/factories.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.320393 allianceauth-4.0.2/allianceauth/menu/tests/integration/__init__.py
--rw-r--r--   0        0        0     6367 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/integration/test_admin.py
--rw-r--r--   0        0        0     3736 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/integration/test_dashboard.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.320393 allianceauth-4.0.2/allianceauth/menu/tests/templatetags/__init__.py
--rw-r--r--   0        0        0     1688 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/templatetags/test_menu_items.py
--rw-r--r--   0        0        0    11656 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/templatetags/test_menu_menu_items.py
--rw-r--r--   0        0        0      833 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/test_forms.py
--rw-r--r--   0        0        0     2511 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/test_hooks.py
--rw-r--r--   0        0        0     3470 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/test_managers.py
--rw-r--r--   0        0        0     4831 2024-05-12 10:07:44.184393 allianceauth-4.0.2/allianceauth/menu/tests/test_models.py
--rw-r--r--   0        0        0     1177 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/menu/tests/utils.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.320393 allianceauth-4.0.2/allianceauth/models.py
--rw-r--r--   0        0        0       39 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/__init__.py
--rw-r--r--   0        0        0     1138 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/admin.py
--rw-r--r--   0        0        0      142 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/apps.py
--rw-r--r--   0        0        0     1320 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/core.py
--rw-r--r--   0        0        0      998 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/handlers.py
--rw-r--r--   0        0        0     3907 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/managers.py
--rw-r--r--   0        0        0     1117 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/migrations/0001_initial.py
--rw-r--r--   0        0        0      353 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/migrations/0002_auto_20160910_1649.py
--rw-r--r--   0        0        0      514 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py
--rw-r--r--   0        0        0      714 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/migrations/0004_performance_tuning.py
--rw-r--r--   0        0        0      512 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/migrations/0005_fix_level_choices.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.329393 allianceauth-4.0.2/allianceauth/notifications/migrations/__init__.py
--rw-r--r--   0        0        0     2772 2024-05-12 10:07:44.185393 allianceauth-4.0.2/allianceauth/notifications/models.py
--rw-r--r--   0        0        0     1857 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/templates/notifications/list.html
--rw-r--r--   0        0        0     1070 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/templates/notifications/list_partial.html
--rw-r--r--   0        0        0      736 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/templates/notifications/view.html
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.329393 allianceauth-4.0.2/allianceauth/notifications/templatetags/__init__.py
--rw-r--r--   0        0        0     1156 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/templatetags/auth_notifications.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.329393 allianceauth-4.0.2/allianceauth/notifications/tests/__init__.py
--rw-r--r--   0        0        0     3073 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/tests/test_core.py
--rw-r--r--   0        0        0     2392 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/tests/test_handlers.py
--rw-r--r--   0        0        0     1120 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/tests/test_init.py
--rw-r--r--   0        0        0     9437 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/tests/test_managers.py
--rw-r--r--   0        0        0     2398 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/tests/test_models.py
--rw-r--r--   0        0        0     2975 2024-05-12 10:07:44.186393 allianceauth-4.0.2/allianceauth/notifications/tests/test_templatetags.py
--rw-r--r--   0        0        0     1463 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/notifications/tests/test_views.py
--rw-r--r--   0        0        0      674 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/notifications/urls.py
--rw-r--r--   0        0        0     3522 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/notifications/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.329393 allianceauth-4.0.2/allianceauth/optimer/__init__.py
--rw-r--r--   0        0        0      158 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/admin.py
--rw-r--r--   0        0        0      124 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/apps.py
--rw-r--r--   0        0        0     1183 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/auth_hooks.py
--rw-r--r--   0        0        0     1368 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/form.py
--rw-r--r--   0        0        0     1047 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/form_widgets.py
--rw-r--r--   0        0        0     1452 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/migrations/0001_initial.py
--rw-r--r--   0        0        0      424 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/migrations/0002_auto_20170413_0442.py
--rw-r--r--   0        0        0     1076 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py
--rw-r--r--   0        0        0      507 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/migrations/0004_on_delete.py
--rw-r--r--   0        0        0     1447 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/migrations/0005_add_type_and_description.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.329393 allianceauth-4.0.2/allianceauth/optimer/migrations/__init__.py
--rw-r--r--   0        0        0     1247 2024-05-12 10:07:44.187393 allianceauth-4.0.2/allianceauth/optimer/models.py
--rw-r--r--   0        0        0     1980 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/templates/optimer/add.html
--rw-r--r--   0        0        0     1803 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/templates/optimer/dashboard.ops.html
--rw-r--r--   0        0        0     2612 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/templates/optimer/fleetoptable.html
--rw-r--r--   0        0        0     4378 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/templates/optimer/management.html
--rw-r--r--   0        0        0     1986 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/templates/optimer/update.html
--rw-r--r--   0        0        0       26 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/tests.py
--rw-r--r--   0        0        0      336 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/urls.py
--rw-r--r--   0        0        0     7139 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/optimer/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.329393 allianceauth-4.0.2/allianceauth/permissions_tool/__init__.py
--rw-r--r--   0        0        0      150 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/permissions_tool/apps.py
--rw-r--r--   0        0        0      821 2024-05-12 10:07:44.188393 allianceauth-4.0.2/allianceauth/permissions_tool/auth_hooks.py
--rw-r--r--   0        0        0      589 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.329393 allianceauth-4.0.2/allianceauth/permissions_tool/migrations/__init__.py
--rw-r--r--   0        0        0      258 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/models.py
--rw-r--r--   0        0        0     3874 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/templates/permissions_tool/audit.html
--rw-r--r--   0        0        0      789 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html
--rw-r--r--   0        0        0     4553 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/templates/permissions_tool/overview.html
--rw-r--r--   0        0        0     5067 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/tests.py
--rw-r--r--   0        0        0      340 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/urls.py
--rw-r--r--   0        0        0     2610 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/permissions_tool/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.330393 allianceauth-4.0.2/allianceauth/project_template/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.330393 allianceauth-4.0.2/allianceauth/project_template/log/.gitkeep
--rw-r--r--   0        0        0      821 2024-05-12 10:07:44.189393 allianceauth-4.0.2/allianceauth/project_template/manage.py
--rw-r--r--   0        0        0       38 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/project_template/project_name/__init__.py
--rw-r--r--   0        0        0     1417 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/project_template/project_name/celery.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.330393 allianceauth-4.0.2/allianceauth/project_template/project_name/settings/__init__.py
--rw-r--r--   0        0        0     9169 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/project_template/project_name/settings/base.py
--rw-r--r--   0        0        0     3260 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/project_template/project_name/settings/local.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/project_template/project_name/static/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/project_template/project_name/templates/.gitkeep
--rw-r--r--   0        0        0      329 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/project_template/project_name/urls.py
--rw-r--r--   0        0        0      432 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/project_template/project_name/wsgi.py
--rw-r--r--   0        0        0     1408 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/project_template/supervisor.conf
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/__init__.py
--rw-r--r--   0        0        0     3954 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/services/abstract.py
--rw-r--r--   0        0        0     2162 2024-05-12 10:07:44.190393 allianceauth-4.0.2/allianceauth/services/admin.py
--rw-r--r--   0        0        0      179 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/apps.py
--rw-r--r--   0        0        0      662 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/auth_hooks.py
--rw-r--r--   0        0        0     2117 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/forms.py
--rw-r--r--   0        0        0     9149 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/hooks.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/management/commands/__init__.py
--rw-r--r--   0        0        0      469 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/management/commands/verify_service_accounts.py
--rw-r--r--   0        0        0      483 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/migrations/0001_squashed_0003_delete_groupcache.py
--rw-r--r--   0        0        0     1220 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/migrations/0002_nameformatter.py
--rw-r--r--   0        0        0      522 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/migrations/0003_remove_broken_link.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/migrations/__init__.py
--rw-r--r--   0        0        0     1000 2024-05-12 10:07:44.191393 allianceauth-4.0.2/allianceauth/services/models.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/modules/__init__.py
--rw-r--r--   0        0        0       30 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/__init__.py
--rw-r--r--   0        0        0     1070 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/admin.py
--rw-r--r--   0        0        0     1290 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/api.py
--rw-r--r--   0        0        0     1062 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/app_settings.py
--rw-r--r--   0        0        0      148 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/apps.py
--rw-r--r--   0        0        0     5974 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/auth_hooks.py
--rw-r--r--   0        0        0     4446 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/core.py
--rw-r--r--   0        0        0      372 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/__init__.py
--rw-r--r--   0        0        0     1681 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/app_settings.py
--rw-r--r--   0        0        0    28997 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/client.py
--rw-r--r--   0        0        0     1009 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/exceptions.py
--rw-r--r--   0        0        0     4590 2024-05-12 10:07:44.192393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/helpers.py
--rw-r--r--   0        0        0     3853 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/models.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/__init__.py
--rw-r--r--   0        0        0     5027 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/example_objects.json
--rw-r--r--   0        0        0     3013 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/factories.py
--rw-r--r--   0        0        0     2784 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py
--rw-r--r--   0        0        0     4477 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py
--rw-r--r--   0        0        0      904 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md
--rw-r--r--   0        0        0    56114 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_client.py
--rw-r--r--   0        0        0     1045 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py
--rw-r--r--   0        0        0     9724 2024-05-12 10:07:44.193393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py
--rw-r--r--   0        0        0     4966 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_models.py
--rw-r--r--   0        0        0     6281 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/managers.py
--rw-r--r--   0        0        0      680 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/migrations/0001_initial.py
--rw-r--r--   0        0        0     2067 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/migrations/0002_service_permissions.py
--rw-r--r--   0        0        0     1538 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/modules/discord/migrations/__init__.py
--rw-r--r--   0        0        0     7138 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/models.py
--rw-r--r--   0        0        0     9517 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/tasks.py
--rw-r--r--   0        0        0     1508 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html
--rw-r--r--   0        0        0      480 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/__init__.py
--rw-r--r--   0        0        0      917 2024-05-12 10:07:44.194393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/factories.py
--rw-r--r--   0        0        0     2639 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/piloting_tasks.py
--rw-r--r--   0        0        0    10400 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_admin.py
--rw-r--r--   0        0        0      525 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_api.py
--rw-r--r--   0        0        0     7200 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     8456 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_core.py
--rw-r--r--   0        0        0    29715 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_integration.py
--rw-r--r--   0        0        0    19956 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_managers.py
--rw-r--r--   0        0        0    11474 2024-05-12 10:07:44.195393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_models.py
--rw-r--r--   0        0        0    17995 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_tasks.py
--rw-r--r--   0        0        0     3201 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_utils.py
--rw-r--r--   0        0        0     6783 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_views.py
--rw-r--r--   0        0        0      538 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discord/urls.py
--rw-r--r--   0        0        0     2561 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discord/utils.py
--rw-r--r--   0        0        0     3635 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discord/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.339393 allianceauth-4.0.2/allianceauth/services/modules/discourse/__init__.py
--rw-r--r--   0        0        0      264 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discourse/admin.py
--rw-r--r--   0        0        0      154 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discourse/apps.py
--rw-r--r--   0        0        0     1878 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discourse/auth_hooks.py
--rw-r--r--   0        0        0     7039 2024-05-12 10:07:44.196393 allianceauth-4.0.2/allianceauth/services/modules/discourse/manager.py
--rw-r--r--   0        0        0      677 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/migrations/0001_initial.py
--rw-r--r--   0        0        0     2096 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.343393 allianceauth-4.0.2/allianceauth/services/modules/discourse/migrations/__init__.py
--rw-r--r--   0        0        0      529 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/models.py
--rw-r--r--   0        0        0      533 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/providers.py
--rw-r--r--   0        0        0     2276 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/tasks.py
--rw-r--r--   0        0        0      663 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/templates/services/discourse/discourse_service_ctrl.html
--rw-r--r--   0        0        0     5209 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/tests.py
--rw-r--r--   0        0        0      176 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/urls.py
--rw-r--r--   0        0        0     3486 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/discourse/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.343393 allianceauth-4.0.2/allianceauth/services/modules/example/__init__.py
--rw-r--r--   0        0        0      156 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/example/apps.py
--rw-r--r--   0        0        0     1336 2024-05-12 10:07:44.197393 allianceauth-4.0.2/allianceauth/services/modules/example/auth_hooks.py
--rw-r--r--   0        0        0      411 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/example/models.py
--rw-r--r--   0        0        0      206 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/example/urls.py
--rw-r--r--   0        0        0       22 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/example/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.343393 allianceauth-4.0.2/allianceauth/services/modules/ips4/__init__.py
--rw-r--r--   0        0        0      240 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/admin.py
--rw-r--r--   0        0        0      139 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/apps.py
--rw-r--r--   0        0        0     1554 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/auth_hooks.py
--rw-r--r--   0        0        0     4199 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/manager.py
--rw-r--r--   0        0        0      737 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/migrations/0001_initial.py
--rw-r--r--   0        0        0     2025 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.343393 allianceauth-4.0.2/allianceauth/services/modules/ips4/migrations/__init__.py
--rw-r--r--   0        0        0      558 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/models.py
--rw-r--r--   0        0        0     1104 2024-05-12 10:07:44.198393 allianceauth-4.0.2/allianceauth/services/modules/ips4/tasks.py
--rw-r--r--   0        0        0     6035 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/ips4/tests.py
--rw-r--r--   0        0        0      495 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/ips4/urls.py
--rw-r--r--   0        0        0     4825 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/ips4/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.343393 allianceauth-4.0.2/allianceauth/services/modules/mumble/__init__.py
--rw-r--r--   0        0        0      455 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/mumble/admin.py
--rw-r--r--   0        0        0      145 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/mumble/apps.py
--rw-r--r--   0        0        0     2958 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/mumble/auth_hooks.py
--rw-r--r--   0        0        0      726 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0001_initial.py
--rw-r--r--   0        0        0     2868 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py
--rw-r--r--   0        0        0      316 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0002_auto_20161212_0100.py
--rw-r--r--   0        0        0      613 2024-05-12 10:07:44.199393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py
--rw-r--r--   0        0        0      548 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py
--rw-r--r--   0        0        0      561 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py
--rw-r--r--   0        0        0     2063 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py
--rw-r--r--   0        0        0      679 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py
--rw-r--r--   0        0        0      398 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0008_mumbleuser_display_name.py
--rw-r--r--   0        0        0     1181 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py
--rw-r--r--   0        0        0      554 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py
--rw-r--r--   0        0        0      390 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0011_auto_20201011_1009.py
--rw-r--r--   0        0        0     1508 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.352393 allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/__init__.py
--rw-r--r--   0        0        0     5630 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/models.py
--rw-r--r--   0        0        0     3142 2024-05-12 10:07:44.200393 allianceauth-4.0.2/allianceauth/services/modules/mumble/tasks.py
--rw-r--r--   0        0        0     1655 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html
--rw-r--r--   0        0        0     8632 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/mumble/tests.py
--rw-r--r--   0        0        0      560 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/mumble/urls.py
--rw-r--r--   0        0        0      994 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/mumble/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.352393 allianceauth-4.0.2/allianceauth/services/modules/openfire/__init__.py
--rw-r--r--   0        0        0      317 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/openfire/admin.py
--rw-r--r--   0        0        0      151 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/openfire/apps.py
--rw-r--r--   0        0        0     3648 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/openfire/auth_hooks.py
--rw-r--r--   0        0        0      263 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/openfire/forms.py
--rw-r--r--   0        0        0     8321 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/openfire/manager.py
--rw-r--r--   0        0        0      687 2024-05-12 10:07:44.201393 allianceauth-4.0.2/allianceauth/services/modules/openfire/migrations/0001_initial.py
--rw-r--r--   0        0        0     2073 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.352393 allianceauth-4.0.2/allianceauth/services/modules/openfire/migrations/__init__.py
--rw-r--r--   0        0        0      495 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/openfire/models.py
--rw-r--r--   0        0        0     2620 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/openfire/tasks.py
--rw-r--r--   0        0        0     1533 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html
--rw-r--r--   0        0        0     9478 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/openfire/tests.py
--rw-r--r--   0        0        0      585 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/openfire/urls.py
--rw-r--r--   0        0        0     7688 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/openfire/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.362393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/__init__.py
--rw-r--r--   0        0        0      310 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/admin.py
--rw-r--r--   0        0        0      145 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/apps.py
--rw-r--r--   0        0        0     2196 2024-05-12 10:07:44.202393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/auth_hooks.py
--rw-r--r--   0        0        0    13459 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/manager.py
--rw-r--r--   0        0        0      683 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/migrations/0001_initial.py
--rw-r--r--   0        0        0     2049 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.363393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/migrations/__init__.py
--rw-r--r--   0        0        0      487 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/models.py
--rw-r--r--   0        0        0     2478 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/tasks.py
--rw-r--r--   0        0        0     8189 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/tests.py
--rw-r--r--   0        0        0      504 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/urls.py
--rw-r--r--   0        0        0     5139 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/phpbb3/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.363393 allianceauth-4.0.2/allianceauth/services/modules/smf/__init__.py
--rw-r--r--   0        0        0      302 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/smf/admin.py
--rw-r--r--   0        0        0      136 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/smf/apps.py
--rw-r--r--   0        0        0     2408 2024-05-12 10:07:44.203393 allianceauth-4.0.2/allianceauth/services/modules/smf/auth_hooks.py
--rw-r--r--   0        0        0    14780 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/manager.py
--rw-r--r--   0        0        0      677 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/migrations/0001_initial.py
--rw-r--r--   0        0        0     2011 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/migrations/0002_service_permissions.py
--rw-r--r--   0        0        0      694 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.363393 allianceauth-4.0.2/allianceauth/services/modules/smf/migrations/__init__.py
--rw-r--r--   0        0        0      475 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/models.py
--rw-r--r--   0        0        0     3740 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/tasks.py
--rw-r--r--   0        0        0     8057 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/tests.py
--rw-r--r--   0        0        0      489 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/urls.py
--rw-r--r--   0        0        0     5143 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/smf/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.363393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/__init__.py
--rw-r--r--   0        0        0     1872 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/admin.py
--rw-r--r--   0        0        0      209 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/apps.py
--rw-r--r--   0        0        0     2128 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/auth_hooks.py
--rw-r--r--   0        0        0      500 2024-05-12 10:07:44.204393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/forms.py
--rw-r--r--   0        0        0    12601 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/manager.py
--rw-r--r--   0        0        0     1995 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py
--rw-r--r--   0        0        0      538 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py
--rw-r--r--   0        0        0      781 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py
--rw-r--r--   0        0        0     2116 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py
--rw-r--r--   0        0        0      784 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.363393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/__init__.py
--rw-r--r--   0        0        0     1567 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/models.py
--rw-r--r--   0        0        0     1723 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/signals.py
--rw-r--r--   0        0        0     3780 2024-05-12 10:07:44.205393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/tasks.py
--rw-r--r--   0        0        0      296 2024-05-12 10:07:44.206393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/templates/admin/teamspeak3/authts/change_list.html
--rw-r--r--   0        0        0     1472 2024-05-12 10:07:44.206393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html
--rw-r--r--   0        0        0     1121 2024-05-12 10:07:44.206393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html
--rw-r--r--   0        0        0    21498 2024-05-12 10:07:44.206393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/tests.py
--rw-r--r--   0        0        0      661 2024-05-12 10:07:44.206393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/urls.py
--rw-r--r--   0        0        0       23 2024-05-12 10:07:44.206393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/util/__init__.py
--rw-r--r--   0        0        0    15106 2024-05-12 10:07:44.206393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/util/ts3.py
--rw-r--r--   0        0        0     5138 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.363393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/__init__.py
--rw-r--r--   0        0        0      314 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/admin.py
--rw-r--r--   0        0        0      148 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/apps.py
--rw-r--r--   0        0        0     1779 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/auth_hooks.py
--rw-r--r--   0        0        0     3685 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/manager.py
--rw-r--r--   0        0        0      685 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/migrations/0001_initial.py
--rw-r--r--   0        0        0     2067 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.368393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/migrations/__init__.py
--rw-r--r--   0        0        0      491 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/models.py
--rw-r--r--   0        0        0     1268 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/tasks.py
--rw-r--r--   0        0        0     7153 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/tests.py
--rw-r--r--   0        0        0      529 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/urls.py
--rw-r--r--   0        0        0     4821 2024-05-12 10:07:44.207393 allianceauth-4.0.2/allianceauth/services/modules/xenforo/views.py
--rw-r--r--   0        0        0    10087 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/signals.py
--rw-r--r--   0        0        0      126 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/static/allianceauth/services/admin.css
--rw-r--r--   0        0        0     1937 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/tasks.py
--rw-r--r--   0        0        0       57 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/public/menublock.html
--rw-r--r--   0        0        0      335 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/public/menuitem.html
--rw-r--r--   0        0        0     1566 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/services/fleetformattertool.html
--rw-r--r--   0        0        0     1232 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/services/service_confirm_delete.html
--rw-r--r--   0        0        0     1285 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/services/service_credentials.html
--rw-r--r--   0        0        0     1147 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/services/service_password.html
--rw-r--r--   0        0        0      239 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/services/service_status.html
--rw-r--r--   0        0        0      100 2024-05-12 10:07:44.208393 allianceauth-4.0.2/allianceauth/services/templates/services/service_username.html
--rw-r--r--   0        0        0     2422 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/templates/services/services.html
--rw-r--r--   0        0        0     1233 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/templates/services/services_ctrl.html
--rw-r--r--   0        0        0      832 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/templates/services/services_ctrl_base.html
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.368393 allianceauth-4.0.2/allianceauth/services/tests/__init__.py
--rw-r--r--   0        0        0     1048 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/tests/test_hooks.py
--rw-r--r--   0        0        0      514 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/tests/test_models.py
--rw-r--r--   0        0        0     4316 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/tests/test_nameformatter.py
--rw-r--r--   0        0        0    12299 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/tests/test_signals.py
--rw-r--r--   0        0        0     3248 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/tests/test_tasks.py
--rw-r--r--   0        0        0      530 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/urls.py
--rw-r--r--   0        0        0     2450 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/services/views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.368393 allianceauth-4.0.2/allianceauth/srp/__init__.py
--rw-r--r--   0        0        0      205 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/srp/admin.py
--rw-r--r--   0        0        0      112 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/srp/apps.py
--rw-r--r--   0        0        0      960 2024-05-12 10:07:44.209393 allianceauth-4.0.2/allianceauth/srp/auth_hooks.py
--rw-r--r--   0        0        0     1724 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/form.py
--rw-r--r--   0        0        0     1961 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/managers.py
--rw-r--r--   0        0        0     2265 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/migrations/0001_initial.py
--rw-r--r--   0        0        0      488 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/migrations/0002_srpuserrequest_srp_status_choices.py
--rw-r--r--   0        0        0     2048 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/migrations/0003_make_strings_more_stringy.py
--rw-r--r--   0        0        0      746 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/migrations/0004_on_delete.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.368393 allianceauth-4.0.2/allianceauth/srp/migrations/__init__.py
--rw-r--r--   0        0        0     1991 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/models.py
--rw-r--r--   0        0        0      388 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/providers.py
--rw-r--r--   0        0        0    24877 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/swagger.json
--rw-r--r--   0        0        0     2597 2024-05-12 10:07:44.210393 allianceauth-4.0.2/allianceauth/srp/templates/srp/add.html
--rw-r--r--   0        0        0    13408 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/templates/srp/data.html
--rw-r--r--   0        0        0     6364 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/templates/srp/management.html
--rw-r--r--   0        0        0     1432 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/templates/srp/request.html
--rw-r--r--   0        0        0     1765 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/templates/srp/update.html
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.368393 allianceauth-4.0.2/allianceauth/srp/tests/__init__.py
--rw-r--r--   0        0        0     3623 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/tests/test_managers.py
--rw-r--r--   0        0        0    28605 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json
--rw-r--r--   0        0        0      363 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/tests/testdata/zkillboard_killmail_api_81973979.json
--rw-r--r--   0        0        0     1342 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/urls.py
--rw-r--r--   0        0        0    17762 2024-05-12 10:07:44.211393 allianceauth-4.0.2/allianceauth/srp/views.py
--rw-r--r--   0        0        0     4616 2024-05-12 10:07:44.212393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/auth-base.css
--rw-r--r--   0        0        0     1173 2024-05-12 10:07:44.212393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/checkbox.css
--rw-r--r--   0        0        0      865 2024-05-12 10:07:44.212393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less
--rw-r--r--   0        0        0     1078 2024-05-12 10:07:44.212393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/darkly/LICENSE
--rw-r--r--   0        0        0      624 2024-05-12 10:07:44.212393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/darkly/darkly.less
--rw-r--r--   0        0        0   122466 2024-05-12 10:07:44.213393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css
--rw-r--r--   0        0        0      979 2024-05-12 10:07:44.213393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly-shared.less
--rw-r--r--   0        0        0     1078 2024-05-12 10:07:44.213393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly/LICENSE
--rw-r--r--   0        0        0      985 2024-05-12 10:07:44.213393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly/flatly.less
--rw-r--r--   0        0        0   123138 2024-05-12 10:07:44.213393 allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css
--rwxr-xr-x   0        0        0    21465 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/allianceauth.png
--rw-r--r--   0        0        0     7686 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/android-chrome-192x192.png
--rw-r--r--   0        0        0    26346 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/android-chrome-512x512.png
--rw-r--r--   0        0        0     7160 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/apple-touch-icon.png
--rw-r--r--   0        0        0      272 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/browserconfig.xml
--rw-r--r--   0        0        0      941 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon-16x16.png
--rw-r--r--   0        0        0     1565 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon-32x32.png
--rwxr-xr-x   0        0        0     2180 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon-96x96.png
--rw-r--r--   0        0        0    15086 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon.ico
--rw-r--r--   0        0        0     4681 2024-05-12 10:07:44.214393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/mstile-150x150.png
--rw-r--r--   0        0        0     2590 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/safari-pinned-tab.svg
--rw-r--r--   0        0        0      478 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/icons/site.webmanifest
--rw-r--r--   0        0        0    10836 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/images/auth-logo.png
--rw-r--r--   0        0        0     2278 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/images/auth-logo.svg
--rw-r--r--   0        0        0      573 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/eve-time.js
--rw-r--r--   0        0        0     1070 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/filterDropDown/LICENSE
--rw-r--r--   0        0        0    10422 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js
--rw-r--r--   0        0        0     4205 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js
--rw-r--r--   0        0        0     7090 2024-05-12 10:07:44.215393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     7074 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     4618 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     7111 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     4618 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     6487 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    15830 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css
--rw-r--r--   0        0        0     7142 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     7126 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     4670 2024-05-12 10:07:44.216393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     7163 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     4670 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     6539 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    15842 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/jquery-ui.min.css
--rw-r--r--   0        0        0     2391 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/refresh-notification-icon.js
--rw-r--r--   0        0        0     2636 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/refresh_notifications.js
--rw-r--r--   0        0        0     1170 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/timerboard.js
--rw-r--r--   0        0        0     1056 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/allianceauth/js/timers.js
--rw-r--r--   0        0        0       26 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/static/robots.txt
--rw-r--r--   0        0        0      119 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/templates/admin/base_site.html
--rw-r--r--   0        0        0      403 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/templates/allianceauth/admin-status/celery_bar_partial.html
--rw-r--r--   0        0        0     1282 2024-05-12 10:07:44.217393 allianceauth-4.0.2/allianceauth/templates/allianceauth/admin-status/esi_check.html
--rw-r--r--   0        0        0       47 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/admin-status/include.html
--rw-r--r--   0        0        0     8149 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/admin-status/overview.html
--rw-r--r--   0        0        0     5350 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/base-bs5.html
--rw-r--r--   0        0        0     2443 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/base.html
--rw-r--r--   0        0        0     1289 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/error.html
--rw-r--r--   0        0        0      928 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/icons.html
--rw-r--r--   0        0        0      996 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/messages-bs5.html
--rw-r--r--   0        0        0     1115 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/messages.html
--rw-r--r--   0        0        0      263 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/night-toggle.html
--rw-r--r--   0        0        0      450 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/notifications_menu_item.html
--rw-r--r--   0        0        0      879 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/side-menu.html
--rw-r--r--   0        0        0      904 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu-admin.html
--rw-r--r--   0        0        0      855 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu-rh-default.html
--rw-r--r--   0        0        0     3086 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu-user-dropdown.html
--rw-r--r--   0        0        0     1576 2024-05-12 10:07:44.218393 allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu.html
--rw-r--r--   0        0        0       96 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/auth-base-css.html
--rw-r--r--   0        0        0      111 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/auth-framework-css.html
--rw-r--r--   0        0        0      171 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/bootstrap-css-bs5.html
--rw-r--r--   0        0        0     1269 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/bootstrap-css.html
--rw-r--r--   0        0        0      503 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/bootstrap-js-bs5.html
--rw-r--r--   0        0        0      613 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/bootstrap-js.html
--rw-r--r--   0        0        0       95 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/checkbox-css.html
--rw-r--r--   0        0        0      343 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/clipboard-js.html
--rw-r--r--   0        0        0      369 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/datatables-css-bs5.html
--rw-r--r--   0        0        0      365 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/datatables-css.html
--rw-r--r--   0        0        0      628 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/datatables-js-bs5.html
--rw-r--r--   0        0        0      626 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/datatables-js.html
--rw-r--r--   0        0        0       86 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/evetime-js.html
--rw-r--r--   0        0        0      111 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/filterdropdown-js.html
--rw-r--r--   0        0        0      350 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/fontawesome.html
--rw-r--r--   0        0        0      237 2024-05-12 10:07:44.219393 allianceauth-4.0.2/allianceauth/templates/bundles/image-auth-logo.html
--rw-r--r--   0        0        0      392 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/jquery-datetimepicker-css.html
--rw-r--r--   0        0        0      387 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/jquery-datetimepicker-js.html
--rw-r--r--   0        0        0      321 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/jquery-js.html
--rw-r--r--   0        0        0      500 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/jquery-ui-css.html
--rw-r--r--   0        0        0      333 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/jquery-ui-js.html
--rw-r--r--   0        0        0      344 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/jquery-visibility-js.html
--rw-r--r--   0        0        0      579 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/moment-js.html
--rw-r--r--   0        0        0      103 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/refresh-notification-icon-js.html
--rw-r--r--   0        0        0       99 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/refresh-notifications-js.html
--rw-r--r--   0        0        0       88 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/timerboard-js.html
--rw-r--r--   0        0        0       84 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/timers-js.html
--rw-r--r--   0        0        0      368 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/x-editable-js.html
--rw-r--r--   0        0        0      375 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templates/bundles/x-editable.css.html
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/templatetags/__init__.py
--rw-r--r--   0        0        0     5665 2024-05-12 10:07:44.220393 allianceauth-4.0.2/allianceauth/templatetags/admin_status.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/tests/__init__.py
--rw-r--r--   0        0        0    11465 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/tests/auth_utils.py
--rw-r--r--   0        0        0     2061 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/tests/test_auth_utils.py
--rw-r--r--   0        0        0     2897 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/tests/test_urls.py
--rw-r--r--   0        0        0     1403 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/tests/test_views.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/theme/__init__.py
--rw-r--r--   0        0        0      153 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/theme/apps.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/theme/bootstrap/__init__.py
--rw-r--r--   0        0        0      241 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/theme/bootstrap/apps.py
--rw-r--r--   0        0        0     1778 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/theme/bootstrap/auth_hooks.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/theme/darkly/__init__.py
--rw-r--r--   0        0        0      240 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/theme/darkly/apps.py
--rw-r--r--   0        0        0     1232 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/theme/darkly/auth_hooks.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/theme/flatly/__init__.py
--rw-r--r--   0        0        0      240 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/theme/flatly/apps.py
--rw-r--r--   0        0        0     1227 2024-05-12 10:07:44.221393 allianceauth-4.0.2/allianceauth/theme/flatly/auth_hooks.py
--rw-r--r--   0        0        0     1537 2024-05-12 10:07:44.222393 allianceauth-4.0.2/allianceauth/theme/hooks.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/theme/materia/__init__.py
--rw-r--r--   0        0        0      244 2024-05-12 10:07:44.222393 allianceauth-4.0.2/allianceauth/theme/materia/apps.py
--rw-r--r--   0        0        0     1243 2024-05-12 10:07:44.222393 allianceauth-4.0.2/allianceauth/theme/materia/auth_hooks.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/theme/templates/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.372393 allianceauth-4.0.2/allianceauth/theme/templates/theme/__init__.py
--rw-r--r--   0        0        0      389 2024-05-12 10:07:44.222393 allianceauth-4.0.2/allianceauth/theme/templates/theme/theme_imports_css.html
--rw-r--r--   0        0        0      376 2024-05-12 10:07:44.222393 allianceauth-4.0.2/allianceauth/theme/templates/theme/theme_imports_js.html
--rw-r--r--   0        0        0      494 2024-05-12 10:07:44.222393 allianceauth-4.0.2/allianceauth/theme/templates/theme/theme_select.html
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.373393 allianceauth-4.0.2/allianceauth/theme/templatetags/__init__.py
--rw-r--r--   0        0        0     1921 2024-05-12 10:07:44.222393 allianceauth-4.0.2/allianceauth/theme/templatetags/theme_tags.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.373393 allianceauth-4.0.2/allianceauth/thirdparty/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.373393 allianceauth-4.0.2/allianceauth/thirdparty/navhelper/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.373393 allianceauth-4.0.2/allianceauth/thirdparty/navhelper/templatetags/__init__.py
--rw-r--r--   0        0        0     2876 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/thirdparty/navhelper/templatetags/navactive.py
--rw-r--r--   0        0        0     3407 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/thirdparty/navhelper/tests.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.373393 allianceauth-4.0.2/allianceauth/timerboard/__init__.py
--rw-r--r--   0        0        0      111 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/admin.py
--rw-r--r--   0        0        0      133 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/apps.py
--rw-r--r--   0        0        0     1141 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/auth_hooks.py
--rw-r--r--   0        0        0     5267 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/form.py
--rw-r--r--   0        0        0     1629 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/migrations/0001_initial.py
--rw-r--r--   0        0        0     1063 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py
--rw-r--r--   0        0        0      763 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/migrations/0003_on_delete.py
--rw-r--r--   0        0        0      811 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/migrations/0004_timer_type.py
--rw-r--r--   0        0        0      410 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/migrations/0005_alter_timer_planet_moon.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.374393 allianceauth-4.0.2/allianceauth/timerboard/migrations/__init__.py
--rw-r--r--   0        0        0     1593 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/models.py
--rw-r--r--   0        0        0     3069 2024-05-12 10:07:44.223393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/dashboard.timers.html
--rw-r--r--   0        0        0     1917 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/form.html
--rw-r--r--   0        0        0      147 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/index_button.html
--rw-r--r--   0        0        0     1021 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html
--rw-r--r--   0        0        0      810 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timer_create_form.html
--rw-r--r--   0        0        0      830 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timer_update_form.html
--rw-r--r--   0        0        0     8213 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timertable.html
--rw-r--r--   0        0        0     5121 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/view.html
--rw-r--r--   0        0        0     8741 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/tests.py
--rw-r--r--   0        0        0      358 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/urls.py
--rw-r--r--   0        0        0     4075 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/timerboard/views.py
--rw-r--r--   0        0        0     2688 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/urls.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.374393 allianceauth-4.0.2/allianceauth/utils/__init__.py
--rw-r--r--   0        0        0      568 2024-05-12 10:07:44.224393 allianceauth-4.0.2/allianceauth/utils/cache.py
--rw-r--r--   0        0        0     1971 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/utils/counters.py
--rw-r--r--   0        0        0      615 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/utils/django.py
--rw-r--r--   0        0        0      844 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/utils/testing.py
--rw-r--r--   0        0        0        0 2024-05-12 10:07:44.375393 allianceauth-4.0.2/allianceauth/utils/tests/__init__.py
--rw-r--r--   0        0        0     1194 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/utils/tests/test_cache.py
--rw-r--r--   0        0        0     3328 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/utils/tests/test_counters.py
--rw-r--r--   0        0        0      777 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/utils/tests/test_django.py
--rw-r--r--   0        0        0      310 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/utils/tests/test_testing.py
--rw-r--r--   0        0        0     3289 2024-05-12 10:07:44.225393 allianceauth-4.0.2/allianceauth/views.py
--rw-r--r--   0        0        0     2498 2024-05-12 10:07:44.248393 allianceauth-4.0.2/pyproject.toml
--rw-r--r--   0        0        0     7491 1970-01-01 00:00:00.000000 allianceauth-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0    18026 2024-05-27 04:40:28.801463 allianceauth-4.1.0/LICENSE
+-rw-r--r--   0        0        0     4980 2024-05-27 04:40:28.801463 allianceauth-4.1.0/README.md
+-rw-r--r--   0        0        0      352 2024-05-27 04:40:28.801463 allianceauth-4.1.0/allianceauth/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.950463 allianceauth-4.1.0/allianceauth/analytics/__init__.py
+-rw-r--r--   0        0        0      401 2024-05-27 04:40:28.801463 allianceauth-4.1.0/allianceauth/analytics/admin.py
+-rw-r--r--   0        0        0      130 2024-05-27 04:40:28.801463 allianceauth-4.1.0/allianceauth/analytics/apps.py
+-rw-r--r--   0        0        0      456 2024-05-27 04:40:28.802464 allianceauth-4.1.0/allianceauth/analytics/fixtures/disable_analytics.json
+-rw-r--r--   0        0        0     1664 2024-05-27 04:40:28.802464 allianceauth-4.1.0/allianceauth/analytics/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1072 2024-05-27 04:40:28.802464 allianceauth-4.1.0/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py
+-rw-r--r--   0        0        0      907 2024-05-27 04:40:28.802464 allianceauth-4.1.0/allianceauth/analytics/migrations/0003_Generate_Identifier.py
+-rw-r--r--   0        0        0     1650 2024-05-27 04:40:28.802464 allianceauth-4.1.0/allianceauth/analytics/migrations/0004_auto_20211015_0502.py
+-rw-r--r--   0        0        0      495 2024-05-27 04:40:28.802464 allianceauth-4.1.0/allianceauth/analytics/migrations/0005_alter_analyticspath_ignore_path.py
+-rw-r--r--   0        0        0     1413 2024-05-27 04:40:28.802464 allianceauth-4.1.0/allianceauth/analytics/migrations/0006_more_ignore_paths.py
+-rw-r--r--   0        0        0      407 2024-05-27 04:40:28.802464 allianceauth-4.1.0/allianceauth/analytics/migrations/0007_analyticstokens_secret.py
+-rw-r--r--   0        0        0     2451 2024-05-27 04:40:28.802464 allianceauth-4.1.0/allianceauth/analytics/migrations/0008_add_AA_GA-4_Team_Token .py
+-rw-r--r--   0        0        0      672 2024-05-27 04:40:28.802464 allianceauth-4.1.0/allianceauth/analytics/migrations/0009_remove_analyticstokens_ignore_paths_and_more.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.956463 allianceauth-4.1.0/allianceauth/analytics/migrations/__init__.py
+-rw-r--r--   0        0        0     1173 2024-05-27 04:40:28.802464 allianceauth-4.1.0/allianceauth/analytics/models.py
+-rw-r--r--   0        0        0     5449 2024-05-27 04:40:28.802464 allianceauth-4.1.0/allianceauth/analytics/tasks.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.956463 allianceauth-4.1.0/allianceauth/analytics/tests/__init__.py
+-rw-r--r--   0        0        0      951 2024-05-27 04:40:28.802464 allianceauth-4.1.0/allianceauth/analytics/tests/test_models.py
+-rw-r--r--   0        0        0     2007 2024-05-27 04:40:28.803464 allianceauth-4.1.0/allianceauth/analytics/tests/test_tasks.py
+-rw-r--r--   0        0        0     1535 2024-05-27 04:40:28.803464 allianceauth-4.1.0/allianceauth/analytics/tests/test_utils.py
+-rw-r--r--   0        0        0      777 2024-05-27 04:40:28.803464 allianceauth-4.1.0/allianceauth/analytics/utils.py
+-rw-r--r--   0        0        0     1178 2024-05-27 04:40:28.803464 allianceauth-4.1.0/allianceauth/apps.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.956463 allianceauth-4.1.0/allianceauth/authentication/__init__.py
+-rw-r--r--   0        0        0    21182 2024-05-27 04:40:28.803464 allianceauth-4.1.0/allianceauth/authentication/admin.py
+-rw-r--r--   0        0        0     1345 2024-05-27 04:40:28.803464 allianceauth-4.1.0/allianceauth/authentication/app_settings.py
+-rw-r--r--   0        0        0      514 2024-05-27 04:40:28.803464 allianceauth-4.1.0/allianceauth/authentication/apps.py
+-rw-r--r--   0        0        0     1243 2024-05-27 04:40:28.803464 allianceauth-4.1.0/allianceauth/authentication/auth_hooks.py
+-rw-r--r--   0        0        0     5150 2024-05-27 04:40:28.803464 allianceauth-4.1.0/allianceauth/authentication/backends.py
+-rw-r--r--   0        0        0      434 2024-05-27 04:40:28.803464 allianceauth-4.1.0/allianceauth/authentication/checks.py
+-rw-r--r--   0        0        0      641 2024-05-27 04:40:28.803464 allianceauth-4.1.0/allianceauth/authentication/constants.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.956463 allianceauth-4.1.0/allianceauth/authentication/core/__init__.py
+-rw-r--r--   0        0        0     1307 2024-05-27 04:40:28.804463 allianceauth-4.1.0/allianceauth/authentication/core/celery_workers.py
+-rw-r--r--   0        0        0     3063 2024-05-27 04:40:28.804463 allianceauth-4.1.0/allianceauth/authentication/decorators.py
+-rw-r--r--   0        0        0     2480 2024-05-27 04:40:28.804463 allianceauth-4.1.0/allianceauth/authentication/forms.py
+-rw-r--r--   0        0        0      776 2024-05-27 04:40:28.804463 allianceauth-4.1.0/allianceauth/authentication/hmac_urls.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.956463 allianceauth-4.1.0/allianceauth/authentication/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.956463 allianceauth-4.1.0/allianceauth/authentication/management/commands/__init__.py
+-rw-r--r--   0        0        0     1026 2024-05-27 04:40:28.804463 allianceauth-4.1.0/allianceauth/authentication/management/commands/checkmains.py
+-rw-r--r--   0        0        0     2709 2024-05-27 04:40:28.804463 allianceauth-4.1.0/allianceauth/authentication/managers.py
+-rw-r--r--   0        0        0     2422 2024-05-27 04:40:28.804463 allianceauth-4.1.0/allianceauth/authentication/middleware.py
+-rw-r--r--   0        0        0     3147 2024-05-27 04:40:28.804463 allianceauth-4.1.0/allianceauth/authentication/migrations/0001_initial.py
+-rw-r--r--   0        0        0      474 2024-05-27 04:40:28.804463 allianceauth-4.1.0/allianceauth/authentication/migrations/0002_auto_20160907_1914.py
+-rw-r--r--   0        0        0      509 2024-05-27 04:40:28.804463 allianceauth-4.1.0/allianceauth/authentication/migrations/0003_authservicesinfo_state.py
+-rw-r--r--   0        0        0     2543 2024-05-27 04:40:28.804463 allianceauth-4.1.0/allianceauth/authentication/migrations/0004_create_permissions.py
+-rw-r--r--   0        0        0     1144 2024-05-27 04:40:28.805464 allianceauth-4.1.0/allianceauth/authentication/migrations/0005_delete_perms.py
+-rw-r--r--   0        0        0     1324 2024-05-27 04:40:28.805464 allianceauth-4.1.0/allianceauth/authentication/migrations/0006_auto_20160910_0542.py
+-rw-r--r--   0        0        0      347 2024-05-27 04:40:28.805464 allianceauth-4.1.0/allianceauth/authentication/migrations/0007_remove_authservicesinfo_is_blue.py
+-rw-r--r--   0        0        0      319 2024-05-27 04:40:28.805464 allianceauth-4.1.0/allianceauth/authentication/migrations/0008_set_state.py
+-rw-r--r--   0        0        0      532 2024-05-27 04:40:28.805464 allianceauth-4.1.0/allianceauth/authentication/migrations/0009_auto_20161021_0228.py
+-rw-r--r--   0        0        0     1235 2024-05-27 04:40:28.805464 allianceauth-4.1.0/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py
+-rw-r--r--   0        0        0      538 2024-05-27 04:40:28.805464 allianceauth-4.1.0/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py
+-rw-r--r--   0        0        0     1567 2024-05-27 04:40:28.805464 allianceauth-4.1.0/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py
+-rw-r--r--   0        0        0     1914 2024-05-27 04:40:28.805464 allianceauth-4.1.0/allianceauth/authentication/migrations/0013_service_modules.py
+-rw-r--r--   0        0        0      660 2024-05-27 04:40:28.805464 allianceauth-4.1.0/allianceauth/authentication/migrations/0014_fleetup_permission.py
+-rw-r--r--   0        0        0    13077 2024-05-27 04:40:28.805464 allianceauth-4.1.0/allianceauth/authentication/migrations/0015_user_profiles.py
+-rw-r--r--   0        0        0     1637 2024-05-27 04:40:28.805464 allianceauth-4.1.0/allianceauth/authentication/migrations/0016_ownershiprecord.py
+-rw-r--r--   0        0        0      612 2024-05-27 04:40:28.805464 allianceauth-4.1.0/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py
+-rw-r--r--   0        0        0      410 2024-05-27 04:40:28.805464 allianceauth-4.1.0/allianceauth/authentication/migrations/0018_alter_state_name_length.py
+-rw-r--r--   0        0        0      545 2024-05-27 04:40:28.806464 allianceauth-4.1.0/allianceauth/authentication/migrations/0018_state_member_factions.py
+-rw-r--r--   0        0        0      295 2024-05-27 04:40:28.806464 allianceauth-4.1.0/allianceauth/authentication/migrations/0019_merge_20211026_0919.py
+-rw-r--r--   0        0        0      841 2024-05-27 04:40:28.806464 allianceauth-4.1.0/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py
+-rw-r--r--   0        0        0     1004 2024-05-27 04:40:28.806464 allianceauth-4.1.0/allianceauth/authentication/migrations/0021_alter_userprofile_language.py
+-rw-r--r--   0        0        0      529 2024-05-27 04:40:28.806464 allianceauth-4.1.0/allianceauth/authentication/migrations/0022_userprofile_theme.py
+-rw-r--r--   0        0        0      683 2024-05-27 04:40:28.806464 allianceauth-4.1.0/allianceauth/authentication/migrations/0023_alter_userprofile_language.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.956463 allianceauth-4.1.0/allianceauth/authentication/migrations/__init__.py
+-rw-r--r--   0        0        0     6050 2024-05-27 04:40:28.806464 allianceauth-4.1.0/allianceauth/authentication/models.py
+-rw-r--r--   0        0        0     7806 2024-05-27 04:40:28.806464 allianceauth-4.1.0/allianceauth/authentication/signals.py
+-rw-r--r--   0        0        0      506 2024-05-27 04:40:28.806464 allianceauth-4.1.0/allianceauth/authentication/static/allianceauth/authentication/css/admin.css
+-rw-r--r--   0        0        0   161344 2024-05-27 04:40:28.807464 allianceauth-4.1.0/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg
+-rw-r--r--   0        0        0     2308 2024-05-27 04:40:28.807464 allianceauth-4.1.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png
+-rw-r--r--   0        0        0     2248 2024-05-27 04:40:28.807464 allianceauth-4.1.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.956463 allianceauth-4.1.0/allianceauth/authentication/task_statistics/__init__.py
+-rw-r--r--   0        0        0     1536 2024-05-27 04:40:28.808463 allianceauth-4.1.0/allianceauth/authentication/task_statistics/counters.py
+-rw-r--r--   0        0        0     3257 2024-05-27 04:40:28.808463 allianceauth-4.1.0/allianceauth/authentication/task_statistics/event_series.py
+-rw-r--r--   0        0        0     1174 2024-05-27 04:40:28.808463 allianceauth-4.1.0/allianceauth/authentication/task_statistics/helpers.py
+-rw-r--r--   0        0        0     1217 2024-05-27 04:40:28.808463 allianceauth-4.1.0/allianceauth/authentication/task_statistics/signals.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.956463 allianceauth-4.1.0/allianceauth/authentication/task_statistics/tests/__init__.py
+-rw-r--r--   0        0        0     1704 2024-05-27 04:40:28.808463 allianceauth-4.1.0/allianceauth/authentication/task_statistics/tests/test_counters.py
+-rw-r--r--   0        0        0     5137 2024-05-27 04:40:28.808463 allianceauth-4.1.0/allianceauth/authentication/task_statistics/tests/test_event_series.py
+-rw-r--r--   0        0        0     1009 2024-05-27 04:40:28.808463 allianceauth-4.1.0/allianceauth/authentication/task_statistics/tests/test_helpers.py
+-rw-r--r--   0        0        0     2719 2024-05-27 04:40:28.808463 allianceauth-4.1.0/allianceauth/authentication/task_statistics/tests/test_signals.py
+-rw-r--r--   0        0        0     1661 2024-05-27 04:40:28.808463 allianceauth-4.1.0/allianceauth/authentication/tasks.py
+-rw-r--r--   0        0        0      423 2024-05-27 04:40:28.808463 allianceauth-4.1.0/allianceauth/authentication/templates/authentication/dashboard.html
+-rw-r--r--   0        0        0      188 2024-05-27 04:40:28.809464 allianceauth-4.1.0/allianceauth/authentication/templates/authentication/dashboard_bs3.html
+-rw-r--r--   0        0        0     2425 2024-05-27 04:40:28.809464 allianceauth-4.1.0/allianceauth/authentication/templates/authentication/dashboard_characters.html
+-rw-r--r--   0        0        0      887 2024-05-27 04:40:28.809464 allianceauth-4.1.0/allianceauth/authentication/templates/authentication/dashboard_groups.html
+-rw-r--r--   0        0        0     3043 2024-05-27 04:40:28.809464 allianceauth-4.1.0/allianceauth/authentication/templates/authentication/tokens.html
+-rw-r--r--   0        0        0     2001 2024-05-27 04:40:28.809464 allianceauth-4.1.0/allianceauth/authentication/templates/public/base.html
+-rw-r--r--   0        0        0      674 2024-05-27 04:40:28.809464 allianceauth-4.1.0/allianceauth/authentication/templates/public/lang_select.html
+-rw-r--r--   0        0        0      493 2024-05-27 04:40:28.809464 allianceauth-4.1.0/allianceauth/authentication/templates/public/login.html
+-rw-r--r--   0        0        0     1604 2024-05-27 04:40:28.809464 allianceauth-4.1.0/allianceauth/authentication/templates/public/middle_box.html
+-rw-r--r--   0        0        0      956 2024-05-27 04:40:28.809464 allianceauth-4.1.0/allianceauth/authentication/templates/public/register.html
+-rw-r--r--   0        0        0      199 2024-05-27 04:40:28.809464 allianceauth-4.1.0/allianceauth/authentication/templates/registration/activate.html
+-rw-r--r--   0        0        0      346 2024-05-27 04:40:28.809464 allianceauth-4.1.0/allianceauth/authentication/templates/registration/activation_email.txt
+-rw-r--r--   0        0        0      446 2024-05-27 04:40:28.809464 allianceauth-4.1.0/allianceauth/authentication/templates/registration/activation_email_html.txt
+-rw-r--r--   0        0        0       49 2024-05-27 04:40:28.809464 allianceauth-4.1.0/allianceauth/authentication/templates/registration/activation_email_subject.txt
+-rw-r--r--   0        0        0      833 2024-05-27 04:40:28.810464 allianceauth-4.1.0/allianceauth/authentication/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.969463 allianceauth-4.1.0/allianceauth/authentication/tests/core/__init__.py
+-rw-r--r--   0        0        0     2685 2024-05-27 04:40:28.810464 allianceauth-4.1.0/allianceauth/authentication/tests/core/test_celery_workers.py
+-rw-r--r--   0        0        0    29475 2024-05-27 04:40:28.810464 allianceauth-4.1.0/allianceauth/authentication/tests/test_admin.py
+-rw-r--r--   0        0        0     3456 2024-05-27 04:40:28.810464 allianceauth-4.1.0/allianceauth/authentication/tests/test_app_settings.py
+-rw-r--r--   0        0        0     7427 2024-05-27 04:40:28.810464 allianceauth-4.1.0/allianceauth/authentication/tests/test_backend.py
+-rw-r--r--   0        0        0     1517 2024-05-27 04:40:28.810464 allianceauth-4.1.0/allianceauth/authentication/tests/test_commands.py
+-rw-r--r--   0        0        0     3538 2024-05-27 04:40:28.810464 allianceauth-4.1.0/allianceauth/authentication/tests/test_decorators.py
+-rw-r--r--   0        0        0     6316 2024-05-27 04:40:28.810464 allianceauth-4.1.0/allianceauth/authentication/tests/test_middleware.py
+-rw-r--r--   0        0        0    11478 2024-05-27 04:40:28.810464 allianceauth-4.1.0/allianceauth/authentication/tests/test_models.py
+-rw-r--r--   0        0        0     3154 2024-05-27 04:40:28.810464 allianceauth-4.1.0/allianceauth/authentication/tests/test_signals.py
+-rw-r--r--   0        0        0    10730 2024-05-27 04:40:28.811463 allianceauth-4.1.0/allianceauth/authentication/tests/test_templatetags.py
+-rw-r--r--   0        0        0     5865 2024-05-27 04:40:28.811463 allianceauth-4.1.0/allianceauth/authentication/tests/test_views.py
+-rw-r--r--   0        0        0     1170 2024-05-27 04:40:28.811463 allianceauth-4.1.0/allianceauth/authentication/urls.py
+-rw-r--r--   0        0        0    14250 2024-05-27 04:40:28.811463 allianceauth-4.1.0/allianceauth/authentication/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.969463 allianceauth-4.1.0/allianceauth/bin/__init__.py
+-rw-r--r--   0        0        0     3680 2024-05-27 04:40:28.811463 allianceauth-4.1.0/allianceauth/bin/allianceauth.py
+-rw-r--r--   0        0        0      274 2024-05-27 04:40:28.811463 allianceauth-4.1.0/allianceauth/context_processors.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.969463 allianceauth-4.1.0/allianceauth/corputils/__init__.py
+-rw-r--r--   0        0        0      140 2024-05-27 04:40:28.811463 allianceauth-4.1.0/allianceauth/corputils/admin.py
+-rw-r--r--   0        0        0      130 2024-05-27 04:40:28.811463 allianceauth-4.1.0/allianceauth/corputils/apps.py
+-rw-r--r--   0        0        0     1043 2024-05-27 04:40:28.811463 allianceauth-4.1.0/allianceauth/corputils/auth_hooks.py
+-rw-r--r--   0        0        0     1970 2024-05-27 04:40:28.811463 allianceauth-4.1.0/allianceauth/corputils/managers.py
+-rw-r--r--   0        0        0     1417 2024-05-27 04:40:28.811463 allianceauth-4.1.0/allianceauth/corputils/migrations/0001_initial.py
+-rw-r--r--   0        0        0     5358 2024-05-27 04:40:28.812464 allianceauth-4.1.0/allianceauth/corputils/migrations/0002_migrate_permissions.py
+-rw-r--r--   0        0        0      844 2024-05-27 04:40:28.812464 allianceauth-4.1.0/allianceauth/corputils/migrations/0003_granular_permissions.py
+-rw-r--r--   0        0        0     2029 2024-05-27 04:40:28.812464 allianceauth-4.1.0/allianceauth/corputils/migrations/0004_member_models.py
+-rw-r--r--   0        0        0     1516 2024-05-27 04:40:28.812464 allianceauth-4.1.0/allianceauth/corputils/migrations/0005_cleanup_permissions.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.969463 allianceauth-4.1.0/allianceauth/corputils/migrations/__init__.py
+-rw-r--r--   0        0        0     7223 2024-05-27 04:40:28.812464 allianceauth-4.1.0/allianceauth/corputils/models.py
+-rw-r--r--   0        0        0   947431 2024-05-27 04:40:28.815463 allianceauth-4.1.0/allianceauth/corputils/swagger.json
+-rw-r--r--   0        0        0      298 2024-05-27 04:40:28.815463 allianceauth-4.1.0/allianceauth/corputils/tasks.py
+-rw-r--r--   0        0        0     1991 2024-05-27 04:40:28.815463 allianceauth-4.1.0/allianceauth/corputils/templates/corputils/base.html
+-rw-r--r--   0        0        0    14560 2024-05-27 04:40:28.815463 allianceauth-4.1.0/allianceauth/corputils/templates/corputils/corpstats.html
+-rw-r--r--   0        0        0     2268 2024-05-27 04:40:28.815463 allianceauth-4.1.0/allianceauth/corputils/templates/corputils/search.html
+-rw-r--r--   0        0        0    16016 2024-05-27 04:40:28.815463 allianceauth-4.1.0/allianceauth/corputils/tests.py
+-rw-r--r--   0        0        0      393 2024-05-27 04:40:28.816464 allianceauth-4.1.0/allianceauth/corputils/urls.py
+-rw-r--r--   0        0        0     6999 2024-05-27 04:40:28.816464 allianceauth-4.1.0/allianceauth/corputils/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.969463 allianceauth-4.1.0/allianceauth/eveonline/__init__.py
+-rw-r--r--   0        0        0     7277 2024-05-27 04:40:28.816464 allianceauth-4.1.0/allianceauth/eveonline/admin.py
+-rw-r--r--   0        0        0      130 2024-05-27 04:40:28.816464 allianceauth-4.1.0/allianceauth/eveonline/apps.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.969463 allianceauth-4.1.0/allianceauth/eveonline/autogroups/__init__.py
+-rw-r--r--   0        0        0     1320 2024-05-27 04:40:28.816464 allianceauth-4.1.0/allianceauth/eveonline/autogroups/admin.py
+-rw-r--r--   0        0        0      229 2024-05-27 04:40:28.816464 allianceauth-4.1.0/allianceauth/eveonline/autogroups/apps.py
+-rw-r--r--   0        0        0     4024 2024-05-27 04:40:28.816464 allianceauth-4.1.0/allianceauth/eveonline/autogroups/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.969463 allianceauth-4.1.0/allianceauth/eveonline/autogroups/migrations/__init__.py
+-rw-r--r--   0        0        0    10691 2024-05-27 04:40:28.817463 allianceauth-4.1.0/allianceauth/eveonline/autogroups/models.py
+-rw-r--r--   0        0        0     2625 2024-05-27 04:40:28.817463 allianceauth-4.1.0/allianceauth/eveonline/autogroups/signals.py
+-rw-r--r--   0        0        0     1403 2024-05-27 04:40:28.817463 allianceauth-4.1.0/allianceauth/eveonline/autogroups/tests/__init__.py
+-rw-r--r--   0        0        0     3221 2024-05-27 04:40:28.817463 allianceauth-4.1.0/allianceauth/eveonline/autogroups/tests/test_managers.py
+-rw-r--r--   0        0        0    12334 2024-05-27 04:40:28.817463 allianceauth-4.1.0/allianceauth/eveonline/autogroups/tests/test_models.py
+-rw-r--r--   0        0        0     7961 2024-05-27 04:40:28.817463 allianceauth-4.1.0/allianceauth/eveonline/autogroups/tests/test_signals.py
+-rw-r--r--   0        0        0      646 2024-05-27 04:40:28.817463 allianceauth-4.1.0/allianceauth/eveonline/evelinks/__init__.py
+-rw-r--r--   0        0        0     1496 2024-05-27 04:40:28.817463 allianceauth-4.1.0/allianceauth/eveonline/evelinks/dotlan.py
+-rw-r--r--   0        0        0     3730 2024-05-27 04:40:28.817463 allianceauth-4.1.0/allianceauth/eveonline/evelinks/eveimageserver.py
+-rw-r--r--   0        0        0     1229 2024-05-27 04:40:28.817463 allianceauth-4.1.0/allianceauth/eveonline/evelinks/evewho.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.969463 allianceauth-4.1.0/allianceauth/eveonline/evelinks/tests/__init__.py
+-rw-r--r--   0        0        0     7329 2024-05-27 04:40:28.818463 allianceauth-4.1.0/allianceauth/eveonline/evelinks/tests/test_evelinks.py
+-rw-r--r--   0        0        0    11505 2024-05-27 04:40:28.818463 allianceauth-4.1.0/allianceauth/eveonline/evelinks/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1700 2024-05-27 04:40:28.818463 allianceauth-4.1.0/allianceauth/eveonline/evelinks/zkillboard.py
+-rw-r--r--   0        0        0     3350 2024-05-27 04:40:28.818463 allianceauth-4.1.0/allianceauth/eveonline/managers.py
+-rw-r--r--   0        0        0     3133 2024-05-27 04:40:28.818463 allianceauth-4.1.0/allianceauth/eveonline/migrations/0001_initial.py
+-rw-r--r--   0        0        0      332 2024-05-27 04:40:28.818463 allianceauth-4.1.0/allianceauth/eveonline/migrations/0002_remove_eveapikeypair_error_count.py
+-rw-r--r--   0        0        0      797 2024-05-27 04:40:28.818463 allianceauth-4.1.0/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py
+-rw-r--r--   0        0        0      403 2024-05-27 04:40:28.818463 allianceauth-4.1.0/allianceauth/eveonline/migrations/0004_eveapikeypair_sso_verified.py
+-rw-r--r--   0        0        0      354 2024-05-27 04:40:28.818463 allianceauth-4.1.0/allianceauth/eveonline/migrations/0005_remove_eveallianceinfo_member_count.py
+-rw-r--r--   0        0        0      655 2024-05-27 04:40:28.818463 allianceauth-4.1.0/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py
+-rw-r--r--   0        0        0     4599 2024-05-27 04:40:28.818463 allianceauth-4.1.0/allianceauth/eveonline/migrations/0007_unique_id_name.py
+-rw-r--r--   0        0        0      854 2024-05-27 04:40:28.818463 allianceauth-4.1.0/allianceauth/eveonline/migrations/0008_remove_apikeys.py
+-rw-r--r--   0        0        0      519 2024-05-27 04:40:28.819464 allianceauth-4.1.0/allianceauth/eveonline/migrations/0009_on_delete.py
+-rw-r--r--   0        0        0      596 2024-05-27 04:40:28.819464 allianceauth-4.1.0/allianceauth/eveonline/migrations/0010_alliance_ticker.py
+-rw-r--r--   0        0        0     1297 2024-05-27 04:40:28.819464 allianceauth-4.1.0/allianceauth/eveonline/migrations/0011_ids_to_integers.py
+-rw-r--r--   0        0        0     1121 2024-05-27 04:40:28.819464 allianceauth-4.1.0/allianceauth/eveonline/migrations/0012_index_additions.py
+-rw-r--r--   0        0        0      428 2024-05-27 04:40:28.819464 allianceauth-4.1.0/allianceauth/eveonline/migrations/0013_evecorporationinfo_ceo_id.py
+-rw-r--r--   0        0        0      416 2024-05-27 04:40:28.819464 allianceauth-4.1.0/allianceauth/eveonline/migrations/0014_auto_20210105_1413.py
+-rw-r--r--   0        0        0     1201 2024-05-27 04:40:28.819464 allianceauth-4.1.0/allianceauth/eveonline/migrations/0015_factions.py
+-rw-r--r--   0        0        0      409 2024-05-27 04:40:28.819464 allianceauth-4.1.0/allianceauth/eveonline/migrations/0016_character_names_are_not_unique.py
+-rw-r--r--   0        0        0      623 2024-05-27 04:40:28.819464 allianceauth-4.1.0/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.969463 allianceauth-4.1.0/allianceauth/eveonline/migrations/__init__.py
+-rw-r--r--   0        0        0    14052 2024-05-27 04:40:28.819464 allianceauth-4.1.0/allianceauth/eveonline/models.py
+-rw-r--r--   0        0        0     9958 2024-05-27 04:40:28.819464 allianceauth-4.1.0/allianceauth/eveonline/providers.py
+-rw-r--r--   0        0        0    41989 2024-05-27 04:40:28.819464 allianceauth-4.1.0/allianceauth/eveonline/swagger.json
+-rw-r--r--   0        0        0     3808 2024-05-27 04:40:28.820464 allianceauth-4.1.0/allianceauth/eveonline/tasks.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.969463 allianceauth-4.1.0/allianceauth/eveonline/templatetags/__init__.py
+-rw-r--r--   0        0        0     8354 2024-05-27 04:40:28.820464 allianceauth-4.1.0/allianceauth/eveonline/templatetags/evelinks.py
+-rw-r--r--   0        0        0     4194 2024-05-27 04:40:28.820464 allianceauth-4.1.0/allianceauth/eveonline/templatetags/examples.html
+-rw-r--r--   0        0        0      739 2024-05-27 04:40:28.820464 allianceauth-4.1.0/allianceauth/eveonline/tests/__init__.py
+-rw-r--r--   0        0        0     6043 2024-05-27 04:40:28.820464 allianceauth-4.1.0/allianceauth/eveonline/tests/esi_client_stub.py
+-rw-r--r--   0        0        0   297070 2024-05-27 04:40:28.821463 allianceauth-4.1.0/allianceauth/eveonline/tests/swagger_old.json
+-rw-r--r--   0        0        0    10079 2024-05-27 04:40:28.821463 allianceauth-4.1.0/allianceauth/eveonline/tests/test_managers.py
+-rw-r--r--   0        0        0    23361 2024-05-27 04:40:28.821463 allianceauth-4.1.0/allianceauth/eveonline/tests/test_models.py
+-rw-r--r--   0        0        0    23834 2024-05-27 04:40:28.821463 allianceauth-4.1.0/allianceauth/eveonline/tests/test_providers.py
+-rw-r--r--   0        0        0    10117 2024-05-27 04:40:28.821463 allianceauth-4.1.0/allianceauth/eveonline/tests/test_tasks.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.969463 allianceauth-4.1.0/allianceauth/eveonline/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.969463 allianceauth-4.1.0/allianceauth/fleetactivitytracking/__init__.py
+-rw-r--r--   0        0        0      156 2024-05-27 04:40:28.822464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/admin.py
+-rw-r--r--   0        0        0      148 2024-05-27 04:40:28.822464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/apps.py
+-rw-r--r--   0        0        0      494 2024-05-27 04:40:28.822464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/auth_hooks.py
+-rw-r--r--   0        0        0      360 2024-05-27 04:40:28.822464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/forms.py
+-rw-r--r--   0        0        0     2291 2024-05-27 04:40:28.822464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/migrations/0001_initial.py
+-rw-r--r--   0        0        0      489 2024-05-27 04:40:28.822464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/migrations/0002_auto_20160905_2220.py
+-rw-r--r--   0        0        0      460 2024-05-27 04:40:28.822464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/migrations/0003_auto_20160906_2354.py
+-rw-r--r--   0        0        0      414 2024-05-27 04:40:28.822464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/migrations/0004_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      510 2024-05-27 04:40:28.822464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/migrations/0005_remove_fat_name.py
+-rw-r--r--   0        0        0      397 2024-05-27 04:40:28.822464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/migrations/0006_auto_20180803_0430.py
+-rw-r--r--   0        0        0      606 2024-05-27 04:40:28.822464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/migrations/0007_sentinel_user.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.973463 allianceauth-4.1.0/allianceauth/fleetactivitytracking/migrations/__init__.py
+-rw-r--r--   0        0        0     1122 2024-05-27 04:40:28.822464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/models.py
+-rw-r--r--   0        0        0   947431 2024-05-27 04:40:28.825463 allianceauth-4.1.0/allianceauth/fleetactivitytracking/swagger.json
+-rw-r--r--   0        0        0     1851 2024-05-27 04:40:28.825463 allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html
+-rw-r--r--   0        0        0     1880 2024-05-27 04:40:28.825463 allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkcreate.html
+-rw-r--r--   0        0        0     2811 2024-05-27 04:40:28.825463 allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html
+-rw-r--r--   0        0        0     4516 2024-05-27 04:40:28.825463 allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html
+-rw-r--r--   0        0        0     1725 2024-05-27 04:40:28.826464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html
+-rw-r--r--   0        0        0     2730 2024-05-27 04:40:28.826464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html
+-rw-r--r--   0        0        0     3011 2024-05-27 04:40:28.826464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html
+-rw-r--r--   0        0        0     5912 2024-05-27 04:40:28.826464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html
+-rw-r--r--   0        0        0     1386 2024-05-27 04:40:28.826464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/urls.py
+-rw-r--r--   0        0        0    16656 2024-05-27 04:40:28.826464 allianceauth-4.1.0/allianceauth/fleetactivitytracking/views.py
+-rw-r--r--   0        0        0       32 2024-05-27 04:40:28.826464 allianceauth-4.1.0/allianceauth/framework/__init__.py
+-rw-r--r--   0        0        0     1421 2024-05-27 04:40:28.826464 allianceauth-4.1.0/allianceauth/framework/api/evecharacter.py
+-rw-r--r--   0        0        0     1723 2024-05-27 04:40:28.826464 allianceauth-4.1.0/allianceauth/framework/api/user.py
+-rw-r--r--   0        0        0      202 2024-05-27 04:40:28.826464 allianceauth-4.1.0/allianceauth/framework/apps.py
+-rw-r--r--   0        0        0     3174 2024-05-27 04:40:28.826464 allianceauth-4.1.0/allianceauth/framework/static/allianceauth/framework/css/auth-framework.css
+-rw-r--r--   0        0        0      209 2024-05-27 04:40:28.827463 allianceauth-4.1.0/allianceauth/framework/templates/framework/dashboard/widget-title.html
+-rw-r--r--   0        0        0      336 2024-05-27 04:40:28.827463 allianceauth-4.1.0/allianceauth/framework/templates/framework/header/page-header.html
+-rw-r--r--   0        0        0       31 2024-05-27 04:40:28.827463 allianceauth-4.1.0/allianceauth/framework/tests/__init__.py
+-rw-r--r--   0        0        0     4468 2024-05-27 04:40:28.827463 allianceauth-4.1.0/allianceauth/framework/tests/test_api_user.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.973463 allianceauth-4.1.0/allianceauth/groupmanagement/__init__.py
+-rw-r--r--   0        0        0     8978 2024-05-27 04:40:28.827463 allianceauth-4.1.0/allianceauth/groupmanagement/admin.py
+-rw-r--r--   0        0        0      252 2024-05-27 04:40:28.827463 allianceauth-4.1.0/allianceauth/groupmanagement/apps.py
+-rw-r--r--   0        0        0     2336 2024-05-27 04:40:28.827463 allianceauth-4.1.0/allianceauth/groupmanagement/auth_hooks.py
+-rw-r--r--   0        0        0     2466 2024-05-27 04:40:28.827463 allianceauth-4.1.0/allianceauth/groupmanagement/forms.py
+-rw-r--r--   0        0        0     4341 2024-05-27 04:40:28.827463 allianceauth-4.1.0/allianceauth/groupmanagement/managers.py
+-rw-r--r--   0        0        0     2243 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0001_initial.py
+-rw-r--r--   0        0        0      685 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py
+-rw-r--r--   0        0        0      261 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0003_default_groups.py
+-rw-r--r--   0        0        0     4322 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0004_authgroup.py
+-rw-r--r--   0        0        0      631 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0005_authgroup_public.py
+-rw-r--r--   0        0        0      607 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py
+-rw-r--r--   0        0        0      877 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0007_on_delete.py
+-rw-r--r--   0        0        0     1430 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py
+-rw-r--r--   0        0        0     1100 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0009_requestlog.py
+-rw-r--r--   0        0        0      614 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0010_authgroup_states.py
+-rw-r--r--   0        0        0      456 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0011_requestlog_date.py
+-rw-r--r--   0        0        0      672 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0012_group_leads.py
+-rw-r--r--   0        0        0      397 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0013_fix_requestlog_date_field.py
+-rw-r--r--   0        0        0      410 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0014_auto_20200918_1412.py
+-rw-r--r--   0        0        0      567 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py
+-rw-r--r--   0        0        0      353 2024-05-27 04:40:28.828463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0016_remove_grouprequest_status_field.py
+-rw-r--r--   0        0        0     2296 2024-05-27 04:40:28.829464 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py
+-rw-r--r--   0        0        0     1082 2024-05-27 04:40:28.829464 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py
+-rw-r--r--   0        0        0      520 2024-05-27 04:40:28.829464 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.980463 allianceauth-4.1.0/allianceauth/groupmanagement/migrations/__init__.py
+-rw-r--r--   0        0        0     8132 2024-05-27 04:40:28.829464 allianceauth-4.1.0/allianceauth/groupmanagement/models.py
+-rw-r--r--   0        0        0     1465 2024-05-27 04:40:28.829464 allianceauth-4.1.0/allianceauth/groupmanagement/signals.py
+-rw-r--r--   0        0        0      333 2024-05-27 04:40:28.829464 allianceauth-4.1.0/allianceauth/groupmanagement/tasks.py
+-rw-r--r--   0        0        0     4516 2024-05-27 04:40:28.829464 allianceauth-4.1.0/allianceauth/groupmanagement/templates/groupmanagement/audit.html
+-rw-r--r--   0        0        0     4003 2024-05-27 04:40:28.829464 allianceauth-4.1.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html
+-rw-r--r--   0        0        0     3764 2024-05-27 04:40:28.829464 allianceauth-4.1.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html
+-rw-r--r--   0        0        0     4854 2024-05-27 04:40:28.829464 allianceauth-4.1.0/allianceauth/groupmanagement/templates/groupmanagement/groups.html
+-rw-r--r--   0        0        0     8485 2024-05-27 04:40:28.829464 allianceauth-4.1.0/allianceauth/groupmanagement/templates/groupmanagement/index.html
+-rw-r--r--   0        0        0      445 2024-05-27 04:40:28.830464 allianceauth-4.1.0/allianceauth/groupmanagement/templates/groupmanagement/menu.html
+-rw-r--r--   0        0        0      254 2024-05-27 04:40:28.830464 allianceauth-4.1.0/allianceauth/groupmanagement/tests/__init__.py
+-rw-r--r--   0        0        0    27572 2024-05-27 04:40:28.830464 allianceauth-4.1.0/allianceauth/groupmanagement/tests/test_admin.py
+-rw-r--r--   0        0        0    17375 2024-05-27 04:40:28.830464 allianceauth-4.1.0/allianceauth/groupmanagement/tests/test_managers.py
+-rw-r--r--   0        0        0    11668 2024-05-27 04:40:28.830464 allianceauth-4.1.0/allianceauth/groupmanagement/tests/test_models.py
+-rw-r--r--   0        0        0     4950 2024-05-27 04:40:28.830464 allianceauth-4.1.0/allianceauth/groupmanagement/tests/test_signals.py
+-rw-r--r--   0        0        0     3999 2024-05-27 04:40:28.830464 allianceauth-4.1.0/allianceauth/groupmanagement/tests/test_views.py
+-rw-r--r--   0        0        0     1651 2024-05-27 04:40:28.830464 allianceauth-4.1.0/allianceauth/groupmanagement/urls.py
+-rw-r--r--   0        0        0    20437 2024-05-27 04:40:28.831463 allianceauth-4.1.0/allianceauth/groupmanagement/views.py
+-rw-r--r--   0        0        0     4570 2024-05-27 04:40:28.831463 allianceauth-4.1.0/allianceauth/hooks.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.984463 allianceauth-4.1.0/allianceauth/hrapplications/__init__.py
+-rw-r--r--   0        0        0      693 2024-05-27 04:40:28.831463 allianceauth-4.1.0/allianceauth/hrapplications/admin.py
+-rw-r--r--   0        0        0      145 2024-05-27 04:40:28.831463 allianceauth-4.1.0/allianceauth/hrapplications/apps.py
+-rw-r--r--   0        0        0     1023 2024-05-27 04:40:28.831463 allianceauth-4.1.0/allianceauth/hrapplications/auth_hooks.py
+-rw-r--r--   0        0        0      353 2024-05-27 04:40:28.831463 allianceauth-4.1.0/allianceauth/hrapplications/forms.py
+-rw-r--r--   0        0        0      900 2024-05-27 04:40:28.831463 allianceauth-4.1.0/allianceauth/hrapplications/managers.py
+-rw-r--r--   0        0        0     6662 2024-05-27 04:40:28.831463 allianceauth-4.1.0/allianceauth/hrapplications/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1036 2024-05-27 04:40:28.831463 allianceauth-4.1.0/allianceauth/hrapplications/migrations/0002_choices_for_questions.py
+-rw-r--r--   0        0        0      415 2024-05-27 04:40:28.831463 allianceauth-4.1.0/allianceauth/hrapplications/migrations/0003_applicationquestion_multi_select.py
+-rw-r--r--   0        0        0     1461 2024-05-27 04:40:28.831463 allianceauth-4.1.0/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      558 2024-05-27 04:40:28.832463 allianceauth-4.1.0/allianceauth/hrapplications/migrations/0005_sorted_questions.py
+-rw-r--r--   0        0        0     1946 2024-05-27 04:40:28.832463 allianceauth-4.1.0/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py
+-rw-r--r--   0        0        0      427 2024-05-27 04:40:28.832463 allianceauth-4.1.0/allianceauth/hrapplications/migrations/0007_auto_20200918_1412.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.984463 allianceauth-4.1.0/allianceauth/hrapplications/migrations/__init__.py
+-rw-r--r--   0        0        0     3237 2024-05-27 04:40:28.832463 allianceauth-4.1.0/allianceauth/hrapplications/models.py
+-rw-r--r--   0        0        0     1411 2024-05-27 04:40:28.832463 allianceauth-4.1.0/allianceauth/hrapplications/templates/hrapplications/corpchoice.html
+-rw-r--r--   0        0        0     2946 2024-05-27 04:40:28.832463 allianceauth-4.1.0/allianceauth/hrapplications/templates/hrapplications/create.html
+-rw-r--r--   0        0        0    12438 2024-05-27 04:40:28.832463 allianceauth-4.1.0/allianceauth/hrapplications/templates/hrapplications/management.html
+-rw-r--r--   0        0        0     1308 2024-05-27 04:40:28.832463 allianceauth-4.1.0/allianceauth/hrapplications/templates/hrapplications/partials/modals/search.html
+-rw-r--r--   0        0        0     2772 2024-05-27 04:40:28.833464 allianceauth-4.1.0/allianceauth/hrapplications/templates/hrapplications/searchview.html
+-rw-r--r--   0        0        0     8251 2024-05-27 04:40:28.833464 allianceauth-4.1.0/allianceauth/hrapplications/templates/hrapplications/view.html
+-rw-r--r--   0        0        0     4165 2024-05-27 04:40:28.833464 allianceauth-4.1.0/allianceauth/hrapplications/tests.py
+-rw-r--r--   0        0        0     1113 2024-05-27 04:40:28.833464 allianceauth-4.1.0/allianceauth/hrapplications/urls.py
+-rw-r--r--   0        0        0    12011 2024-05-27 04:40:28.833464 allianceauth-4.1.0/allianceauth/hrapplications/views.py
+-rw-r--r--   0        0        0     7262 2024-05-27 04:40:28.833464 allianceauth-4.1.0/allianceauth/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    85931 2024-05-27 04:40:28.834463 allianceauth-4.1.0/allianceauth/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    45125 2024-05-27 04:40:28.835463 allianceauth-4.1.0/allianceauth/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   100544 2024-05-27 04:40:28.835463 allianceauth-4.1.0/allianceauth/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2024-05-27 04:40:28.835463 allianceauth-4.1.0/allianceauth/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    83238 2024-05-27 04:40:28.836464 allianceauth-4.1.0/allianceauth/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    35108 2024-05-27 04:40:28.836464 allianceauth-4.1.0/allianceauth/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    96583 2024-05-27 04:40:28.836464 allianceauth-4.1.0/allianceauth/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    46059 2024-05-27 04:40:28.837463 allianceauth-4.1.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   101728 2024-05-27 04:40:28.837463 allianceauth-4.1.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    44568 2024-05-27 04:40:28.838463 allianceauth-4.1.0/allianceauth/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   100475 2024-05-27 04:40:28.838463 allianceauth-4.1.0/allianceauth/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    49616 2024-05-27 04:40:28.838463 allianceauth-4.1.0/allianceauth/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   104822 2024-05-27 04:40:28.839464 allianceauth-4.1.0/allianceauth/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    46390 2024-05-27 04:40:28.839464 allianceauth-4.1.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   101738 2024-05-27 04:40:28.839464 allianceauth-4.1.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17293 2024-05-27 04:40:28.840463 allianceauth-4.1.0/allianceauth/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    88812 2024-05-27 04:40:28.840463 allianceauth-4.1.0/allianceauth/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    45885 2024-05-27 04:40:28.840463 allianceauth-4.1.0/allianceauth/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   101247 2024-05-27 04:40:28.841463 allianceauth-4.1.0/allianceauth/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    45746 2024-05-27 04:40:28.841463 allianceauth-4.1.0/allianceauth/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   106362 2024-05-27 04:40:28.841463 allianceauth-4.1.0/allianceauth/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    57333 2024-05-27 04:40:28.842463 allianceauth-4.1.0/allianceauth/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   112781 2024-05-27 04:40:28.842463 allianceauth-4.1.0/allianceauth/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    26591 2024-05-27 04:40:28.842463 allianceauth-4.1.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    92036 2024-05-27 04:40:28.843464 allianceauth-4.1.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.985463 allianceauth-4.1.0/allianceauth/menu/__init__.py
+-rw-r--r--   0        0        0     3721 2024-05-27 04:40:28.843464 allianceauth-4.1.0/allianceauth/menu/admin.py
+-rw-r--r--   0        0        0      459 2024-05-27 04:40:28.843464 allianceauth-4.1.0/allianceauth/menu/apps.py
+-rw-r--r--   0        0        0      485 2024-05-27 04:40:28.843464 allianceauth-4.1.0/allianceauth/menu/constants.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.985463 allianceauth-4.1.0/allianceauth/menu/core/__init__.py
+-rw-r--r--   0        0        0     1363 2024-05-27 04:40:28.843464 allianceauth-4.1.0/allianceauth/menu/core/menu_item_hooks.py
+-rw-r--r--   0        0        0      892 2024-05-27 04:40:28.843464 allianceauth-4.1.0/allianceauth/menu/core/smart_sync.py
+-rw-r--r--   0        0        0      688 2024-05-27 04:40:28.843464 allianceauth-4.1.0/allianceauth/menu/filters.py
+-rw-r--r--   0        0        0     1397 2024-05-27 04:40:28.843464 allianceauth-4.1.0/allianceauth/menu/forms.py
+-rw-r--r--   0        0        0     1932 2024-05-27 04:40:28.843464 allianceauth-4.1.0/allianceauth/menu/hooks.py
+-rw-r--r--   0        0        0     2288 2024-05-27 04:40:28.843464 allianceauth-4.1.0/allianceauth/menu/managers.py
+-rw-r--r--   0        0        0     3143 2024-05-27 04:40:28.844463 allianceauth-4.1.0/allianceauth/menu/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.985463 allianceauth-4.1.0/allianceauth/menu/migrations/__init__.py
+-rw-r--r--   0        0        0     4094 2024-05-27 04:40:28.844463 allianceauth-4.1.0/allianceauth/menu/models.py
+-rw-r--r--   0        0        0      289 2024-05-27 04:40:28.844463 allianceauth-4.1.0/allianceauth/menu/templates/admin/menu/menuitem/change_list.html
+-rw-r--r--   0        0        0       62 2024-05-27 04:40:28.844463 allianceauth-4.1.0/allianceauth/menu/templates/menu/menu-block.html
+-rw-r--r--   0        0        0     2009 2024-05-27 04:40:28.844463 allianceauth-4.1.0/allianceauth/menu/templates/menu/menu-item-bs5.html
+-rw-r--r--   0        0        0      101 2024-05-27 04:40:28.844463 allianceauth-4.1.0/allianceauth/menu/templates/menu/menu-logo.html
+-rw-r--r--   0        0        0      535 2024-05-27 04:40:28.844463 allianceauth-4.1.0/allianceauth/menu/templates/menu/menu-notification-block.html
+-rw-r--r--   0        0        0     5103 2024-05-27 04:40:28.844463 allianceauth-4.1.0/allianceauth/menu/templates/menu/menu-user.html
+-rw-r--r--   0        0        0     1308 2024-05-27 04:40:28.844463 allianceauth-4.1.0/allianceauth/menu/templates/menu/sortable-side-menu.html
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.985463 allianceauth-4.1.0/allianceauth/menu/templatetags/__init__.py
+-rw-r--r--   0        0        0      893 2024-05-27 04:40:28.844463 allianceauth-4.1.0/allianceauth/menu/templatetags/menu_items.py
+-rw-r--r--   0        0        0     5996 2024-05-27 04:40:28.845463 allianceauth-4.1.0/allianceauth/menu/templatetags/menu_menu_items.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.985463 allianceauth-4.1.0/allianceauth/menu/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.985463 allianceauth-4.1.0/allianceauth/menu/tests/core/__init__.py
+-rw-r--r--   0        0        0     1799 2024-05-27 04:40:28.845463 allianceauth-4.1.0/allianceauth/menu/tests/core/test_menu_item_hooks.py
+-rw-r--r--   0        0        0     1153 2024-05-27 04:40:28.845463 allianceauth-4.1.0/allianceauth/menu/tests/core/test_smart_sync.py
+-rw-r--r--   0        0        0     2763 2024-05-27 04:40:28.845463 allianceauth-4.1.0/allianceauth/menu/tests/factories.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.985463 allianceauth-4.1.0/allianceauth/menu/tests/integration/__init__.py
+-rw-r--r--   0        0        0     6367 2024-05-27 04:40:28.845463 allianceauth-4.1.0/allianceauth/menu/tests/integration/test_admin.py
+-rw-r--r--   0        0        0     3736 2024-05-27 04:40:28.845463 allianceauth-4.1.0/allianceauth/menu/tests/integration/test_dashboard.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.985463 allianceauth-4.1.0/allianceauth/menu/tests/templatetags/__init__.py
+-rw-r--r--   0        0        0     1688 2024-05-27 04:40:28.845463 allianceauth-4.1.0/allianceauth/menu/tests/templatetags/test_menu_items.py
+-rw-r--r--   0        0        0    11656 2024-05-27 04:40:28.845463 allianceauth-4.1.0/allianceauth/menu/tests/templatetags/test_menu_menu_items.py
+-rw-r--r--   0        0        0      833 2024-05-27 04:40:28.846464 allianceauth-4.1.0/allianceauth/menu/tests/test_forms.py
+-rw-r--r--   0        0        0     2511 2024-05-27 04:40:28.846464 allianceauth-4.1.0/allianceauth/menu/tests/test_hooks.py
+-rw-r--r--   0        0        0     3470 2024-05-27 04:40:28.846464 allianceauth-4.1.0/allianceauth/menu/tests/test_managers.py
+-rw-r--r--   0        0        0     4831 2024-05-27 04:40:28.846464 allianceauth-4.1.0/allianceauth/menu/tests/test_models.py
+-rw-r--r--   0        0        0     1177 2024-05-27 04:40:28.846464 allianceauth-4.1.0/allianceauth/menu/tests/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.985463 allianceauth-4.1.0/allianceauth/models.py
+-rw-r--r--   0        0        0       39 2024-05-27 04:40:28.846464 allianceauth-4.1.0/allianceauth/notifications/__init__.py
+-rw-r--r--   0        0        0     1138 2024-05-27 04:40:28.846464 allianceauth-4.1.0/allianceauth/notifications/admin.py
+-rw-r--r--   0        0        0      142 2024-05-27 04:40:28.846464 allianceauth-4.1.0/allianceauth/notifications/apps.py
+-rw-r--r--   0        0        0     1320 2024-05-27 04:40:28.846464 allianceauth-4.1.0/allianceauth/notifications/core.py
+-rw-r--r--   0        0        0      998 2024-05-27 04:40:28.846464 allianceauth-4.1.0/allianceauth/notifications/handlers.py
+-rw-r--r--   0        0        0     3907 2024-05-27 04:40:28.846464 allianceauth-4.1.0/allianceauth/notifications/managers.py
+-rw-r--r--   0        0        0     1117 2024-05-27 04:40:28.846464 allianceauth-4.1.0/allianceauth/notifications/migrations/0001_initial.py
+-rw-r--r--   0        0        0      353 2024-05-27 04:40:28.846464 allianceauth-4.1.0/allianceauth/notifications/migrations/0002_auto_20160910_1649.py
+-rw-r--r--   0        0        0      514 2024-05-27 04:40:28.846464 allianceauth-4.1.0/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      714 2024-05-27 04:40:28.847463 allianceauth-4.1.0/allianceauth/notifications/migrations/0004_performance_tuning.py
+-rw-r--r--   0        0        0      512 2024-05-27 04:40:28.847463 allianceauth-4.1.0/allianceauth/notifications/migrations/0005_fix_level_choices.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.994463 allianceauth-4.1.0/allianceauth/notifications/migrations/__init__.py
+-rw-r--r--   0        0        0     2772 2024-05-27 04:40:28.847463 allianceauth-4.1.0/allianceauth/notifications/models.py
+-rw-r--r--   0        0        0     1857 2024-05-27 04:40:28.847463 allianceauth-4.1.0/allianceauth/notifications/templates/notifications/list.html
+-rw-r--r--   0        0        0     1070 2024-05-27 04:40:28.847463 allianceauth-4.1.0/allianceauth/notifications/templates/notifications/list_partial.html
+-rw-r--r--   0        0        0      736 2024-05-27 04:40:28.847463 allianceauth-4.1.0/allianceauth/notifications/templates/notifications/view.html
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.994463 allianceauth-4.1.0/allianceauth/notifications/templatetags/__init__.py
+-rw-r--r--   0        0        0     1156 2024-05-27 04:40:28.847463 allianceauth-4.1.0/allianceauth/notifications/templatetags/auth_notifications.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.994463 allianceauth-4.1.0/allianceauth/notifications/tests/__init__.py
+-rw-r--r--   0        0        0     3073 2024-05-27 04:40:28.847463 allianceauth-4.1.0/allianceauth/notifications/tests/test_core.py
+-rw-r--r--   0        0        0     2392 2024-05-27 04:40:28.847463 allianceauth-4.1.0/allianceauth/notifications/tests/test_handlers.py
+-rw-r--r--   0        0        0     1120 2024-05-27 04:40:28.847463 allianceauth-4.1.0/allianceauth/notifications/tests/test_init.py
+-rw-r--r--   0        0        0     9437 2024-05-27 04:40:28.847463 allianceauth-4.1.0/allianceauth/notifications/tests/test_managers.py
+-rw-r--r--   0        0        0     2398 2024-05-27 04:40:28.848463 allianceauth-4.1.0/allianceauth/notifications/tests/test_models.py
+-rw-r--r--   0        0        0     2975 2024-05-27 04:40:28.848463 allianceauth-4.1.0/allianceauth/notifications/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1463 2024-05-27 04:40:28.848463 allianceauth-4.1.0/allianceauth/notifications/tests/test_views.py
+-rw-r--r--   0        0        0      674 2024-05-27 04:40:28.848463 allianceauth-4.1.0/allianceauth/notifications/urls.py
+-rw-r--r--   0        0        0     3522 2024-05-27 04:40:28.848463 allianceauth-4.1.0/allianceauth/notifications/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.994463 allianceauth-4.1.0/allianceauth/optimer/__init__.py
+-rw-r--r--   0        0        0      158 2024-05-27 04:40:28.848463 allianceauth-4.1.0/allianceauth/optimer/admin.py
+-rw-r--r--   0        0        0      124 2024-05-27 04:40:28.848463 allianceauth-4.1.0/allianceauth/optimer/apps.py
+-rw-r--r--   0        0        0     1183 2024-05-27 04:40:28.848463 allianceauth-4.1.0/allianceauth/optimer/auth_hooks.py
+-rw-r--r--   0        0        0     1368 2024-05-27 04:40:28.848463 allianceauth-4.1.0/allianceauth/optimer/form.py
+-rw-r--r--   0        0        0     1047 2024-05-27 04:40:28.848463 allianceauth-4.1.0/allianceauth/optimer/form_widgets.py
+-rw-r--r--   0        0        0     1452 2024-05-27 04:40:28.848463 allianceauth-4.1.0/allianceauth/optimer/migrations/0001_initial.py
+-rw-r--r--   0        0        0      424 2024-05-27 04:40:28.848463 allianceauth-4.1.0/allianceauth/optimer/migrations/0002_auto_20170413_0442.py
+-rw-r--r--   0        0        0     1076 2024-05-27 04:40:28.848463 allianceauth-4.1.0/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      507 2024-05-27 04:40:28.849463 allianceauth-4.1.0/allianceauth/optimer/migrations/0004_on_delete.py
+-rw-r--r--   0        0        0     1447 2024-05-27 04:40:28.849463 allianceauth-4.1.0/allianceauth/optimer/migrations/0005_add_type_and_description.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.994463 allianceauth-4.1.0/allianceauth/optimer/migrations/__init__.py
+-rw-r--r--   0        0        0     1247 2024-05-27 04:40:28.849463 allianceauth-4.1.0/allianceauth/optimer/models.py
+-rw-r--r--   0        0        0     1980 2024-05-27 04:40:28.849463 allianceauth-4.1.0/allianceauth/optimer/templates/optimer/add.html
+-rw-r--r--   0        0        0     1702 2024-05-27 04:40:28.849463 allianceauth-4.1.0/allianceauth/optimer/templates/optimer/dashboard.ops.html
+-rw-r--r--   0        0        0     2612 2024-05-27 04:40:28.849463 allianceauth-4.1.0/allianceauth/optimer/templates/optimer/fleetoptable.html
+-rw-r--r--   0        0        0     4378 2024-05-27 04:40:28.849463 allianceauth-4.1.0/allianceauth/optimer/templates/optimer/management.html
+-rw-r--r--   0        0        0     1986 2024-05-27 04:40:28.849463 allianceauth-4.1.0/allianceauth/optimer/templates/optimer/update.html
+-rw-r--r--   0        0        0       26 2024-05-27 04:40:28.849463 allianceauth-4.1.0/allianceauth/optimer/tests.py
+-rw-r--r--   0        0        0      336 2024-05-27 04:40:28.849463 allianceauth-4.1.0/allianceauth/optimer/urls.py
+-rw-r--r--   0        0        0     7139 2024-05-27 04:40:28.849463 allianceauth-4.1.0/allianceauth/optimer/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.994463 allianceauth-4.1.0/allianceauth/permissions_tool/__init__.py
+-rw-r--r--   0        0        0      150 2024-05-27 04:40:28.850463 allianceauth-4.1.0/allianceauth/permissions_tool/apps.py
+-rw-r--r--   0        0        0      821 2024-05-27 04:40:28.850463 allianceauth-4.1.0/allianceauth/permissions_tool/auth_hooks.py
+-rw-r--r--   0        0        0      589 2024-05-27 04:40:28.850463 allianceauth-4.1.0/allianceauth/permissions_tool/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.999463 allianceauth-4.1.0/allianceauth/permissions_tool/migrations/__init__.py
+-rw-r--r--   0        0        0      258 2024-05-27 04:40:28.850463 allianceauth-4.1.0/allianceauth/permissions_tool/models.py
+-rw-r--r--   0        0        0     3874 2024-05-27 04:40:28.850463 allianceauth-4.1.0/allianceauth/permissions_tool/templates/permissions_tool/audit.html
+-rw-r--r--   0        0        0      789 2024-05-27 04:40:28.850463 allianceauth-4.1.0/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html
+-rw-r--r--   0        0        0     4553 2024-05-27 04:40:28.850463 allianceauth-4.1.0/allianceauth/permissions_tool/templates/permissions_tool/overview.html
+-rw-r--r--   0        0        0     5067 2024-05-27 04:40:28.850463 allianceauth-4.1.0/allianceauth/permissions_tool/tests.py
+-rw-r--r--   0        0        0      340 2024-05-27 04:40:28.850463 allianceauth-4.1.0/allianceauth/permissions_tool/urls.py
+-rw-r--r--   0        0        0     2610 2024-05-27 04:40:28.850463 allianceauth-4.1.0/allianceauth/permissions_tool/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.999463 allianceauth-4.1.0/allianceauth/project_template/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.999463 allianceauth-4.1.0/allianceauth/project_template/log/.gitkeep
+-rw-r--r--   0        0        0      821 2024-05-27 04:40:28.851463 allianceauth-4.1.0/allianceauth/project_template/manage.py
+-rw-r--r--   0        0        0       38 2024-05-27 04:40:28.851463 allianceauth-4.1.0/allianceauth/project_template/project_name/__init__.py
+-rw-r--r--   0        0        0     1417 2024-05-27 04:40:28.851463 allianceauth-4.1.0/allianceauth/project_template/project_name/celery.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.999463 allianceauth-4.1.0/allianceauth/project_template/project_name/settings/__init__.py
+-rw-r--r--   0        0        0     9169 2024-05-27 04:40:28.851463 allianceauth-4.1.0/allianceauth/project_template/project_name/settings/base.py
+-rw-r--r--   0        0        0     3260 2024-05-27 04:40:28.851463 allianceauth-4.1.0/allianceauth/project_template/project_name/settings/local.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.999463 allianceauth-4.1.0/allianceauth/project_template/project_name/static/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.999463 allianceauth-4.1.0/allianceauth/project_template/project_name/templates/.gitkeep
+-rw-r--r--   0        0        0      329 2024-05-27 04:40:28.851463 allianceauth-4.1.0/allianceauth/project_template/project_name/urls.py
+-rw-r--r--   0        0        0      432 2024-05-27 04:40:28.851463 allianceauth-4.1.0/allianceauth/project_template/project_name/wsgi.py
+-rw-r--r--   0        0        0     1408 2024-05-27 04:40:28.851463 allianceauth-4.1.0/allianceauth/project_template/supervisor.conf
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.999463 allianceauth-4.1.0/allianceauth/services/__init__.py
+-rw-r--r--   0        0        0     3954 2024-05-27 04:40:28.852463 allianceauth-4.1.0/allianceauth/services/abstract.py
+-rw-r--r--   0        0        0     2162 2024-05-27 04:40:28.852463 allianceauth-4.1.0/allianceauth/services/admin.py
+-rw-r--r--   0        0        0      179 2024-05-27 04:40:28.852463 allianceauth-4.1.0/allianceauth/services/apps.py
+-rw-r--r--   0        0        0      662 2024-05-27 04:40:28.852463 allianceauth-4.1.0/allianceauth/services/auth_hooks.py
+-rw-r--r--   0        0        0     2117 2024-05-27 04:40:28.852463 allianceauth-4.1.0/allianceauth/services/forms.py
+-rw-r--r--   0        0        0     9149 2024-05-27 04:40:28.852463 allianceauth-4.1.0/allianceauth/services/hooks.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.999463 allianceauth-4.1.0/allianceauth/services/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.999463 allianceauth-4.1.0/allianceauth/services/management/commands/__init__.py
+-rw-r--r--   0        0        0      469 2024-05-27 04:40:28.852463 allianceauth-4.1.0/allianceauth/services/management/commands/verify_service_accounts.py
+-rw-r--r--   0        0        0      483 2024-05-27 04:40:28.852463 allianceauth-4.1.0/allianceauth/services/migrations/0001_squashed_0003_delete_groupcache.py
+-rw-r--r--   0        0        0     1220 2024-05-27 04:40:28.852463 allianceauth-4.1.0/allianceauth/services/migrations/0002_nameformatter.py
+-rw-r--r--   0        0        0      522 2024-05-27 04:40:28.852463 allianceauth-4.1.0/allianceauth/services/migrations/0003_remove_broken_link.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.999463 allianceauth-4.1.0/allianceauth/services/migrations/__init__.py
+-rw-r--r--   0        0        0     1000 2024-05-27 04:40:28.852463 allianceauth-4.1.0/allianceauth/services/models.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.999463 allianceauth-4.1.0/allianceauth/services/modules/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-27 04:40:28.853464 allianceauth-4.1.0/allianceauth/services/modules/discord/__init__.py
+-rw-r--r--   0        0        0     1070 2024-05-27 04:40:28.853464 allianceauth-4.1.0/allianceauth/services/modules/discord/admin.py
+-rw-r--r--   0        0        0     1290 2024-05-27 04:40:28.853464 allianceauth-4.1.0/allianceauth/services/modules/discord/api.py
+-rw-r--r--   0        0        0     1062 2024-05-27 04:40:28.853464 allianceauth-4.1.0/allianceauth/services/modules/discord/app_settings.py
+-rw-r--r--   0        0        0      148 2024-05-27 04:40:28.853464 allianceauth-4.1.0/allianceauth/services/modules/discord/apps.py
+-rw-r--r--   0        0        0     5974 2024-05-27 04:40:28.853464 allianceauth-4.1.0/allianceauth/services/modules/discord/auth_hooks.py
+-rw-r--r--   0        0        0     4446 2024-05-27 04:40:28.853464 allianceauth-4.1.0/allianceauth/services/modules/discord/core.py
+-rw-r--r--   0        0        0      372 2024-05-27 04:40:28.853464 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/__init__.py
+-rw-r--r--   0        0        0     1681 2024-05-27 04:40:28.853464 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/app_settings.py
+-rw-r--r--   0        0        0    28997 2024-05-27 04:40:28.853464 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/client.py
+-rw-r--r--   0        0        0     1009 2024-05-27 04:40:28.853464 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/exceptions.py
+-rw-r--r--   0        0        0     4590 2024-05-27 04:40:28.854463 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/helpers.py
+-rw-r--r--   0        0        0     3853 2024-05-27 04:40:28.854463 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/models.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.999463 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/__init__.py
+-rw-r--r--   0        0        0     5027 2024-05-27 04:40:28.854463 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/example_objects.json
+-rw-r--r--   0        0        0     3013 2024-05-27 04:40:28.854463 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/factories.py
+-rw-r--r--   0        0        0     2784 2024-05-27 04:40:28.854463 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py
+-rw-r--r--   0        0        0     4477 2024-05-27 04:40:28.854463 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py
+-rw-r--r--   0        0        0      904 2024-05-27 04:40:28.854463 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md
+-rw-r--r--   0        0        0    56114 2024-05-27 04:40:28.854463 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/test_client.py
+-rw-r--r--   0        0        0     1045 2024-05-27 04:40:28.854463 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py
+-rw-r--r--   0        0        0     9724 2024-05-27 04:40:28.854463 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py
+-rw-r--r--   0        0        0     4966 2024-05-27 04:40:28.855463 allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/test_models.py
+-rw-r--r--   0        0        0     6281 2024-05-27 04:40:28.855463 allianceauth-4.1.0/allianceauth/services/modules/discord/managers.py
+-rw-r--r--   0        0        0      680 2024-05-27 04:40:28.855463 allianceauth-4.1.0/allianceauth/services/modules/discord/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2067 2024-05-27 04:40:28.855463 allianceauth-4.1.0/allianceauth/services/modules/discord/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0     1538 2024-05-27 04:40:28.855463 allianceauth-4.1.0/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.999463 allianceauth-4.1.0/allianceauth/services/modules/discord/migrations/__init__.py
+-rw-r--r--   0        0        0     7138 2024-05-27 04:40:28.855463 allianceauth-4.1.0/allianceauth/services/modules/discord/models.py
+-rw-r--r--   0        0        0     9517 2024-05-27 04:40:28.855463 allianceauth-4.1.0/allianceauth/services/modules/discord/tasks.py
+-rw-r--r--   0        0        0     1508 2024-05-27 04:40:28.855463 allianceauth-4.1.0/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html
+-rw-r--r--   0        0        0      480 2024-05-27 04:40:28.855463 allianceauth-4.1.0/allianceauth/services/modules/discord/tests/__init__.py
+-rw-r--r--   0        0        0      917 2024-05-27 04:40:28.856464 allianceauth-4.1.0/allianceauth/services/modules/discord/tests/factories.py
+-rw-r--r--   0        0        0     2639 2024-05-27 04:40:28.856464 allianceauth-4.1.0/allianceauth/services/modules/discord/tests/piloting_tasks.py
+-rw-r--r--   0        0        0    10400 2024-05-27 04:40:28.856464 allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_admin.py
+-rw-r--r--   0        0        0      525 2024-05-27 04:40:28.856464 allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_api.py
+-rw-r--r--   0        0        0     7200 2024-05-27 04:40:28.856464 allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     8456 2024-05-27 04:40:28.856464 allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_core.py
+-rw-r--r--   0        0        0    29715 2024-05-27 04:40:28.856464 allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_integration.py
+-rw-r--r--   0        0        0    19956 2024-05-27 04:40:28.856464 allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_managers.py
+-rw-r--r--   0        0        0    11474 2024-05-27 04:40:28.856464 allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_models.py
+-rw-r--r--   0        0        0    17995 2024-05-27 04:40:28.856464 allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_tasks.py
+-rw-r--r--   0        0        0     3201 2024-05-27 04:40:28.857463 allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_utils.py
+-rw-r--r--   0        0        0     6783 2024-05-27 04:40:28.857463 allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_views.py
+-rw-r--r--   0        0        0      538 2024-05-27 04:40:28.857463 allianceauth-4.1.0/allianceauth/services/modules/discord/urls.py
+-rw-r--r--   0        0        0     2561 2024-05-27 04:40:28.857463 allianceauth-4.1.0/allianceauth/services/modules/discord/utils.py
+-rw-r--r--   0        0        0     3635 2024-05-27 04:40:28.857463 allianceauth-4.1.0/allianceauth/services/modules/discord/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:28.999463 allianceauth-4.1.0/allianceauth/services/modules/discourse/__init__.py
+-rw-r--r--   0        0        0      264 2024-05-27 04:40:28.857463 allianceauth-4.1.0/allianceauth/services/modules/discourse/admin.py
+-rw-r--r--   0        0        0      154 2024-05-27 04:40:28.857463 allianceauth-4.1.0/allianceauth/services/modules/discourse/apps.py
+-rw-r--r--   0        0        0     1878 2024-05-27 04:40:28.857463 allianceauth-4.1.0/allianceauth/services/modules/discourse/auth_hooks.py
+-rw-r--r--   0        0        0     7039 2024-05-27 04:40:28.857463 allianceauth-4.1.0/allianceauth/services/modules/discourse/manager.py
+-rw-r--r--   0        0        0      677 2024-05-27 04:40:28.857463 allianceauth-4.1.0/allianceauth/services/modules/discourse/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2096 2024-05-27 04:40:28.857463 allianceauth-4.1.0/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.000463 allianceauth-4.1.0/allianceauth/services/modules/discourse/migrations/__init__.py
+-rw-r--r--   0        0        0      529 2024-05-27 04:40:28.858463 allianceauth-4.1.0/allianceauth/services/modules/discourse/models.py
+-rw-r--r--   0        0        0      533 2024-05-27 04:40:28.858463 allianceauth-4.1.0/allianceauth/services/modules/discourse/providers.py
+-rw-r--r--   0        0        0     2276 2024-05-27 04:40:28.858463 allianceauth-4.1.0/allianceauth/services/modules/discourse/tasks.py
+-rw-r--r--   0        0        0      663 2024-05-27 04:40:28.858463 allianceauth-4.1.0/allianceauth/services/modules/discourse/templates/services/discourse/discourse_service_ctrl.html
+-rw-r--r--   0        0        0     5209 2024-05-27 04:40:28.858463 allianceauth-4.1.0/allianceauth/services/modules/discourse/tests.py
+-rw-r--r--   0        0        0      176 2024-05-27 04:40:28.858463 allianceauth-4.1.0/allianceauth/services/modules/discourse/urls.py
+-rw-r--r--   0        0        0     3486 2024-05-27 04:40:28.858463 allianceauth-4.1.0/allianceauth/services/modules/discourse/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.000463 allianceauth-4.1.0/allianceauth/services/modules/example/__init__.py
+-rw-r--r--   0        0        0      156 2024-05-27 04:40:28.858463 allianceauth-4.1.0/allianceauth/services/modules/example/apps.py
+-rw-r--r--   0        0        0     1336 2024-05-27 04:40:28.858463 allianceauth-4.1.0/allianceauth/services/modules/example/auth_hooks.py
+-rw-r--r--   0        0        0      411 2024-05-27 04:40:28.858463 allianceauth-4.1.0/allianceauth/services/modules/example/models.py
+-rw-r--r--   0        0        0      206 2024-05-27 04:40:28.858463 allianceauth-4.1.0/allianceauth/services/modules/example/urls.py
+-rw-r--r--   0        0        0       22 2024-05-27 04:40:28.859463 allianceauth-4.1.0/allianceauth/services/modules/example/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.000463 allianceauth-4.1.0/allianceauth/services/modules/ips4/__init__.py
+-rw-r--r--   0        0        0      240 2024-05-27 04:40:28.859463 allianceauth-4.1.0/allianceauth/services/modules/ips4/admin.py
+-rw-r--r--   0        0        0      139 2024-05-27 04:40:28.859463 allianceauth-4.1.0/allianceauth/services/modules/ips4/apps.py
+-rw-r--r--   0        0        0     1554 2024-05-27 04:40:28.859463 allianceauth-4.1.0/allianceauth/services/modules/ips4/auth_hooks.py
+-rw-r--r--   0        0        0     4199 2024-05-27 04:40:28.859463 allianceauth-4.1.0/allianceauth/services/modules/ips4/manager.py
+-rw-r--r--   0        0        0      737 2024-05-27 04:40:28.859463 allianceauth-4.1.0/allianceauth/services/modules/ips4/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2025 2024-05-27 04:40:28.859463 allianceauth-4.1.0/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.001463 allianceauth-4.1.0/allianceauth/services/modules/ips4/migrations/__init__.py
+-rw-r--r--   0        0        0      558 2024-05-27 04:40:28.859463 allianceauth-4.1.0/allianceauth/services/modules/ips4/models.py
+-rw-r--r--   0        0        0     1104 2024-05-27 04:40:28.859463 allianceauth-4.1.0/allianceauth/services/modules/ips4/tasks.py
+-rw-r--r--   0        0        0     6035 2024-05-27 04:40:28.859463 allianceauth-4.1.0/allianceauth/services/modules/ips4/tests.py
+-rw-r--r--   0        0        0      495 2024-05-27 04:40:28.860463 allianceauth-4.1.0/allianceauth/services/modules/ips4/urls.py
+-rw-r--r--   0        0        0     4825 2024-05-27 04:40:28.860463 allianceauth-4.1.0/allianceauth/services/modules/ips4/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.001463 allianceauth-4.1.0/allianceauth/services/modules/mumble/__init__.py
+-rw-r--r--   0        0        0      455 2024-05-27 04:40:28.860463 allianceauth-4.1.0/allianceauth/services/modules/mumble/admin.py
+-rw-r--r--   0        0        0      145 2024-05-27 04:40:28.860463 allianceauth-4.1.0/allianceauth/services/modules/mumble/apps.py
+-rw-r--r--   0        0        0     2958 2024-05-27 04:40:28.860463 allianceauth-4.1.0/allianceauth/services/modules/mumble/auth_hooks.py
+-rw-r--r--   0        0        0      726 2024-05-27 04:40:28.860463 allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2868 2024-05-27 04:40:28.860463 allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py
+-rw-r--r--   0        0        0      316 2024-05-27 04:40:28.860463 allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0002_auto_20161212_0100.py
+-rw-r--r--   0        0        0      613 2024-05-27 04:40:28.860463 allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py
+-rw-r--r--   0        0        0      548 2024-05-27 04:40:28.860463 allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py
+-rw-r--r--   0        0        0      561 2024-05-27 04:40:28.860463 allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py
+-rw-r--r--   0        0        0     2063 2024-05-27 04:40:28.861463 allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py
+-rw-r--r--   0        0        0      679 2024-05-27 04:40:28.861463 allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py
+-rw-r--r--   0        0        0      398 2024-05-27 04:40:28.861463 allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0008_mumbleuser_display_name.py
+-rw-r--r--   0        0        0     1181 2024-05-27 04:40:28.861463 allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py
+-rw-r--r--   0        0        0      554 2024-05-27 04:40:28.861463 allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py
+-rw-r--r--   0        0        0      390 2024-05-27 04:40:28.861463 allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0011_auto_20201011_1009.py
+-rw-r--r--   0        0        0     1508 2024-05-27 04:40:28.861463 allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.011463 allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/__init__.py
+-rw-r--r--   0        0        0     5630 2024-05-27 04:40:28.861463 allianceauth-4.1.0/allianceauth/services/modules/mumble/models.py
+-rw-r--r--   0        0        0     3142 2024-05-27 04:40:28.861463 allianceauth-4.1.0/allianceauth/services/modules/mumble/tasks.py
+-rw-r--r--   0        0        0     1655 2024-05-27 04:40:28.861463 allianceauth-4.1.0/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html
+-rw-r--r--   0        0        0     8632 2024-05-27 04:40:28.862463 allianceauth-4.1.0/allianceauth/services/modules/mumble/tests.py
+-rw-r--r--   0        0        0      560 2024-05-27 04:40:28.862463 allianceauth-4.1.0/allianceauth/services/modules/mumble/urls.py
+-rw-r--r--   0        0        0      994 2024-05-27 04:40:28.862463 allianceauth-4.1.0/allianceauth/services/modules/mumble/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.011463 allianceauth-4.1.0/allianceauth/services/modules/openfire/__init__.py
+-rw-r--r--   0        0        0      317 2024-05-27 04:40:28.862463 allianceauth-4.1.0/allianceauth/services/modules/openfire/admin.py
+-rw-r--r--   0        0        0      151 2024-05-27 04:40:28.862463 allianceauth-4.1.0/allianceauth/services/modules/openfire/apps.py
+-rw-r--r--   0        0        0     3648 2024-05-27 04:40:28.862463 allianceauth-4.1.0/allianceauth/services/modules/openfire/auth_hooks.py
+-rw-r--r--   0        0        0      263 2024-05-27 04:40:28.862463 allianceauth-4.1.0/allianceauth/services/modules/openfire/forms.py
+-rw-r--r--   0        0        0     8321 2024-05-27 04:40:28.862463 allianceauth-4.1.0/allianceauth/services/modules/openfire/manager.py
+-rw-r--r--   0        0        0      687 2024-05-27 04:40:28.862463 allianceauth-4.1.0/allianceauth/services/modules/openfire/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2073 2024-05-27 04:40:28.862463 allianceauth-4.1.0/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.012463 allianceauth-4.1.0/allianceauth/services/modules/openfire/migrations/__init__.py
+-rw-r--r--   0        0        0      495 2024-05-27 04:40:28.863463 allianceauth-4.1.0/allianceauth/services/modules/openfire/models.py
+-rw-r--r--   0        0        0     2620 2024-05-27 04:40:28.863463 allianceauth-4.1.0/allianceauth/services/modules/openfire/tasks.py
+-rw-r--r--   0        0        0     1533 2024-05-27 04:40:28.863463 allianceauth-4.1.0/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html
+-rw-r--r--   0        0        0     9478 2024-05-27 04:40:28.863463 allianceauth-4.1.0/allianceauth/services/modules/openfire/tests.py
+-rw-r--r--   0        0        0      585 2024-05-27 04:40:28.863463 allianceauth-4.1.0/allianceauth/services/modules/openfire/urls.py
+-rw-r--r--   0        0        0     7688 2024-05-27 04:40:28.863463 allianceauth-4.1.0/allianceauth/services/modules/openfire/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.012463 allianceauth-4.1.0/allianceauth/services/modules/phpbb3/__init__.py
+-rw-r--r--   0        0        0      310 2024-05-27 04:40:28.863463 allianceauth-4.1.0/allianceauth/services/modules/phpbb3/admin.py
+-rw-r--r--   0        0        0      145 2024-05-27 04:40:28.863463 allianceauth-4.1.0/allianceauth/services/modules/phpbb3/apps.py
+-rw-r--r--   0        0        0     2196 2024-05-27 04:40:28.863463 allianceauth-4.1.0/allianceauth/services/modules/phpbb3/auth_hooks.py
+-rw-r--r--   0        0        0    13459 2024-05-27 04:40:28.863463 allianceauth-4.1.0/allianceauth/services/modules/phpbb3/manager.py
+-rw-r--r--   0        0        0      683 2024-05-27 04:40:28.863463 allianceauth-4.1.0/allianceauth/services/modules/phpbb3/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2049 2024-05-27 04:40:28.864463 allianceauth-4.1.0/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.013463 allianceauth-4.1.0/allianceauth/services/modules/phpbb3/migrations/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-27 04:40:28.864463 allianceauth-4.1.0/allianceauth/services/modules/phpbb3/models.py
+-rw-r--r--   0        0        0     2478 2024-05-27 04:40:28.864463 allianceauth-4.1.0/allianceauth/services/modules/phpbb3/tasks.py
+-rw-r--r--   0        0        0     8189 2024-05-27 04:40:28.864463 allianceauth-4.1.0/allianceauth/services/modules/phpbb3/tests.py
+-rw-r--r--   0        0        0      504 2024-05-27 04:40:28.864463 allianceauth-4.1.0/allianceauth/services/modules/phpbb3/urls.py
+-rw-r--r--   0        0        0     5139 2024-05-27 04:40:28.864463 allianceauth-4.1.0/allianceauth/services/modules/phpbb3/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.017463 allianceauth-4.1.0/allianceauth/services/modules/smf/__init__.py
+-rw-r--r--   0        0        0      302 2024-05-27 04:40:28.864463 allianceauth-4.1.0/allianceauth/services/modules/smf/admin.py
+-rw-r--r--   0        0        0      136 2024-05-27 04:40:28.864463 allianceauth-4.1.0/allianceauth/services/modules/smf/apps.py
+-rw-r--r--   0        0        0     2408 2024-05-27 04:40:28.864463 allianceauth-4.1.0/allianceauth/services/modules/smf/auth_hooks.py
+-rw-r--r--   0        0        0    14780 2024-05-27 04:40:28.864463 allianceauth-4.1.0/allianceauth/services/modules/smf/manager.py
+-rw-r--r--   0        0        0      677 2024-05-27 04:40:28.864463 allianceauth-4.1.0/allianceauth/services/modules/smf/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2011 2024-05-27 04:40:28.865463 allianceauth-4.1.0/allianceauth/services/modules/smf/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0      694 2024-05-27 04:40:28.865463 allianceauth-4.1.0/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.017463 allianceauth-4.1.0/allianceauth/services/modules/smf/migrations/__init__.py
+-rw-r--r--   0        0        0      475 2024-05-27 04:40:28.865463 allianceauth-4.1.0/allianceauth/services/modules/smf/models.py
+-rw-r--r--   0        0        0     3740 2024-05-27 04:40:28.865463 allianceauth-4.1.0/allianceauth/services/modules/smf/tasks.py
+-rw-r--r--   0        0        0     8057 2024-05-27 04:40:28.865463 allianceauth-4.1.0/allianceauth/services/modules/smf/tests.py
+-rw-r--r--   0        0        0      489 2024-05-27 04:40:28.865463 allianceauth-4.1.0/allianceauth/services/modules/smf/urls.py
+-rw-r--r--   0        0        0     5143 2024-05-27 04:40:28.865463 allianceauth-4.1.0/allianceauth/services/modules/smf/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.017463 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/__init__.py
+-rw-r--r--   0        0        0     1872 2024-05-27 04:40:28.865463 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/admin.py
+-rw-r--r--   0        0        0      209 2024-05-27 04:40:28.865463 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/apps.py
+-rw-r--r--   0        0        0     2128 2024-05-27 04:40:28.865463 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/auth_hooks.py
+-rw-r--r--   0        0        0      500 2024-05-27 04:40:28.865463 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/forms.py
+-rw-r--r--   0        0        0    12601 2024-05-27 04:40:28.865463 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/manager.py
+-rw-r--r--   0        0        0     1995 2024-05-27 04:40:28.866464 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py
+-rw-r--r--   0        0        0      538 2024-05-27 04:40:28.866464 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py
+-rw-r--r--   0        0        0      781 2024-05-27 04:40:28.866464 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py
+-rw-r--r--   0        0        0     2116 2024-05-27 04:40:28.866464 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py
+-rw-r--r--   0        0        0      784 2024-05-27 04:40:28.866464 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.017463 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/migrations/__init__.py
+-rw-r--r--   0        0        0     1567 2024-05-27 04:40:28.866464 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/models.py
+-rw-r--r--   0        0        0     1723 2024-05-27 04:40:28.866464 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/signals.py
+-rw-r--r--   0        0        0     3780 2024-05-27 04:40:28.866464 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/tasks.py
+-rw-r--r--   0        0        0      296 2024-05-27 04:40:28.866464 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/templates/admin/teamspeak3/authts/change_list.html
+-rw-r--r--   0        0        0     1472 2024-05-27 04:40:28.867463 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html
+-rw-r--r--   0        0        0     1121 2024-05-27 04:40:28.867463 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html
+-rw-r--r--   0        0        0    21498 2024-05-27 04:40:28.867463 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/tests.py
+-rw-r--r--   0        0        0      661 2024-05-27 04:40:28.867463 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/urls.py
+-rw-r--r--   0        0        0       23 2024-05-27 04:40:28.867463 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/util/__init__.py
+-rw-r--r--   0        0        0    15106 2024-05-27 04:40:28.867463 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/util/ts3.py
+-rw-r--r--   0        0        0     5138 2024-05-27 04:40:28.867463 allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.017463 allianceauth-4.1.0/allianceauth/services/modules/xenforo/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-27 04:40:28.867463 allianceauth-4.1.0/allianceauth/services/modules/xenforo/admin.py
+-rw-r--r--   0        0        0      148 2024-05-27 04:40:28.867463 allianceauth-4.1.0/allianceauth/services/modules/xenforo/apps.py
+-rw-r--r--   0        0        0     1779 2024-05-27 04:40:28.867463 allianceauth-4.1.0/allianceauth/services/modules/xenforo/auth_hooks.py
+-rw-r--r--   0        0        0     3685 2024-05-27 04:40:28.868463 allianceauth-4.1.0/allianceauth/services/modules/xenforo/manager.py
+-rw-r--r--   0        0        0      685 2024-05-27 04:40:28.868463 allianceauth-4.1.0/allianceauth/services/modules/xenforo/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2067 2024-05-27 04:40:28.868463 allianceauth-4.1.0/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.017463 allianceauth-4.1.0/allianceauth/services/modules/xenforo/migrations/__init__.py
+-rw-r--r--   0        0        0      491 2024-05-27 04:40:28.868463 allianceauth-4.1.0/allianceauth/services/modules/xenforo/models.py
+-rw-r--r--   0        0        0     1268 2024-05-27 04:40:28.868463 allianceauth-4.1.0/allianceauth/services/modules/xenforo/tasks.py
+-rw-r--r--   0        0        0     7153 2024-05-27 04:40:28.868463 allianceauth-4.1.0/allianceauth/services/modules/xenforo/tests.py
+-rw-r--r--   0        0        0      529 2024-05-27 04:40:28.868463 allianceauth-4.1.0/allianceauth/services/modules/xenforo/urls.py
+-rw-r--r--   0        0        0     4821 2024-05-27 04:40:28.868463 allianceauth-4.1.0/allianceauth/services/modules/xenforo/views.py
+-rw-r--r--   0        0        0    10087 2024-05-27 04:40:28.868463 allianceauth-4.1.0/allianceauth/services/signals.py
+-rw-r--r--   0        0        0      126 2024-05-27 04:40:28.868463 allianceauth-4.1.0/allianceauth/services/static/allianceauth/services/admin.css
+-rw-r--r--   0        0        0     1937 2024-05-27 04:40:28.868463 allianceauth-4.1.0/allianceauth/services/tasks.py
+-rw-r--r--   0        0        0       57 2024-05-27 04:40:28.869463 allianceauth-4.1.0/allianceauth/services/templates/public/menublock.html
+-rw-r--r--   0        0        0      335 2024-05-27 04:40:28.869463 allianceauth-4.1.0/allianceauth/services/templates/public/menuitem.html
+-rw-r--r--   0        0        0     1566 2024-05-27 04:40:28.869463 allianceauth-4.1.0/allianceauth/services/templates/services/fleetformattertool.html
+-rw-r--r--   0        0        0     1232 2024-05-27 04:40:28.869463 allianceauth-4.1.0/allianceauth/services/templates/services/service_confirm_delete.html
+-rw-r--r--   0        0        0     1285 2024-05-27 04:40:28.869463 allianceauth-4.1.0/allianceauth/services/templates/services/service_credentials.html
+-rw-r--r--   0        0        0     1147 2024-05-27 04:40:28.869463 allianceauth-4.1.0/allianceauth/services/templates/services/service_password.html
+-rw-r--r--   0        0        0      239 2024-05-27 04:40:28.869463 allianceauth-4.1.0/allianceauth/services/templates/services/service_status.html
+-rw-r--r--   0        0        0      100 2024-05-27 04:40:28.869463 allianceauth-4.1.0/allianceauth/services/templates/services/service_username.html
+-rw-r--r--   0        0        0     2422 2024-05-27 04:40:28.869463 allianceauth-4.1.0/allianceauth/services/templates/services/services.html
+-rw-r--r--   0        0        0     1233 2024-05-27 04:40:28.869463 allianceauth-4.1.0/allianceauth/services/templates/services/services_ctrl.html
+-rw-r--r--   0        0        0      832 2024-05-27 04:40:28.869463 allianceauth-4.1.0/allianceauth/services/templates/services/services_ctrl_base.html
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.020463 allianceauth-4.1.0/allianceauth/services/tests/__init__.py
+-rw-r--r--   0        0        0     1048 2024-05-27 04:40:28.869463 allianceauth-4.1.0/allianceauth/services/tests/test_hooks.py
+-rw-r--r--   0        0        0      514 2024-05-27 04:40:28.869463 allianceauth-4.1.0/allianceauth/services/tests/test_models.py
+-rw-r--r--   0        0        0     4316 2024-05-27 04:40:28.870463 allianceauth-4.1.0/allianceauth/services/tests/test_nameformatter.py
+-rw-r--r--   0        0        0    12299 2024-05-27 04:40:28.870463 allianceauth-4.1.0/allianceauth/services/tests/test_signals.py
+-rw-r--r--   0        0        0     3248 2024-05-27 04:40:28.870463 allianceauth-4.1.0/allianceauth/services/tests/test_tasks.py
+-rw-r--r--   0        0        0      530 2024-05-27 04:40:28.870463 allianceauth-4.1.0/allianceauth/services/urls.py
+-rw-r--r--   0        0        0     2450 2024-05-27 04:40:28.870463 allianceauth-4.1.0/allianceauth/services/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.020463 allianceauth-4.1.0/allianceauth/srp/__init__.py
+-rw-r--r--   0        0        0      205 2024-05-27 04:40:28.870463 allianceauth-4.1.0/allianceauth/srp/admin.py
+-rw-r--r--   0        0        0      112 2024-05-27 04:40:28.870463 allianceauth-4.1.0/allianceauth/srp/apps.py
+-rw-r--r--   0        0        0      960 2024-05-27 04:40:28.870463 allianceauth-4.1.0/allianceauth/srp/auth_hooks.py
+-rw-r--r--   0        0        0     1724 2024-05-27 04:40:28.870463 allianceauth-4.1.0/allianceauth/srp/form.py
+-rw-r--r--   0        0        0     1961 2024-05-27 04:40:28.870463 allianceauth-4.1.0/allianceauth/srp/managers.py
+-rw-r--r--   0        0        0     2265 2024-05-27 04:40:28.870463 allianceauth-4.1.0/allianceauth/srp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      488 2024-05-27 04:40:28.870463 allianceauth-4.1.0/allianceauth/srp/migrations/0002_srpuserrequest_srp_status_choices.py
+-rw-r--r--   0        0        0     2048 2024-05-27 04:40:28.870463 allianceauth-4.1.0/allianceauth/srp/migrations/0003_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      746 2024-05-27 04:40:28.870463 allianceauth-4.1.0/allianceauth/srp/migrations/0004_on_delete.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.020463 allianceauth-4.1.0/allianceauth/srp/migrations/__init__.py
+-rw-r--r--   0        0        0     1991 2024-05-27 04:40:28.871463 allianceauth-4.1.0/allianceauth/srp/models.py
+-rw-r--r--   0        0        0      388 2024-05-27 04:40:28.871463 allianceauth-4.1.0/allianceauth/srp/providers.py
+-rw-r--r--   0        0        0    24877 2024-05-27 04:40:28.871463 allianceauth-4.1.0/allianceauth/srp/swagger.json
+-rw-r--r--   0        0        0     2597 2024-05-27 04:40:28.871463 allianceauth-4.1.0/allianceauth/srp/templates/srp/add.html
+-rw-r--r--   0        0        0    13408 2024-05-27 04:40:28.871463 allianceauth-4.1.0/allianceauth/srp/templates/srp/data.html
+-rw-r--r--   0        0        0     6364 2024-05-27 04:40:28.871463 allianceauth-4.1.0/allianceauth/srp/templates/srp/management.html
+-rw-r--r--   0        0        0     1432 2024-05-27 04:40:28.871463 allianceauth-4.1.0/allianceauth/srp/templates/srp/request.html
+-rw-r--r--   0        0        0     1765 2024-05-27 04:40:28.871463 allianceauth-4.1.0/allianceauth/srp/templates/srp/update.html
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.020463 allianceauth-4.1.0/allianceauth/srp/tests/__init__.py
+-rw-r--r--   0        0        0     3623 2024-05-27 04:40:28.871463 allianceauth-4.1.0/allianceauth/srp/tests/test_managers.py
+-rw-r--r--   0        0        0    28605 2024-05-27 04:40:28.872463 allianceauth-4.1.0/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json
+-rw-r--r--   0        0        0      363 2024-05-27 04:40:28.872463 allianceauth-4.1.0/allianceauth/srp/tests/testdata/zkillboard_killmail_api_81973979.json
+-rw-r--r--   0        0        0     1342 2024-05-27 04:40:28.872463 allianceauth-4.1.0/allianceauth/srp/urls.py
+-rw-r--r--   0        0        0    17762 2024-05-27 04:40:28.872463 allianceauth-4.1.0/allianceauth/srp/views.py
+-rw-r--r--   0        0        0     4616 2024-05-27 04:40:28.872463 allianceauth-4.1.0/allianceauth/static/allianceauth/css/auth-base.css
+-rw-r--r--   0        0        0     1173 2024-05-27 04:40:28.872463 allianceauth-4.1.0/allianceauth/static/allianceauth/css/checkbox.css
+-rw-r--r--   0        0        0      865 2024-05-27 04:40:28.872463 allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less
+-rw-r--r--   0        0        0     1078 2024-05-27 04:40:28.872463 allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/darkly/LICENSE
+-rw-r--r--   0        0        0      624 2024-05-27 04:40:28.873463 allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.less
+-rw-r--r--   0        0        0   122466 2024-05-27 04:40:28.873463 allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css
+-rw-r--r--   0        0        0      979 2024-05-27 04:40:28.874463 allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/flatly-shared.less
+-rw-r--r--   0        0        0     1078 2024-05-27 04:40:28.874463 allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/flatly/LICENSE
+-rw-r--r--   0        0        0      985 2024-05-27 04:40:28.874463 allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.less
+-rw-r--r--   0        0        0   123138 2024-05-27 04:40:28.874463 allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css
+-rwxr-xr-x   0        0        0    21465 2024-05-27 04:40:28.874463 allianceauth-4.1.0/allianceauth/static/allianceauth/icons/allianceauth.png
+-rw-r--r--   0        0        0     7686 2024-05-27 04:40:28.874463 allianceauth-4.1.0/allianceauth/static/allianceauth/icons/android-chrome-192x192.png
+-rw-r--r--   0        0        0    26346 2024-05-27 04:40:28.875463 allianceauth-4.1.0/allianceauth/static/allianceauth/icons/android-chrome-512x512.png
+-rw-r--r--   0        0        0     7160 2024-05-27 04:40:28.875463 allianceauth-4.1.0/allianceauth/static/allianceauth/icons/apple-touch-icon.png
+-rw-r--r--   0        0        0      272 2024-05-27 04:40:28.875463 allianceauth-4.1.0/allianceauth/static/allianceauth/icons/browserconfig.xml
+-rw-r--r--   0        0        0      941 2024-05-27 04:40:28.875463 allianceauth-4.1.0/allianceauth/static/allianceauth/icons/favicon-16x16.png
+-rw-r--r--   0        0        0     1565 2024-05-27 04:40:28.875463 allianceauth-4.1.0/allianceauth/static/allianceauth/icons/favicon-32x32.png
+-rwxr-xr-x   0        0        0     2180 2024-05-27 04:40:28.875463 allianceauth-4.1.0/allianceauth/static/allianceauth/icons/favicon-96x96.png
+-rw-r--r--   0        0        0    15086 2024-05-27 04:40:28.875463 allianceauth-4.1.0/allianceauth/static/allianceauth/icons/favicon.ico
+-rw-r--r--   0        0        0     4681 2024-05-27 04:40:28.875463 allianceauth-4.1.0/allianceauth/static/allianceauth/icons/mstile-150x150.png
+-rw-r--r--   0        0        0     2590 2024-05-27 04:40:28.875463 allianceauth-4.1.0/allianceauth/static/allianceauth/icons/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      478 2024-05-27 04:40:28.875463 allianceauth-4.1.0/allianceauth/static/allianceauth/icons/site.webmanifest
+-rw-r--r--   0        0        0    10836 2024-05-27 04:40:28.875463 allianceauth-4.1.0/allianceauth/static/allianceauth/images/auth-logo.png
+-rw-r--r--   0        0        0     2278 2024-05-27 04:40:28.875463 allianceauth-4.1.0/allianceauth/static/allianceauth/images/auth-logo.svg
+-rw-r--r--   0        0        0      573 2024-05-27 04:40:28.876463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/eve-time.js
+-rw-r--r--   0        0        0     1070 2024-05-27 04:40:28.876463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/filterDropDown/LICENSE
+-rw-r--r--   0        0        0    10422 2024-05-27 04:40:28.876463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js
+-rw-r--r--   0        0        0     4205 2024-05-27 04:40:28.876463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js
+-rw-r--r--   0        0        0     7090 2024-05-27 04:40:28.876463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0        0        0     7074 2024-05-27 04:40:28.876463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0        0        0     4618 2024-05-27 04:40:28.876463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png
+-rw-r--r--   0        0        0     7111 2024-05-27 04:40:28.876463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     4618 2024-05-27 04:40:28.876463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     6487 2024-05-27 04:40:28.877463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    15830 2024-05-27 04:40:28.877463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css
+-rw-r--r--   0        0        0     7142 2024-05-27 04:40:28.877463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0        0        0     7126 2024-05-27 04:40:28.877463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0        0        0     4670 2024-05-27 04:40:28.877463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777620_256x240.png
+-rw-r--r--   0        0        0     7163 2024-05-27 04:40:28.877463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     4670 2024-05-27 04:40:28.877463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     6539 2024-05-27 04:40:28.877463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    15842 2024-05-27 04:40:28.877463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/jquery-ui.min.css
+-rw-r--r--   0        0        0     2391 2024-05-27 04:40:28.878463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/refresh-notification-icon.js
+-rw-r--r--   0        0        0     2636 2024-05-27 04:40:28.878463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/refresh_notifications.js
+-rw-r--r--   0        0        0     1170 2024-05-27 04:40:28.878463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/timerboard.js
+-rw-r--r--   0        0        0     1056 2024-05-27 04:40:28.878463 allianceauth-4.1.0/allianceauth/static/allianceauth/js/timers.js
+-rw-r--r--   0        0        0       26 2024-05-27 04:40:28.878463 allianceauth-4.1.0/allianceauth/static/robots.txt
+-rw-r--r--   0        0        0      119 2024-05-27 04:40:28.878463 allianceauth-4.1.0/allianceauth/templates/admin/base_site.html
+-rw-r--r--   0        0        0      403 2024-05-27 04:40:28.878463 allianceauth-4.1.0/allianceauth/templates/allianceauth/admin-status/celery_bar_partial.html
+-rw-r--r--   0        0        0     1282 2024-05-27 04:40:28.878463 allianceauth-4.1.0/allianceauth/templates/allianceauth/admin-status/esi_check.html
+-rw-r--r--   0        0        0       47 2024-05-27 04:40:28.878463 allianceauth-4.1.0/allianceauth/templates/allianceauth/admin-status/include.html
+-rw-r--r--   0        0        0     7764 2024-05-27 04:40:28.878463 allianceauth-4.1.0/allianceauth/templates/allianceauth/admin-status/overview.html
+-rw-r--r--   0        0        0     5350 2024-05-27 04:40:28.878463 allianceauth-4.1.0/allianceauth/templates/allianceauth/base-bs5.html
+-rw-r--r--   0        0        0     2443 2024-05-27 04:40:28.878463 allianceauth-4.1.0/allianceauth/templates/allianceauth/base.html
+-rw-r--r--   0        0        0     1289 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/allianceauth/error.html
+-rw-r--r--   0        0        0      928 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/allianceauth/icons.html
+-rw-r--r--   0        0        0      996 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/allianceauth/messages-bs5.html
+-rw-r--r--   0        0        0     1115 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/allianceauth/messages.html
+-rw-r--r--   0        0        0      263 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/allianceauth/night-toggle.html
+-rw-r--r--   0        0        0      450 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/allianceauth/notifications_menu_item.html
+-rw-r--r--   0        0        0      879 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/allianceauth/side-menu.html
+-rw-r--r--   0        0        0      904 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/allianceauth/top-menu-admin.html
+-rw-r--r--   0        0        0      855 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/allianceauth/top-menu-rh-default.html
+-rw-r--r--   0        0        0     3086 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/allianceauth/top-menu-user-dropdown.html
+-rw-r--r--   0        0        0     1576 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/allianceauth/top-menu.html
+-rw-r--r--   0        0        0       96 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/bundles/auth-base-css.html
+-rw-r--r--   0        0        0      111 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/bundles/auth-framework-css.html
+-rw-r--r--   0        0        0      171 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/bundles/bootstrap-css-bs5.html
+-rw-r--r--   0        0        0     1269 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/bundles/bootstrap-css.html
+-rw-r--r--   0        0        0      503 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/bundles/bootstrap-js-bs5.html
+-rw-r--r--   0        0        0      613 2024-05-27 04:40:28.879463 allianceauth-4.1.0/allianceauth/templates/bundles/bootstrap-js.html
+-rw-r--r--   0        0        0       95 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/checkbox-css.html
+-rw-r--r--   0        0        0      343 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/clipboard-js.html
+-rw-r--r--   0        0        0      369 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/datatables-css-bs5.html
+-rw-r--r--   0        0        0      365 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/datatables-css.html
+-rw-r--r--   0        0        0      628 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/datatables-js-bs5.html
+-rw-r--r--   0        0        0      626 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/datatables-js.html
+-rw-r--r--   0        0        0       86 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/evetime-js.html
+-rw-r--r--   0        0        0      111 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/filterdropdown-js.html
+-rw-r--r--   0        0        0      350 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/fontawesome.html
+-rw-r--r--   0        0        0      237 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/image-auth-logo.html
+-rw-r--r--   0        0        0      392 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/jquery-datetimepicker-css.html
+-rw-r--r--   0        0        0      387 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/jquery-datetimepicker-js.html
+-rw-r--r--   0        0        0      321 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/jquery-js.html
+-rw-r--r--   0        0        0      500 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/jquery-ui-css.html
+-rw-r--r--   0        0        0      333 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/jquery-ui-js.html
+-rw-r--r--   0        0        0      344 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/jquery-visibility-js.html
+-rw-r--r--   0        0        0      579 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/moment-js.html
+-rw-r--r--   0        0        0      103 2024-05-27 04:40:28.880463 allianceauth-4.1.0/allianceauth/templates/bundles/refresh-notification-icon-js.html
+-rw-r--r--   0        0        0       99 2024-05-27 04:40:28.881463 allianceauth-4.1.0/allianceauth/templates/bundles/refresh-notifications-js.html
+-rw-r--r--   0        0        0       88 2024-05-27 04:40:28.881463 allianceauth-4.1.0/allianceauth/templates/bundles/timerboard-js.html
+-rw-r--r--   0        0        0       84 2024-05-27 04:40:28.881463 allianceauth-4.1.0/allianceauth/templates/bundles/timers-js.html
+-rw-r--r--   0        0        0      368 2024-05-27 04:40:28.881463 allianceauth-4.1.0/allianceauth/templates/bundles/x-editable-js.html
+-rw-r--r--   0        0        0      375 2024-05-27 04:40:28.881463 allianceauth-4.1.0/allianceauth/templates/bundles/x-editable.css.html
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.032463 allianceauth-4.1.0/allianceauth/templatetags/__init__.py
+-rw-r--r--   0        0        0     5665 2024-05-27 04:40:28.881463 allianceauth-4.1.0/allianceauth/templatetags/admin_status.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.032463 allianceauth-4.1.0/allianceauth/tests/__init__.py
+-rw-r--r--   0        0        0    11465 2024-05-27 04:40:28.881463 allianceauth-4.1.0/allianceauth/tests/auth_utils.py
+-rw-r--r--   0        0        0     2061 2024-05-27 04:40:28.881463 allianceauth-4.1.0/allianceauth/tests/test_auth_utils.py
+-rw-r--r--   0        0        0     2897 2024-05-27 04:40:28.881463 allianceauth-4.1.0/allianceauth/tests/test_urls.py
+-rw-r--r--   0        0        0     1403 2024-05-27 04:40:28.881463 allianceauth-4.1.0/allianceauth/tests/test_views.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.032463 allianceauth-4.1.0/allianceauth/theme/__init__.py
+-rw-r--r--   0        0        0      153 2024-05-27 04:40:28.881463 allianceauth-4.1.0/allianceauth/theme/apps.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.032463 allianceauth-4.1.0/allianceauth/theme/bootstrap/__init__.py
+-rw-r--r--   0        0        0      241 2024-05-27 04:40:28.882463 allianceauth-4.1.0/allianceauth/theme/bootstrap/apps.py
+-rw-r--r--   0        0        0     1778 2024-05-27 04:40:28.882463 allianceauth-4.1.0/allianceauth/theme/bootstrap/auth_hooks.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.036463 allianceauth-4.1.0/allianceauth/theme/darkly/__init__.py
+-rw-r--r--   0        0        0      240 2024-05-27 04:40:28.882463 allianceauth-4.1.0/allianceauth/theme/darkly/apps.py
+-rw-r--r--   0        0        0     1232 2024-05-27 04:40:28.882463 allianceauth-4.1.0/allianceauth/theme/darkly/auth_hooks.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.036463 allianceauth-4.1.0/allianceauth/theme/flatly/__init__.py
+-rw-r--r--   0        0        0      240 2024-05-27 04:40:28.882463 allianceauth-4.1.0/allianceauth/theme/flatly/apps.py
+-rw-r--r--   0        0        0     1227 2024-05-27 04:40:28.882463 allianceauth-4.1.0/allianceauth/theme/flatly/auth_hooks.py
+-rw-r--r--   0        0        0     1537 2024-05-27 04:40:28.882463 allianceauth-4.1.0/allianceauth/theme/hooks.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.037463 allianceauth-4.1.0/allianceauth/theme/materia/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-27 04:40:28.882463 allianceauth-4.1.0/allianceauth/theme/materia/apps.py
+-rw-r--r--   0        0        0     1243 2024-05-27 04:40:28.882463 allianceauth-4.1.0/allianceauth/theme/materia/auth_hooks.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.037463 allianceauth-4.1.0/allianceauth/theme/templates/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.037463 allianceauth-4.1.0/allianceauth/theme/templates/theme/__init__.py
+-rw-r--r--   0        0        0      389 2024-05-27 04:40:28.883463 allianceauth-4.1.0/allianceauth/theme/templates/theme/theme_imports_css.html
+-rw-r--r--   0        0        0      376 2024-05-27 04:40:28.883463 allianceauth-4.1.0/allianceauth/theme/templates/theme/theme_imports_js.html
+-rw-r--r--   0        0        0      494 2024-05-27 04:40:28.883463 allianceauth-4.1.0/allianceauth/theme/templates/theme/theme_select.html
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.037463 allianceauth-4.1.0/allianceauth/theme/templatetags/__init__.py
+-rw-r--r--   0        0        0     1921 2024-05-27 04:40:28.883463 allianceauth-4.1.0/allianceauth/theme/templatetags/theme_tags.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.037463 allianceauth-4.1.0/allianceauth/thirdparty/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.037463 allianceauth-4.1.0/allianceauth/thirdparty/navhelper/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.037463 allianceauth-4.1.0/allianceauth/thirdparty/navhelper/templatetags/__init__.py
+-rw-r--r--   0        0        0     2876 2024-05-27 04:40:28.883463 allianceauth-4.1.0/allianceauth/thirdparty/navhelper/templatetags/navactive.py
+-rw-r--r--   0        0        0     3407 2024-05-27 04:40:28.883463 allianceauth-4.1.0/allianceauth/thirdparty/navhelper/tests.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.037463 allianceauth-4.1.0/allianceauth/timerboard/__init__.py
+-rw-r--r--   0        0        0      111 2024-05-27 04:40:28.883463 allianceauth-4.1.0/allianceauth/timerboard/admin.py
+-rw-r--r--   0        0        0      133 2024-05-27 04:40:28.883463 allianceauth-4.1.0/allianceauth/timerboard/apps.py
+-rw-r--r--   0        0        0     1141 2024-05-27 04:40:28.883463 allianceauth-4.1.0/allianceauth/timerboard/auth_hooks.py
+-rw-r--r--   0        0        0     5267 2024-05-27 04:40:28.883463 allianceauth-4.1.0/allianceauth/timerboard/form.py
+-rw-r--r--   0        0        0     1629 2024-05-27 04:40:28.884463 allianceauth-4.1.0/allianceauth/timerboard/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1063 2024-05-27 04:40:28.884463 allianceauth-4.1.0/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      763 2024-05-27 04:40:28.884463 allianceauth-4.1.0/allianceauth/timerboard/migrations/0003_on_delete.py
+-rw-r--r--   0        0        0      811 2024-05-27 04:40:28.884463 allianceauth-4.1.0/allianceauth/timerboard/migrations/0004_timer_type.py
+-rw-r--r--   0        0        0      410 2024-05-27 04:40:28.884463 allianceauth-4.1.0/allianceauth/timerboard/migrations/0005_alter_timer_planet_moon.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.037463 allianceauth-4.1.0/allianceauth/timerboard/migrations/__init__.py
+-rw-r--r--   0        0        0     1593 2024-05-27 04:40:28.884463 allianceauth-4.1.0/allianceauth/timerboard/models.py
+-rw-r--r--   0        0        0     2893 2024-05-27 04:40:28.884463 allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/dashboard.timers.html
+-rw-r--r--   0        0        0     1917 2024-05-27 04:40:28.884463 allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/form.html
+-rw-r--r--   0        0        0      147 2024-05-27 04:40:28.884463 allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/index_button.html
+-rw-r--r--   0        0        0     1021 2024-05-27 04:40:28.884463 allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html
+-rw-r--r--   0        0        0      810 2024-05-27 04:40:28.884463 allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/timer_create_form.html
+-rw-r--r--   0        0        0      830 2024-05-27 04:40:28.884463 allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/timer_update_form.html
+-rw-r--r--   0        0        0     8213 2024-05-27 04:40:28.884463 allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/timertable.html
+-rw-r--r--   0        0        0     5121 2024-05-27 04:40:28.885463 allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/view.html
+-rw-r--r--   0        0        0     8741 2024-05-27 04:40:28.885463 allianceauth-4.1.0/allianceauth/timerboard/tests.py
+-rw-r--r--   0        0        0      358 2024-05-27 04:40:28.885463 allianceauth-4.1.0/allianceauth/timerboard/urls.py
+-rw-r--r--   0        0        0     4057 2024-05-27 04:40:28.885463 allianceauth-4.1.0/allianceauth/timerboard/views.py
+-rw-r--r--   0        0        0     2688 2024-05-27 04:40:28.885463 allianceauth-4.1.0/allianceauth/urls.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.037463 allianceauth-4.1.0/allianceauth/utils/__init__.py
+-rw-r--r--   0        0        0      568 2024-05-27 04:40:28.885463 allianceauth-4.1.0/allianceauth/utils/cache.py
+-rw-r--r--   0        0        0     1971 2024-05-27 04:40:28.885463 allianceauth-4.1.0/allianceauth/utils/counters.py
+-rw-r--r--   0        0        0      615 2024-05-27 04:40:28.885463 allianceauth-4.1.0/allianceauth/utils/django.py
+-rw-r--r--   0        0        0      844 2024-05-27 04:40:28.885463 allianceauth-4.1.0/allianceauth/utils/testing.py
+-rw-r--r--   0        0        0        0 2024-05-27 04:40:29.037463 allianceauth-4.1.0/allianceauth/utils/tests/__init__.py
+-rw-r--r--   0        0        0     1194 2024-05-27 04:40:28.885463 allianceauth-4.1.0/allianceauth/utils/tests/test_cache.py
+-rw-r--r--   0        0        0     3328 2024-05-27 04:40:28.885463 allianceauth-4.1.0/allianceauth/utils/tests/test_counters.py
+-rw-r--r--   0        0        0      777 2024-05-27 04:40:28.885463 allianceauth-4.1.0/allianceauth/utils/tests/test_django.py
+-rw-r--r--   0        0        0      310 2024-05-27 04:40:28.885463 allianceauth-4.1.0/allianceauth/utils/tests/test_testing.py
+-rw-r--r--   0        0        0     3289 2024-05-27 04:40:28.886463 allianceauth-4.1.0/allianceauth/views.py
+-rw-r--r--   0        0        0     2498 2024-05-27 04:40:28.908463 allianceauth-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7491 1970-01-01 00:00:00.000000 allianceauth-4.1.0/PKG-INFO
```

### Comparing `allianceauth-4.0.2/LICENSE` & `allianceauth-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/README.md` & `allianceauth-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/analytics/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/analytics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py` & `allianceauth-4.1.0/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/analytics/migrations/0003_Generate_Identifier.py` & `allianceauth-4.1.0/allianceauth/analytics/migrations/0003_Generate_Identifier.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/analytics/migrations/0004_auto_20211015_0502.py` & `allianceauth-4.1.0/allianceauth/analytics/migrations/0004_auto_20211015_0502.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/analytics/migrations/0006_more_ignore_paths.py` & `allianceauth-4.1.0/allianceauth/analytics/migrations/0006_more_ignore_paths.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/analytics/migrations/0008_add_AA_GA-4_Team_Token .py` & `allianceauth-4.1.0/allianceauth/analytics/migrations/0008_add_AA_GA-4_Team_Token .py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/analytics/migrations/0009_remove_analyticstokens_ignore_paths_and_more.py` & `allianceauth-4.1.0/allianceauth/analytics/migrations/0009_remove_analyticstokens_ignore_paths_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/analytics/models.py` & `allianceauth-4.1.0/allianceauth/analytics/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/analytics/tasks.py` & `allianceauth-4.1.0/allianceauth/analytics/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/analytics/tests/test_models.py` & `allianceauth-4.1.0/allianceauth/analytics/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/analytics/tests/test_tasks.py` & `allianceauth-4.1.0/allianceauth/analytics/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/analytics/tests/test_utils.py` & `allianceauth-4.1.0/allianceauth/analytics/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/analytics/utils.py` & `allianceauth-4.1.0/allianceauth/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/apps.py` & `allianceauth-4.1.0/allianceauth/apps.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/admin.py` & `allianceauth-4.1.0/allianceauth/authentication/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/app_settings.py` & `allianceauth-4.1.0/allianceauth/authentication/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/apps.py` & `allianceauth-4.1.0/allianceauth/authentication/apps.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/authentication/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/backends.py` & `allianceauth-4.1.0/allianceauth/authentication/backends.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/constants.py` & `allianceauth-4.1.0/allianceauth/authentication/constants.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/core/celery_workers.py` & `allianceauth-4.1.0/allianceauth/authentication/core/celery_workers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/decorators.py` & `allianceauth-4.1.0/allianceauth/authentication/decorators.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/forms.py` & `allianceauth-4.1.0/allianceauth/authentication/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/hmac_urls.py` & `allianceauth-4.1.0/allianceauth/authentication/hmac_urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/management/commands/checkmains.py` & `allianceauth-4.1.0/allianceauth/authentication/management/commands/checkmains.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/managers.py` & `allianceauth-4.1.0/allianceauth/authentication/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/middleware.py` & `allianceauth-4.1.0/allianceauth/authentication/middleware.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0004_create_permissions.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0004_create_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0005_delete_perms.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0005_delete_perms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0006_auto_20160910_0542.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0006_auto_20160910_0542.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0009_auto_20161021_0228.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0009_auto_20161021_0228.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0013_service_modules.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0013_service_modules.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0014_fleetup_permission.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0014_fleetup_permission.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0015_user_profiles.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0015_user_profiles.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0016_ownershiprecord.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0016_ownershiprecord.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0018_state_member_factions.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0018_state_member_factions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0021_alter_userprofile_language.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0021_alter_userprofile_language.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0022_userprofile_theme.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0022_userprofile_theme.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/migrations/0023_alter_userprofile_language.py` & `allianceauth-4.1.0/allianceauth/authentication/migrations/0023_alter_userprofile_language.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/models.py` & `allianceauth-4.1.0/allianceauth/authentication/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/signals.py` & `allianceauth-4.1.0/allianceauth/authentication/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg` & `allianceauth-4.1.0/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png` & `allianceauth-4.1.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png` & `allianceauth-4.1.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/task_statistics/counters.py` & `allianceauth-4.1.0/allianceauth/authentication/task_statistics/counters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/task_statistics/event_series.py` & `allianceauth-4.1.0/allianceauth/authentication/task_statistics/event_series.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/task_statistics/helpers.py` & `allianceauth-4.1.0/allianceauth/authentication/task_statistics/helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/task_statistics/signals.py` & `allianceauth-4.1.0/allianceauth/authentication/task_statistics/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_counters.py` & `allianceauth-4.1.0/allianceauth/authentication/task_statistics/tests/test_counters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_event_series.py` & `allianceauth-4.1.0/allianceauth/authentication/task_statistics/tests/test_event_series.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_helpers.py` & `allianceauth-4.1.0/allianceauth/authentication/task_statistics/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/task_statistics/tests/test_signals.py` & `allianceauth-4.1.0/allianceauth/authentication/task_statistics/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/tasks.py` & `allianceauth-4.1.0/allianceauth/authentication/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/templates/authentication/dashboard_characters.html` & `allianceauth-4.1.0/allianceauth/authentication/templates/authentication/dashboard_characters.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 {% load i18n %}
 <div id="aa-dashboard-panel-characters" class="col-12 col-xl-8 align-self-stretch p-2 ps-0 pe-0 ps-xl-0 pe-xl-2">
-    <div class="card">
+    <div class="card h-100">
         <div class="card-body">
-            <div class="d-flex align-items-center">
-                <h4 class="ms-auto me-auto">
-                    {% translate "Characters" %}
-                </h4>
-            </div>
-            <div class="card-body">
+            {% translate "Characters" as widget_title %}
+            {% include "framework/dashboard/widget-title.html" with title=widget_title %}
+
+            <div>
                 <div style="height: 300px; overflow-y:auto;">
                     <div class="d-flex">
                         <a href="{% url 'authentication:add_character' %}" class="btn btn-primary flex-fill m-1" title="{% translate 'Add Character' %}">
                             <span class="d-md-inline m-2">{% translate 'Add Character' %}</span>
                         </a>
                         <a href="{% url 'authentication:change_main_character' %}" class="btn btn-primary flex-fill m-1" title="{% translate 'Change Main' %}">
                             <span class="d-md-inline m-2">{% translate 'Change Main' %}</span>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% load i18n %}
-****** {{%% ttrraannssllaattee ""CChhaarraacctteerrss"" %%}} ******
+{% translate "Characters" as widget_title %} {% include "framework/dashboard/
+widget-title.html" with title=widget_title %}
 _{_%_ _t_r_a_n_s_l_a_t_e_ _'_A_d_d_ _C_h_a_r_a_c_t_e_r_'_ _%_}_ _{_%_ _t_r_a_n_s_l_a_t_e_ _'_C_h_a_n_g_e_ _M_a_i_n_'_ _%_}
                     {{%% ttrraannssllaattee ""NNaammee"" {{%% ttrraannssllaattee ""CCoorrpp""   {{%% ttrraannssllaattee ""AAlllliiaannccee"" %%}}
                     %%}}                  %%}}
 [{                  {                   {                     {
 {                   {                   {                     {
 char.character_name char.character_name char.corporation_name char.alliance_name|default_if_none:
 }}]                 }}                  }}                    "" }}
```

### Comparing `allianceauth-4.0.2/allianceauth/authentication/templates/authentication/dashboard_groups.html` & `allianceauth-4.1.0/allianceauth/authentication/templates/authentication/dashboard_groups.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 {% load i18n %}
 <div id="aa-dashboard-panel-membership" class="col-12 col-xl-4 align-self-stretch py-2 ps-xl-2">
     <div class="card h-100">
         <div class="card-body">
-            <h4 class="card-title text-center">{% translate "Membership" %}</h4>
-            <div class="card-body">
+            {% translate "Membership" as widget_title %}
+            {% include "framework/dashboard/widget-title.html" with title=widget_title %}
+
+            <div>
                 <div style="height: 300px; overflow-y:auto;">
                     <h5 class="text-center">{% translate "State:" %} {{ request.user.profile.state }}</h5>
                     <table class="table">
                         {% for group in groups %}
                             <tr>
                                 <td class="text-center">{{ group.name }}</td>
                             </tr>
```

#### html2text {}

```diff
@@ -1,4 +1,5 @@
 {% load i18n %}
-****** {{%% ttrraannssllaattee ""MMeemmbbeerrsshhiipp"" %%}} ******
+{% translate "Membership" as widget_title %} {% include "framework/dashboard/
+widget-title.html" with title=widget_title %}
 **** {{%% ttrraannssllaattee ""SSttaattee::"" %%}} {{{{ rreeqquueesstt..uusseerr..pprrooffiillee..ssttaattee }}}} ****
 {{ group.name }}
```

### Comparing `allianceauth-4.0.2/allianceauth/authentication/templates/authentication/tokens.html` & `allianceauth-4.1.0/allianceauth/authentication/templates/authentication/tokens.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/templates/public/base.html` & `allianceauth-4.1.0/allianceauth/authentication/templates/public/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/templates/public/lang_select.html` & `allianceauth-4.1.0/allianceauth/authentication/templates/public/lang_select.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/templates/public/middle_box.html` & `allianceauth-4.1.0/allianceauth/authentication/templates/public/middle_box.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/templates/public/register.html` & `allianceauth-4.1.0/allianceauth/authentication/templates/public/register.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/tests/__init__.py` & `allianceauth-4.1.0/allianceauth/authentication/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/tests/core/test_celery_workers.py` & `allianceauth-4.1.0/allianceauth/authentication/tests/core/test_celery_workers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/tests/test_admin.py` & `allianceauth-4.1.0/allianceauth/authentication/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/tests/test_app_settings.py` & `allianceauth-4.1.0/allianceauth/authentication/tests/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/tests/test_backend.py` & `allianceauth-4.1.0/allianceauth/authentication/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/tests/test_commands.py` & `allianceauth-4.1.0/allianceauth/authentication/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/tests/test_decorators.py` & `allianceauth-4.1.0/allianceauth/authentication/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/tests/test_middleware.py` & `allianceauth-4.1.0/allianceauth/authentication/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/tests/test_models.py` & `allianceauth-4.1.0/allianceauth/authentication/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/tests/test_signals.py` & `allianceauth-4.1.0/allianceauth/authentication/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/tests/test_templatetags.py` & `allianceauth-4.1.0/allianceauth/authentication/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/tests/test_views.py` & `allianceauth-4.1.0/allianceauth/authentication/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/urls.py` & `allianceauth-4.1.0/allianceauth/authentication/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/authentication/views.py` & `allianceauth-4.1.0/allianceauth/authentication/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/bin/allianceauth.py` & `allianceauth-4.1.0/allianceauth/bin/allianceauth.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/corputils/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/corputils/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/corputils/managers.py` & `allianceauth-4.1.0/allianceauth/corputils/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/corputils/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/corputils/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/corputils/migrations/0002_migrate_permissions.py` & `allianceauth-4.1.0/allianceauth/corputils/migrations/0002_migrate_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/corputils/migrations/0003_granular_permissions.py` & `allianceauth-4.1.0/allianceauth/corputils/migrations/0003_granular_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/corputils/migrations/0004_member_models.py` & `allianceauth-4.1.0/allianceauth/corputils/migrations/0004_member_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/corputils/migrations/0005_cleanup_permissions.py` & `allianceauth-4.1.0/allianceauth/corputils/migrations/0005_cleanup_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/corputils/models.py` & `allianceauth-4.1.0/allianceauth/corputils/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/corputils/swagger.json` & `allianceauth-4.1.0/allianceauth/corputils/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/corputils/templates/corputils/base.html` & `allianceauth-4.1.0/allianceauth/corputils/templates/corputils/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/corputils/templates/corputils/corpstats.html` & `allianceauth-4.1.0/allianceauth/corputils/templates/corputils/corpstats.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/corputils/templates/corputils/search.html` & `allianceauth-4.1.0/allianceauth/corputils/templates/corputils/search.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/corputils/tests.py` & `allianceauth-4.1.0/allianceauth/corputils/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/corputils/views.py` & `allianceauth-4.1.0/allianceauth/corputils/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/admin.py` & `allianceauth-4.1.0/allianceauth/eveonline/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/autogroups/admin.py` & `allianceauth-4.1.0/allianceauth/eveonline/autogroups/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/autogroups/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/eveonline/autogroups/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/autogroups/models.py` & `allianceauth-4.1.0/allianceauth/eveonline/autogroups/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/autogroups/signals.py` & `allianceauth-4.1.0/allianceauth/eveonline/autogroups/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/__init__.py` & `allianceauth-4.1.0/allianceauth/eveonline/autogroups/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/test_managers.py` & `allianceauth-4.1.0/allianceauth/eveonline/autogroups/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/test_models.py` & `allianceauth-4.1.0/allianceauth/eveonline/autogroups/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/autogroups/tests/test_signals.py` & `allianceauth-4.1.0/allianceauth/eveonline/autogroups/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/evelinks/__init__.py` & `allianceauth-4.1.0/allianceauth/eveonline/evelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/evelinks/dotlan.py` & `allianceauth-4.1.0/allianceauth/eveonline/evelinks/dotlan.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/evelinks/eveimageserver.py` & `allianceauth-4.1.0/allianceauth/eveonline/evelinks/eveimageserver.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/evelinks/evewho.py` & `allianceauth-4.1.0/allianceauth/eveonline/evelinks/evewho.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/evelinks/tests/test_evelinks.py` & `allianceauth-4.1.0/allianceauth/eveonline/evelinks/tests/test_evelinks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/evelinks/tests/test_templatetags.py` & `allianceauth-4.1.0/allianceauth/eveonline/evelinks/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/evelinks/zkillboard.py` & `allianceauth-4.1.0/allianceauth/eveonline/evelinks/zkillboard.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/managers.py` & `allianceauth-4.1.0/allianceauth/eveonline/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/eveonline/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py` & `allianceauth-4.1.0/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py` & `allianceauth-4.1.0/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/migrations/0007_unique_id_name.py` & `allianceauth-4.1.0/allianceauth/eveonline/migrations/0007_unique_id_name.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/migrations/0008_remove_apikeys.py` & `allianceauth-4.1.0/allianceauth/eveonline/migrations/0008_remove_apikeys.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/migrations/0009_on_delete.py` & `allianceauth-4.1.0/allianceauth/eveonline/migrations/0009_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/migrations/0010_alliance_ticker.py` & `allianceauth-4.1.0/allianceauth/eveonline/migrations/0010_alliance_ticker.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/migrations/0011_ids_to_integers.py` & `allianceauth-4.1.0/allianceauth/eveonline/migrations/0011_ids_to_integers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/migrations/0012_index_additions.py` & `allianceauth-4.1.0/allianceauth/eveonline/migrations/0012_index_additions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/migrations/0015_factions.py` & `allianceauth-4.1.0/allianceauth/eveonline/migrations/0015_factions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py` & `allianceauth-4.1.0/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/models.py` & `allianceauth-4.1.0/allianceauth/eveonline/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/providers.py` & `allianceauth-4.1.0/allianceauth/eveonline/providers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/swagger.json` & `allianceauth-4.1.0/allianceauth/eveonline/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/tasks.py` & `allianceauth-4.1.0/allianceauth/eveonline/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/templatetags/evelinks.py` & `allianceauth-4.1.0/allianceauth/eveonline/templatetags/evelinks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/templatetags/examples.html` & `allianceauth-4.1.0/allianceauth/eveonline/templatetags/examples.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/tests/__init__.py` & `allianceauth-4.1.0/allianceauth/eveonline/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/tests/esi_client_stub.py` & `allianceauth-4.1.0/allianceauth/eveonline/tests/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/tests/swagger_old.json` & `allianceauth-4.1.0/allianceauth/eveonline/tests/swagger_old.json`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/tests/test_managers.py` & `allianceauth-4.1.0/allianceauth/eveonline/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/tests/test_models.py` & `allianceauth-4.1.0/allianceauth/eveonline/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/tests/test_providers.py` & `allianceauth-4.1.0/allianceauth/eveonline/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/eveonline/tests/test_tasks.py` & `allianceauth-4.1.0/allianceauth/eveonline/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/fleetactivitytracking/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/fleetactivitytracking/migrations/0007_sentinel_user.py` & `allianceauth-4.1.0/allianceauth/fleetactivitytracking/migrations/0007_sentinel_user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/fleetactivitytracking/models.py` & `allianceauth-4.1.0/allianceauth/fleetactivitytracking/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/fleetactivitytracking/swagger.json` & `allianceauth-4.1.0/allianceauth/fleetactivitytracking/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html` & `allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkcreate.html` & `allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkcreate.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html` & `allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html` & `allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html` & `allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html` & `allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html` & `allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html` & `allianceauth-4.1.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/fleetactivitytracking/urls.py` & `allianceauth-4.1.0/allianceauth/fleetactivitytracking/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/fleetactivitytracking/views.py` & `allianceauth-4.1.0/allianceauth/fleetactivitytracking/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/framework/api/evecharacter.py` & `allianceauth-4.1.0/allianceauth/framework/api/evecharacter.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/framework/api/user.py` & `allianceauth-4.1.0/allianceauth/framework/api/user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/framework/static/allianceauth/framework/css/auth-framework.css` & `allianceauth-4.1.0/allianceauth/framework/static/allianceauth/framework/css/auth-framework.css`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/framework/tests/test_api_user.py` & `allianceauth-4.1.0/allianceauth/framework/tests/test_api_user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/admin.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/forms.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/managers.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0004_authgroup.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0004_authgroup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0005_authgroup_public.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0005_authgroup_public.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0007_on_delete.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0007_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0009_requestlog.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0009_requestlog.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0010_authgroup_states.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0010_authgroup_states.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0012_group_leads.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0012_group_leads.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/models.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/signals.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/audit.html` & `allianceauth-4.1.0/allianceauth/groupmanagement/templates/groupmanagement/audit.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html` & `allianceauth-4.1.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html` & `allianceauth-4.1.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/groups.html` & `allianceauth-4.1.0/allianceauth/groupmanagement/templates/groupmanagement/groups.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/templates/groupmanagement/index.html` & `allianceauth-4.1.0/allianceauth/groupmanagement/templates/groupmanagement/index.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_admin.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_managers.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_models.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_signals.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/tests/test_views.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/urls.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/groupmanagement/views.py` & `allianceauth-4.1.0/allianceauth/groupmanagement/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hooks.py` & `allianceauth-4.1.0/allianceauth/hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/admin.py` & `allianceauth-4.1.0/allianceauth/hrapplications/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/hrapplications/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/managers.py` & `allianceauth-4.1.0/allianceauth/hrapplications/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/hrapplications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/migrations/0002_choices_for_questions.py` & `allianceauth-4.1.0/allianceauth/hrapplications/migrations/0002_choices_for_questions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py` & `allianceauth-4.1.0/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/migrations/0005_sorted_questions.py` & `allianceauth-4.1.0/allianceauth/hrapplications/migrations/0005_sorted_questions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py` & `allianceauth-4.1.0/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/models.py` & `allianceauth-4.1.0/allianceauth/hrapplications/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/corpchoice.html` & `allianceauth-4.1.0/allianceauth/hrapplications/templates/hrapplications/corpchoice.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/create.html` & `allianceauth-4.1.0/allianceauth/hrapplications/templates/hrapplications/create.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/management.html` & `allianceauth-4.1.0/allianceauth/hrapplications/templates/hrapplications/management.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/partials/modals/search.html` & `allianceauth-4.1.0/allianceauth/hrapplications/templates/hrapplications/partials/modals/search.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/searchview.html` & `allianceauth-4.1.0/allianceauth/hrapplications/templates/hrapplications/searchview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/templates/hrapplications/view.html` & `allianceauth-4.1.0/allianceauth/hrapplications/templates/hrapplications/view.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/tests.py` & `allianceauth-4.1.0/allianceauth/hrapplications/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/urls.py` & `allianceauth-4.1.0/allianceauth/hrapplications/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/hrapplications/views.py` & `allianceauth-4.1.0/allianceauth/hrapplications/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/cs/LC_MESSAGES/django.mo` & `allianceauth-4.1.0/allianceauth/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/cs/LC_MESSAGES/django.po` & `allianceauth-4.1.0/allianceauth/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/de/LC_MESSAGES/django.mo` & `allianceauth-4.1.0/allianceauth/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/de/LC_MESSAGES/django.po` & `allianceauth-4.1.0/allianceauth/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/en/LC_MESSAGES/django.po` & `allianceauth-4.1.0/allianceauth/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/es/LC_MESSAGES/django.mo` & `allianceauth-4.1.0/allianceauth/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/es/LC_MESSAGES/django.po` & `allianceauth-4.1.0/allianceauth/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo` & `allianceauth-4.1.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/fr_FR/LC_MESSAGES/django.po` & `allianceauth-4.1.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/it_IT/LC_MESSAGES/django.mo` & `allianceauth-4.1.0/allianceauth/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/it_IT/LC_MESSAGES/django.po` & `allianceauth-4.1.0/allianceauth/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/ja/LC_MESSAGES/django.mo` & `allianceauth-4.1.0/allianceauth/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/ja/LC_MESSAGES/django.po` & `allianceauth-4.1.0/allianceauth/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo` & `allianceauth-4.1.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/ko_KR/LC_MESSAGES/django.po` & `allianceauth-4.1.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/nl/LC_MESSAGES/django.mo` & `allianceauth-4.1.0/allianceauth/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/nl/LC_MESSAGES/django.po` & `allianceauth-4.1.0/allianceauth/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/pl_PL/LC_MESSAGES/django.mo` & `allianceauth-4.1.0/allianceauth/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/pl_PL/LC_MESSAGES/django.po` & `allianceauth-4.1.0/allianceauth/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/ru/LC_MESSAGES/django.mo` & `allianceauth-4.1.0/allianceauth/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/ru/LC_MESSAGES/django.po` & `allianceauth-4.1.0/allianceauth/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/uk/LC_MESSAGES/django.mo` & `allianceauth-4.1.0/allianceauth/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/uk/LC_MESSAGES/django.po` & `allianceauth-4.1.0/allianceauth/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo` & `allianceauth-4.1.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po` & `allianceauth-4.1.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/admin.py` & `allianceauth-4.1.0/allianceauth/menu/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/core/menu_item_hooks.py` & `allianceauth-4.1.0/allianceauth/menu/core/menu_item_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/core/smart_sync.py` & `allianceauth-4.1.0/allianceauth/menu/core/smart_sync.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/filters.py` & `allianceauth-4.1.0/allianceauth/menu/filters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/forms.py` & `allianceauth-4.1.0/allianceauth/menu/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/hooks.py` & `allianceauth-4.1.0/allianceauth/menu/hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/managers.py` & `allianceauth-4.1.0/allianceauth/menu/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/menu/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/models.py` & `allianceauth-4.1.0/allianceauth/menu/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-item-bs5.html` & `allianceauth-4.1.0/allianceauth/menu/templates/menu/menu-item-bs5.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-notification-block.html` & `allianceauth-4.1.0/allianceauth/menu/templates/menu/menu-notification-block.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/templates/menu/menu-user.html` & `allianceauth-4.1.0/allianceauth/menu/templates/menu/menu-user.html`

 * *Files 2% similar despite different names*

```diff
@@ -56,23 +56,25 @@
                     <li><h6 class="dropdown-header">{% translate "Super User" %}</h6></li>
                     <li>
                         <a class="dropdown-item"  href="https://allianceauth.readthedocs.io/" title="Alliance Auth Documentation"><i class="fa-solid fa-book fa-fw"></i> Alliance Auth Documentation</a>
                     </li>
                     <li>
                         <a class="dropdown-item"  href="https://discord.gg/fjnHAmk" title="Alliance Auth Discord"><i class="fa-brands fa-discord fa-fw"></i> Alliance Auth Discord</a>
                     </li>
-                        <li>
-                            <a class="dropdown-item" href="https://gitlab.com/allianceauth/allianceauth" title="Alliance Auth Git"><i class="fa-brands fa-gitlab fa-fw"></i> Alliance Auth Git</a>
-                        </li>
                     <li>
-                        <a class="dropdown-item" href="{% url 'admin:index' %}">
-                            <i class="fa-solid fa-gear fa-fw"></i> {% translate "Admin" %}
-                        </a>
+                        <a class="dropdown-item" href="https://gitlab.com/allianceauth/allianceauth" title="Alliance Auth Git"><i class="fa-brands fa-gitlab fa-fw"></i> Alliance Auth Git</a>
                     </li>
                 {% endif %}
+                {% if user.is_staff %}
+                <li>
+                    <a class="dropdown-item" href="{% url 'admin:index' %}">
+                        <i class="fa-solid fa-gear fa-fw"></i> {% translate "Admin" %}
+                    </a>
+                </li>
+                {% endif %}
                 <li><hr class="dropdown-divider"></li>
                 {% if user.is_authenticated %}
                     <li>
                         <a class="dropdown-item" href="{% url 'authentication:token_management' %}">
                             <i class="fa-solid fa-user-lock fa-fw"></i> Token Management
                         </a>
                     </li>
```

### Comparing `allianceauth-4.0.2/allianceauth/menu/templates/menu/sortable-side-menu.html` & `allianceauth-4.1.0/allianceauth/menu/templates/menu/sortable-side-menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/templatetags/menu_items.py` & `allianceauth-4.1.0/allianceauth/menu/templatetags/menu_items.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/templatetags/menu_menu_items.py` & `allianceauth-4.1.0/allianceauth/menu/templatetags/menu_menu_items.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/tests/core/test_menu_item_hooks.py` & `allianceauth-4.1.0/allianceauth/menu/tests/core/test_menu_item_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/tests/core/test_smart_sync.py` & `allianceauth-4.1.0/allianceauth/menu/tests/core/test_smart_sync.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/tests/factories.py` & `allianceauth-4.1.0/allianceauth/menu/tests/factories.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/tests/integration/test_admin.py` & `allianceauth-4.1.0/allianceauth/menu/tests/integration/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/tests/integration/test_dashboard.py` & `allianceauth-4.1.0/allianceauth/menu/tests/integration/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/tests/templatetags/test_menu_items.py` & `allianceauth-4.1.0/allianceauth/menu/tests/templatetags/test_menu_items.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/tests/templatetags/test_menu_menu_items.py` & `allianceauth-4.1.0/allianceauth/menu/tests/templatetags/test_menu_menu_items.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/tests/test_forms.py` & `allianceauth-4.1.0/allianceauth/menu/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/tests/test_hooks.py` & `allianceauth-4.1.0/allianceauth/menu/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/tests/test_managers.py` & `allianceauth-4.1.0/allianceauth/menu/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/tests/test_models.py` & `allianceauth-4.1.0/allianceauth/menu/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/menu/tests/utils.py` & `allianceauth-4.1.0/allianceauth/menu/tests/utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/admin.py` & `allianceauth-4.1.0/allianceauth/notifications/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/core.py` & `allianceauth-4.1.0/allianceauth/notifications/core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/handlers.py` & `allianceauth-4.1.0/allianceauth/notifications/handlers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/managers.py` & `allianceauth-4.1.0/allianceauth/notifications/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py` & `allianceauth-4.1.0/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/migrations/0004_performance_tuning.py` & `allianceauth-4.1.0/allianceauth/notifications/migrations/0004_performance_tuning.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/migrations/0005_fix_level_choices.py` & `allianceauth-4.1.0/allianceauth/notifications/migrations/0005_fix_level_choices.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/models.py` & `allianceauth-4.1.0/allianceauth/notifications/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/templates/notifications/list.html` & `allianceauth-4.1.0/allianceauth/notifications/templates/notifications/list.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/templates/notifications/list_partial.html` & `allianceauth-4.1.0/allianceauth/notifications/templates/notifications/list_partial.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/templates/notifications/view.html` & `allianceauth-4.1.0/allianceauth/notifications/templates/notifications/view.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/templatetags/auth_notifications.py` & `allianceauth-4.1.0/allianceauth/notifications/templatetags/auth_notifications.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/tests/test_core.py` & `allianceauth-4.1.0/allianceauth/notifications/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/tests/test_handlers.py` & `allianceauth-4.1.0/allianceauth/notifications/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/tests/test_init.py` & `allianceauth-4.1.0/allianceauth/notifications/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/tests/test_managers.py` & `allianceauth-4.1.0/allianceauth/notifications/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/tests/test_models.py` & `allianceauth-4.1.0/allianceauth/notifications/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/tests/test_templatetags.py` & `allianceauth-4.1.0/allianceauth/notifications/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/tests/test_views.py` & `allianceauth-4.1.0/allianceauth/notifications/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/urls.py` & `allianceauth-4.1.0/allianceauth/notifications/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/notifications/views.py` & `allianceauth-4.1.0/allianceauth/notifications/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/optimer/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/optimer/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/optimer/form.py` & `allianceauth-4.1.0/allianceauth/optimer/form.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/optimer/form_widgets.py` & `allianceauth-4.1.0/allianceauth/optimer/form_widgets.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/optimer/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/optimer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py` & `allianceauth-4.1.0/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/optimer/migrations/0005_add_type_and_description.py` & `allianceauth-4.1.0/allianceauth/optimer/migrations/0005_add_type_and_description.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/optimer/models.py` & `allianceauth-4.1.0/allianceauth/optimer/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/optimer/templates/optimer/add.html` & `allianceauth-4.1.0/allianceauth/optimer/templates/optimer/add.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/optimer/templates/optimer/fleetoptable.html` & `allianceauth-4.1.0/allianceauth/optimer/templates/optimer/fleetoptable.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/optimer/templates/optimer/management.html` & `allianceauth-4.1.0/allianceauth/optimer/templates/optimer/management.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/optimer/templates/optimer/update.html` & `allianceauth-4.1.0/allianceauth/optimer/templates/optimer/update.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/optimer/views.py` & `allianceauth-4.1.0/allianceauth/optimer/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/permissions_tool/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/permissions_tool/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/permissions_tool/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/permissions_tool/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/permissions_tool/templates/permissions_tool/audit.html` & `allianceauth-4.1.0/allianceauth/permissions_tool/templates/permissions_tool/audit.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html` & `allianceauth-4.1.0/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/permissions_tool/templates/permissions_tool/overview.html` & `allianceauth-4.1.0/allianceauth/permissions_tool/templates/permissions_tool/overview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/permissions_tool/tests.py` & `allianceauth-4.1.0/allianceauth/permissions_tool/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/permissions_tool/views.py` & `allianceauth-4.1.0/allianceauth/permissions_tool/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/project_template/manage.py` & `allianceauth-4.1.0/allianceauth/project_template/manage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/project_template/project_name/celery.py` & `allianceauth-4.1.0/allianceauth/project_template/project_name/celery.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/project_template/project_name/settings/base.py` & `allianceauth-4.1.0/allianceauth/project_template/project_name/settings/base.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/project_template/project_name/settings/local.py` & `allianceauth-4.1.0/allianceauth/project_template/project_name/settings/local.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/project_template/supervisor.conf` & `allianceauth-4.1.0/allianceauth/project_template/supervisor.conf`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/abstract.py` & `allianceauth-4.1.0/allianceauth/services/abstract.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/admin.py` & `allianceauth-4.1.0/allianceauth/services/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/services/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/forms.py` & `allianceauth-4.1.0/allianceauth/services/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/hooks.py` & `allianceauth-4.1.0/allianceauth/services/hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/migrations/0002_nameformatter.py` & `allianceauth-4.1.0/allianceauth/services/migrations/0002_nameformatter.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/migrations/0003_remove_broken_link.py` & `allianceauth-4.1.0/allianceauth/services/migrations/0003_remove_broken_link.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/models.py` & `allianceauth-4.1.0/allianceauth/services/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/admin.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/api.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/api.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/app_settings.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/core.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/app_settings.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/client.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/client.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/exceptions.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/helpers.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/models.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/example_objects.json` & `allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/example_objects.json`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/factories.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/factories.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md` & `allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_client.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/discord_client/tests/test_models.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/discord_client/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/managers.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/migrations/0002_service_permissions.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/models.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/tasks.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html` & `allianceauth-4.1.0/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/factories.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/tests/factories.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/piloting_tasks.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/tests/piloting_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_admin.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_api.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_auth_hooks.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_core.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_integration.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_managers.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_models.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_tasks.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_utils.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/tests/test_views.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/urls.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/utils.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discord/views.py` & `allianceauth-4.1.0/allianceauth/services/modules/discord/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discourse/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/services/modules/discourse/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discourse/manager.py` & `allianceauth-4.1.0/allianceauth/services/modules/discourse/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discourse/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/services/modules/discourse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py` & `allianceauth-4.1.0/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discourse/models.py` & `allianceauth-4.1.0/allianceauth/services/modules/discourse/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discourse/providers.py` & `allianceauth-4.1.0/allianceauth/services/modules/discourse/providers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discourse/tasks.py` & `allianceauth-4.1.0/allianceauth/services/modules/discourse/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discourse/templates/services/discourse/discourse_service_ctrl.html` & `allianceauth-4.1.0/allianceauth/services/modules/discourse/templates/services/discourse/discourse_service_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discourse/tests.py` & `allianceauth-4.1.0/allianceauth/services/modules/discourse/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/discourse/views.py` & `allianceauth-4.1.0/allianceauth/services/modules/discourse/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/example/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/services/modules/example/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/ips4/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/services/modules/ips4/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/ips4/manager.py` & `allianceauth-4.1.0/allianceauth/services/modules/ips4/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/ips4/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/services/modules/ips4/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py` & `allianceauth-4.1.0/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/ips4/models.py` & `allianceauth-4.1.0/allianceauth/services/modules/ips4/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/ips4/tasks.py` & `allianceauth-4.1.0/allianceauth/services/modules/ips4/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/ips4/tests.py` & `allianceauth-4.1.0/allianceauth/services/modules/ips4/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/ips4/views.py` & `allianceauth-4.1.0/allianceauth/services/modules/ips4/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/models.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/tasks.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/tests.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/urls.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/mumble/views.py` & `allianceauth-4.1.0/allianceauth/services/modules/mumble/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/openfire/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/services/modules/openfire/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/openfire/manager.py` & `allianceauth-4.1.0/allianceauth/services/modules/openfire/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/openfire/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/services/modules/openfire/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py` & `allianceauth-4.1.0/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/openfire/tasks.py` & `allianceauth-4.1.0/allianceauth/services/modules/openfire/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html` & `allianceauth-4.1.0/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/openfire/tests.py` & `allianceauth-4.1.0/allianceauth/services/modules/openfire/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/openfire/urls.py` & `allianceauth-4.1.0/allianceauth/services/modules/openfire/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/openfire/views.py` & `allianceauth-4.1.0/allianceauth/services/modules/openfire/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/phpbb3/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/services/modules/phpbb3/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/phpbb3/manager.py` & `allianceauth-4.1.0/allianceauth/services/modules/phpbb3/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/phpbb3/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/services/modules/phpbb3/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py` & `allianceauth-4.1.0/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/phpbb3/tasks.py` & `allianceauth-4.1.0/allianceauth/services/modules/phpbb3/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/phpbb3/tests.py` & `allianceauth-4.1.0/allianceauth/services/modules/phpbb3/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/phpbb3/views.py` & `allianceauth-4.1.0/allianceauth/services/modules/phpbb3/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/smf/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/services/modules/smf/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/smf/manager.py` & `allianceauth-4.1.0/allianceauth/services/modules/smf/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/smf/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/services/modules/smf/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/smf/migrations/0002_service_permissions.py` & `allianceauth-4.1.0/allianceauth/services/modules/smf/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py` & `allianceauth-4.1.0/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/smf/tasks.py` & `allianceauth-4.1.0/allianceauth/services/modules/smf/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/smf/tests.py` & `allianceauth-4.1.0/allianceauth/services/modules/smf/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/smf/views.py` & `allianceauth-4.1.0/allianceauth/services/modules/smf/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/admin.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/manager.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/models.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/signals.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/tasks.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/tests.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/urls.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/util/ts3.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/util/ts3.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/teamspeak3/views.py` & `allianceauth-4.1.0/allianceauth/services/modules/teamspeak3/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/xenforo/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/services/modules/xenforo/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/xenforo/manager.py` & `allianceauth-4.1.0/allianceauth/services/modules/xenforo/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/xenforo/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/services/modules/xenforo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py` & `allianceauth-4.1.0/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/xenforo/tasks.py` & `allianceauth-4.1.0/allianceauth/services/modules/xenforo/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/xenforo/tests.py` & `allianceauth-4.1.0/allianceauth/services/modules/xenforo/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/xenforo/urls.py` & `allianceauth-4.1.0/allianceauth/services/modules/xenforo/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/modules/xenforo/views.py` & `allianceauth-4.1.0/allianceauth/services/modules/xenforo/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/signals.py` & `allianceauth-4.1.0/allianceauth/services/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/tasks.py` & `allianceauth-4.1.0/allianceauth/services/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/templates/services/fleetformattertool.html` & `allianceauth-4.1.0/allianceauth/services/templates/services/fleetformattertool.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/templates/services/service_confirm_delete.html` & `allianceauth-4.1.0/allianceauth/services/templates/services/service_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/templates/services/service_credentials.html` & `allianceauth-4.1.0/allianceauth/services/templates/services/service_credentials.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/templates/services/service_password.html` & `allianceauth-4.1.0/allianceauth/services/templates/services/service_password.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/templates/services/services.html` & `allianceauth-4.1.0/allianceauth/services/templates/services/services.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/templates/services/services_ctrl.html` & `allianceauth-4.1.0/allianceauth/services/templates/services/services_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/templates/services/services_ctrl_base.html` & `allianceauth-4.1.0/allianceauth/services/templates/services/services_ctrl_base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/tests/test_hooks.py` & `allianceauth-4.1.0/allianceauth/services/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/tests/test_models.py` & `allianceauth-4.1.0/allianceauth/services/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/tests/test_nameformatter.py` & `allianceauth-4.1.0/allianceauth/services/tests/test_nameformatter.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/tests/test_signals.py` & `allianceauth-4.1.0/allianceauth/services/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/tests/test_tasks.py` & `allianceauth-4.1.0/allianceauth/services/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/urls.py` & `allianceauth-4.1.0/allianceauth/services/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/services/views.py` & `allianceauth-4.1.0/allianceauth/services/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/srp/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/form.py` & `allianceauth-4.1.0/allianceauth/srp/form.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/managers.py` & `allianceauth-4.1.0/allianceauth/srp/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/srp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/migrations/0003_make_strings_more_stringy.py` & `allianceauth-4.1.0/allianceauth/srp/migrations/0003_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/migrations/0004_on_delete.py` & `allianceauth-4.1.0/allianceauth/srp/migrations/0004_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/models.py` & `allianceauth-4.1.0/allianceauth/srp/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/swagger.json` & `allianceauth-4.1.0/allianceauth/srp/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/templates/srp/add.html` & `allianceauth-4.1.0/allianceauth/srp/templates/srp/add.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/templates/srp/data.html` & `allianceauth-4.1.0/allianceauth/srp/templates/srp/data.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/templates/srp/management.html` & `allianceauth-4.1.0/allianceauth/srp/templates/srp/management.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/templates/srp/request.html` & `allianceauth-4.1.0/allianceauth/srp/templates/srp/request.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/templates/srp/update.html` & `allianceauth-4.1.0/allianceauth/srp/templates/srp/update.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/tests/test_managers.py` & `allianceauth-4.1.0/allianceauth/srp/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json` & `allianceauth-4.1.0/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/urls.py` & `allianceauth-4.1.0/allianceauth/srp/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/srp/views.py` & `allianceauth-4.1.0/allianceauth/srp/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/css/auth-base.css` & `allianceauth-4.1.0/allianceauth/static/allianceauth/css/auth-base.css`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/css/checkbox.css` & `allianceauth-4.1.0/allianceauth/static/allianceauth/css/checkbox.css`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less` & `allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/darkly/LICENSE` & `allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/darkly/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/darkly/darkly.less` & `allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.less`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css` & `allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly-shared.less` & `allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/flatly-shared.less`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly/LICENSE` & `allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/flatly/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly/flatly.less` & `allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.less`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css` & `allianceauth-4.1.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/allianceauth.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/icons/allianceauth.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/android-chrome-192x192.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/icons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/android-chrome-512x512.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/icons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/apple-touch-icon.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon-16x16.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon-32x32.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon-96x96.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/favicon.ico` & `allianceauth-4.1.0/allianceauth/static/allianceauth/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/mstile-150x150.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/icons/safari-pinned-tab.svg` & `allianceauth-4.1.0/allianceauth/static/allianceauth/icons/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/images/auth-logo.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/images/auth-logo.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/images/auth-logo.svg` & `allianceauth-4.1.0/allianceauth/static/allianceauth/images/auth-logo.svg`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/eve-time.js` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/eve-time.js`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/filterDropDown/LICENSE` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/filterDropDown/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_444444_256x240.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_555555_256x240.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777620_256x240.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777777_256x240.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_cc0000_256x240.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_ffffff_256x240.png` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/jquery-ui.min.css` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/jquery-ui/1.13.2/css/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/refresh-notification-icon.js` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/refresh-notification-icon.js`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/refresh_notifications.js` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/refresh_notifications.js`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/timerboard.js` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/timerboard.js`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/static/allianceauth/js/timers.js` & `allianceauth-4.1.0/allianceauth/static/allianceauth/js/timers.js`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/allianceauth/admin-status/esi_check.html` & `allianceauth-4.1.0/allianceauth/templates/allianceauth/admin-status/esi_check.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/allianceauth/admin-status/overview.html` & `allianceauth-4.1.0/allianceauth/templates/allianceauth/admin-status/overview.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,63 @@
 {% load i18n %}
 {% load humanize %}
 
 {% if notifications %}
     <div id="aa-dashboard-panel-admin-notifications" class="col-12 align-self-stretch pb-2">
         <div class="card">
             <div class="card-body">
-                <div class="d-flex align-items-center">
-                    <div class="w-100 align-self-stretch">
-                        <h4 class="ms-auto me-auto text-center">
-                            {% translate "Alliance Auth Notifications" %}
-                        </h4>
-
-                        <div class="card-body">
-                            <ul class="list-group">
-                                {% for notif in notifications %}
-                                    <li class="list-group-item">
-                                        {% if notif.state == 'opened' %}
-                                            <span class="badge bg-success">{% translate "Open" %}</span>
-                                        {% else %}
-                                            <span class="badge bg-danger">{% translate "Closed" %}</span>
-                                        {% endif %}
-                                        <a href="{{ notif.web_url }}" target="_blank">#{{ notif.iid }} {{ notif.title }}</a>
-                                    </li>
-                                {% empty %}
-                                    <div class="alert alert-primary" role="alert">
-                                        {% translate "No notifications at this time" %}
-                                    </div>
-                                {% endfor %}
-                            </ul>
-
-                            <div class="text-end">
-                                <a href="https://gitlab.com/allianceauth/allianceauth/issues" target="_blank" class="me-1">
-                                    <span class="badge" style="background-color: rgb(230 83 40);">
-                                        <i class="fab fa-gitlab" aria-hidden="true"></i>
-                                        {% translate 'Powered by GitLab' %}
-                                    </span>
-                                </a>
-                                <a href="https://discord.com/invite/fjnHAmk" target="_blank">
-                                    <span class="badge" style="background-color: rgb(110 133 211);">
-                                        <i class="fab fa-discord" aria-hidden="true"></i>
-                                        {% translate 'Support Discord' %}
-                                    </span>
-                                </a>
+                {% translate "Alliance Auth Notifications" as widget_title %}
+                {% include "framework/dashboard/widget-title.html" with title=widget_title %}
+
+                <div>
+                    <ul class="list-group">
+                        {% for notif in notifications %}
+                            <li class="list-group-item">
+                                {% if notif.state == 'opened' %}
+                                    <span class="badge bg-success">{% translate "Open" %}</span>
+                                {% else %}
+                                    <span class="badge bg-danger">{% translate "Closed" %}</span>
+                                {% endif %}
+                                <a href="{{ notif.web_url }}" target="_blank">#{{ notif.iid }} {{ notif.title }}</a>
+                            </li>
+                        {% empty %}
+                            <div class="alert alert-primary" role="alert">
+                                {% translate "No notifications at this time" %}
                             </div>
-                        </div>
+                        {% endfor %}
+                    </ul>
+
+                    <div class="text-end pt-3">
+                        <a href="https://gitlab.com/allianceauth/allianceauth/issues" target="_blank" class="me-1 text-decoration-none">
+                            <span class="badge" style="background-color: rgb(230 83 40);">
+                                <i class="fab fa-gitlab" aria-hidden="true"></i>
+                                {% translate 'Powered by GitLab' %}
+                            </span>
+                        </a>
+                        <a href="https://discord.com/invite/fjnHAmk" target="_blank" class="text-decoration-none">
+                            <span class="badge" style="background-color: rgb(110 133 211);">
+                                <i class="fab fa-discord" aria-hidden="true"></i>
+                                {% translate 'Support Discord' %}
+                            </span>
+                        </a>
                     </div>
                 </div>
             </div>
         </div>
     </div>
 {% endif %}
 
-<div class="col-12 align-self-stretch pb-2">
+<div class="col-12 align-self-stretch py-2">
     <div class="card">
-        <div class="card-body d-flex flex-row flex-wrap">
+        <div class="card-body row">
             <div id="aa-dashboard-panel-software-version" class="col-xl-6 col-lg-12 col-md-12 col-sm-12">
-                <h4 class="ms-auto me-auto text-center">
-                    {% translate "Software Version" %}
-                </h4>
+                {% translate "Software Version" as widget_title %}
+                {% include "framework/dashboard/widget-title.html" with title=widget_title %}
 
-                <div class="card-body">
+                <div>
                     <ul class="list-group list-group-horizontal w-100" role="group" aria-label="{% translate 'Software Version' %}">
                         <li class="list-group-item w-100">
                             <div class="btn h-100 w-100 cursor-default">
                                 <h5 class="list-group-item-heading">{% translate "Current" %}</h5>
                                 <p class="list-group-item-text">{{ current_version }}</p>
                             </div>
                         </li>
@@ -94,19 +88,18 @@
                             </li>
                         {% endif %}
                     </ul>
                 </div>
             </div>
 
             <div id="aa-dashboard-panel-task-queue" class="col-xl-6 col-lg-12 col-md-12 col-sm-12">
-                <h4 class="ms-auto me-auto text-center">
-                    {% translate "Task Queue" %}
-                </h4>
+                {% translate "Task Queue" as widget_title %}
+                {% include "framework/dashboard/widget-title.html" with title=widget_title %}
 
-                <div class="card-body">
+                <div>
                     <p>
                         {% blocktranslate with total=tasks_total|intcomma latest=earliest_task|timesince|default:"?" %}
                             Status of {{ total }} processed tasks • last {{ latest }}
                         {% endblocktranslate %}
                     </p>
 
                     <div
```

#### html2text {}

```diff
@@ -1,30 +1,33 @@
 {% load i18n %} {% load humanize %} {% if notifications %}
-****** {{%% ttrraannssllaattee ""AAlllliiaannccee AAuutthh NNoottiiffiiccaattiioonnss"" %%}} ******
+{% translate "Alliance Auth Notifications" as widget_title %} {% include
+"framework/dashboard/widget-title.html" with title=widget_title %}
     * {% for notif in notifications %}
     * {% if notif.state == 'opened' %} {% translate "Open" %} {% else %} {%
       translate "Closed" %} {% endif %} _#_{_{_ _n_o_t_i_f_._i_i_d_ _}_}_ _{_{_ _n_o_t_i_f_._t_i_t_l_e_ _}_}
     * {% empty %}
       {% translate "No notifications at this time" %}
     * {% endfor %}
 _{_%_ _t_r_a_n_s_l_a_t_e_ _'_P_o_w_e_r_e_d_ _b_y_ _G_i_t_L_a_b_'_ _%_}
 _{_%_ _t_r_a_n_s_l_a_t_e_ _'_S_u_p_p_o_r_t_ _D_i_s_c_o_r_d_'_ _%_}
 {% endif %}
-****** {{%% ttrraannssllaattee ""SSooffttwwaarree VVeerrssiioonn"" %%}} ******
+{% translate "Software Version" as widget_title %} {% include "framework/
+dashboard/widget-title.html" with title=widget_title %}
     * **** {{%% ttrraannssllaattee ""CCuurrrreenntt"" %%}} ****
       {{ current_version }}
     * _**_**_ _{{_%%_ _tt_rr_aa_nn_ss_ll_aa_tt_ee_ _""_LL_aa_tt_ee_ss_tt_ _SS_tt_aa_bb_ll_ee_""_ _%%_}}_ _**_**
       _{_{_ _l_a_t_e_s_t___p_a_t_c_h___v_e_r_s_i_o_n_ _}_}_ _{_%_ _i_f_ _n_o_t_ _l_a_t_e_s_t___p_a_t_c_h_ _%_}
       _{_%_ _t_r_a_n_s_l_a_t_e_ _"_U_p_d_a_t_e_ _a_v_a_i_l_a_b_l_e_"_ _%_}_{_%_ _e_n_d_i_f_ _%_}
     * {% if latest_beta %}
     * _**_**_ _{{_%%_ _tt_rr_aa_nn_ss_ll_aa_tt_ee_ _""_LL_aa_tt_ee_ss_tt_ _PP_rr_ee_--_RR_ee_ll_ee_aa_ss_ee_""_ _%%_}}_ _**_**
       _{_{_ _l_a_t_e_s_t___b_e_t_a___v_e_r_s_i_o_n_ _}_}
       _{_%_ _t_r_a_n_s_l_a_t_e_ _"_P_r_e_-_R_e_l_e_a_s_e_ _a_v_a_i_l_a_b_l_e_"_ _%_}
     * {% endif %}
-****** {{%% ttrraannssllaattee ""TTaasskk QQuueeuuee"" %%}} ******
+{% translate "Task Queue" as widget_title %} {% include "framework/dashboard/
+widget-title.html" with title=widget_title %}
 {% blocktranslate with total=tasks_total|intcomma
 latest=earliest_task|timesince|default:"?" %} Status of {{ total }} processed
 tasks â¢ last {{ latest }} {% endblocktranslate %}
 {% include "allianceauth/admin-status/celery_bar_partial.html" with
 label="suceeded" level="success" tasks_count=tasks_succeeded %} {% include
 "allianceauth/admin-status/celery_bar_partial.html" with label="retried"
 level="info" tasks_count=tasks_retried %} {% include "allianceauth/admin-
```

### Comparing `allianceauth-4.0.2/allianceauth/templates/allianceauth/base-bs5.html` & `allianceauth-4.1.0/allianceauth/templates/allianceauth/base-bs5.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/allianceauth/base.html` & `allianceauth-4.1.0/allianceauth/templates/allianceauth/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/allianceauth/error.html` & `allianceauth-4.1.0/allianceauth/templates/allianceauth/error.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/allianceauth/icons.html` & `allianceauth-4.1.0/allianceauth/templates/allianceauth/icons.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/allianceauth/messages-bs5.html` & `allianceauth-4.1.0/allianceauth/templates/allianceauth/messages-bs5.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/allianceauth/messages.html` & `allianceauth-4.1.0/allianceauth/templates/allianceauth/messages.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/allianceauth/side-menu.html` & `allianceauth-4.1.0/allianceauth/templates/allianceauth/side-menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu-admin.html` & `allianceauth-4.1.0/allianceauth/templates/allianceauth/top-menu-admin.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu-rh-default.html` & `allianceauth-4.1.0/allianceauth/templates/allianceauth/top-menu-rh-default.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu-user-dropdown.html` & `allianceauth-4.1.0/allianceauth/templates/allianceauth/top-menu-user-dropdown.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/allianceauth/top-menu.html` & `allianceauth-4.1.0/allianceauth/templates/allianceauth/top-menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/bundles/bootstrap-css.html` & `allianceauth-4.1.0/allianceauth/templates/bundles/bootstrap-css.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/bundles/bootstrap-js.html` & `allianceauth-4.1.0/allianceauth/templates/bundles/bootstrap-js.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/bundles/datatables-js-bs5.html` & `allianceauth-4.1.0/allianceauth/templates/bundles/datatables-js-bs5.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/bundles/datatables-js.html` & `allianceauth-4.1.0/allianceauth/templates/bundles/datatables-js.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templates/bundles/moment-js.html` & `allianceauth-4.1.0/allianceauth/templates/bundles/moment-js.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/templatetags/admin_status.py` & `allianceauth-4.1.0/allianceauth/templatetags/admin_status.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/tests/auth_utils.py` & `allianceauth-4.1.0/allianceauth/tests/auth_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/tests/test_auth_utils.py` & `allianceauth-4.1.0/allianceauth/tests/test_auth_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/tests/test_urls.py` & `allianceauth-4.1.0/allianceauth/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/tests/test_views.py` & `allianceauth-4.1.0/allianceauth/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/theme/bootstrap/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/theme/bootstrap/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/theme/darkly/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/theme/darkly/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/theme/flatly/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/theme/flatly/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/theme/hooks.py` & `allianceauth-4.1.0/allianceauth/theme/hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/theme/materia/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/theme/materia/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/theme/templatetags/theme_tags.py` & `allianceauth-4.1.0/allianceauth/theme/templatetags/theme_tags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/thirdparty/navhelper/templatetags/navactive.py` & `allianceauth-4.1.0/allianceauth/thirdparty/navhelper/templatetags/navactive.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/thirdparty/navhelper/tests.py` & `allianceauth-4.1.0/allianceauth/thirdparty/navhelper/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/auth_hooks.py` & `allianceauth-4.1.0/allianceauth/timerboard/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/form.py` & `allianceauth-4.1.0/allianceauth/timerboard/form.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/migrations/0001_initial.py` & `allianceauth-4.1.0/allianceauth/timerboard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py` & `allianceauth-4.1.0/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/migrations/0003_on_delete.py` & `allianceauth-4.1.0/allianceauth/timerboard/migrations/0003_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/migrations/0004_timer_type.py` & `allianceauth-4.1.0/allianceauth/timerboard/migrations/0004_timer_type.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/models.py` & `allianceauth-4.1.0/allianceauth/timerboard/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/dashboard.timers.html` & `allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/dashboard.timers.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 {% load i18n %}
 {% load evelinks %}
 
 <div class="col-12 align-self-stretch py-2">
     <div class="card h-100">
         <div class="card-body">
-            <h4 class="card-title text-center">{% translate "Upcoming Timers" %}</h4>
-            <div class="card-body">
-                <div>
-                    <table class="table">
-                        <thead>
+            {% translate "Upcoming Timers" as widget_title %}
+            {% include "framework/dashboard/widget-title.html" with title=widget_title %}
+
+            <div>
+                <table class="table">
+                    <thead>
+                        <tr>
+                            <th class="text-center">{% translate "Details" %}</th>
+                            <th class="text-center">{% translate "Timer" %}</th>
+                            <th class="text-center">{% translate "Type" %}</th>
+                            <th class="text-center">{% translate "System" %}</th>
+                            <th class="text-center">{% translate "EVE Time" %}</th>
+                        </tr>
+                    </thead>
+
+                    <tbody>
+                        {% for timer in timers %}
                             <tr>
-                                <th class="text-center">{% translate "Details" %}</th>
-                                <th class="text-center">{% translate "Timer" %}</th>
-                                <th class="text-center">{% translate "Type" %}</th>
-                                <th class="text-center">{% translate "System" %}</th>
-                                <th class="text-center">{% translate "EVE Time" %}</th>
+                                <td class="text-center">
+                                    {{ timer.details }}
+                                </td>
+                                <td class="text-center">
+                                    {{ timer.get_timer_type_display }}
+                                </td>
+                                <td class="text-center" nowrap>
+                                    {% if timer.objective == "Hostile" %}
+                                        <div class="badge bg-danger">
+                                            {% translate "Hostile" %}
+                                        </div>
+                                    {% endif %}
+                                    {% if timer.objective == "Friendly" %}
+                                        <div class="badge bg-primary">
+                                            {% translate "Friendly" %}
+                                        </div>
+                                    {% endif %}
+                                    {% if timer.objective == "Neutral" %}
+                                        <div class="badge bg-default">
+                                            {% translate "Neutral" %}
+                                        </div>
+                                    {% endif %}
+                                </td>
+                                <td class="text-center"><a href="{{ timer.system|dotlan_solar_system_url }}">
+                                    {{ timer.system }} {{ timer.planet_moon }}
+                                    </a>
+                                </td>
+                                <td class="text-center" nowrap>{{ timer.eve_time | date:"Y-m-d H:i" }}</td>
                             </tr>
-                        </thead>
-
-                        <tbody>
-                            {% for timer in timers %}
-                                <tr>
-                                    <td class="text-center">
-                                        {{ timer.details }}
-                                    </td>
-                                    <td class="text-center">
-                                        {{ timer.get_timer_type_display }}
-                                    </td>
-                                    <td class="text-center" nowrap>
-                                        {% if timer.objective == "Hostile" %}
-                                            <div class="badge bg-danger">
-                                                {% translate "Hostile" %}
-                                            </div>
-                                        {% endif %}
-                                        {% if timer.objective == "Friendly" %}
-                                            <div class="badge bg-primary">
-                                                {% translate "Friendly" %}
-                                            </div>
-                                        {% endif %}
-                                        {% if timer.objective == "Neutral" %}
-                                            <div class="badge bg-default">
-                                                {% translate "Neutral" %}
-                                            </div>
-                                        {% endif %}
-                                    </td>
-                                    <td class="text-center"><a href="{{ timer.system|dotlan_solar_system_url }}">
-                                        {{ timer.system }} {{ timer.planet_moon }}
-                                        </a>
-                                    </td>
-                                    <td class="text-center" nowrap>{{ timer.eve_time | date:"Y-m-d H:i" }}</td>
-                                </tr>
-                            {% endfor %}
-                        </tbody>
-                    </table>
-                </div>
+                        {% endfor %}
+                    </tbody>
+                </table>
             </div>
         </div>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% load i18n %} {% load evelinks %}
-****** {{%% ttrraannssllaattee ""UUppccoommiinngg TTiimmeerrss"" %%}} ******
+{% translate "Upcoming Timers" as widget_title %} {% include "framework/
+dashboard/widget-title.html" with title=widget_title %}
 {{%% ttrraannssllaattee  {{%% ttrraannssllaattee ""TTiimmeerr"" %%}}      {{%% ttrraannssllaattee    {{%% ttrraannssllaattee      {{%% ttrraannssllaattee
 ""DDeettaaiillss"" %%}}                               ""TTyyppee"" %%}}       ""SSyysstteemm"" %%}}       ""EEVVEE TTiimmee"" %%}}
                                            {% if
                                            timer.objective
                                            == "Hostile" %}
                                            {% translate
                                            "Hostile" %}
```

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/form.html` & `allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/form.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html` & `allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timer_create_form.html` & `allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/timer_create_form.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timer_update_form.html` & `allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/timer_update_form.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/timertable.html` & `allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/timertable.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/templates/timerboard/view.html` & `allianceauth-4.1.0/allianceauth/timerboard/templates/timerboard/view.html`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/tests.py` & `allianceauth-4.1.0/allianceauth/timerboard/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/timerboard/views.py` & `allianceauth-4.1.0/allianceauth/timerboard/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     def form_valid(self, form):
         messages.success(self.request, _('Saved changes to the timer.'))
         return super().form_valid(form)
 
 
 class RemoveTimerView(TimerManagementView, DeleteView):
-    form_class = TimerForm
+    pass
 
 
 def dashboard_timers(request):
     if request.user.has_perm(TIMER_VIEW_PERMISSION):
         try:
             corp = request.user.profile.main_character.corporation
         except (EveCorporationInfo.DoesNotExist, AttributeError):
```

### Comparing `allianceauth-4.0.2/allianceauth/urls.py` & `allianceauth-4.1.0/allianceauth/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/utils/cache.py` & `allianceauth-4.1.0/allianceauth/utils/cache.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/utils/counters.py` & `allianceauth-4.1.0/allianceauth/utils/counters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/utils/django.py` & `allianceauth-4.1.0/allianceauth/utils/django.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/utils/testing.py` & `allianceauth-4.1.0/allianceauth/utils/testing.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/utils/tests/test_cache.py` & `allianceauth-4.1.0/allianceauth/utils/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/utils/tests/test_counters.py` & `allianceauth-4.1.0/allianceauth/utils/tests/test_counters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/utils/tests/test_django.py` & `allianceauth-4.1.0/allianceauth/utils/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/allianceauth/views.py` & `allianceauth-4.1.0/allianceauth/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/pyproject.toml` & `allianceauth-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `allianceauth-4.0.2/PKG-INFO` & `allianceauth-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth
-Version: 4.0.2
+Version: 4.1.0
 Summary: An auth system for EVE Online to help in-game organizations
 Keywords: allianceauth,eveonline
 Author-email: Alliance Auth <adarnof@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

