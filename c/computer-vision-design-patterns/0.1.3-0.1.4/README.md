# Comparing `tmp/computer_vision_design_patterns-0.1.3.tar.gz` & `tmp/computer_vision_design_patterns-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computer_vision_design_patterns-0.1.3.tar", max compression
+gzip compressed data, was "computer_vision_design_patterns-0.1.4.tar", max compression
```

## Comparing `computer_vision_design_patterns-0.1.3.tar` & `computer_vision_design_patterns-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-03-15 19:53:30.502092 computer_vision_design_patterns-0.1.3/computer_vision_design_patterns/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 19:53:30.503135 computer_vision_design_patterns-0.1.3/computer_vision_design_patterns/alarm.py
--rw-r--r--   0        0        0     1070 2024-03-15 23:43:16.152608 computer_vision_design_patterns-0.1.3/computer_vision_design_patterns/counter.py
--rw-r--r--   0        0        0     1353 2024-04-26 23:53:10.802100 computer_vision_design_patterns-0.1.3/computer_vision_design_patterns/event.py
--rw-r--r--   0        0        0      445 2024-05-08 15:26:59.605413 computer_vision_design_patterns-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      303 2024-05-08 15:22:11.610238 computer_vision_design_patterns-0.1.3/README.md
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 computer_vision_design_patterns-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-15 19:53:30.502092 computer_vision_design_patterns-0.1.4/computer_vision_design_patterns/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 19:53:30.503135 computer_vision_design_patterns-0.1.4/computer_vision_design_patterns/alarm.py
+-rw-r--r--   0        0        0     1058 2024-05-27 18:26:34.879102 computer_vision_design_patterns-0.1.4/computer_vision_design_patterns/counter.py
+-rw-r--r--   0        0        0     1245 2024-05-27 18:26:34.907330 computer_vision_design_patterns-0.1.4/computer_vision_design_patterns/event.py
+-rw-r--r--   0        0        0      442 2024-05-27 18:39:16.745368 computer_vision_design_patterns-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      303 2024-05-08 15:22:11.610238 computer_vision_design_patterns-0.1.4/README.md
+-rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 computer_vision_design_patterns-0.1.4/PKG-INFO
```

### Comparing `computer_vision_design_patterns-0.1.3/computer_vision_design_patterns/counter.py` & `computer_vision_design_patterns-0.1.4/computer_vision_design_patterns/counter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-import time
 from abc import ABC, abstractmethod
 
 from transitions import Machine, State
 
 
 class Counter(ABC, Machine):
     inactive = State(name="inactive")
```

### Comparing `computer_vision_design_patterns-0.1.3/computer_vision_design_patterns/event.py` & `computer_vision_design_patterns-0.1.4/computer_vision_design_patterns/event.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 import time
-from abc import ABC, abstractmethod
+from abc import ABC
 
 from transitions import Machine, State
 
 # Auto deactivating Event
 
 # Manual deactivating Event
 
 
 class Event(ABC, Machine):
     inactive = State(name="inactive")
     active = State(name="active")
 
     states = [inactive, active]
     transitions = [
-        {"trigger": "activate", "source": inactive, "dest": active},
+        {"trigger": "activate", "source": "*", "dest": active},
         {"trigger": "deactivate", "source": "*", "dest": inactive},
     ]
 
     def __init__(self):
         Machine.__init__(self, states=Event.states,
                          transitions=Event.transitions,
                          initial=Event.inactive)
@@ -42,11 +42,7 @@
                 self.deactivate()
                 self._last_call_time = None
 
     def retrive_state(self):
         self._update_timer()
 
         return self.state
-
-    def is_active(self):
-        self._update_timer()
-        return self.is_active()
```

### Comparing `computer_vision_design_patterns-0.1.3/PKG-INFO` & `computer_vision_design_patterns-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: computer-vision-design-patterns
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Federico Lanzani
-Author-email: federico@federicolanzani.com
+Author-email: hello@federicolanzani.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

