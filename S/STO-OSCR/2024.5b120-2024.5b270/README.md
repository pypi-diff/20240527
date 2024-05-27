# Comparing `tmp/sto_oscr-2024.5b120.tar.gz` & `tmp/sto_oscr-2024.5b270.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Tue Jan  1 00:00:00 1980, max compression
```

## Comparing `sto_oscr-2024.5b120.tar` & `sto_oscr-2024.5b270.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/.flake8
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/__init__.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/cli.py
--rw-r--r--   0        0        0    14305 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/combat.py
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/datamodels.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/detection.py
--rw-r--r--   0        0        0    11062 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/iofunc.py
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/liveparser.py
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/main.py
--rw-r--r--   0        0        0    23569 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/parser.py
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/utilities.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/LICENSE
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/pyproject.toml
--rw-r--r--   0        0        0    41256 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/PKG-INFO
+-rw-r--r--   0        0        0       58 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/.flake8
+-rw-r--r--   0        0        0       98 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1381 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/OSCR/__init__.py
+-rw-r--r--   0        0        0     2569 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/OSCR/cli.py
+-rw-r--r--   0        0        0    14305 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/OSCR/combat.py
+-rw-r--r--   0        0        0    16440 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/OSCR/datamodels.py
+-rw-r--r--   0        0        0    10460 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/OSCR/detection.py
+-rw-r--r--   0        0        0    11062 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/OSCR/iofunc.py
+-rw-r--r--   0        0        0     9887 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/OSCR/liveparser.py
+-rw-r--r--   0        0        0     9632 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/OSCR/main.py
+-rw-r--r--   0        0        0    23901 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/OSCR/parser.py
+-rw-r--r--   0        0        0     3212 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/OSCR/utilities.py
+-rw-r--r--   0        0        0    35149 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/LICENSE
+-rw-r--r--   0        0        0      181 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/README.md
+-rw-r--r--   0        0        0      899 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/pyproject.toml
+-rw-r--r--   0        0        0    41256 1980-01-01 00:00:00.000000 sto_oscr-2024.5b270/PKG-INFO
```

### Comparing `sto_oscr-2024.5b120/OSCR/__init__.py` & `sto_oscr-2024.5b270/OSCR/__init__.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.5b120/OSCR/cli.py` & `sto_oscr-2024.5b270/OSCR/cli.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.5b120/OSCR/combat.py` & `sto_oscr-2024.5b270/OSCR/combat.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.5b120/OSCR/datamodels.py` & `sto_oscr-2024.5b270/OSCR/datamodels.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.5b120/OSCR/detection.py` & `sto_oscr-2024.5b270/OSCR/detection.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.5b120/OSCR/iofunc.py` & `sto_oscr-2024.5b270/OSCR/iofunc.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.5b120/OSCR/liveparser.py` & `sto_oscr-2024.5b270/OSCR/liveparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,16 +179,16 @@
                         or attack_data[8] == 'HitPoints')
                 is_kill = 'Kill' in attack_data[9]
                 magnitude = abs(magnitude)
                 magnitude2 = abs(magnitude2)
 
                 # ignore self damage and damage from unknown sources
                 try:
-                    attacker_handle = attack_data[1].split(' ', 1)[1][:-1]
-                    target_handle = attack_data[5].split(' ', 1)[1][:-1]
+                    attacker_handle = attack_data[1].split('@', 2)[-1][:-1]
+                    target_handle = attack_data[5].split('@', 2)[-1][:-1]
                 except IndexError:
                     if not is_heal:
                         continue
 
                 if player_attacks:
                     if attacker_handle not in self._players:
                         with self._lock:
```

### Comparing `sto_oscr-2024.5b120/OSCR/main.py` & `sto_oscr-2024.5b270/OSCR/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .iofunc import get_combat_log_data, reset_temp_folder, save_log, split_log_by_lines
 from .parser import analyze_combat
 from .utilities import datetime_to_display, to_datetime
 
 
 class OSCR():
 
-    version = '2024.05b120'
+    version = '2024.05b270'
 
     def __init__(self, log_path: str = None, settings: dict = None):
         self.log_path = log_path
         self.combats: list[Combat] = list()
         self.combats_pointer = None
         self.excess_log_lines = list()
         self.combatlog_tempfiles = list()
@@ -112,15 +112,15 @@
         for line_num, line in enumerate(log_lines):
             time_data, attack_data = line.split('::')
             log_time = to_datetime(time_data)
             if last_log_time - log_time > combat_delta:
                 if len(current_combat.log_data) >= 20:
                     current_combat.start_time = last_log_time
                     self.combats.append(current_combat)
