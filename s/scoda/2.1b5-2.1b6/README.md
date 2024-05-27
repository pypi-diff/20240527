# Comparing `tmp/scoda-2.1b5.tar.gz` & `tmp/scoda-2.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-2.1b5.tar", last modified: Fri May 24 12:28:52 2024, max compression
+gzip compressed data, was "scoda-2.1b6.tar", last modified: Mon May 27 14:59:19 2024, max compression
```

## Comparing `scoda-2.1b5.tar` & `scoda-2.1b6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:28:52.454274 scoda-2.1b5/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-24 12:28:48.000000 scoda-2.1b5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-24 12:28:52.454274 scoda-2.1b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-24 12:28:48.000000 scoda-2.1b5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-24 12:28:48.000000 scoda-2.1b5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:28:52.446274 scoda-2.1b5/scoda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:28:52.446274 scoda-2.1b5/scoda/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/config/settings.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:28:52.446274 scoda-2.1b5/scoda/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/elements/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/elements/composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/elements/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/elements/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:28:52.450274 scoda-2.1b5/scoda/enumerations/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/enumerations/message_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/enumerations/tokenisation_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/enumerations/tokeniser_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:28:52.450274 scoda-2.1b5/scoda/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/exceptions/bar_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/exceptions/sequence_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/exceptions/tokenisation_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/exceptions/track_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:28:52.450274 scoda-2.1b5/scoda/midi/
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/midi/midi_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/midi/midi_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/midi/midi_track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:28:52.450274 scoda-2.1b5/scoda/misc/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/misc/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/misc/music_theory.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/misc/scoda_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/misc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:28:52.450274 scoda-2.1b5/scoda/sequences/
--rw-r--r--   0 runner    (1001) docker     (127)    21887 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/sequences/absolute_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/sequences/abstract_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    31799 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/sequences/relative_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    23992 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/sequences/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:28:52.450274 scoda-2.1b5/scoda/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/settings/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:28:52.450274 scoda-2.1b5/scoda/tokenisation/
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/tokenisation/base_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/tokenisation/gridlike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/tokenisation/midilike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26129 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/tokenisation/notelike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-05-24 12:28:48.000000 scoda-2.1b5/scoda/tokenisation/transposed_notelike_tokenisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:28:52.450274 scoda-2.1b5/scoda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-24 12:28:52.000000 scoda-2.1b5/scoda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-24 12:28:52.000000 scoda-2.1b5/scoda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:28:52.000000 scoda-2.1b5/scoda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-24 12:28:52.000000 scoda-2.1b5/scoda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 12:28:52.000000 scoda-2.1b5/scoda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:28:52.454274 scoda-2.1b5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.139394 scoda-2.1b6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-27 14:59:09.000000 scoda-2.1b6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-27 14:59:19.139394 scoda-2.1b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-27 14:59:09.000000 scoda-2.1b6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-27 14:59:09.000000 scoda-2.1b6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.135394 scoda-2.1b6/scoda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.135394 scoda-2.1b6/scoda/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/config/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.135394 scoda-2.1b6/scoda/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/elements/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/elements/composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/elements/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/elements/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.135394 scoda-2.1b6/scoda/enumerations/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/enumerations/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/enumerations/tokenisation_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/enumerations/tokeniser_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.135394 scoda-2.1b6/scoda/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/exceptions/bar_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/exceptions/sequence_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/exceptions/tokenisation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/exceptions/track_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.139394 scoda-2.1b6/scoda/midi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/midi/midi_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/midi/midi_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/midi/midi_track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.139394 scoda-2.1b6/scoda/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/misc/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/misc/music_theory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/misc/scoda_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/misc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.139394 scoda-2.1b6/scoda/sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)    21887 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/sequences/absolute_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/sequences/abstract_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31799 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/sequences/relative_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23992 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/sequences/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.139394 scoda-2.1b6/scoda/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/settings/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.139394 scoda-2.1b6/scoda/tokenisation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/tokenisation/base_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/tokenisation/gridlike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/tokenisation/midilike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30014 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/tokenisation/notelike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/tokenisation/transposed_notelike_tokenisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.139394 scoda-2.1b6/scoda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-27 14:59:19.000000 scoda-2.1b6/scoda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-27 14:59:19.000000 scoda-2.1b6/scoda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:59:19.000000 scoda-2.1b6/scoda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-27 14:59:19.000000 scoda-2.1b6/scoda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 14:59:19.000000 scoda-2.1b6/scoda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:59:19.139394 scoda-2.1b6/setup.cfg
```

### Comparing `scoda-2.1b5/LICENSE.md` & `scoda-2.1b6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/PKG-INFO` & `scoda-2.1b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda
-Version: 2.1b5
+Version: 2.1b6
 Summary: A MIDI and music data manipulation library
 Author-email: Felix Schön <schoen@kr.tuwien.ac.at>
 License: MIT License
         
         Copyright (c) 2023 Felix Schön
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `scoda-2.1b5/README.md` & `scoda-2.1b6/README.md`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/pyproject.toml` & `scoda-2.1b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scoda"
-version = "2.1-beta.5"
+version = "2.1-beta.6"
 authors = [{ name = "Felix Schön", email = "schoen@kr.tuwien.ac.at" }]
 description = "A MIDI and music data manipulation library"
 readme = "README.md"
 requires-python = ">= 3.11"
 keywords = ["midi", "music"]
 license = { file = "LICENSE.md" }
 dependencies = [
```

### Comparing `scoda-2.1b5/scoda/config/settings.json` & `scoda-2.1b6/scoda/config/settings.json`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/elements/bar.py` & `scoda-2.1b6/scoda/elements/bar.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/elements/composition.py` & `scoda-2.1b6/scoda/elements/composition.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/elements/message.py` & `scoda-2.1b6/scoda/elements/message.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/elements/track.py` & `scoda-2.1b6/scoda/elements/track.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/midi/midi_file.py` & `scoda-2.1b6/scoda/midi/midi_file.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/midi/midi_message.py` & `scoda-2.1b6/scoda/midi/midi_message.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/midi/midi_track.py` & `scoda-2.1b6/scoda/midi/midi_track.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/misc/music_theory.py` & `scoda-2.1b6/scoda/misc/music_theory.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         from_pos = CircleOfFifths.circle_of_fifths_order.index(Note(from_note_val % 12)) - 5
         to_pos = CircleOfFifths.circle_of_fifths_order.index(Note(to_note_val % 12)) - 5
 
         to_pos = (to_pos - from_pos) % 12
 
         distance_right = to_pos
         distance_left = 12 - distance_right
-        distance = None
 
         if distance_left == distance_right:
             distance = distance_right
         elif distance_right < distance_left:
             distance = distance_right
         else:
             distance = -distance_left
```

### Comparing `scoda-2.1b5/scoda/misc/scoda_logging.py` & `scoda-2.1b6/scoda/misc/scoda_logging.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/misc/util.py` & `scoda-2.1b6/scoda/misc/util.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/sequences/absolute_sequence.py` & `scoda-2.1b6/scoda/sequences/absolute_sequence.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/sequences/abstract_sequence.py` & `scoda-2.1b6/scoda/sequences/abstract_sequence.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/sequences/relative_sequence.py` & `scoda-2.1b6/scoda/sequences/relative_sequence.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/sequences/sequence.py` & `scoda-2.1b6/scoda/sequences/sequence.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/settings/settings.py` & `scoda-2.1b6/scoda/settings/settings.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b5/scoda/tokenisation/base_tokenisation.py` & `scoda-2.1b6/scoda/tokenisation/base_tokenisation.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 from scoda.exceptions.tokenisation_exception import TokenisationException
 from scoda.sequences.sequence import Sequence
 from scoda.settings.settings import PPQN
 
 
 class BaseTokeniser(ABC):
 
-    def __init__(self, running_time_sig: bool) -> None:
+    TOKEN_PAD = 0
+    TOKEN_START = 1
+    TOKEN_STOP = 2
+    TOKEN_SEPARATOR = 3
+
+    def __init__(self) -> None:
         super().__init__()
 
         self.flags = dict()
-        self.flags[TokenisationFlags.RUNNING_TIME_SIG] = running_time_sig
 
         self.cur_time = None
         self.cur_time_target = None
         self.cur_rest_buffer = None
 
         self.prv_type = None
         self.prv_note = None
@@ -39,69 +43,72 @@
 
     def reset_previous(self) -> None:
         self.prv_type = None
         self.prv_note = None
         self.prv_value = -1
         self.prv_numerator = -1
 
-    def _general_tokenise_flush_time_buffer(self, time: int, value_shift: int) -> list[int]:
+    def _general_tokenise_flush_time_buffer(self, time: int, index_time_def: int) -> list[int]:
         tokens = []
 
         while time > self.set_max_rest_value:
-            tokens.append(int(self.set_max_rest_value + value_shift))
+            tokens.append(int(self.set_max_rest_value + index_time_def - 1))
             time -= self.set_max_rest_value
 
         if time > 0:
-            tokens.append(int(time + value_shift))
+            tokens.append(int(time + index_time_def - 1))
 
         return tokens
 
-    def _notelike_tokenise_flush_rest_buffer(self, apply_target: bool, wait_token: int, value_shift: int) -> list[int]:
+    def _notelike_tokenise_flush_rest_buffer(self, apply_target: bool, wait_token: int, index_time_def: int) -> list[
+        int]:
         tokens = []
 
         # Insert rests of length up to `set_max_rest_value`
         while self.cur_rest_buffer > self.set_max_rest_value:
-            if not (self.prv_value == self.set_max_rest_value and self.flags.get(TokenisationFlags.RUNNING_VALUE, False)):
-                tokens.append(int(self.set_max_rest_value + value_shift))
+            if not (self.prv_value == self.set_max_rest_value and self.flags.get(TokenisationFlags.RUNNING_VALUE,
+                                                                                 False)):
+                tokens.append(int(self.set_max_rest_value + index_time_def - 1))
                 self.prv_value = self.set_max_rest_value
 
             tokens.append(int(wait_token))
             self.cur_time += self.set_max_rest_value
             self.cur_rest_buffer -= self.set_max_rest_value
 
         # Insert rests smaller than `set_max_rest_value`
         if self.cur_rest_buffer > 0:
             if not (self.prv_value == self.cur_rest_buffer and self.flags.get(TokenisationFlags.RUNNING_VALUE, False)):
-                tokens.append(int(self.cur_rest_buffer + value_shift))
+                tokens.append(int(self.cur_rest_buffer + index_time_def - 1))
                 self.prv_value = self.cur_rest_buffer
             tokens.append(int(wait_token))
 
         self.cur_time += self.cur_rest_buffer
         self.cur_rest_buffer = 0
 
         # If there are open notes, extend the sequence to the minimum needed time target
         if apply_target and self.cur_time_target > self.cur_time:
             self.cur_rest_buffer += self.cur_time_target - self.cur_time
             tokens.extend(
                 self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=wait_token,
-                                                          value_shift=value_shift))
+                                                          index_time_def=index_time_def))
 
         return tokens
 
     def _gridlike_tokenise_flush_grid_buffer(self, min_grid_size: int, wait_token: int) -> list[int]:
         tokens = []
 
         while self.cur_rest_buffer > 0:
             tokens.append(wait_token)
             self.cur_rest_buffer -= min_grid_size
 
         return tokens
 
     @abstractmethod
