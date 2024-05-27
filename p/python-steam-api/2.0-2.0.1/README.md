# Comparing `tmp/python-steam-api-2.0.tar.gz` & `tmp/python_steam_api-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-steam-api-2.0.tar", last modified: Sat Apr  6 16:13:06 2024, max compression
+gzip compressed data, was "python_steam_api-2.0.1.tar", last modified: Mon May 27 15:14:52 2024, max compression
```

## Comparing `python-steam-api-2.0.tar` & `python_steam_api-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:13:06.370955 python-steam-api-2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-06 16:12:46.000000 python-steam-api-2.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-04-06 16:13:06.370955 python-steam-api-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18235 2024-04-06 16:12:46.000000 python-steam-api-2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-06 16:12:46.000000 python-steam-api-2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:13:06.370955 python-steam-api-2.0/python_steam_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-04-06 16:13:06.000000 python-steam-api-2.0/python_steam_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-06 16:13:06.000000 python-steam-api-2.0/python_steam_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:13:06.000000 python-steam-api-2.0/python_steam_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-06 16:13:06.000000 python-steam-api-2.0/python_steam_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-06 16:13:06.000000 python-steam-api-2.0/python_steam_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 16:13:06.370955 python-steam-api-2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:13:06.366955 python-steam-api-2.0/steam_web_api/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/steam.py
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-06 16:12:46.000000 python-steam-api-2.0/steam_web_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:14:52.596397 python_steam_api-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-27 15:14:37.000000 python_steam_api-2.0.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)    19334 2024-05-27 15:14:52.596397 python_steam_api-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18235 2024-05-27 15:14:37.000000 python_steam_api-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-27 15:14:37.000000 python_steam_api-2.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:14:52.592397 python_steam_api-2.0.1/python_steam_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19334 2024-05-27 15:14:52.000000 python_steam_api-2.0.1/python_steam_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-27 15:14:52.000000 python_steam_api-2.0.1/python_steam_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:14:52.000000 python_steam_api-2.0.1/python_steam_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-27 15:14:52.000000 python_steam_api-2.0.1/python_steam_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 15:14:52.000000 python_steam_api-2.0.1/python_steam_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:14:52.596397 python_steam_api-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:14:52.592397 python_steam_api-2.0.1/steam_web_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-27 15:14:37.000000 python_steam_api-2.0.1/steam_web_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-27 15:14:37.000000 python_steam_api-2.0.1/steam_web_api/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-27 15:14:37.000000 python_steam_api-2.0.1/steam_web_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-27 15:14:37.000000 python_steam_api-2.0.1/steam_web_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-27 15:14:37.000000 python_steam_api-2.0.1/steam_web_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-27 15:14:37.000000 python_steam_api-2.0.1/steam_web_api/steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-27 15:14:37.000000 python_steam_api-2.0.1/steam_web_api/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-27 15:14:37.000000 python_steam_api-2.0.1/steam_web_api/utils.py
```

### Comparing `python-steam-api-2.0/LICENCE` & `python_steam_api-2.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `python-steam-api-2.0/PKG-INFO` & `python_steam_api-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-steam-api
-Version: 2.0
+Version: 2.0.1
 Summary: Python Client wrapper for Steam API.
 Author-email: David Salazar <david.asal@hotmail.com>
 Maintainer-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 Project-URL: source, https://github.com/deivit24/python-steam-api
 Project-URL: tracker, https://github.com/deivit24/python-steam-api/issues
 Keywords: api,python,steam community,steam,steamapi
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-steam-api-2.0/README.md` & `python_steam_api-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `python-steam-api-2.0/pyproject.toml` & `python_steam_api-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 license = {file = 'LICENSE'}
 maintainers = [
   {email = 'mathieu.scheltienne@fcbg.ch', name = 'Mathieu Scheltienne'},
 ]
 name = 'python-steam-api'
 readme = 'README.md'
 requires-python = '>=3.9'
