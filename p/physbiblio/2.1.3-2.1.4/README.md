# Comparing `tmp/physbiblio-2.1.3.tar.gz` & `tmp/physbiblio-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physbiblio-2.1.3.tar", last modified: Mon Oct 16 10:35:00 2023, max compression
+gzip compressed data, was "physbiblio-2.1.4.tar", last modified: Mon May 27 07:50:30 2024, max compression
```

## Comparing `physbiblio-2.1.3.tar` & `physbiblio-2.1.4.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2023-10-16 10:35:00.565920 physbiblio-2.1.3/
--rw-r--r--   0 steog88   (1000) steog88   (1000)    19382 2023-10-16 10:35:00.000000 physbiblio-2.1.3/CHANGELOG
--rw-rw-r--   0 steog88   (1000) steog88   (1000)    35147 2019-01-09 15:43:08.000000 physbiblio-2.1.3/LICENSE
--rw-r--r--   0 steog88   (1000) steog88   (1000)    17813 2023-10-16 10:35:00.565920 physbiblio-2.1.3/PKG-INFO
--rwxr-xr-x   0 steog88   (1000) steog88   (1000)      697 2020-07-16 14:03:13.000000 physbiblio-2.1.3/PhysBiblio.exe
--rw-r--r--   0 steog88   (1000) steog88   (1000)    16734 2023-06-07 12:58:11.000000 physbiblio-2.1.3/README.md
-drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2023-10-16 10:35:00.559254 physbiblio-2.1.3/physbiblio/
--rw-r--r--   0 steog88   (1000) steog88   (1000)      556 2020-07-21 09:43:46.000000 physbiblio-2.1.3/physbiblio/__init__.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     9858 2023-09-08 16:21:54.000000 physbiblio-2.1.3/physbiblio/argParser.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     3588 2022-10-31 20:11:59.000000 physbiblio-2.1.3/physbiblio/bibtexWriter.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     1173 2022-06-18 07:42:38.000000 physbiblio-2.1.3/physbiblio/cli.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    42285 2022-11-01 14:24:29.000000 physbiblio-2.1.3/physbiblio/config.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)   182151 2023-09-15 13:49:54.000000 physbiblio-2.1.3/physbiblio/database.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    13329 2023-06-07 11:48:49.000000 physbiblio-2.1.3/physbiblio/databaseCore.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     3562 2022-06-07 22:29:27.000000 physbiblio-2.1.3/physbiblio/errors.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    22218 2023-09-15 13:31:03.000000 physbiblio-2.1.3/physbiblio/export.py
-drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2023-10-16 10:35:00.559254 physbiblio-2.1.3/physbiblio/gui/
--rw-r--r--   0 steog88   (1000) steog88   (1000)      491 2022-06-18 07:42:38.000000 physbiblio-2.1.3/physbiblio/gui/__init__.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     6379 2022-11-01 14:38:25.000000 physbiblio-2.1.3/physbiblio/gui/basicDialogs.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)   140206 2023-09-15 13:49:54.000000 physbiblio-2.1.3/physbiblio/gui/bibWindows.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    28777 2023-09-15 13:49:49.000000 physbiblio-2.1.3/physbiblio/gui/catWindows.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    37554 2023-06-19 16:45:05.000000 physbiblio-2.1.3/physbiblio/gui/commonClasses.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    34589 2023-06-07 12:58:11.000000 physbiblio-2.1.3/physbiblio/gui/dialogWindows.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     3338 2022-06-18 07:42:38.000000 physbiblio-2.1.3/physbiblio/gui/errorManager.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    20112 2023-09-15 13:49:48.000000 physbiblio-2.1.3/physbiblio/gui/expWindows.py
-drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2023-10-16 10:35:00.562587 physbiblio-2.1.3/physbiblio/gui/images/
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     3017 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/application-exit.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     2987 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/application-pdf.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)      793 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/arrow-down.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)      807 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/arrow-up.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     2101 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/delete.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     2339 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/dialog-error.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     1973 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/dialog-ok-apply.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     2312 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/dialog-warning.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     4482 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/download.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     3898 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/edit-clear.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     5150 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/edit-find-replace.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     1242 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/edit-node.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)      778 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/edit-select-all.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     3505 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/edit-undo.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     1007 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/edit-unselect-all.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     1970 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/edit.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     1573 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/emblem-favorite-symbolic.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)      202 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/emblem-important-symbolic.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     1224 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/emblem-question.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)      414 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/emblem-remove.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     2783 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/export-table.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     2427 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/export.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     2658 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/file-add.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)      368 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/file-save.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     3065 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/find.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     2742 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/help-about.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     2314 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/icon.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     1358 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/profiles.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     3743 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/refresh.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)      422 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/refresh2.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     2073 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/settings.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)      204 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/stats.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     2533 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/terminal.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     1459 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/unread-new.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     1415 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/view-filter.png
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     5776 2019-01-09 15:43:08.000000 physbiblio-2.1.3/physbiblio/gui/images/web-search.png
--rw-r--r--   0 steog88   (1000) steog88   (1000)    10551 2022-10-21 14:19:30.000000 physbiblio-2.1.3/physbiblio/gui/inspireStatsGUI.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    79692 2023-09-15 13:49:51.000000 physbiblio-2.1.3/physbiblio/gui/mainWindow.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     2905 2022-06-18 07:42:38.000000 physbiblio-2.1.3/physbiblio/gui/marks.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    19467 2022-11-01 14:33:17.000000 physbiblio-2.1.3/physbiblio/gui/profilesManager.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)   243177 2022-06-18 07:42:38.000000 physbiblio-2.1.3/physbiblio/gui/resourcesPyside6.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     1977 2022-06-18 07:42:38.000000 physbiblio-2.1.3/physbiblio/gui/setuptests.py
-drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2023-10-16 10:35:00.565920 physbiblio-2.1.3/physbiblio/gui/tests/
--rw-r--r--   0 steog88   (1000) steog88   (1000)      512 2019-05-07 21:18:56.000000 physbiblio-2.1.3/physbiblio/gui/tests/__init__.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     8605 2022-11-01 15:43:25.000000 physbiblio-2.1.3/physbiblio/gui/tests/test_basicDialogs.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)   382182 2023-09-15 13:50:04.000000 physbiblio-2.1.3/physbiblio/gui/tests/test_bibWindows.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    76381 2023-09-15 13:49:52.000000 physbiblio-2.1.3/physbiblio/gui/tests/test_catWindows.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    66570 2023-06-19 16:45:05.000000 physbiblio-2.1.3/physbiblio/gui/tests/test_commonClasses.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    66107 2023-06-07 12:58:11.000000 physbiblio-2.1.3/physbiblio/gui/tests/test_dialogWindows.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     3539 2022-06-18 07:42:38.000000 physbiblio-2.1.3/physbiblio/gui/tests/test_errorManager.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    58239 2023-09-15 13:49:51.000000 physbiblio-2.1.3/physbiblio/gui/tests/test_expWindows.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    77615 2022-11-01 15:40:20.000000 physbiblio-2.1.3/physbiblio/gui/tests/test_inspireStatsGUI.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)   222336 2023-09-15 13:49:59.000000 physbiblio-2.1.3/physbiblio/gui/tests/test_mainWindow.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     3397 2022-11-01 15:39:38.000000 physbiblio-2.1.3/physbiblio/gui/tests/test_marks.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    48747 2022-11-01 15:38:58.000000 physbiblio-2.1.3/physbiblio/gui/tests/test_profilesManager.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    45530 2023-09-15 13:49:52.000000 physbiblio-2.1.3/physbiblio/gui/tests/test_threadElements.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    30403 2023-09-15 13:40:41.000000 physbiblio-2.1.3/physbiblio/gui/threadElements.py
--rwxr-xr-x   0 steog88   (1000) steog88   (1000)       61 2022-06-18 07:42:38.000000 physbiblio-2.1.3/physbiblio/gui/update_resources.sh
--rw-r--r--   0 steog88   (1000) steog88   (1000)    22300 2022-10-21 14:23:55.000000 physbiblio-2.1.3/physbiblio/inspireStats.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     2619 2020-07-16 14:12:59.000000 physbiblio-2.1.3/physbiblio/parseAccents.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    18024 2023-06-07 09:54:50.000000 physbiblio-2.1.3/physbiblio/pdf.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     3691 2023-09-14 20:57:13.000000 physbiblio-2.1.3/physbiblio/setuptests.py
-drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2023-10-16 10:35:00.565920 physbiblio-2.1.3/physbiblio/strings/
--rw-rw-r--   0 steog88   (1000) steog88   (1000)      292 2020-02-01 04:21:09.000000 physbiblio-2.1.3/physbiblio/strings/__init__.py
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     1084 2020-02-01 04:21:09.000000 physbiblio-2.1.3/physbiblio/strings/common.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    30932 2023-09-11 17:45:43.000000 physbiblio-2.1.3/physbiblio/strings/gui.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    27836 2023-09-14 13:59:57.000000 physbiblio-2.1.3/physbiblio/strings/main.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     2868 2023-06-07 12:58:11.000000 physbiblio-2.1.3/physbiblio/strings/webimport.py
--rw-rw-r--   0 steog88   (1000) steog88   (1000)     3514 2021-07-05 15:58:20.000000 physbiblio-2.1.3/physbiblio/tablesDef.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     1991 2022-10-31 20:14:32.000000 physbiblio-2.1.3/physbiblio/testLoader.py
-drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2023-10-16 10:35:00.565920 physbiblio-2.1.3/physbiblio/tests/
--rw-rw-r--   0 steog88   (1000) steog88   (1000)      412 2019-08-26 10:19:28.000000 physbiblio-2.1.3/physbiblio/tests/__init__.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    22763 2023-09-08 16:26:34.000000 physbiblio-2.1.3/physbiblio/tests/test_argParser.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     3507 2022-06-18 07:42:38.000000 physbiblio-2.1.3/physbiblio/tests/test_bibtexWriter.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    92610 2022-11-01 14:18:41.000000 physbiblio-2.1.3/physbiblio/tests/test_config.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)   388852 2023-09-15 13:47:15.000000 physbiblio-2.1.3/physbiblio/tests/test_database.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     7124 2022-06-18 07:42:38.000000 physbiblio-2.1.3/physbiblio/tests/test_errors.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    29420 2023-09-14 20:23:55.000000 physbiblio-2.1.3/physbiblio/tests/test_export.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     7695 2022-11-01 14:20:17.000000 physbiblio-2.1.3/physbiblio/tests/test_inspireStats.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)      911 2022-06-18 07:42:38.000000 physbiblio-2.1.3/physbiblio/tests/test_package.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    11877 2022-11-01 14:24:29.000000 physbiblio-2.1.3/physbiblio/tests/test_pdf.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     6485 2022-11-01 14:19:24.000000 physbiblio-2.1.3/physbiblio/tests/test_view.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)      182 2023-10-16 10:35:00.000000 physbiblio-2.1.3/physbiblio/version.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     4057 2020-07-16 14:14:14.000000 physbiblio-2.1.3/physbiblio/view.py
-drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2023-10-16 10:35:00.565920 physbiblio-2.1.3/physbiblio/webimport/
--rw-r--r--   0 steog88   (1000) steog88   (1000)      323 2023-06-07 12:58:11.000000 physbiblio-2.1.3/physbiblio/webimport/__init__.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     4392 2022-11-01 14:16:19.000000 physbiblio-2.1.3/physbiblio/webimport/adsnasa.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    14726 2022-11-01 14:16:19.000000 physbiblio-2.1.3/physbiblio/webimport/arxiv.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     1853 2020-07-16 14:10:21.000000 physbiblio-2.1.3/physbiblio/webimport/doi.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    28959 2023-09-12 09:43:21.000000 physbiblio-2.1.3/physbiblio/webimport/inspire.py
-drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2023-10-16 10:35:00.565920 physbiblio-2.1.3/physbiblio/webimport/tests/
--rw-r--r--   0 steog88   (1000) steog88   (1000)      251 2023-06-07 12:58:11.000000 physbiblio-2.1.3/physbiblio/webimport/tests/__init__.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     7132 2022-06-18 07:42:38.000000 physbiblio-2.1.3/physbiblio/webimport/tests/test_adsnasa.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    29809 2022-10-14 12:39:59.000000 physbiblio-2.1.3/physbiblio/webimport/tests/test_arxiv.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    55482 2022-06-18 07:42:38.000000 physbiblio-2.1.3/physbiblio/webimport/tests/test_inspire.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)    18160 2023-06-07 12:58:11.000000 physbiblio-2.1.3/physbiblio/webimport/tests/test_webimport.py
--rw-r--r--   0 steog88   (1000) steog88   (1000)     6887 2022-11-01 14:16:19.000000 physbiblio-2.1.3/physbiblio/webimport/webInterf.py
-drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2023-10-16 10:35:00.559254 physbiblio-2.1.3/physbiblio.egg-info/
--rw-r--r--   0 steog88   (1000) steog88   (1000)    17813 2023-10-16 10:35:00.000000 physbiblio-2.1.3/physbiblio.egg-info/PKG-INFO
--rw-r--r--   0 steog88   (1000) steog88   (1000)     3916 2023-10-16 10:35:00.000000 physbiblio-2.1.3/physbiblio.egg-info/SOURCES.txt
--rw-r--r--   0 steog88   (1000) steog88   (1000)        1 2023-10-16 10:35:00.000000 physbiblio-2.1.3/physbiblio.egg-info/dependency_links.txt
--rw-r--r--   0 steog88   (1000) steog88   (1000)      215 2023-10-16 10:35:00.000000 physbiblio-2.1.3/physbiblio.egg-info/requires.txt
--rw-r--r--   0 steog88   (1000) steog88   (1000)       11 2023-10-16 10:35:00.000000 physbiblio-2.1.3/physbiblio.egg-info/top_level.txt
--rw-rw-r--   0 steog88   (1000) steog88   (1000)      103 2023-10-16 10:35:00.565920 physbiblio-2.1.3/setup.cfg
--rw-r--r--   0 steog88   (1000) steog88   (1000)     2372 2023-03-10 11:07:31.000000 physbiblio-2.1.3/setup.py
+drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2024-05-27 07:50:30.169927 physbiblio-2.1.4/
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    19472 2024-05-27 07:50:29.000000 physbiblio-2.1.4/CHANGELOG
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)    35147 2019-01-09 15:43:08.000000 physbiblio-2.1.4/LICENSE
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    18386 2024-05-27 07:50:30.169927 physbiblio-2.1.4/PKG-INFO
+-rwxr-xr-x   0 steog88   (1000) steog88   (1000)      697 2020-07-16 14:03:13.000000 physbiblio-2.1.4/PhysBiblio.exe
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    16734 2023-06-07 12:58:11.000000 physbiblio-2.1.4/README.md
+drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2024-05-27 07:50:30.156594 physbiblio-2.1.4/physbiblio/
+-rw-r--r--   0 steog88   (1000) steog88   (1000)      557 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/__init__.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     9859 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/argParser.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     3589 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/bibtexWriter.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     1174 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/cli.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    42334 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/config.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)   182488 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/database.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    13330 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/databaseCore.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     3563 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/errors.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    22219 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/export.py
+drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2024-05-27 07:50:30.159927 physbiblio-2.1.4/physbiblio/gui/
+-rw-r--r--   0 steog88   (1000) steog88   (1000)      492 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/gui/__init__.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     6379 2022-11-01 14:38:25.000000 physbiblio-2.1.4/physbiblio/gui/basicDialogs.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)   140311 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/gui/bibWindows.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    28778 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/gui/catWindows.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    37555 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/gui/commonClasses.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    34734 2024-05-26 21:08:42.000000 physbiblio-2.1.4/physbiblio/gui/dialogWindows.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     3339 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/gui/errorManager.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    20113 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/gui/expWindows.py
+drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2024-05-27 07:50:30.163260 physbiblio-2.1.4/physbiblio/gui/images/
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     3017 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/application-exit.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     2987 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/application-pdf.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)      793 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/arrow-down.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)      807 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/arrow-up.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     2101 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/delete.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     2339 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/dialog-error.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     1973 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/dialog-ok-apply.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     2312 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/dialog-warning.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     4482 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/download.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     3898 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/edit-clear.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     5150 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/edit-find-replace.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     1242 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/edit-node.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)      778 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/edit-select-all.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     3505 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/edit-undo.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     1007 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/edit-unselect-all.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     1970 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/edit.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     1573 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/emblem-favorite-symbolic.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)      202 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/emblem-important-symbolic.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     1224 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/emblem-question.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)      414 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/emblem-remove.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     2783 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/export-table.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     2427 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/export.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     2658 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/file-add.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)      368 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/file-save.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     3065 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/find.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     2742 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/help-about.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     2314 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/icon.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     1358 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/profiles.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     3743 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/refresh.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)      422 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/refresh2.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     2073 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/settings.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)      204 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/stats.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     2533 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/terminal.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     1459 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/unread-new.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     1415 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/view-filter.png
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     5776 2019-01-09 15:43:08.000000 physbiblio-2.1.4/physbiblio/gui/images/web-search.png
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    10552 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/gui/inspireStatsGUI.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    79713 2024-05-27 07:05:43.000000 physbiblio-2.1.4/physbiblio/gui/mainWindow.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     2906 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/gui/marks.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    19468 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/gui/profilesManager.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)   243177 2022-06-18 07:42:38.000000 physbiblio-2.1.4/physbiblio/gui/resourcesPyside6.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     1978 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/gui/setuptests.py
+drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2024-05-27 07:50:30.166594 physbiblio-2.1.4/physbiblio/gui/tests/
+-rw-r--r--   0 steog88   (1000) steog88   (1000)      513 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/gui/tests/__init__.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     8605 2022-11-01 15:43:25.000000 physbiblio-2.1.4/physbiblio/gui/tests/test_basicDialogs.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)   382189 2024-05-26 21:22:34.000000 physbiblio-2.1.4/physbiblio/gui/tests/test_bibWindows.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    76381 2023-09-15 13:49:52.000000 physbiblio-2.1.4/physbiblio/gui/tests/test_catWindows.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    66570 2023-06-19 16:45:05.000000 physbiblio-2.1.4/physbiblio/gui/tests/test_commonClasses.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    66107 2024-05-26 21:12:52.000000 physbiblio-2.1.4/physbiblio/gui/tests/test_dialogWindows.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     3539 2022-06-18 07:42:38.000000 physbiblio-2.1.4/physbiblio/gui/tests/test_errorManager.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    58239 2023-09-15 13:49:51.000000 physbiblio-2.1.4/physbiblio/gui/tests/test_expWindows.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    77615 2022-11-01 15:40:20.000000 physbiblio-2.1.4/physbiblio/gui/tests/test_inspireStatsGUI.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)   222499 2024-05-27 07:14:41.000000 physbiblio-2.1.4/physbiblio/gui/tests/test_mainWindow.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     3397 2022-11-01 15:39:38.000000 physbiblio-2.1.4/physbiblio/gui/tests/test_marks.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    48747 2022-11-01 15:38:58.000000 physbiblio-2.1.4/physbiblio/gui/tests/test_profilesManager.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    45530 2023-09-15 13:49:52.000000 physbiblio-2.1.4/physbiblio/gui/tests/test_threadElements.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    30404 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/gui/threadElements.py
+-rwxr-xr-x   0 steog88   (1000) steog88   (1000)       61 2022-06-18 07:42:38.000000 physbiblio-2.1.4/physbiblio/gui/update_resources.sh
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    22301 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/inspireStats.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     2619 2020-07-16 14:12:59.000000 physbiblio-2.1.4/physbiblio/parseAccents.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    18025 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/pdf.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     3692 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/setuptests.py
+drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2024-05-27 07:50:30.166594 physbiblio-2.1.4/physbiblio/strings/
+-rw-r--r--   0 steog88   (1000) steog88   (1000)      293 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/strings/__init__.py
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)     1084 2020-02-01 04:21:09.000000 physbiblio-2.1.4/physbiblio/strings/common.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    30932 2023-09-11 17:45:43.000000 physbiblio-2.1.4/physbiblio/strings/gui.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    27836 2023-09-14 13:59:57.000000 physbiblio-2.1.4/physbiblio/strings/main.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     2868 2023-06-07 12:58:11.000000 physbiblio-2.1.4/physbiblio/strings/webimport.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     3515 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/tablesDef.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     1992 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/testLoader.py
+drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2024-05-27 07:50:30.166594 physbiblio-2.1.4/physbiblio/tests/
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)      412 2019-08-26 10:19:28.000000 physbiblio-2.1.4/physbiblio/tests/__init__.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    22763 2023-09-08 16:26:34.000000 physbiblio-2.1.4/physbiblio/tests/test_argParser.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     3507 2022-06-18 07:42:38.000000 physbiblio-2.1.4/physbiblio/tests/test_bibtexWriter.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    92610 2022-11-01 14:18:41.000000 physbiblio-2.1.4/physbiblio/tests/test_config.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)   388852 2023-09-15 13:47:15.000000 physbiblio-2.1.4/physbiblio/tests/test_database.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     7124 2022-06-18 07:42:38.000000 physbiblio-2.1.4/physbiblio/tests/test_errors.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    29420 2023-09-14 20:23:55.000000 physbiblio-2.1.4/physbiblio/tests/test_export.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     7695 2022-11-01 14:20:17.000000 physbiblio-2.1.4/physbiblio/tests/test_inspireStats.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)      911 2022-06-18 07:42:38.000000 physbiblio-2.1.4/physbiblio/tests/test_package.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    11877 2022-11-01 14:24:29.000000 physbiblio-2.1.4/physbiblio/tests/test_pdf.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     6485 2022-11-01 14:19:24.000000 physbiblio-2.1.4/physbiblio/tests/test_view.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)      156 2024-05-27 07:50:29.000000 physbiblio-2.1.4/physbiblio/version.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     4058 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/view.py
+drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2024-05-27 07:50:30.166594 physbiblio-2.1.4/physbiblio/webimport/
+-rw-r--r--   0 steog88   (1000) steog88   (1000)      324 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/webimport/__init__.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     4393 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/webimport/adsnasa.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    14727 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/webimport/arxiv.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     1854 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/webimport/doi.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    29024 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/webimport/inspire.py
+drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2024-05-27 07:50:30.169927 physbiblio-2.1.4/physbiblio/webimport/tests/
+-rw-r--r--   0 steog88   (1000) steog88   (1000)      252 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/webimport/tests/__init__.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     7132 2022-06-18 07:42:38.000000 physbiblio-2.1.4/physbiblio/webimport/tests/test_adsnasa.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    29809 2022-10-14 12:39:59.000000 physbiblio-2.1.4/physbiblio/webimport/tests/test_arxiv.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    55482 2022-06-18 07:42:38.000000 physbiblio-2.1.4/physbiblio/webimport/tests/test_inspire.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    18267 2024-05-27 07:05:43.000000 physbiblio-2.1.4/physbiblio/webimport/tests/test_webimport.py
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     6888 2024-05-26 21:06:38.000000 physbiblio-2.1.4/physbiblio/webimport/webInterf.py
+drwxr-xr-x   0 steog88   (1000) steog88   (1000)        0 2024-05-27 07:50:30.169927 physbiblio-2.1.4/physbiblio.egg-info/
+-rw-r--r--   0 steog88   (1000) steog88   (1000)    18386 2024-05-27 07:50:30.000000 physbiblio-2.1.4/physbiblio.egg-info/PKG-INFO
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     3916 2024-05-27 07:50:30.000000 physbiblio-2.1.4/physbiblio.egg-info/SOURCES.txt
+-rw-r--r--   0 steog88   (1000) steog88   (1000)        1 2024-05-27 07:50:30.000000 physbiblio-2.1.4/physbiblio.egg-info/dependency_links.txt
+-rw-r--r--   0 steog88   (1000) steog88   (1000)      215 2024-05-27 07:50:30.000000 physbiblio-2.1.4/physbiblio.egg-info/requires.txt
+-rw-r--r--   0 steog88   (1000) steog88   (1000)       11 2024-05-27 07:50:30.000000 physbiblio-2.1.4/physbiblio.egg-info/top_level.txt
+-rw-rw-r--   0 steog88   (1000) steog88   (1000)      103 2024-05-27 07:50:30.169927 physbiblio-2.1.4/setup.cfg
+-rw-r--r--   0 steog88   (1000) steog88   (1000)     2372 2023-03-10 11:07:31.000000 physbiblio-2.1.4/setup.py
```

### Comparing `physbiblio-2.1.3/CHANGELOG` & `physbiblio-2.1.4/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2.1.4 (2024-05-27):
+    * bug fixing and updates with recent PySide6 and python versions
+
 2.1.3 (2023-09-16):
     * exportForTexFile runs checkDuplicates
     * small internal improvements
     * bug fixing
 
 2.1.2 (2023-09-11):
     * function printDuplicates to show the output nicely, command line option to check and print the duplicates