-    def tokenise(self, sequence: Sequence, insert_border_tokens: bool = False) -> list[int]:
+    def tokenise(self, sequence: Sequence, insert_trailing_separator_token: bool = True,
+                 insert_border_tokens: bool = False) -> list[int]:
         pass
 
     @staticmethod
     @abstractmethod
     def detokenise(tokens: list[int]) -> Sequence:
         pass
```

### Comparing `scoda-2.1b5/scoda/tokenisation/gridlike_tokenisation.py` & `scoda-2.1b6/scoda/tokenisation/gridlike_tokenisation.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 from scoda.enumerations.tokenisation_flags import TokenisationFlags
 from scoda.exceptions.tokenisation_exception import TokenisationException
 from scoda.sequences.sequence import Sequence
 from scoda.tokenisation.base_tokenisation import BaseTokeniser
 
 
 class BaseGridlikeTokeniser(BaseTokeniser, ABC):
+    TOKEN_SEPARATOR = None
 
     def __init__(self, running_time_sig: bool) -> None:
-        super().__init__(running_time_sig)
+        super().__init__()
+
+        self.flags[TokenisationFlags.RUNNING_TIME_SIG] = running_time_sig
 
 
 class GridlikeTokeniser(BaseGridlikeTokeniser):
     """Tokeniser that uses grid-like temporal representation. Note that input sequences are expected to represent bars,
     as the grid size definition is redone for each input sequence.
 
     [        0] ... pad
@@ -28,20 +31,20 @@
     [116 - 203] ... note off
     [204 - 218] ... time signature numerator in eights from 2/8 to 16/8
     """
 
     def __init__(self, running_time_sig: bool) -> None:
         super().__init__(running_time_sig)
 
-    def tokenise(self, bar_seq: Sequence, apply_buffer: bool = True, insert_border_tokens: bool = False) -> list[int]:
+    def tokenise(self, bar_sequence: Sequence, apply_buffer: bool = True) -> list[int]:
         tokens = []
         min_grid_size = self.set_max_rest_value
 
         # First pass to get minimum grid size
