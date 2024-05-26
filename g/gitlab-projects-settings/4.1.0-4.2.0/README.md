# Comparing `tmp/gitlab_projects_settings-4.1.0.tar.gz` & `tmp/gitlab_projects_settings-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_settings-4.1.0.tar", last modified: Fri May 17 02:44:43 2024, max compression
+gzip compressed data, was "gitlab_projects_settings-4.2.0.tar", last modified: Sun May 26 22:48:20 2024, max compression
```

## Comparing `gitlab_projects_settings-4.1.0.tar` & `gitlab_projects_settings-4.2.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.090166 gitlab_projects_settings-4.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.080166 gitlab_projects_settings-4.1.0/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      703 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    11981 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.080166 gitlab_projects_settings-4.1.0/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     5380 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7748 2024-05-17 02:44:43.090166 gitlab_projects_settings-4.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6067 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.089166 gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7748 2024-05-17 02:44:43.000000 gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1075 2024-05-17 02:44:43.000000 gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 02:44:43.000000 gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2024-05-17 02:44:43.000000 gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2024-05-17 02:44:43.000000 gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 02:44:43.000000 gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.083166 gitlab_projects_settings-4.1.0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 02:44:43.090166 gitlab_projects_settings-4.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2868 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.084167 gitlab_projects_settings-4.1.0/src/
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.085167 gitlab_projects_settings-4.1.0/src/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18062 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/cli/entrypoint.py
--rwxrwxrwx   0 root         (0) root         (0)     9111 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.085167 gitlab_projects_settings-4.1.0/src/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14811 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/features/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.086166 gitlab_projects_settings-4.1.0/src/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      754 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     3810 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/package/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     6845 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/package/updates.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.087166 gitlab_projects_settings-4.1.0/src/prints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/prints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2549 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/prints/boxes.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/prints/colors.py
--rw-rw-rw-   0 root         (0) root         (0)     1565 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/prints/themes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.088167 gitlab_projects_settings-4.1.0/src/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1788 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/system/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 02:44:43.089166 gitlab_projects_settings-4.1.0/src/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11789 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/types/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      728 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/types/namespaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2024-05-17 02:44:38.000000 gitlab_projects_settings-4.1.0/src/types/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:48:20.680583 gitlab_projects_settings-4.2.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:48:20.671583 gitlab_projects_settings-4.2.0/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      703 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    11981 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:48:20.671583 gitlab_projects_settings-4.2.0/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     5728 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8398 2024-05-26 22:48:20.680583 gitlab_projects_settings-4.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6717 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:48:20.680583 gitlab_projects_settings-4.2.0/gitlab_projects_settings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8398 2024-05-26 22:48:20.000000 gitlab_projects_settings-4.2.0/gitlab_projects_settings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1075 2024-05-26 22:48:20.000000 gitlab_projects_settings-4.2.0/gitlab_projects_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-26 22:48:20.000000 gitlab_projects_settings-4.2.0/gitlab_projects_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-26 22:48:20.000000 gitlab_projects_settings-4.2.0/gitlab_projects_settings.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2024-05-26 22:48:20.000000 gitlab_projects_settings-4.2.0/gitlab_projects_settings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-26 22:48:20.000000 gitlab_projects_settings-4.2.0/gitlab_projects_settings.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:48:20.674583 gitlab_projects_settings-4.2.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-26 22:48:20.680583 gitlab_projects_settings-4.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:48:20.674583 gitlab_projects_settings-4.2.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:48:20.675583 gitlab_projects_settings-4.2.0/src/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18420 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/cli/entrypoint.py
+-rwxrwxrwx   0 root         (0) root         (0)     9306 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:48:20.675583 gitlab_projects_settings-4.2.0/src/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14811 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/features/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:48:20.677583 gitlab_projects_settings-4.2.0/src/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      754 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/package/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     6845 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/package/updates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:48:20.678583 gitlab_projects_settings-4.2.0/src/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/prints/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/prints/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/prints/themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:48:20.678583 gitlab_projects_settings-4.2.0/src/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 22:48:20.679583 gitlab_projects_settings-4.2.0/src/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11789 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/types/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      728 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/types/namespaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2024-05-26 22:48:16.000000 gitlab_projects_settings-4.2.0/src/types/strings.py
```

### Comparing `gitlab_projects_settings-4.1.0/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_settings-4.2.0/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/.chglog/changelog.sh` & `gitlab_projects_settings-4.2.0/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/.chglog/config.yml` & `gitlab_projects_settings-4.2.0/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/.gitlab-ci.yml` & `gitlab_projects_settings-4.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/.style.yapf` & `gitlab_projects_settings-4.2.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/.vscode/extensions.json` & `gitlab_projects_settings-4.2.0/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/.vscode/settings.json` & `gitlab_projects_settings-4.2.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/CHANGELOG.md` & `gitlab_projects_settings-4.2.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,21 @@
 
