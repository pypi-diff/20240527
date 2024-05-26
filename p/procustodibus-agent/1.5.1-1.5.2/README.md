# Comparing `tmp/procustodibus_agent-1.5.1.tar.gz` & `tmp/procustodibus_agent-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procustodibus_agent-1.5.1.tar", last modified: Fri May  3 18:59:11 2024, max compression
+gzip compressed data, was "procustodibus_agent-1.5.2.tar", last modified: Sun May 26 22:07:05 2024, max compression
```

## Comparing `procustodibus_agent-1.5.1.tar` & `procustodibus_agent-1.5.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-03 18:59:11.124505 procustodibus_agent-1.5.1/
--rw-rw-r--   0 justin    (1000) justin    (1000)     1076 2024-01-15 23:37:44.000000 procustodibus_agent-1.5.1/LICENSE
--rw-rw-r--   0 justin    (1000) justin    (1000)       30 2021-11-09 19:41:28.000000 procustodibus_agent-1.5.1/MANIFEST.in
--rw-r--r--   0 justin    (1000) justin    (1000)     7885 2024-05-03 18:59:11.124505 procustodibus_agent-1.5.1/PKG-INFO
--rw-rw-r--   0 justin    (1000) justin    (1000)     4732 2024-04-05 18:04:50.000000 procustodibus_agent-1.5.1/README.md
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-03 18:59:11.104457 procustodibus_agent-1.5.1/procustodibus_agent/
--rw-rw-r--   0 justin    (1000) justin    (1000)      208 2024-05-03 18:21:41.000000 procustodibus_agent-1.5.1/procustodibus_agent/__init__.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     3153 2024-05-03 18:21:40.000000 procustodibus_agent-1.5.1/procustodibus_agent/agent.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    10970 2023-12-10 23:12:39.000000 procustodibus_agent-1.5.1/procustodibus_agent/api.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     1895 2024-05-03 18:21:40.000000 procustodibus_agent-1.5.1/procustodibus_agent/cli.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    18953 2024-05-03 18:21:40.000000 procustodibus_agent-1.5.1/procustodibus_agent/cnf.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     5464 2024-01-15 23:37:44.000000 procustodibus_agent-1.5.1/procustodibus_agent/connectivity.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     1398 2022-06-29 01:32:50.000000 procustodibus_agent-1.5.1/procustodibus_agent/credentials.py
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-03 18:59:11.108467 procustodibus_agent-1.5.1/procustodibus_agent/executor/
--rw-rw-r--   0 justin    (1000) justin    (1000)      122 2024-04-05 18:04:48.000000 procustodibus_agent-1.5.1/procustodibus_agent/executor/__init__.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    34310 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.1/procustodibus_agent/executor/execution.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    20632 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.1/procustodibus_agent/executor/sys_cmd.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     7432 2024-04-05 18:04:47.000000 procustodibus_agent-1.5.1/procustodibus_agent/ip_route.py
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-03 18:59:11.112476 procustodibus_agent-1.5.1/procustodibus_agent/mfa/
--rw-rw-r--   0 justin    (1000) justin    (1000)     7123 2022-06-29 01:32:56.000000 procustodibus_agent-1.5.1/procustodibus_agent/mfa/__init__.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     2656 2023-03-17 00:35:09.000000 procustodibus_agent-1.5.1/procustodibus_agent/mfa/api.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     4347 2022-06-29 01:32:56.000000 procustodibus_agent-1.5.1/procustodibus_agent/mfa/cli.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     4073 2021-08-02 23:52:55.000000 procustodibus_agent-1.5.1/procustodibus_agent/resolve_hostname.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     3841 2021-05-16 20:05:23.000000 procustodibus_agent-1.5.1/procustodibus_agent/wg.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    13359 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.1/procustodibus_agent/wg_cnf.py
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-03 18:59:11.112476 procustodibus_agent-1.5.1/procustodibus_agent/windows/
--rw-rw-r--   0 justin    (1000) justin    (1000)     5763 2024-04-05 18:04:50.000000 procustodibus_agent-1.5.1/procustodibus_agent/windows/cnf.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     2132 2024-04-05 18:04:50.000000 procustodibus_agent-1.5.1/procustodibus_agent/windows/service.py
--rw-rw-r--   0 justin    (1000) justin    (1000)      344 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.1/procustodibus_agent/windows/service_config.py
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-03 18:59:11.116486 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/
--rw-r--r--   0 justin    (1000) justin    (1000)     7885 2024-05-03 18:59:11.000000 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/PKG-INFO
--rw-rw-r--   0 justin    (1000) justin    (1000)     1130 2024-05-03 18:59:11.000000 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)        1 2024-05-03 18:59:11.000000 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      187 2024-05-03 18:59:11.000000 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/entry_points.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      714 2024-05-03 18:59:11.000000 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/requires.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)       20 2024-05-03 18:59:11.000000 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/top_level.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)        1 2020-08-17 01:25:01.000000 procustodibus_agent-1.5.1/procustodibus_agent.egg-info/zip-safe
--rw-rw-r--   0 justin    (1000) justin    (1000)       92 2024-03-17 03:21:19.000000 procustodibus_agent-1.5.1/pyproject.toml
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-03 18:59:11.116486 procustodibus_agent-1.5.1/requirements/
--rw-rw-r--   0 justin    (1000) justin    (1000)       50 2020-08-14 21:08:08.000000 procustodibus_agent-1.5.1/requirements/dev.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      585 2023-03-17 00:35:09.000000 procustodibus_agent-1.5.1/requirements/lint.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      124 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.1/requirements/prod.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)       73 2020-10-09 21:04:40.000000 procustodibus_agent-1.5.1/requirements/test.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      591 2024-05-03 18:59:11.124505 procustodibus_agent-1.5.1/setup.cfg
--rw-rw-r--   0 justin    (1000) justin    (1000)     2273 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.1/setup.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-26 22:07:05.427158 procustodibus_agent-1.5.2/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1076 2024-01-15 23:37:44.000000 procustodibus_agent-1.5.2/LICENSE
+-rw-rw-r--   0 justin    (1000) justin    (1000)       30 2021-11-09 19:41:28.000000 procustodibus_agent-1.5.2/MANIFEST.in
+-rw-r--r--   0 justin    (1000) justin    (1000)     7888 2024-05-26 22:07:05.427158 procustodibus_agent-1.5.2/PKG-INFO
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4735 2024-05-26 21:53:23.000000 procustodibus_agent-1.5.2/README.md
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-26 22:07:05.411100 procustodibus_agent-1.5.2/procustodibus_agent/
+-rw-rw-r--   0 justin    (1000) justin    (1000)      208 2024-05-26 21:53:50.000000 procustodibus_agent-1.5.2/procustodibus_agent/__init__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     3153 2024-05-26 01:12:28.000000 procustodibus_agent-1.5.2/procustodibus_agent/agent.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    10970 2024-05-26 01:11:32.000000 procustodibus_agent-1.5.2/procustodibus_agent/api.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1895 2024-05-26 01:11:32.000000 procustodibus_agent-1.5.2/procustodibus_agent/cli.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    18953 2024-05-26 01:12:28.000000 procustodibus_agent-1.5.2/procustodibus_agent/cnf.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     5464 2024-05-26 01:12:28.000000 procustodibus_agent-1.5.2/procustodibus_agent/connectivity.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1398 2024-05-26 01:11:32.000000 procustodibus_agent-1.5.2/procustodibus_agent/credentials.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-26 22:07:05.411100 procustodibus_agent-1.5.2/procustodibus_agent/executor/
+-rw-rw-r--   0 justin    (1000) justin    (1000)      122 2024-04-05 18:04:48.000000 procustodibus_agent-1.5.2/procustodibus_agent/executor/__init__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    34310 2024-05-26 01:12:28.000000 procustodibus_agent-1.5.2/procustodibus_agent/executor/execution.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    20632 2024-05-26 01:12:28.000000 procustodibus_agent-1.5.2/procustodibus_agent/executor/sys_cmd.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     7432 2024-05-26 01:12:28.000000 procustodibus_agent-1.5.2/procustodibus_agent/ip_route.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-26 22:07:05.411100 procustodibus_agent-1.5.2/procustodibus_agent/mfa/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     7123 2022-06-29 01:32:56.000000 procustodibus_agent-1.5.2/procustodibus_agent/mfa/__init__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2656 2023-03-17 00:35:09.000000 procustodibus_agent-1.5.2/procustodibus_agent/mfa/api.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4347 2024-05-26 01:11:32.000000 procustodibus_agent-1.5.2/procustodibus_agent/mfa/cli.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4073 2024-05-26 01:12:28.000000 procustodibus_agent-1.5.2/procustodibus_agent/resolve_hostname.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     3841 2024-05-26 01:12:28.000000 procustodibus_agent-1.5.2/procustodibus_agent/wg.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    13359 2024-05-26 01:12:28.000000 procustodibus_agent-1.5.2/procustodibus_agent/wg_cnf.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-26 22:07:05.415114 procustodibus_agent-1.5.2/procustodibus_agent/windows/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     5763 2024-05-26 01:12:28.000000 procustodibus_agent-1.5.2/procustodibus_agent/windows/cnf.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2132 2024-05-26 01:12:28.000000 procustodibus_agent-1.5.2/procustodibus_agent/windows/service.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)      344 2024-05-26 01:11:32.000000 procustodibus_agent-1.5.2/procustodibus_agent/windows/service_config.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-26 22:07:05.415114 procustodibus_agent-1.5.2/procustodibus_agent.egg-info/
+-rw-r--r--   0 justin    (1000) justin    (1000)     7888 2024-05-26 22:07:05.000000 procustodibus_agent-1.5.2/procustodibus_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1130 2024-05-26 22:07:05.000000 procustodibus_agent-1.5.2/procustodibus_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)        1 2024-05-26 22:07:05.000000 procustodibus_agent-1.5.2/procustodibus_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      187 2024-05-26 22:07:05.000000 procustodibus_agent-1.5.2/procustodibus_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      714 2024-05-26 22:07:05.000000 procustodibus_agent-1.5.2/procustodibus_agent.egg-info/requires.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       20 2024-05-26 22:07:05.000000 procustodibus_agent-1.5.2/procustodibus_agent.egg-info/top_level.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)        1 2020-08-17 01:25:01.000000 procustodibus_agent-1.5.2/procustodibus_agent.egg-info/zip-safe
+-rw-rw-r--   0 justin    (1000) justin    (1000)       92 2024-03-17 03:21:19.000000 procustodibus_agent-1.5.2/pyproject.toml
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2024-05-26 22:07:05.415114 procustodibus_agent-1.5.2/requirements/
+-rw-rw-r--   0 justin    (1000) justin    (1000)       50 2020-08-14 21:08:08.000000 procustodibus_agent-1.5.2/requirements/dev.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      585 2023-03-17 00:35:09.000000 procustodibus_agent-1.5.2/requirements/lint.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      124 2024-04-05 18:04:49.000000 procustodibus_agent-1.5.2/requirements/prod.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       73 2020-10-09 21:04:40.000000 procustodibus_agent-1.5.2/requirements/test.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      591 2024-05-26 22:07:05.427158 procustodibus_agent-1.5.2/setup.cfg
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2273 2024-05-26 01:11:32.000000 procustodibus_agent-1.5.2/setup.py
```

### Comparing `procustodibus_agent-1.5.1/LICENSE` & `procustodibus_agent-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/PKG-INFO` & `procustodibus_agent-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procustodibus_agent
-Version: 1.5.1
+Version: 1.5.2
 Summary: Synchronizes your WireGuard settings with Pro Custodibus.
 Home-page: https://www.procustodibus.com/
 Author: Arcem Tene
 Author-email: dev@arcemtene.com
 License: MIT
 Project-URL: Changelog, https://docs.procustodibus.com/guide/agents/download/#changelog
 Project-URL: Documentation, https://docs.procustodibus.com/guide/agents/run/
