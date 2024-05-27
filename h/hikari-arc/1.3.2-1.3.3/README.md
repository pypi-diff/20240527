# Comparing `tmp/hikari_arc-1.3.2.tar.gz` & `tmp/hikari_arc-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_arc-1.3.2.tar", last modified: Fri May 24 22:41:56 2024, max compression
+gzip compressed data, was "hikari_arc-1.3.3.tar", last modified: Mon May 27 13:13:15 2024, max compression
```

## Comparing `hikari_arc-1.3.2.tar` & `hikari_arc-1.3.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.375348 hikari_arc-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-24 22:41:56.375348 hikari_arc-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.363348 hikari_arc-1.3.2/arc/
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.363348 hikari_arc-1.3.2/arc/abc/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54147 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28769 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/concurrency_limiting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/hookable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/option.py
--rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/abc/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17850 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.363348 hikari_arc-1.3.2/arc/command/
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.367348 hikari_arc-1.3.2/arc/command/option/
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.367348 hikari_arc-1.3.2/arc/command/option/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/custom/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/custom/member.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/mentionable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/option/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    35491 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/slash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/command/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.367348 hikari_arc-1.3.2/arc/context/
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/context/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)    39976 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/context/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.367348 hikari_arc-1.3.2/arc/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.367348 hikari_arc-1.3.2/arc/internal/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/sigparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/internal/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.371348 hikari_arc-1.3.2/arc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/utils/concurrency_limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.371348 hikari_arc-1.3.2/arc/utils/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/utils/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/utils/hooks/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/utils/hooks/limiters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/utils/loops.py
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/arc/utils/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/cron_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/doc_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.371348 hikari_arc-1.3.2/hikari_arc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-24 22:41:56.000000 hikari_arc-1.3.2/hikari_arc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-24 22:41:56.000000 hikari_arc-1.3.2/hikari_arc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 22:41:56.000000 hikari_arc-1.3.2/hikari_arc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 22:41:56.000000 hikari_arc-1.3.2/hikari_arc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-24 22:41:56.000000 hikari_arc-1.3.2/hikari_arc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-24 22:41:56.000000 hikari_arc-1.3.2/hikari_arc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/rest_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 22:41:56.375348 hikari_arc-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:41:56.371348 hikari_arc-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/tests/test_context_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/tests/test_di.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/tests/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/tests/test_sigparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-24 22:41:53.000000 hikari_arc-1.3.2/tests/test_slash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.210282 hikari_arc-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-27 13:13:15.210282 hikari_arc-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.194283 hikari_arc-1.3.3/arc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.198283 hikari_arc-1.3.3/arc/abc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54155 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28462 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/concurrency_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/hookable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/abc/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17850 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.198283 hikari_arc-1.3.3/arc/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.198283 hikari_arc-1.3.3/arc/command/option/
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.202283 hikari_arc-1.3.3/arc/command/option/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/custom/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/custom/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/mentionable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/option/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35491 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/slash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/command/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.202283 hikari_arc-1.3.3/arc/context/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/context/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39976 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.202283 hikari_arc-1.3.3/arc/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.202283 hikari_arc-1.3.3/arc/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/sigparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/internal/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.202283 hikari_arc-1.3.3/arc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/utils/concurrency_limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.206282 hikari_arc-1.3.3/arc/utils/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/utils/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/utils/hooks/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/utils/hooks/limiters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/utils/loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/arc/utils/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/cron_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/doc_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.206282 hikari_arc-1.3.3/hikari_arc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-27 13:13:15.000000 hikari_arc-1.3.3/hikari_arc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-27 13:13:15.000000 hikari_arc-1.3.3/hikari_arc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:13:15.000000 hikari_arc-1.3.3/hikari_arc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:13:15.000000 hikari_arc-1.3.3/hikari_arc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-27 13:13:15.000000 hikari_arc-1.3.3/hikari_arc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 13:13:15.000000 hikari_arc-1.3.3/hikari_arc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/rest_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:13:15.210282 hikari_arc-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:13:15.206282 hikari_arc-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/tests/test_context_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/tests/test_di.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/tests/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/tests/test_sigparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-27 13:13:11.000000 hikari_arc-1.3.3/tests/test_slash.py
```

### Comparing `hikari_arc-1.3.2/LICENSE` & `hikari_arc-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/PKG-INFO` & `hikari_arc-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-arc
-Version: 1.3.2
+Version: 1.3.3
 Summary: A command handler for hikari with a focus on type-safety and correctness.
 Home-page: https://github.com/hypergonial/hikari-arc
 Author: hypergonial
 Author-email: git@hypergonial.com
 Maintainer: hypergonial
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hikari_arc-1.3.2/README.md` & `hikari_arc-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/__init__.py` & `hikari_arc-1.3.3/arc/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/__main__.py` & `hikari_arc-1.3.3/arc/__main__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/abc/__init__.py` & `hikari_arc-1.3.3/arc/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/abc/client.py` & `hikari_arc-1.3.3/arc/abc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,16 +329,16 @@
             if ctx.is_valid:
                 await ctx.respond("❌ Something went wrong. Please contact the bot developer.")
 
     async def _create_overriding_ctx_for_command(self, ctx: Context[te.Self]) -> alluka.OverridingContext:
         inj_ctx = alluka.OverridingContext.from_client(self.injector)
 
         for hook in self._injection_hooks:
