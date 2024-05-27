# Comparing `tmp/torchbringer-0.2.5.tar.gz` & `tmp/torchbringer-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbringer-0.2.5.tar", last modified: Mon May 27 19:41:01 2024, max compression
+gzip compressed data, was "torchbringer-0.2.6.tar", last modified: Mon May 27 20:00:25 2024, max compression
```

## Comparing `torchbringer-0.2.5.tar` & `torchbringer-0.2.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:41:01.283092 torchbringer-0.2.5/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-27 00:48:39.000000 torchbringer-0.2.5/LICENSE
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 19:41:01.283092 torchbringer-0.2.5/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6547 2024-05-27 00:48:39.000000 torchbringer-0.2.5/README.md
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-27 19:41:01.283092 torchbringer-0.2.5/setup.cfg
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1155 2024-05-27 19:40:48.000000 torchbringer-0.2.5/setup.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:41:01.273092 torchbringer-0.2.5/torchbringer/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-27 19:40:56.000000 torchbringer-0.2.5/torchbringer/__init__.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:41:01.273092 torchbringer-0.2.5/torchbringer/components/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2939 2024-05-27 19:36:45.000000 torchbringer-0.2.5/torchbringer/components/builders.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      781 2024-05-27 02:31:46.000000 torchbringer-0.2.5/torchbringer/components/epsilon.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      208 2024-05-27 19:35:27.000000 torchbringer-0.2.5/torchbringer/components/layers.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-27 00:48:39.000000 torchbringer-0.2.5/torchbringer/components/replay_memory.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:41:01.273092 torchbringer-0.2.5/torchbringer/examples/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5109 2024-05-27 19:40:23.000000 torchbringer-0.2.5/torchbringer/examples/breakout_local_dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-27 00:48:39.000000 torchbringer-0.2.5/torchbringer/examples/cartpole_grpc_dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-27 14:59:27.000000 torchbringer-0.2.5/torchbringer/examples/cartpole_local_dqn.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:41:01.273092 torchbringer-0.2.5/torchbringer/learners/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5286 2024-05-27 18:40:02.000000 torchbringer-0.2.5/torchbringer/learners/dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-27 00:48:39.000000 torchbringer-0.2.5/torchbringer/learners/learner_utils.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:41:01.273092 torchbringer-0.2.5/torchbringer/servers/
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:41:01.283092 torchbringer-0.2.5/torchbringer/servers/grpc/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-27 00:48:39.000000 torchbringer-0.2.5/torchbringer/servers/grpc/torchbringer_grpc_client.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-27 00:48:39.000000 torchbringer-0.2.5/torchbringer/servers/grpc/torchbringer_grpc_server.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-27 00:48:39.000000 torchbringer-0.2.5/torchbringer/servers/grpc/torchbringer_pb2.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-27 00:48:39.000000 torchbringer-0.2.5/torchbringer/servers/grpc/torchbringer_pb2.pyi
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-27 00:48:39.000000 torchbringer-0.2.5/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      840 2024-05-27 18:44:28.000000 torchbringer-0.2.5/torchbringer/servers/torchbringer_agent.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 19:41:01.283092 torchbringer-0.2.5/torchbringer.egg-info/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 19:41:01.000000 torchbringer-0.2.5/torchbringer.egg-info/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      870 2024-05-27 19:41:01.000000 torchbringer-0.2.5/torchbringer.egg-info/SOURCES.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-27 19:41:01.000000 torchbringer-0.2.5/torchbringer.egg-info/dependency_links.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       98 2024-05-27 19:41:01.000000 torchbringer-0.2.5/torchbringer.egg-info/requires.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-27 19:41:01.000000 torchbringer-0.2.5/torchbringer.egg-info/top_level.txt
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 20:00:25.563094 torchbringer-0.2.6/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-27 00:48:39.000000 torchbringer-0.2.6/LICENSE
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 20:00:25.563094 torchbringer-0.2.6/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6547 2024-05-27 00:48:39.000000 torchbringer-0.2.6/README.md
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-27 20:00:25.563094 torchbringer-0.2.6/setup.cfg
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1155 2024-05-27 20:00:10.000000 torchbringer-0.2.6/setup.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 20:00:25.563094 torchbringer-0.2.6/torchbringer/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-27 20:00:13.000000 torchbringer-0.2.6/torchbringer/__init__.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 20:00:25.563094 torchbringer-0.2.6/torchbringer/components/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2939 2024-05-27 19:36:45.000000 torchbringer-0.2.6/torchbringer/components/builders.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      781 2024-05-27 02:31:46.000000 torchbringer-0.2.6/torchbringer/components/epsilon.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      208 2024-05-27 19:35:27.000000 torchbringer-0.2.6/torchbringer/components/layers.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-27 00:48:39.000000 torchbringer-0.2.6/torchbringer/components/replay_memory.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 20:00:25.563094 torchbringer-0.2.6/torchbringer/examples/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5107 2024-05-27 20:00:03.000000 torchbringer-0.2.6/torchbringer/examples/breakout_local_dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-27 00:48:39.000000 torchbringer-0.2.6/torchbringer/examples/cartpole_grpc_dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-27 14:59:27.000000 torchbringer-0.2.6/torchbringer/examples/cartpole_local_dqn.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 20:00:25.563094 torchbringer-0.2.6/torchbringer/learners/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5286 2024-05-27 18:40:02.000000 torchbringer-0.2.6/torchbringer/learners/dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-27 00:48:39.000000 torchbringer-0.2.6/torchbringer/learners/learner_utils.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 20:00:25.563094 torchbringer-0.2.6/torchbringer/servers/
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 20:00:25.563094 torchbringer-0.2.6/torchbringer/servers/grpc/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-27 00:48:39.000000 torchbringer-0.2.6/torchbringer/servers/grpc/torchbringer_grpc_client.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-27 00:48:39.000000 torchbringer-0.2.6/torchbringer/servers/grpc/torchbringer_grpc_server.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-27 00:48:39.000000 torchbringer-0.2.6/torchbringer/servers/grpc/torchbringer_pb2.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-27 00:48:39.000000 torchbringer-0.2.6/torchbringer/servers/grpc/torchbringer_pb2.pyi
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-27 00:48:39.000000 torchbringer-0.2.6/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      840 2024-05-27 18:44:28.000000 torchbringer-0.2.6/torchbringer/servers/torchbringer_agent.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 20:00:25.563094 torchbringer-0.2.6/torchbringer.egg-info/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 20:00:25.000000 torchbringer-0.2.6/torchbringer.egg-info/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      870 2024-05-27 20:00:25.000000 torchbringer-0.2.6/torchbringer.egg-info/SOURCES.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-27 20:00:25.000000 torchbringer-0.2.6/torchbringer.egg-info/dependency_links.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       98 2024-05-27 20:00:25.000000 torchbringer-0.2.6/torchbringer.egg-info/requires.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-27 20:00:25.000000 torchbringer-0.2.6/torchbringer.egg-info/top_level.txt
```

### Comparing `torchbringer-0.2.5/LICENSE` & `torchbringer-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.5/PKG-INFO` & `torchbringer-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbringer
-Version: 0.2.5
+Version: 0.2.6
 Summary: A PyTorch library for deep reinforcement learning 
 Home-page: https://github.com/moraguma/TorchBringer
 Author: Moraguma
 Author-email: g170603@dac.unicamp.br
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchbringer-0.2.5/README.md` & `torchbringer-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.5/setup.py` & `torchbringer-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='torchbringer',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.2.5',    
+    version='0.2.6',    
     description='A PyTorch library for deep reinforcement learning ',
     url='https://github.com/moraguma/TorchBringer',
     author='Moraguma',
     author_email='g170603@dac.unicamp.br',
     license='MIT',
     packages=find_namespace_packages(),
     install_requires=[
```

### Comparing `torchbringer-0.2.5/torchbringer/components/builders.py` & `torchbringer-0.2.6/torchbringer/components/builders.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.5/torchbringer/components/epsilon.py` & `torchbringer-0.2.6/torchbringer/components/epsilon.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.5/torchbringer/components/replay_memory.py` & `torchbringer-0.2.6/torchbringer/components/replay_memory.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.5/torchbringer/examples/breakout_local_dqn.py` & `torchbringer-0.2.6/torchbringer/examples/breakout_local_dqn.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     
     state = torch.tensor(state, dtype=torch.float32, device=device).unsqueeze(0)
     for t in count():
         observation, reward, terminated, truncated, _ = env.step(dqn.step(state, reward, terminal).item())
         cummulative_reward += reward
         cummulative_loss += dqn.get_past_loss()
 
-        state = None if terminated else torch.tensor(observation, dtype=torch.float32, device=device).unsqueeze(0) 
+        state = None if terminated else torch.tensor(observation, dtype=torch.uint8, device=device).unsqueeze(0) 
         reward = torch.tensor([reward], device=device)
         terminal = terminated or truncated
 
         frames_done += 1
         if frames_done % log_interval == 0:
             current_time = time.time()
             print("Finished %d/%d frames in %s - ETR: %ss; TE: %ss" % (frames_done, total_frames, datetime.timedelta(seconds=int(current_time - last_log_time)), datetime.timedelta(seconds=int((current_time - starting_time) / frames_done * (total_frames - frames_done))), datetime.timedelta(seconds=int(current_time - starting_time))))
```

### Comparing `torchbringer-0.2.5/torchbringer/examples/cartpole_grpc_dqn.py` & `torchbringer-0.2.6/torchbringer/examples/cartpole_grpc_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.5/torchbringer/examples/cartpole_local_dqn.py` & `torchbringer-0.2.6/torchbringer/examples/cartpole_local_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.5/torchbringer/learners/dqn.py` & `torchbringer-0.2.6/torchbringer/learners/dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.5/torchbringer/servers/grpc/torchbringer_grpc_client.py` & `torchbringer-0.2.6/torchbringer/servers/grpc/torchbringer_grpc_client.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.5/torchbringer/servers/grpc/torchbringer_grpc_server.py` & `torchbringer-0.2.6/torchbringer/servers/grpc/torchbringer_grpc_server.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.5/torchbringer/servers/grpc/torchbringer_pb2.py` & `torchbringer-0.2.6/torchbringer/servers/grpc/torchbringer_pb2.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.5/torchbringer/servers/grpc/torchbringer_pb2.pyi` & `torchbringer-0.2.6/torchbringer/servers/grpc/torchbringer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.5/torchbringer/servers/grpc/torchbringer_pb2_grpc.py` & `torchbringer-0.2.6/torchbringer/servers/grpc/torchbringer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.5/torchbringer/servers/torchbringer_agent.py` & `torchbringer-0.2.6/torchbringer/servers/torchbringer_agent.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.5/torchbringer.egg-info/PKG-INFO` & `torchbringer-0.2.6/torchbringer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbringer
-Version: 0.2.5
+Version: 0.2.6
 Summary: A PyTorch library for deep reinforcement learning 
 Home-page: https://github.com/moraguma/TorchBringer
 Author: Moraguma
 Author-email: g170603@dac.unicamp.br
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchbringer-0.2.5/torchbringer.egg-info/SOURCES.txt` & `torchbringer-0.2.6/torchbringer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

