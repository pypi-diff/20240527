# Comparing `tmp/synapse_token_authenticator-0.4.6.tar.gz` & `tmp/synapse_token_authenticator-0.5.0.tar.gz`

## Comparing `synapse_token_authenticator-0.4.6.tar` & `synapse_token_authenticator-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/CHANGELOG.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/CODEOWNERS
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/cliff.toml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/.github/CODEOWNERS
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/.github/workflows/main.yml
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/.github/workflows/python.yml
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/synapse_token_authenticator/__init__.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/synapse_token_authenticator/config.py
--rw-r--r--   0        0        0    13575 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/synapse_token_authenticator/token_authenticator.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/synapse_token_authenticator/utils.py
--rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/__init__.py
--rw-r--r--   0        0        0    13774 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/server.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/test_custom.py
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/test_jwt.py
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/test_oidc.py
--rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/unittest.py
--rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/utils.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/test_utils/html_parsers.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/tests/test_utils/logging_setup.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/.gitignore
--rw-r--r--   0        0        0    34468 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/LICENSE
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/README.md
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/CODEOWNERS
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/cliff.toml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/.github/workflows/python.yml
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/synapse_token_authenticator/__init__.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/synapse_token_authenticator/config.py
+-rw-r--r--   0        0        0    13652 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/synapse_token_authenticator/token_authenticator.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/synapse_token_authenticator/utils.py
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0    13774 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/tests/server.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/tests/test_custom.py
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/tests/test_jwt.py
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/tests/test_oidc.py
+-rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/tests/unittest.py
+-rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/tests/utils.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/tests/test_utils/html_parsers.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/tests/test_utils/logging_setup.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/.gitignore
+-rw-r--r--   0        0        0    34468 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/README.md
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 synapse_token_authenticator-0.5.0/PKG-INFO
```

### Comparing `synapse_token_authenticator-0.4.6/CHANGELOG.md` & `synapse_token_authenticator-0.5.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.5.0] - 2024-05-24
+
+### Bug Fixes
+
+- Use SimpleHttpClient with proxy enabled
+- [**breaking**]: Account for baseurl with path in oidc metadata
+  - The oidc issuer base URL must be configured with a trailing slash to function properly, this must be checked in existing configurations.
+- Post introspection req urlencoded
+
 ## [0.4.6] - 2024-05-06
 
 ### Features
 
 - Add custom jwt flow
 
 ## [0.4.5] - 2024-04-25
```

### Comparing `synapse_token_authenticator-0.4.6/cliff.toml` & `synapse_token_authenticator-0.5.0/cliff.toml`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.6/.github/workflows/publish.yml` & `synapse_token_authenticator-0.5.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.6/.github/workflows/python.yml` & `synapse_token_authenticator-0.5.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.6/synapse_token_authenticator/config.py` & `synapse_token_authenticator-0.5.0/synapse_token_authenticator/config.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.6/synapse_token_authenticator/token_authenticator.py` & `synapse_token_authenticator-0.5.0/synapse_token_authenticator/token_authenticator.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,22 +211,23 @@
             logger.info("Wrong login type")
             return None
         if "token" not in login_dict:
             logger.info("Missing token")
             return None
         token = login_dict["token"]
 
+        client = self.api._hs.get_proxied_http_client()
         oidc = self.config.oidc
-        oidc_metadata = await get_oidp_metadata(oidc.issuer, self.api.http_client)
+        oidc_metadata = await get_oidp_metadata(oidc.issuer, client)
 
         # Further validation using token introspection
         data = {"token": token, "token_type_hint": "access_token", "scope": "openid"}
 
         try:
-            introspection_resp = await self.api.http_client.post_json_get_json(
+            introspection_resp = await client.post_urlencoded_get_json(
                 oidc_metadata.introspection_endpoint,
                 data,
                 headers=basic_auth(oidc.client_id, oidc.client_secret),
             )
         except HttpResponseException as e:
             if e.code == 401:
                 logger.info("User's access token is invalid")
@@ -299,14 +300,16 @@
             logger.info("Wrong login type")
             return None
         if "token" not in login_dict:
             logger.info("Missing token")
             return None
         token = login_dict["token"]
 
+        client = self.api._hs.get_proxied_http_client()
+
         check_claims = {}
 
         user_id_str = self.api.get_qualified_user_id(username)
         check_claims["urn:messaging:matrix:localpart"] = username
         check_claims["urn:messaging:matrix:mxid"] = user_id_str
 
         if self.config.custom_flow.require_expiry:
@@ -346,15 +349,15 @@
             if self.config.custom_flow.notification_access_token is not None:
                 headers = {
                     b"Authorization": [
                         b"Bearer " + self.config.custom_flow.notification_access_token
                     ]
                 }
 
-            await self.api.http_client.post_json_get_json(
+            await client.post_json_get_json(
                 self.config.custom_flow.notify_on_registration_uri,
                 {"token": login_dict["token"]},
                 headers=headers,
             )
 
             logger.info("Registered user %s (%s)", user_id, payload["name"])
```

