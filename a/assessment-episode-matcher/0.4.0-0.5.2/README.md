# Comparing `tmp/assessment_episode_matcher-0.4.0.tar.gz` & `tmp/assessment_episode_matcher-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assessment_episode_matcher-0.4.0.tar", last modified: Sun May 26 01:12:40 2024, max compression
+gzip compressed data, was "assessment_episode_matcher-0.5.2.tar", last modified: Mon May 27 04:17:03 2024, max compression
```

## Comparing `assessment_episode_matcher-0.4.0.tar` & `assessment_episode_matcher-0.5.2.tar`

### file list

```diff
@@ -1,66 +1,69 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.569871 assessment_episode_matcher-0.4.0/
--rw-rw-rw-   0        0        0     1235 2024-05-17 18:46:24.000000 assessment_episode_matcher-0.4.0/LICENSE
--rw-rw-rw-   0        0        0       26 2024-05-23 22:46:12.000000 assessment_episode_matcher-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0      523 2024-05-26 01:12:40.566872 assessment_episode_matcher-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-05-24 22:35:01.000000 assessment_episode_matcher-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.263395 assessment_episode_matcher-0.4.0/assessment_episode_matcher/
--rw-rw-rw-   0        0        0      275 2024-05-23 23:19:26.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/__init__.py
--rw-rw-rw-   0        0        0      267 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/audits.py
-drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.338348 assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/__init__.py
--rw-rw-rw-   0        0        0     4487 2024-05-26 00:55:49.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/az_blob_query.py
--rw-rw-rw-   0        0        0     9458 2024-05-22 23:27:05.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/az_tables_query.py
--rw-rw-rw-   0        0        0     1067 2024-05-26 01:04:22.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/file_types.py
--rw-rw-rw-   0        0        0     3921 2024-05-18 20:57:07.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.362000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/configs/
--rw-rw-rw-   0        0        0        0 2024-05-24 21:35:01.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/configs/__init__.py
--rw-rw-rw-   0        0        0      972 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/configs/audit.py
--rw-rw-rw-   0        0        0      604 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/configs/episodes.py
--rw-rw-rw-   0        0        0     8591 2024-05-17 22:40:20.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/data_config.py
--rw-rw-rw-   0        0        0     5365 2024-05-17 19:24:47.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/data_prep.py
-drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.377893 assessment_episode_matcher-0.4.0/assessment_episode_matcher/exporters/
--rw-rw-rw-   0        0        0     1615 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/exporters/NADAbase.py
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/exporters/__init__.py
--rw-rw-rw-   0        0        0     2409 2024-05-26 01:03:13.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/exporters/main.py
-drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.410041 assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/__init__.py
--rw-rw-rw-   0        0        0    13006 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/aod.py
--rw-rw-rw-   0        0        0     8834 2024-05-26 01:07:05.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/assessments.py
--rw-rw-rw-   0        0        0     6726 2024-05-26 00:23:34.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/episodes.py
--rw-rw-rw-   0        0        0     2941 2024-05-23 02:41:28.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/main.py
-drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.451591 assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/__init__.py
--rw-rw-rw-   0        0        0     4403 2024-05-18 20:54:57.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/date_checks.py
--rw-rw-rw-   0        0        0     5697 2024-05-26 01:09:01.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/errors.py
--rw-rw-rw-   0        0        0     5321 2024-05-18 20:55:18.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/increasing_slack.py
--rw-rw-rw-   0        0        0    21314 2024-05-22 23:38:15.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/main.py
--rw-rw-rw-   0        0        0     1004 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/matching_stats.py
--rw-rw-rw-   0        0        0     1993 2024-05-19 23:10:24.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/mytypes.py
-drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.471242 assessment_episode_matcher-0.4.0/assessment_episode_matcher/setup/
--rw-rw-rw-   0        0        0        0 2024-05-19 22:35:00.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/setup/__init__.py
--rw-rw-rw-   0        0        0     4933 2024-05-26 00:16:34.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/setup/bootstrap.py
--rw-rw-rw-   0        0        0     2318 2024-05-19 22:34:48.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/setup/log_management.py
--rw-rw-rw-   0        0        0     8652 2024-05-26 01:04:25.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/test_surveytxt.py
-drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.485705 assessment_episode_matcher-0.4.0/assessment_episode_matcher/tests/
--rw-rw-rw-   0        0        0       23 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/tests/__init__.py
--rw-rw-rw-   0        0        0     1377 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/tests/matching_test.py
-drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.547697 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/
--rw-rw-rw-   0        0        0        0 2024-05-17 21:30:48.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/__init__.py
--rw-rw-rw-   0        0        0     1270 2024-05-18 20:54:35.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/base.py
--rw-rw-rw-   0        0        0     1693 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/ccare_to_aztable.py
--rw-rw-rw-   0        0        0    13615 2024-05-19 23:11:34.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/df_ops_base.py
--rw-rw-rw-   0        0        0     7323 2024-05-18 19:37:57.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/dtypes.py
--rw-rw-rw-   0        0        0     1557 2024-05-22 23:17:51.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/environment.py
--rw-rw-rw-   0        0        0     1972 2024-05-22 23:41:56.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/fromstr.py
--rw-rw-rw-   0        0        0      748 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/group_utils.py
--rw-rw-rw-   0        0        0    11458 2024-05-25 23:06:26.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/io.py
--rw-rw-rw-   0        0        0       21 2024-05-26 01:12:15.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher/version.py
-drwxrwxrwx   0        0        0        0 2024-05-26 01:12:40.561874 assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/
--rw-rw-rw-   0        0        0      523 2024-05-26 01:12:40.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2290 2024-05-26 01:12:40.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 01:12:40.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-05-26 01:12:40.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-26 01:12:40.000000 assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2024-05-17 19:08:24.000000 assessment_episode_matcher-0.4.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 01:12:40.570870 assessment_episode_matcher-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1342 2024-05-24 03:53:56.000000 assessment_episode_matcher-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:17:03.412838 assessment_episode_matcher-0.5.2/
+-rw-rw-rw-   0        0        0     1235 2024-05-17 18:46:24.000000 assessment_episode_matcher-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0       26 2024-05-23 22:46:12.000000 assessment_episode_matcher-0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      523 2024-05-27 04:17:03.407787 assessment_episode_matcher-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2024-05-27 04:16:19.000000 assessment_episode_matcher-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 04:17:02.806818 assessment_episode_matcher-0.5.2/assessment_episode_matcher/
+-rw-rw-rw-   0        0        0      275 2024-05-23 23:19:26.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/__init__.py
+-rw-rw-rw-   0        0        0      267 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/audits.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:17:02.904542 assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/__init__.py
+-rw-rw-rw-   0        0        0     5165 2024-05-27 01:14:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/az_blob_query.py
+-rw-rw-rw-   0        0        0     9458 2024-05-22 23:27:05.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/az_tables_query.py
+-rw-rw-rw-   0        0        0     1594 2024-05-27 02:50:37.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/file_types.py
+-rw-rw-rw-   0        0        0     3921 2024-05-18 20:57:07.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:17:02.932368 assessment_episode_matcher-0.5.2/assessment_episode_matcher/configs/
+-rw-rw-rw-   0        0        0        0 2024-05-24 21:35:01.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/configs/__init__.py
+-rw-rw-rw-   0        0        0      972 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/configs/audit.py
+-rw-rw-rw-   0        0        0      631 2024-05-26 21:44:37.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/configs/episodes.py
+-rw-rw-rw-   0        0        0     8591 2024-05-17 22:40:20.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/data_config.py
+-rw-rw-rw-   0        0        0     5899 2024-05-27 00:25:15.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/data_prep.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:17:02.953173 assessment_episode_matcher-0.5.2/assessment_episode_matcher/exporters/
+-rw-rw-rw-   0        0        0     1848 2024-05-26 23:42:24.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/exporters/NADAbase.py
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/exporters/__init__.py
+-rw-rw-rw-   0        0        0     3850 2024-05-27 01:14:46.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/exporters/main.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:17:03.009614 assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/__init__.py
+-rw-rw-rw-   0        0        0    14368 2024-05-27 02:49:09.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/aod.py
+-rw-rw-rw-   0        0        0     8836 2024-05-26 22:49:07.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/assessments.py
+-rw-rw-rw-   0        0        0     6681 2024-05-26 21:50:05.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/episodes.py
+-rw-rw-rw-   0        0        0     3749 2024-05-27 00:19:22.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/main.py
+-rw-rw-rw-   0        0        0     1485 2024-05-26 23:26:37.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/nada_indexed.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:17:03.101048 assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/__init__.py
+-rw-rw-rw-   0        0        0     4403 2024-05-18 20:54:57.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/date_checks.py
+-rw-rw-rw-   0        0        0     4510 2024-05-27 03:27:36.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/errors.py
+-rw-rw-rw-   0        0        0     5321 2024-05-18 20:55:18.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/increasing_slack.py
+-rw-rw-rw-   0        0        0    21314 2024-05-22 23:38:15.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/main.py
+-rw-rw-rw-   0        0        0     1004 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/matching_stats.py
+-rw-rw-rw-   0        0        0     2592 2024-05-27 02:55:23.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/mytypes.py
+-rw-rw-rw-   0        0        0     3965 2024-05-27 03:29:54.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/nada.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:17:03.140411 assessment_episode_matcher-0.5.2/assessment_episode_matcher/setup/
+-rw-rw-rw-   0        0        0        0 2024-05-19 22:35:00.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/setup/__init__.py
+-rw-rw-rw-   0        0        0     4933 2024-05-26 00:16:34.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/setup/bootstrap.py
+-rw-rw-rw-   0        0        0     2318 2024-05-19 22:34:48.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/setup/log_management.py
+-rw-rw-rw-   0        0        0     8870 2024-05-27 03:01:01.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/test_surveytxt.py
+-rw-rw-rw-   0        0        0     8366 2024-05-26 22:16:46.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/test_surveytxt_local.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:17:03.215437 assessment_episode_matcher-0.5.2/assessment_episode_matcher/tests/
+-rw-rw-rw-   0        0        0       23 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/tests/__init__.py
+-rw-rw-rw-   0        0        0     1377 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/tests/matching_test.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:17:03.371374 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-17 21:30:48.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/__init__.py
+-rw-rw-rw-   0        0        0     1270 2024-05-18 20:54:35.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/base.py
+-rw-rw-rw-   0        0        0     1693 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/ccare_to_aztable.py
+-rw-rw-rw-   0        0        0    13615 2024-05-19 23:11:34.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/df_ops_base.py
+-rw-rw-rw-   0        0        0     7323 2024-05-18 19:37:57.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/dtypes.py
+-rw-rw-rw-   0        0        0     1557 2024-05-22 23:17:51.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/environment.py
+-rw-rw-rw-   0        0        0     1972 2024-05-22 23:41:56.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/fromstr.py
+-rw-rw-rw-   0        0        0      748 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/group_utils.py
+-rw-rw-rw-   0        0        0    11458 2024-05-25 23:06:26.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/io.py
+-rw-rw-rw-   0        0        0       21 2024-05-27 04:15:38.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher/version.py
+drwxrwxrwx   0        0        0        0 2024-05-27 04:17:03.383132 assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/
+-rw-rw-rw-   0        0        0      523 2024-05-27 04:17:02.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2429 2024-05-27 04:17:02.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 04:17:02.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-05-27 04:17:02.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-27 04:17:02.000000 assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2024-05-17 19:08:24.000000 assessment_episode_matcher-0.5.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 04:17:03.416469 assessment_episode_matcher-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1342 2024-05-24 03:53:56.000000 assessment_episode_matcher-0.5.2/setup.py
```

### Comparing `assessment_episode_matcher-0.4.0/LICENSE` & `assessment_episode_matcher-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/PKG-INFO` & `assessment_episode_matcher-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assessment_episode_matcher
-Version: 0.4.0
+Version: 0.5.2
 Author: Aftab Jalal
 Author-email: mj@auditlytics.nz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/az_blob_query.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/az_blob_query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 
 import logging
 from typing import Any
 from io import BytesIO
 import pandas as pd
 from azure.storage.blob import BlobServiceClient #, BlobClient, ContainerClient
 
+from assessment_episode_matcher.mytypes import CSVTypeObject
 from assessment_episode_matcher.utils.environment import ConfigKeys, ConfigManager
-from assessment_episode_matcher.azutil.file_types import BlobCSVFilePrepper, BlobParquetFilePrepper
+from assessment_episode_matcher.azutil.file_types import BlobCSVFilePrepper, BlobDataFrameCSVFilePrepper, BlobDataFrameParquetFilePrepper
 # import mylogging
 
 # logging = mylogging.get('azure.storage')
 
 
 class AzureBlobQuery(object):
   def __init__(self):
@@ -39,46 +40,61 @@
       
 
   # @st.cache
   def load_data(self, container_name, blob_url):
       
       try:
         # blob_service_client = BlobServiceClient.from_connection_string(self.connection_string)
-        blob_client = self.blob_service_client.get_blob_client(container=container_name, blob=blob_url)
+        blob_client = self.blob_service_client\
+                          .get_blob_client(container=container_name
+                                           , blob=blob_url)
         blob_data = blob_client.download_blob().readall()
 
         logging.debug(f"Loaded blob bytes of length {len(blob_data)}.")
    
         return BytesIO(blob_data)
       
       except Exception as e:
         # Log the exception
         logging.error(f"An error occurred while loading data from Blob Storage: {str(e)}")
         # You may want to display a user-friendly message in the Streamlit app
         # st.warning("An error occurred while loading the data. Please try again later.")
         return None       
 
 
