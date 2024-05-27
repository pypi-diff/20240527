# Comparing `tmp/totolo-1.6.0.tar.gz` & `tmp/totolo-1.6.0.dev202405271003.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totolo-1.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "totolo-1.6.0.dev202405271003.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `totolo-1.6.0.tar` & `totolo-1.6.0.dev202405271003.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0      834 2024-05-27 10:02:31.119749 totolo-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2024-05-27 10:02:31.119749 totolo-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1096 2024-05-27 10:02:31.119749 totolo-1.6.0/.github/workflows/coverage-branch.yaml
--rw-r--r--   0        0        0     1106 2024-05-27 10:02:31.119749 totolo-1.6.0/.github/workflows/coverage.yaml
--rw-r--r--   0        0        0     5091 2024-05-27 10:02:31.119749 totolo-1.6.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      825 2024-05-27 10:02:31.119749 totolo-1.6.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0     3088 2024-05-27 10:02:31.119749 totolo-1.6.0/.gitignore
--rw-r--r--   0        0        0     1550 2024-05-27 10:02:31.119749 totolo-1.6.0/.vscode/launch.json
--rw-r--r--   0        0        0      277 2024-05-27 10:02:31.119749 totolo-1.6.0/.vscode/settings.json
--rw-r--r--   0        0        0     1071 2024-05-27 10:02:31.119749 totolo-1.6.0/LICENSE
--rw-r--r--   0        0        0     4126 2024-05-27 10:02:31.119749 totolo-1.6.0/README.md
--rw-r--r--   0        0        0     1104 2024-05-27 10:02:31.119749 totolo-1.6.0/examples/basics.py
--rw-r--r--   0        0        0     1663 2024-05-27 10:02:31.119749 totolo-1.6.0/pyproject.toml
--rw-r--r--   0        0        0       60 2024-05-27 10:02:31.119749 totolo-1.6.0/requirements-dev.txt
--rw-r--r--   0        0        0        0 2024-05-27 10:02:31.119749 totolo-1.6.0/tests/__init__.py
--rw-r--r--   0        0        0       24 2024-05-27 10:02:31.119749 totolo-1.6.0/tests/data/cycles1.th.txt
--rw-r--r--   0        0        0       47 2024-05-27 10:02:31.119749 totolo-1.6.0/tests/data/cycles2.th.txt
--rw-r--r--   0        0        0       71 2024-05-27 10:02:31.119749 totolo-1.6.0/tests/data/cycles3.th.txt
--rw-r--r--   0        0        0   173716 2024-05-27 10:02:31.119749 totolo-1.6.0/tests/data/film-timeout-top100.st.txt
--rw-r--r--   0        0        0   332534 2024-05-27 10:02:31.119749 totolo-1.6.0/tests/data/flat.tar.gz
--rw-r--r--   0        0        0      166 2024-05-27 10:02:31.119749 totolo-1.6.0/tests/data/messy.st.txt
--rw-r--r--   0        0        0   332557 2024-05-27 10:02:31.119749 totolo-1.6.0/tests/data/sample-2023.07.23.tar.gz
--rw-r--r--   0        0        0    34632 2024-05-27 10:02:31.123749 totolo-1.6.0/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt
--rw-r--r--   0        0        0    28133 2024-05-27 10:02:31.123749 totolo-1.6.0/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt
--rw-r--r--   0        0        0    48760 2024-05-27 10:02:31.123749 totolo-1.6.0/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt
--rw-r--r--   0        0        0  1011578 2024-05-27 10:02:31.127749 totolo-1.6.0/tests/data/sample-2023.07.23/notes/themes/primary.th.txt
--rw-r--r--   0        0        0    14882 2024-05-27 10:02:31.127749 totolo-1.6.0/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt
--rwxr-xr-x   0        0        0    10486 2024-05-27 10:02:31.127749 totolo-1.6.0/tests/data/scifi1920-mergelist.xlsx
--rw-r--r--   0        0        0      428 2024-05-27 10:02:31.127749 totolo-1.6.0/tests/data/storytree.st.txt
--rw-r--r--   0        0        0  1011579 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/data/to-2023.07.09.th.txt
--rw-r--r--   0        0        0     2365 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/data/to-sample-2023.07.09-copy.st.txt
--rw-r--r--   0        0        0     2365 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/data/to-sample-2023.07.09.st.txt
--rw-r--r--   0        0        0        0 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/lib/__init__.py
--rw-r--r--   0        0        0      745 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/lib/test_excel.py
--rw-r--r--   0        0        0      800 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/lib/test_files.py
--rw-r--r--   0        0        0      794 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/lib/test_logging.py
--rw-r--r--   0        0        0     1419 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/lib/test_textformat.py
--rw-r--r--   0        0        0     6568 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/test_entries.py
--rw-r--r--   0        0        0     6158 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/test_impl.py
--rw-r--r--   0        0        0     1909 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/test_toset.py
--rw-r--r--   0        0        0    15548 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/test_totolo.py
--rw-r--r--   0        0        0        0 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1968 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/utils/test_mergefiles.py
--rw-r--r--   0        0        0     3191 2024-05-27 10:02:31.131749 totolo-1.6.0/tests/utils/test_mergelist.py
--rw-r--r--   0        0        0      191 2024-05-27 10:02:31.131749 totolo-1.6.0/totolo/__init__.py
--rw-r--r--   0        0        0     1201 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/api.py
--rw-r--r--   0        0        0     1893 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/collection.py
--rw-r--r--   0        0        0        0 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/impl/__init__.py
--rw-r--r--   0        0        0     3367 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/impl/core.py
--rw-r--r--   0        0        0     6631 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/impl/entry.py
--rw-r--r--   0        0        0     4595 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/impl/field.py
--rw-r--r--   0        0        0      666 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/impl/keyword.py
--rw-r--r--   0        0        0     8062 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/impl/parser.py
--rw-r--r--   0        0        0        0 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/lib/__init__.py
--rw-r--r--   0        0        0     1690 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/lib/excel.py
--rw-r--r--   0        0        0     1134 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/lib/files.py
--rw-r--r--   0        0        0      248 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/lib/log.py
--rw-r--r--   0        0        0     1283 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/lib/textformat.py
--rw-r--r--   0        0        0     3733 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/story.py
--rw-r--r--   0        0        0     2442 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/theme.py
--rw-r--r--   0        0        0    11997 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/themeontology.py
--rw-r--r--   0        0        0        0 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/util/__init__.py
--rw-r--r--   0        0        0     2303 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/util/mergefiles.py
--rw-r--r--   0        0        0     7321 2024-05-27 10:02:31.135749 totolo-1.6.0/totolo/util/mergelist.py
--rw-r--r--   0        0        0     4560 1970-01-01 00:00:00.000000 totolo-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      834 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1096 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/.github/workflows/coverage-branch.yaml
+-rw-r--r--   0        0        0     1106 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/.github/workflows/coverage.yaml
+-rw-r--r--   0        0        0     5091 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      825 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     3088 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/.gitignore
+-rw-r--r--   0        0        0     1550 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/.vscode/launch.json
+-rw-r--r--   0        0        0      277 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/.vscode/settings.json
+-rw-r--r--   0        0        0     1071 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/LICENSE
+-rw-r--r--   0        0        0     4126 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/README.md
+-rw-r--r--   0        0        0     1104 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/examples/basics.py
+-rw-r--r--   0        0        0     1663 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/pyproject.toml
+-rw-r--r--   0        0        0       60 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/tests/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/tests/data/cycles1.th.txt
+-rw-r--r--   0        0        0       47 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/tests/data/cycles2.th.txt
+-rw-r--r--   0        0        0       71 2024-05-27 10:02:32.166142 totolo-1.6.0.dev202405271003/tests/data/cycles3.th.txt
+-rw-r--r--   0        0        0   173716 2024-05-27 10:02:32.170142 totolo-1.6.0.dev202405271003/tests/data/film-timeout-top100.st.txt
+-rw-r--r--   0        0        0   332534 2024-05-27 10:02:32.170142 totolo-1.6.0.dev202405271003/tests/data/flat.tar.gz
+-rw-r--r--   0        0        0      166 2024-05-27 10:02:32.170142 totolo-1.6.0.dev202405271003/tests/data/messy.st.txt
+-rw-r--r--   0        0        0   332557 2024-05-27 10:02:32.170142 totolo-1.6.0.dev202405271003/tests/data/sample-2023.07.23.tar.gz
+-rw-r--r--   0        0        0    34632 2024-05-27 10:02:32.170142 totolo-1.6.0.dev202405271003/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt
+-rw-r--r--   0        0        0    28133 2024-05-27 10:02:32.170142 totolo-1.6.0.dev202405271003/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt
+-rw-r--r--   0        0        0    48760 2024-05-27 10:02:32.170142 totolo-1.6.0.dev202405271003/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt
+-rw-r--r--   0        0        0  1011578 2024-05-27 10:02:32.174142 totolo-1.6.0.dev202405271003/tests/data/sample-2023.07.23/notes/themes/primary.th.txt
+-rw-r--r--   0        0        0    14882 2024-05-27 10:02:32.178142 totolo-1.6.0.dev202405271003/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt
+-rwxr-xr-x   0        0        0    10486 2024-05-27 10:02:32.178142 totolo-1.6.0.dev202405271003/tests/data/scifi1920-mergelist.xlsx
+-rw-r--r--   0        0        0      428 2024-05-27 10:02:32.178142 totolo-1.6.0.dev202405271003/tests/data/storytree.st.txt
+-rw-r--r--   0        0        0  1011579 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/data/to-2023.07.09.th.txt
+-rw-r--r--   0        0        0     2365 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/data/to-sample-2023.07.09-copy.st.txt
+-rw-r--r--   0        0        0     2365 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/data/to-sample-2023.07.09.st.txt
+-rw-r--r--   0        0        0        0 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/lib/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/lib/test_excel.py
+-rw-r--r--   0        0        0      800 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/lib/test_files.py
+-rw-r--r--   0        0        0      794 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/lib/test_logging.py
+-rw-r--r--   0        0        0     1419 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/lib/test_textformat.py
+-rw-r--r--   0        0        0     6568 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/test_entries.py
+-rw-r--r--   0        0        0     6158 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/test_impl.py
+-rw-r--r--   0        0        0     1909 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/test_toset.py
+-rw-r--r--   0        0        0    15548 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/test_totolo.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1968 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/utils/test_mergefiles.py
+-rw-r--r--   0        0        0     3191 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/tests/utils/test_mergelist.py
+-rw-r--r--   0        0        0      207 2024-05-27 10:03:41.863281 totolo-1.6.0.dev202405271003/totolo/__init__.py
+-rw-r--r--   0        0        0     1201 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/api.py
+-rw-r--r--   0        0        0     1893 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/collection.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/impl/__init__.py
+-rw-r--r--   0        0        0     3367 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/impl/core.py
+-rw-r--r--   0        0        0     6631 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/impl/entry.py
+-rw-r--r--   0        0        0     4595 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/impl/field.py
+-rw-r--r--   0        0        0      666 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/impl/keyword.py
+-rw-r--r--   0        0        0     8062 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/impl/parser.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/lib/__init__.py
+-rw-r--r--   0        0        0     1690 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/lib/excel.py
+-rw-r--r--   0        0        0     1134 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/lib/files.py
+-rw-r--r--   0        0        0      248 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/lib/log.py
+-rw-r--r--   0        0        0     1283 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/lib/textformat.py
+-rw-r--r--   0        0        0     3733 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/story.py
+-rw-r--r--   0        0        0     2442 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/theme.py
+-rw-r--r--   0        0        0    11997 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/themeontology.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/util/__init__.py
+-rw-r--r--   0        0        0     2303 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/util/mergefiles.py
+-rw-r--r--   0        0        0     7321 2024-05-27 10:02:32.182142 totolo-1.6.0.dev202405271003/totolo/util/mergelist.py
+-rw-r--r--   0        0        0     4576 1970-01-01 00:00:00.000000 totolo-1.6.0.dev202405271003/PKG-INFO
```

### Comparing `totolo-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `totolo-1.6.0.dev202405271003/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `totolo-1.6.0.dev202405271003/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/.github/workflows/coverage-branch.yaml` & `totolo-1.6.0.dev202405271003/.github/workflows/coverage-branch.yaml`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/.github/workflows/coverage.yaml` & `totolo-1.6.0.dev202405271003/.github/workflows/coverage.yaml`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/.github/workflows/publish.yaml` & `totolo-1.6.0.dev202405271003/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/.github/workflows/test.yaml` & `totolo-1.6.0.dev202405271003/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/.gitignore` & `totolo-1.6.0.dev202405271003/.gitignore`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/.vscode/launch.json` & `totolo-1.6.0.dev202405271003/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/LICENSE` & `totolo-1.6.0.dev202405271003/LICENSE`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/README.md` & `totolo-1.6.0.dev202405271003/README.md`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/examples/basics.py` & `totolo-1.6.0.dev202405271003/examples/basics.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/pyproject.toml` & `totolo-1.6.0.dev202405271003/pyproject.toml`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/data/film-timeout-top100.st.txt` & `totolo-1.6.0.dev202405271003/tests/data/film-timeout-top100.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/data/flat.tar.gz` & `totolo-1.6.0.dev202405271003/tests/data/flat.tar.gz`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/data/sample-2023.07.23.tar.gz` & `totolo-1.6.0.dev202405271003/tests/data/sample-2023.07.23.tar.gz`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt` & `totolo-1.6.0.dev202405271003/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt` & `totolo-1.6.0.dev202405271003/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt` & `totolo-1.6.0.dev202405271003/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/data/sample-2023.07.23/notes/themes/primary.th.txt` & `totolo-1.6.0.dev202405271003/tests/data/sample-2023.07.23/notes/themes/primary.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt` & `totolo-1.6.0.dev202405271003/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/data/scifi1920-mergelist.xlsx` & `totolo-1.6.0.dev202405271003/tests/data/scifi1920-mergelist.xlsx`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/data/to-2023.07.09.th.txt` & `totolo-1.6.0.dev202405271003/tests/data/to-2023.07.09.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/data/to-sample-2023.07.09-copy.st.txt` & `totolo-1.6.0.dev202405271003/tests/data/to-sample-2023.07.09-copy.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/data/to-sample-2023.07.09.st.txt` & `totolo-1.6.0.dev202405271003/tests/data/to-sample-2023.07.09.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/lib/test_excel.py` & `totolo-1.6.0.dev202405271003/tests/lib/test_excel.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/lib/test_files.py` & `totolo-1.6.0.dev202405271003/tests/lib/test_files.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/lib/test_logging.py` & `totolo-1.6.0.dev202405271003/tests/lib/test_logging.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/lib/test_textformat.py` & `totolo-1.6.0.dev202405271003/tests/lib/test_textformat.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/test_entries.py` & `totolo-1.6.0.dev202405271003/tests/test_entries.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/test_impl.py` & `totolo-1.6.0.dev202405271003/tests/test_impl.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/test_toset.py` & `totolo-1.6.0.dev202405271003/tests/test_toset.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/test_totolo.py` & `totolo-1.6.0.dev202405271003/tests/test_totolo.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/utils/test_mergefiles.py` & `totolo-1.6.0.dev202405271003/tests/utils/test_mergefiles.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/tests/utils/test_mergelist.py` & `totolo-1.6.0.dev202405271003/tests/utils/test_mergelist.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/api.py` & `totolo-1.6.0.dev202405271003/totolo/api.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/collection.py` & `totolo-1.6.0.dev202405271003/totolo/collection.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/impl/core.py` & `totolo-1.6.0.dev202405271003/totolo/impl/core.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/impl/entry.py` & `totolo-1.6.0.dev202405271003/totolo/impl/entry.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/impl/field.py` & `totolo-1.6.0.dev202405271003/totolo/impl/field.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/impl/keyword.py` & `totolo-1.6.0.dev202405271003/totolo/impl/keyword.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/impl/parser.py` & `totolo-1.6.0.dev202405271003/totolo/impl/parser.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/lib/excel.py` & `totolo-1.6.0.dev202405271003/totolo/lib/excel.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/lib/files.py` & `totolo-1.6.0.dev202405271003/totolo/lib/files.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/lib/textformat.py` & `totolo-1.6.0.dev202405271003/totolo/lib/textformat.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/story.py` & `totolo-1.6.0.dev202405271003/totolo/story.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/theme.py` & `totolo-1.6.0.dev202405271003/totolo/theme.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/themeontology.py` & `totolo-1.6.0.dev202405271003/totolo/themeontology.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/util/mergefiles.py` & `totolo-1.6.0.dev202405271003/totolo/util/mergefiles.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/totolo/util/mergelist.py` & `totolo-1.6.0.dev202405271003/totolo/util/mergelist.py`

 * *Files identical despite different names*

### Comparing `totolo-1.6.0/PKG-INFO` & `totolo-1.6.0.dev202405271003/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totolo
-Version: 1.6.0
+Version: 1.6.0.dev202405271003
 Summary: The Python interface to themeontology.org.
 Author-email: Mikael Onsjö <mikael@odinlake.net>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Documentation, https://github.com/theme-ontology/theming
 Project-URL: Home, https://www.themeontology.org/
 Project-URL: Source, https://github.com/theme-ontology/python-totolo
```

