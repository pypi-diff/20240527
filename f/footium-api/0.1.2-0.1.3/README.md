# Comparing `tmp/footium_api-0.1.2.tar.gz` & `tmp/footium_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "footium_api-0.1.2.tar", last modified: Sun May 19 00:41:17 2024, max compression
+gzip compressed data, was "footium_api-0.1.3.tar", last modified: Sun May 26 22:02:37 2024, max compression
```

## Comparing `footium_api-0.1.2.tar` & `footium_api-0.1.3.tar`

### file list

```diff
@@ -1,44 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:41:17.372030 footium_api-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-19 00:41:05.000000 footium_api-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-19 00:41:17.372030 footium_api-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-19 00:41:05.000000 footium_api-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:41:17.364030 footium_api-0.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 00:41:05.000000 footium_api-0.1.2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-19 00:41:05.000000 footium_api-0.1.2/examples/setup_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-19 00:41:05.000000 footium_api-0.1.2/examples/try_best_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-19 00:41:05.000000 footium_api-0.1.2/examples/try_club_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-19 00:41:05.000000 footium_api-0.1.2/examples/try_footium_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-19 00:41:05.000000 footium_api-0.1.2/examples/try_formations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-19 00:41:05.000000 footium_api-0.1.2/examples/try_get_next_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-19 00:41:05.000000 footium_api-0.1.2/examples/try_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:41:17.368030 footium_api-0.1.2/footium_api/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-19 00:41:05.000000 footium_api-0.1.2/footium_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-19 00:41:05.000000 footium_api-0.1.2/footium_api/gql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-19 00:41:05.000000 footium_api-0.1.2/footium_api/key_signer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:41:17.368030 footium_api-0.1.2/footium_api/mutations/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-19 00:41:05.000000 footium_api-0.1.2/footium_api/mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-19 00:41:05.000000 footium_api-0.1.2/footium_api/mutations/lineups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:41:17.368030 footium_api-0.1.2/footium_api/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-19 00:41:05.000000 footium_api-0.1.2/footium_api/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-19 00:41:05.000000 footium_api-0.1.2/footium_api/queries/all_clubs_basic_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-19 00:41:05.000000 footium_api-0.1.2/footium_api/queries/club_tournaments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-19 00:41:05.000000 footium_api-0.1.2/footium_api/queries/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-19 00:41:05.000000 footium_api-0.1.2/footium_api/queries/formations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-19 00:41:05.000000 footium_api-0.1.2/footium_api/queries/lineups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-19 00:41:05.000000 footium_api-0.1.2/footium_api/queries/players.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-19 00:41:05.000000 footium_api-0.1.2/footium_api/queries/server_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-19 00:41:05.000000 footium_api-0.1.2/footium_api/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:41:17.368030 footium_api-0.1.2/footium_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-19 00:41:17.000000 footium_api-0.1.2/footium_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-19 00:41:17.000000 footium_api-0.1.2/footium_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 00:41:17.000000 footium_api-0.1.2/footium_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-19 00:41:17.000000 footium_api-0.1.2/footium_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 00:41:17.000000 footium_api-0.1.2/footium_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-19 00:41:05.000000 footium_api-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 00:41:17.372030 footium_api-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-19 00:41:05.000000 footium_api-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:41:17.368030 footium_api-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-19 00:41:05.000000 footium_api-0.1.2/tests/test_get_all_clubs_basic_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-19 00:41:05.000000 footium_api-0.1.2/tests/test_gql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-19 00:41:05.000000 footium_api-0.1.2/tests/test_key_signer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-19 00:41:05.000000 footium_api-0.1.2/tests/test_report_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:02:37.862044 footium_api-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-26 22:02:26.000000 footium_api-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-26 22:02:37.862044 footium_api-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-26 22:02:26.000000 footium_api-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:02:37.854044 footium_api-0.1.3/footium_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/cached_gql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/gql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/key_signer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:02:37.858044 footium_api-0.1.3/footium_api/mutations/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/mutations/lineups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:02:37.858044 footium_api-0.1.3/footium_api/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/queries/all_clubs_basic_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/queries/club_tournaments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/queries/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/queries/formations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/queries/lineups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/queries/players.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/queries/server_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-26 22:02:26.000000 footium_api-0.1.3/footium_api/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:02:37.858044 footium_api-0.1.3/footium_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-26 22:02:37.000000 footium_api-0.1.3/footium_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-26 22:02:37.000000 footium_api-0.1.3/footium_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 22:02:37.000000 footium_api-0.1.3/footium_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-26 22:02:37.000000 footium_api-0.1.3/footium_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 22:02:37.000000 footium_api-0.1.3/footium_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-26 22:02:26.000000 footium_api-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 22:02:37.862044 footium_api-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-26 22:02:26.000000 footium_api-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:02:37.858044 footium_api-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-26 22:02:26.000000 footium_api-0.1.3/tests/test_cached_gql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-26 22:02:26.000000 footium_api-0.1.3/tests/test_get_all_clubs_basic_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-26 22:02:26.000000 footium_api-0.1.3/tests/test_gql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-26 22:02:26.000000 footium_api-0.1.3/tests/test_key_signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-26 22:02:26.000000 footium_api-0.1.3/tests/test_report_strategy.py
```

### Comparing `footium_api-0.1.2/LICENSE` & `footium_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.2/examples/try_footium_api.py` & `footium_api-0.1.3/footium_api/mutations/lineups.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,50 @@
-from setup_environment import *  # noqa: F403
-from footium_api import GqlConnection
-from footium_api.queries import (
-    get_formations,
-    get_lineup_for_club,
-    get_server_timestamp,
-)
-from footium_api.mutations import prepare_lineup_to_sign, submit_lineup
-from key_signer import KeySigner
-
-gql = GqlConnection()
-formations = get_formations(gql)
-for formation in formations:
-    print(f"{formation.id}: {formation.name}")
-lineup = get_lineup_for_club(gql, 2879, False)
-# print(lineup)
-timestamp = get_server_timestamp(gql)
-print(timestamp)
-
+import json
 
