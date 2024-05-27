# Comparing `tmp/foundationallm-0.7.5.tar.gz` & `tmp/foundationallm-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundationallm-0.7.5.tar", last modified: Thu May 23 12:19:31 2024, max compression
+gzip compressed data, was "foundationallm-0.7.6.tar", last modified: Mon May 27 10:08:46 2024, max compression
```

## Comparing `foundationallm-0.7.5.tar` & `foundationallm-0.7.6.tar`

### file list

```diff
@@ -1,31 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 12:19:31.470050 foundationallm-0.7.5/
--rw-rw-rw-   0        0        0      201 2024-05-07 13:15:07.000000 foundationallm-0.7.5/LICENSE
--rw-rw-rw-   0        0        0      633 2024-05-23 12:19:31.469045 foundationallm-0.7.5/PKG-INFO
--rw-rw-rw-   0        0        0       88 2024-05-23 11:31:53.000000 foundationallm-0.7.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 12:19:31.417898 foundationallm-0.7.5/foundationallm/
-drwxrwxrwx   0        0        0        0 2024-05-23 12:19:31.438540 foundationallm-0.7.5/foundationallm/config/
--rw-rw-rw-   0        0        0      177 2023-12-14 16:50:30.000000 foundationallm-0.7.5/foundationallm/config/__init__.py
--rw-rw-rw-   0        0        0     4874 2024-05-23 11:10:06.000000 foundationallm-0.7.5/foundationallm/config/configuration.py
--rw-rw-rw-   0        0        0      605 2023-12-14 16:50:30.000000 foundationallm-0.7.5/foundationallm/config/context.py
--rw-rw-rw-   0        0        0      378 2024-03-15 16:01:06.000000 foundationallm-0.7.5/foundationallm/config/environment_variables.py
--rw-rw-rw-   0        0        0      556 2023-12-14 16:50:30.000000 foundationallm-0.7.5/foundationallm/config/user_identity.py
-drwxrwxrwx   0        0        0        0 2024-05-23 12:19:31.418900 foundationallm-0.7.5/foundationallm/models/
-drwxrwxrwx   0        0        0        0 2024-05-23 12:19:31.453538 foundationallm-0.7.5/foundationallm/models/authentication/
--rw-rw-rw-   0        0        0       55 2024-05-07 13:15:07.000000 foundationallm-0.7.5/foundationallm/models/authentication/__init__.py
--rw-rw-rw-   0        0        0      157 2024-05-07 13:15:07.000000 foundationallm-0.7.5/foundationallm/models/authentication/authentication_types.py
-drwxrwxrwx   0        0        0        0 2024-05-23 12:19:31.465542 foundationallm-0.7.5/foundationallm/models/orchestration/
--rw-rw-rw-   0        0        0      402 2024-05-23 12:09:21.000000 foundationallm-0.7.5/foundationallm/models/orchestration/__init__.py
--rw-rw-rw-   0        0        0      272 2024-04-24 17:34:13.000000 foundationallm-0.7.5/foundationallm/models/orchestration/citation.py
--rw-rw-rw-   0        0        0      502 2024-05-07 13:15:07.000000 foundationallm-0.7.5/foundationallm/models/orchestration/completion_request_base.py
--rw-rw-rw-   0        0        0      523 2024-04-24 17:34:13.000000 foundationallm-0.7.5/foundationallm/models/orchestration/completion_response.py
--rw-rw-rw-   0        0        0      469 2024-05-23 12:16:43.000000 foundationallm-0.7.5/foundationallm/models/orchestration/endpoint_settings.py
--rw-rw-rw-   0        0        0      370 2023-12-14 16:50:30.000000 foundationallm-0.7.5/foundationallm/models/orchestration/message_history_item.py
--rw-rw-rw-   0        0        0      154 2024-05-07 13:15:07.000000 foundationallm-0.7.5/foundationallm/models/orchestration/operation_types.py
--rw-rw-rw-   0        0        0      939 2024-05-07 13:15:07.000000 foundationallm-0.7.5/foundationallm/models/orchestration/orchestration_settings.py
-drwxrwxrwx   0        0        0        0 2024-05-23 12:19:31.467541 foundationallm-0.7.5/foundationallm.egg-info/
--rw-rw-rw-   0        0        0      633 2024-05-23 12:19:31.000000 foundationallm-0.7.5/foundationallm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2024-05-23 12:19:31.000000 foundationallm-0.7.5/foundationallm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 12:19:31.000000 foundationallm-0.7.5/foundationallm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-23 12:19:31.000000 foundationallm-0.7.5/foundationallm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      633 2024-05-23 12:19:22.000000 foundationallm-0.7.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 12:19:31.470050 foundationallm-0.7.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.986018 foundationallm-0.7.6/
+-rw-rw-rw-   0        0        0      201 2024-05-07 13:15:07.000000 foundationallm-0.7.6/LICENSE
+-rw-rw-rw-   0        0        0      892 2024-05-27 10:08:46.985017 foundationallm-0.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-05-23 14:45:46.000000 foundationallm-0.7.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.926317 foundationallm-0.7.6/foundationallm/
+drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.947341 foundationallm-0.7.6/foundationallm/config/
+-rw-rw-rw-   0        0        0      177 2023-12-14 16:50:30.000000 foundationallm-0.7.6/foundationallm/config/__init__.py
+-rw-rw-rw-   0        0        0     4874 2024-05-23 11:10:06.000000 foundationallm-0.7.6/foundationallm/config/configuration.py
+-rw-rw-rw-   0        0        0      605 2023-12-14 16:50:30.000000 foundationallm-0.7.6/foundationallm/config/context.py
+-rw-rw-rw-   0        0        0      378 2024-03-15 16:01:06.000000 foundationallm-0.7.6/foundationallm/config/environment_variables.py
+-rw-rw-rw-   0        0        0      556 2023-12-14 16:50:30.000000 foundationallm-0.7.6/foundationallm/config/user_identity.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.927318 foundationallm-0.7.6/foundationallm/models/
+drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.968997 foundationallm-0.7.6/foundationallm/models/agents/
+-rw-rw-rw-   0        0        0      409 2024-05-23 14:45:46.000000 foundationallm-0.7.6/foundationallm/models/agents/__init__.py
+-rw-rw-rw-   0        0        0      815 2024-05-07 13:15:07.000000 foundationallm-0.7.6/foundationallm/models/agents/agent_base.py
+-rw-rw-rw-   0        0        0      316 2024-04-24 17:34:13.000000 foundationallm-0.7.6/foundationallm/models/agents/agent_conversation_history_settings.py
+-rw-rw-rw-   0        0        0      274 2024-04-24 17:34:13.000000 foundationallm-0.7.6/foundationallm/models/agents/agent_gatekeeper_settings.py
+-rw-rw-rw-   0        0        0      594 2024-05-07 13:15:07.000000 foundationallm-0.7.6/foundationallm/models/agents/agent_vectorization_settings.py
+-rw-rw-rw-   0        0        0      361 2024-04-24 17:34:13.000000 foundationallm-0.7.6/foundationallm/models/agents/knowledge_management_agent.py
+-rw-rw-rw-   0        0        0      518 2024-05-07 13:15:07.000000 foundationallm-0.7.6/foundationallm/models/agents/knowledge_management_completion_request.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.971500 foundationallm-0.7.6/foundationallm/models/authentication/
+-rw-rw-rw-   0        0        0       55 2024-05-07 13:15:07.000000 foundationallm-0.7.6/foundationallm/models/authentication/__init__.py
+-rw-rw-rw-   0        0        0      157 2024-05-07 13:15:07.000000 foundationallm-0.7.6/foundationallm/models/authentication/authentication_types.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.982013 foundationallm-0.7.6/foundationallm/models/orchestration/
+-rw-rw-rw-   0        0        0      402 2024-05-23 14:45:46.000000 foundationallm-0.7.6/foundationallm/models/orchestration/__init__.py
+-rw-rw-rw-   0        0        0      272 2024-04-24 17:34:13.000000 foundationallm-0.7.6/foundationallm/models/orchestration/citation.py
+-rw-rw-rw-   0        0        0      502 2024-05-07 13:15:07.000000 foundationallm-0.7.6/foundationallm/models/orchestration/completion_request_base.py
+-rw-rw-rw-   0        0        0      523 2024-04-24 17:34:13.000000 foundationallm-0.7.6/foundationallm/models/orchestration/completion_response.py
+-rw-rw-rw-   0        0        0      469 2024-05-23 14:45:46.000000 foundationallm-0.7.6/foundationallm/models/orchestration/endpoint_settings.py
+-rw-rw-rw-   0        0        0      370 2023-12-14 16:50:30.000000 foundationallm-0.7.6/foundationallm/models/orchestration/message_history_item.py
+-rw-rw-rw-   0        0        0      154 2024-05-23 14:45:46.000000 foundationallm-0.7.6/foundationallm/models/orchestration/operation_types.py
+-rw-rw-rw-   0        0        0      939 2024-05-07 13:15:07.000000 foundationallm-0.7.6/foundationallm/models/orchestration/orchestration_settings.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:08:46.984019 foundationallm-0.7.6/foundationallm.egg-info/
+-rw-rw-rw-   0        0        0      892 2024-05-27 10:08:46.000000 foundationallm-0.7.6/foundationallm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1340 2024-05-27 10:08:46.000000 foundationallm-0.7.6/foundationallm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 10:08:46.000000 foundationallm-0.7.6/foundationallm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-27 10:08:46.000000 foundationallm-0.7.6/foundationallm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      651 2024-05-27 10:06:29.000000 foundationallm-0.7.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 10:08:46.987018 foundationallm-0.7.6/setup.cfg
```

### Comparing `foundationallm-0.7.5/foundationallm/config/configuration.py` & `foundationallm-0.7.6/foundationallm/config/configuration.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.5/foundationallm/config/context.py` & `foundationallm-0.7.6/foundationallm/config/context.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.5/foundationallm/config/user_identity.py` & `foundationallm-0.7.6/foundationallm/config/user_identity.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.5/foundationallm/models/orchestration/completion_response.py` & `foundationallm-0.7.6/foundationallm/models/orchestration/completion_response.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.5/foundationallm/models/orchestration/orchestration_settings.py` & `foundationallm-0.7.6/foundationallm/models/orchestration/orchestration_settings.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.5/foundationallm.egg-info/SOURCES.txt` & `foundationallm-0.7.6/foundationallm.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 foundationallm.egg-info/dependency_links.txt
 foundationallm.egg-info/top_level.txt
 foundationallm/config/__init__.py
 foundationallm/config/configuration.py
 foundationallm/config/context.py
 foundationallm/config/environment_variables.py
 foundationallm/config/user_identity.py
