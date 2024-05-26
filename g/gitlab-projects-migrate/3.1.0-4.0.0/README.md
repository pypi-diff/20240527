# Comparing `tmp/gitlab_projects_migrate-3.1.0.tar.gz` & `tmp/gitlab_projects_migrate-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_migrate-3.1.0.tar", last modified: Fri May 17 02:44:47 2024, max compression
+gzip compressed data, was "gitlab_projects_migrate-4.0.0.tar", last modified: Sun May 26 22:45:52 2024, max compression
```

## Comparing `gitlab_projects_migrate-3.1.0.tar` & `gitlab_projects_migrate-4.0.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.018808 gitlab_projects_migrate-3.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.008808 gitlab_projects_migrate-3.1.0/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      702 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    11965 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.009808 gitlab_projects_migrate-3.1.0/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     4720 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7248 2024-05-17 02:44:47.018808 gitlab_projects_migrate-3.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5565 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.017808 gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7248 2024-05-17 02:44:46.000000 gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1068 2024-05-17 02:44:47.000000 gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 02:44:46.000000 gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2024-05-17 02:44:46.000000 gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2024-05-17 02:44:46.000000 gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-17 02:44:46.000000 gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.011808 gitlab_projects_migrate-3.1.0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 02:44:47.018808 gitlab_projects_migrate-3.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2875 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.011808 gitlab_projects_migrate-3.1.0/src/
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.012808 gitlab_projects_migrate-3.1.0/src/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29592 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/cli/entrypoint.py
--rwxrwxrwx   0 root         (0) root         (0)     8605 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.013808 gitlab_projects_migrate-3.1.0/src/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12565 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/features/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.014808 gitlab_projects_migrate-3.1.0/src/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     3810 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/package/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     6845 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/package/updates.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.015808 gitlab_projects_migrate-3.1.0/src/prints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/prints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2549 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/prints/boxes.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/prints/colors.py
--rw-rw-rw-   0 root         (0) root         (0)     1565 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/prints/themes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.016808 gitlab_projects_migrate-3.1.0/src/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1788 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/system/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:47.017808 gitlab_projects_migrate-3.1.0/src/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/types/namespaces.py
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/types/paths.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2024-05-17 02:44:43.000000 gitlab_projects_migrate-3.1.0/src/types/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:45:52.065030 gitlab_projects_migrate-4.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:45:52.056030 gitlab_projects_migrate-4.0.0/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      702 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    11965 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:45:52.057031 gitlab_projects_migrate-4.0.0/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     5363 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7788 2024-05-26 22:45:52.065030 gitlab_projects_migrate-4.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6105 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:45:52.064031 gitlab_projects_migrate-4.0.0/gitlab_projects_migrate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7788 2024-05-26 22:45:52.000000 gitlab_projects_migrate-4.0.0/gitlab_projects_migrate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-05-26 22:45:52.000000 gitlab_projects_migrate-4.0.0/gitlab_projects_migrate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-26 22:45:52.000000 gitlab_projects_migrate-4.0.0/gitlab_projects_migrate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2024-05-26 22:45:52.000000 gitlab_projects_migrate-4.0.0/gitlab_projects_migrate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2024-05-26 22:45:52.000000 gitlab_projects_migrate-4.0.0/gitlab_projects_migrate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-26 22:45:52.000000 gitlab_projects_migrate-4.0.0/gitlab_projects_migrate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:45:52.059030 gitlab_projects_migrate-4.0.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-26 22:45:52.065030 gitlab_projects_migrate-4.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2875 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:45:52.059030 gitlab_projects_migrate-4.0.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:45:52.060030 gitlab_projects_migrate-4.0.0/src/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    33390 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/cli/entrypoint.py
+-rwxrwxrwx   0 root         (0) root         (0)     9112 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:45:52.061030 gitlab_projects_migrate-4.0.0/src/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14236 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/features/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:45:52.062030 gitlab_projects_migrate-4.0.0/src/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/package/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     6845 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/package/updates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:45:52.063030 gitlab_projects_migrate-4.0.0/src/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/prints/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/prints/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/prints/themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:45:52.063030 gitlab_projects_migrate-4.0.0/src/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:45:52.064031 gitlab_projects_migrate-4.0.0/src/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/types/namespaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/types/paths.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2024-05-26 22:45:48.000000 gitlab_projects_migrate-4.0.0/src/types/strings.py
```

### Comparing `gitlab_projects_migrate-3.1.0/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_migrate-4.0.0/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/.chglog/changelog.sh` & `gitlab_projects_migrate-4.0.0/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/.chglog/config.yml` & `gitlab_projects_migrate-4.0.0/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/.gitlab-ci.yml` & `gitlab_projects_migrate-4.0.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/.style.yapf` & `gitlab_projects_migrate-4.0.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/.vscode/extensions.json` & `gitlab_projects_migrate-4.0.0/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/.vscode/settings.json` & `gitlab_projects_migrate-4.0.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/CHANGELOG.md` & `gitlab_projects_migrate-4.0.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,31 @@
 
