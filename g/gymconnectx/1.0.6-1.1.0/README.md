# Comparing `tmp/gymconnectx-1.0.6.tar.gz` & `tmp/gymconnectx-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymconnectx-1.0.6.tar", last modified: Sun May 19 08:35:05 2024, max compression
+gzip compressed data, was "gymconnectx-1.1.0.tar", last modified: Mon May 27 19:28:52 2024, max compression
```

## Comparing `gymconnectx-1.0.6.tar` & `gymconnectx-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:35:05.874998 gymconnectx-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-19 08:35:01.000000 gymconnectx-1.0.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-19 08:35:05.874998 gymconnectx-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-19 08:35:01.000000 gymconnectx-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:35:05.870998 gymconnectx-1.0.6/gymconnectx/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-19 08:35:01.000000 gymconnectx-1.0.6/gymconnectx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:35:05.874998 gymconnectx-1.0.6/gymconnectx/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-19 08:35:01.000000 gymconnectx-1.0.6/gymconnectx/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26371 2024-05-19 08:35:01.000000 gymconnectx-1.0.6/gymconnectx/envs/gymconnectxenv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:35:05.874998 gymconnectx-1.0.6/gymconnectx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-19 08:35:05.000000 gymconnectx-1.0.6/gymconnectx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-19 08:35:05.000000 gymconnectx-1.0.6/gymconnectx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 08:35:05.000000 gymconnectx-1.0.6/gymconnectx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 08:35:05.000000 gymconnectx-1.0.6/gymconnectx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 08:35:05.000000 gymconnectx-1.0.6/gymconnectx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 08:35:01.000000 gymconnectx-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 08:35:05.874998 gymconnectx-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-19 08:35:01.000000 gymconnectx-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:28:52.888334 gymconnectx-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-27 19:28:48.000000 gymconnectx-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-27 19:28:52.888334 gymconnectx-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-27 19:28:48.000000 gymconnectx-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:28:52.888334 gymconnectx-1.1.0/gymconnectx/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-27 19:28:48.000000 gymconnectx-1.1.0/gymconnectx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:28:52.888334 gymconnectx-1.1.0/gymconnectx/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:28:48.000000 gymconnectx-1.1.0/gymconnectx/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   149356 2024-05-27 19:28:48.000000 gymconnectx-1.1.0/gymconnectx/assets/imgBase64.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:28:52.888334 gymconnectx-1.1.0/gymconnectx/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 19:28:48.000000 gymconnectx-1.1.0/gymconnectx/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26564 2024-05-27 19:28:48.000000 gymconnectx-1.1.0/gymconnectx/envs/gymconnectxenv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:28:52.888334 gymconnectx-1.1.0/gymconnectx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-27 19:28:52.000000 gymconnectx-1.1.0/gymconnectx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-27 19:28:52.000000 gymconnectx-1.1.0/gymconnectx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:28:52.000000 gymconnectx-1.1.0/gymconnectx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 19:28:52.000000 gymconnectx-1.1.0/gymconnectx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 19:28:52.000000 gymconnectx-1.1.0/gymconnectx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-27 19:28:48.000000 gymconnectx-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:28:52.892334 gymconnectx-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-27 19:28:48.000000 gymconnectx-1.1.0/setup.py
```

### Comparing `gymconnectx-1.0.6/LICENSE.md` & `gymconnectx-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gymconnectx-1.0.6/PKG-INFO` & `gymconnectx-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gymconnectx
-Version: 1.0.6
+Version: 1.1.0
 Summary: An OpenAI Gym Environment Connect X Game with GUI. ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N.
 Home-page: https://github.com/fauzisho/GymConnectX
 Author: Fauzi Sholichin
 License: MIT License
         
         Copyright (c) 2024 Fauzi Sholichin
```

### Comparing `gymconnectx-1.0.6/README.md` & `gymconnectx-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gymconnectx-1.0.6/gymconnectx/__init__.py` & `gymconnectx-1.1.0/gymconnectx/__init__.py`

 * *Files identical despite different names*

### Comparing `gymconnectx-1.0.6/gymconnectx/envs/gymconnectxenv.py` & `gymconnectx-1.1.0/gymconnectx/envs/gymconnectxenv.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,39 +251,42 @@
 
         """
         pygame.quit()
         sys.exit()
 
 
 class ConnectGameEnv(gym.Env):
-    def __init__(self, connect=4, width=7, height=7, reward_winner=1, reward_loser=-1, living_reward=0, max_steps=100,
-                 delay=100, square_size=100, avatar_player_1=None, avatar_player_2=None):
+    def __init__(self, connect=4, width=7, height=7, reward_winner=1, reward_loser=-1, living_reward=0, reward_draw=0.5,
+                 max_steps=100, delay=100, square_size=100, avatar_player_1=None, avatar_player_2=None):
         """
         Initializes a new ConnectGameEnv, which is a gaming environment for playing games like Connect Four.
 
         :param connect: Number of consecutive tokens required to win (default is 4).
         :param width: Width of the game board (number of columns, default is 7).
         :param height: Height of the game board (number of rows, default is 7).
         :param reward_winner: Reward given to the winner at the end of the game (default is 1).
         :param reward_loser: Reward (penalty) given to the loser at the end of the game (default is -1).
         :param living_reward: Reward given at each step of the game, applicable to all ongoing games (default is 0).
         :param max_steps: Maximum number of steps the game can take before ending (default is 100).
         :param delay: Time delay (in milliseconds) between moves, primarily used for GUI purposes (default is 100).