+foundationallm/models/agents/__init__.py
+foundationallm/models/agents/agent_base.py
+foundationallm/models/agents/agent_conversation_history_settings.py
+foundationallm/models/agents/agent_gatekeeper_settings.py
+foundationallm/models/agents/agent_vectorization_settings.py
+foundationallm/models/agents/knowledge_management_agent.py
+foundationallm/models/agents/knowledge_management_completion_request.py
 foundationallm/models/authentication/__init__.py
 foundationallm/models/authentication/authentication_types.py
 foundationallm/models/orchestration/__init__.py
 foundationallm/models/orchestration/citation.py
 foundationallm/models/orchestration/completion_request_base.py
 foundationallm/models/orchestration/completion_response.py
 foundationallm/models/orchestration/endpoint_settings.py
```

### Comparing `foundationallm-0.7.5/pyproject.toml` & `foundationallm-0.7.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "foundationallm"
-version = "0.7.5"
+version = "0.7.6"
 authors = [
   { name="FoundationaLLM", email="dev@foundationallm.ai" },
 ]
 description = "Enables integration with the FoundationaLLM platform."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
@@ -14,8 +14,8 @@
 ]
 
 [project.urls]
 Homepage = "https://foundationallm.ai"
 Issues = "https://github.com/solliancenet/foundationallm/issues"
 
 [tool.setuptools.packages.find]
-include = ['*authentication', '*config', '*models.orchestration']
+include = ['*authentication', '*config', '*models.orchestration', '*models.agents']
```