+<a name="4.0.0"></a>
+## [4.0.0](https://gitlab.com/AdrianDC/gitlab-projects-migrate/compare/3.1.0...4.0.0) (2024-05-27)
+
+### Bug Fixes
+
+* **gitlab:** fix project import 'path_with_namespace' in dry run
+* **main:** exclusive '--archive-sources' and '--delete-sources'
+
+### Cleanups
+
+* **entrypoint:** turn 'confirm' function into generic handler
+
+### Documentation
+
+* **readme:** add '--archive-sources' and '--delete-sources' examples
+
+### Features
+
+* **entrypoint:** identify already existing project, group, subgroup
+* **entrypoint:** improve outputs logs upon delections
+* **main:** show newer updates message upon incompatible arguments
+
+
 <a name="3.1.0"></a>
 ## [3.1.0](https://gitlab.com/AdrianDC/gitlab-projects-migrate/compare/3.0.1...3.1.0) (2024-05-17)
 
 ### Bug Fixes
 
 * **gitlab:** restore 'import_project' file argument as BufferedReader
 * **gitlab:** raise runtime error upon failed project imports
```

### Comparing `gitlab_projects_migrate-3.1.0/LICENSE` & `gitlab_projects_migrate-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/PKG-INFO` & `gitlab_projects_migrate-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-migrate
-Version: 3.1.0
+Version: 4.0.0
 Summary: Migrate GitLab projects from a GitLab group to another GitLab's group
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-migrate
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-migrate/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-migrate/blob/main/CHANGELOG.md
@@ -64,14 +64,18 @@
 gitlab-projects-migrate
 
 # Migrate projects from one group to another, then migrate subgroups
 gitlab-projects-migrate 'https://gitlab.com' 'old/group' 'https://gitlab.com' 'new/group'
 gitlab-projects-migrate 'https://gitlab.com' 'old/group/subgroup1' 'https://gitlab.com' 'new/group/subgroup1'
 gitlab-projects-migrate 'https://gitlab.com' 'old/group/subgroup2' 'https://gitlab.com' 'new/group/subgroup2'
 
+# Migrate projects from one group to another, then archive or delete sources
+gitlab-projects-migrate --archive-sources 'https://gitlab.com' 'old_group_1' 'https://gitlab.com' 'new_group_1'
+gitlab-projects-migrate --delete-sources 'https://gitlab.com' 'old_group_2' 'https://gitlab.com' 'new_group_2'
+
 # Migrate projects from one GitLab to another GitLab
 gitlab-projects-migrate 'https://old.gitlab.com' 'group/subgroup' 'https://new.gitlab.com'
 ```
 
 <!-- prettier-ignore-end -->
 
 ---
@@ -79,17 +83,18 @@
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
 usage: gitlab-projects-migrate [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-I INPUT_TOKEN]
-                               [-O OUTPUT_TOKEN] [--archive-exports FOLDER] [--delete-sources] [--dry-run]
-                               [--exclude-group] [--exclude-subgroups] [--exclude-projects] [--keep-members]
-                               [--overwrite] [--set-avatar FILE] [--update-description] [--]
+                               [-O OUTPUT_TOKEN] [--archive-exports FOLDER] [--archive-sources | --delete-sources]
+                               [--dry-run] [--exclude-group] [--exclude-subgroups] [--exclude-projects]
+                               [--keep-members] [--overwrite] [--rename-project NAME] [--set-avatar FILE]
+                               [--update-description] [--]
                                [input_gitlab] [input_path] [output_gitlab] [output_namespace]
 
 gitlab-projects-migrate: Migrate GitLab projects from a GitLab group to another GitLab's group
 
 internal arguments:
   -h, --help                # Show this help message
   --version                 # Show the current version
@@ -100,21 +105,23 @@
 
 credentials arguments:
   -I INPUT_TOKEN            # Input GitLab API token (default: GITLAB_INPUT_TOKEN or GITLAB_TOKEN environments)
   -O OUTPUT_TOKEN           # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN, GITLAB_TOKEN environments, or INPUT_TOKEN argument)
 
 migration arguments:
   --archive-exports FOLDER  # Store exported projects and groups to a folder
+  --archive-sources         # Archive sources after successful migration
   --delete-sources          # Delete sources after successful migration
   --dry-run                 # Enable dry run mode to check without saving
   --exclude-group           # Exclude parent group migration
   --exclude-subgroups       # Exclude children subgroups migration
   --exclude-projects        # Exclude children projects migration
   --keep-members            # Keep input members after importing on output GitLab
   --overwrite               # Overwrite existing projects on output GitLab
+  --rename-project NAME     # Rename GitLab output project (only for single input project)
 
 general settings arguments:
   --set-avatar FILE         # Set avatar of GitLab output projects and groups
   --update-description      # Update description of GitLab output projects and groups automatically
 
 positional arguments:
   --                        # Positional arguments separator (recommended)
```

### Comparing `gitlab_projects_migrate-3.1.0/README.md` & `gitlab_projects_migrate-4.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 gitlab-projects-migrate
 
 # Migrate projects from one group to another, then migrate subgroups
 gitlab-projects-migrate 'https://gitlab.com' 'old/group' 'https://gitlab.com' 'new/group'
 gitlab-projects-migrate 'https://gitlab.com' 'old/group/subgroup1' 'https://gitlab.com' 'new/group/subgroup1'
 gitlab-projects-migrate 'https://gitlab.com' 'old/group/subgroup2' 'https://gitlab.com' 'new/group/subgroup2'
 
