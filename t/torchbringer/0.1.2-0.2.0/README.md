# Comparing `tmp/torchbringer-0.1.2.tar.gz` & `tmp/torchbringer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbringer-0.1.2.tar", last modified: Sun May 26 16:34:07 2024, max compression
+gzip compressed data, was "torchbringer-0.2.0.tar", last modified: Mon May 27 13:10:27 2024, max compression
```

## Comparing `torchbringer-0.1.2.tar` & `torchbringer-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.506785 torchbringer-0.1.2/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-25 23:44:21.000000 torchbringer-0.1.2/LICENSE
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7296 2024-05-26 16:34:07.506785 torchbringer-0.1.2/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6527 2024-05-26 16:33:08.000000 torchbringer-0.1.2/README.md
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-26 16:34:07.506785 torchbringer-0.1.2/setup.cfg
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1130 2024-05-26 16:34:01.000000 torchbringer-0.1.2/setup.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.496785 torchbringer-0.1.2/torchbringer/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-26 16:34:01.000000 torchbringer-0.1.2/torchbringer/__init__.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.496785 torchbringer-0.1.2/torchbringer/components/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2757 2024-05-26 15:48:03.000000 torchbringer-0.1.2/torchbringer/components/builders.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      610 2024-05-25 16:10:22.000000 torchbringer-0.1.2/torchbringer/components/epsilon.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-25 17:27:12.000000 torchbringer-0.1.2/torchbringer/components/replay_memory.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.496785 torchbringer-0.1.2/torchbringer/examples/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-26 15:39:23.000000 torchbringer-0.1.2/torchbringer/examples/cartpole_grpc_dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-26 15:39:22.000000 torchbringer-0.1.2/torchbringer/examples/cartpole_local_dqn.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.496785 torchbringer-0.1.2/torchbringer/learners/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     4941 2024-05-26 15:47:32.000000 torchbringer-0.1.2/torchbringer/learners/dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-25 15:17:44.000000 torchbringer-0.1.2/torchbringer/learners/learner_utils.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.496785 torchbringer-0.1.2/torchbringer/servers/
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.506785 torchbringer-0.1.2/torchbringer/servers/grpc/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-26 15:38:36.000000 torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_grpc_client.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-26 15:41:48.000000 torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_grpc_server.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-26 15:50:10.000000 torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_pb2.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-26 15:50:10.000000 torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_pb2.pyi
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-26 15:52:44.000000 torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      583 2024-05-26 15:38:36.000000 torchbringer-0.1.2/torchbringer/servers/torchbringer_agent.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:34:07.506785 torchbringer-0.1.2/torchbringer.egg-info/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7296 2024-05-26 16:34:07.000000 torchbringer-0.1.2/torchbringer.egg-info/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      792 2024-05-26 16:34:07.000000 torchbringer-0.1.2/torchbringer.egg-info/SOURCES.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-26 16:34:07.000000 torchbringer-0.1.2/torchbringer.egg-info/dependency_links.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       84 2024-05-26 16:34:07.000000 torchbringer-0.1.2/torchbringer.egg-info/requires.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-26 16:34:07.000000 torchbringer-0.1.2/torchbringer.egg-info/top_level.txt
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.573182 torchbringer-0.2.0/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-27 00:48:39.000000 torchbringer-0.2.0/LICENSE
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 13:10:27.573182 torchbringer-0.2.0/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6547 2024-05-27 00:48:39.000000 torchbringer-0.2.0/README.md
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-27 13:10:27.573182 torchbringer-0.2.0/setup.cfg
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1155 2024-05-27 13:07:40.000000 torchbringer-0.2.0/setup.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.553182 torchbringer-0.2.0/torchbringer/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-27 13:07:32.000000 torchbringer-0.2.0/torchbringer/__init__.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.553182 torchbringer-0.2.0/torchbringer/components/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2851 2024-05-27 12:38:47.000000 torchbringer-0.2.0/torchbringer/components/builders.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      781 2024-05-27 02:31:46.000000 torchbringer-0.2.0/torchbringer/components/epsilon.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/components/replay_memory.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.563182 torchbringer-0.2.0/torchbringer/examples/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     4153 2024-05-27 13:06:27.000000 torchbringer-0.2.0/torchbringer/examples/breakout_local_dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/examples/cartpole_grpc_dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/examples/cartpole_local_dqn.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.563182 torchbringer-0.2.0/torchbringer/learners/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5210 2024-05-27 13:04:44.000000 torchbringer-0.2.0/torchbringer/learners/dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/learners/learner_utils.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.563182 torchbringer-0.2.0/torchbringer/servers/
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.573182 torchbringer-0.2.0/torchbringer/servers/grpc/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_grpc_client.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_grpc_server.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_pb2.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_pb2.pyi
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      583 2024-05-27 00:48:39.000000 torchbringer-0.2.0/torchbringer/servers/torchbringer_agent.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 13:10:27.573182 torchbringer-0.2.0/torchbringer.egg-info/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 13:10:27.000000 torchbringer-0.2.0/torchbringer.egg-info/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      836 2024-05-27 13:10:27.000000 torchbringer-0.2.0/torchbringer.egg-info/SOURCES.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-27 13:10:27.000000 torchbringer-0.2.0/torchbringer.egg-info/dependency_links.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       98 2024-05-27 13:10:27.000000 torchbringer-0.2.0/torchbringer.egg-info/requires.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-27 13:10:27.000000 torchbringer-0.2.0/torchbringer.egg-info/top_level.txt
```

### Comparing `torchbringer-0.1.2/LICENSE` & `torchbringer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.2/PKG-INFO` & `torchbringer-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbringer
-Version: 0.1.2
+Version: 0.2.0
 Summary: A PyTorch library for deep reinforcement learning 
 Home-page: https://github.com/moraguma/TorchBringer
 Author: Moraguma
 Author-email: g170603@dac.unicamp.br
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -15,14 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=70.0.0
 Requires-Dist: torch==2.3.0
 Requires-Dist: gymnasium==0.29.1
 Requires-Dist: aim==3.19.3
 Requires-Dist: numpy
