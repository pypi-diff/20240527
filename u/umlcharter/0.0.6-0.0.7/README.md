# Comparing `tmp/umlcharter-0.0.6.tar.gz` & `tmp/umlcharter-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umlcharter-0.0.6.tar", last modified: Thu May 16 14:57:47 2024, max compression
+gzip compressed data, was "umlcharter-0.0.7.tar", last modified: Mon May 27 15:22:45 2024, max compression
```

## Comparing `umlcharter-0.0.6.tar` & `umlcharter-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:47.705645 umlcharter-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 14:57:43.000000 umlcharter-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-16 14:57:47.705645 umlcharter-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-16 14:57:43.000000 umlcharter-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:57:47.705645 umlcharter-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-16 14:57:43.000000 umlcharter-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:47.701645 umlcharter-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:43.000000 umlcharter-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22213 2024-05-16 14:57:43.000000 umlcharter-0.0.6/tests/test_sequence_diagram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:47.701645 umlcharter-0.0.6/umlcharter/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:47.705645 umlcharter-0.0.6/umlcharter/charts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/charts/sequence_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/charts/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:47.705645 umlcharter-0.0.6/umlcharter/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/generators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:47.705645 umlcharter-0.0.6/umlcharter/generators/d2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/generators/d2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/generators/d2/d2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/generators/d2/sequence_diagram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:47.705645 umlcharter-0.0.6/umlcharter/generators/mermaid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/generators/mermaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/generators/mermaid/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/generators/mermaid/sequence_diagram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:47.705645 umlcharter-0.0.6/umlcharter/generators/plantuml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/generators/plantuml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/generators/plantuml/plantuml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/generators/plantuml/sequence_diagram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:47.705645 umlcharter-0.0.6/umlcharter/generators/sequencediagramorg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/generators/sequencediagramorg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/generators/sequencediagramorg/sequence_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-16 14:57:43.000000 umlcharter-0.0.6/umlcharter/generators/sequencediagramorg/sequencediagramorg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:57:47.705645 umlcharter-0.0.6/umlcharter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-16 14:57:47.000000 umlcharter-0.0.6/umlcharter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-16 14:57:47.000000 umlcharter-0.0.6/umlcharter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:57:47.000000 umlcharter-0.0.6/umlcharter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 14:57:47.000000 umlcharter-0.0.6/umlcharter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:45.434495 umlcharter-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-27 15:22:42.000000 umlcharter-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-27 15:22:45.434495 umlcharter-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-27 15:22:42.000000 umlcharter-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:22:45.434495 umlcharter-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-27 15:22:42.000000 umlcharter-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:45.430495 umlcharter-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:42.000000 umlcharter-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26585 2024-05-27 15:22:42.000000 umlcharter-0.0.7/tests/test_sequence_diagram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:45.430495 umlcharter-0.0.7/umlcharter/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:45.430495 umlcharter-0.0.7/umlcharter/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14101 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/charts/sequence_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/charts/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:45.430495 umlcharter-0.0.7/umlcharter/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/generators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:45.434495 umlcharter-0.0.7/umlcharter/generators/d2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/generators/d2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/generators/d2/d2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/generators/d2/sequence_diagram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:45.434495 umlcharter-0.0.7/umlcharter/generators/mermaid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/generators/mermaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/generators/mermaid/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/generators/mermaid/sequence_diagram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:45.434495 umlcharter-0.0.7/umlcharter/generators/plantuml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/generators/plantuml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/generators/plantuml/plantuml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/generators/plantuml/sequence_diagram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:45.434495 umlcharter-0.0.7/umlcharter/generators/sequencediagramorg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/generators/sequencediagramorg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/generators/sequencediagramorg/sequence_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-27 15:22:42.000000 umlcharter-0.0.7/umlcharter/generators/sequencediagramorg/sequencediagramorg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:22:45.434495 umlcharter-0.0.7/umlcharter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-27 15:22:45.000000 umlcharter-0.0.7/umlcharter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-27 15:22:45.000000 umlcharter-0.0.7/umlcharter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:22:45.000000 umlcharter-0.0.7/umlcharter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 15:22:45.000000 umlcharter-0.0.7/umlcharter.egg-info/top_level.txt
```

### Comparing `umlcharter-0.0.6/LICENSE` & `umlcharter-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `umlcharter-0.0.6/PKG-INFO` & `umlcharter-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umlcharter
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package for quick diagrams creation without a need to learn new DSL
 Home-page: https://github.com/mikalaiyurkin/charter
 Author: Mikalai Yurkin
 Author-email: yurkin.mikalai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `umlcharter-0.0.6/README.md` & `umlcharter-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `umlcharter-0.0.6/setup.py` & `umlcharter-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `umlcharter-0.0.6/tests/test_sequence_diagram.py` & `umlcharter-0.0.7/tests/test_sequence_diagram.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,16 +60,16 @@
 @enduml
 """,
             ),
             (
                 D2,
                 """title: Diagram Only Participants {
 shape: sequence_diagram
-p1: First
-p2: Second
+p1: First 
+p2: Second 
 }
 """,
             ),
             (
                 SequenceDiagramOrg,
                 """title Diagram Only Participants
 participant "First" as p1
