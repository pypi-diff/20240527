# Comparing `tmp/torchbringer-0.2.0.tar.gz` & `tmp/torchbringer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbringer-0.2.0.tar", last modified: Mon May 27 13:10:27 2024, max compression
+gzip compressed data, was "torchbringer-0.2.1.tar", last modified: Mon May 27 15:07:29 2024, max compression
```

## Comparing `torchbringer-0.2.0.tar` & `torchbringer-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.573182 torchbringer-0.2.0/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-27 00:48:39.000000 torchbringer-0.2.0/LICENSE
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 13:10:27.573182 torchbringer-0.2.0/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6547 2024-05-27 00:48:39.000000 torchbringer-0.2.0/README.md
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-27 13:10:27.573182 torchbringer-0.2.0/setup.cfg
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1155 2024-05-27 13:07:40.000000 torchbringer-0.2.0/setup.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.553182 torchbringer-0.2.0/torchbringer/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-27 13:07:32.000000 torchbringer-0.2.0/torchbringer/__init__.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.553182 torchbringer-0.2.0/torchbringer/components/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2851 2024-05-27 12:38:47.000000 torchbringer-0.2.0/torchbringer/components/builders.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      781 2024-05-27 02:31:46.000000 torchbringer-0.2.0/torchbringer/components/epsilon.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/components/replay_memory.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.563182 torchbringer-0.2.0/torchbringer/examples/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     4153 2024-05-27 13:06:27.000000 torchbringer-0.2.0/torchbringer/examples/breakout_local_dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/examples/cartpole_grpc_dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/examples/cartpole_local_dqn.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.563182 torchbringer-0.2.0/torchbringer/learners/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5210 2024-05-27 13:04:44.000000 torchbringer-0.2.0/torchbringer/learners/dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/learners/learner_utils.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.563182 torchbringer-0.2.0/torchbringer/servers/
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.573182 torchbringer-0.2.0/torchbringer/servers/grpc/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_grpc_client.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_grpc_server.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_pb2.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_pb2.pyi
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      583 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/servers/torchbringer_agent.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.573182 torchbringer-0.2.0/torchbringer.egg-info/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 13:10:27.000000 torchbringer-0.2.0/torchbringer.egg-info/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      836 2024-05-27 13:10:27.000000 torchbringer-0.2.0/torchbringer.egg-info/SOURCES.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-27 13:10:27.000000 torchbringer-0.2.0/torchbringer.egg-info/dependency_links.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       98 2024-05-27 13:10:27.000000 torchbringer-0.2.0/torchbringer.egg-info/requires.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-27 13:10:27.000000 torchbringer-0.2.0/torchbringer.egg-info/top_level.txt
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.293095 torchbringer-0.2.1/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-27 00:48:39.000000 torchbringer-0.2.1/LICENSE
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 15:07:29.293095 torchbringer-0.2.1/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6547 2024-05-27 00:48:39.000000 torchbringer-0.2.1/README.md
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-27 15:07:29.293095 torchbringer-0.2.1/setup.cfg
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1155 2024-05-27 15:07:27.000000 torchbringer-0.2.1/setup.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.283095 torchbringer-0.2.1/torchbringer/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-27 15:07:22.000000 torchbringer-0.2.1/torchbringer/__init__.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.283095 torchbringer-0.2.1/torchbringer/components/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2851 2024-05-27 12:38:47.000000 torchbringer-0.2.1/torchbringer/components/builders.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      781 2024-05-27 02:31:46.000000 torchbringer-0.2.1/torchbringer/components/epsilon.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/components/replay_memory.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.283095 torchbringer-0.2.1/torchbringer/examples/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     4814 2024-05-27 15:06:32.000000 torchbringer-0.2.1/torchbringer/examples/breakout_local_dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/examples/cartpole_grpc_dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-27 14:59:27.000000 torchbringer-0.2.1/torchbringer/examples/cartpole_local_dqn.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.283095 torchbringer-0.2.1/torchbringer/learners/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5210 2024-05-27 13:04:44.000000 torchbringer-0.2.1/torchbringer/learners/dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/learners/learner_utils.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.283095 torchbringer-0.2.1/torchbringer/servers/
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.293095 torchbringer-0.2.1/torchbringer/servers/grpc/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_grpc_client.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_grpc_server.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_pb2.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_pb2.pyi
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      583 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/servers/torchbringer_agent.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.293095 torchbringer-0.2.1/torchbringer.egg-info/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 15:07:29.000000 torchbringer-0.2.1/torchbringer.egg-info/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      836 2024-05-27 15:07:29.000000 torchbringer-0.2.1/torchbringer.egg-info/SOURCES.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-27 15:07:29.000000 torchbringer-0.2.1/torchbringer.egg-info/dependency_links.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       98 2024-05-27 15:07:29.000000 torchbringer-0.2.1/torchbringer.egg-info/requires.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-27 15:07:29.000000 torchbringer-0.2.1/torchbringer.egg-info/top_level.txt
```

### Comparing `torchbringer-0.2.0/LICENSE` & `torchbringer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.0/PKG-INFO` & `torchbringer-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbringer
-Version: 0.2.0
+Version: 0.2.1
 Summary: A PyTorch library for deep reinforcement learning 
 Home-page: https://github.com/moraguma/TorchBringer
 Author: Moraguma
 Author-email: g170603@dac.unicamp.br
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchbringer-0.2.0/README.md` & `torchbringer-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.0/setup.py` & `torchbringer-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='torchbringer',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.2.0',    
+    version='0.2.1',    
     description='A PyTorch library for deep reinforcement learning ',
     url='https://github.com/moraguma/TorchBringer',
     author='Moraguma',
     author_email='g170603@dac.unicamp.br',
     license='MIT',
     packages=find_namespace_packages(),
     install_requires=[
```

### Comparing `torchbringer-0.2.0/torchbringer/components/builders.py` & `torchbringer-0.2.1/torchbringer/components/builders.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.0/torchbringer/components/epsilon.py` & `torchbringer-0.2.1/torchbringer/components/epsilon.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.0/torchbringer/components/replay_memory.py` & `torchbringer-0.2.1/torchbringer/components/replay_memory.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.0/torchbringer/examples/breakout_local_dqn.py` & `torchbringer-0.2.1/torchbringer/examples/breakout_local_dqn.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Based on Mnih, Volodymyr, et al. "Playing atari with deep reinforcement learning." arXiv preprint arXiv:1312.5602 (2013).
 
+import datetime
+import time
 import gymnasium as gym
 from itertools import count
 from aim import Run
 
 import torch
 import cv2
 import numpy as np
@@ -117,24 +119,26 @@
 
 dqn = TorchBringerAgent()
 dqn.initialize(config)
 run = Run(experiment="DQN Breakout")
 
 run["hparams"] = config
 
-steps_done = 0
-
+frames_done = 0
+log_interval = 10000
 if torch.cuda.is_available():
     print("Running on GPU!")
-    num_episodes = 600
+    total_frames = 10000000
 else:
     print("Running on CPU!")
-    num_episodes = 50
+    total_frames = 1000
 
-for i_episode in range(num_episodes):
+starting_time = time.time()
+last_log_time = time.time()
+for i_episode in count():
     # Initialize the environment and get its state
     state, info = env.reset()
     reward = torch.tensor([0.0], device=device)
     terminal = False
 
     cummulative_reward = 0.0
     
@@ -143,14 +147,23 @@
         observation, reward, terminated, truncated, _ = env.step(dqn.step(state, reward, terminal).item())
         cummulative_reward += reward
 
         state = None if terminated else torch.tensor(observation, dtype=torch.float32, device=device).unsqueeze(0) 
         reward = torch.tensor([reward], device=device)
         terminal = terminated or truncated
 
+        frames_done += 1
+        if frames_done % log_interval == 0:
+            current_time = time.time()
+            print("Finished %d/%d frames in %s - ETR: %ss; TE: %ss" % (frames_done, total_frames, datetime.timedelta(seconds=int(current_time - last_log_time)), datetime.timedelta(seconds=int((current_time - starting_time) / frames_done * total_frames)), datetime.timedelta(seconds=int(current_time - starting_time))))
+            last_log_time = current_time
+
         if terminal:
             run.track({"Episode reward": cummulative_reward}, step=i_episode)
 
             dqn.step(state, reward, terminal)
             break
 
-print('Complete')
+    if frames_done >= total_frames:
+        break
+
+print("Complete in %.2fs" % (time.time() - starting_time))
```

### Comparing `torchbringer-0.2.0/torchbringer/examples/cartpole_grpc_dqn.py` & `torchbringer-0.2.1/torchbringer/examples/cartpole_grpc_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.0/torchbringer/examples/cartpole_local_dqn.py` & `torchbringer-0.2.1/torchbringer/examples/cartpole_local_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.0/torchbringer/learners/dqn.py` & `torchbringer-0.2.1/torchbringer/learners/dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_grpc_client.py` & `torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_grpc_client.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_grpc_server.py` & `torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_grpc_server.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_pb2.py` & `torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_pb2.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_pb2.pyi` & `torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_pb2_grpc.py` & `torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.0/torchbringer/servers/torchbringer_agent.py` & `torchbringer-0.2.1/torchbringer/servers/torchbringer_agent.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.0/torchbringer.egg-info/PKG-INFO` & `torchbringer-0.2.1/torchbringer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbringer
-Version: 0.2.0
+Version: 0.2.1
 Summary: A PyTorch library for deep reinforcement learning 
 Home-page: https://github.com/moraguma/TorchBringer
 Author: Moraguma
 Author-email: g170603@dac.unicamp.br
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchbringer-0.2.0/torchbringer.egg-info/SOURCES.txt` & `torchbringer-0.2.1/torchbringer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