+Requires-Dist: opencv-python
 Requires-Dist: protobuf
 Requires-Dist: grpcio
 
 TorchBringer is an open-source framework that provides a simple interface for operating with pre-implemented deep reinforcement learning algorithms built on top of PyTorch. The interfaces provided can be used to operate deep RL agents either locally or remotely via gRPC. Currently, TorchBringer supports the following algorithms
 
 - [x] DQN
 
@@ -40,28 +41,29 @@
 
 ```python
 import gymnasium as gym
 from itertools import count
 import torch
 from torchbringer.servers.torchbringer_agent import TorchBringerAgent
 
+device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
 env = gym.make("CartPole-v1")
 state, info = env.reset()
 
 config = {
     # Check the reference section to understand config formatting
 }
 
 dqn = TorchBringerAgent()
 dqn.initialize(config)
 steps_done = 0
 
 num_episodes = 600
 for i_episode in range(num_episodes):
-    # Initialize the environment and get its state
     state, info = env.reset()
     reward = torch.tensor([0.0], device=device)
     terminal = False
     
     state = torch.tensor(state, dtype=torch.float32, device=device).unsqueeze(0)
     for t in count():
         observation, reward, terminated, truncated, _ = env.step(dqn.step(state, reward, terminal).item())
```

### Comparing `torchbringer-0.1.2/README.md` & `torchbringer-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,28 +16,29 @@
 
 ```python
 import gymnasium as gym
 from itertools import count
 import torch
 from torchbringer.servers.torchbringer_agent import TorchBringerAgent
 
+device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
 env = gym.make("CartPole-v1")
 state, info = env.reset()
 
 config = {
     # Check the reference section to understand config formatting
 }
 
 dqn = TorchBringerAgent()
 dqn.initialize(config)
 steps_done = 0
 
 num_episodes = 600
 for i_episode in range(num_episodes):
-    # Initialize the environment and get its state
     state, info = env.reset()
     reward = torch.tensor([0.0], device=device)
     terminal = False
     
     state = torch.tensor(state, dtype=torch.float32, device=device).unsqueeze(0)
     for t in count():
         observation, reward, terminated, truncated, _ = env.step(dqn.step(state, reward, terminal).item())
```

