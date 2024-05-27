# Comparing `tmp/schwab_api_wrapper-0.0.9.tar.gz` & `tmp/schwab_api_wrapper-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab_api_wrapper-0.0.9.tar", last modified: Mon May 27 15:06:37 2024, max compression
+gzip compressed data, was "schwab_api_wrapper-0.1.0.tar", last modified: Mon May 27 20:54:31 2024, max compression
```

## Comparing `schwab_api_wrapper-0.0.9.tar` & `schwab_api_wrapper-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 15:06:37.973269 schwab_api_wrapper-0.0.9/
--rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/LICENSE
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 15:06:37.973048 schwab_api_wrapper-0.0.9/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/README.md
--rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-27 15:05:58.000000 schwab_api_wrapper-0.0.9/pyproject.toml
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 15:06:37.969459 schwab_api_wrapper-0.0.9/schwab_api_wrapper/
--rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)      559 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/__main__.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 15:06:37.970861 schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/market_hours_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/price_history_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/quotes_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/response_aware_retry.py
--rw-r--r--   0 owengordon   (501) staff       (20)    36931 2024-05-26 22:26:28.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/schwab.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 15:06:37.972001 schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/accounts_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/orders_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     5497 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/transactions_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper/utils.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 15:06:37.972798 schwab_api_wrapper-0.0.9/schwab_api_wrapper.egg-info/
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 15:06:37.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)      879 2024-05-27 15:06:37.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-27 15:06:37.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-27 15:06:37.000000 schwab_api_wrapper-0.0.9/schwab_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-27 15:06:37.973318 schwab_api_wrapper-0.0.9/setup.cfg
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 15:06:37.972270 schwab_api_wrapper-0.0.9/tests/
--rw-r--r--   0 owengordon   (501) staff       (20)    45372 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.9/tests/test_schawb_api.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 20:54:31.020486 schwab_api_wrapper-0.1.0/
+-rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/LICENSE
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 20:54:31.020263 schwab_api_wrapper-0.1.0/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/README.md
+-rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-27 20:54:01.000000 schwab_api_wrapper-0.1.0/pyproject.toml
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 20:54:31.017187 schwab_api_wrapper-0.1.0/schwab_api_wrapper/
+-rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      559 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/__main__.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 20:54:31.018435 schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/market_hours_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/price_history_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/quotes_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      248 2024-05-27 20:30:46.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/oauth_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/response_aware_retry.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    37772 2024-05-27 20:45:57.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/schwab.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 20:54:31.019540 schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/accounts_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/orders_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     6225 2024-05-27 17:27:34.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/transactions_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-05-27 20:38:24.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/utils.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 20:54:31.020046 schwab_api_wrapper-0.1.0/schwab_api_wrapper.egg-info/
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 20:54:31.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)      915 2024-05-27 20:54:31.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-27 20:54:31.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-27 20:54:31.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-27 20:54:31.020533 schwab_api_wrapper-0.1.0/setup.cfg
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 20:54:31.019836 schwab_api_wrapper-0.1.0/tests/
+-rw-r--r--   0 owengordon   (501) staff       (20)    46341 2024-05-27 20:52:23.000000 schwab_api_wrapper-0.1.0/tests/test_schawb_api.py
```

### Comparing `schwab_api_wrapper-0.0.9/LICENSE` & `schwab_api_wrapper-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.9/PKG-INFO` & `schwab_api_wrapper-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.0.9
+Version: 0.1.0
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.0.9/pyproject.toml` & `schwab_api_wrapper-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schwab_api_wrapper"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Owen Gordon", email="owengordon330@outlook.com" },
 ]
 description = "A wrapper package around the schwab http api"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `schwab_api_wrapper-0.0.9/schwab_api_wrapper/__main__.py` & `schwab_api_wrapper-0.1.0/schwab_api_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/errors_schema.py` & `schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/errors_schema.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/market_hours_schemas.py` & `schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/market_hours_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/price_history_schemas.py` & `schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/price_history_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.9/schwab_api_wrapper/market_data/quotes_schemas.py` & `schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/quotes_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.9/schwab_api_wrapper/response_aware_retry.py` & `schwab_api_wrapper-0.1.0/schwab_api_wrapper/response_aware_retry.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.9/schwab_api_wrapper/schwab.py` & `schwab_api_wrapper-0.1.0/schwab_api_wrapper/schwab.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,24 @@
     TransactionResponse,
     Transaction,
     TransactionType,
 )
 from .trader_api.orders_schemas import Order, OrderRequest, PreviewOrder, OrderResponse
 from .trader_api.errors_schema import AccountsAndTradingError
 
+from .oauth_schemas import Token, OAuthError
+
+
+class OAuthException(Exception):
+    def __init__(self, title, error: OAuthError):
+        super().__init__(title)
+        self.title = title
+        self.error = error
+
+
 
 # TODO if the response doesn't have a .json() field it will error at us
 # I think we just let it fail in this case because pydantic verification will fail anyways too
 # Either this or we specifically check for a missing json field in an otherwise well-formed response
 
 
 class SchwabAPI:
@@ -135,15 +145,19 @@
             "Authorization": f"Bearer {self.access_token}",
         }
     
     def get_refresh_token_expiration(self) -> datetime:
         return self.refresh_token_valid_until
 
     def refresh(self):
-        token = self.refresh_access_token()
+        token, error = self.refresh_access_token()
+
+        if error is not None:
+            raise OAuthException(f"Unable to generate refresh token", error)
+        
         self.save_token(token)
 
         self.retry_session = requests.Session()
         self.retry_session.mount("http://", self.adapter)
         self.retry_session.mount("https://", self.adapter)
 
         self.session = requests.Session()
@@ -175,15 +189,15 @@
 
         logging.getLogger(__name__).debug(
             f"OAuth Authorize Response url: {response.url}"
         )
 
         return response.url
 
-    def generate_refresh_token(self, authorization_code) -> dict:
+    def generate_refresh_token(self, authorization_code) -> tuple[Optional[Token], Optional[OAuthError]]:
         # Access Token" - Request Example (CURL)
         # {curl -X POST \https://api.schwabapi.com/v1/oauth/token \-H 'Authorization: Basic {BASE64_ENCODED_Client_ID:Client_Secret} \-H 'Content-Type: application/x-www-form-urlencoded' \-d 'grant_type=authorization_code&code={AUTHORIZATION_CODE_VALUE}&redirect_uri=https://example_url.com/callback_example'}
         # Response Example (body)
         # Example - Access Token Response
         # {  "expires_in": 1800,  //Number of seconds access_token is valid for  "token_type": "Bearer",  "scope": "api",  "refresh_token": "{REFRESH_TOKEN_HERE}", //Valid for 7 days  "access_token": "{ACCESS_TOKEN_HERE}", //Valid for 30 minutes  "id_token": "{JWT_HERE}"}
 
         payload = {
@@ -202,24 +216,27 @@
             data=payload,
         )
 
         logging.getLogger(__name__).info(
             f"Schwab API | POST `{TOKEN_URL}` | Status: {response.status_code}"
         )
 
-        assert (
-            response.status_code == STATUS_CODE_OK
-        ), "Failed to obtain tokens [error code = %s]" % (response.status_code)
+        if response.status_code == STATUS_CODE_OK:
+            token = Token(**response.json())
+            logging.getLogger(__name__).debug("Response JSON:\n" + pformat(token))
 
-        logging.getLogger(__name__).debug("Response JSON:\n" + pformat(response.json()))
+            print("New Token:")
+            pprint(token)
 
-        print("New Token:")
-        pprint(response.json())
+            return token, None
+        else:
+            error = OAuthError(**response.json())
+            logging.getLogger(__name__).debug("Response JSON:\n" + pformat(error))
 
-        return response.json()
+            return None, error
 
     def renew_refresh_token(self):
 
         authorization_url = self.app_authorization()
 
         print()
         print("Authorization URL:")
@@ -229,41 +246,45 @@
         print("2. Copy the resulting redirected URL from the browser address bar")
         print()
 
         url = input("Enter resulting redirected URL here: ")
 
         authorization_code, session_id = get_code_from_url(url)
 
-        token = self.generate_refresh_token(authorization_code)
+        token, error = self.generate_refresh_token(authorization_code)
+
+        if error is not None:
+            raise OAuthException(f"Unable to generate refresh token", error)
+        
         self.save_token(token)
 
-    def save_token(self, token: dict):
-        self.refresh_token = token[KEY_TOKEN_REFRESH]  # valid for 7 days
+    def save_token(self, token: Token):
+        self.refresh_token = token.refresh_token # valid for 7 days
         self.refresh_token_valid_until = datetime.now(timezone.utc) + timedelta(
             days=7
         )  # utc time refresh token is valid until
-        self.access_token = token[KEY_TOKEN_ACCESS]  # valid for 30 minutes
+        self.access_token = token.access_token  # valid for 30 minutes
         self.access_token_valid_until = datetime.now(timezone.utc) + timedelta(
             seconds=1800
         )  # utc time when access token is invalid
-        self.id_token = token[KEY_TOKEN_ID]
+        self.id_token = token.id_token
 
         self.parameters[KEY_ACCESS_TOKEN_VALID_UNTIL] = (
             self.access_token_valid_until.isoformat()
         )
         self.parameters[KEY_REFRESH_TOKEN_VALID_UNTIL] = (
             self.refresh_token_valid_until.isoformat()
         )
 
-        self.parameters.update(token)
+        self.parameters.update(token.model_dump())
 
         with open(self.parameters_file, "w") as fin:
             json.dump(self.parameters, fin, indent=4)
 
-    def refresh_access_token(self) -> dict:
+    def refresh_access_token(self) -> tuple[Optional[Token], Optional[OAuthError]]:
         # "Refresh Token" - Request Example (cURL)
         # curl -X POST \
         #     https://api.schwabapi.com/v1/oauth/token \
         #     -H 'Authorization: Basic {BASE64_ENCODED_Client_ID:Client_Secret} \
         #     -H 'Content-Type: application/x-www-form-urlencoded' \
         #     -d 'grant_type=refresh_token&refresh_token={REFRESH_TOKEN_GENERATED_FROM_PRIOR_STEP}
         # Response Example (body)
@@ -285,21 +306,27 @@
             data=payload,
         )
 
         logging.getLogger(__name__).info(
             f"Schwab API | POST `{TOKEN_URL}` | Status: {response.status_code}"
         )
 
-        logging.getLogger(__name__).debug("Response JSON:\n" + pformat(response.json()))
+        if response.status_code == STATUS_CODE_OK:
+            token = Token(**response.json())
+            logging.getLogger(__name__).debug("Response JSON:\n" + pformat(token))
 
-        assert (
-            response.status_code == STATUS_CODE_OK
-        ), "Failed to obtain tokens [error code = %s]" % (response.status_code)
+            print("New Token:")
+            pprint(token)
+
+            return token, None
+        else:
+            error = OAuthError(**response.json())
+            logging.getLogger(__name__).debug("Response JSON:\n" + pformat(error))
 
-        return response.json()
+            return None, error
 
     def quotes(
         self,
         symbols: list[str],
         quotes_fields: Optional[list[QuotesField]] = None,
         indicative: bool = False,
         retry: bool = False,
```