+<a name="4.2.0"></a>
+## [4.2.0](https://gitlab.com/AdrianDC/gitlab-projects-settings/compare/4.1.0...4.2.0) (2024-05-27)
+
+### Documentation
+
+* **readme:** add 'gitlab-projects-settings' examples documentation
+
+### Features
+
+* **entrypoint:** improve outputs logs upon delections
+* **main:** show newer updates message upon incompatible arguments
+
+
 <a name="4.1.0"></a>
 ## [4.1.0](https://gitlab.com/AdrianDC/gitlab-projects-settings/compare/4.0.0...4.1.0) (2024-05-17)
 
 ### Features
 
 * **entrypoint:** implement prompt confirmation upon deletions
 * **gitlab:** isolate 'ProtectionLevels' enumeration
```

### Comparing `gitlab_projects_settings-4.1.0/LICENSE` & `gitlab_projects_settings-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/PKG-INFO` & `gitlab_projects_settings-4.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 4.1.0
+Version: 4.2.0
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
@@ -54,22 +54,44 @@
 
 The following step is required before using the tool:
 
 - The GitLab user tokens must be created with an `api` scope (a short expiration date is recommended)
 
 ---
 
+## Examples
+
+<!-- prettier-ignore-start -->
+
+```bash
+# Show the helper menu
+gitlab-projects-settings
+
+# Protect all projects' tags under a group
+gitlab-projects-settings --protect-tags -- 'https://gitlab.com' 'group'
+
+# Update all avatars and descriptions under a group
+gitlab-projects-settings --set-avatar ./avatar.png --update-description 'https://gitlab.com' 'group'
+
+# Automatically detect and reset features of projects based on usage
+gitlab-projects-settings --reset-features 'https://gitlab.com' 'group/project'
+```
+
+<!-- prettier-ignore-end -->
+
+---
+
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
 usage: gitlab-projects-settings [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-t TOKEN]
-                                [--dry-run] [--exclude-group] [--exclude-subgroups] [--exclude-projects]
+                                [--dry-run] [--dump] [--exclude-group] [--exclude-subgroups] [--exclude-projects]
                                 [--available-features] [--reset-features [KEEP_FEATURES]]
                                 [--disable-features FEATURES] [--enable-features FEATURES] [--reset-members]
                                 [--set-avatar FILE] [--set-description TEXT] [--update-description]
                                 [--run-housekeeping] [--archive-project | --unarchive-project] [--delete-group]
                                 [--delete-project] [--protect-branches] [--protect-tags [LEVEL]] [--]
                                 [gitlab] [path]
 
@@ -84,14 +106,15 @@
                                     # or unset by using 'UNSET' as 'VAL'
 
 credentials arguments:
   -t TOKEN                          # GitLab API token (default: GITLAB_TOKEN environment)
 
 common settings arguments:
   --dry-run                         # Enable dry run mode to check without saving
+  --dump                            # Dump Python objects of groups and projects
   --exclude-group                   # Exclude parent group settings
   --exclude-subgroups               # Exclude children subgroups settings
   --exclude-projects                # Exclude children projects settings
 
 general settings arguments:
   --available-features              # List the available GitLab project features known by the tool
   --reset-features [KEEP_FEATURES]  # Reset features of GitLab projects based on usage
```

### Comparing `gitlab_projects_settings-4.1.0/README.md` & `gitlab_projects_settings-4.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,44 @@
 
 The following step is required before using the tool:
 
 - The GitLab user tokens must be created with an `api` scope (a short expiration date is recommended)
 
 ---
 
+## Examples
+
+<!-- prettier-ignore-start -->
+
+```bash
+# Show the helper menu
+gitlab-projects-settings
+
+# Protect all projects' tags under a group
+gitlab-projects-settings --protect-tags -- 'https://gitlab.com' 'group'
+
+# Update all avatars and descriptions under a group
+gitlab-projects-settings --set-avatar ./avatar.png --update-description 'https://gitlab.com' 'group'
+
+# Automatically detect and reset features of projects based on usage
+gitlab-projects-settings --reset-features 'https://gitlab.com' 'group/project'
+```
+
+<!-- prettier-ignore-end -->
+
+---
+
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
 usage: gitlab-projects-settings [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-t TOKEN]
