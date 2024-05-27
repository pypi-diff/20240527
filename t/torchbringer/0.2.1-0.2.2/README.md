# Comparing `tmp/torchbringer-0.2.1.tar.gz` & `tmp/torchbringer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbringer-0.2.1.tar", last modified: Mon May 27 15:07:29 2024, max compression
+gzip compressed data, was "torchbringer-0.2.2.tar", last modified: Mon May 27 18:37:16 2024, max compression
```

## Comparing `torchbringer-0.2.1.tar` & `torchbringer-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.293095 torchbringer-0.2.1/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-27 00:48:39.000000 torchbringer-0.2.1/LICENSE
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 15:07:29.293095 torchbringer-0.2.1/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6547 2024-05-27 00:48:39.000000 torchbringer-0.2.1/README.md
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-27 15:07:29.293095 torchbringer-0.2.1/setup.cfg
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1155 2024-05-27 15:07:27.000000 torchbringer-0.2.1/setup.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.283095 torchbringer-0.2.1/torchbringer/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-27 15:07:22.000000 torchbringer-0.2.1/torchbringer/__init__.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.283095 torchbringer-0.2.1/torchbringer/components/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2851 2024-05-27 12:38:47.000000 torchbringer-0.2.1/torchbringer/components/builders.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      781 2024-05-27 02:31:46.000000 torchbringer-0.2.1/torchbringer/components/epsilon.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/components/replay_memory.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.283095 torchbringer-0.2.1/torchbringer/examples/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     4814 2024-05-27 15:06:32.000000 torchbringer-0.2.1/torchbringer/examples/breakout_local_dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/examples/cartpole_grpc_dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-27 14:59:27.000000 torchbringer-0.2.1/torchbringer/examples/cartpole_local_dqn.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.283095 torchbringer-0.2.1/torchbringer/learners/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5210 2024-05-27 13:04:44.000000 torchbringer-0.2.1/torchbringer/learners/dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/learners/learner_utils.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.283095 torchbringer-0.2.1/torchbringer/servers/
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.293095 torchbringer-0.2.1/torchbringer/servers/grpc/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_grpc_client.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_grpc_server.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_pb2.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_pb2.pyi
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      583 2024-05-27 00:48:39.000000 torchbringer-0.2.1/torchbringer/servers/torchbringer_agent.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 15:07:29.293095 torchbringer-0.2.1/torchbringer.egg-info/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 15:07:29.000000 torchbringer-0.2.1/torchbringer.egg-info/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      836 2024-05-27 15:07:29.000000 torchbringer-0.2.1/torchbringer.egg-info/SOURCES.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-27 15:07:29.000000 torchbringer-0.2.1/torchbringer.egg-info/dependency_links.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       98 2024-05-27 15:07:29.000000 torchbringer-0.2.1/torchbringer.egg-info/requires.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-27 15:07:29.000000 torchbringer-0.2.1/torchbringer.egg-info/top_level.txt
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.883089 torchbringer-0.2.2/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-27 00:48:39.000000 torchbringer-0.2.2/LICENSE
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 18:37:16.883089 torchbringer-0.2.2/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6547 2024-05-27 00:48:39.000000 torchbringer-0.2.2/README.md
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-27 18:37:16.883089 torchbringer-0.2.2/setup.cfg
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1155 2024-05-27 18:37:03.000000 torchbringer-0.2.2/setup.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.873089 torchbringer-0.2.2/torchbringer/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-27 18:37:06.000000 torchbringer-0.2.2/torchbringer/__init__.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.873089 torchbringer-0.2.2/torchbringer/components/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2851 2024-05-27 12:38:47.000000 torchbringer-0.2.2/torchbringer/components/builders.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      781 2024-05-27 02:31:46.000000 torchbringer-0.2.2/torchbringer/components/epsilon.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/components/replay_memory.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.883089 torchbringer-0.2.2/torchbringer/examples/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     4856 2024-05-27 18:35:52.000000 torchbringer-0.2.2/torchbringer/examples/breakout_local_dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/examples/cartpole_grpc_dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-27 14:59:27.000000 torchbringer-0.2.2/torchbringer/examples/cartpole_local_dqn.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.883089 torchbringer-0.2.2/torchbringer/learners/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5210 2024-05-27 13:04:44.000000 torchbringer-0.2.2/torchbringer/learners/dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/learners/learner_utils.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.883089 torchbringer-0.2.2/torchbringer/servers/
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.883089 torchbringer-0.2.2/torchbringer/servers/grpc/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_grpc_client.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_grpc_server.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_pb2.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_pb2.pyi
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      583 2024-05-27 00:48:39.000000 torchbringer-0.2.2/torchbringer/servers/torchbringer_agent.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-27 18:37:16.883089 torchbringer-0.2.2/torchbringer.egg-info/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7345 2024-05-27 18:37:16.000000 torchbringer-0.2.2/torchbringer.egg-info/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      836 2024-05-27 18:37:16.000000 torchbringer-0.2.2/torchbringer.egg-info/SOURCES.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-27 18:37:16.000000 torchbringer-0.2.2/torchbringer.egg-info/dependency_links.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       98 2024-05-27 18:37:16.000000 torchbringer-0.2.2/torchbringer.egg-info/requires.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-27 18:37:16.000000 torchbringer-0.2.2/torchbringer.egg-info/top_level.txt
```

### Comparing `torchbringer-0.2.1/LICENSE` & `torchbringer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.1/PKG-INFO` & `torchbringer-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbringer
-Version: 0.2.1
+Version: 0.2.2
 Summary: A PyTorch library for deep reinforcement learning 
 Home-page: https://github.com/moraguma/TorchBringer
 Author: Moraguma
 Author-email: g170603@dac.unicamp.br
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchbringer-0.2.1/README.md` & `torchbringer-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.1/setup.py` & `torchbringer-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='torchbringer',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.2.1',    
+    version='0.2.2',    
     description='A PyTorch library for deep reinforcement learning ',
     url='https://github.com/moraguma/TorchBringer',
     author='Moraguma',
     author_email='g170603@dac.unicamp.br',
     license='MIT',
     packages=find_namespace_packages(),
     install_requires=[
```

### Comparing `torchbringer-0.2.1/torchbringer/components/builders.py` & `torchbringer-0.2.2/torchbringer/components/builders.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.1/torchbringer/components/epsilon.py` & `torchbringer-0.2.2/torchbringer/components/epsilon.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.1/torchbringer/components/replay_memory.py` & `torchbringer-0.2.2/torchbringer/components/replay_memory.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.1/torchbringer/examples/breakout_local_dqn.py` & `torchbringer-0.2.2/torchbringer/examples/breakout_local_dqn.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
         self.past_frames = []
         self.stacked_frames = stacked_frames
         self.frames_clipped = frames_clipped
     
 
     def preprocess_state(self, state):
-        return cv2.resize(cv2.cvtColor(state, cv2.COLOR_RGB2GRAY), (110, 84))[:, 13:97]
+        return cv2.resize(cv2.cvtColor(state, cv2.COLOR_RGB2GRAY), (110, 84))[:, 13:97] / 255.0
 
 
     def get_current_state(self):
         return np.array(self.past_frames)
 
 
     def step(self, action):
@@ -47,15 +47,15 @@
         self.past_frames[self.stacked_frames-1, :, :] = self.preprocess_state(observation)
 
         return self.get_current_state(), total_reward, terminated, truncated, info
 
 
     def reset(self):
         state, info = self.env.reset()
-        self.past_frames = np.zeros((self.stacked_frames, 84, 84))
+        self.past_frames = np.zeros((self.stacked_frames, 84, 84), dtype=np.float16)
         self.past_frames[:, :, :] = self.preprocess_state(state)
 
         return self.get_current_state(), info
 
 # if GPU is to be used
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
@@ -150,15 +150,15 @@
         state = None if terminated else torch.tensor(observation, dtype=torch.float32, device=device).unsqueeze(0) 
         reward = torch.tensor([reward], device=device)
         terminal = terminated or truncated
 
         frames_done += 1
         if frames_done % log_interval == 0:
             current_time = time.time()
-            print("Finished %d/%d frames in %s - ETR: %ss; TE: %ss" % (frames_done, total_frames, datetime.timedelta(seconds=int(current_time - last_log_time)), datetime.timedelta(seconds=int((current_time - starting_time) / frames_done * total_frames)), datetime.timedelta(seconds=int(current_time - starting_time))))
+            print("Finished %d/%d frames in %s - ETR: %ss; TE: %ss" % (frames_done, total_frames, datetime.timedelta(seconds=int(current_time - last_log_time)), datetime.timedelta(seconds=int((current_time - starting_time) / frames_done * (total_frames - frames_done))), datetime.timedelta(seconds=int(current_time - starting_time))))
             last_log_time = current_time
 
         if terminal:
             run.track({"Episode reward": cummulative_reward}, step=i_episode)
 
             dqn.step(state, reward, terminal)
             break
```

### Comparing `torchbringer-0.2.1/torchbringer/examples/cartpole_grpc_dqn.py` & `torchbringer-0.2.2/torchbringer/examples/cartpole_grpc_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.1/torchbringer/examples/cartpole_local_dqn.py` & `torchbringer-0.2.2/torchbringer/examples/cartpole_local_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.1/torchbringer/learners/dqn.py` & `torchbringer-0.2.2/torchbringer/learners/dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_grpc_client.py` & `torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_grpc_client.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_grpc_server.py` & `torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_grpc_server.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_pb2.py` & `torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_pb2.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_pb2.pyi` & `torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.1/torchbringer/servers/grpc/torchbringer_pb2_grpc.py` & `torchbringer-0.2.2/torchbringer/servers/grpc/torchbringer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.1/torchbringer/servers/torchbringer_agent.py` & `torchbringer-0.2.2/torchbringer/servers/torchbringer_agent.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.2.1/torchbringer.egg-info/PKG-INFO` & `torchbringer-0.2.2/torchbringer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbringer
-Version: 0.2.1
+Version: 0.2.2
 Summary: A PyTorch library for deep reinforcement learning 
 Home-page: https://github.com/moraguma/TorchBringer
 Author: Moraguma
 Author-email: g170603@dac.unicamp.br
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchbringer-0.2.1/torchbringer.egg-info/SOURCES.txt` & `torchbringer-0.2.2/torchbringer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