-        for message in bar_seq.rel.messages:
+        for message in bar_sequence.rel.messages:
             msg_type = message.message_type
 
             if msg_type == MessageType.WAIT:
                 self.cur_rest_buffer += message.time
             elif msg_type in [MessageType.NOTE_ON, MessageType.NOTE_OFF, MessageType.TIME_SIGNATURE]:
                 if self.cur_rest_buffer > 0:
                     min_grid_size = math.gcd(int(min_grid_size), int(self.cur_rest_buffer))
@@ -54,15 +57,15 @@
 
         # Limit grid size
         min_grid_size = min(min_grid_size, self.set_max_rest_value)
 
         tokens.append(min_grid_size + 3)
 
         # Second pass to generate tokens
-        for message in bar_seq.rel.messages:
+        for message in bar_sequence.rel.messages:
             msg_type = message.message_type
 
             if msg_type == MessageType.WAIT:
                 self.cur_rest_buffer += message.time
 
                 self.prv_type = MessageType.WAIT
             elif msg_type == MessageType.NOTE_ON:
@@ -97,18 +100,14 @@
 
                 self.prv_type = MessageType.TIME_SIGNATURE
                 self.prv_numerator = numerator
 
         if apply_buffer and self.cur_rest_buffer > 0:
             tokens.extend(self._gridlike_tokenise_flush_grid_buffer(min_grid_size=min_grid_size, wait_token=3))
 
-        if insert_border_tokens:
-            tokens.insert(0, 1)
-            tokens.append(2)
-
         return tokens
 
     @staticmethod
     def detokenise(tokens: list[int]) -> Sequence:
         seq = Sequence()
         prv_type = None
         min_grid_size = math.nan
@@ -139,60 +138,11 @@
 
                 prv_type = MessageType.NOTE_OFF
             elif 204 <= token <= 218:
                 seq.rel.add_message(
                     Message(message_type=MessageType.TIME_SIGNATURE, numerator=token - 204 + 2, denominator=8))
 
                 prv_type = MessageType.TIME_SIGNATURE
-
-        return seq
-
-    @staticmethod
-    def get_info_notes(tokens: list[int], invalid_value: int = -1) -> list[int]:
-        info = []
-
-        for token in tokens:
-            if not 28 <= token <= 115:
-                info.append(invalid_value)
             else:
-                info.append(token - 28 + 21)
+                raise TokenisationException(f"Encountered invalid token during detokenisation: {token}")
 
-        return info
-
-    @staticmethod
-    def get_info_circle_of_fifths(tokens: list[int], invalid_value: int = -1) -> list[int]:
-        info = []
-
-        for token in tokens:
-            if not 28 <= token <= 115:
-                info.append(invalid_value)
-            else:
-                info.append((token - 28 + 21) % 12)
-
-        return info
-
-    @staticmethod
-    def get_info_elapsed_ticks(tokens: list[int]) -> list[int]:
-        info = []
-        cur_time = 0
-        prv_type = None
-        min_grid_size = math.nan
-
-        for token in tokens:
-            info.append(cur_time)
-
-            if token == 3:
-                if math.isnan(min_grid_size):
-                    raise TokenisationException(f"Grid size not initialised")
-
-                cur_time += min_grid_size
-                prv_type = MessageType.INTERNAL
-            elif 4 <= token <= 27:
-                if prv_type == MessageType.WAIT:
-                    raise TokenisationException(f"Illegal consecutive grid size definition")
-
-                min_grid_size = token - 3
-                prv_type = MessageType.WAIT
-            else:
-                prv_type = "general_message"
-
-        return info
+        return seq
```

### Comparing `scoda-2.1b5/scoda/tokenisation/notelike_tokenisation.py` & `scoda-2.1b6/scoda/tokenisation/notelike_tokenisation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import math
-from abc import ABC
+from abc import ABC, abstractmethod
 from typing import Any
 
 from scoda.elements.message import Message
 from scoda.enumerations.message_type import MessageType
 from scoda.enumerations.tokenisation_flags import TokenisationFlags
 from scoda.exceptions.tokenisation_exception import TokenisationException
 from scoda.misc.music_theory import CircleOfFifths
@@ -11,17 +11,93 @@
 from scoda.settings.settings import PPQN
 from scoda.tokenisation.base_tokenisation import BaseTokeniser
 
 
 class BaseNotelikeTokeniser(BaseTokeniser, ABC):
 
     def __init__(self, running_value: bool, running_time_sig: bool) -> None:
-        super().__init__(running_time_sig)
+        super().__init__()
 
         self.flags[TokenisationFlags.RUNNING_VALUE] = running_value