-                                [--dry-run] [--exclude-group] [--exclude-subgroups] [--exclude-projects]
+                                [--dry-run] [--dump] [--exclude-group] [--exclude-subgroups] [--exclude-projects]
                                 [--available-features] [--reset-features [KEEP_FEATURES]]
                                 [--disable-features FEATURES] [--enable-features FEATURES] [--reset-members]
                                 [--set-avatar FILE] [--set-description TEXT] [--update-description]
                                 [--run-housekeeping] [--archive-project | --unarchive-project] [--delete-group]
                                 [--delete-project] [--protect-branches] [--protect-tags [LEVEL]] [--]
                                 [gitlab] [path]
 
@@ -48,14 +70,15 @@
                                     # or unset by using 'UNSET' as 'VAL'
 
 credentials arguments:
   -t TOKEN                          # GitLab API token (default: GITLAB_TOKEN environment)
 
 common settings arguments:
   --dry-run                         # Enable dry run mode to check without saving
+  --dump                            # Dump Python objects of groups and projects
   --exclude-group                   # Exclude parent group settings
   --exclude-subgroups               # Exclude children subgroups settings
   --exclude-projects                # Exclude children projects settings
 
 general settings arguments:
   --available-features              # List the available GitLab project features known by the tool
   --reset-features [KEEP_FEATURES]  # Reset features of GitLab projects based on usage
```

### Comparing `gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/PKG-INFO` & `gitlab_projects_settings-4.2.0/gitlab_projects_settings.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-settings
-Version: 4.1.0
+Version: 4.2.0
 Summary: Configure GitLab groups and projects settings automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-settings
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-settings/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-settings/blob/main/CHANGELOG.md
@@ -54,22 +54,44 @@
 
 The following step is required before using the tool:
 
 - The GitLab user tokens must be created with an `api` scope (a short expiration date is recommended)
 
 ---
 
+## Examples
+
+<!-- prettier-ignore-start -->
+
+```bash
+# Show the helper menu
+gitlab-projects-settings
+
+# Protect all projects' tags under a group
+gitlab-projects-settings --protect-tags -- 'https://gitlab.com' 'group'
+
+# Update all avatars and descriptions under a group
+gitlab-projects-settings --set-avatar ./avatar.png --update-description 'https://gitlab.com' 'group'
+
+# Automatically detect and reset features of projects based on usage
+gitlab-projects-settings --reset-features 'https://gitlab.com' 'group/project'
+```
+
+<!-- prettier-ignore-end -->
+
+---
+
 ## Usage
 
 <!-- prettier-ignore-start -->
 <!-- readme-help-start -->
 
 ```yaml
 usage: gitlab-projects-settings [-h] [--version] [--update-check] [--settings] [--set GROUP KEY VAL] [-t TOKEN]
-                                [--dry-run] [--exclude-group] [--exclude-subgroups] [--exclude-projects]
+                                [--dry-run] [--dump] [--exclude-group] [--exclude-subgroups] [--exclude-projects]
                                 [--available-features] [--reset-features [KEEP_FEATURES]]
                                 [--disable-features FEATURES] [--enable-features FEATURES] [--reset-members]
                                 [--set-avatar FILE] [--set-description TEXT] [--update-description]
                                 [--run-housekeeping] [--archive-project | --unarchive-project] [--delete-group]
                                 [--delete-project] [--protect-branches] [--protect-tags [LEVEL]] [--]
                                 [gitlab] [path]
 
@@ -84,14 +106,15 @@
                                     # or unset by using 'UNSET' as 'VAL'
 
 credentials arguments:
   -t TOKEN                          # GitLab API token (default: GITLAB_TOKEN environment)
 
 common settings arguments:
   --dry-run                         # Enable dry run mode to check without saving
+  --dump                            # Dump Python objects of groups and projects
   --exclude-group                   # Exclude parent group settings
   --exclude-subgroups               # Exclude children subgroups settings
   --exclude-projects                # Exclude children projects settings
 
 general settings arguments:
   --available-features              # List the available GitLab project features known by the tool
   --reset-features [KEEP_FEATURES]  # Reset features of GitLab projects based on usage
```

### Comparing `gitlab_projects_settings-4.1.0/gitlab_projects_settings.egg-info/SOURCES.txt` & `gitlab_projects_settings-4.2.0/gitlab_projects_settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/setup.py` & `gitlab_projects_settings-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/src/cli/entrypoint.py` & `gitlab_projects_settings-4.2.0/src/cli/entrypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from ..system.platform import Platform
 from ..types.namespaces import Namespaces
 
 # Entrypoint class, pylint: disable=too-few-public-methods
 class Entrypoint:
 
     # Enumerations
