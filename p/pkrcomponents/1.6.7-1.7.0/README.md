# Comparing `tmp/pkrcomponents-1.6.7.tar.gz` & `tmp/pkrcomponents-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.6.7.tar", last modified: Fri May 24 21:44:17 2024, max compression
+gzip compressed data, was "pkrcomponents-1.7.0.tar", last modified: Mon May 27 12:51:51 2024, max compression
```

## Comparing `pkrcomponents-1.6.7.tar` & `pkrcomponents-1.7.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:44:17.923889 pkrcomponents-1.6.7/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:44:17.408491 pkrcomponents-1.6.7/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.6.7/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.6.7/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-1.6.7/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-24 21:44:17.923889 pkrcomponents-1.6.7/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-1.6.7/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.6.7/README.rst
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1040 2024-05-24 21:42:15.000000 pkrcomponents-1.6.7/coverage.txt
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:44:17.704985 pkrcomponents-1.6.7/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.6.7/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.6.7/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1593 2024-05-24 00:57:29.000000 pkrcomponents-1.6.7/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-1.6.7/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.6.7/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.6.7/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.6.7/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.6.7/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.6.7/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.6.7/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.6.7/pkrcomponents/lookup_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:44:17.736442 pkrcomponents-1.6.7/pkrcomponents/models/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:44:17.799880 pkrcomponents-1.6.7/pkrcomponents/models/actions/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.6.7/pkrcomponents/models/actions/move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.6.7/pkrcomponents/models/actions/sequence.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.6.7/pkrcomponents/models/actions/street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.6.7/pkrcomponents/models/amount.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:44:17.885930 pkrcomponents-1.6.7/pkrcomponents/models/cards/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.6.7/pkrcomponents/models/cards/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.6.7/pkrcomponents/models/cards/rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.6.7/pkrcomponents/models/cards/suit.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:44:17.892243 pkrcomponents-1.6.7/pkrcomponents/models/pots/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.6.7/pkrcomponents/models/pots/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.6.7/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      999 2024-05-15 15:52:00.000000 pkrcomponents-1.6.7/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15964 2024-05-24 00:19:33.000000 pkrcomponents-1.6.7/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    12206 2024-05-24 00:59:50.000000 pkrcomponents-1.6.7/pkrcomponents/table_player.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    10341 2024-05-24 21:37:58.000000 pkrcomponents-1.6.7/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-24 21:44:17.908858 pkrcomponents-1.6.7/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      797 2024-05-24 21:44:16.000000 pkrcomponents-1.6.7/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.6.7/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-24 21:44:17.923889 pkrcomponents-1.6.7/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1385 2024-05-24 19:24:47.000000 pkrcomponents-1.6.7/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.924429 pkrcomponents-1.7.0/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.270443 pkrcomponents-1.7.0/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.7.0/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.7.0/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-1.7.0/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-27 12:51:51.916894 pkrcomponents-1.7.0/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-1.7.0/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/README.rst
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1040 2024-05-27 12:48:33.000000 pkrcomponents-1.7.0/coverage.txt
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.526616 pkrcomponents-1.7.0/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1593 2024-05-24 00:57:29.000000 pkrcomponents-1.7.0/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-1.7.0/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.7.0/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.7.0/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.7.0/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/pkrcomponents/lookup_table.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.574880 pkrcomponents-1.7.0/pkrcomponents/models/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.684695 pkrcomponents-1.7.0/pkrcomponents/models/actions/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.7.0/pkrcomponents/models/actions/move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.7.0/pkrcomponents/models/actions/sequence.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.7.0/pkrcomponents/models/actions/street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.7.0/pkrcomponents/models/amount.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.831285 pkrcomponents-1.7.0/pkrcomponents/models/cards/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.7.0/pkrcomponents/models/cards/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.7.0/pkrcomponents/models/cards/rank.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.7.0/pkrcomponents/models/cards/suit.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.874130 pkrcomponents-1.7.0/pkrcomponents/models/pots/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.7.0/pkrcomponents/models/pots/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.7.0/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      999 2024-05-15 15:52:00.000000 pkrcomponents-1.7.0/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    16718 2024-05-27 11:48:40.000000 pkrcomponents-1.7.0/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    12484 2024-05-27 09:29:53.000000 pkrcomponents-1.7.0/pkrcomponents/table_player.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    10639 2024-05-25 01:06:35.000000 pkrcomponents-1.7.0/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.902431 pkrcomponents-1.7.0/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      797 2024-05-27 12:51:49.000000 pkrcomponents-1.7.0/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-27 12:51:51.925767 pkrcomponents-1.7.0/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1385 2024-05-24 19:24:47.000000 pkrcomponents-1.7.0/setup.py
```

### Comparing `pkrcomponents-1.6.7/LICENSE.txt` & `pkrcomponents-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/MANIFEST.in` & `pkrcomponents-1.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/PKG-INFO` & `pkrcomponents-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 1.6.7
+Version: 1.7.0
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
```

### Comparing `pkrcomponents-1.6.7/coverage.txt` & `pkrcomponents-1.7.0/coverage.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Name                            Stmts   Miss  Cover
 ---------------------------------------------------
 pkrcomponents/__init__.py           0      0   100%
 pkrcomponents/_common.py           48      0   100%
 pkrcomponents/action.py            32      0   100%
 pkrcomponents/bitcard.py           68      0   100%