+        self.flags[TokenisationFlags.RUNNING_TIME_SIG] = running_time_sig
+
+
+class BaseLargeDictionaryNotelikeTokeniser(BaseNotelikeTokeniser, ABC):
+    SUPPORTED_VALUES = [2, 3, 4, 6, 8, 9, 12, 16, 18, 24, 32, 36, 48, 64, 72, 96]
+    NOTE_SECTION_SIZE = None
+
+    def __init__(self, running_time_sig: bool) -> None:
+        super().__init__(False, running_time_sig)
+
+    def tokenise(self, sequence: Sequence, apply_buffer: bool = True, reset_time: bool = True) -> list[int]:
+        tokens = []
+        event_pairings = sequence.abs.get_message_time_pairings(
+            [MessageType.NOTE_ON, MessageType.NOTE_OFF, MessageType.TIME_SIGNATURE, MessageType.INTERNAL])
+
+        for event_pairing in event_pairings:
+            msg_type = event_pairing[0].message_type
+            msg_time = event_pairing[0].time
+
+            if msg_type == MessageType.NOTE_ON:
+                msg_note = event_pairing[0].note
+                msg_value = event_pairing[1].time - msg_time
+
+                if not (21 <= msg_note <= 108):
+                    raise TokenisationException(f"Invalid note: {msg_note}")
+                if msg_value not in LargeDictionaryNotelikeTokeniser.SUPPORTED_VALUES:
+                    raise TokenisationException(f"Invalid note value: {msg_value}")
+
+                # Check if message occurs at current time, if not place rest messages
+                if not self.cur_time == msg_time:
+                    self.cur_rest_buffer += msg_time - self.cur_time
+                    tokens.extend(
+                        self._general_tokenise_flush_time_buffer(time=self.cur_rest_buffer, index_time_def=4))
+                    self.cur_time += self.cur_rest_buffer
+                    self.cur_rest_buffer = 0
+
+                # Callback
+                self._tokenise_note(tokens, msg_note, msg_value)
+
+                self.cur_time_target = max(self.cur_time_target, self.cur_time + msg_value)
+                self.prv_note = msg_note
+            elif msg_type == MessageType.TIME_SIGNATURE:
+                msg_numerator = event_pairing[0].numerator
+                msg_denominator = event_pairing[0].denominator
+
+                numerator = self._time_signature_to_eights(msg_numerator, msg_denominator)
+
+                # Check if time signature has to be defined
+                if not (self.prv_numerator == numerator and self.flags.get(TokenisationFlags.RUNNING_TIME_SIG, False)):
+                    self.cur_rest_buffer += msg_time - self.cur_time
+                    tokens.extend(
+                        self._general_tokenise_flush_time_buffer(time=self.cur_rest_buffer, index_time_def=4))
+                    self.cur_time += self.cur_rest_buffer
+                    self.cur_rest_buffer = 0
+
+                    tokens.append(numerator - 2 + len(self.SUPPORTED_VALUES) * self.NOTE_SECTION_SIZE + 4 + 24)
+
+                self.prv_numerator = numerator
+            elif msg_type == MessageType.INTERNAL:
+                self.cur_rest_buffer += msg_time - self.cur_time
+
+        if apply_buffer:
+            self.cur_rest_buffer = max(self.cur_time_target - self.cur_time, self.cur_rest_buffer)
+            tokens.extend(
+                self._general_tokenise_flush_time_buffer(time=self.cur_rest_buffer, index_time_def=4))
+            self.cur_time += self.cur_rest_buffer
+            self.cur_rest_buffer = 0
+
+        if reset_time:
+            self.reset_time()
+
+        return tokens
+
+    @abstractmethod
+    def _tokenise_note(self, tokens: list[int], msg_note: int, msg_value: int) -> None:
+        pass
 
 
 class StandardNotelikeTokeniser(BaseNotelikeTokeniser):
     """Tokeniser that uses note-like temporal representation.
 
     [        0] ... pad
     [        1] ... start
@@ -35,16 +111,15 @@
     """
 
     def __init__(self, running_value: bool, running_pitch: bool, running_time_sig: bool) -> None:
         super().__init__(running_value, running_time_sig)
 
         self.flags[TokenisationFlags.RUNNING_PITCH] = running_pitch
 
-    def tokenise(self, sequence: Sequence, apply_buffer: bool = True, reset_time: bool = True,
-                 insert_trailing_separator_token: bool = True, insert_border_tokens: bool = False) -> list[int]:
+    def tokenise(self, sequence: Sequence, apply_buffer: bool = True, reset_time: bool = True) -> list[int]:
         tokens = []
         event_pairings = sequence.abs.get_message_time_pairings(
             [MessageType.NOTE_ON, MessageType.NOTE_OFF, MessageType.TIME_SIGNATURE, MessageType.INTERNAL])
 
         for event_pairing in event_pairings:
             msg_type = event_pairing[0].message_type
             msg_time = event_pairing[0].time
@@ -56,19 +131,19 @@
                 if not (21 <= msg_note <= 108):
                     raise TokenisationException(f"Invalid note: {msg_note}")
 
                 # Check if message occurs at current time, if not place rest messages
                 if not self.cur_time == msg_time:
                     self.cur_rest_buffer += msg_time - self.cur_time
                     tokens.extend(
-                        self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=4, value_shift=4))
+                        self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=4, index_time_def=5))
 
                 # Check if value of note has to be defined
                 if not (self.prv_value == msg_value and self.flags.get(TokenisationFlags.RUNNING_VALUE, False)):
-                    tokens.extend(self._general_tokenise_flush_time_buffer(msg_value, value_shift=4))
+                    tokens.extend(self._general_tokenise_flush_time_buffer(msg_value, index_time_def=5))
 
                 # Check if pitch of note has to be defined
                 if not (self.prv_note == msg_note and self.flags.get(TokenisationFlags.RUNNING_PITCH, False)):
                     tokens.append(msg_note - 21 + 29)
                 else:
                     tokens.append(132)
 
@@ -82,37 +157,30 @@
 
                 numerator = self._time_signature_to_eights(msg_numerator, msg_denominator)
 
                 # Check if time signature has to be defined
                 if not (self.prv_numerator == numerator and self.flags.get(TokenisationFlags.RUNNING_TIME_SIG, False)):
                     self.cur_rest_buffer += msg_time - self.cur_time
                     tokens.extend(
-                        self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=4, value_shift=4))
+                        self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=4, index_time_def=5))
                     tokens.append(numerator - 2 + 117)
 
                 self.prv_type = MessageType.TIME_SIGNATURE
                 self.prv_numerator = numerator
             elif msg_type == MessageType.INTERNAL:
                 self.cur_rest_buffer += msg_time - self.cur_time
                 self.prv_type = MessageType.INTERNAL
 
         if apply_buffer:
             tokens.extend(
-                self._notelike_tokenise_flush_rest_buffer(apply_target=True, wait_token=4, value_shift=4))
+                self._notelike_tokenise_flush_rest_buffer(apply_target=True, wait_token=4, index_time_def=5))
 
         if reset_time:
             self.reset_time()
 
-        if insert_trailing_separator_token:
-            tokens.append(3)
-
-        if insert_border_tokens:
-            tokens.insert(0, 1)
-            tokens.append(2)
-
         return tokens
 
     @staticmethod
     def detokenise(tokens: list[int]) -> Sequence:
         seq = Sequence()
         cur_time = 0
         prv_type = None
@@ -278,15 +346,15 @@
                 prv_value_volatile = 0
             for v_d in range(1, 24 + 1):
                 if bar_capacity - bar_time >= prv_value_volatile + v_d:
                     valid_tokens.append(v_d + 4)
         # [ 29 - 116] ... note
         if h_started_not_stopped and h_bar_valid_time_signature and h_has_prv_value:
             for n in range(21, 108 + 1):
-                if prv_note not in pnt_concurrent_notes:
+                if n not in pnt_concurrent_notes:
                     valid_tokens.append(n - 21 + 29)
         # [117 - 131] ... time signature numerator in eights from 2/8 to 16/8
         if h_started_not_stopped and not h_bar_contains_time_signature and bar_time == 0:
             for t in range(117, 131 + 1):
                 valid_tokens.append(t)
         # [      132] ... note with previous pitch (running pitch only)
         if h_started_not_stopped and h_bar_valid_time_signature and running_pitch and h_has_prv_value and h_note_not_open(
@@ -306,14 +374,84 @@
                  "prv_type": prv_type,
                  "prv_note": prv_note,
                  "prv_value": prv_value}
 
         return valid_tokens, state
 
 