### Comparing `schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/accounts_schemas.py` & `schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/accounts_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/orders_schemas.py` & `schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/orders_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.9/schwab_api_wrapper/trader_api/transactions_schemas.py` & `schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/transactions_schemas.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,23 +61,26 @@
     userId: int
     systemUserName: str
     firstName: str
     lastName: str
     brokerRepCode: str
 
 
-class AssetType(Enum):
+class AssetType(str, Enum):
     EQUITY = "EQUITY"
     OPTION = "OPTION"
     INDEX = "INDEX"
     MUTUAL_FUND = "MUTUAL_FUND"
     CASH_EQUIVALENT = "CASH_EQUIVALENT"
     FIXED_INCOME = "FIXED_INCOME"
     CURRENCY = "CURRENCY"
     COLLECTIVE_INVESTMENT = "COLLECTIVE_INVESTMENT"
+    PRODUCT = "PRODUCT"
+    FUTURE = "FUTURE"
+    FOREX = "FOREX"
 
 
 class CashEquivalentType(Enum):
     SWEEP_VEHICLE = "SWEEP_VEHICLE"
     SAVINGS = "SAVINGS"
     MONEY_MARKET_FUND = "MONEY_MARKET_FUND"
     UNKNOWN = "UNKNOWN"