-            if inspect.iscoroutinefunction(hook):
-                await hook(ctx, inj_ctx)
+            if inspect.isawaitable(hook):
+                await hook(ctx, inj_ctx)  # type: ignore
             else:
                 hook(ctx, inj_ctx)
         return inj_ctx
 
     def _provide_command_locale(self, request: CommandLocaleRequest) -> LocaleResponse:
         """Provide a locale for a command."""
         if self._command_locale_provider is None:
```

### Comparing `hikari_arc-1.3.2/arc/abc/command.py` & `hikari_arc-1.3.3/arc/abc/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import abc
 import asyncio
-import inspect
 import typing as t
 
 import attr
 import hikari
 
 from arc.abc.concurrency_limiting import ConcurrencyLimiterProto, HasConcurrencyLimiter
 from arc.abc.error_handler import HasErrorHandler
@@ -545,18 +544,15 @@
         bool
             Whether the command should be aborted.
         """
         aborted = False
         try:
             hooks = command._resolve_hooks()
             for hook in hooks:
-                if inspect.iscoroutinefunction(hook):
-                    res = await ctx._injection_ctx.call_with_async_di(hook, ctx)
-                else:
-                    res = ctx._injection_ctx.call_with_di(hook, ctx)
+                res = await ctx._injection_ctx.call_with_async_di(hook, ctx)
 
                 res = t.cast(HookResult | None, res)
 
                 if res and res._abort:
                     aborted = True
         except Exception as e:
             aborted = True
@@ -565,18 +561,15 @@
         return aborted
 
     async def _handle_post_hooks(self, command: CallableCommandProto[ClientT], ctx: Context[ClientT]) -> None:
         """Handle all post-execution hooks for a command, and release the concurrency limiter if applicable."""
         try:
             post_hooks = command._resolve_post_hooks()
             for hook in post_hooks:
-                if inspect.iscoroutinefunction(hook):
-                    await ctx._injection_ctx.call_with_async_di(hook, ctx)
-                else:
-                    ctx._injection_ctx.call_with_di(hook, ctx)
+                await ctx._injection_ctx.call_with_async_di(hook, ctx)
         except Exception as e:
             await command._handle_exception(ctx, e)
         finally:
             if (limiter := command._resolve_concurrency_limiter()) is not None:
                 limiter.release(ctx)
 
     async def _handle_callback(
```

### Comparing `hikari_arc-1.3.2/arc/abc/concurrency_limiting.py` & `hikari_arc-1.3.3/arc/abc/concurrency_limiting.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/abc/error_handler.py` & `hikari_arc-1.3.3/arc/abc/error_handler.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/abc/hookable.py` & `hikari_arc-1.3.3/arc/abc/hookable.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/abc/limiter.py` & `hikari_arc-1.3.3/arc/abc/limiter.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/abc/option.py` & `hikari_arc-1.3.3/arc/abc/option.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/abc/plugin.py` & `hikari_arc-1.3.3/arc/abc/plugin.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/client.py` & `hikari_arc-1.3.3/arc/client.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/__init__.py` & `hikari_arc-1.3.3/arc/command/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/message.py` & `hikari_arc-1.3.3/arc/command/message.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/option/__init__.py` & `hikari_arc-1.3.3/arc/command/option/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/option/attachment.py` & `hikari_arc-1.3.3/arc/command/option/attachment.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/option/bool.py` & `hikari_arc-1.3.3/arc/command/option/bool.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/option/channel.py` & `hikari_arc-1.3.3/arc/command/option/channel.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/option/custom/color.py` & `hikari_arc-1.3.3/arc/command/option/custom/color.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/option/custom/member.py` & `hikari_arc-1.3.3/arc/command/option/custom/member.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/option/float.py` & `hikari_arc-1.3.3/arc/command/option/float.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/option/int.py` & `hikari_arc-1.3.3/arc/command/option/int.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/option/mentionable.py` & `hikari_arc-1.3.3/arc/command/option/mentionable.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/option/role.py` & `hikari_arc-1.3.3/arc/command/option/role.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/option/str.py` & `hikari_arc-1.3.3/arc/command/option/str.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/option/user.py` & `hikari_arc-1.3.3/arc/command/option/user.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/slash.py` & `hikari_arc-1.3.3/arc/command/slash.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/command/user.py` & `hikari_arc-1.3.3/arc/command/user.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/context/__init__.py` & `hikari_arc-1.3.3/arc/context/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/context/autocomplete.py` & `hikari_arc-1.3.3/arc/context/autocomplete.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/context/base.py` & `hikari_arc-1.3.3/arc/context/base.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/errors.py` & `hikari_arc-1.3.3/arc/errors.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/events.py` & `hikari_arc-1.3.3/arc/events.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/extension.py` & `hikari_arc-1.3.3/arc/extension.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/internal/__init__.py` & `hikari_arc-1.3.3/arc/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/internal/about.py` & `hikari_arc-1.3.3/arc/internal/about.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 
 __author__: t.Final[str] = "hypergonial"
 __author_email__: t.Final[str] = "git@hypergonial.com"
 __maintainer__: t.Final[str] = "hypergonial"
 __license__: t.Final[str] = "MIT"
 __url__: t.Final[str] = "https://github.com/hypergonial/hikari-arc"
-__version__: t.Final[str] = "1.3.2"
+__version__: t.Final[str] = "1.3.3"
 
 # MIT License
 #
 # Copyright (c) 2023-present hypergonial
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
```

### Comparing `hikari_arc-1.3.2/arc/internal/deprecation.py` & `hikari_arc-1.3.3/arc/internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/internal/options.py` & `hikari_arc-1.3.3/arc/internal/options.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/internal/sigparse.py` & `hikari_arc-1.3.3/arc/internal/sigparse.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/internal/sync.py` & `hikari_arc-1.3.3/arc/internal/sync.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/internal/types.py` & `hikari_arc-1.3.3/arc/internal/types.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/internal/version.py` & `hikari_arc-1.3.3/arc/internal/version.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/locale.py` & `hikari_arc-1.3.3/arc/locale.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/plugin.py` & `hikari_arc-1.3.3/arc/plugin.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/utils/__init__.py` & `hikari_arc-1.3.3/arc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/utils/concurrency_limiter.py` & `hikari_arc-1.3.3/arc/utils/concurrency_limiter.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/utils/hooks/__init__.py` & `hikari_arc-1.3.3/arc/utils/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/utils/hooks/basic.py` & `hikari_arc-1.3.3/arc/utils/hooks/basic.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/utils/hooks/limiters.py` & `hikari_arc-1.3.3/arc/utils/hooks/limiters.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/utils/loops.py` & `hikari_arc-1.3.3/arc/utils/loops.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/arc/utils/ratelimiter.py` & `hikari_arc-1.3.3/arc/utils/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/hikari_arc.egg-info/PKG-INFO` & `hikari_arc-1.3.3/hikari_arc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-arc
-Version: 1.3.2
+Version: 1.3.3
 Summary: A command handler for hikari with a focus on type-safety and correctness.
 Home-page: https://github.com/hypergonial/hikari-arc
 Author: hypergonial
 Author-email: git@hypergonial.com
 Maintainer: hypergonial
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hikari_arc-1.3.2/hikari_arc.egg-info/SOURCES.txt` & `hikari_arc-1.3.3/hikari_arc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/pyproject.toml` & `hikari_arc-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/setup.py` & `hikari_arc-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/tests/test_client.py` & `hikari_arc-1.3.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/tests/test_context_command.py` & `hikari_arc-1.3.3/tests/test_context_command.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/tests/test_di.py` & `hikari_arc-1.3.3/tests/test_di.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/tests/test_inheritance.py` & `hikari_arc-1.3.3/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/tests/test_options.py` & `hikari_arc-1.3.3/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/tests/test_sigparse.py` & `hikari_arc-1.3.3/tests/test_sigparse.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.2/tests/test_slash.py` & `hikari_arc-1.3.3/tests/test_slash.py`

 * *Files identical despite different names*