+class LargeDictionaryNotelikeTokeniser(BaseLargeDictionaryNotelikeTokeniser):
+    """Tokeniser that uses note-like temporal representation.
+
+    [        0] ... pad
+    [        1] ... start
+    [        2] ... stop
+    [        3] ... bar separator
+    [  4 -  27] ... wait
+    [ 28 - 115] ... notes with duration of 2 ticks
+    [116 - 203] ... notes with duration of 3 ticks
+    [204 - 291] ... notes with duration of 4 ticks
+    [292 - 379] ... notes with duration of 6 ticks
+    [380 - 467] ... notes with duration of 8 ticks
+    [468 - 555] ... notes with duration of 9 ticks
+    [556 - 643] ... notes with duration of 12 ticks
+    [644 - 731] ... notes with duration of 16 ticks
+    [732 - 819] ... notes with duration of 18 ticks
+    [820 - 907] ... notes with duration of 24 ticks
+    [908 - 995] ... notes with duration of 32 ticks
+    [996 -1083] ... notes with duration of 36 ticks
+    [1084-1171] ... notes with duration of 48 ticks
+    [1172-1259] ... notes with duration of 64 ticks
+    [1260-1347] ... notes with duration of 72 ticks
+    [1348-1435] ... notes with duration of 96 ticks
+    [1436-1450] ... time signature numerator in eights from 2/8 to 16/8
+    """
+
+    def __init__(self, running_time_sig: bool) -> None:
+        super().__init__(running_time_sig)
+
+    NOTE_SECTION_SIZE = 88
+
+    def _tokenise_note(self, tokens: list[int], msg_note: int, msg_value: int) -> None:
+        # Add token representing pitch and value
+        tokens.append(
+            msg_note - 21 + 28 + LargeDictionaryNotelikeTokeniser.SUPPORTED_VALUES.index(msg_value) * 88)
+
+    @staticmethod
+    def detokenise(tokens: list[int]) -> Sequence:
+        seq = Sequence()
+        cur_time = 0
+        note_section_size = LargeDictionaryNotelikeTokeniser.NOTE_SECTION_SIZE
+
+        boundary_token_ts = len(LargeDictionaryNotelikeTokeniser.SUPPORTED_VALUES) * note_section_size + 4 + 24
+
+        for token in tokens:
+            if token <= 3:
+                pass
+            elif 4 <= token <= 27:
+                cur_time += token - 3
+            elif 28 <= token <= boundary_token_ts - 1:
+                note_pitch = (token - 28) % note_section_size + 21
+                note_value = LargeDictionaryNotelikeTokeniser.SUPPORTED_VALUES[(token - 28) // note_section_size]
+
+                seq.add_absolute_message(
+                    Message(message_type=MessageType.NOTE_ON, note=note_pitch, time=cur_time))
+                seq.add_absolute_message(
+                    Message(message_type=MessageType.NOTE_OFF, note=note_pitch, time=cur_time + note_value))
+            elif boundary_token_ts <= token <= boundary_token_ts + 14:
+                seq.add_absolute_message(
+                    Message(message_type=MessageType.TIME_SIGNATURE, time=cur_time,
+                            numerator=token - boundary_token_ts + 2,
+                            denominator=8)
+                )
+            else:
+                raise TokenisationException(f"Encountered invalid token during detokenisation: {token}")
+
+        return seq
+
+
 class CoFNotelikeTokeniser(BaseNotelikeTokeniser):
     """Tokeniser that uses note-like temporal representation with circle of fifths distances between notes.
 
     [        0] ... pad
     [        1] ... start
     [        2] ... stop
     [        3] ... bar separator
@@ -335,16 +473,15 @@
         super().reset_previous()
 
         # A4 as base note
         self.prv_note = 69
         self.prv_octave = 4
 
     def tokenise(self, sequence: Sequence, apply_buffer: bool = True, reset_base_note: bool = True,
-                 reset_time: bool = True, insert_trailing_separator_token: bool = True,
-                 insert_border_tokens: bool = False) -> list[int]:
+                 reset_time: bool = True) -> list[int]:
         tokens = []
         event_pairings = sequence.abs.get_message_time_pairings(
             [MessageType.NOTE_ON, MessageType.NOTE_OFF, MessageType.TIME_SIGNATURE, MessageType.INTERNAL])
 
         for event_pairing in event_pairings:
             msg_type = event_pairing[0].message_type
             msg_time = event_pairing[0].time
@@ -356,30 +493,32 @@
                 if not (21 <= msg_note <= 108):
                     raise TokenisationException(f"Invalid note: {msg_note}")
 
                 # Check if message occurs at current time, if not place rest messages
                 if not self.cur_time == msg_time:
                     self.cur_rest_buffer += msg_time - self.cur_time
                     tokens.extend(
-                        self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=4, value_shift=4))
+                        self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=4, index_time_def=5))
 
                 # Check if value of note has to be defined
                 if not (self.prv_value == msg_value and self.flags.get(TokenisationFlags.RUNNING_VALUE, False)):
-                    tokens.extend(self._general_tokenise_flush_time_buffer(msg_value, value_shift=4))
+                    tokens.extend(self._general_tokenise_flush_time_buffer(msg_value, index_time_def=5))
 
-                # Check if octave of note hast to be defined
+                # Get distances
                 octave_tgt = msg_note // 12 - 1
-                if not (self.prv_octave == octave_tgt and self.flags.get(TokenisationFlags.RUNNING_OCTAVE, False)):
-                    octave_src = self.prv_note // 12 - 1
-                    octave_shift = octave_tgt - octave_src
-                    assert -8 <= octave_shift <= 8
-                    tokens.append((octave_shift + 8) + 29)
+                octave_src = self.prv_note // 12 - 1
+                octave_shift = octave_tgt - octave_src
+                assert -8 <= octave_shift <= 8
 
                 cof_dist = CircleOfFifths.get_distance(self.prv_note, msg_note)
+                assert -5 <= cof_dist <= 6
 
+                # Insert octave shift (if necessary) and note distance
+                if not (self.prv_octave == octave_tgt and self.flags.get(TokenisationFlags.RUNNING_OCTAVE, False)):
+                    tokens.append((octave_shift + 8) + 29)
                 tokens.append((cof_dist + 5) + 46)
 
                 self.cur_time_target = max(self.cur_time_target, self.cur_time + msg_value)
                 self.prv_type = MessageType.NOTE_ON
                 self.prv_note = msg_note
                 self.prv_octave = octave_tgt
                 self.prv_value = msg_value
@@ -389,37 +528,30 @@
 
                 numerator = self._time_signature_to_eights(msg_numerator, msg_denominator)
 
                 # Check if time signature has to be defined
                 if not (self.prv_numerator == numerator and self.flags.get(TokenisationFlags.RUNNING_TIME_SIG, False)):
                     self.cur_rest_buffer += msg_time - self.cur_time
                     tokens.extend(
-                        self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=4, value_shift=4))
+                        self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=4, index_time_def=5))
                     tokens.append(numerator - 2 + 58)
 
                 self.prv_type = MessageType.TIME_SIGNATURE
                 self.prv_numerator = numerator
             elif msg_type == MessageType.INTERNAL:
                 self.cur_rest_buffer += msg_time - self.cur_time
                 self.prv_type = MessageType.INTERNAL
 
         if apply_buffer:
             tokens.extend(
-                self._notelike_tokenise_flush_rest_buffer(apply_target=True, wait_token=4, value_shift=4))
+                self._notelike_tokenise_flush_rest_buffer(apply_target=True, wait_token=4, index_time_def=5))
 
         if reset_time:
             self.reset_time()
 
-        if insert_trailing_separator_token:
-            tokens.append(3)
-
-        if insert_border_tokens:
-            tokens.insert(0, 1)
-            tokens.append(2)
-
         return tokens
 
     @staticmethod
     def detokenise(tokens: list[int]) -> Sequence:
         seq = Sequence()
         cur_time = 0
         prv_type = None
@@ -441,15 +573,15 @@
                 else:
                     prv_value = token - 4
                 prv_type = MessageType.INTERNAL
             elif 29 <= token <= 45:
                 prv_octave += token - 29 - 8
             elif 46 <= token <= 57:
                 note_base = CircleOfFifths.from_distance(prv_note, (token - 46) - 5)
-                note = note_base + prv_octave * 12 + 12
+                note = note_base + prv_octave * 12 + 12  # Shifts notes to A0
 
                 seq.add_absolute_message(
                     Message(message_type=MessageType.NOTE_ON, note=note, time=cur_time))
                 seq.add_absolute_message(
                     Message(message_type=MessageType.NOTE_OFF, note=note, time=cur_time + prv_value))
                 prv_type = MessageType.NOTE_ON
                 prv_note = note
@@ -460,146 +592,103 @@
                 )
                 prv_type = MessageType.TIME_SIGNATURE
             else:
                 raise TokenisationException(f"Encountered invalid token during detokenisation: {token}")
 
         return seq
 
-    @staticmethod
-    def get_info_notes(tokens: list[int], invalid_value: int = -1) -> list[int]:
-        raise NotImplementedError
-
-    @staticmethod
-    def get_info_circle_of_fifths(tokens: list[int], invalid_value: int = -1) -> list[int]:
-        raise NotImplementedError
-
-    @staticmethod
-    def get_info_elapsed_ticks(tokens: list[int]) -> list[int]:
-        raise NotImplementedError
 
-
-class LargeDictionaryNotelikeTokeniser(BaseNotelikeTokeniser):
-    """Tokeniser that uses note-like temporal representation.
+class LargeDictionaryCoFNotelikeTokeniser(BaseLargeDictionaryNotelikeTokeniser):
+    """Tokeniser that uses note-like temporal representation with circle of fifths distances between notes.
 
     [        0] ... pad
     [        1] ... start
     [        2] ... stop
     [        3] ... bar separator
     [  4 -  27] ... wait
-    [ 28 - 115] ... notes with duration of 2 ticks
-    [116 - 203] ... notes with duration of 3 ticks
-    [204 - 291] ... notes with duration of 4 ticks
-    [292 - 379] ... notes with duration of 6 ticks
-    [380 - 467] ... notes with duration of 8 ticks
-    [468 - 555] ... notes with duration of 9 ticks
-    [556 - 643] ... notes with duration of 12 ticks
-    [644 - 731] ... notes with duration of 16 ticks
-    [732 - 819] ... notes with duration of 18 ticks
-    [820 - 907] ... notes with duration of 24 ticks
-    [908 - 995] ... notes with duration of 32 ticks
-    [996 -1083] ... notes with duration of 36 ticks
-    [1084-1171] ... notes with duration of 48 ticks
-    [1172-1259] ... notes with duration of 64 ticks
-    [1260-1347] ... notes with duration of 72 ticks
-    [1348-1435] ... notes with duration of 96 ticks
-    [1436-1450] ... time signature numerator in eights from 2/8 to 16/8
+    [ 28 - 231] ... notes with duration of 2 ticks
+    [232 - 435] ... notes with duration of 3 ticks
+    [436 - 639] ... notes with duration of 4 ticks
+    [640 - 843] ... notes with duration of 6 ticks
+    [844 -1047] ... notes with duration of 8 ticks
+    [1048-1251] ... notes with duration of 9 ticks
+    [1252-1455] ... notes with duration of 12 ticks
+    [1456-1659] ... notes with duration of 16 ticks
+    [1660-1863] ... notes with duration of 18 ticks
+    [1864-2067] ... notes with duration of 24 ticks
+    [2068-2271] ... notes with duration of 32 ticks
+    [2272-2475] ... notes with duration of 36 ticks
+    [2476-2679] ... notes with duration of 48 ticks
+    [2680-2883] ... notes with duration of 64 ticks
+    [2884-3087] ... notes with duration of 72 ticks
+    [3088-3291] ... notes with duration of 96 ticks
+    [3292-3307] ... time signature numerator in eights from 2/8 to 16/8
     """
 
-    SUPPORTED_VALUES = [2, 3, 4, 6, 8, 9, 12, 16, 18, 24, 32, 36, 48, 64, 72, 96]
-
     def __init__(self, running_time_sig: bool) -> None:
-        super().__init__(False, running_time_sig)
-
-    def tokenise(self, sequence: Sequence, apply_buffer: bool = True, reset_time: bool = True,
-                 insert_border_tokens: bool = False) -> list[int]:
-        tokens = []
-        event_pairings = sequence.abs.get_message_time_pairings(
-            [MessageType.NOTE_ON, MessageType.NOTE_OFF, MessageType.TIME_SIGNATURE, MessageType.INTERNAL])
-
-        for event_pairing in event_pairings:
-            msg_type = event_pairing[0].message_type
-            msg_time = event_pairing[0].time
-
-            if msg_type == MessageType.NOTE_ON:
-                msg_note = event_pairing[0].note
-                msg_value = event_pairing[1].time - msg_time
-
-                if not (21 <= msg_note <= 108):
-                    raise TokenisationException(f"Invalid note: {msg_note}")
-                if msg_value not in LargeDictionaryNotelikeTokeniser.SUPPORTED_VALUES:
-                    raise TokenisationException(f"Invalid note value: {msg_value}")
-
-                # Check if message occurs at current time, if not place rest messages
-                if not self.cur_time == msg_time:
-                    self.cur_rest_buffer += msg_time - self.cur_time
-                    tokens.extend(
-                        self._general_tokenise_flush_time_buffer(time=self.cur_rest_buffer, value_shift=3))
-                    self.cur_time += self.cur_rest_buffer
-                    self.cur_rest_buffer = 0
-
-                # Add token representing pitch and value
-                tokens.append(
-                    msg_note - 21 + 28 + LargeDictionaryNotelikeTokeniser.SUPPORTED_VALUES.index(msg_value) * 88)
-
-                self.cur_time_target = max(self.cur_time_target, self.cur_time + msg_value)
-            elif msg_type == MessageType.TIME_SIGNATURE:
-                msg_numerator = event_pairing[0].numerator
-                msg_denominator = event_pairing[0].denominator
-
-                numerator = self._time_signature_to_eights(msg_numerator, msg_denominator)
+        super().__init__(running_time_sig)
 
-                # Check if time signature has to be defined
-                if not (self.prv_numerator == numerator and self.flags.get(TokenisationFlags.RUNNING_TIME_SIG, False)):
-                    self.cur_rest_buffer += msg_time - self.cur_time
-                    tokens.extend(
-                        self._general_tokenise_flush_time_buffer(time=self.cur_rest_buffer, value_shift=3))
-                    self.cur_time += self.cur_rest_buffer
-                    self.cur_rest_buffer = 0
-                    tokens.append(numerator - 2 + len(LargeDictionaryNotelikeTokeniser.SUPPORTED_VALUES) * 88 + 4 + 24)
+        self.prv_octave = None
 
-                self.prv_numerator = numerator
-            elif msg_type == MessageType.INTERNAL:
-                self.cur_rest_buffer += msg_time - self.cur_time
+    NOTE_SECTION_SIZE = 204
 
-        if apply_buffer:
-            self.cur_rest_buffer = max(self.cur_time_target - self.cur_time, self.cur_rest_buffer)
-            tokens.extend(
-                self._general_tokenise_flush_time_buffer(time=self.cur_rest_buffer, value_shift=3))
-            self.cur_time += self.cur_rest_buffer
-            self.cur_rest_buffer = 0
+    def reset_previous(self) -> None:
+        super().reset_previous()
 
-        if reset_time:
-            self.reset_time()
+        # A4 as base note
+        self.prv_note = 69
+        self.prv_octave = 4
 
-        if insert_border_tokens:
-            tokens.insert(0, 1)
-            tokens.append(2)
+    def _tokenise_note(self, tokens: list[int], msg_note: int, msg_value: int) -> None:
+        # Get distances
+        octave_tgt = msg_note // 12 - 1
+        octave_src = self.prv_note // 12 - 1
+        octave_shift = octave_tgt - octave_src
+        assert -8 <= octave_shift <= 8
+
+        cof_dist = CircleOfFifths.get_distance(self.prv_note, msg_note)
+        assert -5 <= cof_dist <= 6
+
+        token_value = (28 +
+                       (cof_dist + 5) +
+                       ((octave_shift + 8) * 12) +
+                       self.SUPPORTED_VALUES.index(msg_value) * LargeDictionaryCoFNotelikeTokeniser.NOTE_SECTION_SIZE)
 
-        return tokens
+        tokens.append(token_value)
 
     @staticmethod
     def detokenise(tokens: list[int]) -> Sequence:
         seq = Sequence()
         cur_time = 0
+        prv_note = 69  # A4 is base note
+        note_section_size = LargeDictionaryCoFNotelikeTokeniser.NOTE_SECTION_SIZE
 
-        boundary_token_ts = len(LargeDictionaryNotelikeTokeniser.SUPPORTED_VALUES) * 88 + 4 + 24
+        boundary_token_ts = len(
+            LargeDictionaryNotelikeTokeniser.SUPPORTED_VALUES) * note_section_size + 4 + 24
 
         for token in tokens:
-            if token <= 2:
+            if token <= 3:
                 pass
             elif 4 <= token <= 27:
                 cur_time += token - 3
             elif 28 <= token <= boundary_token_ts - 1:
-                note_pitch = (token - 28) % 88 + 21
-                note_value = LargeDictionaryNotelikeTokeniser.SUPPORTED_VALUES[(token - 28) // 88]
+                note_cof_distance = ((token - 28) % note_section_size) % 12 - 5
+                note_octave_shift = ((token - 28) % note_section_size) // 12 - 8
+                note_value = LargeDictionaryNotelikeTokeniser.SUPPORTED_VALUES[(token - 28) // note_section_size]
+
+                octave = prv_note // 12 - 1
+                octave += note_octave_shift
+                note_base = CircleOfFifths.from_distance(prv_note, note_cof_distance)
+                note = note_base + octave * 12 + 12  # Shifts notes to A0
 
                 seq.add_absolute_message(
-                    Message(message_type=MessageType.NOTE_ON, note=note_pitch, time=cur_time))
+                    Message(message_type=MessageType.NOTE_ON, note=note, time=cur_time))
                 seq.add_absolute_message(
-                    Message(message_type=MessageType.NOTE_OFF, note=note_pitch, time=cur_time + note_value))
+                    Message(message_type=MessageType.NOTE_OFF, note=note, time=cur_time + note_value))
+                prv_note = note
             elif boundary_token_ts <= token <= boundary_token_ts + 14:
                 seq.add_absolute_message(
                     Message(message_type=MessageType.TIME_SIGNATURE, time=cur_time,
                             numerator=token - boundary_token_ts + 2,
                             denominator=8)
                 )
             else:
```

### Comparing `scoda-2.1b5/scoda/tokenisation/transposed_notelike_tokenisation.py` & `scoda-2.1b6/scoda/tokenisation/transposed_notelike_tokenisation.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,17 +9,20 @@
 from scoda.settings.settings import PPQN
 from scoda.tokenisation.base_tokenisation import BaseTokeniser
 
 
 class BaseTransposedNotelikeTokeniser(BaseTokeniser, ABC):
 
     def __init__(self, running_time_sig: bool) -> None:
-        super().__init__(running_time_sig)
+        super().__init__()
+
+        self.flags[TokenisationFlags.RUNNING_TIME_SIG] = running_time_sig
 
 
+# TODO
 class TransposedNotelikeTokeniser(BaseTransposedNotelikeTokeniser):
     """Tokeniser that uses transposed temporal representation with a note-like approach, i.e., all occurrences of a note
     are shown first before any other note is handled. Note that input sequences are expected to represent bars,
     as the transposed representation is done on a per-bar basis.
 
     [        0] ... pad
     [        1] ... start
@@ -33,18 +36,18 @@
     """
 
     def __init__(self, running_value: bool, running_time_sig: bool) -> None:
         super().__init__(running_time_sig)
 
         self.flags[TokenisationFlags.RUNNING_VALUE] = running_value
 
-    def tokenise(self, bar_seq: Sequence, apply_buffer: bool = True, reset_time: bool = True,
+    def tokenise(self, bar_sequence: Sequence, apply_buffer: bool = True, reset_time: bool = True,
                  insert_border_tokens: bool = False) -> list[int]:
         tokens = []
-        event_pairings = bar_seq.abs.get_message_time_pairings(
+        event_pairings = bar_sequence.abs.get_message_time_pairings(
             [MessageType.NOTE_ON, MessageType.NOTE_OFF, MessageType.TIME_SIGNATURE, MessageType.INTERNAL])
 
         event_pairings_by_note = dict()
 
         # Entries consist of (message type, hashable)
         ordered_type_value_pairs = list()
 
@@ -96,51 +99,54 @@
                     if not (21 <= msg_note <= 108):
                         raise TokenisationException(f"Invalid note: {msg_note}")
 
                     # Check if message occurs at current time, if not place rest messages
                     if not self.cur_time == msg_time:
                         self.cur_rest_buffer += msg_time - self.cur_time
                         tokens.extend(
-                            self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=4, value_shift=5))
+                            self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=4,
+                                                                      index_time_def=6))
 
                     # Check if value of note has to be defined
                     if not (self.prv_value == msg_value and self.flags.get(TokenisationFlags.RUNNING_VALUE, False)):