@@ -89,26 +92,40 @@
     symbol: str
     description: str
     instrumentId: int
     netChange: float
     type: CashEquivalentType
 
 
+class CollectiveInvestmentType(Enum):
+    UNIT_INVESTMENT_TRUST = "UNIT_INVESTMENT_TRUST"
+    EXCHANGE_TRADED_FUND = "EXCHANGE_TRADED_FUND"
+    CLOSED_END_FUND = "CLOSED_END_FUND"
+    INDEX = "INDEX"
+    UNITS = "UNITS"
+
+
 class CollectiveInvestment(BaseModel):
-    pass
+    assetType: Literal[AssetType.COLLECTIVE_INVESTMENT]
+    cusip: str
+    symbol: str
+    description: str
+    instrumentId: int
+    netChange: float
+    type: CollectiveInvestmentType
 
 
 class Currency(BaseModel):
     assetType: Literal[AssetType.CURRENCY]
     status: str
     cusip: Optional[str] = None
     symbol: str
     description: str
-    instrumentid: int
-    netChange: Optional[float]
+    instrumentId: int
+    netChange: Optional[float] = None
     closingPrice: float
 
 
 class EquityType(Enum):
     COMMON_STOCK = "COMMON_STOCK"
     PREFERRED_STOCK = "PREFERRED_STOCK"
     DEPOSITORY_RECEIPT = "DEPOSITORY_RECEIPT"
@@ -123,49 +140,49 @@
     WHEN_ISSUED = "WHEN_ISSUED"
     UNKNOWN = "UNKNOWN"
 
 
 class TransactionEquity(BaseModel):
     assetType: Literal[AssetType.EQUITY]
     status: str