-version = '2.0'
+version = '2.0.1'
 
 [project.optional-dependencies]
 all = [
   'python-steam-api[build]',
   'python-steam-api[style]',
 ]
 build = [
```

### Comparing `python-steam-api-2.0/python_steam_api.egg-info/PKG-INFO` & `python_steam_api-2.0.1/python_steam_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-steam-api
-Version: 2.0
+Version: 2.0.1
 Summary: Python Client wrapper for Steam API.
 Author-email: David Salazar <david.asal@hotmail.com>
 Maintainer-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 Project-URL: source, https://github.com/deivit24/python-steam-api
 Project-URL: tracker, https://github.com/deivit24/python-steam-api/issues
 Keywords: api,python,steam community,steam,steamapi
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-steam-api-2.0/steam_web_api/apps.py` & `python_steam_api-2.0.1/steam_web_api/apps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,144 +1,158 @@
-import json
-import typing
-
-from bs4 import BeautifulSoup
-from requests import Response, request
-
-from .client import Client
-from .constants import API_APP_DETAILS_URL, API_APP_SEARCH_URL
-from .utils import buildUrlWithParamsForSearch
-
-
-class Apps:
-    """Steam Apps API client"""
-
-    def __init__(self, client: Client):
-        """Constructor for Steam Apps class"""
-        self.__client = client
-        self.__search_url = API_APP_SEARCH_URL
-        self.__app_details_url = API_APP_DETAILS_URL
-
-    def get_app_details(self, app_id: int, country="US", filters: typing.Optional[str] = "basic") -> dict:
-        """Obtains an apps details
-
-        Args:
-            app_id (int): App ID. For example 546560 (Half-Life-Alyx)
-            country (str): ISO Country Code
-            filters (str): list of keys to return, e.g. "name,platforms,price_overview". If you use multiple appids, you must set this parameter to "price_overview".
-                The filter basic returns the following keys:
-                    type
-                    name
-                    steam_appid
-                    required_age
-                    dlc
-                    detailed_description
-                    about_the_game
-                    supported_languages
-                    detailed_description
-                    supported_languages
-                    header_image
-                    website
-                    pc_requirements
-                    mac_requirements
-                    linux_requirements
-                Any key names except those listed under basic are acceptable as filter values.
-                Optional filters:
-                    controller_support,
-                    fullgame,
-                    legal_notice,
-                    developers,
-                    demos,
-                    price_overview,
-                    metacritic,
-                    categories,
-                    genres,
-                    screenshots,
-                    movies,
-                    recommendations,
-                    achievements,
-        """
-        response = request("get", self.__app_details_url, params={"appids": app_id, "cc": country, "filters": filters})
-        json_loaded_response = json.loads(response.text)
-        return json_loaded_response
-
-    def get_user_stats(self, steam_id: int, app_id: int) -> dict:
-        """Obtains a user's stats for a specific app, includes only completed achievements
-        along with app specific information
-
-        Args:
-            steam_id (int): Steam 64 ID
-            app_id (int): App ID
-        """
-        response = self.__client.request(
-            "get",
-            "/ISteamUserStats/GetUserStatsForGame/v2/",
-            params={"steamid": steam_id, "appid": app_id},
-        )
-        return response
-
-    def get_user_achievements(self, steam_id: int, app_id: int) -> dict:
-        """Obtains information of the user's achievments in the app
-
-        Args:
-            steam_id (int): Steam 64 ID
-            app_id (int): App ID
-        """
-        response = self.__client.request(
-            "get",
-            "/ISteamUserStats/GetPlayerAchievements/v1/",
-            params={"steamid": steam_id, "appid": app_id},
-        )
-        return response
-
-    # Is term meant to be any or a string, I'm not familiar enough with steam search so I'll leave it as is
-    def search_games(self, term, country="US"):
-        """Searches for games using the information given
-        Args:
-            term (Any): Search term
-            country (str): ISO Country Code
-        """
-        url = self.search_url(term, country)
-        result = request("get", url)
-        html = self.__validator(result)
-        soup = BeautifulSoup(html, features="html.parser")
-        links = soup.find_all("a")
-        apps = []
-        for link in links:
-            if link.has_attr("data-ds-appid"):
-                app = {}
-                string_id = link["data-ds-appid"]
-                href = link["href"].replace("\\", "").replace('"', "")
-                app["id"] = [int(i) for i in string_id.replace("\\", "").replace('"', "").split(",")]
-                app["link"] = href
-                divs = link.select("div")
-                for div in divs:
-                    if div["class"][0] == '\\"match_name\\"':
-                        app["name"] = div.text
-                    if div["class"][0] == '\\"match_price\\"':
-                        app["price"] = div.text
-                    if div["class"][0] == '\\"match_img\\"':
-                        app["img"] = div.img["src"].replace("\\", "").replace('"', "")
-                apps.append(app)
-        return {"apps": apps}
-
-    # This should be a private method imo, I don't know how you would like to name them so I'll leave it as is
-    # (Maybe change it to all caps since __search_url and __app_details_url are constants?)
-    def search_url(self, search, country="US"):
-        params = {"f": "games", "cc": country, "realm": 1, "l": "english"}
-        result = buildUrlWithParamsForSearch((self.__search_url), search, params=params)
-        return result
-
-    def __validator(self, result: Response) -> typing.Union[str, dict]:
-        try:
-            body = json.dumps(result.text)
-        except Exception:
-            body = {}
-
-        if isinstance(body, dict) and body.get("code", None) is not None:
-            raise Exception(body.get("description"))
-        elif result.status_code >= 400:
-            raise Exception(" ".join([str(result.status_code), result.reason]))
-        elif len(result.text) == 0:
-            return "OK"
-        else:
-            return body
+import json
+import typing
+
+from bs4 import BeautifulSoup
+from requests import Response, request
+
+from .client import Client
+from .constants import API_APP_DETAILS_URL, API_APP_SEARCH_URL
+from .utils import buildUrlWithParamsForSearch
+
+
+class Apps:
+    """Steam Apps API client"""
+
+    def __init__(self, client: Client):
+        """Constructor for Steam Apps class"""
+        self.__client = client
+        self.__search_url = API_APP_SEARCH_URL
+        self.__app_details_url = API_APP_DETAILS_URL
+
+    def get_app_details(self, app_id: int, country="US", filters: typing.Optional[str] = "basic") -> dict:
+        """Obtains an apps details
+
+        Args:
+            app_id (int): App ID. For example 546560 (Half-Life-Alyx)
+            country (str): ISO Country Code
+            filters (str): list of keys to return, e.g. "name,platforms,price_overview". If you use multiple appids,
+            you must set this parameter to "price_overview".
+                The filter basic returns the following keys:
+                    type
+                    name
+                    steam_appid
+                    required_age
+                    dlc
+                    detailed_description
+                    about_the_game
+                    supported_languages
+                    detailed_description
+                    supported_languages
+                    header_image
+                    website
+                    pc_requirements
+                    mac_requirements
+                    linux_requirements
+                Any key names except those listed under basic are acceptable as filter values.
+                Optional filters:
+                    controller_support,
+                    fullgame,
+                    legal_notice,
+                    developers,
+                    demos,
+                    price_overview,
+                    metacritic,
+                    categories,
+                    genres,
+                    screenshots,
+                    movies,
+                    recommendations,
+                    achievements,
+        """
+        response = request("get", self.__app_details_url, params={"appids": app_id, "cc": country, "filters": filters})
+        json_loaded_response = json.loads(response.text)
+        return json_loaded_response
+
+    def get_user_stats(self, steam_id: int, app_id: int) -> dict:
+        """Obtains a user's stats for a specific app, includes only completed achievements
+        along with app specific information
+
+        Args:
+            steam_id (int): Steam 64 ID
+            app_id (int): App ID
+        """
+        response = self.__client.request(
+            "get",
+            "/ISteamUserStats/GetUserStatsForGame/v2/",
+            params={"steamid": steam_id, "appid": app_id},
+        )
+        return response
+
+    def get_user_achievements(self, steam_id: int, app_id: int, language: str = "en") -> dict:
+        """Obtains information of the user's achievements in the app
+
+        Args:
+            steam_id (int): Steam 64 ID
+            app_id (int): App ID
+            language: (str) Abbriviated language
+        """
+        response = self.__client.request(
+            "get",
+            "/ISteamUserStats/GetPlayerAchievements/v1/",
+            params={"steamid": steam_id, "appid": app_id, "l": language},
+        )
+        return response
+
+    # Is term meant to be any or a string, I'm not familiar enough with steam search so I'll leave it as is
+    def search_games(self, term, country="US"):
+        """Searches for games using the information given
+        Args:
+            term (Any): Search term
+            country (str): ISO Country Code
+        """
+        url = self.search_url(term, country)
+        result = request("get", url)
+        html = self.__validator(result)
+
+        # Decode the HTML content for Unicode escape sequences
+        decoded_html = html.encode("utf-8").decode("unicode_escape")
+
+        # Parse the decoded HTML with BeautifulSoup
+        soup = BeautifulSoup(decoded_html, features="html.parser")
+        links = soup.find_all("a")
+        apps = []
+        for link in links:
+            if link.has_attr("data-ds-appid"):
+                app = {}
+                string_id = link["data-ds-appid"]
+                href = link["href"].replace("\\", "").replace('"', "")
+                app["id"] = [int(i) for i in string_id.replace("\\", "").replace('"', "").split(",")]
+                app["link"] = href
+
+                # Extracting the div elements and their content
+                divs = link.find_all("div")
+                for div in divs:
+                    class_name = div.get("class")[0].strip('\\"')
+                    if class_name == "match_name":
+                        app["name"] = div.text
+                    elif class_name == "match_price":
+                        app["price"] = div.text
+                    elif class_name == "match_img":
+                        img_tag = div.find("img")
+                        if img_tag and img_tag.has_attr("src"):
+                            app["img"] = img_tag["src"].replace("\\", "").replace('"', "")
+
+                apps.append(app)
+
+        return {"apps": apps}
+
+    # This should be a private method imo, I don't know how you would like to name them so I'll leave it as is
+    # (Maybe change it to all caps since __search_url and __app_details_url are constants?)
+    def search_url(self, search, country="US"):
+        params = {"f": "games", "cc": country, "realm": 1, "l": "english"}
+        result = buildUrlWithParamsForSearch((self.__search_url), search, params=params)
+        return result
+
+    def __validator(self, result: Response) -> typing.Union[str, dict]:
+        try:
+            body = json.dumps(result.text)
+        except Exception:
+            body = {}
+
+        if isinstance(body, dict) and body.get("code", None) is not None:
+            raise Exception(body.get("description"))
+        elif result.status_code >= 400:
+            raise Exception(" ".join([str(result.status_code), result.reason]))
+        elif len(result.text) == 0:
+            return "OK"
+        else:
+            return body
```

### Comparing `python-steam-api-2.0/steam_web_api/client.py` & `python_steam_api-2.0.1/steam_web_api/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import json
-import typing
-
-import requests
-
-from .constants import API_BASE_URL
-from .utils import buildUrlWithParams, mergeDict, retry
-
-
-class Client:
-    """Steams API HTTP client"""
-
-    def __init__(self, key: str, headers: dict = {}):
-        """Constructor for TypeForm API client"""
-        self.__headers = mergeDict(
-            {
-                "Content-Type": "application/json",
-                "Accept": "application/json",
-            },
-            headers,
-        )
-        self.key = key
-
-    @retry(times=3, exceptions=(ValueError, TypeError))
-    def request(self, method: str, url: str, data: any = {}, params: dict = {}, headers={}) -> typing.Union[str, dict]:
-        requestUrl = buildUrlWithParams((API_BASE_URL + url), self.key, params)
-        requestHeaders = mergeDict(self.__headers, headers)
-        requestData = json.dumps(data) if len(data.keys()) > 0 else ""
-        result = requests.request(method, requestUrl, data=requestData, headers=requestHeaders)
-        return self.__validator(result)
-
-    def __validator(self, result: requests.Response) -> typing.Union[str, dict]:
-        try:
-            body = json.loads(result.text)
-        except Exception:
-            body = {}
-
-        if isinstance(body, dict) and body.get("code", None) is not None:
-            raise Exception(body.get("description"))
-        elif result.status_code >= 400:
-            raise Exception(" ".join([str(result.status_code), result.reason]))
-        elif len(result.text) == 0:
-            return "OK"
-        else:
-            return body
+import json
+import typing
+
+import requests
+
+from .constants import API_BASE_URL
+from .utils import buildUrlWithParams, mergeDict, retry
+
+
+class Client:
+    """Streams API HTTP client"""
+
+    def __init__(self, key: str, headers: dict = {}):
+        """Constructor for TypeForm API client"""
+        self.__headers = mergeDict(
+            {
+                "Content-Type": "application/json",
+                "Accept": "application/json",
+            },
+            headers,
+        )
+        self.key = key
+
+    @retry(times=3, exceptions=(ValueError, TypeError))
+    def request(self, method: str, url: str, data: any = {}, params: dict = {}, headers={}) -> typing.Union[str, dict]:
+        requestUrl = buildUrlWithParams((API_BASE_URL + url), self.key, params)
+        requestHeaders = mergeDict(self.__headers, headers)
+        requestData = json.dumps(data) if len(data.keys()) > 0 else ""
+        result = requests.request(method, requestUrl, data=requestData, headers=requestHeaders)
+        return self.__validator(result)
+
+    def __validator(self, result: requests.Response) -> typing.Union[str, dict]:
+        try:
+            body = json.loads(result.text)
+        except Exception:
+            body = {}
+
+        if isinstance(body, dict) and body.get("code", None) is not None:
+            raise Exception(body.get("description"))
+        elif result.status_code >= 400:
+            raise Exception(" ".join([str(result.status_code), result.reason, result.text]))
+        elif len(result.text) == 0:
+            return "OK"
+        else:
+            return body
```

### Comparing `python-steam-api-2.0/steam_web_api/users.py` & `python_steam_api-2.0.1/steam_web_api/users.py`

 * *Files identical despite different names*

### Comparing `python-steam-api-2.0/steam_web_api/utils.py` & `python_steam_api-2.0.1/steam_web_api/utils.py`

 * *Files identical despite different names*

