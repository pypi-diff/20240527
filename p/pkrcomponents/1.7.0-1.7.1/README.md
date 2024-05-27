# Comparing `tmp/pkrcomponents-1.7.0.tar.gz` & `tmp/pkrcomponents-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.7.0.tar", last modified: Mon May 27 12:51:51 2024, max compression
+gzip compressed data, was "pkrcomponents-1.7.1.tar", last modified: Mon May 27 17:13:29 2024, max compression
```

## Comparing `pkrcomponents-1.7.0.tar` & `pkrcomponents-1.7.1.tar`

### file list

```diff
@@ -1,43 +1,49 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.924429 pkrcomponents-1.7.0/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.270443 pkrcomponents-1.7.0/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.7.0/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.7.0/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-1.7.0/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-27 12:51:51.916894 pkrcomponents-1.7.0/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-1.7.0/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/README.rst
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1040 2024-05-27 12:48:33.000000 pkrcomponents-1.7.0/coverage.txt
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.526616 pkrcomponents-1.7.0/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1593 2024-05-24 00:57:29.000000 pkrcomponents-1.7.0/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-1.7.0/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.7.0/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.7.0/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.7.0/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/pkrcomponents/lookup_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.574880 pkrcomponents-1.7.0/pkrcomponents/models/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.684695 pkrcomponents-1.7.0/pkrcomponents/models/actions/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.7.0/pkrcomponents/models/actions/move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.7.0/pkrcomponents/models/actions/sequence.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.7.0/pkrcomponents/models/actions/street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.7.0/pkrcomponents/models/amount.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.831285 pkrcomponents-1.7.0/pkrcomponents/models/cards/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.7.0/pkrcomponents/models/cards/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.7.0/pkrcomponents/models/cards/rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.7.0/pkrcomponents/models/cards/suit.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.874130 pkrcomponents-1.7.0/pkrcomponents/models/pots/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.7.0/pkrcomponents/models/pots/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.7.0/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      999 2024-05-15 15:52:00.000000 pkrcomponents-1.7.0/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    16718 2024-05-27 11:48:40.000000 pkrcomponents-1.7.0/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    12484 2024-05-27 09:29:53.000000 pkrcomponents-1.7.0/pkrcomponents/table_player.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    10639 2024-05-25 01:06:35.000000 pkrcomponents-1.7.0/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 12:51:51.902431 pkrcomponents-1.7.0/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      797 2024-05-27 12:51:49.000000 pkrcomponents-1.7.0/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.7.0/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-27 12:51:51.925767 pkrcomponents-1.7.0/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1385 2024-05-24 19:24:47.000000 pkrcomponents-1.7.0/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.519946 pkrcomponents-1.7.1/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:28.841163 pkrcomponents-1.7.1/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.7.1/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.7.1/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-1.7.1/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-27 17:13:29.510715 pkrcomponents-1.7.1/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-1.7.1/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/README.rst
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1400 2024-05-27 17:11:19.000000 pkrcomponents-1.7.1/coverage.txt
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.224331 pkrcomponents-1.7.1/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1593 2024-05-24 00:57:29.000000 pkrcomponents-1.7.1/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-1.7.1/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.7.1/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      628 2024-05-27 15:52:21.000000 pkrcomponents-1.7.1/pkrcomponents/buy_in.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.7.1/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      790 2024-05-27 15:24:49.000000 pkrcomponents-1.7.1/pkrcomponents/level.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.7.1/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/pkrcomponents/lookup_table.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.254996 pkrcomponents-1.7.1/pkrcomponents/models/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.340250 pkrcomponents-1.7.1/pkrcomponents/models/actions/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.7.1/pkrcomponents/models/actions/move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.7.1/pkrcomponents/models/actions/sequence.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.7.1/pkrcomponents/models/actions/street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.7.1/pkrcomponents/models/amount.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.431150 pkrcomponents-1.7.1/pkrcomponents/models/cards/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.7.1/pkrcomponents/models/cards/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.7.1/pkrcomponents/models/cards/rank.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.7.1/pkrcomponents/models/cards/suit.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.450161 pkrcomponents-1.7.1/pkrcomponents/models/pots/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.7.1/pkrcomponents/models/pots/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2246 2024-05-27 16:04:03.000000 pkrcomponents-1.7.1/pkrcomponents/payout.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.7.1/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1039 2024-05-27 14:58:43.000000 pkrcomponents-1.7.1/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    16718 2024-05-27 11:48:40.000000 pkrcomponents-1.7.1/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    12484 2024-05-27 09:29:53.000000 pkrcomponents-1.7.1/pkrcomponents/table_player.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2717 2024-05-27 17:10:53.000000 pkrcomponents-1.7.1/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.485081 pkrcomponents-1.7.1/pkrcomponents/utils/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:06:12.000000 pkrcomponents-1.7.1/pkrcomponents/utils/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      365 2024-05-27 17:06:53.000000 pkrcomponents-1.7.1/pkrcomponents/utils/validators.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:13:29.500214 pkrcomponents-1.7.1/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      934 2024-05-27 17:13:27.000000 pkrcomponents-1.7.1/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.7.1/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-27 17:13:29.519946 pkrcomponents-1.7.1/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1385 2024-05-24 19:24:47.000000 pkrcomponents-1.7.1/setup.py
```

### Comparing `pkrcomponents-1.7.0/LICENSE.txt` & `pkrcomponents-1.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/MANIFEST.in` & `pkrcomponents-1.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/PKG-INFO` & `pkrcomponents-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 1.7.0
+Version: 1.7.1
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
```

### Comparing `pkrcomponents-1.7.0/coverage.txt` & `pkrcomponents-1.7.1/coverage.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-Name                            Stmts   Miss  Cover
----------------------------------------------------
-pkrcomponents/__init__.py           0      0   100%
-pkrcomponents/_common.py           48      0   100%
-pkrcomponents/action.py            32      0   100%
-pkrcomponents/bitcard.py           68      0   100%
-pkrcomponents/board.py             81      0   100%
-pkrcomponents/card.py             112      1    99%
-pkrcomponents/constants.py         71      0   100%
-pkrcomponents/evaluator.py         28      0   100%
-pkrcomponents/hand.py             226      0   100%
-pkrcomponents/listings.py          16      0   100%
-pkrcomponents/lookup_table.py     112      0   100%
-pkrcomponents/players.py           96      0   100%
-pkrcomponents/pot.py               25      0   100%
-pkrcomponents/table.py            326      8    98%
-pkrcomponents/table_player.py     253      4    98%
-pkrcomponents/tournament.py       258      0   100%
----------------------------------------------------
-TOTAL                            1752     13    99%
+Name                                Stmts   Miss  Cover
+-------------------------------------------------------
+pkrcomponents/__init__.py               0      0   100%
+pkrcomponents/_common.py               48      0   100%
+pkrcomponents/action.py                32      0   100%
+pkrcomponents/bitcard.py               68      0   100%
+pkrcomponents/board.py                 81      0   100%
+pkrcomponents/buy_in.py                14      0   100%
+pkrcomponents/card.py                 112      1    99%
+pkrcomponents/constants.py             71      0   100%
+pkrcomponents/evaluator.py             28      0   100%
+pkrcomponents/hand.py                 226      0   100%
+pkrcomponents/level.py                 17      0   100%
+pkrcomponents/listings.py              16      0   100%
+pkrcomponents/lookup_table.py         112      0   100%
+pkrcomponents/payout.py                39      0   100%
+pkrcomponents/players.py               96      0   100%
+pkrcomponents/pot.py                   13      0   100%
+pkrcomponents/table.py                326      8    98%
+pkrcomponents/table_player.py         253      4    98%
+pkrcomponents/tournament.py            46      0   100%
+pkrcomponents/utils/__init__.py         0      0   100%
+pkrcomponents/utils/validators.py       7      1    86%
+-------------------------------------------------------
+TOTAL                                1605     14    99%
```

### Comparing `pkrcomponents-1.7.0/pkrcomponents/_common.py` & `pkrcomponents-1.7.1/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/action.py` & `pkrcomponents-1.7.1/pkrcomponents/action.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/bitcard.py` & `pkrcomponents-1.7.1/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/board.py` & `pkrcomponents-1.7.1/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/card.py` & `pkrcomponents-1.7.1/pkrcomponents/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/constants.py` & `pkrcomponents-1.7.1/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/evaluator.py` & `pkrcomponents-1.7.1/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/hand.py` & `pkrcomponents-1.7.1/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/listings.py` & `pkrcomponents-1.7.1/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/lookup_table.py` & `pkrcomponents-1.7.1/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/models/actions/move.py` & `pkrcomponents-1.7.1/pkrcomponents/models/actions/move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/models/actions/street.py` & `pkrcomponents-1.7.1/pkrcomponents/models/actions/street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/models/amount.py` & `pkrcomponents-1.7.1/pkrcomponents/models/amount.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/models/cards/card.py` & `pkrcomponents-1.7.1/pkrcomponents/models/cards/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/models/cards/rank.py` & `pkrcomponents-1.7.1/pkrcomponents/models/cards/rank.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/models/cards/suit.py` & `pkrcomponents-1.7.1/pkrcomponents/models/cards/suit.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/models/pots/pot.py` & `pkrcomponents-1.7.1/pkrcomponents/models/pots/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/players.py` & `pkrcomponents-1.7.1/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/table.py` & `pkrcomponents-1.7.1/pkrcomponents/table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents/table_player.py` & `pkrcomponents-1.7.1/pkrcomponents/table_player.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.0/pkrcomponents.egg-info/SOURCES.txt` & `pkrcomponents-1.7.1/pkrcomponents.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,26 +7,31 @@
 setup.py
 .pytest_cache/README.md
 pkrcomponents/__init__.py
 pkrcomponents/_common.py
 pkrcomponents/action.py
 pkrcomponents/bitcard.py
 pkrcomponents/board.py
+pkrcomponents/buy_in.py
 pkrcomponents/card.py
 pkrcomponents/constants.py
 pkrcomponents/evaluator.py
 pkrcomponents/hand.py
+pkrcomponents/level.py
 pkrcomponents/listings.py
 pkrcomponents/lookup_table.py
+pkrcomponents/payout.py
 pkrcomponents/players.py
 pkrcomponents/pot.py
 pkrcomponents/table.py
 pkrcomponents/table_player.py
 pkrcomponents/tournament.py
 pkrcomponents/models/amount.py
 pkrcomponents/models/actions/move.py
 pkrcomponents/models/actions/sequence.py
 pkrcomponents/models/actions/street.py
 pkrcomponents/models/cards/card.py
 pkrcomponents/models/cards/rank.py
 pkrcomponents/models/cards/suit.py
-pkrcomponents/models/pots/pot.py
+pkrcomponents/models/pots/pot.py
+pkrcomponents/utils/__init__.py
+pkrcomponents/utils/validators.py
```

### Comparing `pkrcomponents-1.7.0/setup.py` & `pkrcomponents-1.7.1/setup.py`

 * *Files identical despite different names*