-    cusip: str
+    cusip: Optional[str] = None
     symbol: str
     description: Optional[str] = None
     instrumentId: int
     netChange: Optional[float] = None
     closingPrice: float
     type: EquityType
 
 
 class TransactionFixedIncome(BaseModel):
-    pass
+    assetType: Literal[AssetType.FIXED_INCOME]
 
 
 class Forex(BaseModel):
-    pass
+    assetType: Literal[AssetType.FOREX]
 
 
 class Future(BaseModel):
-    pass
+    assetType: Literal[AssetType.FUTURE]
 
 
 class Index(BaseModel):
-    pass
+    assetType: Literal[AssetType.INDEX]
 
 
 class TransactionMutualFund(BaseModel):
-    pass
+    assetType: Literal[AssetType.MUTUAL_FUND]
 
 
 class TransactionOption(BaseModel):
-    pass
+    assetType: Literal[AssetType.OPTION]
 
 
 class Product(BaseModel):
-    pass
+    assetType: Literal[AssetType.PRODUCT]
 
 
 TransactionInstrument = Union[
     TransactionCashEquivalent,
     CollectiveInvestment,
     Currency,
     TransactionEquity,
```

### Comparing `schwab_api_wrapper-0.0.9/schwab_api_wrapper/utils.py` & `schwab_api_wrapper-0.1.0/schwab_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.9/schwab_api_wrapper.egg-info/PKG-INFO` & `schwab_api_wrapper-0.1.0/schwab_api_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.0.9
+Version: 0.1.0
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.0.9/schwab_api_wrapper.egg-info/SOURCES.txt` & `schwab_api_wrapper-0.1.0/schwab_api_wrapper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 schwab_api_wrapper/__init__.py
 schwab_api_wrapper/__main__.py
+schwab_api_wrapper/oauth_schemas.py
 schwab_api_wrapper/response_aware_retry.py
 schwab_api_wrapper/schwab.py
 schwab_api_wrapper/utils.py
 schwab_api_wrapper.egg-info/PKG-INFO
 schwab_api_wrapper.egg-info/SOURCES.txt
 schwab_api_wrapper.egg-info/dependency_links.txt
 schwab_api_wrapper.egg-info/top_level.txt
```

### Comparing `schwab_api_wrapper-0.0.9/tests/test_schawb_api.py` & `schwab_api_wrapper-0.1.0/tests/test_schawb_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 )
 
 from schwab_api_wrapper.market_data.quotes_schemas import QuoteResponse
 from schwab_api_wrapper.market_data.errors_schema import MarketDataError
 from schwab_api_wrapper.market_data.market_hours_schemas import MarketHoursResponse
 from schwab_api_wrapper.market_data.price_history_schemas import CandleList
 
-from schwab_api_wrapper.schwab import SchwabAPI
+from schwab_api_wrapper.schwab import SchwabAPI, OAuthException
 
 logging.basicConfig(level=logging.INFO)
 
 
 PARAMETERS_FILE_NAME = "fakefile.json"
 
 fake_json = {
@@ -65,14 +65,16 @@
             responses.POST,
             TOKEN_URL,
             json={
                 KEY_TOKEN_ACCESS: "new_access_token",
                 KEY_TTL: 1800,
                 KEY_TOKEN_REFRESH: "new_refresh_token",
                 KEY_TOKEN_ID: "new_id_token",
+                "scope": "api",
+                "token_type": "Bearer"
             },
             status=200,
         )
 
         # Call the method under test
         self.api.refresh()
 
@@ -81,14 +83,35 @@
         self.assertEqual(self.api.refresh_token, "new_refresh_token")
         self.assertEqual(self.api.id_token, "new_id_token")
         self.assertLess(
             self.api.access_token_valid_until,
             datetime.now(timezone.utc) + timedelta(minutes=30),
         )
 
+    @patch("builtins.open", new_callable=mock_open, read_data=json.dumps(fake_json))
+    @responses.activate
+    def test_refresh_token_failure(self, mock_file):
+        # Mock the HTTP POST response for a successful token refresh
+        # Set up the mock response
+        responses.add(
+            responses.POST,
+            TOKEN_URL,
+            json={
+                'error': 'unsupported_token_type',
+                'error_description': (
+                    '400 Bad Request: "{"error_description":"Exception while authenticating refresh token [tokenDigest=******, Exception=Failed refresh token authentication [tokenDigest=******]]","error":"refresh_token_authentication_error"}"'
+                )
+            },
+            status=400,
+        )
+
+        with self.assertRaises(OAuthException):
+            # Call the method under test
+            self.api.refresh()
+
     @responses.activate
     def test_account_numbers_success(self):
         responses.add(
             responses.GET,
             ACCOUNT_NUMBERS_URL,
             json=[{"accountNumber": "12345", "hashValue": "abcde"}],
             status=200,
```

