# Comparing `tmp/mpcrl-1.2.1rc1.tar.gz` & `tmp/mpcrl-1.2.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcrl-1.2.1rc1.tar", last modified: Mon Apr 15 15:20:50 2024, max compression
+gzip compressed data, was "mpcrl-1.2.1rc2.tar", last modified: Mon May 27 11:46:09 2024, max compression
```

## Comparing `mpcrl-1.2.1rc1.tar` & `mpcrl-1.2.1rc2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.393318 mpcrl-1.2.1rc1/
--rw-rw-rw-   0        0        0     1093 2022-11-28 16:28:05.000000 mpcrl-1.2.1rc1/LICENSE
--rw-rw-rw-   0        0        0     6178 2024-04-15 15:20:50.388285 mpcrl-1.2.1rc1/PKG-INFO
--rw-rw-rw-   0        0        0     4935 2024-04-12 22:21:05.000000 mpcrl-1.2.1rc1/README.md
--rw-rw-rw-   0        0        0     2195 2024-04-11 13:47:55.000000 mpcrl-1.2.1rc1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 15:20:50.394284 mpcrl-1.2.1rc1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.092159 mpcrl-1.2.1rc1/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.131464 mpcrl-1.2.1rc1/src/mpcrl/
--rw-rw-rw-   0        0        0     1289 2024-04-15 14:55:11.000000 mpcrl-1.2.1rc1/src/mpcrl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.164863 mpcrl-1.2.1rc1/src/mpcrl/agents/
-drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.185846 mpcrl-1.2.1rc1/src/mpcrl/agents/common/
--rw-rw-rw-   0        0        0    27020 2024-04-15 15:18:33.000000 mpcrl-1.2.1rc1/src/mpcrl/agents/common/agent.py
--rw-rw-rw-   0        0        0     3707 2024-04-11 13:45:23.000000 mpcrl-1.2.1rc1/src/mpcrl/agents/common/globopt_learning_agent.py
--rw-rw-rw-   0        0        0    14240 2024-04-15 14:42:04.000000 mpcrl-1.2.1rc1/src/mpcrl/agents/common/learning_agent.py
--rw-rw-rw-   0        0        0     1749 2024-04-11 13:45:25.000000 mpcrl-1.2.1rc1/src/mpcrl/agents/common/rl_learning_agent.py
--rw-rw-rw-   0        0        0    23054 2024-04-13 20:46:44.000000 mpcrl-1.2.1rc1/src/mpcrl/agents/lstd_dpg.py
--rw-rw-rw-   0        0        0    15340 2024-04-13 19:50:03.000000 mpcrl-1.2.1rc1/src/mpcrl/agents/lstd_q_learning.py
-drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.231047 mpcrl-1.2.1rc1/src/mpcrl/core/
--rw-rw-rw-   0        0        0        0 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc1/src/mpcrl/core/__init__.py
--rw-rw-rw-   0        0        0     9809 2024-04-15 11:58:24.000000 mpcrl-1.2.1rc1/src/mpcrl/core/callbacks.py
--rw-rw-rw-   0        0        0     1609 2023-01-07 11:39:22.000000 mpcrl-1.2.1rc1/src/mpcrl/core/errors.py
--rw-rw-rw-   0        0        0     3461 2024-04-12 22:21:05.000000 mpcrl-1.2.1rc1/src/mpcrl/core/experience.py
--rw-rw-rw-   0        0        0    16018 2024-04-12 22:21:05.000000 mpcrl-1.2.1rc1/src/mpcrl/core/exploration.py
--rw-rw-rw-   0        0        0    12085 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc1/src/mpcrl/core/parameters.py
--rw-rw-rw-   0        0        0     7143 2023-10-26 16:39:17.000000 mpcrl-1.2.1rc1/src/mpcrl/core/schedulers.py
--rw-rw-rw-   0        0        0     2537 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc1/src/mpcrl/core/update.py
--rw-rw-rw-   0        0        0     4713 2024-04-11 13:48:00.000000 mpcrl-1.2.1rc1/src/mpcrl/core/warmstart.py
-drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.276213 mpcrl-1.2.1rc1/src/mpcrl/optim/
--rw-rw-rw-   0        0        0      482 2024-04-11 13:45:23.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/__init__.py
--rw-rw-rw-   0        0        0     7193 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/adam.py
--rw-rw-rw-   0        0        0     2600 2024-04-11 13:45:13.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/base_optimizer.py
--rw-rw-rw-   0        0        0     6668 2024-04-11 13:45:13.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/gradient_based_optimizer.py
--rw-rw-rw-   0        0        0     5624 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/gradient_descent.py
--rw-rw-rw-   0        0        0     2429 2024-04-11 13:45:15.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/gradient_free_optimizer.py
--rw-rw-rw-   0        0        0     6712 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/newton_method.py
--rw-rw-rw-   0        0        0     6532 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc1/src/mpcrl/optim/rmsprop.py
-drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.299216 mpcrl-1.2.1rc1/src/mpcrl/util/
--rw-rw-rw-   0        0        0     2785 2023-08-28 20:00:11.000000 mpcrl-1.2.1rc1/src/mpcrl/util/control.py
--rw-rw-rw-   0        0        0      800 2023-09-21 13:43:47.000000 mpcrl-1.2.1rc1/src/mpcrl/util/iters.py
--rw-rw-rw-   0        0        0     4855 2023-10-26 16:35:58.000000 mpcrl-1.2.1rc1/src/mpcrl/util/math.py
--rw-rw-rw-   0        0        0      933 2023-09-21 13:43:47.000000 mpcrl-1.2.1rc1/src/mpcrl/util/named.py
--rw-rw-rw-   0        0        0      638 2023-12-29 16:11:53.000000 mpcrl-1.2.1rc1/src/mpcrl/util/seeding.py
-drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.113464 mpcrl-1.2.1rc1/src/mpcrl/wrappers/
-drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.326800 mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/
--rw-rw-rw-   0        0        0      224 2024-04-15 13:57:59.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/__init__.py
--rw-rw-rw-   0        0        0     4615 2024-04-15 14:38:03.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/evaluate.py
--rw-rw-rw-   0        0        0     8402 2024-04-11 13:45:23.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/log.py
--rw-rw-rw-   0        0        0     1261 2024-04-11 13:45:23.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/record_updates.py
--rw-rw-rw-   0        0        0     4832 2024-04-15 12:11:27.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.343797 mpcrl-1.2.1rc1/src/mpcrl/wrappers/envs/
--rw-rw-rw-   0        0        0      137 2023-10-26 16:37:23.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/envs/__init__.py
--rw-rw-rw-   0        0        0     4446 2024-04-11 13:47:27.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/envs/monitor_episodes.py
--rw-rw-rw-   0        0        0     4939 2023-09-21 13:43:47.000000 mpcrl-1.2.1rc1/src/mpcrl/wrappers/envs/monitor_infos.py
-drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.382282 mpcrl-1.2.1rc1/src/mpcrl.egg-info/
--rw-rw-rw-   0        0        0     6178 2024-04-15 15:20:50.000000 mpcrl-1.2.1rc1/src/mpcrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1530 2024-04-15 15:20:50.000000 mpcrl-1.2.1rc1/src/mpcrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 15:20:50.000000 mpcrl-1.2.1rc1/src/mpcrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2024-04-15 15:20:50.000000 mpcrl-1.2.1rc1/src/mpcrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-15 15:20:50.000000 mpcrl-1.2.1rc1/src/mpcrl.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 15:20:50.377290 mpcrl-1.2.1rc1/tests/
--rw-rw-rw-   0        0        0    16493 2024-04-12 22:21:05.000000 mpcrl-1.2.1rc1/tests/test_agent.py
--rw-rw-rw-   0        0        0    24223 2024-04-12 22:21:05.000000 mpcrl-1.2.1rc1/tests/test_core.py
--rw-rw-rw-   0        0        0    12018 2024-04-15 15:18:20.000000 mpcrl-1.2.1rc1/tests/test_examples.py
--rw-rw-rw-   0        0        0    18686 2024-04-11 13:45:13.000000 mpcrl-1.2.1rc1/tests/test_optim.py
--rw-rw-rw-   0        0        0     5040 2023-12-29 16:11:53.000000 mpcrl-1.2.1rc1/tests/test_util.py
--rw-rw-rw-   0        0        0    16530 2024-04-15 14:49:52.000000 mpcrl-1.2.1rc1/tests/test_wrappers.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:09.502302 mpcrl-1.2.1rc2/
+-rw-rw-rw-   0        0        0     1093 2022-11-28 16:28:05.000000 mpcrl-1.2.1rc2/LICENSE
+-rw-rw-rw-   0        0        0     6181 2024-05-27 11:46:09.499268 mpcrl-1.2.1rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     4935 2024-04-12 22:21:05.000000 mpcrl-1.2.1rc2/README.md
+-rw-rw-rw-   0        0        0     2198 2024-05-27 11:44:16.000000 mpcrl-1.2.1rc2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 11:46:09.503292 mpcrl-1.2.1rc2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:09.272598 mpcrl-1.2.1rc2/src/
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:09.309670 mpcrl-1.2.1rc2/src/mpcrl/
+-rw-rw-rw-   0        0        0     1289 2024-05-27 11:43:53.000000 mpcrl-1.2.1rc2/src/mpcrl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:09.335641 mpcrl-1.2.1rc2/src/mpcrl/agents/
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:09.351406 mpcrl-1.2.1rc2/src/mpcrl/agents/common/
+-rw-rw-rw-   0        0        0    27021 2024-05-27 11:44:53.000000 mpcrl-1.2.1rc2/src/mpcrl/agents/common/agent.py
+-rw-rw-rw-   0        0        0     3707 2024-04-11 13:45:23.000000 mpcrl-1.2.1rc2/src/mpcrl/agents/common/globopt_learning_agent.py
+-rw-rw-rw-   0        0        0    14240 2024-04-26 08:06:19.000000 mpcrl-1.2.1rc2/src/mpcrl/agents/common/learning_agent.py
+-rw-rw-rw-   0        0        0     1749 2024-04-11 13:45:25.000000 mpcrl-1.2.1rc2/src/mpcrl/agents/common/rl_learning_agent.py
+-rw-rw-rw-   0        0        0    23061 2024-04-26 08:17:41.000000 mpcrl-1.2.1rc2/src/mpcrl/agents/lstd_dpg.py
+-rw-rw-rw-   0        0        0    15936 2024-05-27 11:44:53.000000 mpcrl-1.2.1rc2/src/mpcrl/agents/lstd_q_learning.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:09.386620 mpcrl-1.2.1rc2/src/mpcrl/core/
+-rw-rw-rw-   0        0        0        0 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc2/src/mpcrl/core/__init__.py
+-rw-rw-rw-   0        0        0     9809 2024-04-15 11:58:24.000000 mpcrl-1.2.1rc2/src/mpcrl/core/callbacks.py
+-rw-rw-rw-   0        0        0     1609 2023-01-07 11:39:22.000000 mpcrl-1.2.1rc2/src/mpcrl/core/errors.py
+-rw-rw-rw-   0        0        0     3461 2024-04-12 22:21:05.000000 mpcrl-1.2.1rc2/src/mpcrl/core/experience.py
+-rw-rw-rw-   0        0        0    21308 2024-04-26 07:59:59.000000 mpcrl-1.2.1rc2/src/mpcrl/core/exploration.py
+-rw-rw-rw-   0        0        0    12085 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc2/src/mpcrl/core/parameters.py
+-rw-rw-rw-   0        0        0     7143 2023-10-26 16:39:17.000000 mpcrl-1.2.1rc2/src/mpcrl/core/schedulers.py
+-rw-rw-rw-   0        0        0     2537 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc2/src/mpcrl/core/update.py
+-rw-rw-rw-   0        0        0     4713 2024-04-11 13:48:00.000000 mpcrl-1.2.1rc2/src/mpcrl/core/warmstart.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:09.418446 mpcrl-1.2.1rc2/src/mpcrl/optim/
+-rw-rw-rw-   0        0        0      482 2024-04-11 13:45:23.000000 mpcrl-1.2.1rc2/src/mpcrl/optim/__init__.py
+-rw-rw-rw-   0        0        0     7193 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc2/src/mpcrl/optim/adam.py
+-rw-rw-rw-   0        0        0     2600 2024-04-11 13:45:13.000000 mpcrl-1.2.1rc2/src/mpcrl/optim/base_optimizer.py
+-rw-rw-rw-   0        0        0     6668 2024-04-11 13:45:13.000000 mpcrl-1.2.1rc2/src/mpcrl/optim/gradient_based_optimizer.py
+-rw-rw-rw-   0        0        0     5624 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc2/src/mpcrl/optim/gradient_descent.py
+-rw-rw-rw-   0        0        0     2429 2024-04-11 13:45:15.000000 mpcrl-1.2.1rc2/src/mpcrl/optim/gradient_free_optimizer.py
+-rw-rw-rw-   0        0        0     6712 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc2/src/mpcrl/optim/newton_method.py
+-rw-rw-rw-   0        0        0     6532 2023-10-26 16:39:29.000000 mpcrl-1.2.1rc2/src/mpcrl/optim/rmsprop.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:09.435875 mpcrl-1.2.1rc2/src/mpcrl/util/
+-rw-rw-rw-   0        0        0     2785 2023-08-28 20:00:11.000000 mpcrl-1.2.1rc2/src/mpcrl/util/control.py
+-rw-rw-rw-   0        0        0      800 2023-09-21 13:43:47.000000 mpcrl-1.2.1rc2/src/mpcrl/util/iters.py
+-rw-rw-rw-   0        0        0     4855 2023-10-26 16:35:58.000000 mpcrl-1.2.1rc2/src/mpcrl/util/math.py
+-rw-rw-rw-   0        0        0      933 2023-09-21 13:43:47.000000 mpcrl-1.2.1rc2/src/mpcrl/util/named.py
+-rw-rw-rw-   0        0        0      638 2023-12-29 16:11:53.000000 mpcrl-1.2.1rc2/src/mpcrl/util/seeding.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:09.285596 mpcrl-1.2.1rc2/src/mpcrl/wrappers/
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:09.455057 mpcrl-1.2.1rc2/src/mpcrl/wrappers/agents/
+-rw-rw-rw-   0        0        0      224 2024-04-15 13:57:59.000000 mpcrl-1.2.1rc2/src/mpcrl/wrappers/agents/__init__.py
+-rw-rw-rw-   0        0        0     4614 2024-04-24 11:00:32.000000 mpcrl-1.2.1rc2/src/mpcrl/wrappers/agents/evaluate.py
+-rw-rw-rw-   0        0        0     8402 2024-04-11 13:45:23.000000 mpcrl-1.2.1rc2/src/mpcrl/wrappers/agents/log.py
+-rw-rw-rw-   0        0        0     1261 2024-04-11 13:45:23.000000 mpcrl-1.2.1rc2/src/mpcrl/wrappers/agents/record_updates.py
+-rw-rw-rw-   0        0        0     4832 2024-04-15 12:11:27.000000 mpcrl-1.2.1rc2/src/mpcrl/wrappers/agents/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:09.466232 mpcrl-1.2.1rc2/src/mpcrl/wrappers/envs/
+-rw-rw-rw-   0        0        0      137 2023-10-26 16:37:23.000000 mpcrl-1.2.1rc2/src/mpcrl/wrappers/envs/__init__.py
+-rw-rw-rw-   0        0        0     4446 2024-04-11 13:47:27.000000 mpcrl-1.2.1rc2/src/mpcrl/wrappers/envs/monitor_episodes.py
+-rw-rw-rw-   0        0        0     4939 2023-09-21 13:43:47.000000 mpcrl-1.2.1rc2/src/mpcrl/wrappers/envs/monitor_infos.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:09.496622 mpcrl-1.2.1rc2/src/mpcrl.egg-info/
+-rw-rw-rw-   0        0        0     6181 2024-05-27 11:46:09.000000 mpcrl-1.2.1rc2/src/mpcrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1530 2024-05-27 11:46:09.000000 mpcrl-1.2.1rc2/src/mpcrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 11:46:09.000000 mpcrl-1.2.1rc2/src/mpcrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-05-27 11:46:09.000000 mpcrl-1.2.1rc2/src/mpcrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-27 11:46:09.000000 mpcrl-1.2.1rc2/src/mpcrl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:09.489704 mpcrl-1.2.1rc2/tests/
+-rw-rw-rw-   0        0        0    16493 2024-04-12 22:21:05.000000 mpcrl-1.2.1rc2/tests/test_agent.py
+-rw-rw-rw-   0        0        0    26208 2024-04-19 11:28:12.000000 mpcrl-1.2.1rc2/tests/test_core.py
+-rw-rw-rw-   0        0        0    12018 2024-05-27 09:45:42.000000 mpcrl-1.2.1rc2/tests/test_examples.py
+-rw-rw-rw-   0        0        0    18686 2024-04-11 13:45:13.000000 mpcrl-1.2.1rc2/tests/test_optim.py
+-rw-rw-rw-   0        0        0     5040 2023-12-29 16:11:53.000000 mpcrl-1.2.1rc2/tests/test_util.py
+-rw-rw-rw-   0        0        0    16530 2024-04-15 14:49:52.000000 mpcrl-1.2.1rc2/tests/test_wrappers.py
```

### Comparing `mpcrl-1.2.1rc1/LICENSE` & `mpcrl-1.2.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/PKG-INFO` & `mpcrl-1.2.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcrl
-Version: 1.2.1rc1
+Version: 1.2.1rc2
 Summary: Reinforcement Learning with Model Predictive Control
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/mpc-reinforcement-learning
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues
 Keywords: reinforcement-learning,model-predictive-control,optimization,casadi
 Classifier: Programming Language :: Python