+# Migrate projects from one group to another, then archive or delete sources
+gitlab-projects-migrate --archive-sources 'https://gitlab.com' 'old_group_1' 'https://gitlab.com' 'new_group_1'
+gitlab-projects-migrate --delete-sources 'https://gitlab.com' 'old_group_2' 'https://gitlab.com' 'new_group_2'
+
 # Migrate projects from one GitLab to another GitLab
 gitlab-projects-migrate 'https://old.gitlab.com' 'group/subgroup' 'https://new.gitlab.com'
 ```
 
 <!-- prettier-ignore-end -->
 
 ---
@@ -43,17 +47,18 @@
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
 usage: gitlab-projects-migrate [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-I INPUT_TOKEN]
-                               [-O OUTPUT_TOKEN] [--archive-exports FOLDER] [--delete-sources] [--dry-run]
-                               [--exclude-group] [--exclude-subgroups] [--exclude-projects] [--keep-members]
-                               [--overwrite] [--set-avatar FILE] [--update-description] [--]
+                               [-O OUTPUT_TOKEN] [--archive-exports FOLDER] [--archive-sources | --delete-sources]
+                               [--dry-run] [--exclude-group] [--exclude-subgroups] [--exclude-projects]
+                               [--keep-members] [--overwrite] [--rename-project NAME] [--set-avatar FILE]
+                               [--update-description] [--]
                                [input_gitlab] [input_path] [output_gitlab] [output_namespace]
 
 gitlab-projects-migrate: Migrate GitLab projects from a GitLab group to another GitLab's group
 
 internal arguments:
   -h, --help                # Show this help message
   --version                 # Show the current version
@@ -64,21 +69,23 @@
 
 credentials arguments:
   -I INPUT_TOKEN            # Input GitLab API token (default: GITLAB_INPUT_TOKEN or GITLAB_TOKEN environments)
   -O OUTPUT_TOKEN           # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN, GITLAB_TOKEN environments, or INPUT_TOKEN argument)
 
 migration arguments:
   --archive-exports FOLDER  # Store exported projects and groups to a folder
+  --archive-sources         # Archive sources after successful migration
   --delete-sources          # Delete sources after successful migration
   --dry-run                 # Enable dry run mode to check without saving
   --exclude-group           # Exclude parent group migration
   --exclude-subgroups       # Exclude children subgroups migration
   --exclude-projects        # Exclude children projects migration
   --keep-members            # Keep input members after importing on output GitLab
   --overwrite               # Overwrite existing projects on output GitLab
+  --rename-project NAME     # Rename GitLab output project (only for single input project)
 
 general settings arguments:
   --set-avatar FILE         # Set avatar of GitLab output projects and groups
   --update-description      # Update description of GitLab output projects and groups automatically
 
 positional arguments:
   --                        # Positional arguments separator (recommended)
```

### Comparing `gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/PKG-INFO` & `gitlab_projects_migrate-4.0.0/gitlab_projects_migrate.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-migrate
-Version: 3.1.0
+Version: 4.0.0
 Summary: Migrate GitLab projects from a GitLab group to another GitLab's group
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-migrate
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-migrate/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-migrate/blob/main/CHANGELOG.md
@@ -64,14 +64,18 @@
 gitlab-projects-migrate
 
 # Migrate projects from one group to another, then migrate subgroups
 gitlab-projects-migrate 'https://gitlab.com' 'old/group' 'https://gitlab.com' 'new/group'
 gitlab-projects-migrate 'https://gitlab.com' 'old/group/subgroup1' 'https://gitlab.com' 'new/group/subgroup1'
 gitlab-projects-migrate 'https://gitlab.com' 'old/group/subgroup2' 'https://gitlab.com' 'new/group/subgroup2'
 
+# Migrate projects from one group to another, then archive or delete sources
+gitlab-projects-migrate --archive-sources 'https://gitlab.com' 'old_group_1' 'https://gitlab.com' 'new_group_1'
+gitlab-projects-migrate --delete-sources 'https://gitlab.com' 'old_group_2' 'https://gitlab.com' 'new_group_2'
+
 # Migrate projects from one GitLab to another GitLab
 gitlab-projects-migrate 'https://old.gitlab.com' 'group/subgroup' 'https://new.gitlab.com'
 ```
 
 <!-- prettier-ignore-end -->
 
 ---
@@ -79,17 +83,18 @@
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
 usage: gitlab-projects-migrate [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-I INPUT_TOKEN]
-                               [-O OUTPUT_TOKEN] [--archive-exports FOLDER] [--delete-sources] [--dry-run]
-                               [--exclude-group] [--exclude-subgroups] [--exclude-projects] [--keep-members]
-                               [--overwrite] [--set-avatar FILE] [--update-description] [--]
+                               [-O OUTPUT_TOKEN] [--archive-exports FOLDER] [--archive-sources | --delete-sources]
+                               [--dry-run] [--exclude-group] [--exclude-subgroups] [--exclude-projects]
+                               [--keep-members] [--overwrite] [--rename-project NAME] [--set-avatar FILE]
+                               [--update-description] [--]
                                [input_gitlab] [input_path] [output_gitlab] [output_namespace]
 
 gitlab-projects-migrate: Migrate GitLab projects from a GitLab group to another GitLab's group
 
 internal arguments:
   -h, --help                # Show this help message
   --version                 # Show the current version
@@ -100,21 +105,23 @@
 
 credentials arguments:
   -I INPUT_TOKEN            # Input GitLab API token (default: GITLAB_INPUT_TOKEN or GITLAB_TOKEN environments)
   -O OUTPUT_TOKEN           # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN, GITLAB_TOKEN environments, or INPUT_TOKEN argument)
 
 migration arguments:
   --archive-exports FOLDER  # Store exported projects and groups to a folder
+  --archive-sources         # Archive sources after successful migration
   --delete-sources          # Delete sources after successful migration
   --dry-run                 # Enable dry run mode to check without saving
   --exclude-group           # Exclude parent group migration
   --exclude-subgroups       # Exclude children subgroups migration
   --exclude-projects        # Exclude children projects migration
   --keep-members            # Keep input members after importing on output GitLab
   --overwrite               # Overwrite existing projects on output GitLab
+  --rename-project NAME     # Rename GitLab output project (only for single input project)
 
 general settings arguments:
   --set-avatar FILE         # Set avatar of GitLab output projects and groups
   --update-description      # Update description of GitLab output projects and groups automatically
 
 positional arguments:
   --                        # Positional arguments separator (recommended)
```