-key_signer = KeySigner()
-lineup_message = prepare_lineup_to_sign(gql, lineup)
-
-# signature = "0x2a1e2db05a713e5965563d27bb12e07b715808980fefba0dd2f124fef4c63b99516d3e9c0cc1d3604beaf24fe22bf375690fc0bea460cdad6a46b2f5a97c147b1c"
-# address = "0x1839faea698cbae6ede826c09d943de1dba7dd96"
-signature = key_signer.sign_message(lineup_message)
-address = key_signer.get_eth_address()
-is_legit = key_signer.validate_signed_message(signature, lineup_message)
-print(f"signature: {signature}, is_legit: {is_legit}")
-result = submit_lineup(
-    gql, message=lineup_message, signed_message=signature, address=address
-)
+from footium_api import GqlConnection
+from footium_api.queries import get_server_timestamp
 
-if result.code == 200:
-    print("Lineup submitted successfully")
-else:
-    print(f"Error: {result.message}")
 
-print("done")
+def prepare_lineup_to_sign(gql: GqlConnection, lineup):
+    timestamp = get_server_timestamp(gql)
+    message = {
+        "id": -1,
+        "type": "LINEUP_SET",
+        "data": {
+            "lineup": {
+                "id": lineup.id,
+                "clubId": lineup.clubId,
+                "isSelected": lineup.isSelected,
+                "tacticsId": lineup.tacticsId,
+            },
+            "tactics": {
+                "id": lineup.tactics.id,
+                "mentality": lineup.tactics.mentality,
+                "formationId": lineup.tactics.formationId,
+            },
+            "playerLineups": lineup.playerLineups.to_list(),
+        },
+        "timestamp": timestamp,
+    }
+    json_message = json.dumps(message)
+    return json_message
+
+
+def submit_lineup(gql: GqlConnection, message, signed_message, address):
+    query = """
+mutation SubmitAction($action: String!, $signature: String!, $address: String!) {
+    submitAction(action: $action, signature: $signature, address: $address)
+    {
+        code
+        error
+        message
+        __typename
+    }
+}
+"""
+    variables = {
+        "signature": signed_message,
+        "address": address,
+        "action": message,
+    }
+    response = gql.send_mutation(query, variables)
+    return response
```

### Comparing `footium_api-0.1.2/footium_api/gql_connection.py` & `footium_api-0.1.3/footium_api/gql_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,23 +43,24 @@
         )
         boxed_response = Box(response)
         return boxed_response
 
     def send_paging_query(
         self, 
         query: str, 
-        variables: Dict[str, Any] = {}, 
+        variables: Dict[str, Any] = None, 
         operation_name: Optional[str] = None, 
         skip: int = 0, 
         page_size: int = 20, 
         take: Optional[int] = None
     ) -> Union[Box, list]:
         gql_query = gql(query)
         results = None
         count = 0
+        variables = variables or {}
         while True:
             variables["skip"] = skip
             variables["take"] = page_size
             response = self.client.execute(
                 gql_query, variable_values=variables, operation_name=operation_name
             )
             boxed_response = Box(response)
```

### Comparing `footium_api-0.1.2/footium_api/key_signer.py` & `footium_api-0.1.3/footium_api/key_signer.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.2/footium_api/queries/__init__.py` & `footium_api-0.1.3/footium_api/queries/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from .formations import get_formations, get_formations_as_pd
 from .lineups import get_lineup_for_club
 from .server_metadata import get_server_timestamp
-from .club_tournaments import get_clubs_tournament_for_owners
+from .club_tournaments import get_clubs_tournament_for_owners, get_clubs_tournament_for_wallet, get_clubs_tournament_for_club_ids
 from .players import get_players, get_players_in_clubs
 from .all_clubs_basic_info import get_all_clubs_basic_info
 from .fixtures import get_next_fixtures
 
 __all__ = [
     "get_formations",
     "get_formations_as_pd",
     "get_lineup_for_club",
     "get_server_timestamp",
-    "get_clubs_tournament_for_owners",
+    "get_clubs_tournament_for_owners", "get_clubs_tournament_for_wallet", "get_clubs_tournament_for_club_ids",
     "get_players",
     "get_players_in_clubs",
     "get_all_clubs_basic_info",
     "get_next_fixtures",
 ]
```

### Comparing `footium_api-0.1.2/footium_api/queries/fixtures.py` & `footium_api-0.1.3/footium_api/queries/fixtures.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.2/footium_api/queries/formations.py` & `footium_api-0.1.3/footium_api/queries/formations.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.2/footium_api/queries/lineups.py` & `footium_api-0.1.3/footium_api/queries/lineups.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.2/footium_api/queries/players.py` & `footium_api-0.1.3/footium_api/queries/players.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.2/footium_api/report.py` & `footium_api-0.1.3/footium_api/report.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.2/tests/test_get_all_clubs_basic_info.py` & `footium_api-0.1.3/tests/test_get_all_clubs_basic_info.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.2/tests/test_gql_connection.py` & `footium_api-0.1.3/tests/test_gql_connection.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.2/tests/test_key_signer.py` & `footium_api-0.1.3/tests/test_key_signer.py`

 * *Files identical despite different names*

### Comparing `footium_api-0.1.2/tests/test_report_strategy.py` & `footium_api-0.1.3/tests/test_report_strategy.py`

 * *Files identical despite different names*