-                        tokens.extend(self._general_tokenise_flush_time_buffer(msg_value, value_shift=5))
+                        tokens.extend(self._general_tokenise_flush_time_buffer(msg_value, index_time_def=6))
 
                     # Play note
                     tokens.append(3)
 
                     self.cur_time_target = max(self.cur_time_target, self.cur_time + msg_value)
                     self.prv_type = MessageType.NOTE_ON
                     self.prv_value = msg_value
                 elif msg_type == MessageType.TIME_SIGNATURE:
                     msg_numerator = event_pairing[0].numerator
                     msg_denominator = event_pairing[0].denominator
 
                     numerator = self._time_signature_to_eights(msg_numerator, msg_denominator)
 
                     # Check if time signature has to be defined
-                    if not (self.prv_numerator == numerator and self.flags.get(TokenisationFlags.RUNNING_TIME_SIG, False)):
+                    if not (self.prv_numerator == numerator and self.flags.get(TokenisationFlags.RUNNING_TIME_SIG,
+                                                                               False)):
                         self.cur_rest_buffer += msg_time - self.cur_time
                         tokens.extend(
-                            self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=4, value_shift=5))
+                            self._notelike_tokenise_flush_rest_buffer(apply_target=False, wait_token=4,
+                                                                      index_time_def=6))
                         tokens.append(numerator - 2 + 118)
 
                     self.prv_type = MessageType.TIME_SIGNATURE
                     self.prv_numerator = numerator
                 elif msg_type == MessageType.INTERNAL:
                     self.cur_rest_buffer += msg_time - self.cur_time
                     self.prv_type = MessageType.INTERNAL
 
             # Reset time to beginning of bar
             self.cur_time = 0
 
         if apply_buffer:
             tokens.extend(
-                self._notelike_tokenise_flush_rest_buffer(apply_target=True, wait_token=4, value_shift=5))
+                self._notelike_tokenise_flush_rest_buffer(apply_target=True, wait_token=4, index_time_def=6))
 
         if reset_time:
             self.reset_time()
 
         # Insert bar border mark
         tokens.append(5)
 