@@ -18,15 +18,15 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions>=4.5.0
 Requires-Dist: numba>=0.57.1
-Requires-Dist: csnlp>=1.5.10
+Requires-Dist: csnlp>=1.5.11rc2
 Requires-Dist: scipy>=1.11.0
 Requires-Dist: gymnasium>=0.28.1
 
 # Reinforcement Learning with Model Predictive Control
 
 **mpcrl** is a library for training model-based Reinforcement Learning (RL) agents with Model Predictive Control (MPC) as function approximation. This framework, also known as MPC-based RL, was first proposed in [[1]](#1) and has so far been shown effective in various applications and with different learning algorithms, e.g., [[2](#2),[3](#3)].
```

### Comparing `mpcrl-1.2.1rc1/README.md` & `mpcrl-1.2.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/pyproject.toml` & `mpcrl-1.2.1rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "typing_extensions >= 4.5.0",
     "numba >= 0.57.1",
-    "csnlp >= 1.5.10",
+    "csnlp >= 1.5.11rc2",
     "scipy >= 1.11.0",
     "gymnasium >= 0.28.1",
 ]
 keywords = [
     "reinforcement-learning",
     "model-predictive-control",
     "optimization",
```

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/__init__.py` & `mpcrl-1.2.1rc2/src/mpcrl/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.1rc1"
+__version__ = "1.2.1rc2"
 
 __all__ = [
     "Agent",
     "ExperienceReplay",
     "GlobOptLearningAgent",
     "LearnableParameter",
     "LearnableParametersDict",
```

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/agents/common/agent.py` & `mpcrl-1.2.1rc2/src/mpcrl/agents/common/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,16 +71,16 @@
             `perturbation_parameter`, `action_parameter` and `action_constraint`.
         fixed_parameters : dict[str, array_like] or collection of, optional
             A dict (or collection of dict, in case of `csnlp.MultistartNlp`) whose keys
             are the names of the MPC parameters and the values are their corresponding
             values. Use this to specify fixed parameters, that is, non-learnable. If
             `None`, then no fixed parameter is assumed.
         exploration : ExplorationStrategy, optional
-            Exploration strategy for inducing exploration in the MPC policy. By default
-            `None`, in which case `NoExploration` is used.
+            Exploration strategy for inducing exploration in the online MPC policy. By
+            default `None`, in which case `NoExploration` is used.
         warmstart: "last" or "last-successful" or WarmStartStrategy, optional
             The warmstart strategy for the MPC's NLP. If `last-successful`, the last
             successful solution is used to warm start the solver for the next iteration.
             If `last`, the last solution is used, regardless of success or failure.
             Furthermore, a `WarmStartStrategy` object can be passed to specify a
             strategy for generating multiple warmstart points for the NLP. This is
             useful to generate multiple initial conditions for very non-convex problems.
@@ -328,15 +328,15 @@
             The first optimal action according to the solution of `V(s)`, possibly
             perturbed by exploration noise
         Solution
             The solution of the MPC approximating `V(s)` at the given state.
         """
         V = self._V
         exploration = self._exploration
-        exploration_mode = self._exploration.mode
+        exploration_mode = exploration.mode
         na = V.na
         if deterministic or exploration_mode is None or not exploration.can_explore():
             pert = None
         else:
             pert = exploration.perturbation(self.cost_perturbation_method, size=(na, 1))
 
         grad_pert = pert if exploration_mode == "gradient-based" else None
```

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/agents/common/globopt_learning_agent.py` & `mpcrl-1.2.1rc2/src/mpcrl/agents/common/globopt_learning_agent.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/agents/common/learning_agent.py` & `mpcrl-1.2.1rc2/src/mpcrl/agents/common/learning_agent.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/agents/common/rl_learning_agent.py` & `mpcrl-1.2.1rc2/src/mpcrl/agents/common/rl_learning_agent.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/agents/lstd_dpg.py` & `mpcrl-1.2.1rc2/src/mpcrl/agents/lstd_dpg.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,16 +101,16 @@
             the updates of the learnable parameters, based on the current gradient-based
             RL algorithm.
         learnable_parameters : LearnableParametersDict
             A special dict containing the learnable parameters of the MPC, together with
             their bounds and values. This dict is complementary with `fixed_parameters`,
             which contains the MPC parameters that are not learnt by the agent.
         exploration : ExplorationStrategy, optional
-            Exploration strategy for inducing exploration in the MPC policy (it is
-            mandatory to explore in DPG).
+            Exploration strategy for inducing exploration in the online MPC policy (it
+            is mandatory to explore in DPG).
         fixed_parameters : dict[str, array_like] or collection of, optional
             A dict (or collection of dict, in case of `csnlp.MultistartNlp`) whose keys
             are the names of the MPC parameters and the values are their corresponding
             values. Use this to specify fixed parameters, that is, non-learnable. If
             `None`, then no fixed parameter is assumed.
         experience : int or ExperienceReplay, optional
             The container for experience replay memory. If `None` is passed, then a
```

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/agents/lstd_q_learning.py` & `mpcrl-1.2.1rc2/src/mpcrl/agents/lstd_q_learning.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy.typing as npt
 from csnlp import Solution
 from csnlp.wrappers import Mpc, NlpSensitivity
 from gymnasium import Env
 from typing_extensions import TypeAlias
 
 from ..core.experience import ExperienceReplay
-from ..core.exploration import ExplorationStrategy
+from ..core.exploration import ExplorationStrategy, NoExploration
 from ..core.parameters import LearnableParametersDict
 from ..core.update import UpdateStrategy
 from ..core.warmstart import WarmStartStrategy
 from ..optim.gradient_based_optimizer import GradientBasedOptimizer
 from .common.agent import ActType, ObsType, SymType
 from .common.rl_learning_agent import LrType, RlLearningAgent
 
@@ -96,16 +96,18 @@
             which contains the MPC parameters that are not learnt by the agent.
         fixed_parameters : dict[str, array_like] or collection of, optional
             A dict (or collection of dict, in case of `csnlp.MultistartNlp`) whose keys
             are the names of the MPC parameters and the values are their corresponding
             values. Use this to specify fixed parameters, that is, non-learnable. If
             `None`, then no fixed parameter is assumed.
         exploration : ExplorationStrategy, optional
-            Exploration strategy for inducing exploration in the MPC policy. By default
-            `None`, in which case `NoExploration` is used in the fixed-MPC agent.
+            Exploration strategy for inducing exploration in the online MPC policy. By
+            default `None`, in which case `NoExploration` is used. Should not be set
+            when offpolicy learning, as the exploration should be taken care in the
+            offpolicy data generation.
         experience : int or ExperienceReplay, optional
             The container for experience replay memory. If `None` is passed, then a
             memory with length 1 is created, i.e., it keeps only the latest memory
             transition.  If an integer `n` is passed, then a memory with the length `n`
             is created and with sample size `n`.
             In the case of LSTD Q-learning, each memory item consists of the action
             value function's gradient and hessian computed at each (succesful) env's
@@ -184,23 +186,27 @@
         raises: bool = True,
     ) -> float:
         truncated = terminated = False
         timestep = 0
         rewards = 0.0
         state = init_state
         action_space = getattr(env, "action_space", None)
+        # NOTE: if no exploration is set, then we can get away by solving one MPC per
+        # iteration, instead of two. The reason is that `a=argmin V(s)` and `min Q(s,a)`
+        # are the same thing, because `a` has not been modified by any perturbation.
+        no_exploration = isinstance(self.exploration, NoExploration)
 
         # solve for the first action
         action, solV = self.state_value(state, False, action_space=action_space)
         if not solV.success:
             self.on_mpc_failure(episode, None, solV.status, raises)
 
         while not (truncated or terminated):
-            # compute Q(s,a)
-            solQ = self.action_value(state, action)
+            # compute Q(s,a), or copy V(s) if no exploration is set
+            solQ = solV if no_exploration else self.action_value(state, action)
 
             # step the system with action computed at the previous iteration
             new_state, cost, truncated, terminated, _ = env.step(action)
             self.on_env_step(env, episode, timestep)
 
             # compute V(s+) and store transition
             new_action, solV = self.state_value(
@@ -244,19 +250,19 @@
     ) -> Union[
         Callable[[cs.DM], np.ndarray], Callable[[cs.DM], tuple[np.ndarray, np.ndarray]]
     ]:
         """Internal utility to compute the derivative of Q(s,a) w.r.t. the learnable
         parameters, a.k.a., theta."""
         order = self.optimizer._order
         theta = cs.vvcat(self._learnable_pars.sym.values())
-        nlp = self._Q.nlp
+        nlp = (self._V if isinstance(self.exploration, NoExploration) else self._Q).nlp
         x_lam_p = cs.vertcat(nlp.primal_dual, nlp.p)
 
         # compute first order sensitivity
-        snlp = NlpSensitivity(self._Q.nlp, theta)
+        snlp = NlpSensitivity(nlp, theta)
         gradient = snlp.jacobians["L-p"]  # exact gradient, i.e., dQ/dtheta
 
         if hessian_type == "none":
             assert order == 1, "Expected 1st-order optimizer with `hessian_type=none`."
 
             sensitivity = cs.Function(
                 "S", (x_lam_p,), (gradient,), ("x_lam_p",), ("dQ",), {"cse": True}
```

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/core/callbacks.py` & `mpcrl-1.2.1rc2/src/mpcrl/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/core/errors.py` & `mpcrl-1.2.1rc2/src/mpcrl/core/errors.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/core/experience.py` & `mpcrl-1.2.1rc2/src/mpcrl/core/experience.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/core/exploration.py` & `mpcrl-1.2.1rc2/src/mpcrl/core/exploration.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,14 +84,17 @@
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(hook={self.hook},mode={self.mode})"
 
 
 class NoExploration(ExplorationStrategy):
     """Strategy where no exploration is allowed at any time or, in other words, the
     policy is always deterministic (only based on the current state, and not perturbed).
+
+    This is a special kind of `ExplorationStrategy`, the only one without any
+    `hook` and `mode`.
     """
 
     def __init__(self) -> None:
         """Instiates a no-exploration strategy."""
         super().__init__()
         del self._hook, self._mode
 
@@ -260,15 +263,15 @@
             epsilon = NoScheduling[float](epsilon)
         self.epsilon_scheduler = epsilon
 
     @property
     def hook(
         self,
     ) -> Optional[Literal["on_update", "on_episode_end", "on_timestep_end"]]:
-        # return hook only if the strength or epislon scheduler requires to be stepped
+        # return hook only if the strength or epsilon scheduler requires to be stepped
         return (
             None
             if isinstance(self.strength_scheduler, NoScheduling)
             and isinstance(self.epsilon_scheduler, NoScheduling)
             else self._hook
         )
 
@@ -284,14 +287,129 @@
     def __repr__(self) -> str:
         clsn = self.__class__.__name__
         eps = self.epsilon_scheduler.value
         stn = self.strength_scheduler.value
         return f"{clsn}(eps={eps},stn={stn},hook={self.hook},mode={self.mode})"
 
 
+class OrnsteinUhlenbeckExploration(ExplorationStrategy):
+    """
+    Exploraiton based on the Ornstein-Uhlenbeck Brownian motion with friction. See
+    implementation from  https://github.com/DLR-RM/stable-baselines3/tree/master.
+
+    Note: since this exploration strategy creates a particular noise process, it is
+    independent of the agent's `cost_perturbation_method` field.
+    """
+
+    def __init__(
+        self,
+        mean: Union[Scheduler[npt.NDArray[np.floating]], npt.NDArray[np.floating]],
+        sigma: Union[Scheduler[npt.NDArray[np.floating]], npt.NDArray[np.floating]],
+        theta: float = 0.15,
+        dt: float = 1.0,
+        initial_noise: Optional[npt.ArrayLike] = None,
+        hook: Literal["on_update", "on_episode_end", "on_timestep_end"] = "on_update",
+        mode: Literal["gradient-based", "additive"] = "gradient-based",
+        seed: RngType = None,
+    ) -> None:
+        """Creates a new Ornstein-Uhlenbeck exploration strategy.
+
+        Parameters
+        ----------
+        mean : scheduler or array/supports-algebraic-operations
+            Mean of the stochastic process. Should have the same shape as the action.
+        sigma : scheduler or array/supports-algebraic-operations
+            Standard deviation of the stochastic process. Should have the same shape as
+            the action.
+        theta : float, optional
+            Coefficient of attraction of the process towards mean, by default `0.15`.
+        dt : float, optional
+            Time step of the process, by default `1.0`.
+        initial_noise : array-like, optional
+            A default initial noise. By default `None`, in which case it is set to zero.
+        hook : {'on_update', 'on_episode_end', 'on_timestep_end'}, optional
+            Specifies to which callback to hook, i.e., when to step the exploration's
+            schedulers (if any) to, e.g., decay the chances of exploring or the
+            perturbation strength (see `step` method also). The options are:
+             - `on_update` steps the exploration after each agent's update
+             - `on_episode_end` steps the exploration after each episode's end
+             - `on_timestep_end` steps the exploration after each env's timestep.
+
+            By default, 'on_update' is selected.
+        mode : {'gradient-based', 'additive'} optional
+            Mode of application of explorative perturbations to the MPC. If `additive`,
+            then the drawn pertubation is added to the optimal action computed by the
+            MPC. By default, `gradient-based` is selected, and in this mode the
+            pertubations enter  directly in the MPC objective and multiplied by the
+            first action, thus affecting its gradient.
+        seed : None, int, array_like[ints], SeedSequence, BitGenerator, Generator
+            Number to seed the RNG engine used for randomizing the exploration. By
+            default, `None`.
+        """
+        super().__init__(hook, mode)
+        if not isinstance(mean, Scheduler):
+            mean = NoScheduling[npt.NDArray[np.floating]](mean)
+        self.mean_scheduler = mean
+        if not isinstance(sigma, Scheduler):
+            sigma = NoScheduling[npt.NDArray[np.floating]](sigma)
+        self.sigma_scheduler = sigma
+        self.theta = theta
+        self.dt = dt
+        self.initial_noise = initial_noise
+        self.reset(seed)
+
+    @property
+    def hook(
+        self,
+    ) -> Optional[Literal["on_update", "on_episode_end", "on_timestep_end"]]:
+        # return hook only if the mean or sigma scheduler requires to be stepped
+        return (
+            None
+            if isinstance(self.mean_scheduler, NoScheduling)
+            and isinstance(self.sigma_scheduler, NoScheduling)
+            else self._hook
+        )
+
+    def reset(self, seed: RngType = None) -> None:
+        """Resets the exploration RNG."""
+        self.np_random = np.random.default_rng(seed)
+        self._prev_noise = (
+            np.zeros_like(self.mean_scheduler.value)
+            if self.initial_noise is None
+            else np.asarray(self.initial_noise)
+        )
+
+    def can_explore(self) -> bool:
+        return True
+
+    def step(self, *_, **__) -> None:
+        """Updates the mean and std of the noise according to their schedulers."""
+        self.mean_scheduler.step()
+        self.sigma_scheduler.step()
+
+    def perturbation(self, *_: Any, **__: Any) -> npt.NDArray[np.floating]:
+        sigma = self.sigma_scheduler.value
+        noise = (
+            self._prev_noise
+            + (self.theta * self.dt) * (self.mean_scheduler.value - self._prev_noise)
+            + np.sqrt(self.dt) * (sigma * self.np_random.normal(size=np.shape(sigma)))
+        )
+        self._prev_noise = noise
+        return noise
+
+    def __repr__(self) -> str:
+        clsn = self.__class__.__name__
+        mean = self.mean_scheduler.value
+        sigma = self.sigma_scheduler.value
+        return (
+            f"{clsn}(mean={mean},sigma={sigma},theta={self.theta},dt={self.dt},"
+            f"hook={self.hook},mode={self.mode})"
+        )
+
+
 class StepWiseExploration(ExplorationStrategy):
     """Wrapper exploration class that enables a base exploration strategy to change only
     every N steps, thus yielding a step-wise strategy with steps of the given length.
     This is useful when, e.g., the exploration strategy must be kept constant across
     time for a number of steps.
 
     Note
```

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/core/parameters.py` & `mpcrl-1.2.1rc2/src/mpcrl/core/parameters.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/core/schedulers.py` & `mpcrl-1.2.1rc2/src/mpcrl/core/schedulers.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/core/update.py` & `mpcrl-1.2.1rc2/src/mpcrl/core/update.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/core/warmstart.py` & `mpcrl-1.2.1rc2/src/mpcrl/core/warmstart.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/optim/adam.py` & `mpcrl-1.2.1rc2/src/mpcrl/optim/adam.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/optim/base_optimizer.py` & `mpcrl-1.2.1rc2/src/mpcrl/optim/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/optim/gradient_based_optimizer.py` & `mpcrl-1.2.1rc2/src/mpcrl/optim/gradient_based_optimizer.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/optim/gradient_descent.py` & `mpcrl-1.2.1rc2/src/mpcrl/optim/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/optim/gradient_free_optimizer.py` & `mpcrl-1.2.1rc2/src/mpcrl/optim/gradient_free_optimizer.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/optim/newton_method.py` & `mpcrl-1.2.1rc2/src/mpcrl/optim/newton_method.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/optim/rmsprop.py` & `mpcrl-1.2.1rc2/src/mpcrl/optim/rmsprop.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/util/control.py` & `mpcrl-1.2.1rc2/src/mpcrl/util/control.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/util/iters.py` & `mpcrl-1.2.1rc2/src/mpcrl/util/iters.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/util/math.py` & `mpcrl-1.2.1rc2/src/mpcrl/util/math.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/util/named.py` & `mpcrl-1.2.1rc2/src/mpcrl/util/named.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/util/seeding.py` & `mpcrl-1.2.1rc2/src/mpcrl/util/seeding.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/evaluate.py` & `mpcrl-1.2.1rc2/src/mpcrl/wrappers/agents/evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         agent: LearningAgent[SymType, ExpType],
         eval_env: Env[ObsType, ActType],
         hook: Literal["on_episode_end", "on_timestep_end", "on_update"],
         frequency: int,
         n_eval_episodes: int = 1,
         eval_immediately: bool = False,
         *,
-        deterministic: bool = False,
+        deterministic: bool = True,
         seed: RngType = None,
         raises: bool = True,
         env_reset_options: Optional[dict[str, Any]] = None,
         fix_seed: bool = False,
     ) -> None:
         """Creates an instance of the evaluation wrapper around the agent.
```

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/log.py` & `mpcrl-1.2.1rc2/src/mpcrl/wrappers/agents/log.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/record_updates.py` & `mpcrl-1.2.1rc2/src/mpcrl/wrappers/agents/record_updates.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/wrappers/agents/wrapper.py` & `mpcrl-1.2.1rc2/src/mpcrl/wrappers/agents/wrapper.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/wrappers/envs/monitor_episodes.py` & `mpcrl-1.2.1rc2/src/mpcrl/wrappers/envs/monitor_episodes.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl/wrappers/envs/monitor_infos.py` & `mpcrl-1.2.1rc2/src/mpcrl/wrappers/envs/monitor_infos.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/src/mpcrl.egg-info/PKG-INFO` & `mpcrl-1.2.1rc2/src/mpcrl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcrl
-Version: 1.2.1rc1
+Version: 1.2.1rc2
 Summary: Reinforcement Learning with Model Predictive Control
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/mpc-reinforcement-learning
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues
 Keywords: reinforcement-learning,model-predictive-control,optimization,casadi
 Classifier: Programming Language :: Python
@@ -18,15 +18,15 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions>=4.5.0
 Requires-Dist: numba>=0.57.1
-Requires-Dist: csnlp>=1.5.10
+Requires-Dist: csnlp>=1.5.11rc2
 Requires-Dist: scipy>=1.11.0
 Requires-Dist: gymnasium>=0.28.1
 
 # Reinforcement Learning with Model Predictive Control
 
 **mpcrl** is a library for training model-based Reinforcement Learning (RL) agents with Model Predictive Control (MPC) as function approximation. This framework, also known as MPC-based RL, was first proposed in [[1]](#1) and has so far been shown effective in various applications and with different learning algorithms, e.g., [[2](#2),[3](#3)].
```

### Comparing `mpcrl-1.2.1rc1/src/mpcrl.egg-info/SOURCES.txt` & `mpcrl-1.2.1rc2/src/mpcrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/tests/test_agent.py` & `mpcrl-1.2.1rc2/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/tests/test_core.py` & `mpcrl-1.2.1rc2/tests/test_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -274,14 +274,21 @@
         self.assertIsInstance(exploration.np_random, np.random.Generator)
 
     def test_greedy_exploration__always_explores(self):
         exploration = E.GreedyExploration(strength=0.5)
         self.assertTrue(exploration.can_explore())
         do_test_str_and_repr(self, exploration)
 
+    @parameterized.expand(((False,), (True,)))
+    def test_greedy_exploration__hook(self, strength):
+        strength_scheduler = S.LinearScheduler(0, 1, 10) if strength else 0
+        exploration = E.GreedyExploration(strength_scheduler)
+        hook = exploration.hook
+        self.assertEqual(hook is not None, strength)
+
     @parameterized.expand([("uniform",), ("normal",), ("standard_normal",)])
     def test_greedy_exploration__perturbs(self, method: str):
         exploration = E.GreedyExploration(strength=0.5)
         exploration.perturbation(method)
 
     def test_epsilon_greedy_exploration__never_explores__with_zero_epsilon(self):
         epsilon, epsilon_decay_rate = 0.0, 0.75
@@ -326,14 +333,49 @@
         )
 
         exploration.step()
 
         epsilon_scheduler.step.assert_called_once()
         strength_scheduler.step.assert_called_once()
 
+    @parameterized.expand(product([False, True], [False, True]))
+    def test_epsilon_greedy_exploration__hook(self, epsilon, strength):
+        epsilon_scheduler = S.LinearScheduler(0, 1, 10) if epsilon else 0
+        strength_scheduler = S.LinearScheduler(0, 1, 10) if strength else 0
+        exploration = E.EpsilonGreedyExploration(epsilon_scheduler, strength_scheduler)
+        hook = exploration.hook
+        self.assertEqual(hook is not None, epsilon or strength)
+
+    def test_ornsteinuhlenbeck_exploration__always_explores(self):
+        exploration = E.OrnsteinUhlenbeckExploration(0, 0.5)
+        self.assertTrue(exploration.can_explore())
+
+    def test_ornsteinuhlenbeck_exploration__decays_mean_and_sigma(self):
+        class MockScheduler(S.NoScheduling):
+            ...
+
+        mean_scheduler = MockScheduler(None)
+        sigma_scheduler = MockScheduler(None)
+        mean_scheduler.step = Mock()
+        sigma_scheduler.step = Mock()
+        exploration = E.OrnsteinUhlenbeckExploration(mean_scheduler, sigma_scheduler)
+
+        exploration.step()
+
+        mean_scheduler.step.assert_called_once()
+        sigma_scheduler.step.assert_called_once()
+
+    @parameterized.expand(product([False, True], [False, True]))
+    def test_ornsteinuhlenbeck_exploration__hook(self, mean, sigma):
+        mean_scheduler = S.LinearScheduler(0, 1, 10) if mean else 0
+        sigma_scheduler = S.LinearScheduler(0, 1, 10) if sigma else 0
+        exploration = E.OrnsteinUhlenbeckExploration(mean_scheduler, sigma_scheduler)
+        hook = exploration.hook
+        self.assertEqual(hook is not None, mean or sigma)
+
     def test_stepwise_exploration__has_same_hook_and_mode_as_base_exploration(self):
         hook, mode = Mock(), Mock()
         base_exploration = Mock()
         base_exploration.hook = hook
         base_exploration.mode = mode
         exploration = E.StepWiseExploration(base_exploration, 5, 10)
         self.assertIs(exploration.hook, hook)
```

### Comparing `mpcrl-1.2.1rc1/tests/test_examples.py` & `mpcrl-1.2.1rc2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/tests/test_optim.py` & `mpcrl-1.2.1rc2/tests/test_optim.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/tests/test_util.py` & `mpcrl-1.2.1rc2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.2.1rc1/tests/test_wrappers.py` & `mpcrl-1.2.1rc2/tests/test_wrappers.py`

 * *Files identical despite different names*