### Comparing `torchbringer-0.1.2/setup.py` & `torchbringer-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='torchbringer',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.1.2',    
+    version='0.2.0',    
     description='A PyTorch library for deep reinforcement learning ',
     url='https://github.com/moraguma/TorchBringer',
     author='Moraguma',
     author_email='g170603@dac.unicamp.br',
     license='MIT',
     packages=find_namespace_packages(),
     install_requires=[
         'setuptools>=70.0.0',
         'torch==2.3.0',
         'gymnasium==0.29.1',
         'aim==3.19.3',
         'numpy',
+        'opencv-python',
         'protobuf',
         'grpcio'                    
     ],
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
```

### Comparing `torchbringer-0.1.2/torchbringer/components/builders.py` & `torchbringer-0.2.0/torchbringer/components/builders.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 LEARNER_STRING_TO_CLASS = {
     "dqn": DQN
 }
 SPACE_STRING_TO_CLASS = {
     "discrete": gym.spaces.Discrete
 }
 EPSILON_STRING_TO_FUNC = {
-    "exp_decrease": epsilon.exp_decrease
+    "exp_decrease": epsilon.exp_decrease,
+    "lin_decrease": epsilon.lin_decrease
 }
 LAYER_STRING_TO_CLASS = {
     "linear": nn.Linear,
-    "relu": nn.ReLU
+    "relu": nn.ReLU,
+    "conv2d": nn.Conv2d,
+    "flatten": nn.Flatten
 }
 LOSS_STRING_TO_FUNC = {
     "smooth_l1_loss": nn.SmoothL1Loss()
 }
 OPTIMIZER_STRING_TO_CLASS = {
     "adamw": optim.AdamW
 }
```

### Comparing `torchbringer-0.1.2/torchbringer/components/epsilon.py` & `torchbringer-0.2.0/torchbringer/components/epsilon.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,8 +15,13 @@
 
 """
 Functions in this file return the epsilon threshold at a specific step. They should be called as 
 f(steps_done, *args)
 """
 
 def exp_decrease(steps_done, start, end, steps_to_end):
-    return end + (start - end) * math.exp(-1. * steps_done / steps_to_end)
+    return end + (start - end) * math.exp(-1. * steps_done / steps_to_end)
+
+
+def lin_decrease(steps_done, start, end, steps_to_end):
+    progress = (steps_done / steps_to_end)
+    return end + (start - end) * (progress if progress <= 1 else 1.0)
```

### Comparing `torchbringer-0.1.2/torchbringer/components/replay_memory.py` & `torchbringer-0.2.0/torchbringer/components/replay_memory.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.2/torchbringer/examples/cartpole_grpc_dqn.py` & `torchbringer-0.2.0/torchbringer/examples/cartpole_grpc_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.2/torchbringer/examples/cartpole_local_dqn.py` & `torchbringer-0.2.0/torchbringer/examples/cartpole_local_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.2/torchbringer/learners/dqn.py` & `torchbringer-0.2.0/torchbringer/learners/dqn.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,26 +67,32 @@
             # Transpose batch
             transitions = self.memory.sample(self.batch_size)
             batch = Transition(*zip(*transitions))
 
             # Mask used to consider only non-terminal states
             non_final_mask = torch.tensor(tuple(map(lambda s: s is not None,
                                                 batch.next_state)), device=device, dtype=torch.bool)
-            non_final_next_states = torch.cat([s for s in batch.next_state if s is not None])
+            
+            non_final_next_states = [s for s in batch.next_state if s is not None]
+            if len(non_final_next_states) == 0:
+                non_final_next_states = None
+            else:
+                non_final_next_states = torch.cat([s for s in batch.next_state if s is not None])
             state_batch = torch.cat(batch.state)
             action_batch = torch.cat(batch.action)
             reward_batch = torch.cat(batch.reward)
 
             # Compute Q(s_t, a) for state action pairs in batch
             state_action_values = self.policy_net(state_batch).gather(1, action_batch)
 
             # Compute the expected Q values (r +  γ max_a ​Q(s′,a))
             next_state_values = torch.zeros(self.batch_size, device=device)