-pkrcomponents/board.py             81      1    99%
-pkrcomponents/card.py             112      2    98%
+pkrcomponents/board.py             81      0   100%
+pkrcomponents/card.py             112      1    99%
 pkrcomponents/constants.py         71      0   100%
 pkrcomponents/evaluator.py         28      0   100%
 pkrcomponents/hand.py             226      0   100%
 pkrcomponents/listings.py          16      0   100%
 pkrcomponents/lookup_table.py     112      0   100%
-pkrcomponents/players.py           96      7    93%
-pkrcomponents/pot.py               25      2    92%
-pkrcomponents/table.py            317     49    85%
-pkrcomponents/table_player.py     248     30    88%
-pkrcomponents/tournament.py       256      1    99%
+pkrcomponents/players.py           96      0   100%
+pkrcomponents/pot.py               25      0   100%
+pkrcomponents/table.py            326      8    98%
+pkrcomponents/table_player.py     253      4    98%
+pkrcomponents/tournament.py       258      0   100%
 ---------------------------------------------------
-TOTAL                            1736     92    95%
+TOTAL                            1752     13    99%
```

### Comparing `pkrcomponents-1.6.7/pkrcomponents/_common.py` & `pkrcomponents-1.7.0/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/action.py` & `pkrcomponents-1.7.0/pkrcomponents/action.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/bitcard.py` & `pkrcomponents-1.7.0/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/board.py` & `pkrcomponents-1.7.0/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/card.py` & `pkrcomponents-1.7.0/pkrcomponents/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/constants.py` & `pkrcomponents-1.7.0/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/evaluator.py` & `pkrcomponents-1.7.0/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/hand.py` & `pkrcomponents-1.7.0/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/listings.py` & `pkrcomponents-1.7.0/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/lookup_table.py` & `pkrcomponents-1.7.0/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/models/actions/move.py` & `pkrcomponents-1.7.0/pkrcomponents/models/actions/move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/models/actions/street.py` & `pkrcomponents-1.7.0/pkrcomponents/models/actions/street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/models/amount.py` & `pkrcomponents-1.7.0/pkrcomponents/models/amount.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/models/cards/card.py` & `pkrcomponents-1.7.0/pkrcomponents/models/cards/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/models/cards/rank.py` & `pkrcomponents-1.7.0/pkrcomponents/models/cards/rank.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/models/cards/suit.py` & `pkrcomponents-1.7.0/pkrcomponents/models/cards/suit.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/models/pots/pot.py` & `pkrcomponents-1.7.0/pkrcomponents/models/pots/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/players.py` & `pkrcomponents-1.7.0/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/pot.py` & `pkrcomponents-1.7.0/pkrcomponents/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/pkrcomponents/table.py` & `pkrcomponents-1.7.0/pkrcomponents/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,173 +44,170 @@
         self._is_mtt = False
         self._street = Street.PREFLOP
         self.max_players = max_players
         self._hand_has_started = False
         self._cnt_bets = 0
 
     @property
-    def board(self):
+    def board(self) -> Board:
         """Returns the associated board """
         return self._board
 
     @property
-    def deck(self):
+    def deck(self) -> Deck:
         """Returns the associated deck """
         return self._deck
 
     @property
-    def players(self):
+    def players(self) -> Players:
         """Returns the associated players """
         return self._players
 
     @property