### Comparing `synapse_token_authenticator-0.4.6/synapse_token_authenticator/utils.py` & `synapse_token_authenticator-0.5.0/synapse_token_authenticator/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.id_token_signing_alg_values_supported: list[str] = configuration[
             "id_token_signing_alg_values_supported"
         ]
 
 
 async def get_oidp_metadata(issuer, client) -> OpenIDProviderMetadata:
     config = await client.get_json(
-        urljoin(issuer, "/.well-known/openid-configuration"),
+        urljoin(issuer, ".well-known/openid-configuration"),
     )
     return OpenIDProviderMetadata(issuer, config)
 
 
 def basic_auth(username: str, password: str) -> dict[bytes, bytes]:
     authorization = b64encode(
         b":".join((username.encode("utf8"), password.encode("utf8")))
```

### Comparing `synapse_token_authenticator-0.4.6/tests/__init__.py` & `synapse_token_authenticator-0.5.0/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,31 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import base64
-import json
+import logging
 import time
 from typing import Any
 from unittest.mock import AsyncMock, Mock, patch
+from urllib.parse import parse_qs
 
 from jwcrypto import jwk, jwt
 from synapse.server import HomeServer
 from synapse.util import Clock
 from twisted.internet.testing import MemoryReactor
 from typing_extensions import override
 
 import tests.unittest as synapsetest
 from tests.test_utils import FakeResponse as Response
 
 admins = {}
+logger = logging.getLogger(__name__)
 
 
 class ModuleApiTestCase(synapsetest.HomeserverTestCase):
     @classmethod
     def setUpClass(cls):
         async def set_user_admin(user_id: str, admin: bool):
             return admins.update({user_id: admin})
@@ -177,23 +179,23 @@
             }
         )
     else:
         return Response(code=404)
 
 
 def mock_idp_post(uri, data_raw, **kwargs):
-    data = json.loads(data_raw)
+    query = data_raw.decode()
+    data = parse_qs(query)
     hostname = "https://idp.example.test"
-
     if uri == f"{hostname}/oauth/v2/introspect":
         # Fail if no access token is provided
         if data is None:
             return Response(code=401)
         # Fail if access token is incorrect
-        if data["token"] != "zitadel_access_token":
+        if data.get("token")[0] != "zitadel_access_token":
             return Response(code=401)
 
         return Response.json(
             payload={
                 "active": True,
                 "iss": hostname,
                 "localpart": "alice",
```

### Comparing `synapse_token_authenticator-0.4.6/tests/server.py` & `synapse_token_authenticator-0.5.0/tests/server.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.6/tests/test_custom.py` & `synapse_token_authenticator-0.5.0/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.6/tests/test_jwt.py` & `synapse_token_authenticator-0.5.0/tests/test_jwt.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.6/tests/test_oidc.py` & `synapse_token_authenticator-0.5.0/tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.6/tests/unittest.py` & `synapse_token_authenticator-0.5.0/tests/unittest.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.6/tests/utils.py` & `synapse_token_authenticator-0.5.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.6/tests/test_utils/__init__.py` & `synapse_token_authenticator-0.5.0/tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.6/tests/test_utils/html_parsers.py` & `synapse_token_authenticator-0.5.0/tests/test_utils/html_parsers.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.6/tests/test_utils/logging_setup.py` & `synapse_token_authenticator-0.5.0/tests/test_utils/logging_setup.py`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.6/LICENSE` & `synapse_token_authenticator-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synapse_token_authenticator-0.4.6/README.md` & `synapse_token_authenticator-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,16 @@
   # Algorithm of the tokens, defaults to HS512 (optional)
   algorithm: HS512
   # Allow registration of new users, defaults to false (optional)
   allow_registration: false
   # Require tokens to have an expiry set, defaults to true (optional)
   require_expiry: true
 oidc:
-  issuer: "https://idp.example.com"
+  # Include trailing slash
+  issuer: "https://idp.example.com/"
   client_id: "<IDP client id>"
   client_secret: "<IDP client secret>"
   # Zitadel Organization ID, used for masking. (Optional)
   organization_id: 1234
   # Zitadel Project ID, used for validating the audience of the returned token.
   project_id: 5678
   # Limits access to specified clients. Allows any client if not set (optional)
```

### Comparing `synapse_token_authenticator-0.4.6/pyproject.toml` & `synapse_token_authenticator-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["jwcrypto", "twisted"]
-version = "0.4.6"
+version = "0.5.0"
 
 [project.urls]
 Documentation = "https://github.com/famedly/synapse-token-authenticator"
 Issues = "https://github.com/famedly/synapse-token-authenticator/issues"
 Source = "https://github.com/famedly/synapse-token-authenticator"
 
 [tool.hatch.envs.default]
```

### Comparing `synapse_token_authenticator-0.4.6/PKG-INFO` & `synapse_token_authenticator-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: synapse-token-authenticator
-Version: 0.4.6
+Version: 0.5.0
 Summary: Synapse authentication module which allows for authenticating and registering using JWTs
 Project-URL: Documentation, https://github.com/famedly/synapse-token-authenticator
 Project-URL: Issues, https://github.com/famedly/synapse-token-authenticator/issues
 Project-URL: Source, https://github.com/famedly/synapse-token-authenticator
 Author-email: Sorunome <mail@sorunome.de>, Amanda Graven <amanda@graven.dev>, Jan Christian Grünhage <jan.christian@gruenhage.xyz>
 License-Expression: AGPL-3.0-only
 License-File: LICENSE
@@ -55,15 +55,16 @@
   # Algorithm of the tokens, defaults to HS512 (optional)
   algorithm: HS512
   # Allow registration of new users, defaults to false (optional)
   allow_registration: false
   # Require tokens to have an expiry set, defaults to true (optional)
   require_expiry: true
 oidc:
-  issuer: "https://idp.example.com"
+  # Include trailing slash
+  issuer: "https://idp.example.com/"
   client_id: "<IDP client id>"
   client_secret: "<IDP client secret>"
   # Zitadel Organization ID, used for masking. (Optional)
   organization_id: 1234
   # Zitadel Project ID, used for validating the audience of the returned token.
   project_id: 5678
   # Limits access to specified clients. Allows any client if not set (optional)
```