-  def write_data(self, container_name:str, blob_url:str
+  def write_dataframe(self, container_name:str, blob_url:str
                  , data:pd.DataFrame) -> dict[str, Any]:
 
     blob_client = self.blob_service_client.get_blob_client(container=container_name
                                                       , blob=blob_url)
     if blob_url[-3:] =='csv':
-      p = BlobCSVFilePrepper()
-      file = p.get_file_for_blob(data)
+      p = BlobDataFrameCSVFilePrepper()    
     else:
-      p = BlobParquetFilePrepper()
-      file = p.get_file_for_blob(data)
+      p = BlobDataFrameParquetFilePrepper()
+      
+    file = p.get_file_for_blob(data)
        
     result_dict = blob_client.upload_blob(file, overwrite=True)
 
-    return result_dict 
+    return result_dict
+  
+
 
+  def write_csv(self, container_name:str, blob_url:str
+                 , data:CSVTypeObject) -> dict[str, Any]:
+    
+    csvprep = BlobCSVFilePrepper()
+    csv_data = csvprep.get_file_for_blob(data)
 
+    # Upload the CSV data to Azure Blob Storage
+    blob_client = self.blob_service_client \
+                  .get_blob_client(container=container_name
+                                  , blob=blob_url)
+    result_dict = blob_client.upload_blob(csv_data, overwrite=True)
+    return result_dict
 
   # def _get_parquet(self, df:pd.DataFrame) -> bytes:
   #   with tempfile.TemporaryDirectory() as temp_dir:
   #       temp_file_path = os.path.join(temp_dir, "temp.parquet")
   #       df.to_parquet(temp_file_path, engine="pyarrow")
 
   #       # Read the Parquet file into memory
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/az_tables_query.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/az_tables_query.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/file_types.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/file_types.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,59 @@
 import os
+import csv
 from abc import ABC, abstractmethod
 from typing import Any
 # from enum import Enum, auto
 from io import StringIO
 import tempfile
 import pandas as pd
 
+from assessment_episode_matcher.mytypes import CSVTypeObject
+
 # class BlobFileType(Enum):
 #    CSV =  auto()
 #    PARQUET = auto()
 
 class BlobFilePrepper(ABC):
   # file_type: BlobFileType
   
   @abstractmethod
-  def get_file_for_blob(self, data:pd.DataFrame) -> Any:
+  def get_file_for_blob(self, data:Any) -> Any:
     pass   
    
 
-class BlobParquetFilePrepper(BlobFilePrepper):
+class BlobDataFrameParquetFilePrepper(BlobFilePrepper):
   
   def get_file_for_blob(self, data:pd.DataFrame):
     with tempfile.TemporaryDirectory() as temp_dir:
         temp_file_path = os.path.join(temp_dir, "temp.parquet")
         data.to_parquet(temp_file_path, engine="pyarrow")
 
         # Read the Parquet file into memory
         with open(temp_file_path, "rb") as file:
             parquet_data = file.read()
             return parquet_data
         
 
-class BlobCSVFilePrepper(BlobFilePrepper):
+class BlobDataFrameCSVFilePrepper(BlobFilePrepper):
   
   def get_file_for_blob(self, data:pd.DataFrame):
     csv_buffer = StringIO()
     data.to_csv(csv_buffer, index=False)
     return csv_buffer.getvalue()
+
+
+class BlobCSVFilePrepper(BlobFilePrepper):
+  
+  def get_file_for_blob(self, data:CSVTypeObject):
+    # Create a buffer to store the CSV data
+    buffer = StringIO()
+    writer = csv.writer(buffer, quoting=csv.QUOTE_ALL)
+    
+    writer.writerow(data.header)
+
+    for warning in data.rows:
+      writer.writerow(warning.to_list())
+
+    # Get the CSV data from the buffer
+    csv_data = buffer.getvalue()
+    return csv_data
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/azutil/helper.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/azutil/helper.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/configs/audit.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/configs/audit.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/configs/episodes.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/configs/episodes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
   # List of columns we care about
   
 date_cols=['START DATE', 'END DATE']
 
 columns_of_interest = ['ESTABLISHMENT IDENTIFIER', 'GEOGRAPHICAL LOCATION'
                          , 'EPISODE ID','PERSON ID', 'SPECIFY DRUG OF CONCERN'
-                         , 'PRINCIPAL DRUG OF CONCERN'
+                         , 'PRINCIPAL DRUG OF CONCERN', 'STAFF'
                          , 'START DATE', 'END DATE', 'SLK']
 rename_columns = {
     'SPECIFY DRUG OF CONCERN': 'PDCSubstanceOfConcern',
-    'PRINCIPAL DRUG OF CONCERN': 'PDCCode',
+    'PRINCIPAL DRUG OF CONCERN': 'PDCCode', 'STAFF': 'Staff',
     'START DATE': 'CommencementDate', 'END DATE': 'EndDate',
     'EPISODE ID': 'PMSEpisodeID', 'PERSON ID': 'PMSPersonID',    
 }
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/data_config.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/data_config.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/data_prep.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/data_prep.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,336 +1,369 @@
 00000000: 0d0a 696d 706f 7274 206c 6f67 6769 6e67  ..import logging
 00000010: 0d0a 2320 6672 6f6d 2074 7970 696e 6720  ..# from typing 
 00000020: 696d 706f 7274 204f 7074 696f 6e61 6c0d  import Optional.
 00000030: 0a69 6d70 6f72 7420 7061 6e64 6173 2061  .import pandas a
-00000040: 7320 7064 0d0a 0d0a 6672 6f6d 2064 6174  s pd....from dat
-00000050: 615f 636f 6e66 6967 2069 6d70 6f72 7420  a_config import 
-00000060: 6b65 6570 5f70 6172 656e 745f 6669 656c  keep_parent_fiel
-00000070: 6473 2c20 6d75 6c73 656c 6563 745f 6f70  ds, mulselect_op
-00000080: 7469 6f6e 5f74 6f5f 6e61 6461 6669 656c  tion_to_nadafiel
-00000090: 640d 0a66 726f 6d20 6d79 7479 7065 7320  d..from mytypes 
-000000a0: 696d 706f 7274 2050 7572 706f 7365 0d0a  import Purpose..
-000000b0: 6672 6f6d 2075 7469 6c73 2e62 6173 6520  from utils.base 
-000000c0: 696d 706f 7274 2063 6865 636b 5f66 6f72  import check_for
-000000d0: 5f73 7472 696e 670d 0a66 726f 6d20 7574  _string..from ut
-000000e0: 696c 732e 6474 7970 6573 2069 6d70 6f72  ils.dtypes impor
-000000f0: 7420 6669 785f 6e75 6d65 7269 6373 0d0a  t fix_numerics..
-00000100: 6672 6f6d 2075 7469 6c73 2e64 665f 6f70  from utils.df_op
-00000110: 735f 6261 7365 2069 6d70 6f72 7420 636f  s_base import co
-00000120: 6e63 6174 5f64 726f 705f 7061 7265 6e74  ncat_drop_parent
-00000130: 2c20 5c0d 0a20 2020 2020 2020 2020 2020  , \..           
-00000140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000150: 2064 726f 705f 6669 656c 6473 5f62 795f   drop_fields_by_
-00000160: 7265 6765 7820 5c0d 0a20 2020 2020 2020  regex \..       
-00000170: 2020 2020 2020 2020 2020 2020 2020 202c                 ,
-00000180: 2020 2064 726f 705f 6669 656c 6473 2c5c     drop_fields,\
-00000190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000001a0: 2020 2020 2020 2020 2020 2020 746f 5f6e              to_n
-000001b0: 756d 5f79 6e5f 6e6f 6e65 2c20 746f 5f6e  um_yn_none, to_n
-000001c0: 756d 5f62 6f6f 6c5f 6e6f 6e65 2c74 7261  um_bool_none,tra
-000001d0: 6e73 666f 726d 5f6d 756c 7469 706c 650d  nsform_multiple.
-000001e0: 0a66 726f 6d20 7574 696c 732e 6672 6f6d  .from utils.from
-000001f0: 7374 7220 696d 706f 7274 2063 6c65 616e  str import clean
-00000200: 5f61 6e64 5f70 6172 7365 5f6a 736f 6e0d  _and_parse_json.
-00000210: 0a66 726f 6d20 696d 706f 7274 6572 732e  .from importers.
-00000220: 616f 6420 696d 706f 7274 2065 7870 616e  aod import expan
-00000230: 645f 6472 7567 5f69 6e66 6f0d 0a0d 0a23  d_drug_info....#
-00000240: 206c 6f67 6765 7220 3d20 6d79 6c6f 6767   logger = mylogg
-00000250: 6572 2e67 6574 285f 5f6e 616d 655f 5f29  er.get(__name__)
-00000260: 0d0a 0d0a 0d0a 6465 6620 6765 745f 7375  ......def get_su
-00000270: 7276 6579 6461 7461 5f65 7870 616e 6465  rveydata_expande
-00000280: 6428 6466 3a20 7064 2e44 6174 6146 7261  d(df: pd.DataFra
-00000290: 6d65 2c20 7072 6570 5f74 7970 653a 2050  me, prep_type: P
-000002a0: 7572 706f 7365 2920 2d3e 2070 642e 4461  urpose) -> pd.Da
-000002b0: 7461 4672 616d 653a 0d0a 2020 2020 6466  taFrame:..    df
-000002c0: 5f73 7572 7665 7964 6174 6120 3d20 6466  _surveydata = df
-000002d0: 5b27 5375 7276 6579 4461 7461 275d 2e61  ['SurveyData'].a
-000002e0: 7070 6c79 2863 6c65 616e 5f61 6e64 5f70  pply(clean_and_p
-000002f0: 6172 7365 5f6a 736f 6e29 0d0a 2020 2020  arse_json)..    
-00000300: 0d0a 2020 2020 2320 4669 6c74 6572 206f  ..    # Filter o
-00000310: 7574 2069 6e76 616c 6964 206f 7220 6d69  ut invalid or mi
-00000320: 7373 696e 6720 4a53 4f4e 2064 6174 610d  ssing JSON data.
-00000330: 0a20 2020 2076 616c 6964 5f73 7572 7665  .    valid_surve
-00000340: 7964 6174 6120 3d20 6466 5f73 7572 7665  ydata = df_surve
-00000350: 7964 6174 612e 6170 706c 7928 6c61 6d62  ydata.apply(lamb
-00000360: 6461 2078 3a20 6973 696e 7374 616e 6365  da x: isinstance
-00000370: 2878 2c20 6469 6374 2929 0d0a 2020 2020  (x, dict))..    
-00000380: 6466 5f73 7572 7665 7964 6174 6120 3d20  df_surveydata = 
-00000390: 6466 5f73 7572 7665 7964 6174 615b 7661  df_surveydata[va
-000003a0: 6c69 645f 7375 7276 6579 6461 7461 5d0d  lid_surveydata].
-000003b0: 0a20 2020 200d 0a20 2020 2064 665f 7375  .    ..    df_su
-000003c0: 7276 6579 6461 7461 5f65 7870 616e 6465  rveydata_expande
-000003d0: 6420 3d20 7064 2e6a 736f 6e5f 6e6f 726d  d = pd.json_norm
-000003e0: 616c 697a 6528 6466 5f73 7572 7665 7964  alize(df_surveyd
-000003f0: 6174 612e 746f 6c69 7374 2829 2c20 6d61  ata.tolist(), ma
-00000400: 785f 6c65 7665 6c3d 3129 0d0a 2020 2020  x_level=1)..    
-00000410: 0d0a 2020 2020 6966 2070 7265 705f 7479  ..    if prep_ty
-00000420: 7065 203d 3d20 5075 7270 6f73 652e 4d41  pe == Purpose.MA
-00000430: 5443 4849 4e47 3a0d 0a20 2020 2020 2020  TCHING:..       
-00000440: 2064 665f 7375 7276 6579 6461 7461 5f65   df_surveydata_e
-00000450: 7870 616e 6465 6420 3d20 6466 5f73 7572  xpanded = df_sur
-00000460: 7665 7964 6174 615f 6578 7061 6e64 6564  veydata_expanded
-00000470: 5b5b 2743 6c69 656e 7454 7970 6527 2c20  [['ClientType', 
-00000480: 2750 4443 275d 5d0d 0a20 2020 200d 0a20  'PDC']]..    .. 
-00000490: 2020 2069 6620 6b65 6570 5f70 6172 656e     if keep_paren
-000004a0: 745f 6669 656c 6473 3a20 2327 6b65 6570  t_fields: #'keep
-000004b0: 5f70 6172 656e 745f 6669 656c 6473 2720  _parent_fields' 
-000004c0: 696e 206c 6f63 616c 7328 293a 0d0a 2020  in locals():..  
-000004d0: 2020 2020 2020 6578 6973 7469 6e67 5f63        existing_c
-000004e0: 6f6c 756d 6e73 5f74 6f5f 7265 6d6f 7665  olumns_to_remove
-000004f0: 203d 205b 636f 6c20 666f 7220 636f 6c20   = [col for col 
-00000500: 696e 206b 6565 705f 7061 7265 6e74 5f66  in keep_parent_f
-00000510: 6965 6c64 7320 6966 2063 6f6c 2069 6e20  ields if col in 
-00000520: 6466 5f73 7572 7665 7964 6174 615f 6578  df_surveydata_ex
-00000530: 7061 6e64 6564 2e63 6f6c 756d 6e73 5d0d  panded.columns].
-00000540: 0a20 2020 2020 2020 2069 6620 6578 6973  .        if exis
-00000550: 7469 6e67 5f63 6f6c 756d 6e73 5f74 6f5f  ting_columns_to_
-00000560: 7265 6d6f 7665 3a0d 0a20 2020 2020 2020  remove:..       
-00000570: 2020 2020 2064 665f 7375 7276 6579 6461       df_surveyda
-00000580: 7461 5f65 7870 616e 6465 6420 3d20 6472  ta_expanded = dr
-00000590: 6f70 5f66 6965 6c64 7328 6466 5f73 7572  op_fields(df_sur
-000005a0: 7665 7964 6174 615f 6578 7061 6e64 6564  veydata_expanded
-000005b0: 2c20 6b65 6570 5f70 6172 656e 745f 6669  , keep_parent_fi
-000005c0: 656c 6473 290d 0a20 2020 200d 0a20 2020  elds)..    ..   
-000005d0: 2064 665f 6669 6e61 6c20 3d20 636f 6e63   df_final = conc
-000005e0: 6174 5f64 726f 705f 7061 7265 6e74 2864  at_drop_parent(d
-000005f0: 662e 6c6f 635b 7661 6c69 645f 7375 7276  f.loc[valid_surv
-00000600: 6579 6461 7461 2e69 6e64 6578 5d2c 2064  eydata.index], d
-00000610: 665f 7375 7276 6579 6461 7461 5f65 7870  f_surveydata_exp
-00000620: 616e 6465 642c 2064 726f 705f 7061 7265  anded, drop_pare
-00000630: 6e74 5f6e 616d 653d 2753 7572 7665 7944  nt_name='SurveyD
-00000640: 6174 6127 290d 0a20 2020 200d 0a20 2020  ata')..    ..   
-00000650: 2072 6574 7572 6e20 6466 5f66 696e 616c   return df_final
-00000660: 0d0a 0d0a 0d0a 6465 6620 6e61 6461 6669  ......def nadafi
-00000670: 656c 645f 6672 6f6d 5f6d 756c 7469 7365  eld_from_multise
-00000680: 6c65 6374 2864 6631 3a70 642e 4461 7461  lect(df1:pd.Data
-00000690: 4672 616d 6529 202d 3e20 7064 2e44 6174  Frame) -> pd.Dat
-000006a0: 6146 7261 6d65 3a0d 0a20 2064 663d 2064  aFrame:..  df= d
-000006b0: 6631 2e63 6f70 7928 290d 0a20 2023 206e  f1.copy()..  # n
-000006c0: 6f5f 616e 7377 6572 5f76 616c 7565 203d  o_answer_value =
-000006d0: 202d 3120 2023 2064 6f20 7468 6973 2074   -1  # do this t
-000006e0: 6f67 6574 6865 7220 6c61 7465 7220 666f  ogether later fo
-000006f0: 7220 616c 6c20 6669 656c 6473 2e0d 0a20  r all fields... 
-00000700: 2066 6f72 2041 544f 4d4d 756c 7469 5365   for ATOMMultiSe
-00000710: 6c65 6374 5175 6573 7469 6f6e 2c20 6e61  lectQuestion, na
-00000720: 6461 6669 656c 645f 7365 6172 6368 7374  dafield_searchst
-00000730: 7220 696e 206d 756c 7365 6c65 6374 5f6f  r in mulselect_o
-00000740: 7074 696f 6e5f 746f 5f6e 6164 6166 6965  ption_to_nadafie
-00000750: 6c64 2e69 7465 6d73 2829 3a0d 0a20 2020  ld.items():..   
-00000760: 2066 6f72 206e 6164 6166 6965 6c64 2c20   for nadafield, 
-00000770: 7365 6172 6368 5f73 7472 2069 6e20 6e61  search_str in na
-00000780: 6461 6669 656c 645f 7365 6172 6368 7374  dafield_searchst
-00000790: 722e 6974 656d 7328 293a 0d0a 2020 2020  r.items():..    
-000007a0: 2020 6966 2041 544f 4d4d 756c 7469 5365    if ATOMMultiSe
-000007b0: 6c65 6374 5175 6573 7469 6f6e 206e 6f74  lectQuestion not
-000007c0: 2069 6e20 6466 2e63 6f6c 756d 6e73 3a0d   in df.columns:.
-000007d0: 0a20 2020 2020 2020 206c 6f67 6769 6e67  .        logging
-000007e0: 2e77 6172 6e28 6622 4e6f 2063 6f6c 756d  .warn(f"No colum
-000007f0: 6e20 7b41 544f 4d4d 756c 7469 5365 6c65  n {ATOMMultiSele
-00000800: 6374 5175 6573 7469 6f6e 7d20 6e61 6461  ctQuestion} nada
-00000810: 6669 656c 645f 6672 6f6d 5f6d 756c 7469  field_from_multi
-00000820: 7365 6c65 6374 2229 0d0a 2020 2020 2020  select")..      
-00000830: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
-00000840: 2020 6466 5b6e 6164 6166 6965 6c64 5d20    df[nadafield] 
-00000850: 3d20 6466 5b41 544f 4d4d 756c 7469 5365  = df[ATOMMultiSe
-00000860: 6c65 6374 5175 6573 7469 6f6e 5d2e 6170  lectQuestion].ap
-00000870: 706c 7928 6c61 6d62 6461 2078 3a20 6368  ply(lambda x: ch
-00000880: 6563 6b5f 666f 725f 7374 7269 6e67 2878  eck_for_string(x
-00000890: 2c20 7365 6172 6368 5f73 7472 2929 0d0a  , search_str))..
-000008a0: 0d0a 2020 7265 7475 726e 2064 660d 0a0d  ..  return df...
-000008b0: 0a0d 0a64 6566 2063 6f6e 7665 7274 5f79  ...def convert_y
-000008c0: 6573 5f6e 6f66 6965 6c64 7328 6466 312c  es_nofields(df1,
-000008d0: 2066 6965 6c64 5f6e 616d 6573 293a 0d0a   field_names):..
-000008e0: 2020 7265 7475 726e 2074 7261 6e73 666f    return transfo
-000008f0: 726d 5f6d 756c 7469 706c 6528 6466 312c  rm_multiple(df1,
-00000900: 2066 6965 6c64 5f6e 616d 6573 2c74 6f5f   field_names,to_
-00000910: 6e75 6d5f 796e 5f6e 6f6e 6529 0d0a 0d0a  num_yn_none)....
-00000920: 6465 6620 636f 6e76 6572 745f 7472 7565  def convert_true
-00000930: 5f66 616c 7365 6669 656c 6473 2864 6631  _falsefields(df1
-00000940: 2c20 6669 656c 645f 6e61 6d65 7329 3a0d  , field_names):.
-00000950: 0a20 2072 6574 7572 6e20 7472 616e 7366  .  return transf
-00000960: 6f72 6d5f 6d75 6c74 6970 6c65 2864 6631  orm_multiple(df1
-00000970: 2c20 6669 656c 645f 6e61 6d65 732c 746f  , field_names,to
-00000980: 5f6e 756d 5f62 6f6f 6c5f 6e6f 6e65 290d  _num_bool_none).
-00000990: 0a0d 0a0d 0a64 6566 2070 7265 705f 6461  .....def prep_da
-000009a0: 7461 6672 616d 655f 6d61 7463 6869 6e67  taframe_matching
-000009b0: 2864 663a 7064 2e44 6174 6146 7261 6d65  (df:pd.DataFrame
-000009c0: 293a 0d0a 0d0a 2020 6c6f 6767 696e 672e  ):....  logging.
-000009d0: 6465 6275 6728 6622 7072 6570 5f64 6174  debug(f"prep_dat
-000009e0: 6166 7261 6d65 206f 6620 6c65 6e67 7468  aframe of length
-000009f0: 207b 6c65 6e28 6466 297d 203a 2022 290d   {len(df)} : ").
-00000a00: 0a20 2064 6632 203d 2067 6574 5f73 7572  .  df2 = get_sur
-00000a10: 7665 7964 6174 615f 6578 7061 6e64 6564  veydata_expanded
-00000a20: 2864 662e 636f 7079 2829 2c20 2050 7572  (df.copy(),  Pur
-00000a30: 706f 7365 2e4d 4154 4348 494e 4729 0d0a  pose.MATCHING)..
-00000a40: 0d0a 2020 6466 352c 2077 6172 6e69 6e67  ..  df5, warning
-00000a50: 735f 616f 6420 3d20 6578 7061 6e64 5f64  s_aod = expand_d
-00000a60: 7275 675f 696e 666f 2864 6632 290d 0a20  rug_info(df2).. 
-00000a70: 2072 6574 7572 6e20 6466 352c 2077 6172   return df5, war
-00000a80: 6e69 6e67 735f 616f 640d 0a0d 0a0d 0a64  nings_aod......d
-00000a90: 6566 2070 7265 705f 6461 7461 6672 616d  ef prep_datafram
-00000aa0: 655f 6e61 6461 2864 663a 7064 2e44 6174  e_nada(df:pd.Dat
-00000ab0: 6146 7261 6d65 293a 0d0a 0d0a 2020 6c6f  aFrame):....  lo
-00000ac0: 6767 696e 672e 6465 6275 6728 6622 7072  gging.debug(f"pr
-00000ad0: 6570 5f64 6174 6166 7261 6d65 206f 6620  ep_dataframe of 
-00000ae0: 6c65 6e67 7468 207b 6c65 6e28 6466 297d  length {len(df)}
-00000af0: 203a 2022 290d 0a20 2064 6632 203d 2067   : ")..  df2 = g
-00000b00: 6574 5f73 7572 7665 7964 6174 615f 6578  et_surveydata_ex
-00000b10: 7061 6e64 6564 2864 662e 636f 7079 2829  panded(df.copy()
-00000b20: 2c20 5075 7270 6f73 652e 4e41 4441 290d  , Purpose.NADA).
-00000b30: 0a20 0d0a 2020 6466 3420 3d20 6472 6f70  . ..  df4 = drop
-00000b40: 5f66 6965 6c64 735f 6279 5f72 6567 6578  _fields_by_regex
-00000b50: 2864 6632 2c72 6567 6578 3d27 436f 6d6d  (df2,regex='Comm
-00000b60: 656e 747c 4e6f 7465 7c49 5453 5027 2920  ent|Note|ITSP') 
-00000b70: 2320 7265 6d6f 7665 202a 476f 616c 7320  # remove *Goals 
-00000b80: 6e6f 7465 732c 2073 6f20 646f 2062 6566  notes, so do bef
-00000b90: 6f72 6520 5044 4320 7374 6570 2028 5044  ore PDC step (PD
-00000ba0: 4347 6f61 6c73 2064 726f 7064 6f77 6e29  CGoals dropdown)
-00000bb0: 0d0a 0d0a 2020 6466 352c 2077 6172 6e69  ....  df5, warni
-00000bc0: 6e67 735f 616f 6420 3d20 6578 7061 6e64  ngs_aod = expand
-00000bd0: 5f64 7275 675f 696e 666f 2864 6634 290d  _drug_info(df4).
-00000be0: 0a0d 0a20 2023 2064 6635 3120 3d20 6578  ...  # df51 = ex
-00000bf0: 7061 6e64 5f61 6374 6976 6974 6965 735f  pand_activities_
-00000c00: 696e 666f 2864 6635 290d 0a20 2064 6635  info(df5)..  df5
-00000c10: 3120 3d20 6e61 6461 6669 656c 645f 6672  1 = nadafield_fr
-00000c20: 6f6d 5f6d 756c 7469 7365 6c65 6374 2864  om_multiselect(d
-00000c30: 6635 290d 0a20 2023 2064 6636 203d 2064  f5)..  # df6 = d
-00000c40: 6635 5b64 6635 2e50 4443 5375 6273 7461  f5[df5.PDCSubsta
-00000c50: 6e63 654f 7247 616d 626c 696e 672e 6e6f  nceOrGambling.no
-00000c60: 746e 6128 295d 2320 7265 6d6f 7665 7320  tna()]# removes 
-00000c70: 726f 7773 2077 6974 686f 7574 2050 4443  rows without PDC
-00000c80: 0d0a 2020 0d0a 2020 7965 735f 6e6f 6669  ..  ..  yes_nofi
-00000c90: 656c 6473 203d 205b 2750 6173 7434 576b  elds = ['Past4Wk
-00000ca0: 4265 656e 4172 7265 7374 6564 272c 2027  BeenArrested', '
-00000cb0: 5061 7374 3457 6b48 6176 6559 6f75 5669  Past4WkHaveYouVi
-00000cc0: 6f6c 656e 6365 4162 7573 6976 6527 5d0d  olenceAbusive'].
-00000cd0: 0a0d 0a20 2064 6635 3220 3d20 636f 6e76  ...  df52 = conv
-00000ce0: 6572 745f 7965 735f 6e6f 6669 656c 6473  ert_yes_nofields
-00000cf0: 2864 6635 312c 2079 6573 5f6e 6f66 6965  (df51, yes_nofie
-00000d00: 6c64 7329 0d0a 2020 626f 6f6c 5f66 6965  lds)..  bool_fie
-00000d10: 6c64 7320 3d20 5b27 4154 4f50 486f 6d65  lds = ['ATOPHome
-00000d20: 6c65 7373 272c 0927 4154 4f50 5269 736b  less',.'ATOPRisk
-00000d30: 4576 6963 7469 6f6e 272c 0927 5072 696d  Eviction',.'Prim
-00000d40: 6172 7943 6172 6567 6976 6572 5f30 2d35  aryCaregiver_0-5
-00000d50: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00000d60: 2020 2020 2009 2750 7269 6d61 7279 4361       .'PrimaryCa
-00000d70: 7265 6769 7665 725f 352d 3135 272c 0927  regiver_5-15',.'
-00000d80: 5061 7374 3457 6b5f 5669 6f6c 656e 7454  Past4Wk_ViolentT
-00000d90: 6f59 6f75 272c 5d0d 0a20 2064 6636 203d  oYou',]..  df6 =
-00000da0: 2063 6f6e 7665 7274 5f74 7275 655f 6661   convert_true_fa
-00000db0: 6c73 6566 6965 6c64 7328 6466 3532 2c20  lsefields(df52, 
-00000dc0: 626f 6f6c 5f66 6965 6c64 7329 0d0a 2020  bool_fields)..  
-00000dd0: 200d 0a20 2064 6637 203d 2066 6978 5f6e   ..  df7 = fix_n
-00000de0: 756d 6572 6963 7328 6466 3629 2020 0d0a  umerics(df6)  ..
-00000df0: 2020 6466 372e 7265 6e61 6d65 2863 6f6c    df7.rename(col
-00000e00: 756d 6e73 3d7b 2745 5354 4142 4c49 5348  umns={'ESTABLISH
-00000e10: 4d45 4e54 2049 4445 4e54 4946 4945 5227  MENT IDENTIFIER'
-00000e20: 3a20 2741 6765 6e63 7943 6f64 6527 7d2c  : 'AgencyCode'},
-00000e30: 2069 6e70 6c61 6365 3d54 7275 6529 0d0a   inplace=True)..
-00000e40: 2020 0d0a 2020 6466 3920 3d20 6466 372e    ..  df9 = df7.
-00000e50: 736f 7274 5f76 616c 7565 7328 6279 3d5b  sort_values(by=[
-00000e60: 2253 4c4b 222c 2022 4173 7365 7373 6d65  "SLK", "Assessme
-00000e70: 6e74 4461 7465 225d 290d 0a20 200d 0a20  ntDate"])..  .. 
-00000e80: 206c 6f67 6769 6e67 2e64 6562 7567 2866   logging.debug(f
-00000e90: 2244 6f6e 6520 5072 6570 7069 6e67 2064  "Done Prepping d
-00000ea0: 6622 290d 0a20 2072 6574 7572 6e20 6466  f")..  return df
-00000eb0: 3920 2c20 7761 726e 696e 6773 5f61 6f64  9 , warnings_aod
-00000ec0: 0d0a 0d0a 0d0a 2320 6465 6620 7072 6570  ......# def prep
-00000ed0: 5f64 6174 6166 7261 6d65 2864 663a 7064  _dataframe(df:pd
-00000ee0: 2e44 6174 6146 7261 6d65 2c20 7072 6570  .DataFrame, prep
-00000ef0: 5f74 7970 653a 204c 6974 6572 616c 5b27  _type: Literal['
-00000f00: 4154 4f4d 272c 2027 4e41 4441 272c 2027  ATOM', 'NADA', '
-00000f10: 4d61 7463 6869 6e67 275d 203d 2027 4154  Matching'] = 'AT
-00000f20: 4f4d 2729 3a0d 0a23 2020 2020 2320 6265  OM'):..#    # be
-00000f30: 6361 7573 6520 5072 6f67 7261 6d20 6973  cause Program is
-00000f40: 2069 6e20 5375 7276 6579 4461 7461 0d0a   in SurveyData..
-00000f50: 2020 0d0a 2320 2020 6966 2070 7265 705f    ..#   if prep_
-00000f60: 7479 7065 203d 3d20 274d 6174 6368 696e  type == 'Matchin
-00000f70: 6727 3a0d 0a23 2020 2020 2072 6574 7572  g':..#     retur
-00000f80: 6e20 7072 6570 5f64 6174 6166 7261 6d65  n prep_dataframe
-00000f90: 5f6d 6174 6368 696e 6728 6466 290d 0a0d  _matching(df)...
-00000fa0: 0a23 2020 206c 6f67 6765 722e 6465 6275  .#   logger.debu
-00000fb0: 6728 6622 7072 6570 5f64 6174 6166 7261  g(f"prep_datafra
-00000fc0: 6d65 206f 6620 6c65 6e67 7468 207b 6c65  me of length {le
-00000fd0: 6e28 6466 297d 203a 2022 290d 0a23 2020  n(df)} : ")..#  
-00000fe0: 2064 6632 203d 2067 6574 5f73 7572 7665   df2 = get_surve
-00000ff0: 7964 6174 615f 6578 7061 6e64 6564 2864  ydata_expanded(d
-00001000: 662e 636f 7079 2829 290d 0a0d 0a23 2020  f.copy())....#  
-00001010: 2064 6633 203d 2064 726f 705f 6669 656c   df3 = drop_fiel
-00001020: 6473 2864 6632 2c5b 274f 4443 275d 290d  ds(df2,['ODC']).
-00001030: 0a23 2020 2064 6634 203d 2064 726f 705f  .#   df4 = drop_
-00001040: 636f 6c73 5f63 6f6e 7461 696e 735f 7265  cols_contains_re
-00001050: 6765 7828 6466 332c 2041 544f 4d5f 4452  gex(df3, ATOM_DR
-00001060: 4f50 5f43 4f4c 434f 4e54 4149 4e53 5f52  OP_COLCONTAINS_R
-00001070: 4547 4558 2920 2320 7265 6d6f 7665 202a  EGEX) # remove *
-00001080: 476f 616c 7320 6e6f 7465 732c 2073 6f20  Goals notes, so 
-00001090: 646f 2062 6566 6f72 6520 5044 4320 7374  do before PDC st
-000010a0: 6570 2028 5044 4347 6f61 6c73 2064 726f  ep (PDCGoals dro
-000010b0: 7064 6f77 6e29 0d0a 2320 2020 6466 3520  pdown)..#   df5 
-000010c0: 3d20 6e6f 726d 616c 697a 655f 6669 7273  = normalize_firs
-000010d0: 745f 656c 656d 656e 7428 6466 342c 2750  t_element(df4,'P
-000010e0: 4443 2729 2023 544f 444f 3a20 2864 662c  DC') #TODO: (df,
-000010f0: 274f 4443 2729 2023 206f 6e6c 7920 7461  'ODC') # only ta
-00001100: 6b65 7320 7468 6520 6669 7273 7420 4f44  kes the first OD
-00001110: 4320 2020 0d0a 0d0a 200d 0a23 2020 2064  C   .... ..#   d
-00001120: 6636 203d 2064 6635 5b64 6635 2e50 4443  f6 = df5[df5.PDC
-00001130: 5375 6273 7461 6e63 654f 7247 616d 626c  SubstanceOrGambl
-00001140: 696e 672e 6e6f 746e 6128 295d 2320 7265  ing.notna()]# re
-00001150: 6d6f 7665 7320 726f 7773 2077 6974 686f  moves rows witho
-00001160: 7574 2050 4443 0d0a 0d0a 2320 2020 2320  ut PDC....#   # 
-00001170: 6466 362e 6c6f 635b 3a2c 2750 726f 6772  df6.loc[:,'Progr
-00001180: 616d 275d 203d 2064 6636 5b27 526f 774b  am'] = df6['RowK
-00001190: 6579 275d 2e73 7472 2e73 706c 6974 2827  ey'].str.split('
-000011a0: 5f27 292e 7374 725b 305d 2023 2068 6173  _').str[0] # has
-000011b0: 2074 6f20 6265 206d 6164 6520 696e 746f   to be made into
-000011c0: 2063 6174 6567 6f72 790d 0a23 2020 2064   category..#   d
-000011d0: 6637 203d 2063 6f6e 7665 7274 5f64 7479  f7 = convert_dty
-000011e0: 7065 7328 6466 3629 0d0a 0d0a 2320 2020  pes(df6)....#   
-000011f0: 2320 6466 2e50 4443 4167 6546 6972 7374  # df.PDCAgeFirst
-00001200: 5573 6564 5b28 6466 2e50 4443 4167 6546  Used[(df.PDCAgeF
-00001210: 6972 7374 5573 6564 2e6e 6f74 6e61 2829  irstUsed.notna()
-00001220: 2920 2620 2864 662e 5044 4341 6765 4669  ) & (df.PDCAgeFi
-00001230: 7273 7455 7365 6420 213d 2027 2729 5d2e  rstUsed != '')].
-00001240: 6173 7479 7065 2869 6e74 290d 0a23 2020  astype(int)..#  
-00001250: 2320 2245 7870 6563 7465 6420 6279 7465  # "Expected byte
-00001260: 732c 2067 6f74 2061 2027 696e 7427 206f  s, got a 'int' o
-00001270: 626a 6563 7422 2c20 2743 6f6e 7665 7273  bject", 'Convers
-00001280: 696f 6e20 6661 696c 6564 2066 6f72 2063  ion failed for c
-00001290: 6f6c 756d 6e20 5044 4341 6765 4669 7273  olumn PDCAgeFirs
-000012a0: 7455 7365 6420 7769 7468 2074 7970 6520  tUsed with type 
-000012b0: 6f62 6a65 6374 270d 0a23 2020 2064 6638  object'..#   df8
-000012c0: 203d 2064 726f 705f 6669 656c 6473 2864   = drop_fields(d
-000012d0: 6637 2c20 5b27 5044 4341 6765 4669 7273  f7, ['PDCAgeFirs
-000012e0: 7455 7365 6427 2c5c 0d0a 2320 2020 2020  tUsed',\..#     
-000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001300: 2020 2020 2020 2027 5072 696d 6172 7943         'PrimaryC
-00001310: 6172 6567 6976 6572 272c 2750 6173 7434  aregiver','Past4
-00001320: 576b 416f 6452 6973 6b73 275d 2920 0d0a  WkAodRisks']) ..
-00001330: 2320 2020 2320 2763 616e 6e6f 7420 6d69  #   # 'cannot mi
-00001340: 7820 6c69 7374 2061 6e64 206e 6f6e 2d6c  x list and non-l
-00001350: 6973 742c 206e 6f6e 2d6e 756c 6c20 7661  ist, non-null va
-00001360: 6c75 6573 272c 200d 0a23 2020 2023 2027  lues', ..#   # '
-00001370: 436f 6e76 6572 7369 6f6e 2066 6169 6c65  Conversion faile
-00001380: 6420 666f 7220 636f 6c75 6d6e 2050 7269  d for column Pri
-00001390: 6d61 7279 4361 7265 6769 7665 722c 2050  maryCaregiver, P
-000013a0: 6173 7434 576b 416f 6452 6973 6b73 2077  ast4WkAodRisks w
-000013b0: 6974 6820 7479 7065 206f 626a 6563 7427  ith type object'
-000013c0: 290d 0a0d 0a23 2020 2069 6620 2753 4c4b  )....#   if 'SLK
-000013d0: 2720 696e 2064 6638 2e63 6f6c 756d 6e73  ' in df8.columns
-000013e0: 3a0d 0a23 2020 2020 2064 6638 2e64 726f  :..#     df8.dro
-000013f0: 7028 636f 6c75 6d6e 733d 5b27 534c 4b27  p(columns=['SLK'
-00001400: 5d2c 2069 6e70 6c61 6365 3d54 7275 6529  ], inplace=True)
-00001410: 200d 0a20 200d 0a23 2020 2064 6638 2e72   ..  ..#   df8.r
-00001420: 656e 616d 6528 636f 6c75 6d6e 733d 7b27  ename(columns={'
-00001430: 5061 7274 6974 696f 6e4b 6579 273a 2027  PartitionKey': '
-00001440: 534c 4b27 7d2c 2069 6e70 6c61 6365 3d54  SLK'}, inplace=T
-00001450: 7275 6529 0d0a 2020 0d0a 2320 2020 6466  rue)..  ..#   df
-00001460: 3920 3d20 6466 382e 736f 7274 5f76 616c  9 = df8.sort_val
-00001470: 7565 7328 6279 3d22 4173 7365 7373 6d65  ues(by="Assessme
-00001480: 6e74 4461 7465 2229 0d0a 200d 0a23 2020  ntDate").. ..#  
-00001490: 2064 6639 5b27 5044 4327 5d20 3d20 6466   df9['PDC'] = df
-000014a0: 395b 2750 4443 5375 6273 7461 6e63 654f  9['PDCSubstanceO
-000014b0: 7247 616d 626c 696e 6727 5d0d 0a20 0d0a  rGambling'].. ..
-000014c0: 2320 2020 6c6f 6767 6572 2e64 6562 7567  #   logger.debug
-000014d0: 2866 2244 6f6e 6520 5072 6570 7069 6e67  (f"Done Prepping
-000014e0: 2064 6622 290d 0a23 2020 2072 6574 7572   df")..#   retur
-000014f0: 6e20 6466 39                             n df9
+00000040: 7320 7064 0d0a 0d0a 6672 6f6d 2061 7373  s pd....from ass
+00000050: 6573 736d 656e 745f 6570 6973 6f64 655f  essment_episode_
+00000060: 6d61 7463 6865 722e 6461 7461 5f63 6f6e  matcher.data_con
+00000070: 6669 6720 696d 706f 7274 206b 6565 705f  fig import keep_
+00000080: 7061 7265 6e74 5f66 6965 6c64 732c 206d  parent_fields, m
+00000090: 756c 7365 6c65 6374 5f6f 7074 696f 6e5f  ulselect_option_
+000000a0: 746f 5f6e 6164 6166 6965 6c64 0d0a 6672  to_nadafield..fr
+000000b0: 6f6d 2061 7373 6573 736d 656e 745f 6570  om assessment_ep
+000000c0: 6973 6f64 655f 6d61 7463 6865 722e 6d79  isode_matcher.my
+000000d0: 7479 7065 7320 696d 706f 7274 2050 7572  types import Pur
+000000e0: 706f 7365 0d0a 6672 6f6d 2061 7373 6573  pose..from asses
+000000f0: 736d 656e 745f 6570 6973 6f64 655f 6d61  sment_episode_ma
+00000100: 7463 6865 722e 7574 696c 732e 6261 7365  tcher.utils.base
+00000110: 2069 6d70 6f72 7420 6368 6563 6b5f 666f   import check_fo
+00000120: 725f 7374 7269 6e67 0d0a 6672 6f6d 2061  r_string..from a
+00000130: 7373 6573 736d 656e 745f 6570 6973 6f64  ssessment_episod
+00000140: 655f 6d61 7463 6865 722e 7574 696c 732e  e_matcher.utils.
+00000150: 6474 7970 6573 2069 6d70 6f72 7420 6669  dtypes import fi
+00000160: 785f 6e75 6d65 7269 6373 0d0a 6672 6f6d  x_numerics..from
+00000170: 2061 7373 6573 736d 656e 745f 6570 6973   assessment_epis
+00000180: 6f64 655f 6d61 7463 6865 722e 7574 696c  ode_matcher.util
+00000190: 732e 6466 5f6f 7073 5f62 6173 6520 696d  s.df_ops_base im
+000001a0: 706f 7274 2063 6f6e 6361 745f 6472 6f70  port concat_drop
+000001b0: 5f70 6172 656e 742c 205c 0d0a 2020 2020  _parent, \..    
+000001c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001d0: 2020 2020 2020 2064 726f 705f 6669 656c         drop_fiel
+000001e0: 6473 5f62 795f 7265 6765 7820 5c0d 0a20  ds_by_regex \.. 
+000001f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000200: 2020 2020 2c20 2020 6472 6f70 5f66 6965      ,   drop_fie
+00000210: 6c64 732c 5c0d 0a20 2020 2020 2020 2020  lds,\..         
+00000220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000230: 746f 5f6e 756d 5f79 6e5f 6e6f 6e65 2c20  to_num_yn_none, 
+00000240: 746f 5f6e 756d 5f62 6f6f 6c5f 6e6f 6e65  to_num_bool_none
+00000250: 2c74 7261 6e73 666f 726d 5f6d 756c 7469  ,transform_multi
+00000260: 706c 650d 0a66 726f 6d20 6173 7365 7373  ple..from assess
+00000270: 6d65 6e74 5f65 7069 736f 6465 5f6d 6174  ment_episode_mat
+00000280: 6368 6572 2e75 7469 6c73 2e66 726f 6d73  cher.utils.froms
+00000290: 7472 2069 6d70 6f72 7420 636c 6561 6e5f  tr import clean_
+000002a0: 616e 645f 7061 7273 655f 6a73 6f6e 0d0a  and_parse_json..
+000002b0: 6672 6f6d 2061 7373 6573 736d 656e 745f  from assessment_
+000002c0: 6570 6973 6f64 655f 6d61 7463 6865 722e  episode_matcher.
+000002d0: 696d 706f 7274 6572 732e 616f 6420 696d  importers.aod im
+000002e0: 706f 7274 2065 7870 616e 645f 6472 7567  port expand_drug
+000002f0: 5f69 6e66 6f0d 0a0d 0a23 206c 6f67 6765  _info....# logge
+00000300: 7220 3d20 6d79 6c6f 6767 6572 2e67 6574  r = mylogger.get
+00000310: 285f 5f6e 616d 655f 5f29 0d0a 0d0a 0d0a  (__name__)......
+00000320: 6465 6620 6765 745f 7375 7276 6579 6461  def get_surveyda
+00000330: 7461 5f65 7870 616e 6465 6428 6466 3a20  ta_expanded(df: 
+00000340: 7064 2e44 6174 6146 7261 6d65 0d0a 2020  pd.DataFrame..  
+00000350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000360: 2020 2020 2020 2020 2020 2c20 7072 6570            , prep
+00000370: 5f74 7970 653a 2050 7572 706f 7365 2920  _type: Purpose) 
+00000380: 2d3e 2070 642e 4461 7461 4672 616d 653a  -> pd.DataFrame:
+00000390: 0d0a 2020 2020 6466 5f73 7572 7665 7964  ..    df_surveyd
+000003a0: 6174 6120 3d20 6466 5b27 5375 7276 6579  ata = df['Survey
+000003b0: 4461 7461 275d 2e61 7070 6c79 2863 6c65  Data'].apply(cle
+000003c0: 616e 5f61 6e64 5f70 6172 7365 5f6a 736f  an_and_parse_jso
+000003d0: 6e29 0d0a 2020 2020 0d0a 2020 2020 2320  n)..    ..    # 
+000003e0: 4669 6c74 6572 206f 7574 2069 6e76 616c  Filter out inval
+000003f0: 6964 206f 7220 6d69 7373 696e 6720 4a53  id or missing JS
+00000400: 4f4e 2064 6174 610d 0a20 2020 2076 616c  ON data..    val
+00000410: 6964 5f73 7572 7665 7964 6174 6120 3d20  id_surveydata = 
+00000420: 6466 5f73 7572 7665 7964 6174 612e 6170  df_surveydata.ap
+00000430: 706c 7928 6c61 6d62 6461 2078 3a20 6973  ply(lambda x: is
+00000440: 696e 7374 616e 6365 2878 2c20 6469 6374  instance(x, dict
+00000450: 2929 0d0a 2020 2020 6466 5f73 7572 7665  ))..    df_surve
+00000460: 7964 6174 6120 3d20 6466 5f73 7572 7665  ydata = df_surve
+00000470: 7964 6174 615b 7661 6c69 645f 7375 7276  ydata[valid_surv
+00000480: 6579 6461 7461 5d0d 0a20 2020 200d 0a20  eydata]..    .. 
+00000490: 2020 2064 665f 7375 7276 6579 6461 7461     df_surveydata
+000004a0: 5f65 7870 616e 6465 6420 3d20 7064 2e6a  _expanded = pd.j
+000004b0: 736f 6e5f 6e6f 726d 616c 697a 6528 6466  son_normalize(df
+000004c0: 5f73 7572 7665 7964 6174 612e 746f 6c69  _surveydata.toli
+000004d0: 7374 2829 2c20 6d61 785f 6c65 7665 6c3d  st(), max_level=
+000004e0: 3129 0d0a 2020 2020 0d0a 2020 2020 6966  1)..    ..    if
+000004f0: 2070 7265 705f 7479 7065 203d 3d20 5075   prep_type == Pu
+00000500: 7270 6f73 652e 4d41 5443 4849 4e47 3a0d  rpose.MATCHING:.
+00000510: 0a20 2020 2020 2020 2064 665f 7375 7276  .        df_surv
+00000520: 6579 6461 7461 5f65 7870 616e 6465 6420  eydata_expanded 
+00000530: 3d20 6466 5f73 7572 7665 7964 6174 615f  = df_surveydata_
+00000540: 6578 7061 6e64 6564 5b5b 2743 6c69 656e  expanded[['Clien
+00000550: 7454 7970 6527 2c20 2750 4443 275d 5d0d  tType', 'PDC']].
+00000560: 0a20 2020 200d 0a20 2020 2069 6620 6b65  .    ..    if ke
+00000570: 6570 5f70 6172 656e 745f 6669 656c 6473  ep_parent_fields
+00000580: 3a20 2327 6b65 6570 5f70 6172 656e 745f  : #'keep_parent_
+00000590: 6669 656c 6473 2720 696e 206c 6f63 616c  fields' in local
+000005a0: 7328 293a 0d0a 2020 2020 2020 2020 6578  s():..        ex
+000005b0: 6973 7469 6e67 5f63 6f6c 756d 6e73 5f74  isting_columns_t
+000005c0: 6f5f 7265 6d6f 7665 203d 205b 636f 6c20  o_remove = [col 
+000005d0: 666f 7220 636f 6c20 696e 206b 6565 705f  for col in keep_
+000005e0: 7061 7265 6e74 5f66 6965 6c64 7320 0d0a  parent_fields ..
+000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000610: 2020 2020 2020 6966 2063 6f6c 2069 6e20        if col in 
+00000620: 6466 5f73 7572 7665 7964 6174 615f 6578  df_surveydata_ex
+00000630: 7061 6e64 6564 2e63 6f6c 756d 6e73 5d0d  panded.columns].
+00000640: 0a20 2020 2020 2020 2069 6620 6578 6973  .        if exis
+00000650: 7469 6e67 5f63 6f6c 756d 6e73 5f74 6f5f  ting_columns_to_
+00000660: 7265 6d6f 7665 3a0d 0a20 2020 2020 2020  remove:..       
+00000670: 2020 2020 2064 665f 7375 7276 6579 6461       df_surveyda
+00000680: 7461 5f65 7870 616e 6465 6420 3d20 6472  ta_expanded = dr
+00000690: 6f70 5f66 6965 6c64 7328 6466 5f73 7572  op_fields(df_sur
+000006a0: 7665 7964 6174 615f 6578 7061 6e64 6564  veydata_expanded
+000006b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000006c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006e0: 2020 202c 206b 6565 705f 7061 7265 6e74     , keep_parent
+000006f0: 5f66 6965 6c64 7329 0d0a 2020 2020 0d0a  _fields)..    ..
+00000700: 2020 2020 6466 5f66 696e 616c 203d 2063      df_final = c
+00000710: 6f6e 6361 745f 6472 6f70 5f70 6172 656e  oncat_drop_paren
+00000720: 7428 6466 2e6c 6f63 5b76 616c 6964 5f73  t(df.loc[valid_s
+00000730: 7572 7665 7964 6174 612e 696e 6465 785d  urveydata.index]
+00000740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000760: 2020 2020 2c20 6466 5f73 7572 7665 7964      , df_surveyd
+00000770: 6174 615f 6578 7061 6e64 6564 0d0a 2020  ata_expanded..  
+00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007a0: 2c20 6472 6f70 5f70 6172 656e 745f 6e61  , drop_parent_na
+000007b0: 6d65 3d27 5375 7276 6579 4461 7461 2729  me='SurveyData')
+000007c0: 0d0a 2020 2020 0d0a 2020 2020 7265 7475  ..    ..    retu
+000007d0: 726e 2064 665f 6669 6e61 6c0d 0a0d 0a0d  rn df_final.....
+000007e0: 0a64 6566 206e 6164 6166 6965 6c64 5f66  .def nadafield_f
+000007f0: 726f 6d5f 6d75 6c74 6973 656c 6563 7428  rom_multiselect(
+00000800: 6466 313a 7064 2e44 6174 6146 7261 6d65  df1:pd.DataFrame
+00000810: 2920 2d3e 2070 642e 4461 7461 4672 616d  ) -> pd.DataFram
+00000820: 653a 0d0a 2020 6466 3d20 6466 312e 636f  e:..  df= df1.co
+00000830: 7079 2829 0d0a 2020 2320 6e6f 5f61 6e73  py()..  # no_ans
+00000840: 7765 725f 7661 6c75 6520 3d20 2d31 2020  wer_value = -1  
+00000850: 2320 646f 2074 6869 7320 746f 6765 7468  # do this togeth
+00000860: 6572 206c 6174 6572 2066 6f72 2061 6c6c  er later for all
+00000870: 2066 6965 6c64 732e 0d0a 2020 666f 7220   fields...  for 
+00000880: 4154 4f4d 4d75 6c74 6953 656c 6563 7451  ATOMMultiSelectQ
+00000890: 7565 7374 696f 6e2c 206e 6164 6166 6965  uestion, nadafie
+000008a0: 6c64 5f73 6561 7263 6873 7472 2069 6e20  ld_searchstr in 
+000008b0: 5c0d 0a20 2020 2020 206d 756c 7365 6c65  \..      mulsele
+000008c0: 6374 5f6f 7074 696f 6e5f 746f 5f6e 6164  ct_option_to_nad
+000008d0: 6166 6965 6c64 2e69 7465 6d73 2829 3a0d  afield.items():.
+000008e0: 0a20 2020 2066 6f72 206e 6164 6166 6965  .    for nadafie
+000008f0: 6c64 2c20 7365 6172 6368 5f73 7472 2069  ld, search_str i
+00000900: 6e20 6e61 6461 6669 656c 645f 7365 6172  n nadafield_sear
+00000910: 6368 7374 722e 6974 656d 7328 293a 0d0a  chstr.items():..
+00000920: 2020 2020 2020 6966 2041 544f 4d4d 756c        if ATOMMul
+00000930: 7469 5365 6c65 6374 5175 6573 7469 6f6e  tiSelectQuestion
+00000940: 206e 6f74 2069 6e20 6466 2e63 6f6c 756d   not in df.colum
+00000950: 6e73 3a0d 0a20 2020 2020 2020 206c 6f67  ns:..        log
+00000960: 6769 6e67 2e77 6172 6e28 6622 4e6f 2063  ging.warn(f"No c
+00000970: 6f6c 756d 6e20 7b41 544f 4d4d 756c 7469  olumn {ATOMMulti
+00000980: 5365 6c65 6374 5175 6573 7469 6f6e 7d20  SelectQuestion} 
+00000990: 6e61 6461 6669 656c 645f 6672 6f6d 5f6d  nadafield_from_m
+000009a0: 756c 7469 7365 6c65 6374 2229 0d0a 2020  ultiselect")..  
+000009b0: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
+000009c0: 2020 2020 2020 6466 5b6e 6164 6166 6965        df[nadafie
+000009d0: 6c64 5d20 3d20 6466 5b41 544f 4d4d 756c  ld] = df[ATOMMul
+000009e0: 7469 5365 6c65 6374 5175 6573 7469 6f6e  tiSelectQuestion
+000009f0: 5d2e 6170 706c 7928 0d0a 2020 2020 2020  ].apply(..      
+00000a00: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+00000a10: 6d62 6461 2078 3a20 6368 6563 6b5f 666f  mbda x: check_fo
+00000a20: 725f 7374 7269 6e67 2878 2c20 7365 6172  r_string(x, sear
+00000a30: 6368 5f73 7472 2929 0d0a 0d0a 2020 7265  ch_str))....  re
+00000a40: 7475 726e 2064 660d 0a0d 0a0d 0a64 6566  turn df......def
+00000a50: 2063 6f6e 7665 7274 5f79 6573 5f6e 6f66   convert_yes_nof
+00000a60: 6965 6c64 7328 6466 312c 2066 6965 6c64  ields(df1, field
+00000a70: 5f6e 616d 6573 293a 0d0a 2020 7265 7475  _names):..  retu
+00000a80: 726e 2074 7261 6e73 666f 726d 5f6d 756c  rn transform_mul
+00000a90: 7469 706c 6528 6466 312c 2066 6965 6c64  tiple(df1, field
+00000aa0: 5f6e 616d 6573 2c74 6f5f 6e75 6d5f 796e  _names,to_num_yn
+00000ab0: 5f6e 6f6e 6529 0d0a 0d0a 6465 6620 636f  _none)....def co
+00000ac0: 6e76 6572 745f 7472 7565 5f66 616c 7365  nvert_true_false
+00000ad0: 6669 656c 6473 2864 6631 2c20 6669 656c  fields(df1, fiel
+00000ae0: 645f 6e61 6d65 7329 3a0d 0a20 2072 6574  d_names):..  ret
+00000af0: 7572 6e20 7472 616e 7366 6f72 6d5f 6d75  urn transform_mu
+00000b00: 6c74 6970 6c65 2864 6631 2c20 6669 656c  ltiple(df1, fiel
+00000b10: 645f 6e61 6d65 732c 746f 5f6e 756d 5f62  d_names,to_num_b
+00000b20: 6f6f 6c5f 6e6f 6e65 290d 0a0d 0a0d 0a23  ool_none)......#
+00000b30: 2064 6566 2070 7265 705f 6461 7461 6672   def prep_datafr
+00000b40: 616d 655f 6d61 7463 6869 6e67 2864 663a  ame_matching(df:
+00000b50: 7064 2e44 6174 6146 7261 6d65 293a 0d0a  pd.DataFrame):..
+00000b60: 0d0a 2320 2020 6c6f 6767 696e 672e 6465  ..#   logging.de
+00000b70: 6275 6728 6622 7072 6570 5f64 6174 6166  bug(f"prep_dataf
+00000b80: 7261 6d65 206f 6620 6c65 6e67 7468 207b  rame of length {
+00000b90: 6c65 6e28 6466 297d 203a 2022 290d 0a23  len(df)} : ")..#
+00000ba0: 2020 2064 6632 203d 2067 6574 5f73 7572     df2 = get_sur
+00000bb0: 7665 7964 6174 615f 6578 7061 6e64 6564  veydata_expanded
+00000bc0: 2864 662e 636f 7079 2829 2c20 2050 7572  (df.copy(),  Pur
+00000bd0: 706f 7365 2e4d 4154 4348 494e 4729 0d0a  pose.MATCHING)..
+00000be0: 0d0a 2320 2020 6466 352c 2077 6172 6e69  ..#   df5, warni
+00000bf0: 6e67 735f 616f 6420 3d20 6578 7061 6e64  ngs_aod = expand
+00000c00: 5f64 7275 675f 696e 666f 2864 6632 290d  _drug_info(df2).
+00000c10: 0a23 2020 2072 6574 7572 6e20 6466 352c  .#   return df5,
+00000c20: 2077 6172 6e69 6e67 735f 616f 640d 0a0d   warnings_aod...
+00000c30: 0a0d 0a64 6566 2070 7265 705f 6461 7461  ...def prep_data
+00000c40: 6672 616d 655f 6e61 6461 2864 663a 7064  frame_nada(df:pd
+00000c50: 2e44 6174 6146 7261 6d65 2c20 636f 6e66  .DataFrame, conf
+00000c60: 6967 3a64 6963 7429 3a0d 0a0d 0a20 206c  ig:dict):....  l
+00000c70: 6f67 6769 6e67 2e64 6562 7567 2866 2270  ogging.debug(f"p
+00000c80: 7265 705f 6461 7461 6672 616d 6520 6f66  rep_dataframe of
+00000c90: 206c 656e 6774 6820 7b6c 656e 2864 6629   length {len(df)
+00000ca0: 7d20 3a20 2229 0d0a 2020 6466 3220 3d20  } : ")..  df2 = 
+00000cb0: 6765 745f 7375 7276 6579 6461 7461 5f65  get_surveydata_e
+00000cc0: 7870 616e 6465 6428 6466 2e63 6f70 7928  xpanded(df.copy(
+00000cd0: 292c 2050 7572 706f 7365 2e4e 4144 4129  ), Purpose.NADA)
+00000ce0: 0d0a 200d 0a20 2064 6634 203d 2064 726f  .. ..  df4 = dro
+00000cf0: 705f 6669 656c 6473 5f62 795f 7265 6765  p_fields_by_rege
+00000d00: 7828 6466 322c 7265 6765 783d 2743 6f6d  x(df2,regex='Com
+00000d10: 6d65 6e74 7c4e 6f74 657c 4954 5350 2729  ment|Note|ITSP')
+00000d20: 2023 2072 656d 6f76 6520 2a47 6f61 6c73   # remove *Goals
+00000d30: 206e 6f74 6573 2c20 736f 2064 6f20 6265   notes, so do be
+00000d40: 666f 7265 2050 4443 2073 7465 7020 2850  fore PDC step (P
+00000d50: 4443 476f 616c 7320 6472 6f70 646f 776e  DCGoals dropdown
+00000d60: 290d 0a0d 0a20 2064 6635 2c20 7761 726e  )....  df5, warn
+00000d70: 696e 6773 5f61 6f64 203d 2065 7870 616e  ings_aod = expan
+00000d80: 645f 6472 7567 5f69 6e66 6f28 6466 342c  d_drug_info(df4,
+00000d90: 2063 6f6e 6669 6729 0d0a 0d0a 2020 2320   config)....  # 
+00000da0: 6466 3531 203d 2065 7870 616e 645f 6163  df51 = expand_ac
+00000db0: 7469 7669 7469 6573 5f69 6e66 6f28 6466  tivities_info(df
+00000dc0: 3529 0d0a 2020 6466 3531 203d 206e 6164  5)..  df51 = nad
+00000dd0: 6166 6965 6c64 5f66 726f 6d5f 6d75 6c74  afield_from_mult
+00000de0: 6973 656c 6563 7428 6466 3529 0d0a 2020  iselect(df5)..  
+00000df0: 2320 6466 3620 3d20 6466 355b 6466 352e  # df6 = df5[df5.
+00000e00: 5044 4353 7562 7374 616e 6365 4f72 4761  PDCSubstanceOrGa
+00000e10: 6d62 6c69 6e67 2e6e 6f74 6e61 2829 5d23  mbling.notna()]#
+00000e20: 2072 656d 6f76 6573 2072 6f77 7320 7769   removes rows wi
+00000e30: 7468 6f75 7420 5044 430d 0a20 200d 0a20  thout PDC..  .. 
+00000e40: 2079 6573 5f6e 6f66 6965 6c64 7320 3d20   yes_nofields = 
+00000e50: 5b27 5061 7374 3457 6b42 6565 6e41 7272  ['Past4WkBeenArr
+00000e60: 6573 7465 6427 2c20 2750 6173 7434 576b  ested', 'Past4Wk
+00000e70: 4861 7665 596f 7556 696f 6c65 6e63 6541  HaveYouViolenceA
+00000e80: 6275 7369 7665 275d 0d0a 0d0a 2020 6466  busive']....  df
+00000e90: 3532 203d 2063 6f6e 7665 7274 5f79 6573  52 = convert_yes
+00000ea0: 5f6e 6f66 6965 6c64 7328 6466 3531 2c20  _nofields(df51, 
+00000eb0: 7965 735f 6e6f 6669 656c 6473 290d 0a20  yes_nofields).. 
+00000ec0: 2062 6f6f 6c5f 6669 656c 6473 203d 205b   bool_fields = [
+00000ed0: 2741 544f 5048 6f6d 656c 6573 7327 2c09  'ATOPHomeless',.
+00000ee0: 2741 544f 5052 6973 6b45 7669 6374 696f  'ATOPRiskEvictio
+00000ef0: 6e27 2c09 2750 7269 6d61 7279 4361 7265  n',.'PrimaryCare
+00000f00: 6769 7665 725f 302d 3527 2c0d 0a20 2020  giver_0-5',..   
+00000f10: 2020 2020 2020 2020 2020 2020 2020 0927                .'
+00000f20: 5072 696d 6172 7943 6172 6567 6976 6572  PrimaryCaregiver
+00000f30: 5f35 2d31 3527 2c09 2750 6173 7434 576b  _5-15',.'Past4Wk
+00000f40: 5f56 696f 6c65 6e74 546f 596f 7527 2c5d  _ViolentToYou',]
+00000f50: 0d0a 2020 6466 3620 3d20 636f 6e76 6572  ..  df6 = conver
+00000f60: 745f 7472 7565 5f66 616c 7365 6669 656c  t_true_falsefiel
+00000f70: 6473 2864 6635 322c 2062 6f6f 6c5f 6669  ds(df52, bool_fi
+00000f80: 656c 6473 290d 0a20 2020 0d0a 2020 6466  elds)..   ..  df
+00000f90: 3720 3d20 6669 785f 6e75 6d65 7269 6373  7 = fix_numerics
+00000fa0: 2864 6636 2920 200d 0a20 2064 6637 2e72  (df6)  ..  df7.r
+00000fb0: 656e 616d 6528 636f 6c75 6d6e 733d 7b27  ename(columns={'
+00000fc0: 4553 5441 424c 4953 484d 454e 5420 4944  ESTABLISHMENT ID
+00000fd0: 454e 5449 4649 4552 273a 2027 4167 656e  ENTIFIER': 'Agen
+00000fe0: 6379 436f 6465 277d 2c20 696e 706c 6163  cyCode'}, inplac
+00000ff0: 653d 5472 7565 290d 0a20 200d 0a20 2064  e=True)..  ..  d
+00001000: 6639 203d 2064 6637 2e73 6f72 745f 7661  f9 = df7.sort_va
+00001010: 6c75 6573 2862 793d 5b22 534c 4b22 2c20  lues(by=["SLK", 
+00001020: 2241 7373 6573 736d 656e 7444 6174 6522  "AssessmentDate"
+00001030: 5d29 0d0a 2020 0d0a 2020 6c6f 6767 696e  ])..  ..  loggin
+00001040: 672e 6465 6275 6728 6622 446f 6e65 2050  g.debug(f"Done P
+00001050: 7265 7070 696e 6720 666f 7220 4e41 4441  repping for NADA
+00001060: 2e20 5c6e 5c74 2220 2b0d 0a20 2020 2020  . \n\t" +..     
+00001070: 2020 2020 2020 2020 2020 2022 2020 4461             "  Da
+00001080: 7461 7365 7420 7368 6170 653a 7b64 6639  taset shape:{df9
+00001090: 2e73 6861 7065 7d29 2e20 5761 726e 696e  .shape}). Warnin
+000010a0: 6773 2073 6861 7065 207b 7761 726e 696e  gs shape {warnin
+000010b0: 6773 5f61 6f64 7d22 290d 0a20 2072 6574  gs_aod}")..  ret
+000010c0: 7572 6e20 6466 3920 2c20 7761 726e 696e  urn df9 , warnin
+000010d0: 6773 5f61 6f64 0d0a 0d0a 0d0a 2320 6465  gs_aod......# de
+000010e0: 6620 7072 6570 5f64 6174 6166 7261 6d65  f prep_dataframe
+000010f0: 2864 663a 7064 2e44 6174 6146 7261 6d65  (df:pd.DataFrame
+00001100: 2c20 7072 6570 5f74 7970 653a 204c 6974  , prep_type: Lit
+00001110: 6572 616c 5b27 4154 4f4d 272c 2027 4e41  eral['ATOM', 'NA
+00001120: 4441 272c 2027 4d61 7463 6869 6e67 275d  DA', 'Matching']
+00001130: 203d 2027 4154 4f4d 2729 3a0d 0a23 2020   = 'ATOM'):..#  
+00001140: 2020 2320 6265 6361 7573 6520 5072 6f67    # because Prog
+00001150: 7261 6d20 6973 2069 6e20 5375 7276 6579  ram is in Survey
+00001160: 4461 7461 0d0a 2020 0d0a 2320 2020 6966  Data..  ..#   if
+00001170: 2070 7265 705f 7479 7065 203d 3d20 274d   prep_type == 'M
+00001180: 6174 6368 696e 6727 3a0d 0a23 2020 2020  atching':..#    
+00001190: 2072 6574 7572 6e20 7072 6570 5f64 6174   return prep_dat
+000011a0: 6166 7261 6d65 5f6d 6174 6368 696e 6728  aframe_matching(
+000011b0: 6466 290d 0a0d 0a23 2020 206c 6f67 6765  df)....#   logge
+000011c0: 722e 6465 6275 6728 6622 7072 6570 5f64  r.debug(f"prep_d
+000011d0: 6174 6166 7261 6d65 206f 6620 6c65 6e67  ataframe of leng
+000011e0: 7468 207b 6c65 6e28 6466 297d 203a 2022  th {len(df)} : "
+000011f0: 290d 0a23 2020 2064 6632 203d 2067 6574  )..#   df2 = get
+00001200: 5f73 7572 7665 7964 6174 615f 6578 7061  _surveydata_expa
+00001210: 6e64 6564 2864 662e 636f 7079 2829 290d  nded(df.copy()).
+00001220: 0a0d 0a23 2020 2064 6633 203d 2064 726f  ...#   df3 = dro
+00001230: 705f 6669 656c 6473 2864 6632 2c5b 274f  p_fields(df2,['O
+00001240: 4443 275d 290d 0a23 2020 2064 6634 203d  DC'])..#   df4 =
+00001250: 2064 726f 705f 636f 6c73 5f63 6f6e 7461   drop_cols_conta
+00001260: 696e 735f 7265 6765 7828 6466 332c 2041  ins_regex(df3, A
+00001270: 544f 4d5f 4452 4f50 5f43 4f4c 434f 4e54  TOM_DROP_COLCONT
+00001280: 4149 4e53 5f52 4547 4558 2920 2320 7265  AINS_REGEX) # re
+00001290: 6d6f 7665 202a 476f 616c 7320 6e6f 7465  move *Goals note
+000012a0: 732c 2073 6f20 646f 2062 6566 6f72 6520  s, so do before 
+000012b0: 5044 4320 7374 6570 2028 5044 4347 6f61  PDC step (PDCGoa
+000012c0: 6c73 2064 726f 7064 6f77 6e29 0d0a 2320  ls dropdown)..# 
+000012d0: 2020 6466 3520 3d20 6e6f 726d 616c 697a    df5 = normaliz
+000012e0: 655f 6669 7273 745f 656c 656d 656e 7428  e_first_element(
+000012f0: 6466 342c 2750 4443 2729 2023 544f 444f  df4,'PDC') #TODO
+00001300: 3a20 2864 662c 274f 4443 2729 2023 206f  : (df,'ODC') # o
+00001310: 6e6c 7920 7461 6b65 7320 7468 6520 6669  nly takes the fi
+00001320: 7273 7420 4f44 4320 2020 0d0a 0d0a 200d  rst ODC   .... .
+00001330: 0a23 2020 2064 6636 203d 2064 6635 5b64  .#   df6 = df5[d
+00001340: 6635 2e50 4443 5375 6273 7461 6e63 654f  f5.PDCSubstanceO
+00001350: 7247 616d 626c 696e 672e 6e6f 746e 6128  rGambling.notna(
+00001360: 295d 2320 7265 6d6f 7665 7320 726f 7773  )]# removes rows
+00001370: 2077 6974 686f 7574 2050 4443 0d0a 0d0a   without PDC....
+00001380: 2320 2020 2320 6466 362e 6c6f 635b 3a2c  #   # df6.loc[:,
+00001390: 2750 726f 6772 616d 275d 203d 2064 6636  'Program'] = df6
+000013a0: 5b27 526f 774b 6579 275d 2e73 7472 2e73  ['RowKey'].str.s
+000013b0: 706c 6974 2827 5f27 292e 7374 725b 305d  plit('_').str[0]
+000013c0: 2023 2068 6173 2074 6f20 6265 206d 6164   # has to be mad
+000013d0: 6520 696e 746f 2063 6174 6567 6f72 790d  e into category.
+000013e0: 0a23 2020 2064 6637 203d 2063 6f6e 7665  .#   df7 = conve
+000013f0: 7274 5f64 7479 7065 7328 6466 3629 0d0a  rt_dtypes(df6)..
+00001400: 0d0a 2320 2020 2320 6466 2e50 4443 4167  ..#   # df.PDCAg
+00001410: 6546 6972 7374 5573 6564 5b28 6466 2e50  eFirstUsed[(df.P
+00001420: 4443 4167 6546 6972 7374 5573 6564 2e6e  DCAgeFirstUsed.n
+00001430: 6f74 6e61 2829 2920 2620 2864 662e 5044  otna()) & (df.PD
+00001440: 4341 6765 4669 7273 7455 7365 6420 213d  CAgeFirstUsed !=
+00001450: 2027 2729 5d2e 6173 7479 7065 2869 6e74   '')].astype(int
+00001460: 290d 0a23 2020 2320 2245 7870 6563 7465  )..#  # "Expecte
+00001470: 6420 6279 7465 732c 2067 6f74 2061 2027  d bytes, got a '
+00001480: 696e 7427 206f 626a 6563 7422 2c20 2743  int' object", 'C
+00001490: 6f6e 7665 7273 696f 6e20 6661 696c 6564  onversion failed
+000014a0: 2066 6f72 2063 6f6c 756d 6e20 5044 4341   for column PDCA
+000014b0: 6765 4669 7273 7455 7365 6420 7769 7468  geFirstUsed with
+000014c0: 2074 7970 6520 6f62 6a65 6374 270d 0a23   type object'..#
+000014d0: 2020 2064 6638 203d 2064 726f 705f 6669     df8 = drop_fi
+000014e0: 656c 6473 2864 6637 2c20 5b27 5044 4341  elds(df7, ['PDCA
+000014f0: 6765 4669 7273 7455 7365 6427 2c5c 0d0a  geFirstUsed',\..
+00001500: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+00001510: 2020 2020 2020 2020 2020 2020 2027 5072               'Pr
+00001520: 696d 6172 7943 6172 6567 6976 6572 272c  imaryCaregiver',
+00001530: 2750 6173 7434 576b 416f 6452 6973 6b73  'Past4WkAodRisks
+00001540: 275d 2920 0d0a 2320 2020 2320 2763 616e  ']) ..#   # 'can
+00001550: 6e6f 7420 6d69 7820 6c69 7374 2061 6e64  not mix list and
+00001560: 206e 6f6e 2d6c 6973 742c 206e 6f6e 2d6e   non-list, non-n
+00001570: 756c 6c20 7661 6c75 6573 272c 200d 0a23  ull values', ..#
+00001580: 2020 2023 2027 436f 6e76 6572 7369 6f6e     # 'Conversion
+00001590: 2066 6169 6c65 6420 666f 7220 636f 6c75   failed for colu
+000015a0: 6d6e 2050 7269 6d61 7279 4361 7265 6769  mn PrimaryCaregi
+000015b0: 7665 722c 2050 6173 7434 576b 416f 6452  ver, Past4WkAodR
+000015c0: 6973 6b73 2077 6974 6820 7479 7065 206f  isks with type o
+000015d0: 626a 6563 7427 290d 0a0d 0a23 2020 2069  bject')....#   i
+000015e0: 6620 2753 4c4b 2720 696e 2064 6638 2e63  f 'SLK' in df8.c
+000015f0: 6f6c 756d 6e73 3a0d 0a23 2020 2020 2064  olumns:..#     d
+00001600: 6638 2e64 726f 7028 636f 6c75 6d6e 733d  f8.drop(columns=
+00001610: 5b27 534c 4b27 5d2c 2069 6e70 6c61 6365  ['SLK'], inplace
+00001620: 3d54 7275 6529 200d 0a20 200d 0a23 2020  =True) ..  ..#  
+00001630: 2064 6638 2e72 656e 616d 6528 636f 6c75   df8.rename(colu
+00001640: 6d6e 733d 7b27 5061 7274 6974 696f 6e4b  mns={'PartitionK
+00001650: 6579 273a 2027 534c 4b27 7d2c 2069 6e70  ey': 'SLK'}, inp
+00001660: 6c61 6365 3d54 7275 6529 0d0a 2020 0d0a  lace=True)..  ..
+00001670: 2320 2020 6466 3920 3d20 6466 382e 736f  #   df9 = df8.so
+00001680: 7274 5f76 616c 7565 7328 6279 3d22 4173  rt_values(by="As
+00001690: 7365 7373 6d65 6e74 4461 7465 2229 0d0a  sessmentDate")..
+000016a0: 200d 0a23 2020 2064 6639 5b27 5044 4327   ..#   df9['PDC'
+000016b0: 5d20 3d20 6466 395b 2750 4443 5375 6273  ] = df9['PDCSubs
+000016c0: 7461 6e63 654f 7247 616d 626c 696e 6727  tanceOrGambling'
+000016d0: 5d0d 0a20 0d0a 2320 2020 6c6f 6767 6572  ].. ..#   logger
+000016e0: 2e64 6562 7567 2866 2244 6f6e 6520 5072  .debug(f"Done Pr
+000016f0: 6570 7069 6e67 2064 6622 290d 0a23 2020  epping df")..#  
+00001700: 2072 6574 7572 6e20 6466 39               return df9
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/exporters/NADAbase.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/exporters/NADAbase.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import pandas as pd
-from utils.dtypes import date_to_str
-from utils.df_ops_base import safe_convert_to_int_strs, prescribe_fields
-from .config.NADAbase import nada_final_fields, notanswered_defaults
+from assessment_episode_matcher.utils.dtypes import date_to_str
+from assessment_episode_matcher.utils.df_ops_base import safe_convert_to_int_strs, prescribe_fields
+from assessment_episode_matcher.exporters.config.NADAbase import nada_final_fields, notanswered_defaults
 
 
 def get_stage_per_episode(df:pd.DataFrame)-> pd.Series:  
   df = df.sort_values(by=["PMSEpisodeID", "AssessmentDate"])
   # Rank the assessments within each client
   return  df.groupby('PMSEpisodeID').cumcount()
 
 
 def set_not_answered(df1:pd.DataFrame, notanswered_cols:list) -> pd.DataFrame:
   df = df1.copy()
   for col in notanswered_cols:
-    df[col].replace('', -1, inplace=True)
-
+    df[col] = df[col].replace('', -1).infer_objects(copy=False)
+    # infer: instruct pandas to infer the data type of the resulting
+    # column and perform any necessary downcasting.
   return df
 
 
 def cols_prep(source_df, dest_columns, fill_new_cols) -> pd.DataFrame:
   
   df_final = source_df.reindex(columns=dest_columns, fill_value=fill_new_cols)
   # 'StandardDrinksPerDay' (_PerOccassionUse) -> Range/average calculation resutls in float
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/exporters/main.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/exporters/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,110 @@
 
 from abc import ABC, abstractmethod
 from typing import Optional
 # from pathlib import Path
 import pandas as pd
 from assessment_episode_matcher.azutil.az_blob_query import AzureBlobQuery
+from assessment_episode_matcher.mytypes import CSVTypeObject
 
 class DataExporter(ABC):
 
   def __init__(self, config) -> None:
     self.config = config
 
   @abstractmethod
-  def export_data(self, data_name:str, data:pd.DataFrame):
+  def export_dataframe(self, data_name:str, data:pd.DataFrame):
     pass
 
 
-# class CSVExporter(DataExporter):
+class CSVExporter(DataExporter):
 
-#   def export_data(self, data_name:str, data:pd.DataFrame):
-#     path = self.config.get("location")
-#     if not path:
-#       raise FileNotFoundError("CSVExporter:No file-path was passed in")
+  def export_dataframe(self, data_name:str, data:pd.DataFrame):
+    path = self.config.get("location")
+    if not path:
+      raise FileNotFoundError("CSVExporter:No file-path was passed in")
     
-#     data.to_csv(f"{path}{data_name}.csv", index=False)
+    data.to_csv(f"{path}{data_name}.csv", index=False)
 
 
-# class ParquetExporter(DataExporter):
+class ParquetExporter(DataExporter):
 
-#   def export_data(self, data_name:str, data:pd.DataFrame):
-#     path = self.config.get("location")
-#     if not path:
-#       raise FileNotFoundError("ParquetExporter:No file-path was passed in")
+  def export_dataframe(self, data_name:str, data:pd.DataFrame):
+    path = self.config.get("location")
+    if not path:
+      raise FileNotFoundError("ParquetExporter:No file-path was passed in")
     
-#     data.to_parquet(f"{path}{data_name}.parquet", index=False)
+    data.to_parquet(f"{path}{data_name}.parquet", index=False)
+
+
+class LocalFileExporter(DataExporter):
+
+  def __init__(self, config) -> None:
+    self.config = config
+
+  """
+  similar to azutil.az_blob_query.write_data()
+  """
+  def export_dataframe(self, data_name:str, data:pd.DataFrame):
+    if data_name[-3:] =='csv':
+      p = CSVExporter(self.config)    
+    else:
+      p = ParquetExporter(self.config)
+    
+    p.export_dataframe(data_name, data)
     
 
+# class ConstructorRequirementError(Exception):
+#   msg:str
+#   source:str
+
+#   def __init__(self, msg: str, source:str="") -> None:
+#     self.msg = msg
+#     self.source = source
+
+    # super().__init__(*args)
+  
+
 class AzureBlobExporter(DataExporter):
   blobClient:AzureBlobQuery
 
   def __init__(self, container_name:str, config:Optional[dict]=None) -> None:
     if config:
       super().__init__(config)
+      # if not hasattr(self.config, 'container_name'):
+      #   raise ConstructorRequirementError(
+      #       msg="Must pass container_name to create a Blob Exporter"
+      #     , source="AzureBlobExporter")
+      # self.container_name = self.config['container_name']
     self.container_name = container_name
     self.blobClient = AzureBlobQuery()
 
-  def export_data(self, data_name:str, data:pd.DataFrame):
+  def export_dataframe(self, data_name:str, data:pd.DataFrame):   
     full_path = data_name
     if hasattr(self, "config"):
       folder_path = self.config.get("location")
       if folder_path:
         full_path = f"{folder_path}/{data_name}"
   
-    result = self.blobClient.write_data(container_name=self.container_name
+    result = self.blobClient.write_dataframe(container_name=self.container_name
                                         , blob_url=full_path
                                         ,data=data)    
     return result
     
-
+  def export_csv(self, data_name:str, data:CSVTypeObject):   
+    full_path = data_name
+    if hasattr(self, "config"):
+      folder_path = self.config.get("location")
+      if folder_path:
+        full_path = f"{folder_path}/{data_name}"
+  
+    result = self.blobClient.write_csv(container_name=self.container_name
+                                        , blob_url=full_path
+                                        ,data=data)    
+    return result
 
 # class AuditExporter(DataExporter):
 #   container_prefix = "audit-matching"
 
 #   def __init__(self, config) -> None:
 #     self.sink_config = config
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/aod.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/aod.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-import logging
+# import logging
 import pandas as pd
-from data_config import PDC_ODC_ATOMfield_names as PDC_ODC_fields
-from importers.config import ATOM
-from utils.fromstr import range_average
-from utils.df_ops_base import drop_fields
+from assessment_episode_matcher.data_config import PDC_ODC_ATOMfield_names as PDC_ODC_fields
+from assessment_episode_matcher.utils.fromstr import range_average
+from assessment_episode_matcher.utils.df_ops_base import drop_fields
+from assessment_episode_matcher.mytypes import AODWarning
 # import mylogging
 # logging = mylogging.get(__name__)
 
 
+
+
 # TODO: use NADA fields
 # DU Heroin use number of days
 # DU Other opioid use number of days
 # DU Cannabis use number of days
 # DU Cocaine use number of days
 # DU Amphetamine use number of days
 # DU Tranquilliser use number of days
@@ -61,74 +63,94 @@
 #          return '', None
 #       typical_qty = range_average(typical_qty)
 #       qty_str = f"{typical_qty}"
 #       if typical_unit:
 #         qty_str = f"{qty_str}; {typical_unit} units."
 #   return qty_str, typical_qty
 
+  # def __init__(self, item:dict, drug_name, field_name, assessment):
 
 
-def get_warning(item, drugname, field_name:str, assessment):  
-  warning = ( assessment.SLK, assessment.RowKey,         
-          { drugname: item.get(drugname),
-           'InvalidValue': item.get(field_name), 'InvalidFieldName': field_name}
-  )
-  return warning
+# def get_warning(item:dict, drugname, field_name:str, assessment):  
+#   warning = ( assessment.SLK, assessment.RowKey,         
+#           { drugname: item.get(drugname),
+#            'InvalidValue': item.get(field_name), 'InvalidFieldName': field_name}
+#   )
+#   return warning
 
-def get_typical_qty(item, field_names:dict[str, str], assessment)->  tuple[float, str, str, tuple|None]: #tuple[float|None, str|None, str]:
+def get_typical_qty(item, field_names:dict[str, str], assessment)->  tuple[float, str, str, AODWarning|None]: #tuple[float|None, str|None, str]:
   field_perocc = field_names['per_occassion']
   field_units = field_names['units']
 
   typical_qty = item.get(field_perocc, 0.0)
   typical_unit = item.get(field_units,'')
  
   if not typical_qty:
-     warning = get_warning(item, field_names['drug_name'], field_perocc, assessment)
+     warning = AODWarning(assessment['SLK'],assessment['RowKey']
+                          ,drug_name=field_names['drug_name']
+                          , field_name=field_perocc)
+    #  warning = get_warning(item, field_names['drug_name'], field_perocc, assessment)
      return typical_qty, "", "", warning
   if not pd.isna(typical_qty):
       if typical_qty == '0': # Don't bother with unit if qty = 0
          return 0.0, "", "0", None
       if typical_qty == 'Other':
         #  logging.warn(f"'Other' used for HowMuchPerOcassion. Un-reportable value { assessment.get('RowKey')}")
-         warning = get_warning(item, field_names['drug_name'], field_perocc, assessment)
+        #  warning = get_warning(item, field_names['drug_name'], field_perocc, assessment)
+         warning = AODWarning(assessment['SLK'],assessment['RowKey']
+                               , drug_name=field_names['drug_name']
+                          , field_name=field_perocc
+                          , field_value=typical_qty)
          return 0.0, "", "", warning
       typical_qty = range_average(typical_qty)
   if not typical_unit:
-     warning = get_warning(item, field_names['drug_name'], field_units, assessment)
+    #  warning = get_warning(item, field_names['drug_name'], field_units, assessment)
+     warning = AODWarning(assessment['SLK'],assessment['RowKey']
+                          ,drug_name=field_names['drug_name']
+                          , field_name=field_units
+                          , field_value=typical_unit)
      return typical_qty, "", f"{typical_qty}", warning
 
   return typical_qty, typical_unit, f"{typical_qty}; {typical_unit}", None
 
 
-def process_drug_list_for_assessment(pdc_odc_colname:str, assessment):
+def process_drug_list_for_assessment(pdc_odc_colname:str, assessment, config:dict):
   row_data = {}
   warnings = []
+  drug_categories= config["drug_categories"]
   for item in assessment[pdc_odc_colname]: #'ODC: []' in row
     # Extract data for each substance
     field_names  = PDC_ODC_fields[pdc_odc_colname]
     field_drug_name = field_names['drug_name']
     field_use_ndays = field_names['used_in_last_4wks']
 
     if not item: # {}
-      continue
+      continue 
 
     substance = item.get(field_drug_name, '')    
     if not substance:
       # logging.error(f"Data Quality error {field_drug_name} not in drug dict. SLK:{assessment['PartitionKey']}, RowKey:{assessment['RowKey']}.")
       continue
     # unique_subtances.append(substance) 
     mapped_drug, found_category = get_drug_category (substance
-                                                     , aod_groupings=ATOM.MAP_AOD_GROUPINGS)
+                                                     , aod_groupings=drug_categories)
     if not found_category:
-       if not row_data or not( 'Another Drug1' in row_data) or pd.isna(row_data['Another Drug1']):
-          row_data['Another Drug1'] = mapped_drug
-          mapped_drug ='Another Drug1'
-       else:
-          row_data['Another Drug2'] = mapped_drug
-          mapped_drug ='Another Drug2'
+      warning = AODWarning(assessment['SLK'],assessment['RowKey']
+                           ,drug_name=substance, field_name=field_drug_name)
+      # warning = get_warning(item
+      #                       , drugname=substance
+      #              ,field_name=field_drug_name
+      #              ,assessment=assessment)
+      warnings.append(warning)
+      if not row_data or not( 'Another Drug1' in row_data) or pd.isna(row_data['Another Drug1']):
+        row_data['Another Drug1'] = mapped_drug
+        mapped_drug ='Another Drug1'
+      else:
+        row_data['Another Drug2'] = mapped_drug
+        mapped_drug ='Another Drug2'
                  
     # if not field_use_ndays in item:
     #   logging.error(f"Data Quality error {field_use_ndays} not in drug({substance})dict. \
     #                SLK:{assessment['SLK']}, RowKey:{assessment['RowKey']}.")
     # if not field_perocc in item:
     #   logging.error(f"Data Quality error {field_perocc} not in drug({substance})dict. \
     #                SLK:{assessment['SLK']}, RowKey:{assessment['RowKey']}.")             
@@ -142,27 +164,27 @@
     row_data [ f"{mapped_drug}_TypicalQtyStr"] = typical_use_str
     if warning:
       warnings.append(warning)
 
   return row_data, warnings
 
 
-def normalize_pdc_odc(df):
+def normalize_pdc_odc(df:pd.DataFrame, config:dict):
   new_data = []
   warnings = []
   for index, row in df.iterrows():
     row_data = {}
     pdc_row_data ={}
     odc_row_data ={}
     if 'PDC' in row and isinstance(row['PDC'], list):
-      pdc_row_data, warnings1 = process_drug_list_for_assessment('PDC', row)
+      pdc_row_data, warnings1 = process_drug_list_for_assessment('PDC', row, config)
       if warnings1:
          warnings.extend(warnings1)
     if 'ODC' in row and isinstance(row['ODC'], list):
-      odc_row_data, warnings2 = process_drug_list_for_assessment('ODC', row)
+      odc_row_data, warnings2 = process_drug_list_for_assessment('ODC', row, config)
       if warnings2:
          warnings.extend(warnings2)
     
     # merge the dicts
     row_data = pdc_row_data | odc_row_data
     if row_data:
         new_data.append(row_data)
@@ -177,18 +199,18 @@
     # # result_df = pd.concat([df, expanded_data], axis=1)
     # # print(set(unique_subtances))
     # # return result_df
     # return expanded_data
 
 
 
-def expand_drug_info(df1:pd.DataFrame) ->  tuple[pd.DataFrame, list]:
+def expand_drug_info(df1:pd.DataFrame, config:dict) ->  tuple[pd.DataFrame, list[AODWarning]]:
 
   #  masked_rows=  df1[('ODC' in df1) and df1['ODC'].apply(lambda x: isinstance(x,list) and len(x) > 0 )]
-  normd_drugs_df, warnings = normalize_pdc_odc(df1)
+  normd_drugs_df, warnings = normalize_pdc_odc(df1, config)
     # debug: normd_drugs_df.loc[2][normd_drugs_df.loc[2].notna()]
   cloned_df = df1.join(normd_drugs_df)
   cloned_df = drop_fields(cloned_df,['PDC','ODC'])
     #debug : cloned_df.loc[2, [c for c in cloned_df.columns if 'Heroin_' in c]]
 
      
   return cloned_df, warnings
@@ -310,11 +332,11 @@
 
           # [{'OtherSubstancesConcernGambling': 'Cocaine', 'DaysInLast28': '5'}],      
           # [],
           # [{'OtherSubstancesConcernGambling': 'Benzodiazepines, n.f.d.', 'DaysInLast28': '15', 'HowMuchPerOccasion': '2'}],      
       ]
   })
 
-  out, warnings = expand_drug_info(df)
-  # TODO : delete PDC and ODC columns
-  print(out)
-  print(warnings)
+  # out, warnings = expand_drug_info(df)
+  # # TODO : delete PDC and ODC columns
+  # print(out)
+  # print(warnings)
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/assessments.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/assessments.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 import pandas as pd
 from assessment_episode_matcher.importers.main import FileSource
 from assessment_episode_matcher.utils import io
 from assessment_episode_matcher.mytypes import Purpose
 from assessment_episode_matcher import data_config
 from assessment_episode_matcher.utils.df_ops_base import has_data
-from assessment_episode_matcher.setup.bootstrap import Bootstrap
+# from assessment_episode_matcher.setup.bootstrap import Bootstrap
 
 
 def filter_by_purpose(df:pd.DataFrame, filters:dict|None) -> pd.DataFrame:
   if not filters:
      return df
   return df[df ['Program'].isin(filters['Program'])]
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/episodes.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/episodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import pandas as pd
 from assessment_episode_matcher.configs import episodes as EpCfg
 from assessment_episode_matcher.data_config import EstablishmentID_Program
 from assessment_episode_matcher.importers.main import FileSource
 from assessment_episode_matcher.utils.dtypes import blank_to_today_str, convert_to_datetime
 from assessment_episode_matcher.utils.df_ops_base import has_data
 from assessment_episode_matcher.utils import io
-from assessment_episode_matcher.setup.bootstrap import Bootstrap
+# from assessment_episode_matcher.setup.bootstrap import Bootstrap
 
 # from utils.io import read_parquet, write_parquet
 
-def prepare(ep_df1:pd.DataFrame, start_date:str, end_date:str) -> pd.DataFrame:
+def prepare(ep_df1:pd.DataFrame) -> pd.DataFrame:
   # processed_folder = Bootstrap.get_path("processed_dir")
 
   ep_df = ep_df1[EpCfg.columns_of_interest].copy()
   ep_df['Program'] = ep_df['ESTABLISHMENT IDENTIFIER'].map(EstablishmentID_Program)
   
 #  convert_to_datetime(atom_df['AssessmentDate'], format='%Y%m%d')
   ep_df[EpCfg.date_cols[0]] = convert_to_datetime(ep_df[EpCfg.date_cols[0]],  format='%d%m%Y'
@@ -97,15 +97,15 @@
     logging.info(f"No Raw episode Data. Returning empty. {file_path}")
     return raw_df, None
   
   raw_df.dropna(subset=['START DATE'], inplace=True)
   # TODO: log the dropped episodes
   raw_df['END DATE'] = raw_df['END DATE'].apply(lambda x: blank_to_today_str(x))
 
-  processed_df = prepare(raw_df, eps_st, eps_end)
+  processed_df = prepare(raw_df)
   return processed_df, file_path
 
 
 # def import_data(eps_st:str,  eps_end:str, file_source:FileSource, prefix:str, suffix:str) -> pd.DataFrame:
 #   """
 #     Load processed episodes dataframe from disk
 #     If not available, load raw, process and save, and then return processed_df
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/importers/main.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/importers/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from abc import ABC, abstractmethod
+import json
 import pandas as pd
 
 from assessment_episode_matcher.azutil.az_blob_query import AzureBlobQuery
 
 class FileSource(ABC):
     def __init__(self, path: str):
         self.path = path
@@ -42,14 +43,24 @@
 
     def load_parquet_file_to_df(self, filepath: str) -> pd.DataFrame:
         full_path = os.path.join(self.path, filepath)
         if os.path.isfile(full_path):
             return pd.read_parquet(full_path)
         else:
             raise FileNotFoundError(f"File not found: {full_path}")
+
+
+    def load_json_file(self, filepath: str) -> pd.DataFrame:
+        full_path = os.path.join(self.path, filepath)
+        if os.path.isfile(full_path):
+            with open(full_path, 'r') as file:
+              json_data = json.load(file)
+              return json_data
+        else:
+            raise FileNotFoundError(f"File not found: {full_path}")        
         
 
 class BlobFileSource(FileSource):
     
     blobClient:AzureBlobQuery
 
     def __init__(self, container_name: str, folder_path:str=""):
@@ -60,14 +71,23 @@
     def list_files(self, prefix: str, suffix: str) -> list[str]:
         files = self.blobClient.list_files(self.container_name,
                                            self.folder_path,
                                            prefix, suffix)
         
         return files
     
+    def load_json_file(self, filename: str, dtype)-> dict:
+        
+        blob_bytes = self.blobClient.load_data(self.container_name,blob_url=filename)
+        if blob_bytes:
+            return json.loads(blob_bytes.read().decode('utf-8'))
+        else:
+            filepath = f"{self.container_name}/{filename}"
+            raise ValueError(f"Failed to load blob data from URL: {filepath}")            
+    
     def load_csv_file_to_df(self, filename: str, dtype)-> pd.DataFrame:
         
         blob_bytes = self.blobClient.load_data(self.container_name,blob_url=filename)
         if blob_bytes:
             return pd.read_csv(blob_bytes, dtype=dtype)
         else:
             filepath = f"{self.container_name}/{filename}"
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/date_checks.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/date_checks.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/errors.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/errors.py`

 * *Files 23% similar despite different names*

```diff
@@ -91,40 +91,9 @@
 
 
 def write_validation_results(errors_warnings:dict[str, pd.DataFrame]
                              , audit_exporter: DataExporter):
     
     for ew_type_name, errs_warns in errors_warnings.items():
       if utdf.has_data(errs_warns):
-        audit_exporter.export_data(f"{ew_type_name}.csv", errs_warns)       
+        audit_exporter.export_dataframe(f"{ew_type_name}.csv", errs_warns)       
        
-    
-
-    # if utdf.has_data(dates_ewdf):
-    #   audit_exporter.export_data("dates_ew", dates_ewdf)
-    #   # dates_ewdf.to_csv(f'{output_folder}dates_ewdf.csv'
-    #   #                   , index=False)
-    
-    # if utdf.has_data(asmt_key_errors):
-    #    audit_exporter.export_data("asmt_key_errors", asmt_key_errors)
-    #   # asmt_key_errors.to_csv(f'{output_folder}asmt_key_errors.csv'
-    #   #                       , index=False)
-
-    # if utdf.has_data(ep_key_errors):
-    #    audit_exporter.export_data("ep_key_errors", ep_key_errors)
-    #   # ep_key_errors.to_csv(f'{output_folder}ep_key_errors.csv'
-    #   #                      , index=False)
-
-    # if utdf.has_data(asmt_key_warn):
-    #   audit_exporter.export_data("asmt_key_warn", asmt_key_warn)
-
-    # if utdf.has_data(ep_key_warn):
-    #   audit_exporter.export_data("ep_key_warn", ep_key_warn)
-
-
-    # if utdf.has_data(asmt_key_warn):
-    #   asmt_key_warn.to_csv(f'{output_folder}asmt_key_warn.csv'
-    #                        , index=False)
-
-    # if utdf.has_data(ep_key_warn):
-    #   ep_key_warn.to_csv(f'{output_folder}ep_key_warn.csv'
-    #                      , index=False)
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/increasing_slack.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/increasing_slack.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/main.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/main.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/matching/matching_stats.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/matching/matching_stats.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/mytypes.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/mytypes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,38 @@
 from enum import Enum, auto
-from dataclasses import dataclass
-from typing import Optional #, KW_ONLY
+from dataclasses import dataclass, fields
+from typing import Any, Optional #, KW_ONLY
 from collections import namedtuple
 
 
+
+@dataclass
+class CSVTypeObject:
+  header:list[str]
+  rows:list
+
+@dataclass
+class AODWarning:
+  SLK:str
+  RowKey:str
+  drug_name:str
+  field_name:str
+  field_value:Optional[str]=""
+   
+  #  def __str__(self):
+  #   return f"{self.SLK},{self.RowKey},{self.drug_name},{self.field_name}"
+  def to_list(self) -> list[str]:
+    f = [getattr(self, field.name) for field in fields(self)]
+    return f
+    # field_values = []
+    # for field in fields(self):
+    #     value = getattr(self, field.name)
+    #     field_values.append(value)
+    # return field_values
+  
 class DataType(Enum):
   ASSESSMENTS = auto()
   EPISODES = auto()
   PROCESSED_ASSESSMENTS = auto()
   PROCESSED_EPISODES = auto()
   # OTHER = auto()
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/setup/bootstrap.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/setup/bootstrap.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/setup/log_management.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/setup/log_management.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/test_surveytxt.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/test_surveytxt.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,30 +74,30 @@
       return json.dumps({"result":"no episode data"})
     #TODO:
     if ep_cache_to_path:
       if ep_cache_to_path[-3:] =='csv':
          ep_cache_to_path = f"{ep_cache_to_path[:-3]}parquet"
          
       exp = AzureBlobExporter(container_name=ep_file_source.container_name) #
-      exp.export_data(data_name=ep_cache_to_path, data=episode_df)   
+      exp.export_dataframe(data_name=ep_cache_to_path, data=episode_df)   
                         # func.HttpResponse(body=json.dumps({"result":"no episode data"}),
                         #         mimetype="application/json", status_code=200)
 
     
     atom_file_source:FileSource = BlobFileSource(container_name=container
                                             , folder_path=asmt_folder)
     atoms_df, atom_cache_to_path = ATOMsImporter.import_data(
                             reporting_start_str, reporting_end_str
                             , atom_file_source
                             , prefix=asmt_folder, suffix="AllPrograms"
                             , purpose=Purpose.NADA, refresh=True)
     
     if atom_cache_to_path:
       exp = AzureBlobExporter(container_name=atom_file_source.container_name) #
-      exp.export_data(data_name=atom_cache_to_path, data=atoms_df)    
+      exp.export_dataframe(data_name=atom_cache_to_path, data=atoms_df)    
                             # , prefix="MDS", suffix="AllPrograms")
     if not utdf.has_data(atoms_df):
       logging.error("No ATOMs")
       return json.dumps({"result":"no ATOM data"})
 
     a_df, e_df, inperiod_atomslk_notin_ep, inperiod_epslk_notin_atom = \
       match_helper.get_data_for_matching2(episode_df, atoms_df
@@ -120,26 +120,33 @@
                             , period_end=reporting_end
                             , audit_exporter=ae)
   
 
     df_reindexed = final_good.reset_index(drop=True)
 
     exp = AzureBlobExporter(container_name=atom_file_source.container_name) #
-    exp.export_data(data_name=f"NADA/{reporting_start_str}-{reporting_end_str}_reindexed.parquet", data=df_reindexed)      
+    p_str = f"{reporting_start_str}-{reporting_end_str}"
+    exp.export_dataframe(data_name=f"NADA/{p_str}/forstxt_{p_str}_reindexed.parquet", data=df_reindexed)
+    # exp.export_data(data_name=f"NADA/{reporting_start_str}-{reporting_end_str}_reindexed.parquet", data=df_reindexed)      
 
     #   # logging.info("Result object", json.dumps(result))
        
     # finally:
     return df_reindexed
     # nada_importfile:Path = Path("data/out") / \
     #                        f"{reporting_start}_{reporting_end}_surveytxt.csv"
     # nada = generate_nada_export(df_reindexed, outfile=nada_importfile)
 
     # return nada
+
+  
+       
+
 if __name__ == "__main__":
+  #  load_blob_config()
     res = main3()
 
 
 
 # def main2():
 #     # TODO:
 #     # envinronemnt setup : Config setup, Expected Directories create, logging setup
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/tests/matching_test.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/tests/matching_test.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/base.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/base.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/ccare_to_aztable.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/ccare_to_aztable.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/df_ops_base.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/df_ops_base.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/dtypes.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/dtypes.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/environment.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/environment.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/fromstr.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/fromstr.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/group_utils.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/group_utils.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher/utils/io.py` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher/utils/io.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/PKG-INFO` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assessment_episode_matcher
-Version: 0.4.0
+Version: 0.5.2
 Author: Aftab Jalal
 Author-email: mj@auditlytics.nz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `assessment_episode_matcher-0.4.0/assessment_episode_matcher.egg-info/SOURCES.txt` & `assessment_episode_matcher-0.5.2/assessment_episode_matcher.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 requirements.txt
 setup.py
 assessment_episode_matcher/__init__.py
 assessment_episode_matcher/audits.py
 assessment_episode_matcher/data_config.py
 assessment_episode_matcher/data_prep.py
 assessment_episode_matcher/mytypes.py
+assessment_episode_matcher/nada.py
 assessment_episode_matcher/test_surveytxt.py
+assessment_episode_matcher/test_surveytxt_local.py
 assessment_episode_matcher/version.py
 assessment_episode_matcher.egg-info/PKG-INFO
 assessment_episode_matcher.egg-info/SOURCES.txt
 assessment_episode_matcher.egg-info/dependency_links.txt
 assessment_episode_matcher.egg-info/requires.txt
 assessment_episode_matcher.egg-info/top_level.txt
 assessment_episode_matcher/azutil/__init__.py
@@ -27,14 +29,15 @@
 assessment_episode_matcher/exporters/__init__.py
 assessment_episode_matcher/exporters/main.py
 assessment_episode_matcher/importers/__init__.py
 assessment_episode_matcher/importers/aod.py
 assessment_episode_matcher/importers/assessments.py
 assessment_episode_matcher/importers/episodes.py
 assessment_episode_matcher/importers/main.py
+assessment_episode_matcher/importers/nada_indexed.py
 assessment_episode_matcher/matching/__init__.py
 assessment_episode_matcher/matching/date_checks.py
 assessment_episode_matcher/matching/errors.py
 assessment_episode_matcher/matching/increasing_slack.py
 assessment_episode_matcher/matching/main.py
 assessment_episode_matcher/matching/matching_stats.py
 assessment_episode_matcher/setup/__init__.py
```

### Comparing `assessment_episode_matcher-0.4.0/setup.py` & `assessment_episode_matcher-0.5.2/setup.py`

 * *Files identical despite different names*