-        :param avatar_player_1: avatar image player 1
-        :param avatar_player_2: avatar image player 2
+        :param avatar_player_1: avatar image player 1 base64/path
+        :param avatar_player_2: avatar image player 2 base64/path
+        :param reward_draw: Reward given to both players in case of a draw (default is 0).
+
         Initializes the environment with the specified dimensions and settings. It sets up spaces for observations
         and actions based on the game rules, as well as initializing a renderer for graphical display.
         """
         self.connect = connect
         self.width = width
         self.height = height
 
         self.reward_loser = reward_loser
         self.reward_winner = reward_winner
         self.living_reward = living_reward
+        self.reward_draw = reward_draw
 
         self.max_steps = max_steps
         self.current_step = 0
         self.is_done = False
 
         self.delay = delay
 
@@ -299,15 +302,15 @@
         Processes a move made by the current player by placing a chip in the specified column, then checks for game termination.
 
         :param movecol: The column number (zero-indexed) where the current player wishes to place their chip.
 
         :return: A tuple containing four elements:
             - Observations: Current state of the board from the perspective of both players.
             - Reward_players: A dictionary detailing the rewards for player 1 and player 2 based on the latest move.
-            - Is_done: Boolean value indicating whether the game has ended (either by a win or a full board).
+            - terminated: Boolean value indicating whether the game has ended (either by a win or a full board).
             - Info: A dictionary containing additional information such as legal actions for the next move and the next player.
 
         Raises:
             IndexError: If the move is invalid (e.g., the column is full or out of bounds).
 
         This method updates the game state by inserting a chip into the chosen column, checks for a winner, updates the current
         player, and calculates the rewards based on the state of the game. It also updates the display through the renderer and
@@ -328,19 +331,18 @@
         self.winner, reward_vector = self.check_for_episode_termination(movecol, row)
 
         info = {'legal_actions': self.get_moves(), 'next_player': self.current_player + 1}
         reward_players = {'player_1': reward_vector[0], 'player_2': reward_vector[1]}
         self.is_done = self.winner is not None
         self.renderer.update_display()
 
-        obs = self.get_player_observations()
+        observations = self.get_player_observations()
         terminated = self.is_done
-        truncated = False
 
-        return obs, reward_players, terminated, truncated, info
+        return observations, reward_players, terminated, False, info
 
     def reset(self) -> List[np.ndarray]:
         """
         Resets the game environment to its initial state. This method is typically called at the start of each new game.
 
         :return: A list of numpy arrays representing the initial observations of the game board for both players.
                      Each observation is an ndarray showing the current state of the board from the player's perspective.
@@ -435,15 +437,15 @@
             winner = 1 - self.current_player
             if winner == 0:
                 reward_vector = [self.reward_winner, self.reward_loser]
             elif winner == 1:
                 reward_vector = [self.reward_loser, self.reward_winner]
         elif self.get_moves() == []:
             winner = -1
-            reward_vector = [0, 0]
+            reward_vector = [self.reward_draw, self.reward_draw]
         return winner, reward_vector
 
     def get_moves(self):
         """
            Get the available moves for the current game state.
 
            Returns:
```

### Comparing `gymconnectx-1.0.6/gymconnectx.egg-info/PKG-INFO` & `gymconnectx-1.1.0/gymconnectx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gymconnectx
-Version: 1.0.6
+Version: 1.1.0
 Summary: An OpenAI Gym Environment Connect X Game with GUI. ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N.
 Home-page: https://github.com/fauzisho/GymConnectX
 Author: Fauzi Sholichin
 License: MIT License
         
         Copyright (c) 2024 Fauzi Sholichin
```

### Comparing `gymconnectx-1.0.6/pyproject.toml` & `gymconnectx-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gymconnectx"
-version = "1.0.6"
+version = "1.1.0"
 description = "An OpenAI Gym Environment Connect X Game with GUI. ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N."
 readme = "README.md"
 authors = [{ name = "Fauzi Sholichin" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `gymconnectx-1.0.6/setup.py` & `gymconnectx-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gymconnectx',
-    version='1.0.6',
+    version='1.1.0',
     description='ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N.',
     url='https://github.com/fauzisho/GymConnectX',
     author='Fauzi Sholichin',
     license='MIT License',
     packages=find_packages(),
     install_requires=['gym', 'pygame', 'numpy'],
     classifiers=[
```

