# Comparing `tmp/torchbringer-0.2.3.tar.gz` & `tmp/torchbringer-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbringer-0.2.3.tar", last modified: Mon May 27 18:48:08 2024, max compression
+gzip compressed data, was "torchbringer-0.2.4.tar", last modified: Mon May 27 19:06:48 2024, max compression
```

## Comparing `torchbringer-0.2.3.tar` & `torchbringer-0.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.103092 torchbringer-0.2.3/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-27 00:48:39.000000 torchbringer-0.2.3/LICENSE
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 18:48:08.103092 torchbringer-0.2.3/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6547 2024-05-27 00:48:39.000000 torchbringer-0.2.3/README.md
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-27 18:48:08.103092 torchbringer-0.2.3/setup.cfg
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1155 2024-05-27 18:47:59.000000 torchbringer-0.2.3/setup.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.093092 torchbringer-0.2.3/torchbringer/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-27 18:48:04.000000 torchbringer-0.2.3/torchbringer/__init__.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.093092 torchbringer-0.2.3/torchbringer/components/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2851 2024-05-27 12:38:47.000000 torchbringer-0.2.3/torchbringer/components/builders.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      781 2024-05-27 02:31:46.000000 torchbringer-0.2.3/torchbringer/components/epsilon.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/components/replay_memory.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.093092 torchbringer-0.2.3/torchbringer/examples/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5040 2024-05-27 18:46:40.000000 torchbringer-0.2.3/torchbringer/examples/breakout_local_dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/examples/cartpole_grpc_dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-27 14:59:27.000000 torchbringer-0.2.3/torchbringer/examples/cartpole_local_dqn.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.093092 torchbringer-0.2.3/torchbringer/learners/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5286 2024-05-27 18:40:02.000000 torchbringer-0.2.3/torchbringer/learners/dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/learners/learner_utils.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.093092 torchbringer-0.2.3/torchbringer/servers/
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.103092 torchbringer-0.2.3/torchbringer/servers/grpc/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_grpc_client.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_grpc_server.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_pb2.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_pb2.pyi
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      840 2024-05-27 18:44:28.000000 torchbringer-0.2.3/torchbringer/servers/torchbringer_agent.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.103092 torchbringer-0.2.3/torchbringer.egg-info/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 18:48:07.000000 torchbringer-0.2.3/torchbringer.egg-info/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      836 2024-05-27 18:48:08.000000 torchbringer-0.2.3/torchbringer.egg-info/SOURCES.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-27 18:48:07.000000 torchbringer-0.2.3/torchbringer.egg-info/dependency_links.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       98 2024-05-27 18:48:07.000000 torchbringer-0.2.3/torchbringer.egg-info/requires.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-27 18:48:07.000000 torchbringer-0.2.3/torchbringer.egg-info/top_level.txt
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:06:48.393087 torchbringer-0.2.4/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-27 00:48:39.000000 torchbringer-0.2.4/LICENSE
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 19:06:48.393087 torchbringer-0.2.4/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6547 2024-05-27 00:48:39.000000 torchbringer-0.2.4/README.md
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-27 19:06:48.393087 torchbringer-0.2.4/setup.cfg
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1155 2024-05-27 19:06:22.000000 torchbringer-0.2.4/setup.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:06:48.383087 torchbringer-0.2.4/torchbringer/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-27 19:05:40.000000 torchbringer-0.2.4/torchbringer/__init__.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:06:48.383087 torchbringer-0.2.4/torchbringer/components/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2851 2024-05-27 12:38:47.000000 torchbringer-0.2.4/torchbringer/components/builders.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      781 2024-05-27 02:31:46.000000 torchbringer-0.2.4/torchbringer/components/epsilon.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-27 00:48:39.000000 torchbringer-0.2.4/torchbringer/components/replay_memory.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:06:48.383087 torchbringer-0.2.4/torchbringer/examples/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5041 2024-05-27 19:06:34.000000 torchbringer-0.2.4/torchbringer/examples/breakout_local_dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-27 00:48:39.000000 torchbringer-0.2.4/torchbringer/examples/cartpole_grpc_dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-27 14:59:27.000000 torchbringer-0.2.4/torchbringer/examples/cartpole_local_dqn.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:06:48.383087 torchbringer-0.2.4/torchbringer/learners/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5286 2024-05-27 18:40:02.000000 torchbringer-0.2.4/torchbringer/learners/dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-27 00:48:39.000000 torchbringer-0.2.4/torchbringer/learners/learner_utils.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:06:48.383087 torchbringer-0.2.4/torchbringer/servers/
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:06:48.393087 torchbringer-0.2.4/torchbringer/servers/grpc/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-27 00:48:39.000000 torchbringer-0.2.4/torchbringer/servers/grpc/torchbringer_grpc_client.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-27 00:48:39.000000 torchbringer-0.2.4/torchbringer/servers/grpc/torchbringer_grpc_server.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-27 00:48:39.000000 torchbringer-0.2.4/torchbringer/servers/grpc/torchbringer_pb2.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-27 00:48:39.000000 torchbringer-0.2.4/torchbringer/servers/grpc/torchbringer_pb2.pyi
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-27 00:48:39.000000 torchbringer-0.2.4/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      840 2024-05-27 18:44:28.000000 torchbringer-0.2.4/torchbringer/servers/torchbringer_agent.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:06:48.393087 torchbringer-0.2.4/torchbringer.egg-info/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 19:06:48.000000 torchbringer-0.2.4/torchbringer.egg-info/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      836 2024-05-27 19:06:48.000000 torchbringer-0.2.4/torchbringer.egg-info/SOURCES.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-27 19:06:48.000000 torchbringer-0.2.4/torchbringer.egg-info/dependency_links.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       98 2024-05-27 19:06:48.000000 torchbringer-0.2.4/torchbringer.egg-info/requires.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-27 19:06:48.000000 torchbringer-0.2.4/torchbringer.egg-info/top_level.txt
```

### Comparing `torchbringer-0.2.3/LICENSE` & `torchbringer-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.3/PKG-INFO` & `torchbringer-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbringer
-Version: 0.2.3
+Version: 0.2.4
 Summary: A PyTorch library for deep reinforcement learning 
 Home-page: https://github.com/moraguma/TorchBringer
 Author: Moraguma
 Author-email: g170603@dac.unicamp.br
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchbringer-0.2.3/README.md` & `torchbringer-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.3/setup.py` & `torchbringer-0.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='torchbringer',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.2.3',    
+    version='0.2.4',    
     description='A PyTorch library for deep reinforcement learning ',
     url='https://github.com/moraguma/TorchBringer',
     author='Moraguma',
     author_email='g170603@dac.unicamp.br',
     license='MIT',
     packages=find_namespace_packages(),
     install_requires=[
```

### Comparing `torchbringer-0.2.3/torchbringer/components/builders.py` & `torchbringer-0.2.4/torchbringer/components/builders.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.3/torchbringer/components/epsilon.py` & `torchbringer-0.2.4/torchbringer/components/epsilon.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.3/torchbringer/components/replay_memory.py` & `torchbringer-0.2.4/torchbringer/components/replay_memory.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.3/torchbringer/examples/breakout_local_dqn.py` & `torchbringer-0.2.4/torchbringer/examples/breakout_local_dqn.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     "tau": 0.005,
     "epsilon": {
         "type": "lin_decrease",
         "start": 1.0,
         "end": 0.1,
         "steps_to_end": 1000000
     },
-    "batch_size": 2,
+    "batch_size": 32,
     "grad_clip_value": 100,
     "loss": "smooth_l1_loss",
     "optimizer": {
         "type": "adamw",
         "lr": 1e-4, 
         "amsgrad": True
     },
```

### Comparing `torchbringer-0.2.3/torchbringer/examples/cartpole_grpc_dqn.py` & `torchbringer-0.2.4/torchbringer/examples/cartpole_grpc_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.3/torchbringer/examples/cartpole_local_dqn.py` & `torchbringer-0.2.4/torchbringer/examples/cartpole_local_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.3/torchbringer/learners/dqn.py` & `torchbringer-0.2.4/torchbringer/learners/dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_grpc_client.py` & `torchbringer-0.2.4/torchbringer/servers/grpc/torchbringer_grpc_client.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_grpc_server.py` & `torchbringer-0.2.4/torchbringer/servers/grpc/torchbringer_grpc_server.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_pb2.py` & `torchbringer-0.2.4/torchbringer/servers/grpc/torchbringer_pb2.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_pb2.pyi` & `torchbringer-0.2.4/torchbringer/servers/grpc/torchbringer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_pb2_grpc.py` & `torchbringer-0.2.4/torchbringer/servers/grpc/torchbringer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.3/torchbringer/servers/torchbringer_agent.py` & `torchbringer-0.2.4/torchbringer/servers/torchbringer_agent.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.3/torchbringer.egg-info/PKG-INFO` & `torchbringer-0.2.4/torchbringer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbringer
-Version: 0.2.3
+Version: 0.2.4
 Summary: A PyTorch library for deep reinforcement learning 
 Home-page: https://github.com/moraguma/TorchBringer
 Author: Moraguma
 Author-email: g170603@dac.unicamp.br
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchbringer-0.2.3/torchbringer.egg-info/SOURCES.txt` & `torchbringer-0.2.4/torchbringer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