-    def max_players(self):
+    def max_players(self) -> int:
         """Returns the maximum players that can be added on this table"""
         return self._max_players
 
-    @property
-    def is_full(self):
-        """Returns True if the table is full"""
-        return self.players.len == self.max_players
-
-    @property
-    def is_empty(self):
-        """Returns True if the table is empty"""
-        return self.players.len == 0
-
     @max_players.setter
     def max_players(self, max_value):
         """Setter for max players property"""
         if max_value not in range(1, 11):
             raise ValueError("Number of players should be between 1 and 10")
         else:
             self._max_players = max_value
 
     @property
+    def is_full(self) -> bool:
+        """Returns True if the table is full"""
+        return self.players.len == self.max_players
+
+    @property
+    def is_empty(self) -> bool:
+        """Returns True if the table is empty"""
+        return self.players.len == 0
+
+    @property
     def pot(self):
         """Returns the associated pot """
         return self._pot
 
     @property
-    def tournament(self):
+    def tournament(self) -> Tournament or None:
         """Returns the associated tournament """
         return self._tournament
 
     @property
-    def evaluator(self):
+    def evaluator(self) -> Evaluator:
         """Returns the associated evaluator"""
         return self._evaluator
 
     @tournament.setter
     def tournament(self, tournament):
         """Setter for tournament property"""
         self._tournament = tournament
 
     @property
-    def street(self):
+    def street(self) -> Street:
         """Returns table's current street"""
         return self._street
 
     @street.setter
     def street(self, street):
         """Setter for street property"""
         self._street = Street(street)
 
     @property
-    def level(self):
+    def level(self) -> Level:
         """Returns current level"""
         if self._is_mtt:
             return self._tournament.level
         else:
             return self._level
 
     @level.setter
     def level(self, level):
         """Setter for level property"""
         self._level = level
 
     @property
-    def playing_order(self):
+    def playing_order(self) -> list[int]:
         """Returns the list of the indexes of players on the table, with order depending on current street"""
         if self._street == Street.PREFLOP:
             return self.players.preflop_ordered_seats
         else:
             return self.players.postflop_ordered_seats
 
     @property
-    def players_waiting(self):
+    def players_waiting(self) -> list:
         """Returns the list of players on the table that are waiting to play"""
         return [self.players[i] for i in self.playing_order if self.players[i].can_play]
 
     @property
-    def street_ended(self):
+    def street_ended(self) -> bool:
         """Returns True if the street has ended"""
-        # First case: there is no player left in waiting_list
-        # Second case: there is only one player left in waiting_list that can still play and he has nothing to call
         return len(self.players_waiting) == 0 or (
                 self.nb_waiting == 1
                 and self.nb_in_game == 1
                 and self.players_waiting[0].to_call == 0
                 and self.street != Street.SHOWDOWN) or (
                 self.street == Street.SHOWDOWN and len(self.unrevealed_players) == 0
         )
 
-
     @property
-    def players_in_game(self):
+    def players_in_game(self) -> list:
         """Returns the list of players on the table that are still in the game (they can make an action)"""
         return [self.players[i] for i in self.playing_order if self.players[i].in_game]
 
     @property
-    def players_involved(self):
+    def players_involved(self) -> list:
         """Returns the list of players on the table that didn't fold yet"""
         return [self.players[i] for i in self.playing_order if not self.players[i].folded]
 
     @property
-    def hand_ended(self):
+    def hand_ended(self) -> bool:
         """Returns True if the hand has ended"""
         return len(self.players_involved) == 1 or self.street == Street.SHOWDOWN
 
     @property
-    def next_street_ready(self):
+    def next_street_ready(self) -> bool:
         """Returns True if the next street is ready to be played"""
         return self.street_ended and not self.hand_ended
 
     @property
-    def next_hand_ready(self):
+    def next_hand_ready(self) -> bool:
         """Returns True if the next hand is ready to be played"""
         return self.hand_ended and self.street_ended
 
     @property
-    def seats_playing(self):
+    def seats_playing(self) -> list[int]:
         """Returns the list of seats of players waiting to play"""
         return [pl.seat for pl in self.players_waiting]
 
     @property
-    def nb_waiting(self):
+    def nb_waiting(self) -> int:
         """Returns the number of players waiting to play"""
         return len(self.players_waiting)
 
     @property