-                    current_combat = Combat()
+                current_combat = Combat()
                 if len(self.combats) >= total_combats:
                     self.excess_log_lines = log_lines[line_num:]
                     return
             splitted_line = attack_data.split(',')
             current_line = LogLine(
                     log_time,
                     *splitted_line[:10],
```

### Comparing `sto_oscr-2024.5b120/OSCR/parser.py` & `sto_oscr-2024.5b270/OSCR/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,32 +77,21 @@
             # Combat Duration
             # Heals, damage taken and self-damage don't affect combat time
             if ability_target.name != '*':
                 try:
                     actor_combat_durations[line.owner_id][1] = timestamp
                 except KeyError:
                     actor_combat_durations[line.owner_id] = [timestamp, timestamp]
-                try:
-                    actor_combat_durations[line.source_id][1] = timestamp
-                except KeyError:
-                    actor_combat_durations[line.source_id] = [timestamp, timestamp]
+                if not line.source_id.startswith('P'):
+                    try:
+                        actor_combat_durations[line.source_id][1] = timestamp
+                    except KeyError:
+                        actor_combat_durations[line.source_id] = [timestamp, timestamp]
 
             # get table data
-            if miss_flag:
-                ability_target.misses += 1
-                source_ability.misses += 1
-            if kill_flag:
-                ability_target.kills += 1
-                source_ability.kills += 1
-            if flank_flag:
-                ability_target.flank_num += 1
-                source_ability.flank_num += 1
-            if crit_flag:
-                ability_target.crit_num += 1
-                source_ability.crit_num += 1
 
             magnitude = abs(line.magnitude)
             magnitude2 = abs(line.magnitude2)
             ability_target.total_damage += magnitude
             ability_target.total_base_damage += magnitude2
             ability_target.total_attacks += 1
             source_ability.total_damage += magnitude
@@ -126,14 +115,30 @@
                 ability_target.max_one_hit = magnitude
             if magnitude > source_ability.max_one_hit:
                 source_ability.max_one_hit = magnitude
 
             target_item.graph_data[relative_combat_sec] += magnitude
             source_item.graph_data[relative_combat_sec] += magnitude
 
+            if miss_flag:
+                ability_target.misses += 1
+                source_ability.misses += 1
+            if flank_flag:
+                ability_target.flank_num += 1
+                source_ability.flank_num += 1
+            if crit_flag:
+                ability_target.crit_num += 1
+                source_ability.crit_num += 1
+            if kill_flag:
+                ability_target.kills += 1
+                source_ability.kills += 1
+                if (combat.map == 'Hive Space'
+                        and ability_target.handle == 'Mission_Space_Borg_Queen_Diamond'):
+                    break  # ignore all lines after the Queen kill line in the Hive Space queue
+
     for actor_id, (start_time, end_time) in actor_combat_durations.items():
         actor_combat_durations[actor_id] = round((end_time - start_time).total_seconds(), 1)
 
     merge_single_lines(dmg_out_model)
     combat_duration = combat_duration_delta.total_seconds()
     complete_damage_tree(dmg_out_model, actor_combat_durations, combat_duration)
     complete_damage_tree(dmg_in_model, actor_combat_durations, combat_duration)
@@ -469,15 +474,16 @@
     Parameters:
     - :param tree_model: tree model to analyze and improve
     '''
     for player in tree_model._player._children:
         new_pet_groups = dict()
 
         for ability_or_petgroup in player._children:
-            if not ability_or_petgroup._children or ability_or_petgroup._children[0].child_count == 0:
+            if (len(ability_or_petgroup._children) < 1
+                    or ability_or_petgroup._children[0].child_count == 0):
                 continue
 
             for pet in reversed(ability_or_petgroup._children):
                 if pet.child_count == 1:
                     ability_name = pet._children[0].data
                     if ability_or_petgroup.data == ability_name:
                         new_pet_group_name = ability_name
```

### Comparing `sto_oscr-2024.5b120/OSCR/utilities.py` & `sto_oscr-2024.5b270/OSCR/utilities.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.5b120/LICENSE` & `sto_oscr-2024.5b270/LICENSE`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.5b120/pyproject.toml` & `sto_oscr-2024.5b270/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.5b120/PKG-INFO` & `sto_oscr-2024.5b270/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: STO-OSCR
-Version: 2024.5b120
+Version: 2024.5b270
 Summary: Open Source Combatlog Reader for Star Trek Online.
 Project-URL: Homepage, https://github.com/STOCD/OSCR
 Project-URL: Repository, https://github.com/STOCD/OSCR.git
 Project-URL: Bug Tracker, https://github.com/STOCD/OSCR/issues
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