-            with torch.no_grad():
-                next_state_values[non_final_mask] = self.target_net(non_final_next_states).max(1).values
+            if not non_final_next_states is None:
+                with torch.no_grad():
+                    next_state_values[non_final_mask] = self.target_net(non_final_next_states).max(1).values
             expected_state_action_values = (next_state_values * self.gamma) + reward_batch
 
             # Compute loss
             step_loss = self.loss(state_action_values, expected_state_action_values.unsqueeze(1))
 
             # Optimize the model
             self.optimizer.zero_grad()
```

### Comparing `torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_grpc_client.py` & `torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_grpc_client.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_grpc_server.py` & `torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_grpc_server.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_pb2.py` & `torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_pb2.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_pb2.pyi` & `torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.2/torchbringer/servers/grpc/torchbringer_pb2_grpc.py` & `torchbringer-0.2.0/torchbringer/servers/grpc/torchbringer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.2/torchbringer/servers/torchbringer_agent.py` & `torchbringer-0.2.0/torchbringer/servers/torchbringer_agent.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.2/torchbringer.egg-info/PKG-INFO` & `torchbringer-0.2.0/torchbringer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbringer
-Version: 0.1.2
+Version: 0.2.0
 Summary: A PyTorch library for deep reinforcement learning 
 Home-page: https://github.com/moraguma/TorchBringer
 Author: Moraguma
 Author-email: g170603@dac.unicamp.br
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -15,14 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=70.0.0
 Requires-Dist: torch==2.3.0
 Requires-Dist: gymnasium==0.29.1
 Requires-Dist: aim==3.19.3
 Requires-Dist: numpy
+Requires-Dist: opencv-python
 Requires-Dist: protobuf
 Requires-Dist: grpcio
 
 TorchBringer is an open-source framework that provides a simple interface for operating with pre-implemented deep reinforcement learning algorithms built on top of PyTorch. The interfaces provided can be used to operate deep RL agents either locally or remotely via gRPC. Currently, TorchBringer supports the following algorithms
 
 - [x] DQN
 
@@ -40,28 +41,29 @@
 
 ```python
 import gymnasium as gym
 from itertools import count
 import torch
 from torchbringer.servers.torchbringer_agent import TorchBringerAgent
 
+device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
 env = gym.make("CartPole-v1")
 state, info = env.reset()
 
 config = {
     # Check the reference section to understand config formatting
 }
 
 dqn = TorchBringerAgent()
 dqn.initialize(config)
 steps_done = 0
 
 num_episodes = 600
 for i_episode in range(num_episodes):
-    # Initialize the environment and get its state
     state, info = env.reset()
     reward = torch.tensor([0.0], device=device)
     terminal = False
     
     state = torch.tensor(state, dtype=torch.float32, device=device).unsqueeze(0)
     for t in count():
         observation, reward, terminated, truncated, _ = env.step(dqn.step(state, reward, terminal).item())
```

### Comparing `torchbringer-0.1.2/torchbringer.egg-info/SOURCES.txt` & `torchbringer-0.2.0/torchbringer.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 torchbringer.egg-info/SOURCES.txt
 torchbringer.egg-info/dependency_links.txt
 torchbringer.egg-info/requires.txt
 torchbringer.egg-info/top_level.txt
 torchbringer/components/builders.py
 torchbringer/components/epsilon.py
 torchbringer/components/replay_memory.py
+torchbringer/examples/breakout_local_dqn.py
 torchbringer/examples/cartpole_grpc_dqn.py
 torchbringer/examples/cartpole_local_dqn.py
 torchbringer/learners/dqn.py
 torchbringer/learners/learner_utils.py
 torchbringer/servers/torchbringer_agent.py
 torchbringer/servers/grpc/torchbringer_grpc_client.py
 torchbringer/servers/grpc/torchbringer_grpc_server.py
```