-    def nb_in_game(self):
+    def nb_in_game(self) -> int:
         """Returns the number of players still in the game"""
         return len(self.players_in_game)
 
     @property
-    def nb_involved(self):
+    def nb_involved(self) -> int:
         """Returns the number of players who didn't fold yet"""
         return len(self.players_involved)
 
     @property
-    def hand_has_started(self):
+    def hand_has_started(self) -> bool:
         """Returns True if the hand has started"""
         return self._hand_has_started
 
     @property
-    def hand_can_start(self):
+    def hand_can_start(self) -> bool:
         """Returns True if the hand can start"""
         return self.players.len >= 2 and not self.hand_has_started
 
     def start_hand(self):
         """Starts a new hand"""
         self._hand_has_started = True
         self.street = Street.PREFLOP
@@ -256,24 +253,24 @@
 
     def river(self, card=None):
         """Draw a river and steps to this new street"""
         self.draw_river(card)
         self.street = "river"
         self.street_reset()
 
+    def advance_to_showdown(self):
+        """Advance to showdown"""
+        self.street = Street.SHOWDOWN
+        self.street_reset()
+
     def add_tournament(self, tournament):
         """Associates table with a tournament"""
         self.tournament = tournament
         self._is_mtt = True
 
-    def change_bb_seat(self, seat: int):
-        """Change the big blind seat and redistribute positions"""
-        self.players.bb = seat
-        self.players.distribute_positions()
-
     def add_player(self, player):
         """
         Add a player to the table
         """
         player.sit(self)
         if self.players.len > 1:
             self.players.distribute_positions()
@@ -292,26 +289,29 @@
         """
         Set a player as the hero
         """
         for p in self.players:
             p.is_hero = False
         player.is_hero = True
 
-    def set_bb_seat(self, player):
+    def set_bb_seat(self, player_seat: int):
         """
-        Set the seat of the big blind
+        Set the seat of the big blind player and redistribute positions
         """
-        seat = player.seat
-        self.players.bb = seat
+        self.players.bb = player_seat
         if self.players.len > 1:
             self.players.distribute_positions()
 
-    def set_max_players(self, max_players):
+    def advance_bb_seat(self):
+        """Advances the Big Blind seat"""
+        self.players.advance_bb_seat()
+
+    def set_max_players(self, max_players: int):
         """
-        Set the maximum number of players
+        Set the maximum number of players on the table
         """
         self.max_players = max_players
         if self.players.len > 1:
             self.players.distribute_positions()
 
     def post_antes(self):
         """Preflop Ante posting for players on the table"""
@@ -358,15 +358,15 @@
     def min_bet(self):
         """Returns table current minimum bet a player can make"""
         if not hasattr(self, "_min_bet"):
             self._min_bet = self.level.bb*2
         return self._min_bet
 
     @min_bet.setter
-    def min_bet(self, value):
+    def min_bet(self, value: float):
         """Setter for min bet property"""
         if value > self.min_bet:
             self._min_bet = value
 
     @property
     def min_bet_bb(self):
         """Returns the minimum bet in big blinds"""
@@ -376,15 +376,29 @@
     def pot_value(self):
         """Returns the pot's value"""
         return self.pot.value
 
     @property
     def pot_value_bb(self):
         """Returns the pot's value in big blinds"""
-        return self.pot.value/self.level.bb
+        return self.pot_value/self.level.bb
+
+    @property
+    def average_stack(self):
+        """Returns the average stack of players on the table"""
+        return sum(pl.init_stack for pl in self.players) / self.players.len
+
+    @property
+    def average_stack_bb(self):
+        """Returns the average stack in big blinds"""
+        return round(self.average_stack/self.level.bb, 2)
+
+    def estimated_players_remaining(self):
+        """Returns the estimated number of players remaining in the tournament"""
+        return self.tournament.estimated_players_remaining(average_stack=self.average_stack)
 
     def advance_seat_playing(self):
         """Advances seat playing to next available player"""
         player = self.current_player
         while not player.can_play and self.nb_waiting > 0:
             idx = self.playing_order.index(player.seat) + 1
             try:
@@ -450,30 +464,30 @@
         scores = [score for score in self.winners.keys()]
         scores.sort()
         for score in scores:
             players = self.winners[score]
             self.split_pot(players)
 
     @property