```

### Comparing `physbiblio-2.1.3/LICENSE` & `physbiblio-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/PKG-INFO` & `physbiblio-2.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: physbiblio
-Version: 2.1.3
-Summary: A bibliography manager in Python (using Sqlite and PySide6)
-Home-page: https://github.com/steog88/PhysBiblio
-Author: Stefano Gariazzo
-Author-email: stefano.gariazzo@gmail.com
-License: GPL-3.0
-Keywords: bibliography,hep-ph,high-energy-physics,bibtex
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Provides: physbiblio
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # [PhysBiblio](https://github.com/steog88/PhysBiblio)
 Bibliography manager in Python  
 by S. Gariazzo (stefano.gariazzo@gmail.com)
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/steog88/PhysBiblio/blob/master/LICENSE)
 [![PyPI version](https://img.shields.io/pypi/v/physbiblio.svg?style=flat-square)](https://pypi.org/project/physbiblio/)
 [![PyPI version](https://img.shields.io/pypi/pyversions/physbiblio.svg?style=flat-square)](https://pypi.org/project/physbiblio/)
```

### Comparing `physbiblio-2.1.3/PhysBiblio.exe` & `physbiblio-2.1.4/PhysBiblio.exe`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/README.md` & `physbiblio-2.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,53 @@
+Metadata-Version: 2.1
+Name: physbiblio
+Version: 2.1.4
+Summary: A bibliography manager in Python (using Sqlite and PySide6)
+Home-page: https://github.com/steog88/PhysBiblio
+Author: Stefano Gariazzo
+Author-email: stefano.gariazzo@gmail.com
+License: GPL-3.0
+Keywords: bibliography,hep-ph,high-energy-physics,bibtex
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Provides: physbiblio
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ads
+Requires-Dist: appdirs
+Requires-Dist: argparse
+Requires-Dist: bibtexparser>=1.1.0
+Requires-Dist: dictdiffer
+Requires-Dist: feedparser
+Requires-Dist: matplotlib>=3.6.2
+Requires-Dist: outdated
+Requires-Dist: pylatexenc>=2.0
+Requires-Dist: pyparsing>=2.4.0
+Requires-Dist: pyside6>=6.4.0
+Requires-Dist: pytz
+Requires-Dist: requests>=2.25
+Requires-Dist: urllib3>=1.26
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pyyaml; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
 # [PhysBiblio](https://github.com/steog88/PhysBiblio)
 Bibliography manager in Python  
 by S. Gariazzo (stefano.gariazzo@gmail.com)
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/steog88/PhysBiblio/blob/master/LICENSE)
 [![PyPI version](https://img.shields.io/pypi/v/physbiblio.svg?style=flat-square)](https://pypi.org/project/physbiblio/)
 [![PyPI version](https://img.shields.io/pypi/pyversions/physbiblio.svg?style=flat-square)](https://pypi.org/project/physbiblio/)
```

### Comparing `physbiblio-2.1.3/physbiblio/__init__.py` & `physbiblio-2.1.4/physbiblio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """The package that contains all the modules used by the PhysBiblio,
 including the `gui` subpackage.
 
 This file is part of the physbiblio package.
 """
+
 __author__ = "Stefano Gariazzo"
 __email__ = "stefano.gariazzo@gmail.com"
 
 __all__ = [
     "bibtexWriter",
     "cli",
     "config",
```

### Comparing `physbiblio-2.1.3/physbiblio/argParser.py` & `physbiblio-2.1.4/physbiblio/argParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module that manages the command line calls of PhysBiblio.
 
 This file is part of the physbiblio package.
 """
+
 import argparse
 import datetime
 import sys
 
 from PySide6.QtWidgets import QApplication
 
 try:
```

### Comparing `physbiblio-2.1.3/physbiblio/bibtexWriter.py` & `physbiblio-2.1.4/physbiblio/bibtexWriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module that contains the PBBibTexWriter class
 (needed to override _entry_to_bibtex).
 
 This file is part of the physbiblio package.
 """
+
 import traceback
 
 from bibtexparser.bwriter import BibTexWriter
 
 try:
     from physbiblio.strings.main import BibtexWriterStrings as bwstr
 except ImportError:
```

### Comparing `physbiblio-2.1.3/physbiblio/cli.py` & `physbiblio-2.1.4/physbiblio/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module that creates a command line interface to manually run
 the PhysBiblio internal commands.
 
 This file is part of the physbiblio package.
 """
+
 import code
 import readline  # optional, will allow Up/Down/History in the console
 import traceback
 
 try:
     import physbiblio.webimport.webInterf as webInt
     from physbiblio.config import pbConfig
```

### Comparing `physbiblio-2.1.3/physbiblio/config.py` & `physbiblio-2.1.4/physbiblio/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Manages the configuration of PhysBiblio, from saving to reading.
 
 This file is part of the physbiblio package.
 """
+
 import ast
 import logging
 import logging.handlers
 import os
 import sys
 import traceback
 from collections import OrderedDict
@@ -1050,17 +1051,19 @@
         allProf = self.globalDb.getProfiles()
         profiles = {}
         for e in allProf:
             profiles[e["name"]] = {
                 "n": e["name"],
                 "d": e["description"],
                 "f": e["oldCfg"],
-                "db": e["databasefile"]
-                if os.sep in e["databasefile"]
-                else os.path.join(self.dataPath, e["databasefile"]),
+                "db": (
+                    e["databasefile"]
+                    if os.sep in e["databasefile"]
+                    else os.path.join(self.dataPath, e["databasefile"])
+                ),
             }
         return (
             self.globalDb.getDefaultProfile(),
             profiles,
             self.globalDb.getProfileOrder(),
         )
```

### Comparing `physbiblio-2.1.3/physbiblio/database.py` & `physbiblio-2.1.4/physbiblio/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module that manages the actions on the database (and few more).
 
 This file is part of the physbiblio package.
 """
+
 import ast
 import datetime
 import os
 import re
 import traceback
 from sqlite3 import DatabaseError, InterfaceError, OperationalError, ProgrammingError
 
@@ -122,17 +123,19 @@
                 if "cats" in searchFields.keys():
                     first = False
                     newContent.append(
                         {
                             "type": "Categories",
                             "logical": None,
                             "field": "",
-                            "operator": "all the following"
-                            if searchFields["cats"]["operator"] == "and"
-                            else "at least one among",
+                            "operator": (
+                                "all the following"
+                                if searchFields["cats"]["operator"] == "and"
+                                else "at least one among"
+                            ),
                             "content": searchFields["cats"]["id"],
                         }
                     )
                     del searchFields["cats"]
                 if not first:
                     try:
                         ceop = searchFields["catExpOperator"]
@@ -146,31 +149,35 @@
                     pass
                 if "exps" in searchFields.keys():
                     newContent.append(
                         {
                             "type": "Experiments",
                             "logical": ceop,
                             "field": "",
-                            "operator": "all the following"
-                            if searchFields["exps"]["operator"] == "and"
-                            else "at least one among",
+                            "operator": (
+                                "all the following"
+                                if searchFields["exps"]["operator"] == "and"
+                                else "at least one among"
+                            ),
                             "content": searchFields["exps"]["id"],
                         }
                     )
                     del searchFields["exps"]
                 if "marks" in searchFields.keys():
                     newContent.append(
                         {
                             "type": "Marks",
                             "logical": searchFields["marks"]["connection"],
                             "field": None,
                             "operator": None,
-                            "content": ["any"]
-                            if searchFields["marks"]["operator"] == "!="
-                            else [searchFields["marks"]["str"]],
+                            "content": (
+                                ["any"]
+                                if searchFields["marks"]["operator"] == "!="
+                                else [searchFields["marks"]["str"]]
+                            ),
                         }
                     )
                     del searchFields["marks"]
                 for t in self.bibs.searchPossibleTypes:
                     if t in searchFields.keys():
                         newContent.append(
                             {
@@ -1675,19 +1682,19 @@
 
         Output:
             the modified 'data' dict
         """
         data["arxiv"] = (
             arxiv
             if arxiv
-            else element["arxiv"]
-            if "arxiv" in element
-            else element["eprint"]
-            if "eprint" in element
-            else ""
+            else (
+                element["arxiv"]
+                if "arxiv" in element
+                else element["eprint"] if "eprint" in element else ""
+            )
         )
         return data
 
     def _prepareInsertBasic(self, data, element, bibkey=None):
         """Read the bibtex key when preparing
         to insert an entry to the database
 
@@ -1836,17 +1843,15 @@
         Output:
             the modified 'data' dict
         """
         for k in ("abstract", "crossref", "doi", "isbn"):
             data[k] = (
                 kwargs[k]
                 if k in kwargs and kwargs[k]
-                else element[k]
-                if k in element
-                else None
+                else element[k] if k in element else None
             )
         for k in ("ads", "comments", "inspire", "old_keys", "scholar"):
             data[k] = kwargs[k] if k in kwargs and kwargs[k] else None
         for k in (
             "book",
             "exp_paper",
             "lecture",
@@ -2082,15 +2087,15 @@
 
         Output:
             a dictionary (key is processed bibtex, value is a set of possible duplicates)
         """
 
         def checkres(key, mat, match, matched, reason):
             if len([k for k in mat if k["bibkey"] != key]) > 0:
-                matched[reason] = [m["bibkey"] for m in mat if m["bibkey"] != k]
+                matched[reason] = [m["bibkey"] for m in mat if m["bibkey"] != key]
                 match = True
             return match, matched
 
         if entries is None:
             entries = self.getAll()
         duplicates = {}
         self.runningCheckDuplicates = True
@@ -4870,25 +4875,29 @@
             return False
         if key != result["bibkey"]:
             self.updateBibkey(key, result["bibkey"])
             key = result["bibkey"]
             self.newKey = key  # saved for searchOAIUpdates
         self.updateRecordFromINSPIRE(
             result,
-            useOld=self.getByBibkey(key, saveQuery=False, verbose=False)
-            if not reloadAll
-            else [
-                {
-                    **{
-                        k: ""
-                        for x, k in physBiblioWeb.webSearch["inspire"].correspondences
-                    },
-                    **{"bibkey": key},
-                }
-            ],
+            useOld=(
+                self.getByBibkey(key, saveQuery=False, verbose=False)
+                if not reloadAll
+                else [
+                    {
+                        **{
+                            k: ""
+                            for x, k in physBiblioWeb.webSearch[
+                                "inspire"
+                            ].correspondences
+                        },
+                        **{"bibkey": key},
+                    }
+                ]
+            ),
             force=True,
         )
         if verbose > 0:
             pBLogger.info(dstr.Bibs.iidSaved % inspireID)
         return True
 
     def updateInspireID(self, string, key=None, number=None):
```

### Comparing `physbiblio-2.1.3/physbiblio/databaseCore.py` & `physbiblio-2.1.4/physbiblio/databaseCore.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module that manages the actions on the database (and few more).
 
 This file is part of the physbiblio package.
 """
+
 import ast
 import os
 import sqlite3
 import sys
 import traceback
 from sqlite3 import (
     DatabaseError,
```

### Comparing `physbiblio-2.1.3/physbiblio/errors.py` & `physbiblio-2.1.4/physbiblio/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module that contains the pBErrorManager and pBLogger definitions.
 
 This file is part of the physbiblio package.
 """
+
 import logging
 import logging.handlers
 import sys
 import traceback
 
 try:
     from physbiblio.config import addFileHandler, getLogLevel, pbConfig
```

### Comparing `physbiblio-2.1.3/physbiblio/export.py` & `physbiblio-2.1.4/physbiblio/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Classes and functions that manage the export
 of the database entries into .bib files.
 
 This file is part of the physbiblio package.
 """
+
 import codecs
 import os
 import re
 import shutil
 import traceback
 
 import bibtexparser
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/basicDialogs.py` & `physbiblio-2.1.4/physbiblio/gui/basicDialogs.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/bibWindows.py` & `physbiblio-2.1.4/physbiblio/gui/bibWindows.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module with the classes and functions that manage
 the entries windows and panels.
 
 This file is part of the physbiblio package.
 """
+
 import ast
 import datetime
 import os
 import re
 import traceback
 
 import bibtexparser
@@ -2669,17 +2670,19 @@
                             "logical": None,
                             "field": None,
                             "type": bwstr.SR.text,
                             "operator": None,
                             "content": "",
                         }
                     ],
-                    "limit": "100000"
-                    if replace
-                    else "%s" % pbConfig.params["defaultLimitBibtexs"],
+                    "limit": (
+                        "100000"
+                        if replace
+                        else "%s" % pbConfig.params["defaultLimitBibtexs"]
+                    ),
                     "offset": "0",
                     "replaceFields": {
                         "regex": False,
                         "double": False,
                         "fieOld": "author",
                         "old": "",
                         "fieNew": "author",
@@ -3093,17 +3096,19 @@
             self.textValues[ix]["content"].installEventFilter(self)
 
         elif previous["type"] in (bwstr.SR.cats, bwstr.SR.exps):
             self.textValues[ix]["field"] = None
 
             self.textValues[ix]["operator"] = PBComboBox(
                 self,
-                self.operators["catexp"]
-                if previous["type"] == bwstr.SR.cats
-                else self.operators["catexp"][0:3],
+                (
+                    self.operators["catexp"]
+                    if previous["type"] == bwstr.SR.cats
+                    else self.operators["catexp"][0:3]
+                ),
                 current=previous["operator"],
             )
             self.currGrid.addWidget(self.textValues[ix]["operator"], ix, 2, 1, 2)
 
             if previous["content"] == "":
                 previous["content"] = []
             self.textValues[ix]["content"] = QPushButton(
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/catWindows.py` & `physbiblio-2.1.4/physbiblio/gui/catWindows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module with the classes and functions that manage
 the categories windows and panels.
 
 This file is part of the physbiblio package.
 """
+
 import traceback
 
 from PySide6.QtCore import Qt, QTimer
 from PySide6.QtGui import QAction, QCursor
 from PySide6.QtWidgets import QLineEdit, QPushButton, QToolTip, QTreeView, QVBoxLayout
 
 try:
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/commonClasses.py` & `physbiblio-2.1.4/physbiblio/gui/commonClasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module with many classes that are further extended
 in the other physbiblio.gui modules.
 
 This file is part of the physbiblio package.
 """
+
 import time
 import traceback
 from queue import Empty
 from weakref import WeakValueDictionary
 
 import PySide6
 from PySide6.QtCore import (
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/dialogWindows.py` & `physbiblio-2.1.4/physbiblio/gui/dialogWindows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module with the classes and functions
 that manage the some dialog windows.
 
 This file is part of the physbiblio package.
 """
+
 import ast
 import traceback
 
 from PySide6.QtCore import Qt, Signal
 from PySide6.QtGui import QTextCursor
 from PySide6.QtWidgets import (
     QCheckBox,
@@ -267,17 +268,19 @@
             )
             grid.addWidget(
                 PBLabel(
                     "%s (<i>%s</i>%s)"
                     % (
                         configuration_params[k].description,
                         k,
-                        (" - " + dwstr.globalSett)
-                        if configuration_params[k].isGlobal
-                        else "",
+                        (
+                            (" - " + dwstr.globalSett)
+                            if configuration_params[k].isGlobal
+                            else ""
+                        ),
                     )
                 ),
                 i - 1,
                 0,
                 1,
                 2,
             )
@@ -311,18 +314,18 @@
                                     int(configuration_params["loggingLevel"].default)
                                 ],
                             ),
                         ]
                     )
             elif k == "logFileName":
                 self.textValues.append([k, QPushButton(val)])
-                self.textValues[-1][1].clicked.connect(self.editFile)
+                self.textValues[-1][1].clicked.connect(lambda x: self.editFile())
             elif k == "defaultCategories":
                 self.textValues.append([k, QPushButton(val)])
-                self.textValues[-1][1].clicked.connect(self.editDefCats)
+                self.textValues[-1][1].clicked.connect(lambda x: self.editDefCats())
             elif configuration_params[k].special == "boolean":
                 self.textValues.append([k, PBTrueFalseCombo(self, val)])
             else:
                 self.textValues.append([k, QLineEdit(val)])
             grid.addWidget(self.textValues[i - 1][1], i - 1, 2, 1, 2)
 
         # OK button
@@ -990,17 +993,19 @@
         self.grid.addWidget(self.bibButton, 0, 2, 1, 2)
 
         self.texButtons = []
         for ix in range(self.numTexFields):
             self.grid.addWidget(PBLabelRight(dwstr.texNames), ix + 1, 0, 1, 2)
             self.texButtons.append(
                 QPushButton(
-                    dwstr.selFile
-                    if self.texFileNames[ix] == ""
-                    else "%s" % self.texFileNames[ix],
+                    (
+                        dwstr.selFile
+                        if self.texFileNames[ix] == ""
+                        else "%s" % self.texFileNames[ix]
+                    ),
                     self,
                 )
             )
             self.texButtons[ix].clicked.connect(lambda s=False, p=ix: self.onAskTex(p))
             self.grid.addWidget(self.texButtons[ix], ix + 1, 2, 1, 2)
 
         i = 2 + self.numTexFields
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/errorManager.py` & `physbiblio-2.1.4/physbiblio/gui/errorManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module with the class that manages errors when the GUI is active.
 
 This file is part of the physbiblio package.
 """
+
 import logging
 import traceback
 from io import StringIO
 
 from PySide6.QtWidgets import QMessageBox
 
 try:
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/expWindows.py` & `physbiblio-2.1.4/physbiblio/gui/expWindows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module with the classes and functions that manage
 the experiments windows and panels.
 
 This file is part of the physbiblio package.
 """
+
 import traceback
 
 from PySide6.QtCore import Qt, QTimer
 from PySide6.QtGui import QAction, QCursor
 from PySide6.QtWidgets import QLineEdit, QPushButton, QToolTip
 
 try:
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/application-exit.png` & `physbiblio-2.1.4/physbiblio/gui/images/application-exit.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/application-pdf.png` & `physbiblio-2.1.4/physbiblio/gui/images/application-pdf.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/arrow-down.png` & `physbiblio-2.1.4/physbiblio/gui/images/arrow-down.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/arrow-up.png` & `physbiblio-2.1.4/physbiblio/gui/images/arrow-up.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/delete.png` & `physbiblio-2.1.4/physbiblio/gui/images/delete.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/dialog-error.png` & `physbiblio-2.1.4/physbiblio/gui/images/dialog-error.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/dialog-ok-apply.png` & `physbiblio-2.1.4/physbiblio/gui/images/dialog-ok-apply.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/dialog-warning.png` & `physbiblio-2.1.4/physbiblio/gui/images/dialog-warning.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/download.png` & `physbiblio-2.1.4/physbiblio/gui/images/download.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/edit-clear.png` & `physbiblio-2.1.4/physbiblio/gui/images/edit-clear.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/edit-find-replace.png` & `physbiblio-2.1.4/physbiblio/gui/images/edit-find-replace.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/edit-node.png` & `physbiblio-2.1.4/physbiblio/gui/images/edit-node.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/edit-select-all.png` & `physbiblio-2.1.4/physbiblio/gui/images/edit-select-all.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/edit-undo.png` & `physbiblio-2.1.4/physbiblio/gui/images/edit-undo.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/edit-unselect-all.png` & `physbiblio-2.1.4/physbiblio/gui/images/edit-unselect-all.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/edit.png` & `physbiblio-2.1.4/physbiblio/gui/images/edit.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/emblem-favorite-symbolic.png` & `physbiblio-2.1.4/physbiblio/gui/images/emblem-favorite-symbolic.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/emblem-question.png` & `physbiblio-2.1.4/physbiblio/gui/images/emblem-question.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/export-table.png` & `physbiblio-2.1.4/physbiblio/gui/images/export-table.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/export.png` & `physbiblio-2.1.4/physbiblio/gui/images/export.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/file-add.png` & `physbiblio-2.1.4/physbiblio/gui/images/file-add.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/find.png` & `physbiblio-2.1.4/physbiblio/gui/images/find.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/help-about.png` & `physbiblio-2.1.4/physbiblio/gui/images/help-about.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/icon.png` & `physbiblio-2.1.4/physbiblio/gui/images/icon.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/profiles.png` & `physbiblio-2.1.4/physbiblio/gui/images/profiles.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/refresh.png` & `physbiblio-2.1.4/physbiblio/gui/images/refresh.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/settings.png` & `physbiblio-2.1.4/physbiblio/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/terminal.png` & `physbiblio-2.1.4/physbiblio/gui/images/terminal.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/unread-new.png` & `physbiblio-2.1.4/physbiblio/gui/images/unread-new.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/view-filter.png` & `physbiblio-2.1.4/physbiblio/gui/images/view-filter.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/images/web-search.png` & `physbiblio-2.1.4/physbiblio/gui/images/web-search.png`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/inspireStatsGUI.py` & `physbiblio-2.1.4/physbiblio/gui/inspireStatsGUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module with the classes that manage the authorStats
 and paperStats plots.
 
 This file is part of the physbiblio package.
 """
+
 import datetime
 import traceback
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.backends.backend_qtagg import FigureCanvasQTAgg as FigureCanvas
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/mainWindow.py` & `physbiblio-2.1.4/physbiblio/gui/mainWindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module that contains the class for the main window of PhysBiblio.
 
 This file is part of the physbiblio package.
 """
+
 import ast
 import glob
 import os
 import signal
 import sys
 import traceback
 from queue import Queue
@@ -1168,15 +1169,15 @@
         kwargs["pbMax"] = app.pbMax.emit
         kwargs["pbVal"] = app.pbVal.emit
         thr = Thread_func(ws, *args, parent=self, **kwargs)
 
         ws.finished.connect(ws.deleteLater)
         thr.finished.connect(app.enableClose)
         thr.finished.connect(thr.deleteLater)
-        app.closeButton.clicked.connect(lambda a=app, t=thr: closePrintText(a, t))
+        app.closeButton.clicked.connect(lambda *x, a=app, t=thr: closePrintText(a, t))
         if stopFlag:
             app.stopped.connect(thr.setStopFlag)
 
         pBErrorManager.tempHandler(ws, format="%(message)s")
         if addMessage:
             pBLogger.info(addMessage)
         thr.start()
@@ -1557,31 +1558,31 @@
                     pbConfig.globalDb.updateSearchField(
                         idS, "replaceFields", replaceFields
                     )
                     pbConfig.globalDb.commit()
                 pBDB.bibs.fetchFromDict(searchFields, limitOffset=offs)
                 self.runReplace(
                     replaceFields,
-                    newTab=mwstr.newTab
-                    if newSearchWin.newTabCheck.isChecked()
-                    else None,
+                    newTab=(
+                        mwstr.newTab if newSearchWin.newTabCheck.isChecked() else None
+                    ),
                 )
             else:
                 if newSearchWin.save:
                     pbConfig.globalDb.updateSearchField(idS, "searchDict", searchFields)
                     pbConfig.globalDb.updateSearchField(idS, "limitNum", lim)
                     pbConfig.globalDb.updateSearchField(idS, "offsetNum", offs)
                     pbConfig.globalDb.commit()
                 self.runSearchBiblio(
                     searchFields,
                     lim,
                     offs,
-                    newTab=mwstr.newTab
-                    if newSearchWin.newTabCheck.isChecked()
-                    else None,
+                    newTab=(
+                        mwstr.newTab if newSearchWin.newTabCheck.isChecked() else None
+                    ),
                 )
 
     def delSearchBiblio(self, idS, name):
         """Delete a saved search from the database
 
         Parameters:
             idS: the search id in the database
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/marks.py` & `physbiblio-2.1.4/physbiblio/gui/marks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module with the class that manages marks for the bibtex entries.
 
 This file is part of the physbiblio package.
 """
+
 import traceback
 
 from PySide6.QtWidgets import QCheckBox, QGroupBox, QHBoxLayout, QRadioButton
 
 try:
     import physbiblio.gui.resourcesPyside6
     from physbiblio.strings.gui import MarksStrings as mstr
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/profilesManager.py` & `physbiblio-2.1.4/physbiblio/gui/profilesManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module with the classes and functions
 that enter the profiles management.
 
 This file is part of the physbiblio package.
 """
+
 import glob
 import os
 import shutil
 import traceback
 
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QIcon
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/resourcesPyside6.py` & `physbiblio-2.1.4/physbiblio/gui/resourcesPyside6.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/setuptests.py` & `physbiblio-2.1.4/physbiblio/gui/setuptests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Utilities for in the tests of the physbiblio modules.
 
 This file is part of the physbiblio package.
 """
+
 import traceback
 import unittest
 from io import StringIO
 from unittest.mock import MagicMock, patch
 
 from PySide6.QtWidgets import QApplication, QFileDialog
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/tests/__init__.py` & `physbiblio-2.1.4/physbiblio/gui/tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The package that contains the tests for the `physbiblio.gui` subpackage.
 
 This file is part of the physbiblio package.
 """
+
 from physbiblio import __author__, __email__, __version__, __version_date__
 
 __all__ = [
     "test_basicDialogs",
     "test_bibWindows",
     "test_catWindows",
     "test_commonClasses",
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/tests/test_basicDialogs.py` & `physbiblio-2.1.4/physbiblio/gui/tests/test_basicDialogs.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/tests/test_bibWindows.py` & `physbiblio-2.1.4/physbiblio/gui/tests/test_bibWindows.py`

 * *Files 0% similar despite different names*

```diff
@@ -7368,22 +7368,24 @@
             _cf.assert_called_once_with(sbw, histIndex=0)
 
         sbw = SearchBibsWindow(replace=True)
         sbw.historic = ["a", "b", "c"]
         self.assertEqual(sbw.currentHistoric, 0)
         sbw.readForm()
         with patch.object(
-            SearchBibsWindow, "readForm", wraps=sbw.readForm, autospec=True
+            SearchBibsWindow,
+            "readForm",
+            wraps=sbw.readForm,
         ) as _rf, patch(
             "physbiblio.gui.bibWindows.SearchBibsWindow.cleanLayout", autospec=True
         ) as _cl, patch(
             "physbiblio.gui.bibWindows.SearchBibsWindow.createForm", autospec=True
         ) as _cf:
             QTest.keyPress(sbw, Qt.Key_Down)
-            _rf.assert_called_once_with(sbw)
+            _rf.assert_called_once_with()
             _cl.assert_called_once_with(sbw)
             self.assertEqual(sbw.currentHistoric, 0)
             self.assertEqual(
                 sbw.historic[0],
                 {
                     "limit": "100000",
                     "nrows": 1,
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/tests/test_catWindows.py` & `physbiblio-2.1.4/physbiblio/gui/tests/test_catWindows.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/tests/test_commonClasses.py` & `physbiblio-2.1.4/physbiblio/gui/tests/test_commonClasses.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/tests/test_dialogWindows.py` & `physbiblio-2.1.4/physbiblio/gui/tests/test_dialogWindows.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/tests/test_errorManager.py` & `physbiblio-2.1.4/physbiblio/gui/tests/test_errorManager.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/tests/test_expWindows.py` & `physbiblio-2.1.4/physbiblio/gui/tests/test_expWindows.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/tests/test_inspireStatsGUI.py` & `physbiblio-2.1.4/physbiblio/gui/tests/test_inspireStatsGUI.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/tests/test_mainWindow.py` & `physbiblio-2.1.4/physbiblio/gui/tests/test_mainWindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1681,20 +1681,27 @@
             _th.assert_called_once_with(pBErrorManager, ws, format="%(message)s")
             thr.start.assert_called_once_with()
             app.exec.assert_called_once_with()
             _info.assert_called_once_with("Closing...")
             _rth.assert_called_once_with(pBErrorManager)
             _sbm.assert_not_called()
             _done.assert_called_once_with(self.mainW)
-        app.reject = MagicMock()
-        thr.wait = MagicMock()
         app.enableClose()
-        QTest.mouseClick(app.closeButton, Qt.LeftButton, delay=10)
-        app.reject.assert_called_once()
-        thr.wait.assert_called_once()
+        with patch.object(
+            PrintText,
+            "reject",
+            wraps=app.reject,
+        ) as _r, patch.object(
+            Thread_cleanSpare,
+            "wait",
+            wraps=thr.wait,
+        ) as _w:
+            QTest.mouseClick(app.closeButton, Qt.LeftButton, delay=10)
+            _w.assert_called_once()
+            _r.assert_called_once()
 
         ws.newText.connect.reset_mock()
         func.reset_mock()
         ws.finished.connect.reset_mock()
         thr.finished.connect.reset_mock()
         app.stopped.connect.reset_mock()
         thr.start.reset_mock()
```

### Comparing `physbiblio-2.1.3/physbiblio/gui/tests/test_marks.py` & `physbiblio-2.1.4/physbiblio/gui/tests/test_marks.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/tests/test_profilesManager.py` & `physbiblio-2.1.4/physbiblio/gui/tests/test_profilesManager.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/tests/test_threadElements.py` & `physbiblio-2.1.4/physbiblio/gui/tests/test_threadElements.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/gui/threadElements.py` & `physbiblio-2.1.4/physbiblio/gui/threadElements.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module with the classes that are used to run threads.
 
 This file is part of the physbiblio package.
 """
+
 import time
 import traceback
 from urllib.request import URLError
 
 import bibtexparser
 from outdated import check_outdated
 from PySide6.QtCore import Signal
```

### Comparing `physbiblio-2.1.3/physbiblio/inspireStats.py` & `physbiblio-2.1.4/physbiblio/inspireStats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module that uses INSPIRE-HEP to get author
 (number of papers, h index, citations) and paper statistics (citations).
 
 Uses matplotlib to do plots.
 
 This file is part of the physbiblio package.
 """
+
 import datetime
 import json
 import os
 import os.path as osp
 import traceback
 
 import dateutil
```

### Comparing `physbiblio-2.1.3/physbiblio/parseAccents.py` & `physbiblio-2.1.4/physbiblio/parseAccents.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/pdf.py` & `physbiblio-2.1.4/physbiblio/pdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This module manages the saved PDF files and opens them if required.
 
 This file is part of the physbiblio package.
 """
+
 import os
 import os.path as osp
 import shutil
 import subprocess
 import traceback
 from urllib.request import HTTPError, URLError, urlopen
```

### Comparing `physbiblio-2.1.3/physbiblio/setuptests.py` & `physbiblio-2.1.4/physbiblio/setuptests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Utilities for in the tests of the physbiblio modules.
 
 This file is part of the physbiblio package.
 """
+
 import datetime
 import os
 import sys
 import traceback
 import unittest
 from io import StringIO
 from unittest.mock import patch
```

### Comparing `physbiblio-2.1.3/physbiblio/strings/common.py` & `physbiblio-2.1.4/physbiblio/strings/common.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/strings/gui.py` & `physbiblio-2.1.4/physbiblio/strings/gui.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/strings/main.py` & `physbiblio-2.1.4/physbiblio/strings/main.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/strings/webimport.py` & `physbiblio-2.1.4/physbiblio/strings/webimport.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/tablesDef.py` & `physbiblio-2.1.4/physbiblio/tablesDef.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Static definitions of the structure (column names and content)
 for the tables of the database.
 
 This file is part of the physbiblio package.
 """
+
 import traceback
 
 try:
     from physbiblio.strings.main import TablesDefStrings as tdstr
 except ImportError:
     print("Could not find physbiblio and its modules!")
     print(traceback.format_exc())
```

### Comparing `physbiblio-2.1.3/physbiblio/testLoader.py` & `physbiblio-2.1.4/physbiblio/testLoader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Adapting the code from setuptools.command.test:ScanningLoader,
 which is not finding tests in python3.
 
 This file is part of the physbiblio package.
 """
+
 from unittest import TestLoader
 
 from pkg_resources import resource_exists, resource_listdir
 
 
 class PBScanningLoader(TestLoader):
     """Custom ScanningLoader implementation to be used
```

### Comparing `physbiblio-2.1.3/physbiblio/tests/test_argParser.py` & `physbiblio-2.1.4/physbiblio/tests/test_argParser.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/tests/test_bibtexWriter.py` & `physbiblio-2.1.4/physbiblio/tests/test_bibtexWriter.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/tests/test_config.py` & `physbiblio-2.1.4/physbiblio/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/tests/test_database.py` & `physbiblio-2.1.4/physbiblio/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/tests/test_errors.py` & `physbiblio-2.1.4/physbiblio/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/tests/test_export.py` & `physbiblio-2.1.4/physbiblio/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/tests/test_inspireStats.py` & `physbiblio-2.1.4/physbiblio/tests/test_inspireStats.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/tests/test_package.py` & `physbiblio-2.1.4/physbiblio/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/tests/test_pdf.py` & `physbiblio-2.1.4/physbiblio/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/tests/test_view.py` & `physbiblio-2.1.4/physbiblio/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/view.py` & `physbiblio-2.1.4/physbiblio/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module that opens the external links.
 
 This file is part of the physbiblio package.
 """
+
 import subprocess
 import traceback
 
 try:
     from physbiblio.config import pbConfig
     from physbiblio.database import pBDB
     from physbiblio.errors import pBLogger
```

### Comparing `physbiblio-2.1.3/physbiblio/webimport/adsnasa.py` & `physbiblio-2.1.4/physbiblio/webimport/adsnasa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module that deals with importing info from the ADS API.
 
 This file is part of the physbiblio package.
 """
+
 import traceback
 
 import ads
 
 try:
     from physbiblio.config import pbConfig
     from physbiblio.errors import pBLogger
```

### Comparing `physbiblio-2.1.3/physbiblio/webimport/arxiv.py` & `physbiblio-2.1.4/physbiblio/webimport/arxiv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module that deals with importing info from the arXiv API.
 
 Uses feedparser module to read the page content.
 
 This file is part of the physbiblio package.
 """
+
 import re
 import traceback
 
 import feedparser
 
 try:
     from bibtexparser.bibdatabase import BibDatabase
```

### Comparing `physbiblio-2.1.3/physbiblio/webimport/doi.py` & `physbiblio-2.1.4/physbiblio/webimport/doi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module that deals with importing info from the DOI.org API.
 
 This file is part of the physbiblio package.
 """
+
 import traceback
 
 try:
     from physbiblio.config import pbConfig
     from physbiblio.errors import pBLogger
     from physbiblio.parseAccents import parse_accents_str
     from physbiblio.strings.webimport import DOIStrings
```

### Comparing `physbiblio-2.1.3/physbiblio/webimport/inspire.py` & `physbiblio-2.1.4/physbiblio/webimport/inspire.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module that deals with importing info from the INSPIRE-HEP API.
 
 This file is part of the physbiblio package.
 """
+
 import json
 import re
 import time
 import traceback
 
 import bibtexparser
 
@@ -649,34 +650,36 @@
                 tmpDict["year"] = pi["year"]
             except KeyError:
                 pass
             try:
                 tmpDict["pages"] = (
                     pi["artid"]
                     if "artid" in pi.keys()
-                    else "%s-%s" % (pi["page_start"], pi["page_end"])
-                    if ("page_start" in pi.keys() and "page_end" in pi.keys())
-                    else pi["page_start"]
-                    if "page_start" in pi.keys()
-                    else None
+                    else (
+                        "%s-%s" % (pi["page_start"], pi["page_end"])
+                        if ("page_start" in pi.keys() and "page_end" in pi.keys())
+                        else pi["page_start"] if "page_start" in pi.keys() else None
+                    )
                 )
             except KeyError:
                 tmpDict["pages"] = None
         except (IndexError, KeyError, TypeError):
             tmpDict["journal"] = None
             tmpDict["volume"] = None
             tmpDict["pages"] = None
         # dates
         try:
             tmpDict["firstdate"] = (
                 record["metadata"]["preprint_date"]
                 if "preprint_date" in record["metadata"].keys()
-                else record["metadata"]["legacy_creation_date"]
-                if "legacy_creation_date" in record["metadata"].keys()
-                else record["metadata"]["earliest_date"]
+                else (
+                    record["metadata"]["legacy_creation_date"]
+                    if "legacy_creation_date" in record["metadata"].keys()
+                    else record["metadata"]["earliest_date"]
+                )
             )
         except (KeyError, TypeError):
             tmpDict["firstdate"] = None
         try:
             tmpDict["pubdate"] = record["metadata"]["imprints"][0]["date"]
         except (IndexError, KeyError, TypeError):
             tmpDict["pubdate"] = None
```

### Comparing `physbiblio-2.1.3/physbiblio/webimport/tests/test_adsnasa.py` & `physbiblio-2.1.4/physbiblio/webimport/tests/test_adsnasa.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/webimport/tests/test_arxiv.py` & `physbiblio-2.1.4/physbiblio/webimport/tests/test_arxiv.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/webimport/tests/test_inspire.py` & `physbiblio-2.1.4/physbiblio/webimport/tests/test_inspire.py`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/physbiblio/webimport/tests/test_webimport.py` & `physbiblio-2.1.4/physbiblio/webimport/tests/test_webimport.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,27 +56,25 @@
                 + 'perspectives.}",\n         arxiv = "1507.08204",\n    '
                 + '   authors = "S. Gariazzo and C. Giunti and M. Laveder '
                 + 'and Y. F. Li and E. M. Zavanin",\n}',
             ],
             "doi": [
                 "10.1088/0954-3899/43/3/033001",
                 """@article{Gariazzo_2015,
-	doi = {10.1088/0954-3899/43/3/033001},
-	url = {"""
-                + pbConfig.doiUrl
-                + """10.1088%2F0954-3899%2F43%2F3%2F033001},
-	year = 2015,
-	month = {mar},
-	publisher = {{IOP} Publishing},
-	volume = {43},
-	number = {3},
-	pages = {033001},
-	author = {S Gariazzo and C Giunti and M Laveder and Y F Li and E M Zavanin},
-	title = {Light sterile neutrinos},
-	journal = {Journal of Physics G: Nuclear and Particle Physics}
+	doi={10.1088/0954-3899/43/3/033001},
+	url={http://dx.doi.org/10.1088/0954-3899/43/3/033001},
+	year={2015},
+	month=mar,
+	publisher={IOP Publishing},
+	volume={43},
+	number={3},
+	author={Gariazzo, S and Giunti, C and Laveder, M and Li, Y F and Zavanin, E M},
+	title={Light sterile neutrinos},
+	journal={Journal of Physics G: Nuclear and Particle Physics},
+	pages={033001}
 }""",
             ],
             "inspire": [
                 "Gariazzo:2015rra",
                 """@article{Gariazzo:2015rra,
     author = "Gariazzo, S. and Giunti, C. and Laveder, M. and Li, Y. F. and Zavanin, E. M.",
     title = "{Light sterile neutrinos}",
@@ -103,24 +101,29 @@
                 self.assertEqual(
                     physBiblioWeb.webSearch[method]
                     .retrieveUrlAll(strings[0], searchType="id")
                     .strip(),
                     strings[1].strip(),
                 )
             else:
-                self.assertEqual(
+                res1 = (
                     physBiblioWeb.webSearch[method]
                     .retrieveUrlFirst(strings[0])
-                    .strip(),
-                    strings[1].strip(),
+                    .strip()
+                    .lower()
                 )
-                self.assertEqual(
-                    physBiblioWeb.webSearch[method].retrieveUrlAll(strings[0]).strip(),
-                    strings[1].strip(),
+                res2 = (
+                    physBiblioWeb.webSearch[method]
+                    .retrieveUrlAll(strings[0])
+                    .strip()
+                    .lower()
                 )
+                for s in strings[1].strip().split("\n"):
+                    self.assertIn(s.strip().lower(), res1)
+                    self.assertIn(s.strip().lower(), res2)
 
     def test_methods_insuccess(self):
         """Test webimport using missing and/or invalid identifiers"""
         print(physBiblioWeb.webSearch.keys())
         self.maxDiff = None
         tests = {
             "arxiv": ["1801.15000", ""],
```

### Comparing `physbiblio-2.1.3/physbiblio/webimport/webInterf.py` & `physbiblio-2.1.4/physbiblio/webimport/webInterf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module that creates the base class WebInterf,
 which will be used by other modules in this package.
 
 Uses urllib to download url content.
 
 This file is part of the physbiblio package.
 """
+
 import os
 import pkgutil
 import socket
 import ssl
 import traceback
 from urllib.request import HTTPError, Request, URLError, urlopen
```

### Comparing `physbiblio-2.1.3/physbiblio.egg-info/PKG-INFO` & `physbiblio-2.1.4/physbiblio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physbiblio
-Version: 2.1.3
+Version: 2.1.4
 Summary: A bibliography manager in Python (using Sqlite and PySide6)
 Home-page: https://github.com/steog88/PhysBiblio
 Author: Stefano Gariazzo
 Author-email: stefano.gariazzo@gmail.com
 License: GPL-3.0
 Keywords: bibliography,hep-ph,high-energy-physics,bibtex
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,16 +18,35 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides: physbiblio
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: ads
+Requires-Dist: appdirs
+Requires-Dist: argparse
+Requires-Dist: bibtexparser>=1.1.0
+Requires-Dist: dictdiffer
+Requires-Dist: feedparser
+Requires-Dist: matplotlib>=3.6.2
+Requires-Dist: outdated
+Requires-Dist: pylatexenc>=2.0
+Requires-Dist: pyparsing>=2.4.0
+Requires-Dist: pyside6>=6.4.0
+Requires-Dist: pytz
+Requires-Dist: requests>=2.25
+Requires-Dist: urllib3>=1.26
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pyyaml; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 # [PhysBiblio](https://github.com/steog88/PhysBiblio)
 Bibliography manager in Python  
 by S. Gariazzo (stefano.gariazzo@gmail.com)
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/steog88/PhysBiblio/blob/master/LICENSE)
 [![PyPI version](https://img.shields.io/pypi/v/physbiblio.svg?style=flat-square)](https://pypi.org/project/physbiblio/)
```

### Comparing `physbiblio-2.1.3/physbiblio.egg-info/SOURCES.txt` & `physbiblio-2.1.4/physbiblio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `physbiblio-2.1.3/setup.py` & `physbiblio-2.1.4/setup.py`

 * *Files identical despite different names*

