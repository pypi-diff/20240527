# Comparing `tmp/iniUts-1.1.8.tar.gz` & `tmp/iniUts-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iniUts-1.1.8.tar", last modified: Tue Apr 16 22:56:20 2024, max compression
+gzip compressed data, was "iniUts-1.1.9.tar", last modified: Mon May 27 13:02:12 2024, max compression
```

## Comparing `iniUts-1.1.8.tar` & `iniUts-1.1.9.tar`

### file list

```diff
@@ -1,834 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:20.248799 iniUts-1.1.8/
--rw-rw-rw-   0        0        0      465 2023-04-28 18:31:34.000000 iniUts-1.1.8/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-04-26 17:09:25.000000 iniUts-1.1.8/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-04-26 17:09:25.000000 iniUts-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4695 2024-04-16 22:56:20.247801 iniUts-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3696 2024-04-16 22:56:01.000000 iniUts-1.1.8/README.md
--rw-rw-rw-   0        0        0      212 2024-04-16 22:37:47.000000 iniUts-1.1.8/commands.txt
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.076644 iniUts-1.1.8/iniUts/
--rw-rw-rw-   0        0        0     7237 2024-04-16 22:51:59.000000 iniUts-1.1.8/iniUts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.107642 iniUts-1.1.8/iniUts.egg-info/
--rw-rw-rw-   0        0        0     4695 2024-04-16 22:56:16.000000 iniUts-1.1.8/iniUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    42662 2024-04-16 22:56:16.000000 iniUts-1.1.8/iniUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 22:56:16.000000 iniUts-1.1.8/iniUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-16 22:56:16.000000 iniUts-1.1.8/iniUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       20 2024-02-02 17:09:39.000000 iniUts-1.1.8/run.py
--rw-rw-rw-   0        0        0       42 2024-04-16 22:56:20.248799 iniUts-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      742 2024-04-16 22:56:11.000000 iniUts-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:16.978645 iniUts-1.1.8/venv/
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:16.978645 iniUts-1.1.8/venv/Lib/
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.042644 iniUts-1.1.8/venv/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.112772 iniUts-1.1.8/venv/Lib/site-packages/_distutils_hack/
--rw-rw-rw-   0        0        0     6128 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/_distutils_hack/__init__.py
--rw-rw-rw-   0        0        0       44 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/_distutils_hack/override.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.116772 iniUts-1.1.8/venv/Lib/site-packages/pip/
--rw-rw-rw-   0        0        0      357 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/__init__.py
--rw-rw-rw-   0        0        0      854 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/__main__.py
--rw-rw-rw-   0        0        0     1444 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/__pip-runner__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.147925 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/
--rw-rw-rw-   0        0        0      515 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/__init__.py
--rw-rw-rw-   0        0        0    10243 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/build_env.py
--rw-rw-rw-   0        0        0    10370 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/cache.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.177029 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/cli/
--rw-rw-rw-   0        0        0      132 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-rw-rw-   0        0        0     6690 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-rw-rw-   0        0        0     8733 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-rw-rw-   0        0        0    30117 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-rw-rw-   0        0        0      774 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-rw-rw-   0        0        0     2816 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/cli/main.py
--rw-rw-rw-   0        0        0     4338 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-rw-rw-   0        0        0    10801 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/cli/parser.py
--rw-rw-rw-   0        0        0     1968 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-rw-rw-   0        0        0    18369 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-rw-rw-   0        0        0     5118 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-rw-rw-   0        0        0      116 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.217028 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/
--rw-rw-rw-   0        0        0     3882 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-rw-rw-   0        0        0     7952 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/cache.py
--rw-rw-rw-   0        0        0     1782 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/check.py
--rw-rw-rw-   0        0        0     4287 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/completion.py
--rw-rw-rw-   0        0        0     9815 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-rw-rw-   0        0        0     6854 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/debug.py
--rw-rw-rw-   0        0        0     5335 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/download.py
--rw-rw-rw-   0        0        0     3172 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-rw-rw-   0        0        0     1703 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/hash.py
--rw-rw-rw-   0        0        0     1132 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/help.py
--rw-rw-rw-   0        0        0     4793 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/index.py
--rw-rw-rw-   0        0        0     3188 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/inspect.py
--rw-rw-rw-   0        0        0    28920 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/install.py
--rw-rw-rw-   0        0        0    12450 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/list.py
--rw-rw-rw-   0        0        0     5697 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/search.py
--rw-rw-rw-   0        0        0     6419 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/show.py
--rw-rw-rw-   0        0        0     3886 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-rw-rw-   0        0        0     6476 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-rw-rw-   0        0        0    13839 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/configuration.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.235028 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/distributions/
--rw-rw-rw-   0        0        0      858 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-rw-rw-   0        0        0     1743 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/distributions/base.py
--rw-rw-rw-   0        0        0      842 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-rw-rw-   0        0        0     6709 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-rw-rw-   0        0        0     1277 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-rw-rw-   0        0        0    23737 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.245027 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/index/
--rw-rw-rw-   0        0        0       30 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/index/__init__.py
--rw-rw-rw-   0        0        0    16504 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/index/collector.py
--rw-rw-rw-   0        0        0    37889 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-rw-rw-   0        0        0     6556 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/index/sources.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.251026 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/locations/
--rw-rw-rw-   0        0        0    15365 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-rw-rw-   0        0        0     6102 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-rw-rw-   0        0        0     7680 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-rw-rw-   0        0        0     2556 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/locations/base.py
--rw-rw-rw-   0        0        0      340 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/main.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.261028 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/metadata/
--rw-rw-rw-   0        0        0     4339 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-rw-rw-   0        0        0     2595 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/metadata/_json.py
--rw-rw-rw-   0        0        0    25907 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/metadata/base.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.267027 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/metadata/importlib/
--rw-rw-rw-   0        0        0      135 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-rw-rw-   0        0        0     1882 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-rw-rw-   0        0        0     8297 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-rw-rw-   0        0        0     7456 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-rw-rw-   0        0        0    10035 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.294027 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/models/
--rw-rw-rw-   0        0        0       63 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/models/__init__.py
--rw-rw-rw-   0        0        0      990 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/models/candidate.py
--rw-rw-rw-   0        0        0     6931 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-rw-rw-   0        0        0     2520 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/models/format_control.py
--rw-rw-rw-   0        0        0     1030 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/models/index.py
--rw-rw-rw-   0        0        0     2818 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/models/installation_report.py
--rw-rw-rw-   0        0        0    20819 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/models/link.py
--rw-rw-rw-   0        0        0      738 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/models/scheme.py
--rw-rw-rw-   0        0        0     4643 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-rw-rw-   0        0        0     1907 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-rw-rw-   0        0        0     4272 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/models/target_python.py
--rw-rw-rw-   0        0        0     3600 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/models/wheel.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.313027 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/network/
--rw-rw-rw-   0        0        0       50 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/network/__init__.py
--rw-rw-rw-   0        0        0    20541 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/network/auth.py
--rw-rw-rw-   0        0        0     3935 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/network/cache.py
--rw-rw-rw-   0        0        0     6096 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/network/download.py
--rw-rw-rw-   0        0        0     7638 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-rw-rw-   0        0        0    18607 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/network/session.py
--rw-rw-rw-   0        0        0     4073 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/network/utils.py
--rw-rw-rw-   0        0        0     1791 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.319027 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.335028 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/build/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
--rw-rw-rw-   0        0        0     4832 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-rw-rw-   0        0        0     1422 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
--rw-rw-rw-   0        0        0     1474 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-rw-rw-   0        0        0     2198 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-rw-rw-   0        0        0     1075 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
--rw-rw-rw-   0        0        0     1417 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-rw-rw-   0        0        0     3064 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-rw-rw-   0        0        0     6806 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/check.py
--rw-rw-rw-   0        0        0     9816 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/freeze.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.343028 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/install/
--rw-rw-rw-   0        0        0       51 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-rw-rw-   0        0        0     1282 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-rw-rw-   0        0        0    27457 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-rw-rw-   0        0        0    28155 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-rw-rw-   0        0        0     7161 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/pyproject.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.356030 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/req/
--rw-rw-rw-   0        0        0     2738 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/req/__init__.py
--rw-rw-rw-   0        0        0    19028 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/req/constructors.py
--rw-rw-rw-   0        0        0    17872 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/req/req_file.py
--rw-rw-rw-   0        0        0    35130 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/req/req_install.py
--rw-rw-rw-   0        0        0     4704 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/req/req_set.py
--rw-rw-rw-   0        0        0    24676 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.360027 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-rw-rw-   0        0        0      583 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/base.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.363027 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/legacy/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-rw-rw-   0        0        0    24128 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.383029 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-rw-rw-   0        0        0     5173 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-rw-rw-   0        0        0    21320 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-rw-rw-   0        0        0    32300 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-rw-rw-   0        0        0     5705 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-rw-rw-   0        0        0     9824 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-rw-rw-   0        0        0     3100 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-rw-rw-   0        0        0     6030 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-rw-rw-   0        0        0    12592 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-rw-rw-   0        0        0     8378 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.504029 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-rw-rw-   0        0        0     3351 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-rw-rw-   0        0        0     1015 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/_log.py
--rw-rw-rw-   0        0        0     1665 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-rw-rw-   0        0        0     1884 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/compat.py
--rw-rw-rw-   0        0        0     5377 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-rw-rw-   0        0        0      242 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-rw-rw-   0        0        0     3627 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-rw-rw-   0        0        0     3206 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-rw-rw-   0        0        0     2118 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-rw-rw-   0        0        0     1169 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-rw-rw-   0        0        0     3064 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-rw-rw-   0        0        0     5122 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-rw-rw-   0        0        0      716 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-rw-rw-   0        0        0     3113 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-rw-rw-   0        0        0     5118 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-rw-rw-   0        0        0    11603 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/logging.py
--rw-rw-rw-   0        0        0    23739 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/misc.py
--rw-rw-rw-   0        0        0     1193 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/models.py
--rw-rw-rw-   0        0        0     2108 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-rw-rw-   0        0        0     4435 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-rw-rw-   0        0        0     9207 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-rw-rw-   0        0        0     9312 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-rw-rw-   0        0        0     8821 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-rw-rw-   0        0        0     1759 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/urls.py
--rw-rw-rw-   0        0        0     3456 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-rw-rw-   0        0        0     4549 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/utils/wheel.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.516027 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/vcs/
--rw-rw-rw-   0        0        0      596 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-rw-rw-   0        0        0     3519 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-rw-rw-   0        0        0    18121 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/vcs/git.py
--rw-rw-rw-   0        0        0     5249 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-rw-rw-   0        0        0    11729 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-rw-rw-   0        0        0    22811 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-rw-rw-   0        0        0    11842 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_internal/wheel_builder.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.533027 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/
--rw-rw-rw-   0        0        0     4993 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.561028 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/cachecontrol/
--rw-rw-rw-   0        0        0      676 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-rw-rw-   0        0        0     1737 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-rw-rw-   0        0        0     6392 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-rw-rw-   0        0        0     1952 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.579028 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
--rw-rw-rw-   0        0        0      303 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-rw-rw-   0        0        0     5352 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-rw-rw-   0        0        0     1386 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-rw-rw-   0        0        0    18384 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-rw-rw-   0        0        0     4292 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-rw-rw-   0        0        0     4828 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-rw-rw-   0        0        0     7173 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-rw-rw-   0        0        0     1417 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.586039 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/certifi/
--rw-rw-rw-   0        0        0       94 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-rw-rw-   0        0        0      255 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-rw-rw-   0        0        0     4279 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/certifi/core.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.707029 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/
--rw-rw-rw-   0        0        0     4797 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-rw-rw-   0        0        0    31274 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-rw-rw-   0        0        0     1763 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-rw-rw-   0        0        0    10032 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-rw-rw-   0        0        0     3915 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-rw-rw-   0        0        0     5420 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.710027 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/cli/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-rw-rw-   0        0        0     3242 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-rw-rw-   0        0        0     3732 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-rw-rw-   0        0        0      542 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-rw-rw-   0        0        0     1860 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-rw-rw-   0        0        0     1683 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-rw-rw-   0        0        0     4006 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-rw-rw-   0        0        0    12176 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-rw-rw-   0        0        0     3934 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-rw-rw-   0        0        0    13566 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-rw-rw-   0        0        0     1753 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-rw-rw-   0        0        0    36913 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-rw-rw-   0        0        0     1753 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-rw-rw-   0        0        0    20735 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-rw-rw-   0        0        0     1759 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-rw-rw-   0        0        0    14537 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-rw-rw-   0        0        0    25796 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-rw-rw-   0        0        0    42498 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-rw-rw-   0        0        0     1752 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-rw-rw-   0        0        0    27055 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-rw-rw-   0        0        0   104562 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-rw-rw-   0        0        0    98484 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-rw-rw-   0        0        0    98196 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-rw-rw-   0        0        0   101363 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-rw-rw-   0        0        0   128035 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-rw-rw-   0        0        0   102774 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-rw-rw-   0        0        0    95372 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-rw-rw-   0        0        0     5380 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-rw-rw-   0        0        0     6077 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-rw-rw-   0        0        0     3715 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-rw-rw-   0        0        0     2131 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-rw-rw-   0        0        0    30391 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.713029 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/metadata/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-rw-rw-   0        0        0    13560 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-rw-rw-   0        0        0      402 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/resultdict.py
--rw-rw-rw-   0        0        0     6400 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-rw-rw-   0        0        0     4137 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-rw-rw-   0        0        0     4007 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-rw-rw-   0        0        0    14848 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-rw-rw-   0        0        0     8505 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-rw-rw-   0        0        0     2812 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-rw-rw-   0        0        0      244 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/chardet/version.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.759027 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/
--rw-rw-rw-   0        0        0      266 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-rw-rw-   0        0        0     2522 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-rw-rw-   0        0        0    11128 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-rw-rw-   0        0        0     3325 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.927026 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/tests/
--rw-rw-rw-   0        0        0       75 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-rw-rw-   0        0        0     2839 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-rw-rw-   0        0        0    10678 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-rw-rw-   0        0        0     6741 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-rw-rw-   0        0        0     1866 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-rw-rw-   0        0        0     1079 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-rw-rw-   0        0        0     3709 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-rw-rw-   0        0        0     6181 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-rw-rw-   0        0        0     7134 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.066028 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distlib/
--rw-rw-rw-   0        0        0      581 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-rw-rw-   0        0        0    41259 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-rw-rw-   0        0        0    51697 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-rw-rw-   0        0        0    20834 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-rw-rw-   0        0        0    51991 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-rw-rw-   0        0        0    14811 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-rw-rw-   0        0        0     5058 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-rw-rw-   0        0        0    39801 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-rw-rw-   0        0        0    10820 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-rw-rw-   0        0        0    18102 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rw-rw-rw-   0        0        0    66262 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-rw-rw-   0        0        0    23513 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distlib/version.py
--rw-rw-rw-   0        0        0    43898 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.077029 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distro/
--rw-rw-rw-   0        0        0      981 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
--rw-rw-rw-   0        0        0       64 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
--rw-rw-rw-   0        0        0    49330 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/distro/distro.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.108029 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/idna/
--rw-rw-rw-   0        0        0      849 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-rw-rw-   0        0        0     3374 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-rw-rw-   0        0        0      321 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-rw-rw-   0        0        0    12950 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/idna/core.py
--rw-rw-rw-   0        0        0    44375 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-rw-rw-   0        0        0     1881 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-rw-rw-   0        0        0       21 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-rw-rw-   0        0        0   206539 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.114027 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/msgpack/
--rw-rw-rw-   0        0        0     1132 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-rw-rw-   0        0        0     1081 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-rw-rw-   0        0        0     6079 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-rw-rw-   0        0        0    34544 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.142027 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8487 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4676 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.144028 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pkg_resources/
--rw-rw-rw-   0        0        0   109364 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.160027 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/platformdirs/
--rw-rw-rw-   0        0        0    20155 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-rw-rw-   0        0        0     1476 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-rw-rw-   0        0        0     7211 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-rw-rw-   0        0        0     7132 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-rw-rw-   0        0        0     3678 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-rw-rw-   0        0        0     8809 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-rw-rw-   0        0        0      160 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-rw-rw-   0        0        0     9573 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.218027 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/
--rw-rw-rw-   0        0        0     2983 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-rw-rw-   0        0        0      353 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-rw-rw-   0        0        0    23685 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-rw-rw-   0        0        0     1697 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/console.py
--rw-rw-rw-   0        0        0     1938 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.229030 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/filters/
--rw-rw-rw-   0        0        0    40386 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-rw-rw-   0        0        0     4178 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.312028 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/
--rw-rw-rw-   0        0        0     5424 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-rw-rw-   0        0        0     4176 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-rw-rw-   0        0        0     3314 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-rw-rw-   0        0        0     5094 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-rw-rw-   0        0        0    35610 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-rw-rw-   0        0        0    21938 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-rw-rw-   0        0        0     4981 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-rw-rw-   0        0        0    19351 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-rw-rw-   0        0        0     5073 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-rw-rw-   0        0        0     2212 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-rw-rw-   0        0        0     5014 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-rw-rw-   0        0        0     7335 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-rw-rw-   0        0        0     4674 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-rw-rw-   0        0        0    11753 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-rw-rw-   0        0        0    34618 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.344028 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/lexers/
--rw-rw-rw-   0        0        0    12130 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-rw-rw-   0        0        0    72281 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-rw-rw-   0        0        0    53424 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-rw-rw-   0        0        0      986 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-rw-rw-   0        0        0     2591 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-rw-rw-   0        0        0     3072 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-rw-rw-   0        0        0     3092 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-rw-rw-   0        0        0     6882 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-rw-rw-   0        0        0     6257 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/style.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.346029 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/styles/
--rw-rw-rw-   0        0        0     3700 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-rw-rw-   0        0        0     6184 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/token.py
--rw-rw-rw-   0        0        0    63223 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-rw-rw-   0        0        0    10230 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pygments/util.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.396028 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9116 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6567 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    13387 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   224445 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.398028 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    24215 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9523 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    38646 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    26692 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13488 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10646 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     8670 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.404029 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/
--rw-rw-rw-   0        0        0      491 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-rw-rw-   0        0        0      138 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-rw-rw-   0        0        0    11920 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.418026 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/
--rw-rw-rw-   0        0        0      546 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-rw-rw-   0        0        0    10927 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.502027 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/
--rw-rw-rw-   0        0        0     5169 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-rw-rw-   0        0        0      435 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-rw-rw-   0        0        0     1495 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-rw-rw-   0        0        0    19697 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-rw-rw-   0        0        0     6449 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/api.py
--rw-rw-rw-   0        0        0    10187 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-rw-rw-   0        0        0      575 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-rw-rw-   0        0        0     1286 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-rw-rw-   0        0        0    18560 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-rw-rw-   0        0        0     3823 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-rw-rw-   0        0        0     3879 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/help.py
--rw-rw-rw-   0        0        0      733 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-rw-rw-   0        0        0    35288 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/models.py
--rw-rw-rw-   0        0        0      695 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-rw-rw-   0        0        0    30373 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-rw-rw-   0        0        0     4235 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-rw-rw-   0        0        0     2912 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-rw-rw-   0        0        0    33460 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/requests/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.515028 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/resolvelib/
--rw-rw-rw-   0        0        0      537 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.518029 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-rw-rw-   0        0        0      156 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-rw-rw-   0        0        0     5871 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-rw-rw-   0        0        0     1601 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-rw-rw-   0        0        0    20511 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-rw-rw-   0        0        0     4963 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.942760 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/
--rw-rw-rw-   0        0        0     6090 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
--rw-rw-rw-   0        0        0     8478 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
--rw-rw-rw-   0        0        0    10096 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-rw-rw-   0        0        0   140235 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-rw-rw-   0        0        0     1064 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-rw-rw-   0        0        0     2100 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-rw-rw-   0        0        0      265 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
--rw-rw-rw-   0        0        0      799 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_fileno.py
--rw-rw-rw-   0        0        0     9695 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-rw-rw-   0        0        0     3225 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-rw-rw-   0        0        0     1236 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
--rw-rw-rw-   0        0        0     1387 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_null_file.py
--rw-rw-rw-   0        0        0     7063 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-rw-rw-   0        0        0      423 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
--rw-rw-rw-   0        0        0     5472 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-rw-rw-   0        0        0    19919 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-rw-rw-   0        0        0      351 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
--rw-rw-rw-   0        0        0      417 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
--rw-rw-rw-   0        0        0    22820 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-rw-rw-   0        0        0     1926 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
--rw-rw-rw-   0        0        0     2783 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-rw-rw-   0        0        0     1840 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-rw-rw-   0        0        0      890 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/abc.py
--rw-rw-rw-   0        0        0    10368 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/align.py
--rw-rw-rw-   0        0        0     6906 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
--rw-rw-rw-   0        0        0     3264 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/bar.py
--rw-rw-rw-   0        0        0     9842 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/box.py
--rw-rw-rw-   0        0        0     4509 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/cells.py
--rw-rw-rw-   0        0        0    18224 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/color.py
--rw-rw-rw-   0        0        0     1054 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-rw-rw-   0        0        0     7131 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/columns.py
--rw-rw-rw-   0        0        0    99218 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/console.py
--rw-rw-rw-   0        0        0     1288 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
--rw-rw-rw-   0        0        0     5497 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/containers.py
--rw-rw-rw-   0        0        0     6630 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/control.py
--rw-rw-rw-   0        0        0     8082 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-rw-rw-   0        0        0      972 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-rw-rw-   0        0        0     2501 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
--rw-rw-rw-   0        0        0      642 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/errors.py
--rw-rw-rw-   0        0        0     1683 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-rw-rw-   0        0        0     2508 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
--rw-rw-rw-   0        0        0     9584 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-rw-rw-   0        0        0     5032 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/json.py
--rw-rw-rw-   0        0        0     3252 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-rw-rw-   0        0        0    14007 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/layout.py
--rw-rw-rw-   0        0        0    14273 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/live.py
--rw-rw-rw-   0        0        0     3667 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
--rw-rw-rw-   0        0        0    11903 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/logging.py
--rw-rw-rw-   0        0        0     8198 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/markup.py
--rw-rw-rw-   0        0        0     5305 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/measure.py
--rw-rw-rw-   0        0        0     4970 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/padding.py
--rw-rw-rw-   0        0        0      828 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/pager.py
--rw-rw-rw-   0        0        0     3396 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/palette.py
--rw-rw-rw-   0        0        0    10574 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/panel.py
--rw-rw-rw-   0        0        0    35852 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
--rw-rw-rw-   0        0        0    59706 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/progress.py
--rw-rw-rw-   0        0        0     8165 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-rw-rw-   0        0        0    11303 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
--rw-rw-rw-   0        0        0     1391 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
--rw-rw-rw-   0        0        0      166 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/region.py
--rw-rw-rw-   0        0        0     4431 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/repr.py
--rw-rw-rw-   0        0        0     4602 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/rule.py
--rw-rw-rw-   0        0        0     2843 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/scope.py
--rw-rw-rw-   0        0        0     1591 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/screen.py
--rw-rw-rw-   0        0        0    24247 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/segment.py
--rw-rw-rw-   0        0        0     4339 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
--rw-rw-rw-   0        0        0     4425 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/status.py
--rw-rw-rw-   0        0        0    27073 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/style.py
--rw-rw-rw-   0        0        0     1258 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/styled.py
--rw-rw-rw-   0        0        0    35173 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
--rw-rw-rw-   0        0        0    39684 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/table.py
--rw-rw-rw-   0        0        0     3370 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-rw-rw-   0        0        0    45525 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/text.py
--rw-rw-rw-   0        0        0     3777 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/theme.py
--rw-rw-rw-   0        0        0      102 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/themes.py
--rw-rw-rw-   0        0        0    29604 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
--rw-rw-rw-   0        0        0     9169 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/rich/tree.py
--rw-rw-rw-   0        0        0    34549 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/six.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.976944 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tenacity/
--rw-rw-rw-   0        0        0    20493 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-rw-rw-   0        0        0     3551 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-rw-rw-   0        0        0     2179 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-rw-rw-   0        0        0     1682 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-rw-rw-   0        0        0     1562 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-rw-rw-   0        0        0     2372 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-rw-rw-   0        0        0     1383 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-rw-rw-   0        0        0     8746 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-rw-rw-   0        0        0     3086 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-rw-rw-   0        0        0     2142 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-rw-rw-   0        0        0     8024 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:18.983174 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tomli/
--rw-rw-rw-   0        0        0      396 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-rw-rw-   0        0        0    22633 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-rw-rw-   0        0        0     2943 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
--rw-rw-rw-   0        0        0      254 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.034016 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/truststore/
--rw-rw-rw-   0        0        0      403 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/truststore/__init__.py
--rw-rw-rw-   0        0        0     9893 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/truststore/_api.py
--rw-rw-rw-   0        0        0    17694 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/truststore/_macos.py
--rw-rw-rw-   0        0        0     2324 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/truststore/_openssl.py
--rw-rw-rw-   0        0        0     1130 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/truststore/_ssl_constants.py
--rw-rw-rw-   0        0        0    17468 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/truststore/_windows.py
--rw-rw-rw-   0        0        0   111130 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.066934 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/
--rw-rw-rw-   0        0        0     3333 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-rw-rw-   0        0        0    10811 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-rw-rw-   0        0        0       64 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-rw-rw-   0        0        0    20300 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-rw-rw-   0        0        0    39990 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.122934 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-rw-rw-   0        0        0      957 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.128935 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-rw-rw-   0        0        0    17632 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-rw-rw-   0        0        0    13922 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-rw-rw-   0        0        0    11036 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-rw-rw-   0        0        0     4528 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-rw-rw-   0        0        0    17081 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-rw-rw-   0        0        0    34448 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-rw-rw-   0        0        0     7097 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-rw-rw-   0        0        0     8217 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-rw-rw-   0        0        0     8579 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-rw-rw-   0        0        0     2440 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.131936 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/packages/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.142934 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-rw-rw-   0        0        0     1417 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-rw-rw-   0        0        0     5343 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
--rw-rw-rw-   0        0        0    34665 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-rw-rw-   0        0        0    19752 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-rw-rw-   0        0        0     6691 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-rw-rw-   0        0        0    30641 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.178933 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/util/
--rw-rw-rw-   0        0        0     1155 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-rw-rw-   0        0        0     4901 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-rw-rw-   0        0        0     1605 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-rw-rw-   0        0        0      498 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-rw-rw-   0        0        0     3997 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-rw-rw-   0        0        0     3510 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-rw-rw-   0        0        0    22013 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-rw-rw-   0        0        0    17177 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-rw-rw-   0        0        0     5758 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-rw-rw-   0        0        0     6895 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-rw-rw-   0        0        0    10168 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-rw-rw-   0        0        0    14296 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-rw-rw-   0        0        0     5403 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-rw-rw-   0        0        0      493 2024-02-02 17:04:59.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/vendor.txt
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.190935 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/webencodings/
--rw-rw-rw-   0        0        0    10579 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-rw-rw-   0        0        0     8979 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-rw-rw-   0        0        0     1305 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-rw-rw-   0        0        0     6563 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-rw-rw-   0        0        0     4307 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:17.128015 iniUts-1.1.8/venv/Lib/site-packages/pip-23.3.2.dist-info/
--rw-rw-rw-   0        0        0    10286 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip-23.3.2.dist-info/AUTHORS.txt
--rw-rw-rw-   0        0        0     1093 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip-23.3.2.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0      125 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip-23.3.2.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2024-02-02 17:05:00.000000 iniUts-1.1.8/venv/Lib/site-packages/pip-23.3.2.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.191933 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/
--rw-rw-rw-   0        0        0   108568 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.196935 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
--rw-rw-rw-   0        0        0    24701 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.248934 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/
--rw-rw-rw-   0        0        0      506 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-rw-rw-   0        0        0     4504 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-rw-rw-   0        0        0     2741 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-rw-rw-   0        0        0     2706 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-rw-rw-   0        0        0      884 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-rw-rw-   0        0        0     3494 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-rw-rw-   0        0        0     3886 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-rw-rw-   0        0        0     3566 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-rw-rw-   0        0        0     2836 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.264934 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-rw-rw-   0        0        0     5420 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-rw-rw-   0        0        0    13515 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.275931 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/
--rw-rw-rw-   0        0        0    15526 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.282933 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/
--rw-rw-rw-   0        0        0       83 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   132569 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-rw-rw-   0        0        0    18410 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.313933 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8496 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4706 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.344936 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9159 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6426 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213310 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.346937 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23668 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9023 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39129 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25341 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13402 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10787 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-rw-rw-   0        0        0     8425 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.348934 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/extern/
--rw-rw-rw-   0        0        0     2426 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/pkg_resources/extern/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.621936 iniUts-1.1.8/venv/Lib/site-packages/setuptools/
--rw-rw-rw-   0        0        0     8429 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/__init__.py
--rw-rw-rw-   0        0        0      218 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_deprecation_warning.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.776008 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/
--rw-rw-rw-   0        0        0      537 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/__init__.py
--rw-rw-rw-   0        0        0     1330 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/_collections.py
--rw-rw-rw-   0        0        0      411 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/_functools.py
--rw-rw-rw-   0        0        0      239 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
--rw-rw-rw-   0        0        0    19672 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-rw-rw-   0        0        0     8603 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
--rw-rw-rw-   0        0        0    14789 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-rw-rw-   0        0        0    47369 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
--rw-rw-rw-   0        0        0    17973 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/cmd.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.835004 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/
--rw-rw-rw-   0        0        0      430 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
--rw-rw-rw-   0        0        0     1614 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-rw-rw-   0        0        0     5441 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
--rw-rw-rw-   0        0        0     4701 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-rw-rw-   0        0        0    22051 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-rw-rw-   0        0        0     5617 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/build.py
--rw-rw-rw-   0        0        0     7728 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
--rw-rw-rw-   0        0        0    31558 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
--rw-rw-rw-   0        0        0    16568 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
--rw-rw-rw-   0        0        0     5624 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-rw-rw-   0        0        0     4888 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/check.py
--rw-rw-rw-   0        0        0     2603 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
--rw-rw-rw-   0        0        0    13137 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/config.py
--rw-rw-rw-   0        0        0    30221 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/install.py
--rw-rw-rw-   0        0        0     2779 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
--rw-rw-rw-   0        0        0     2785 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-rw-rw-   0        0        0     1189 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
--rw-rw-rw-   0        0        0     8434 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
--rw-rw-rw-   0        0        0     1936 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-rw-rw-   0        0        0      672 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
--rw-rw-rw-   0        0        0    11765 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/register.py
--rw-rw-rw-   0        0        0    19241 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
--rw-rw-rw-   0        0        0     7477 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
--rw-rw-rw-   0        0        0     4920 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/config.py
--rw-rw-rw-   0        0        0     9451 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/core.py
--rw-rw-rw-   0        0        0    12537 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-rw-rw-   0        0        0      139 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/debug.py
--rw-rw-rw-   0        0        0     3423 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
--rw-rw-rw-   0        0        0     8082 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
--rw-rw-rw-   0        0        0    50186 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/dist.py
--rw-rw-rw-   0        0        0     3589 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/errors.py
--rw-rw-rw-   0        0        0    10270 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/extension.py
--rw-rw-rw-   0        0        0    17910 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-rw-rw-   0        0        0     8226 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/file_util.py
--rw-rw-rw-   0        0        0    13713 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/filelist.py
--rw-rw-rw-   0        0        0     1972 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/log.py
--rw-rw-rw-   0        0        0    30235 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-rw-rw-   0        0        0    23602 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
--rw-rw-rw-   0        0        0      217 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
--rw-rw-rw-   0        0        0      639 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/py39compat.py
--rw-rw-rw-   0        0        0     3517 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/spawn.py
--rw-rw-rw-   0        0        0    18858 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
--rw-rw-rw-   0        0        0    12096 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/text_file.py
--rw-rw-rw-   0        0        0    15641 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
--rw-rw-rw-   0        0        0    18128 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/util.py
--rw-rw-rw-   0        0        0    12952 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/version.py
--rw-rw-rw-   0        0        0     5248 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
--rw-rw-rw-   0        0        0     1972 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_entry_points.py
--rw-rw-rw-   0        0        0     2392 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_imp.py
--rw-rw-rw-   0        0        0     1311 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_importlib.py
--rw-rw-rw-   0        0        0      675 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_itertools.py
--rw-rw-rw-   0        0        0      749 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_path.py
--rw-rw-rw-   0        0        0      501 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_reqs.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.864003 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.913004 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/
--rw-rw-rw-   0        0        0    30130 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-rw-rw-   0        0        0     1862 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-rw-rw-   0        0        0      743 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-rw-rw-   0        0        0     1828 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-rw-rw-   0        0        0     2895 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-rw-rw-   0        0        0     2068 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-rw-rw-   0        0        0     1154 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-rw-rw-   0        0        0     2166 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.950003 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/
--rw-rw-rw-   0        0        0      506 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-rw-rw-   0        0        0     4504 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-rw-rw-   0        0        0     2741 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-rw-rw-   0        0        0     2706 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-rw-rw-   0        0        0      884 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-rw-rw-   0        0        0     3494 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-rw-rw-   0        0        0     3886 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-rw-rw-   0        0        0     3566 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-rw-rw-   0        0        0     2836 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.977003 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/jaraco/
--rw-rw-rw-   0        0        0        0 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-rw-rw-   0        0        0     5420 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
--rw-rw-rw-   0        0        0    13512 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.984003 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/
--rw-rw-rw-   0        0        0    15517 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.997002 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/more_itertools/
--rw-rw-rw-   0        0        0       82 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   117959 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-rw-rw-   0        0        0    16256 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-rw-rw-   0        0        0    15130 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:20.035004 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8493 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4700 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:20.062003 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9159 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6426 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213310 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:20.063005 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23668 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9023 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39129 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25341 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13402 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10787 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:20.093003 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/tomli/
--rw-rw-rw-   0        0        0      396 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-rw-rw-   0        0        0    22633 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-rw-rw-   0        0        0     2943 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
--rw-rw-rw-   0        0        0      254 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
--rw-rw-rw-   0        0        0    87149 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
--rw-rw-rw-   0        0        0     8425 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/_vendor/zipp.py
--rw-rw-rw-   0        0        0     7346 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/archive_util.py
--rw-rw-rw-   0        0        0    19539 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/build_meta.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:20.208802 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/
--rw-rw-rw-   0        0        0      396 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/__init__.py
--rw-rw-rw-   0        0        0     2381 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/alias.py
--rw-rw-rw-   0        0        0    16623 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/bdist_egg.py
--rw-rw-rw-   0        0        0     1182 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
--rw-rw-rw-   0        0        0     6595 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/build.py
--rw-rw-rw-   0        0        0     4415 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/build_clib.py
--rw-rw-rw-   0        0        0    15821 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/build_ext.py
--rw-rw-rw-   0        0        0    14115 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/build_py.py
--rw-rw-rw-   0        0        0     7012 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/develop.py
--rw-rw-rw-   0        0        0     4800 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/dist_info.py
--rw-rw-rw-   0        0        0    85662 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/easy_install.py
--rw-rw-rw-   0        0        0    31188 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/editable_wheel.py
--rw-rw-rw-   0        0        0    26795 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/egg_info.py
--rw-rw-rw-   0        0        0     5163 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/install.py
--rw-rw-rw-   0        0        0     2226 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/install_egg_info.py
--rw-rw-rw-   0        0        0     3875 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/install_lib.py
--rw-rw-rw-   0        0        0     2612 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/install_scripts.py
--rw-rw-rw-   0        0        0     4946 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/py36compat.py
--rw-rw-rw-   0        0        0      468 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/register.py
--rw-rw-rw-   0        0        0     2128 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/rotate.py
--rw-rw-rw-   0        0        0      658 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/saveopts.py
--rw-rw-rw-   0        0        0     7071 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/sdist.py
--rw-rw-rw-   0        0        0     5086 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/setopt.py
--rw-rw-rw-   0        0        0     8102 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/test.py
--rw-rw-rw-   0        0        0      462 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/upload.py
--rw-rw-rw-   0        0        0     7494 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/command/upload_docs.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:20.215800 iniUts-1.1.8/venv/Lib/site-packages/setuptools/config/
--rw-rw-rw-   0        0        0     1121 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/config/__init__.py
--rw-rw-rw-   0        0        0    13398 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:20.243799 iniUts-1.1.8/venv/Lib/site-packages/setuptools/config/_validate_pyproject/
--rw-rw-rw-   0        0        0     1038 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-rw-rw-   0        0        0    11266 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-rw-rw-   0        0        0     1153 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-rw-rw-   0        0        0     1612 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-rw-rw-   0        0        0   269900 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-rw-rw-   0        0        0     8736 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-rw-rw-   0        0        0    16319 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/config/expand.py
--rw-rw-rw-   0        0        0    19304 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
--rw-rw-rw-   0        0        0    25198 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/config/setupcfg.py
--rw-rw-rw-   0        0        0      949 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/dep_util.py
--rw-rw-rw-   0        0        0     5499 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/depends.py
--rw-rw-rw-   0        0        0    20799 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/discovery.py
--rw-rw-rw-   0        0        0    45578 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/dist.py
--rw-rw-rw-   0        0        0     2464 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/errors.py
--rw-rw-rw-   0        0        0     5591 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/extension.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:20.245800 iniUts-1.1.8/venv/Lib/site-packages/setuptools/extern/
--rw-rw-rw-   0        0        0     2512 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/extern/__init__.py
--rw-rw-rw-   0        0        0     4873 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/glob.py
--rw-rw-rw-   0        0        0     3824 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/installer.py
--rw-rw-rw-   0        0        0      812 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/launch.py
--rw-rw-rw-   0        0        0     1210 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/logging.py
--rw-rw-rw-   0        0        0     4857 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/monkey.py
--rw-rw-rw-   0        0        0    47724 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/msvc.py
--rw-rw-rw-   0        0        0     3093 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/namespaces.py
--rw-rw-rw-   0        0        0    40020 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/package_index.py
--rw-rw-rw-   0        0        0      245 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/py34compat.py
--rw-rw-rw-   0        0        0    14348 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/sandbox.py
--rw-rw-rw-   0        0        0      941 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/unicode_utils.py
--rw-rw-rw-   0        0        0      144 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/version.py
--rw-rw-rw-   0        0        0     8376 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/wheel.py
--rw-rw-rw-   0        0        0      718 2024-02-02 17:04:37.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools/windows_support.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:56:19.674935 iniUts-1.1.8/venv/Lib/site-packages/setuptools-65.5.0.dist-info/
--rw-rw-rw-   0        0        0     2740 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools-65.5.0.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2024-02-02 17:04:38.000000 iniUts-1.1.8/venv/Lib/site-packages/setuptools-65.5.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 13:02:12.222464 iniUts-1.1.9/
+-rw-rw-rw-   0        0        0      465 2023-04-28 18:31:34.000000 iniUts-1.1.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-04-26 17:09:25.000000 iniUts-1.1.9/LICENCE.txt
+-rw-rw-rw-   0        0        0       56 2024-05-27 13:00:37.000000 iniUts-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4746 2024-05-27 13:02:12.222464 iniUts-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3747 2024-05-27 13:01:20.000000 iniUts-1.1.9/README.md
+-rw-rw-rw-   0        0        0      204 2024-05-27 12:54:53.000000 iniUts-1.1.9/commands.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 13:02:12.174464 iniUts-1.1.9/iniUts/
+-rw-rw-rw-   0        0        0     6314 2024-05-27 12:55:25.000000 iniUts-1.1.9/iniUts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:02:12.220463 iniUts-1.1.9/iniUts.egg-info/
+-rw-rw-rw-   0        0        0     4746 2024-05-27 13:02:11.000000 iniUts-1.1.9/iniUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-27 13:02:12.000000 iniUts-1.1.9/iniUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 13:02:11.000000 iniUts-1.1.9/iniUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-27 13:02:11.000000 iniUts-1.1.9/iniUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1043 2024-05-27 12:55:47.000000 iniUts-1.1.9/run.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 13:02:12.223464 iniUts-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      742 2024-05-27 13:00:27.000000 iniUts-1.1.9/setup.py
```

### Comparing `iniUts-1.1.8/LICENCE.txt` & `iniUts-1.1.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `iniUts-1.1.8/PKG-INFO` & `iniUts-1.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iniUts
-Version: 1.1.8
+Version: 1.1.9
 Summary: Ini file manipulator
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: iniUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,18 @@
 #
 ### Installation
 
 ```sh
 pip install iniUts
 ```
 
+## GitHub
+https://github.com/ZdekPyPi/IniUts
+
+
 ## Usage
 #
 <!-- //==================================================== -->
 ## read
 ##### test.ini file
 ```ini
 [Person]