-    def cnt_bets(self):
+    def cnt_bets(self) -> int:
         """Returns the number of bets made on the table"""
         return self._cnt_bets
 
     @cnt_bets.setter
     def cnt_bets(self, value):
         """Setter for cnt bets property"""
         self._cnt_bets = value
 
     @property
-    def preflop_bet_factors(self):
+    def preflop_bet_factors(self) -> list:
         """Returns the preflop bet factors"""
         return self._preflop_bet_factors
 
     @property
-    def postflop_bet_factors(self):
+    def postflop_bet_factors(self) -> list:
         """Returns the postflop bet factors"""
         return self._postflop_bet_factors
 
     def hand_reset(self):
         """
         Reset the hand
         """
@@ -484,9 +498,7 @@
         self.players.hand_reset()
         self._hand_has_started = False
 
     def advance_to_next_hand(self):
         """Advance to the next hand"""
         self.hand_reset()
         self.players.advance_bb_seat()
-
-
```

### Comparing `pkrcomponents-1.6.7/pkrcomponents/table_player.py` & `pkrcomponents-1.7.0/pkrcomponents/table_player.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,44 +84,50 @@
 
     @property
     def stack_to_pot_ratio(self):
         """Player's stack to pot ratio"""
         return float("inf") if self.table.pot.value == 0 else self.stack/self.table.pot.value
 
     @property
-    def m_factor(self):
+    def m_factor(self) -> float:
         """Player's M factor"""
-        return self.stack/self.table.cost_per_round
+        return round(self.stack/self.table.cost_per_round, 2)
 
     @property
-    def m_factor_eff(self):
+    def m_factor_eff(self) -> float:
         """Player's effective M factor"""
-        return self.m_factor * (self.table.players.len / 10)
+        return round(self.m_factor * (self.table.players.len / 10), 2)
 
     @property
-    def folded(self):
+    def folded(self) -> bool:
         """Boolean indicating if player folded"""
         return self._folded
 
     @folded.setter
     def folded(self, folded):
         """Setter for Boolean indicating if player folded"""
         self._folded = folded
 
     @property
-    def init_stack(self):
+    def init_stack(self) -> float:
         """Returns player's stack at the beginning of the hand"""
         return self._init_stack
 
     @init_stack.setter
     def init_stack(self, stack):
         """Setter for player's stack at the beginning of the hand"""
         self._init_stack = max(0.0, float(stack))
         self.stack = self.init_stack
 
+    def reset_init_stack(self):
+        """Reset player's initial stack"""
+        if self.stack == 0:
+            self.table.remove_player(self)
+        self.init_stack = self.stack
+
     @property
     def table(self):
         """Returns associated table"""
         return self._table
 
     @property
     def has_table(self):
@@ -201,14 +207,15 @@
         self.played = False
         self.current_bet = 0
 
     def reset_hand_status(self):
         """Reset hand status"""
         self.reset_street_status()
         self.folded = False
+        self.reset_init_stack()
         self.delete_combo()
 
     @property
     def to_call(self):
         """float indicating the amount to call to continue on the table"""
         return min(self.table.pot.highest_bet-self.current_bet, self.stack)
```

### Comparing `pkrcomponents-1.6.7/pkrcomponents/tournament.py` & `pkrcomponents-1.7.0/pkrcomponents/tournament.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,21 +382,25 @@
     def next_reward(self):
         return self.payouts.closest_payout(self.players_remaining).reward
 
     @property
     def players_to_next_tier(self):
         return self.players_remaining - self.payouts.closest_payout(self.players_remaining).tier
 
+    def estimated_players_remaining(self, average_stack: float) -> int:
+        """
+        Estimate the number of players remaining in the tournament based on the average stack of the remaining players
+        """
+        return min(round(self.total_chips / average_stack), self.total_players)
+
     def __str__(self):
         return f"Name: {self.name}\nId: {self.id}\nBuy-in: {self.buyin}\nMoney: {self.money_type}"
 
     def to_json(self):
         return {
             "level": self.level.to_json(),
             "id": self.id,
             "name": self.name,
             "buy_in": self.buyin.to_json(),
             "is_ko": self.is_ko,
             "money_type": self.money_type
         }
-
-
```

### Comparing `pkrcomponents-1.6.7/pkrcomponents.egg-info/SOURCES.txt` & `pkrcomponents-1.7.0/pkrcomponents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.7/setup.py` & `pkrcomponents-1.7.0/setup.py`

 * *Files identical despite different names*