@@ -162,15 +162,15 @@
     --volume /srv/containers/wireguard/conf:/etc/wireguard \
     procustodibus-agent:dev
 ```
 
 Run all (docker-based) installer tests:
 ```
 docker-compose -f test_install/docker-compose.yml build --pull
-tox -e py310 test_install
+tox -e py310 -- test_install
 ```
 
 Manually run pre-push hook on all version-controlled files:
 ```
 tox -e pre-commit -- run -a --hook-stage push
 ```
```

### Comparing `procustodibus_agent-1.5.1/README.md` & `procustodibus_agent-1.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     --volume /srv/containers/wireguard/conf:/etc/wireguard \
     procustodibus-agent:dev
 ```
 
 Run all (docker-based) installer tests:
 ```
 docker-compose -f test_install/docker-compose.yml build --pull
-tox -e py310 test_install
+tox -e py310 -- test_install
 ```
 
 Manually run pre-push hook on all version-controlled files:
 ```
 tox -e pre-commit -- run -a --hook-stage push
 ```
```

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/agent.py` & `procustodibus_agent-1.5.2/procustodibus_agent/agent.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/api.py` & `procustodibus_agent-1.5.2/procustodibus_agent/api.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/cli.py` & `procustodibus_agent-1.5.2/procustodibus_agent/cli.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/cnf.py` & `procustodibus_agent-1.5.2/procustodibus_agent/cnf.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/connectivity.py` & `procustodibus_agent-1.5.2/procustodibus_agent/connectivity.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/credentials.py` & `procustodibus_agent-1.5.2/procustodibus_agent/credentials.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/executor/execution.py` & `procustodibus_agent-1.5.2/procustodibus_agent/executor/execution.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/executor/sys_cmd.py` & `procustodibus_agent-1.5.2/procustodibus_agent/executor/sys_cmd.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/ip_route.py` & `procustodibus_agent-1.5.2/procustodibus_agent/ip_route.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/mfa/__init__.py` & `procustodibus_agent-1.5.2/procustodibus_agent/mfa/__init__.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/mfa/api.py` & `procustodibus_agent-1.5.2/procustodibus_agent/mfa/api.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/mfa/cli.py` & `procustodibus_agent-1.5.2/procustodibus_agent/mfa/cli.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/resolve_hostname.py` & `procustodibus_agent-1.5.2/procustodibus_agent/resolve_hostname.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/wg.py` & `procustodibus_agent-1.5.2/procustodibus_agent/wg.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/wg_cnf.py` & `procustodibus_agent-1.5.2/procustodibus_agent/wg_cnf.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/windows/cnf.py` & `procustodibus_agent-1.5.2/procustodibus_agent/windows/cnf.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent/windows/service.py` & `procustodibus_agent-1.5.2/procustodibus_agent/windows/service.py`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent.egg-info/PKG-INFO` & `procustodibus_agent-1.5.2/procustodibus_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procustodibus_agent
-Version: 1.5.1
+Version: 1.5.2
 Summary: Synchronizes your WireGuard settings with Pro Custodibus.
 Home-page: https://www.procustodibus.com/
 Author: Arcem Tene
 Author-email: dev@arcemtene.com
 License: MIT
 Project-URL: Changelog, https://docs.procustodibus.com/guide/agents/download/#changelog
 Project-URL: Documentation, https://docs.procustodibus.com/guide/agents/run/
@@ -162,15 +162,15 @@
     --volume /srv/containers/wireguard/conf:/etc/wireguard \
     procustodibus-agent:dev
 ```
 
 Run all (docker-based) installer tests:
 ```
 docker-compose -f test_install/docker-compose.yml build --pull
-tox -e py310 test_install
+tox -e py310 -- test_install
 ```
 
 Manually run pre-push hook on all version-controlled files:
 ```
 tox -e pre-commit -- run -a --hook-stage push
 ```
```

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent.egg-info/SOURCES.txt` & `procustodibus_agent-1.5.2/procustodibus_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/procustodibus_agent.egg-info/requires.txt` & `procustodibus_agent-1.5.2/procustodibus_agent.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/requirements/lint.txt` & `procustodibus_agent-1.5.2/requirements/lint.txt`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/setup.cfg` & `procustodibus_agent-1.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `procustodibus_agent-1.5.1/setup.py` & `procustodibus_agent-1.5.2/setup.py`

 * *Files identical despite different names*

