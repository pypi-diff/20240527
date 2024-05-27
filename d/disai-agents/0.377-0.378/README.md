# Comparing `tmp/disai-agents-0.377.tar.gz` & `tmp/disai-agents-0.378.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disai-agents-0.377.tar", last modified: Mon May 27 09:03:36 2024, max compression
+gzip compressed data, was "disai-agents-0.378.tar", last modified: Mon May 27 09:34:11 2024, max compression
```

## Comparing `disai-agents-0.377.tar` & `disai-agents-0.378.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 09:03:36.926358 disai-agents-0.377/
--rw-rw-rw-   0        0        0      280 2024-05-27 09:03:36.926358 disai-agents-0.377/PKG-INFO
--rw-rw-rw-   0        0        0       34 2024-05-27 08:13:54.000000 disai-agents-0.377/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 09:03:36.894722 disai-agents-0.377/disai-agents/
--rw-rw-rw-   0        0        0      147 2024-05-27 09:01:23.000000 disai-agents-0.377/disai-agents/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 09:03:36.898351 disai-agents-0.377/disai-agents/disai_jazz/
--rw-rw-rw-   0        0        0      197 2024-05-25 13:23:39.000000 disai-agents-0.377/disai-agents/disai_jazz/__init__.py
--rw-rw-rw-   0        0        0      413 2024-05-25 13:23:37.000000 disai-agents-0.377/disai-agents/disai_jazz/agent.py
--rw-rw-rw-   0        0        0      537 2024-05-25 13:23:41.000000 disai-agents-0.377/disai-agents/disai_jazz/arch.py
--rw-rw-rw-   0        0        0     3098 2024-05-27 07:56:48.000000 disai-agents-0.377/disai-agents/disai_jazz/openai_model.py
--rw-rw-rw-   0        0        0      145 2024-05-25 13:23:46.000000 disai-agents-0.377/disai-agents/disai_jazz/task.py
--rw-rw-rw-   0        0        0      332 2024-05-25 13:23:48.000000 disai-agents-0.377/disai-agents/disai_jazz/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-27 09:03:36.899351 disai-agents-0.377/disai-agents/disai_jazza/
--rw-rw-rw-   0        0        0       76 2024-05-27 09:01:10.000000 disai-agents-0.377/disai-agents/disai_jazza/__init__.py
--rw-rw-rw-   0        0        0      121 2024-05-27 09:01:16.000000 disai-agents-0.377/disai-agents/disai_jazza/arch.py
-drwxrwxrwx   0        0        0        0 2024-05-27 09:03:36.925352 disai-agents-0.377/disai_agents.egg-info/
--rw-rw-rw-   0        0        0      280 2024-05-27 09:03:36.000000 disai-agents-0.377/disai_agents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-05-27 09:03:36.000000 disai-agents-0.377/disai_agents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 09:03:36.000000 disai-agents-0.377/disai_agents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-27 09:03:36.000000 disai-agents-0.377/disai_agents.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-27 09:03:36.000000 disai-agents-0.377/disai_agents.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 09:03:36.927366 disai-agents-0.377/setup.cfg
--rw-rw-rw-   0        0        0      448 2024-05-27 09:02:42.000000 disai-agents-0.377/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:34:11.071807 disai-agents-0.378/
+-rw-rw-rw-   0        0        0      280 2024-05-27 09:34:11.071807 disai-agents-0.378/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2024-05-27 08:13:54.000000 disai-agents-0.378/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 09:34:11.044996 disai-agents-0.378/disai-agents/
+-rw-rw-rw-   0        0        0      147 2024-05-27 09:01:23.000000 disai-agents-0.378/disai-agents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:34:11.048022 disai-agents-0.378/disai-agents/disai_jazz/
+-rw-rw-rw-   0        0        0      197 2024-05-25 13:23:39.000000 disai-agents-0.378/disai-agents/disai_jazz/__init__.py
+-rw-rw-rw-   0        0        0      413 2024-05-25 13:23:37.000000 disai-agents-0.378/disai-agents/disai_jazz/agent.py
+-rw-rw-rw-   0        0        0      537 2024-05-25 13:23:41.000000 disai-agents-0.378/disai-agents/disai_jazz/arch.py
+-rw-rw-rw-   0        0        0     3098 2024-05-27 07:56:48.000000 disai-agents-0.378/disai-agents/disai_jazz/openai_model.py
+-rw-rw-rw-   0        0        0      145 2024-05-25 13:23:46.000000 disai-agents-0.378/disai-agents/disai_jazz/task.py
+-rw-rw-rw-   0        0        0      332 2024-05-25 13:23:48.000000 disai-agents-0.378/disai-agents/disai_jazz/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:34:11.048996 disai-agents-0.378/disai-agents/disai_jazza/
+-rw-rw-rw-   0        0        0       76 2024-05-27 09:01:10.000000 disai-agents-0.378/disai-agents/disai_jazza/__init__.py
+-rw-rw-rw-   0        0        0      121 2024-05-27 09:01:16.000000 disai-agents-0.378/disai-agents/disai_jazza/arch.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:34:11.070834 disai-agents-0.378/disai_agents.egg-info/
+-rw-rw-rw-   0        0        0      280 2024-05-27 09:34:10.000000 disai-agents-0.378/disai_agents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-05-27 09:34:11.000000 disai-agents-0.378/disai_agents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 09:34:10.000000 disai-agents-0.378/disai_agents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-27 09:34:10.000000 disai-agents-0.378/disai_agents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-27 09:34:10.000000 disai-agents-0.378/disai_agents.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 09:34:11.072805 disai-agents-0.378/setup.cfg
+-rw-rw-rw-   0        0        0      472 2024-05-27 09:33:40.000000 disai-agents-0.378/setup.py
```

### Comparing `disai-agents-0.377/disai-agents/disai_jazz/arch.py` & `disai-agents-0.378/disai-agents/disai_jazz/arch.py`

 * *Files identical despite different names*

### Comparing `disai-agents-0.377/disai-agents/disai_jazz/openai_model.py` & `disai-agents-0.378/disai-agents/disai_jazz/openai_model.py`

 * *Files identical despite different names*