### Comparing `gitlab_projects_migrate-3.1.0/gitlab_projects_migrate.egg-info/SOURCES.txt` & `gitlab_projects_migrate-4.0.0/gitlab_projects_migrate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/setup.py` & `gitlab_projects_migrate-4.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/src/cli/entrypoint.py` & `gitlab_projects_migrate-4.0.0/src/cli/entrypoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 # Standard libraries
 from argparse import Namespace
 from enum import Enum
+import re
 from tempfile import NamedTemporaryFile
 from typing import Optional
 
 # Modules libraries
 from gitlab.exceptions import GitlabGetError
 from gitlab.v4.objects import (
     Group as GitLabGroup,
@@ -22,22 +23,22 @@
 from ..package.bundle import Bundle
 from ..prints.colors import Colors
 from ..prints.themes import Themes
 from ..system.platform import Platform
 from ..types.namespaces import Namespaces
 from ..types.paths import Paths
 
-# Entrypoint class, pylint: disable=too-few-public-methods,too-many-statements
+# Entrypoint class, pylint: disable=too-few-public-methods,too-many-nested-blocks,too-many-statements
 class Entrypoint:
 
     # Constants
     EXPORTS_PREFIX: str = f'{Bundle.NAME}-exports-'
 
     # Enumerations
-    Result = Enum('Result', ['SUCCESS', 'FINALIZE', 'ERROR'])
+    Result = Enum('Result', ['SUCCESS', 'FINALIZE', 'ERROR', 'CRITICAL'])
 
     # CLI, pylint: disable=too-many-branches
     @staticmethod
     def cli(options: Namespace) -> Result:
 
         # Variables
         input_group: Optional[GitLabGroup] = None
@@ -136,50 +137,74 @@
                 print(f'{Colors.BOLD} - GitLab output group: '
                       f'{Colors.GREEN}{options.output_namespace}'
                       f'{Colors.RED} (Non-existent output group)'
                       f'{Colors.RESET}')
                 print(' ')
                 Platform.flush()
 
+        # Validate options
+        if options.rename_project and not input_project:
+            raise RuntimeError(
+                'Renaming project is only allowed with a single input project')
+
         # Handle single project
         if input_project:
 
             # Validate types
             assert output_namespace
 
             # Handle project
             Entrypoint.project(
                 options,
                 input_gitlab,
                 output_gitlab,
                 input_project.path_with_namespace,
                 input_project.namespace['id'],
                 output_namespace.full_path,
+                options.rename_project,
             )
 
-            # Delete input project after validation
-            if options.delete_sources:
+            # Handle sources
+            if options.archive_sources or options.delete_sources:
                 print(f'{Colors.BOLD} - GitLab input project: '
                       f'{Colors.GREEN}{input_project.path_with_namespace}'
                       f'{Colors.CYAN} ({Namespaces.text(input_project.description)})'
                       f'{Colors.RESET}')
                 Platform.flush()
-                if not Entrypoint.confirm(
-                        'project',
+
+                # Archive input project
+                if options.archive_sources:
+                    input_gitlab.project_set_archive(
                         input_project.path_with_namespace,
-                ):
-                    raise PermissionError()
+                        enabled=True,
+                    )
+                    print(f'{Colors.BOLD}   - Archive sources project: '
+                          f'{Colors.GREEN}Success'
+                          f'{Colors.RESET}')
+                    print(' ')
+                    Platform.flush()
 
                 # Delete input project
-                input_gitlab.project_delete(input_project.path_with_namespace)
-                print(f'{Colors.BOLD}   - Delete sources project: '
-                      f'{Colors.GREEN}Success'
-                      f'{Colors.RESET}')
-                print(' ')
-                Platform.flush()
+                elif options.delete_sources:
+
+                    # Confirm project deletion
+                    if not Entrypoint.confirm(
+                            'Delete project',
+                            input_project.path_with_namespace,
+                            'deletion',
+                    ):
+                        raise PermissionError()
+
+                    # Delete input project
+                    input_gitlab.project_delete(input_project.path_with_namespace)
+                    print(f'{Colors.BOLD}   - Delete sources project: '
+                          f'{Colors.GREEN}Success'
+                          f'{Colors.RESET}')
+                    print(' ')
+                    Platform.flush()
 
         # Handle group recursively
         elif input_group:
 
             # Handle group if missing
             if not options.exclude_group:
                 result = Entrypoint.group(
@@ -251,16 +276,17 @@
             if options.delete_sources:
                 print(f'{Colors.BOLD} - GitLab input group: '
                       f'{Colors.GREEN}{input_group.full_path}'
                       f'{Colors.CYAN} ({Namespaces.text(input_group.description)})'
                       f'{Colors.RESET}')
                 Platform.flush()
                 if not Entrypoint.confirm(
-                        'group',
+                        'Delete group',
                         input_group.full_path,
+                        'deletion',
                 ):
                     raise PermissionError()
 
                 # Delete input group
                 input_gitlab.group_delete(input_group.full_path)
                 print(f'{Colors.BOLD}   - Delete sources group: '
                       f'{Colors.GREEN}Success'
@@ -291,47 +317,71 @@
                         project.path_with_namespace,
                         input_namespace.full_path,
                         output_namespace.full_path,
                     )
                     if result in [Entrypoint.Result.FINALIZE, Entrypoint.Result.ERROR]:
                         return result
 
-                    # Delete input project after validation
-                    if options.delete_sources:
+                    # Handle sources
+                    if options.archive_sources or options.delete_sources:
                         print(f'{Colors.BOLD} - GitLab input project: '
                               f'{Colors.GREEN}{project.path_with_namespace}'
                               f'{Colors.CYAN} ({Namespaces.text(project.description)})'
                               f'{Colors.RESET}')
                         Platform.flush()
-                        if not Entrypoint.confirm(
-                                'project',
+
+                        # Archive input project
+                        if options.archive_sources:
+                            input_gitlab.project_set_archive(
                                 project.path_with_namespace,
-                        ):
-                            return Entrypoint.Result.SUCCESS
+                                enabled=True,
+                            )
+                            print(f'{Colors.BOLD}   - Archive sources project: '
+                                  f'{Colors.GREEN}Success'
+                                  f'{Colors.RESET}')
+                            print(' ')
+                            Platform.flush()
 
                         # Delete input project
-                        input_gitlab.project_delete(project.path_with_namespace)
-                        print(f'{Colors.BOLD}   - Delete sources project: '
-                              f'{Colors.GREEN}Success'
-                              f'{Colors.RESET}')
-                        print(' ')
-                        Platform.flush()
+                        elif options.delete_sources:
+
+                            # Confirm project deletion
+                            if not Entrypoint.confirm(
+                                    'Delete project',
+                                    project.path_with_namespace,
+                                    'deletion',
+                            ):
+                                print(' ')
+                                Platform.flush()
+                                return Entrypoint.Result.SUCCESS
+
+                            # Delete input project
+                            input_gitlab.project_delete(project.path_with_namespace)
+                            print(f'{Colors.BOLD}   - Delete sources project: '
+                                  f'{Colors.GREEN}Success'
+                                  f'{Colors.RESET}')
+                            print(' ')
+                            Platform.flush()
 
         # Result
         return Entrypoint.Result.SUCCESS
 
     # Confirm
     @staticmethod
-    def confirm(description: str, text: str = '') -> bool:
+    def confirm(
+        description: str,
+        text: str = '',
+        action: str = '',
+    ) -> bool:
 
         # Header
         print(
-            f'{Colors.BOLD}   - Delete {description}: Confirm "'
+            f'{Colors.BOLD}   - {description}: Confirm "'
             f'{Colors.RED}{text}'
-            f'{Colors.BOLD}" deletion:'
+            f'{Colors.BOLD}" {action}:'
             f'{Colors.RESET}', end='')
         Platform.flush()
 
         # Get user configuration
         answer: bool = questionary.confirm(
             message='',
             default=False,
@@ -339,15 +389,15 @@
             style=Themes.confirmation_style(),
             auto_enter=True,
         ).ask()
 
         # Result
         return answer
 
-    # Group, pylint: disable=too-many-arguments
+    # Group, pylint: disable=too-many-arguments,too-many-locals
     @staticmethod
     def group(
         options: Namespace,
         input_gitlab: GitLabFeature,
         output_gitlab: GitLabFeature,
         criteria_input_group: str,
         criteria_output_group: str,
@@ -372,22 +422,31 @@
               f'{Colors.CYAN}({Namespaces.text(input_group.description)})'
               f'{Colors.RESET}')
         Platform.flush()
 
         # Migration mode
         if not migration:
             output_subgroup = output_gitlab.group(criteria_output_group)
-            print(f'{Colors.BOLD}   - Already exists in GitLab output: '
+            print(f'{Colors.BOLD}   - Already existing group in GitLab output: '
                   f'{Colors.GREEN}{output_subgroup.full_path}'
                   f'{Colors.CYAN} ({Namespaces.text(output_subgroup.description)})'
                   f'{Colors.RESET}')
             print(' ')
             Platform.flush()
             return Entrypoint.Result.SUCCESS
 
+        # Confirm group is exportable
+        export_limitations = input_gitlab.group_export_limitations(input_group.full_path)
+        if export_limitations and not Entrypoint.confirm(
+                'Limited group export',
+                input_group.full_path,
+                'which uses "' + ("\", \"").join(export_limitations) + '"',
+        ):
+            raise PermissionError()
+
         # Export group
         print(f'{Colors.BOLD}   - Exporting from: '
               f'{Colors.GREEN}{input_group.full_path}'
               f'{Colors.RESET}')
         Platform.flush()
         with NamedTemporaryFile(
                 prefix=Paths.slugify(f'{Entrypoint.EXPORTS_PREFIX}'
@@ -463,63 +522,91 @@
     def project(
         options: Namespace,
         input_gitlab: GitLabFeature,
         output_gitlab: GitLabFeature,
         criteria_project: str,
         criteria_input_namespace: str,
         criteria_output_namespace: str,
+        rename_project: str = '',
     ) -> Result:
 
         # Variables
         output_project: GitLabProjectImport
 
         # Acquire input project
         input_project = input_gitlab.project(criteria_project)
 
         # Acquire input namespace
         input_namespace = input_gitlab.namespace(criteria_input_namespace)
 
+        # Parse input subpath
+        input_subpath = Namespaces.subpath(
+            input_namespace.full_path,
+            input_project.path_with_namespace,
+        )
+
         # Acquire output namespace
         output_namespace = output_gitlab.namespace(
             criteria_output_namespace,
             optional=True,
         )
 
+        # Project project name
+        output_project_name: str = rename_project if rename_project else input_project.name
+
+        # Parse output path
+        output_subnamespace, output_path = Namespaces.split_namespace(
+            input_subpath,
+            relative=True,
+        )
+        if output_path:
+            output_path = re.sub(
+                f'{input_project.name}$',
+                output_project_name,
+                output_path,
+            )
+
         # Show project details
         print(f'{Colors.BOLD} - GitLab input project: '
               f'{Colors.YELLOW_LIGHT}{input_project.path_with_namespace} '
               f'{Colors.CYAN}({Namespaces.text(input_project.description)})'
               f'{Colors.RESET}')
         Platform.flush()
 
         # Ignore existing projects
-        input_subpath = Namespaces.subpath(
-            input_namespace.full_path,
-            input_project.path_with_namespace,
-        )
-        if not options.overwrite and input_subpath in [
+        if not options.overwrite and output_path in [
                 Namespaces.subpath(
                     output_namespace.full_path,
                     output_project.path_with_namespace,
                 ) for output_project in output_gitlab.namespace_projects(
                     criteria_output_namespace)
         ]:
             project = output_gitlab.project(
                 f'{output_namespace.full_path}/{input_subpath}')
-            print(f'{Colors.BOLD}   - Already exists in GitLab output: '
+            print(f'{Colors.BOLD}   - Already existing project in GitLab output: '
                   f'{Colors.GREEN}{project.path_with_namespace}'
                   f'{Colors.CYAN} ({Namespaces.text(project.description)})'
                   f'{Colors.RESET}')
             print(' ')
             Platform.flush()
             return Entrypoint.Result.SUCCESS
 
+        # Confirm project is exportable
+        export_limitations = input_gitlab.project_export_limitations(
+            input_project.path_with_namespace)
+        if export_limitations and not Entrypoint.confirm(
+                'Limited project export',
+                input_project.path_with_namespace,
+                'which uses "' + ("\", \"").join(export_limitations) + '"',
+        ):
+            raise PermissionError()
+
         # Export project
         print(f'{Colors.BOLD}   - Exporting from: '
-              f'{Colors.GREEN}{options.input_path}'
+              f'{Colors.GREEN}{output_namespace.full_path}'
               f'{Colors.CYAN} / {input_subpath}'
               f'{Colors.RESET}')
         Platform.flush()
         with NamedTemporaryFile(
                 prefix=Paths.slugify(f'{Entrypoint.EXPORTS_PREFIX}'
                                      f'-{input_project.path_with_namespace}-'),
                 suffix='.tar.gz',
@@ -531,36 +618,33 @@
                 input_project.path_with_namespace,
                 options.keep_members,
             )
 
             # Existing project removal
             if options.overwrite:
                 if not Entrypoint.confirm(
-                        'project',
+                        'Delete project',
                         f'{output_namespace.full_path}/{input_subpath}',
+                        'deletion',
                 ):
                     raise PermissionError()
                 output_gitlab.project_delete(
                     f'{output_namespace.full_path}/{input_subpath}')
 
             # Import project
             print(f'{Colors.BOLD}   - Importing to: '
                   f'{Colors.GREEN}{options.output_namespace}'
-                  f'{Colors.CYAN} / {input_subpath}'
+                  f'{Colors.CYAN} / {output_subnamespace}{output_path}'
                   f'{Colors.RESET}')
             Platform.flush()
-            output_subnamespace, output_path = Namespaces.split_namespace(
-                input_subpath,
-                relative=True,
-            )
             output_project = output_gitlab.project_import(
                 file_export.name,
                 f'{options.output_namespace}{output_subnamespace}',
                 output_path,
-                input_project.name,
+                output_project_name,
                 options.overwrite,
             )
 
         # Acquire subgroup description
         output_subgroup_description: str
         if options.dry_run:
             output_subgroup_description = input_project.description
@@ -570,15 +654,15 @@
             output_subgroup = output_gitlab.group(
                 f'{options.output_namespace}{output_subnamespace}')
             output_subgroup_description = output_subgroup.description
 
         # Update project description
         if options.update_description:
             group_description = Namespaces.describe(
-                name=input_project.name,
+                name=output_project_name,
                 description=output_subgroup_description,
             )
             if not output_project.description or \
                     not output_project.description.endswith(f' - {group_description}'):
                 description = f'{Namespaces.describe(name=output_project.name)}' \
                                 f' - {group_description}'
                 output_gitlab.project_set_description(
@@ -661,34 +745,44 @@
             input_subpath,
             relative=True,
         )
 
         # Migration mode
         if migration:
 
-            # Ignore existing group
+            # Ignore existing subgroup
             if input_subpath in [
                     Namespaces.subpath(
                         output_group.full_path,
                         output_subgroup.full_path,
                     ) for output_subgroup in output_group.descendant_groups.list(
                         get_all=True,
                         include_subgroups=True,
                     )
             ]:
                 output_subgroup = output_gitlab.group(
                     f'{output_group.full_path}/{input_subpath}')
-                print(f'{Colors.BOLD}   - Already exists in GitLab output: '
+                print(f'{Colors.BOLD}   - Already existing subgroup in GitLab output: '
                       f'{Colors.GREEN}{output_subgroup.full_path}'
                       f'{Colors.CYAN} ({Namespaces.text(output_subgroup.description)})'
                       f'{Colors.RESET}')
                 print(' ')
                 Platform.flush()
                 return Entrypoint.Result.SUCCESS
 
+            # Confirm subgroup is exportable
+            export_limitations = input_gitlab.group_export_limitations(
+                input_subgroup.full_path)
+            if export_limitations and not Entrypoint.confirm(
+                    'Limited subgroup export',
+                    input_subgroup.full_path,
+                    'which uses "' + ("\", \"").join(export_limitations) + '"',
+            ):
+                raise PermissionError()
+
             # Export subgroup
             print(f'{Colors.BOLD}   - Exporting from: '
                   f'{Colors.GREEN}{input_subgroup.full_path}'
                   f'{Colors.RESET}')
             Platform.flush()
             with NamedTemporaryFile(
                     prefix=Paths.slugify(f'{Entrypoint.EXPORTS_PREFIX}'
```

### Comparing `gitlab_projects_migrate-3.1.0/src/cli/main.py` & `gitlab_projects_migrate-4.0.0/src/cli/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ..package.updates import Updates
 from ..package.version import Version
 from ..prints.colors import Colors
 from ..system.platform import Platform
 from ..types.paths import Paths
 from .entrypoint import Entrypoint
 
-# Main, pylint: disable=too-many-statements
+# Main, pylint: disable=too-many-branches,too-many-statements
 def main() -> None:
 
     # Variables
     group: _ArgumentGroup
     result: Entrypoint.Result = Entrypoint.Result.ERROR
 
     # Arguments creation
@@ -113,15 +113,22 @@
     group.add_argument(
         '--archive-exports',
         dest='archive_exports',
         action='store',
         metavar='FOLDER',
         help='Store exported projects and groups to a folder',
     )
-    group.add_argument(
+    subgroup = group.add_mutually_exclusive_group()
+    subgroup.add_argument(
+        '--archive-sources',
+        dest='archive_sources',
+        action='store_true',
+        help='Archive sources after successful migration',
+    )
+    subgroup.add_argument(
         '--delete-sources',
         dest='delete_sources',
         action='store_true',
         help='Delete sources after successful migration',
     )
     group.add_argument(
         '--dry-run',
@@ -155,14 +162,21 @@
     )
     group.add_argument(
         '--overwrite',
         dest='overwrite',
         action='store_true',
         help='Overwrite existing projects on output GitLab',
     )
+    group.add_argument(
+        '--rename-project',
+        dest='rename_project',
+        action='store',
+        metavar='NAME',
+        help='Rename GitLab output project (only for single input project)',
+    )
 
     # Arguments general settings definitions
     group = parser.add_argument_group('general settings arguments')
     group.add_argument(
         '--set-avatar',
         dest='set_avatar',
         action='store',
@@ -266,19 +280,15 @@
         if not updates.check():
             updates.check(older=True)
         sys_exit(0)
 
     # Arguments validation
     if not options.input_token or not options.input_gitlab or not options.input_path \
             or not options.output_gitlab or not options.output_namespace:
-        print(' ')
-        parser.print_help()
-        print(' ')
-        Platform.flush()
-        sys_exit(1)
+        result = Entrypoint.Result.CRITICAL
 
     # Prepare archive exports
     if options.archive_exports:
         options.archive_exports_dir = Paths.resolve(Path('.') / options.archive_exports)
         Path(options.archive_exports_dir).mkdir(parents=True, exist_ok=True)
 
     # Arguments adaptations
@@ -286,15 +296,20 @@
         options.output_token = options.input_token
 
     # Header
     print(' ')
     Platform.flush()
 
     # CLI entrypoint
-    result = Entrypoint.cli(options)
+    if result != Entrypoint.Result.CRITICAL:
+        result = Entrypoint.cli(options)
+
+    # CLI helper
+    else:
+        parser.print_help()
 
     # Footer
     print(' ')
     Platform.flush()
 
     # Check for daily updates
     if updates.enabled and updates.daily:
```

### Comparing `gitlab_projects_migrate-3.1.0/src/features/gitlab.py` & `gitlab_projects_migrate-4.0.0/src/features/gitlab.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from shutil import make_archive, unpack_archive
 from tempfile import TemporaryDirectory
 from time import sleep
 from typing import Any, cast, List, Optional
 
 # Modules libraries
 from gitlab import Gitlab
-from gitlab.exceptions import GitlabDeleteError, GitlabGetError
+from gitlab.exceptions import GitlabDeleteError, GitlabGetError, GitlabListError
 from gitlab.v4.objects import Group, Namespace, Project, ProjectImport, User
 
 # Components
 from ..types.namespaces import Namespaces
 
-# GitLabFeature class
+# GitLabFeature class, pylint: disable=too-many-public-methods
 class GitLabFeature:
 
     # Constants
     TIMEOUT_DELETION: int = 300
 
     # Members
     __dry_run: bool = False
@@ -132,14 +132,30 @@
                 unpack_archive(archive, temp_directory, 'gztar')
                 for path in Path(join(temp_directory, 'tree', 'groups')).glob(
                         join('*', 'members.ndjson')):
                     path.unlink()
                 remove(archive)
                 make_archive(stem, 'gztar', temp_directory)
 
+    # Group export limitations
+    def group_export_limitations(self, criteria: str) -> List[str]:
+
+        # Variables
+        result: List[str] = []
+
+        # Get group
+        group = self.group(criteria)
+
+        # Limitations: CI variables
+        if group.variables.list():
+            result += ['Variables']
+
+        # Result
+        return result
+
     # Group import, pylint: disable=too-many-arguments
     def group_import(
         self,
         archive: str,
         parent: str,
         path: str,
         name: str,
@@ -305,14 +321,44 @@
                 if stem.endswith('.tar.gz'):
                     stem = stem[:-len('.tar.gz')]
                 unpack_archive(archive, temp_directory, 'gztar')
                 remove(join(temp_directory, 'tree', 'project', 'project_members.ndjson'))
                 remove(archive)
                 make_archive(stem, 'gztar', temp_directory)
 
+    # Project export limitations
+    def project_export_limitations(self, criteria: str) -> List[str]:
+
+        # Variables
+        result: List[str] = []
+
+        # Get project
+        project = self.project(criteria)
+
+        # Limitations: Packages registry
+        try:
+            if project.packages.list(get_all=False):
+                result += ['Packages registry']
+        except GitlabListError:
+            pass
+
+        # Limitations: Container registry
+        try:
+            if project.repositories.list(get_all=False):
+                result += ['Container registry']
+        except GitlabListError:
+            pass
+
+        # Limitations: CI variables
+        if project.variables.list():
+            result += ['Variables']
+
+        # Result
+        return result
+
     # Project import, pylint: disable=too-many-arguments
     def project_import(
         self,
         archive: str,
         group: str,
         path: str,
         name: str,
@@ -321,24 +367,26 @@
 
         # Validate project access
         if self.__dry_run:
             ProjectTuple = namedtuple('ProjectTuple', [
                 'id',
                 'name',
                 'description',
+                'path_with_namespace',
             ])
             return cast(
                 ProjectImport,
                 ProjectTuple(
                     id='dry-run',
                     name=name,
                     description=Namespaces.capitalize(
                         name,
                         words=True,
                     ),
+                    path_with_namespace=path,
                 ),
             )
 
         # Upload project import
         with open(archive, 'rb') as file:
             project_imported = self.__gitlab.projects.import_project(
                 file, # type: ignore[arg-type] # TODO: BufferedReader instead of str # pylint: disable=fixme
@@ -373,14 +421,27 @@
                     project.members.delete(member.id)
                 except GitlabDeleteError:
                     pass
 
             # Save project
             project.save()
 
+    # Project set archive
+    def project_set_archive(self, criteria: str, enabled: bool) -> None:
+
+        # Archive project
+        if not self.__dry_run and enabled:
+            project = self.project(criteria)
+            project.archive()
+
+        # Unarchive project
+        elif not self.__dry_run:
+            project = self.project(criteria)
+            project.unarchive()
+
     # Project set avatar
     def project_set_avatar(self, criteria: str, file: str) -> None:
 
         # Set project avatar
         if not self.__dry_run:
             project = self.project(criteria)
             with open(file, 'rb') as avatar:
```

### Comparing `gitlab_projects_migrate-3.1.0/src/package/bundle.py` & `gitlab_projects_migrate-4.0.0/src/package/bundle.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/src/package/settings.py` & `gitlab_projects_migrate-4.0.0/src/package/settings.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/src/package/updates.py` & `gitlab_projects_migrate-4.0.0/src/package/updates.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/src/package/version.py` & `gitlab_projects_migrate-4.0.0/src/package/version.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/src/prints/boxes.py` & `gitlab_projects_migrate-4.0.0/src/prints/boxes.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/src/prints/colors.py` & `gitlab_projects_migrate-4.0.0/src/prints/colors.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/src/prints/themes.py` & `gitlab_projects_migrate-4.0.0/src/prints/themes.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/src/system/platform.py` & `gitlab_projects_migrate-4.0.0/src/system/platform.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/src/types/namespaces.py` & `gitlab_projects_migrate-4.0.0/src/types/namespaces.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/src/types/paths.py` & `gitlab_projects_migrate-4.0.0/src/types/paths.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-3.1.0/src/types/strings.py` & `gitlab_projects_migrate-4.0.0/src/types/strings.py`

 * *Files identical despite different names*