@@ -205,91 +211,7 @@
 
                 prv_type = MessageType.TIME_SIGNATURE
                 prv_numerator = numerator
             else:
                 raise TokenisationException(f"Encountered invalid token during detokenisation: {token}")
 
         return seq
-
-    @staticmethod
-    def get_info_notes(tokens: list[int], invalid_value: int = -1) -> list[int]:
-        info = []
-
-        prv_note = math.nan
-
-        for token in tokens:
-            if token == 3:
-                if math.isnan(prv_note):
-                    raise TokenisationException(f"Note value not initialised")
-
-                info.append(prv_note)
-            elif 30 <= token <= 117:
-                info.append(invalid_value)
-                prv_note = token - 30 + 21
-            else:
-                info.append(invalid_value)
-
-        return info
-
-    @staticmethod
-    def get_info_circle_of_fifths(tokens: list[int], invalid_value: int = -1) -> list[int]:
-        info = []
-
-        prv_note = math.nan
-
-        for token in tokens:
-            if token == 3:
-                if math.isnan(prv_note):
-                    raise TokenisationException(f"Note value not initialised")
-
-                info.append(prv_note % 12)
-            elif 30 <= token <= 117:
-                info.append(invalid_value)
-                prv_note = token - 30 + 21
-            else:
-                info.append(invalid_value)
-
-        return info
-
-    @staticmethod
-    def get_info_elapsed_ticks(tokens: list[int]) -> list[int]:
-        info = []
-
-        time_bar_start = 0
-        cur_time_bar = 0
-
-        prv_type = None
-        prv_value = math.nan
-        prv_numerator = math.nan
-
-        for token in tokens:
-            info.append(time_bar_start + cur_time_bar)
-
-            if token == 4:
-                cur_time_bar += prv_value
-
-                prv_type = MessageType.WAIT
-            elif token == 5:
-                time_bar_start += prv_numerator * PPQN / 2
-                cur_time_bar = 0
-
-                prv_type = "bar_border"
-            elif 6 <= token <= 29:
-                if prv_type == "value_definition":
-                    prv_value += token - 5
-                else:
-                    prv_value = token - 5
-
-                prv_type = "value_definition"
-            elif 30 <= token <= 117:
-                cur_time_bar = 0
-
-                prv_type = "note_definition"
-            elif 118 <= token <= 132:
-                numerator = token - 118 + 2
-
-                prv_type = MessageType.TIME_SIGNATURE
-                prv_numerator = numerator
-            else:
-                prv_type = "general_message"
-
-        return info
```

### Comparing `scoda-2.1b5/scoda.egg-info/PKG-INFO` & `scoda-2.1b6/scoda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda
-Version: 2.1b5
+Version: 2.1b6
 Summary: A MIDI and music data manipulation library
 Author-email: Felix Schön <schoen@kr.tuwien.ac.at>
 License: MIT License
         
         Copyright (c) 2023 Felix Schön
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `scoda-2.1b5/scoda.egg-info/SOURCES.txt` & `scoda-2.1b6/scoda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