-    Result = Enum('Result', ['SUCCESS', 'FINALIZE', 'ERROR'])
+    Result = Enum('Result', ['SUCCESS', 'FINALIZE', 'ERROR', 'CRITICAL'])
 
     # CLI, pylint: disable=too-many-branches
     @staticmethod
     def cli(options: Namespace) -> Result:
 
         # Variables
         group: Optional[GitLabGroup] = None
@@ -233,14 +233,16 @@
 
         # Delete group after validation
         if options.delete_group:
             if not Entrypoint.confirm(
                     group_type,
                     group.full_path,
             ):
+                print(' ')
+                Platform.flush()
                 return Entrypoint.Result.SUCCESS
 
             # Delete group
             gitlab.group_delete(criteria)
             print(f'{Colors.BOLD}   - Delete {group_type}: '
                   f'{Colors.GREEN}Success'
                   f'{Colors.RESET}')
@@ -293,14 +295,19 @@
         if options.set_avatar:
             gitlab.group_set_avatar(criteria, options.set_avatar)
             print(f'{Colors.BOLD}   - Set avatar: '
                   f'{Colors.CYAN}{options.set_avatar}'
                   f'{Colors.RESET}')
             Platform.flush()
 
+        # Dump group object
+        if options.dump:
+            print(' ')
+            print(group.to_json())
+
         # Footer
         print(' ')
         Platform.flush()
 
         # Result
         return Entrypoint.Result.SUCCESS
 
@@ -324,14 +331,16 @@
 
         # Delete project after validation
         if options.delete_project:
             if not Entrypoint.confirm(
                     'project',
                     project.path_with_namespace,
             ):
+                print(' ')
+                Platform.flush()
                 return Entrypoint.Result.SUCCESS
 
             # Delete project
             gitlab.project_delete(criteria)
             print(f'{Colors.BOLD}   - Delete project: '
                   f'{Colors.GREEN}Success'
                   f'{Colors.RESET}')
@@ -493,13 +502,18 @@
                 Platform.flush()
             else:
                 print(f'{Colors.BOLD}   - Protecting tags: '
                       f'{Colors.GREEN}Already done'
                       f'{Colors.RESET}')
                 Platform.flush()
 
+        # Dump group object
+        if options.dump:
+            print(' ')
+            print(project.to_json())
+
         # Footer
         print(' ')
         Platform.flush()
 
         # Result
         return Entrypoint.Result.SUCCESS
```

### Comparing `gitlab_projects_settings-4.1.0/src/cli/main.py` & `gitlab_projects_settings-4.2.0/src/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,14 +91,20 @@
     group.add_argument(
         '--dry-run',
         dest='dry_run',
         action='store_true',
         help='Enable dry run mode to check without saving',
     )
     group.add_argument(
+        '--dump',
+        dest='dump',
+        action='store_true',
+        help='Dump Python objects of groups and projects',
+    )
+    group.add_argument(
         '--exclude-group',
         dest='exclude_group',
         action='store_true',
         help='Exclude parent group settings',
     )
     group.add_argument(
         '--exclude-subgroups',
@@ -288,26 +294,27 @@
     if options.update_check:
         if not updates.check():
             updates.check(older=True)
         sys_exit(0)
 
     # Arguments validation
     if not options.token or not options.gitlab or not options.path:
-        print(' ')
-        parser.print_help()
-        print(' ')
-        Platform.flush()
-        sys_exit(1)
+        result = Entrypoint.Result.CRITICAL
 
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

### Comparing `gitlab_projects_settings-4.1.0/src/features/gitlab.py` & `gitlab_projects_settings-4.2.0/src/features/gitlab.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/src/package/bundle.py` & `gitlab_projects_settings-4.2.0/src/package/bundle.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/src/package/settings.py` & `gitlab_projects_settings-4.2.0/src/package/settings.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/src/package/updates.py` & `gitlab_projects_settings-4.2.0/src/package/updates.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/src/package/version.py` & `gitlab_projects_settings-4.2.0/src/package/version.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/src/prints/boxes.py` & `gitlab_projects_settings-4.2.0/src/prints/boxes.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/src/prints/colors.py` & `gitlab_projects_settings-4.2.0/src/prints/colors.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/src/prints/themes.py` & `gitlab_projects_settings-4.2.0/src/prints/themes.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/src/system/platform.py` & `gitlab_projects_settings-4.2.0/src/system/platform.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/src/types/gitlab.py` & `gitlab_projects_settings-4.2.0/src/types/gitlab.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/src/types/namespaces.py` & `gitlab_projects_settings-4.2.0/src/types/namespaces.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_settings-4.1.0/src/types/strings.py` & `gitlab_projects_settings-4.2.0/src/types/strings.py`

 * *Files identical despite different names*

