# Comparing `tmp/torchbringer-0.2.2.tar.gz` & `tmp/torchbringer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbringer-0.2.2.tar", last modified: Mon May 27 18:37:16 2024, max compression
+gzip compressed data, was "torchbringer-0.2.3.tar", last modified: Mon May 27 18:48:08 2024, max compression
```

## Comparing `torchbringer-0.2.2.tar` & `torchbringer-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.883089 torchbringer-0.2.2/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-27 00:48:39.000000 torchbringer-0.2.2/LICENSE
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 18:37:16.883089 torchbringer-0.2.2/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6547 2024-05-27 00:48:39.000000 torchbringer-0.2.2/README.md
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-27 18:37:16.883089 torchbringer-0.2.2/setup.cfg
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1155 2024-05-27 18:37:03.000000 torchbringer-0.2.2/setup.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.873089 torchbringer-0.2.2/torchbringer/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-27 18:37:06.000000 torchbringer-0.2.2/torchbringer/__init__.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.873089 torchbringer-0.2.2/torchbringer/components/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2851 2024-05-27 12:38:47.000000 torchbringer-0.2.2/torchbringer/components/builders.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      781 2024-05-27 02:31:46.000000 torchbringer-0.2.2/torchbringer/components/epsilon.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/components/replay_memory.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.883089 torchbringer-0.2.2/torchbringer/examples/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     4856 2024-05-27 18:35:52.000000 torchbringer-0.2.2/torchbringer/examples/breakout_local_dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/examples/cartpole_grpc_dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-27 14:59:27.000000 torchbringer-0.2.2/torchbringer/examples/cartpole_local_dqn.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.883089 torchbringer-0.2.2/torchbringer/learners/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5210 2024-05-27 13:04:44.000000 torchbringer-0.2.2/torchbringer/learners/dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/learners/learner_utils.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.883089 torchbringer-0.2.2/torchbringer/servers/
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.883089 torchbringer-0.2.2/torchbringer/servers/grpc/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_grpc_client.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_grpc_server.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_pb2.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_pb2.pyi
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      583 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/servers/torchbringer_agent.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.883089 torchbringer-0.2.2/torchbringer.egg-info/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 18:37:16.000000 torchbringer-0.2.2/torchbringer.egg-info/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      836 2024-05-27 18:37:16.000000 torchbringer-0.2.2/torchbringer.egg-info/SOURCES.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-27 18:37:16.000000 torchbringer-0.2.2/torchbringer.egg-info/dependency_links.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       98 2024-05-27 18:37:16.000000 torchbringer-0.2.2/torchbringer.egg-info/requires.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-27 18:37:16.000000 torchbringer-0.2.2/torchbringer.egg-info/top_level.txt
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.103092 torchbringer-0.2.3/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-27 00:48:39.000000 torchbringer-0.2.3/LICENSE
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 18:48:08.103092 torchbringer-0.2.3/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6547 2024-05-27 00:48:39.000000 torchbringer-0.2.3/README.md
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-27 18:48:08.103092 torchbringer-0.2.3/setup.cfg
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1155 2024-05-27 18:47:59.000000 torchbringer-0.2.3/setup.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.093092 torchbringer-0.2.3/torchbringer/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-27 18:48:04.000000 torchbringer-0.2.3/torchbringer/__init__.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.093092 torchbringer-0.2.3/torchbringer/components/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2851 2024-05-27 12:38:47.000000 torchbringer-0.2.3/torchbringer/components/builders.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      781 2024-05-27 02:31:46.000000 torchbringer-0.2.3/torchbringer/components/epsilon.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/components/replay_memory.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.093092 torchbringer-0.2.3/torchbringer/examples/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5040 2024-05-27 18:46:40.000000 torchbringer-0.2.3/torchbringer/examples/breakout_local_dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/examples/cartpole_grpc_dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-27 14:59:27.000000 torchbringer-0.2.3/torchbringer/examples/cartpole_local_dqn.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.093092 torchbringer-0.2.3/torchbringer/learners/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5286 2024-05-27 18:40:02.000000 torchbringer-0.2.3/torchbringer/learners/dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/learners/learner_utils.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.093092 torchbringer-0.2.3/torchbringer/servers/
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.103092 torchbringer-0.2.3/torchbringer/servers/grpc/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_grpc_client.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_grpc_server.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_pb2.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_pb2.pyi
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-27 00:48:39.000000 torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      840 2024-05-27 18:44:28.000000 torchbringer-0.2.3/torchbringer/servers/torchbringer_agent.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:48:08.103092 torchbringer-0.2.3/torchbringer.egg-info/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 18:48:07.000000 torchbringer-0.2.3/torchbringer.egg-info/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      836 2024-05-27 18:48:08.000000 torchbringer-0.2.3/torchbringer.egg-info/SOURCES.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-27 18:48:07.000000 torchbringer-0.2.3/torchbringer.egg-info/dependency_links.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       98 2024-05-27 18:48:07.000000 torchbringer-0.2.3/torchbringer.egg-info/requires.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-27 18:48:07.000000 torchbringer-0.2.3/torchbringer.egg-info/top_level.txt
```

### Comparing `torchbringer-0.2.2/LICENSE` & `torchbringer-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.2/PKG-INFO` & `torchbringer-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbringer
-Version: 0.2.2
+Version: 0.2.3
 Summary: A PyTorch library for deep reinforcement learning 
 Home-page: https://github.com/moraguma/TorchBringer
 Author: Moraguma
 Author-email: g170603@dac.unicamp.br
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchbringer-0.2.2/README.md` & `torchbringer-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.2/setup.py` & `torchbringer-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='torchbringer',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.2.2',    
+    version='0.2.3',    
     description='A PyTorch library for deep reinforcement learning ',
     url='https://github.com/moraguma/TorchBringer',
     author='Moraguma',
     author_email='g170603@dac.unicamp.br',
     license='MIT',
     packages=find_namespace_packages(),
     install_requires=[
```

### Comparing `torchbringer-0.2.2/torchbringer/components/builders.py` & `torchbringer-0.2.3/torchbringer/components/builders.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.2/torchbringer/components/epsilon.py` & `torchbringer-0.2.3/torchbringer/components/epsilon.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.2/torchbringer/components/replay_memory.py` & `torchbringer-0.2.3/torchbringer/components/replay_memory.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.2/torchbringer/examples/breakout_local_dqn.py` & `torchbringer-0.2.3/torchbringer/examples/breakout_local_dqn.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     "tau": 0.005,
     "epsilon": {
         "type": "lin_decrease",
         "start": 1.0,
         "end": 0.1,
         "steps_to_end": 1000000
     },
-    "batch_size": 32,
+    "batch_size": 2,
     "grad_clip_value": 100,
     "loss": "smooth_l1_loss",
     "optimizer": {
         "type": "adamw",
         "lr": 1e-4, 
         "amsgrad": True
     },
@@ -137,32 +137,35 @@
 for i_episode in count():
     # Initialize the environment and get its state
     state, info = env.reset()
     reward = torch.tensor([0.0], device=device)
     terminal = False
 
     cummulative_reward = 0.0
+    cummulative_loss = 0.0
+    first_episode_frame = frames_done
     
     state = torch.tensor(state, dtype=torch.float32, device=device).unsqueeze(0)
     for t in count():
         observation, reward, terminated, truncated, _ = env.step(dqn.step(state, reward, terminal).item())
         cummulative_reward += reward
+        cummulative_loss += dqn.get_past_loss()
 
         state = None if terminated else torch.tensor(observation, dtype=torch.float32, device=device).unsqueeze(0) 
         reward = torch.tensor([reward], device=device)
         terminal = terminated or truncated
 
         frames_done += 1
         if frames_done % log_interval == 0:
             current_time = time.time()
             print("Finished %d/%d frames in %s - ETR: %ss; TE: %ss" % (frames_done, total_frames, datetime.timedelta(seconds=int(current_time - last_log_time)), datetime.timedelta(seconds=int((current_time - starting_time) / frames_done * (total_frames - frames_done))), datetime.timedelta(seconds=int(current_time - starting_time))))
             last_log_time = current_time
 
         if terminal:
-            run.track({"Episode reward": cummulative_reward}, step=i_episode)
+            run.track({"Episode reward": cummulative_reward, "Average loss": cummulative_loss / (frames_done - first_episode_frame)}, step=i_episode)
 
             dqn.step(state, reward, terminal)
             break
 
     if frames_done >= total_frames:
         break
```

### Comparing `torchbringer-0.2.2/torchbringer/examples/cartpole_grpc_dqn.py` & `torchbringer-0.2.3/torchbringer/examples/cartpole_grpc_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.2/torchbringer/examples/cartpole_local_dqn.py` & `torchbringer-0.2.3/torchbringer/examples/cartpole_local_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.2/torchbringer/learners/dqn.py` & `torchbringer-0.2.3/torchbringer/learners/dqn.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         self.optimizer = builders.build_optimizer(self.policy_net, config["optimizer"])
 
         self.past_state = None
         self.past_action = None
 
         self.steps_done = 0
 
+        self.past_loss = 0.0
+
 
     def experience(self, state, reward, terminal):
         if not self.past_state is None:
             self.memory.push(self.past_state, self.past_action, state, reward)
         
         if terminal:
             self.past_state = None
@@ -89,14 +91,15 @@
             if not non_final_next_states is None:
                 with torch.no_grad():
                     next_state_values[non_final_mask] = self.target_net(non_final_next_states).max(1).values
             expected_state_action_values = (next_state_values * self.gamma) + reward_batch
 
             # Compute loss
             step_loss = self.loss(state_action_values, expected_state_action_values.unsqueeze(1))
+            self.past_loss = step_loss.item()
 
             # Optimize the model
             self.optimizer.zero_grad()
             step_loss.backward()
 
             if not self.grad_clip_value is None:
                 torch.nn.utils.clip_grad_value_(self.policy_net.parameters(), self.grad_clip_value)
```

### Comparing `torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_grpc_client.py` & `torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_grpc_client.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_grpc_server.py` & `torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_grpc_server.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_pb2.py` & `torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_pb2.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_pb2.pyi` & `torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_pb2_grpc.py` & `torchbringer-0.2.3/torchbringer/servers/grpc/torchbringer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.2/torchbringer/servers/torchbringer_agent.py` & `torchbringer-0.2.3/torchbringer/servers/torchbringer_agent.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,8 +12,14 @@
     def initialize(self, config):
         self.learner = builders.build_learner(config)
     
 
     def step(self, state, reward, terminal):
         self.learner.experience(state, reward, terminal)
         self.learner.optimize()
-        return torch.tensor([], device=device) if state is None else self.learner.select_action(state)
+        return torch.tensor([], device=device) if state is None else self.learner.select_action(state)
+    
+    # TODO: This should be returned by the step function to avoid multiple calls when dealing with remote learning
+    def get_past_loss(self):
+        if hasattr(self.learner, "past_loss"):
+            return self.learner.past_loss
+        return 0.0
```

### Comparing `torchbringer-0.2.2/torchbringer.egg-info/PKG-INFO` & `torchbringer-0.2.3/torchbringer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbringer
-Version: 0.2.2
+Version: 0.2.3
 Summary: A PyTorch library for deep reinforcement learning 
 Home-page: https://github.com/moraguma/TorchBringer
 Author: Moraguma
 Author-email: g170603@dac.unicamp.br
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchbringer-0.2.2/torchbringer.egg-info/SOURCES.txt` & `torchbringer-0.2.3/torchbringer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