@@ -183,18 +183,18 @@
 """,
             ),
             (
                 D2,
                 True,
                 """title: Diagram Interaction\\nand Auto Activation {
 shape: sequence_diagram
-p1: First\\nParticipant
-p2: Second\\nParticipant
-p3: Third\\nParticipant
-p4: Fourth\\nParticipant
+p1: First\\nParticipant 
+p2: Second\\nParticipant 
+p3: Third\\nParticipant 
+p4: Fourth\\nParticipant 
 p1.0 -> p2.1: Go to second
 p2.1 -> p1.0: Return to first {style.stroke-dash: 3}
 p1.2 -> p3.3: Go to third
 p3.3 -> p4.4: Go to fourth
 p4.4 -> p4.4: Go to self
 p4.4 -> p3.3: Return to third {style.stroke-dash: 3}
 p3.3 -> p1.2: Return to first {style.stroke-dash: 3}
@@ -202,18 +202,18 @@
 """,
             ),
             (
                 D2,
                 False,
                 """title: Diagram Interaction\\nand Auto Activation {
 shape: sequence_diagram
-p1: First\\nParticipant
-p2: Second\\nParticipant
-p3: Third\\nParticipant
-p4: Fourth\\nParticipant
+p1: First\\nParticipant 
+p2: Second\\nParticipant 
+p3: Third\\nParticipant 
+p4: Fourth\\nParticipant 
 p1 -> p2: Go to second
 p2 -> p1: Return to first {style.stroke-dash: 3}
 p1 -> p3: Go to third
 p3 -> p4: Go to fourth
 p4 -> p4: Go to self
 p4 -> p3: Return to third {style.stroke-dash: 3}
 p3 -> p1: Return to first {style.stroke-dash: 3}
@@ -320,16 +320,16 @@
 @enduml
 """,
             ),
             (
                 D2,
                 """title: Diagram Interaction and Manual Activation {
 shape: sequence_diagram
-p1: First
-p2: Second
+p1: First 
+p2: Second 
 p1.0 -> p2.1: Go to second
 p2.1 -> p2.1: Go to self
 p2.1 -> p1.0: Return to first {style.stroke-dash: 3}
 }
 """,
             ),
             (
@@ -417,17 +417,17 @@
 @enduml
 """,
             ),
             (
                 D2,
                 """title: Diagram Interaction and Grouping {
 shape: sequence_diagram
-p1: First
-p2: Second
-p3: Third
+p1: First 
+p2: Second 
+p3: Third 
 Group enclosing everything: {
 p1.0 -> p2.1: Go to second
 Group enclosing interaction\\nbetween second and third: {
 p2.1 -> p3.2: Go to third
 p3.2 -> p2.1: Return to second {style.stroke-dash: 3}
 }
 p2.1 -> p1.0: Return to first {style.stroke-dash: 3}
@@ -517,16 +517,16 @@
 @enduml
 """,
             ),
             (
                 D2,
                 """title: Diagram Interaction and Loops {
 shape: sequence_diagram
-p1: First
-p2: Second
+p1: First 
+p2: Second 
 LOOP Infinite loop: {
 style: {
 border-radius: 50
 fill: "#ffdfbf"
 }
 p1.0 -> p2.1: Send request to second
 LOOP Repeat\\nuntil available: {
@@ -637,17 +637,17 @@
 @enduml
 """,
             ),
             (
                 D2,
                 """title: Diagram Interaction and Conditions {
 shape: sequence_diagram
-p1: Viewer
-p2: Drama
-p3: Comedy
+p1: Viewer 
+p2: Drama 
+p3: Comedy 
 p1.0 -> p1.0: What would I like to watch today?
 alt1: ALT {
 style: {
 fill: "#ffdfbf"
 }
 CASE Want a drama: {
 style: {
@@ -759,16 +759,16 @@
 @enduml
 """,
             ),
             (
                 D2,
                 """title: Diagram Interaction and Notes {
 shape: sequence_diagram
-p1: Batman
-p2: Bandit
+p1: Batman 
+p2: Bandit 
 p1."Batman is throwing\\na batarang at the bandit"
 p1.0 -> p2.1: Pheeeeeeu!
 p2.1."Batman has missed!"
 p2.1 -> p1.0: A bad day\\nfor the Gotham :( {style.stroke-dash: 3}
 p1."Batman is sad now"
 }
 """,
@@ -839,16 +839,16 @@
 @enduml
 """,
             ),
             (
                 D2,
                 """title: Empty Transitions between Participants {
 shape: sequence_diagram
-p1: First
-p2: Second
+p1: First 
+p2: Second 
 p1.0 -> p2.1: ''
 p2.1 -> p1.0: '' {style.stroke-dash: 3}
 }
 """,
             ),
             (
                 SequenceDiagramOrg,
@@ -869,14 +869,124 @@
         sd = SequenceDiagram("Empty Transitions between Participants", generator_cls)
         first = sd.participant("First")
         second = sd.participant("Second")
 
         first.go_to(second).return_to(first)
         assert str(sd) == output
 
+    @pytest.mark.parametrize(
+        "generator_cls,output",
+        (
+            (
+                Mermaid,
+                """sequenceDiagram
+Title: Participant types, according to ECB
+actor p1 as Actor
+participant p2 as Boundary
+participant p3 as Control
+participant p4 as Entity
+activate p1
+p1->>p2: Do something
+activate p2
+p2->>p3: Do something
+activate p3
+p3->>p4: Do something
+activate p4
+p4-->>p3: Return
+deactivate p4
+p3-->>p2: Return
+deactivate p3
+p2-->>p1: Return
+deactivate p2
+deactivate p1
+""",
+            ),
+            (
+                PlantUML,
+                """@startuml
+title: Participant types, according to ECB
+actor "Actor" as p1
+boundary "Boundary" as p2
+control "Control" as p3
+entity "Entity" as p4
+activate p1
+p1->p2: Do something
+activate p2
+p2->p3: Do something
+activate p3
+p3->p4: Do something
+activate p4
+p4-->p3: Return
+deactivate p4
+p3-->p2: Return
+deactivate p3
+p2-->p1: Return
+deactivate p2
+deactivate p1
+@enduml
+""",
+            ),
+            (
+                D2,
+                """title: Participant types, according to ECB {
+shape: sequence_diagram
+p1: Actor {shape: person}
+p2: Boundary 
+p3: Control 
+p4: Entity 
+p1.0 -> p2.1: Do something
+p2.1 -> p3.2: Do something
+p3.2 -> p4.3: Do something
+p4.3 -> p3.2: Return {style.stroke-dash: 3}
+p3.2 -> p2.1: Return {style.stroke-dash: 3}
+p2.1 -> p1.0: Return {style.stroke-dash: 3}
+}
+""",
+            ),
+            (
+                SequenceDiagramOrg,
+                """title Participant types, according to ECB
+actor "Actor" as p1
+boundary "Boundary" as p2
+control "Control" as p3
+entity "Entity" as p4
+activate p1
+p1->p2: Do something
+activate p2
+p2->p3: Do something
+activate p3
+p3->p4: Do something
+activate p4
+p4-->p3: Return
+deactivate p4
+p3-->p2: Return
+deactivate p3
+p2-->p1: Return
+deactivate p2
+deactivate p1
+""",
+            ),
+        ),
+    )
+    def test_ecb_types_for_participants(self, generator_cls, output):
+        sd = SequenceDiagram("Participant types, according to ECB", generator_cls)
+        actor = sd.participant("Actor").as_actor()
+        boundary = sd.participant("Boundary").as_boundary()
+        control = sd.participant("Control").as_control()
+        entity = sd.participant("Entity").as_entity()
+
+        actor.go_to(boundary, "Do something").go_to(control, "Do something").go_to(
+            entity, "Do something"
+        )
+        entity.return_to(control, "Return").return_to(boundary, "Return").return_to(
+            actor, "Return"
+        )
+
+        assert str(sd) == output
+
     def test_same_participants(self):
         sd = SequenceDiagram("Same participants", Mock)
 
         sd.participant("Same")
         with pytest.raises(AssertionError):
             sd.participant(
                 "Same"
@@ -911,7 +1021,68 @@
 
     def test_force_case_inside_condition(self):
         sd = SequenceDiagram("Violated order of condition and case #2", Mock)
 
         with pytest.raises(AssertionError):
             with sd.case("A case"):
                 pass
+
+    @pytest.mark.parametrize(
+        "callable_", ("as_actor", "as_boundary", "as_control", "as_entity")
+    )
+    def test_force_participant_type_being_set_only_once(self, callable_):
+        sd = SequenceDiagram("Participant type can be set only once", Mock)
+
+        a = sd.participant("Someone")
+        a.type_ = "SET TO SOMETHING ELSE BUT NOT DEFAULT"
+        with pytest.raises(AssertionError):
+            getattr(a, callable_)()
+
+    @pytest.mark.parametrize(
+        "from_,to_",
+        (
+            ("actor", "actor"),
+            ("actor", "control"),
+            ("actor", "entity"),
+            ("boundary", "boundary"),
+            ("boundary", "entity"),
+            ("control", "actor"),
+            ("entity", "actor"),
+            ("entity", "boundary"),
+        ),
+    )
+    def test_only_certain_forward_interactions_are_available(self, from_, to_):
+        sd = SequenceDiagram("Not available interactions", Mock)
+
+        a = sd.participant("a")
+        b = sd.participant("b")
+
+        a.type_ = from_
+        b.type_ = to_
+
+        with pytest.raises(AssertionError):
+            a.go_to(b, "Do something")
+
+    @pytest.mark.parametrize(
+        "from_,to_",
+        (
+            ("actor", "actor"),
+            ("actor", "control"),
+            ("actor", "entity"),
+            ("boundary", "boundary"),
+            ("boundary", "entity"),
+            ("control", "actor"),
+            ("entity", "actor"),
+            ("entity", "boundary"),
+        ),
+    )
+    def test_only_certain_return_interactions_are_available(self, from_, to_):
+        sd = SequenceDiagram("Not available interactions", Mock)
+
+        a = sd.participant("a")
+        b = sd.participant("b")
+
+        a.type_ = from_
+        b.type_ = to_
+
+        with pytest.raises(AssertionError):
+            a.return_to(b, "Do something")
```

### Comparing `umlcharter-0.0.6/umlcharter/charts/sequence_diagram.py` & `umlcharter-0.0.7/umlcharter/charts/sequence_diagram.py`

 * *Files 19% similar despite different names*

```diff
@@ -59,29 +59,100 @@
     text: str
 
 
 @dataclass
 class SequenceDiagramParticipant:
     sequence_ref: "SequenceDiagram"
     title: str
+    type_: typing.Literal["actor", "boundary", "control", "entity", "default"] = field(
+        init=False, default="default"
+    )
+
+    def __check_can_set_type(self):
+        if self.type_ != "default":
+            raise AssertionError(
+                f"The type of the participant must be set only once. The current type is '{self.type_}'"
+            )
+
+    def as_actor(self):
+        self.__check_can_set_type()
+        self.type_ = "actor"
+        return self
+
+    def as_boundary(self):
+        self.__check_can_set_type()
+        self.type_ = "boundary"
+        return self
+
+    def as_control(self):
+        self.__check_can_set_type()
+        self.type_ = "control"
+        return self
+
+    def as_entity(self):
+        self.__check_can_set_type()
+        self.type_ = "entity"
+        return self
+
+    def __check_if_interaction_is_possible(self, to: "SequenceDiagramParticipant"):
+        """
+        The check is based on the purpose of the participant, according to the ECB.
+        https://en.wikipedia.org/wiki/Entity-control-boundary
+
+        If the type of the participant is not "default" then only the specific interactions are available:
+
+        - Actors may only know and communicate with boundaries.
+        - Boundaries may communicate with actors and controls only.
+        - Controls may know and communicate with boundaries and entities, and if needed other controls.
+        - Entities may only know about other entities but could communicate also with controls.
+
+        |          | default | actor | boundary | control | entity |
+        ------------------------------------------------------------
+        | default  |    v    |   v   |     v    |    v    |   v    |
+        | actor    |    v    |       |     v    |         |        |
+        | boundary |    v    |   v   |          |    v    |        |
+        | control  |    v    |       |     v    |    v    |   v    |
+        | entity   |    v    |       |          |    v    |   v    |
+        """
+        allowed = (
+            {"default", "default"},
+            {"default", "actor"},
+            {"default", "boundary"},
+            {"default", "control"},
+            {"default", "entity"},
+            {"actor", "boundary"},
+            {"boundary", "control"},
+            {"control", "control"},
+            {"control", "entity"},
+            {"entity", "entity"},
+        )
+
+        if {self.type_, to.type_} not in allowed:
+            raise AssertionError(
+                f"The interaction between '{self.type_}' to '{to.type_}' is not allowed. "
+                f"Please correct the types of the participants or remove the use of the types "
+                f"if you do not really care about it."
+            )
 
     def __add_step(
         self, step: typing.Union[ForwardStep, ReturnStep, ParticipantActivationControl]
     ):
         self.sequence_ref._SequenceDiagram__add_step(step)  # noqa
 
     def go_to(
         self, to: "SequenceDiagramParticipant", text: str = ""
     ) -> "SequenceDiagramParticipant":
+        self.__check_if_interaction_is_possible(to)
         self.__add_step(ForwardStep(text, from_participant=self, to_participant=to))
         return to
 
     def return_to(
         self, to: "SequenceDiagramParticipant", text: str = ""
     ) -> "SequenceDiagramParticipant":
+        self.__check_if_interaction_is_possible(to)
         self.__add_step(ReturnStep(text, from_participant=self, to_participant=to))
         return to
 
     @contextmanager
     def activate(self):
         """
         Explicitly activate the participant in the diagram on start of the context manager and ends on its exit.
```

### Comparing `umlcharter-0.0.6/umlcharter/generators/d2/sequence_diagram.py` & `umlcharter-0.0.7/umlcharter/generators/d2/sequence_diagram.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,19 +31,25 @@
             last_targeted_participant = participants[0]
 
         aliases = {
             participant: f"p{index + 1}"
             for index, participant in enumerate(participants)
         }
 
+        participant_types_map = {
+            "default": "",
+            "actor": "{shape: person}",
+            "boundary": "",
+            "control": "",
+            "entity": "",
+        }
+
         generated = f"title: {cls._line_break(sequence_diagram.title)} {{\nshape: sequence_diagram\n"
         for participant in participants:
-            generated += (
-                f"{aliases[participant]}: {cls._line_break(participant.title)}\n"
-            )
+            generated += f"{aliases[participant]}: {cls._line_break(participant.title)} {participant_types_map[participant.type_]}\n"
 
         # NB! In D2 the logic of "activation" phases or "spans" works a bit differently, compared to the other DSLs.
         # You have to know that the participant will be activated
         # BEFORE the flow goes under the new participant control.
         # To align the activation representation with the other DSLs, we have to
         # 1. Check if the step is `ForwardStep` to the participant X
         # 2. If right after the `ForwardStep` participant X is activated -
```

### Comparing `umlcharter-0.0.6/umlcharter/generators/mermaid/sequence_diagram.py` & `umlcharter-0.0.7/umlcharter/generators/mermaid/sequence_diagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,25 @@
                 "rgb(153, 221, 255)",
                 "rgb(51, 187, 255)",
                 "rgb(0, 179, 179)",
                 "rgb(184, 184, 148)",
             ]
         )
 