```

### Comparing `iniUts-1.1.8/README.md` & `iniUts-1.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 #
 ### Installation
 
 ```sh
 pip install iniUts
 ```
 
+## GitHub
+https://github.com/ZdekPyPi/IniUts
+
+
 ## Usage
 #
 <!-- //==================================================== -->
 ## read
 ##### test.ini file
 ```ini
 [Person]
```

### Comparing `iniUts-1.1.8/iniUts/__init__.py` & `iniUts-1.1.9/iniUts/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -147,59 +147,14 @@
         def wrap(function):
             self.section2DataClass(section,function,skip_missing,empty_as_null)
             return function
         return wrap
 
 
 
-ini = IniUts('prd_config.ini')
-#ini = IniUts('prd_config.ini','dev_config.ini',in_prd=False)
 
-#TODAS AS CHAVES DE DEV DEVE CONTER EM PRD
-
-
-# @ini.link('PERSON')
-# class Person():
-#     NAME   : str
-#     age    : int
-#     amount : float
-#     friends: tuple = ','
-#     dob    : datetime = "%Y-%m-%d"
-
-# pass
-# a = 1
-
-# @dataclass
-# class IPS():
-#    ip5   : bool
-
-# @dataclass
-# class IPS2():
-#    ip5   : str
-
-#import os
-#os.system("cls")
-
-#os.environ['ENV'] = 'PRD'
-
-#ini = IniUts('prd_config.ini')
-#ini = IniUts('prd_config.ini','dev_config.ini',in_prd=False)
-#ini.section2DataClass('PERSON',Person)
-#ini.section2DataClass('IPS',IPS)
-#ini.section2DataClass('IPS2',IPS2)
-#print(IPS2.ip5)
-
-#a  =1
-
-#print(ini.read("PERSON","NAME"))
-# ini.Section2Dict('IPS2')
-# # ini.section2DataClass('PERSON',Person)
-# # ini.section2DataClass('PERSON',Person)
-# # print(Person.NAME)
-
-#a  =1
```

### Comparing `iniUts-1.1.8/iniUts.egg-info/PKG-INFO` & `iniUts-1.1.9/iniUts.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iniUts
-Version: 1.1.8
+Version: 1.1.9
 Summary: Ini file manipulator
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: iniUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,18 @@
 #
 ### Installation
 
 ```sh
 pip install iniUts
 ```
 
+## GitHub
+https://github.com/ZdekPyPi/IniUts
+
+
 ## Usage
 #
 <!-- //==================================================== -->
 ## read
 ##### test.ini file
 ```ini
 [Person]
```

### Comparing `iniUts-1.1.8/setup.py` & `iniUts-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='iniUts',
-  version='1.1.8',
+  version='1.1.9',
   description='Ini file manipulator',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