+        participant_types_map = {
+            "default": "participant",
+            "actor": "actor",
+            "boundary": "participant",
+            "control": "participant",
+            "entity": "participant",
+        }
+
         generated = f"sequenceDiagram\nTitle: {cls._remove_line_breaks(sequence_diagram.title)}\n"
         for participant in participants:
-            generated += f"participant {aliases[participant]} as {cls._line_break(participant.title)}\n"
+            generated += f"{participant_types_map[participant.type_]} {aliases[participant]} as {cls._line_break(participant.title)}\n"
 
         for step in sequence:
             if isinstance(step, ParticipantActivationControl):
                 if step.is_active:
                     generated += f"activate {aliases[step.participant]}\n"
                 else:
                     generated += f"deactivate {aliases[step.participant]}\n"
```

### Comparing `umlcharter-0.0.6/umlcharter/generators/plantuml/sequence_diagram.py` & `umlcharter-0.0.7/umlcharter/generators/plantuml/sequence_diagram.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,17 +35,25 @@
             last_targeted_participant = participants[0]
 
         aliases = {
             participant: f"p{index + 1}"
             for index, participant in enumerate(participants)
         }
 
+        participant_types_map = {
+            "default": "participant",
+            "actor": "actor",
+            "boundary": "boundary",
+            "control": "control",
+            "entity": "entity",
+        }
+
         generated = f"@startuml\ntitle: {cls._line_break(sequence_diagram.title)}\n"
         for participant in participants:
-            generated += f'participant "{cls._line_break(participant.title)}" as {aliases[participant]}\n'
+            generated += f'{participant_types_map[participant.type_]} "{cls._line_break(participant.title)}" as {aliases[participant]}\n'
 
         for step in sequence:
             if isinstance(step, ParticipantActivationControl):
                 if step.is_active:
                     # NB! The magic of PlantUML:
                     # you cannot activate the participant right after you have deactivated it,
                     # so you to place something in between.
```

### Comparing `umlcharter-0.0.6/umlcharter/generators/sequencediagramorg/sequence_diagram.py` & `umlcharter-0.0.7/umlcharter/generators/sequencediagramorg/sequence_diagram.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,25 @@
             last_targeted_participant = participants[0]
 
         aliases = {
             participant: f"p{index + 1}"
             for index, participant in enumerate(participants)
         }
 
+        participant_types_map = {
+            "default": "participant",
+            "actor": "actor",
+            "boundary": "boundary",
+            "control": "control",
+            "entity": "entity",
+        }
+
         generated = f"title {cls._line_break(sequence_diagram.title)}\n"
         for participant in participants:
-            generated += f'participant "{cls._line_break(participant.title)}" as {aliases[participant]}\n'
+            generated += f'{participant_types_map[participant.type_]} "{cls._line_break(participant.title)}" as {aliases[participant]}\n'
 
         for step in sequence:
             if isinstance(step, ParticipantActivationControl):
                 if step.is_active:
                     generated += f"activate {aliases[step.participant]}\n"
                 else:
                     generated += f"deactivate {aliases[step.participant]}\n"
```

### Comparing `umlcharter-0.0.6/umlcharter.egg-info/PKG-INFO` & `umlcharter-0.0.7/umlcharter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umlcharter
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package for quick diagrams creation without a need to learn new DSL
 Home-page: https://github.com/mikalaiyurkin/charter
 Author: Mikalai Yurkin
 Author-email: yurkin.mikalai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `umlcharter-0.0.6/umlcharter.egg-info/SOURCES.txt` & `umlcharter-0.0.7/umlcharter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

