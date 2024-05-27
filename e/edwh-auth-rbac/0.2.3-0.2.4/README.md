# Comparing `tmp/edwh_auth_rbac-0.2.3.tar.gz` & `tmp/edwh_auth_rbac-0.2.4.tar.gz`

## Comparing `edwh_auth_rbac-0.2.3.tar` & `edwh_auth_rbac-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/.gitignore
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/class_index.html
--rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/coverage_html_cb_da166b87.js
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/favicon_32_cb_58284776.png
--rw-r--r--   0        0        0    36695 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/function_index.html
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/keybd_closed_cb_ce680311.png
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/status.json
--rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/style_cb_8e611ae1.css
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/z_438b44bce6437be6___init___py.html
--rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/z_438b44bce6437be6_helpers_py.html
--rw-r--r--   0        0        0    15181 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/z_438b44bce6437be6_migrations_py.html
--rw-r--r--   0        0        0   123833 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/z_438b44bce6437be6_model_py.html
--rw-r--r--   0        0        0    61606 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/z_438b44bce6437be6_rbac_py.html
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/z_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0    60186 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/htmlcov/z_a44f0ac069e85531_test_rbac_py.html
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/src/edwh_auth_rbac/__init__.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/src/edwh_auth_rbac/helpers.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/src/edwh_auth_rbac/migrations.py
--rw-r--r--   0        0        0    13312 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/src/edwh_auth_rbac/model.py
--rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/src/edwh_auth_rbac/rbac.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/tests/test_migrate.py
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/tests/test_rbac.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/.gitignore
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/README.md
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/CHANGELOG.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/.gitignore
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/class_index.html
+-rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/coverage_html_cb_da166b87.js
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/favicon_32_cb_58284776.png
+-rw-r--r--   0        0        0    36695 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/function_index.html
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/keybd_closed_cb_ce680311.png
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/status.json
+-rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/style_cb_8e611ae1.css
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/z_438b44bce6437be6___init___py.html
+-rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/z_438b44bce6437be6_helpers_py.html
+-rw-r--r--   0        0        0    15181 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/z_438b44bce6437be6_migrations_py.html
+-rw-r--r--   0        0        0   123833 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/z_438b44bce6437be6_model_py.html
+-rw-r--r--   0        0        0    61606 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/z_438b44bce6437be6_rbac_py.html
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/z_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0    60186 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/htmlcov/z_a44f0ac069e85531_test_rbac_py.html
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/src/edwh_auth_rbac/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/src/edwh_auth_rbac/helpers.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/src/edwh_auth_rbac/migrations.py
+-rw-r--r--   0        0        0    13401 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/src/edwh_auth_rbac/model.py
+-rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/src/edwh_auth_rbac/rbac.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/tests/test_migrate.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/tests/test_rbac.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/.gitignore
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/README.md
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.4/PKG-INFO
```

### Comparing `edwh_auth_rbac-0.2.3/CHANGELOG.md` & `edwh_auth_rbac-0.2.4/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.2.4 (2024-05-27)
+
+### Fix
+
+* Is_uuid now says True if the value already is a uuid.UUID; -> fixes `member_of` behavior ([`5030797`](https://github.com/educationwarehouse/edwh-auth-rbac/commit/503079711fb2613c4df900020fc6625c94373d0b))
+
 ## v0.2.3 (2024-05-27)
 
 
 
 ## v0.2.3 (2024-05-27)
 
 ### Fix
```

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/class_index.html` & `edwh_auth_rbac-0.2.4/htmlcov/class_index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/coverage_html_cb_da166b87.js` & `edwh_auth_rbac-0.2.4/htmlcov/coverage_html_cb_da166b87.js`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/favicon_32_cb_58284776.png` & `edwh_auth_rbac-0.2.4/htmlcov/favicon_32_cb_58284776.png`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/function_index.html` & `edwh_auth_rbac-0.2.4/htmlcov/function_index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/index.html` & `edwh_auth_rbac-0.2.4/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/keybd_closed_cb_ce680311.png` & `edwh_auth_rbac-0.2.4/htmlcov/keybd_closed_cb_ce680311.png`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/status.json` & `edwh_auth_rbac-0.2.4/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/style_cb_8e611ae1.css` & `edwh_auth_rbac-0.2.4/htmlcov/style_cb_8e611ae1.css`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/z_438b44bce6437be6___init___py.html` & `edwh_auth_rbac-0.2.4/htmlcov/z_438b44bce6437be6___init___py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/z_438b44bce6437be6_helpers_py.html` & `edwh_auth_rbac-0.2.4/htmlcov/z_438b44bce6437be6_helpers_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/z_438b44bce6437be6_migrations_py.html` & `edwh_auth_rbac-0.2.4/htmlcov/z_438b44bce6437be6_migrations_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/z_438b44bce6437be6_model_py.html` & `edwh_auth_rbac-0.2.4/htmlcov/z_438b44bce6437be6_model_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/z_438b44bce6437be6_rbac_py.html` & `edwh_auth_rbac-0.2.4/htmlcov/z_438b44bce6437be6_rbac_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/z_a44f0ac069e85531___init___py.html` & `edwh_auth_rbac-0.2.4/htmlcov/z_a44f0ac069e85531___init___py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/htmlcov/z_a44f0ac069e85531_test_rbac_py.html` & `edwh_auth_rbac-0.2.4/htmlcov/z_a44f0ac069e85531_test_rbac_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/src/edwh_auth_rbac/migrations.py` & `edwh_auth_rbac-0.2.4/src/edwh_auth_rbac/migrations.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/src/edwh_auth_rbac/model.py` & `edwh_auth_rbac-0.2.4/src/edwh_auth_rbac/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,45 +54,49 @@
 
     @classmethod
     def encode(cls, password: str) -> str:
         salt = uuid.uuid4().hex
         return salt + ":" + cls.hmac_hash(value=password, key="secret_start", salt=salt)
 
 
-def is_uuid(s) -> bool:
+def is_uuid(s: str | UUID) -> bool:
+    if isinstance(s, UUID):
+        return True
+
     try:
         UUID(s)
         return True
-    except Exception:
+    except Exception as e:
         return False
 
 
 def key_lookup_query(db: DAL, identity_key: IdentityKey, object_type: Optional[ObjectTypes] = None) -> Query:
     if "@" in str(identity_key):
         query = db.identity.email == str(identity_key).lower()
     elif isinstance(identity_key, int):
         query = db.identity.id == identity_key
     elif is_uuid(identity_key):
         query = db.identity.object_id == str(identity_key).lower()
     else:
+        # @remco: why??
         query = db.identity.firstname == identity_key
 
     if object_type:
         query &= db.identity.object_type == object_type
 
     return query
 
 
 def key_lookup(db: DAL, identity_key: IdentityKey, object_type: Optional[ObjectTypes] = None) -> str:
     query = key_lookup_query(db, identity_key, object_type)
 
     rowset = db(query).select(db.identity.object_id)
 
     if len(rowset) != 1:
-        raise ValueError("Keep lookup for {} returned {} results.".format(identity_key, len(rowset)))
+        raise ValueError("Key lookup for {} returned {} results.".format(identity_key, len(rowset)))
 
     return rowset.first().object_id
 
 
 my_datetime = SQLCustomType(
     type="string", native="char(35)", encoder=(lambda x: x.isoformat(" ")), decoder=(lambda x: dateutil.parser.parse(x))
 )
```

### Comparing `edwh_auth_rbac-0.2.3/src/edwh_auth_rbac/rbac.py` & `edwh_auth_rbac-0.2.4/src/edwh_auth_rbac/rbac.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/tests/test_migrate.py` & `edwh_auth_rbac-0.2.4/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.3/tests/test_rbac.py` & `edwh_auth_rbac-0.2.4/tests/test_rbac.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,18 +66,23 @@
 
     def test_user_creation(self, rbac, store):
         store.remco = rbac.add_user("remco@test.nl", "remco", "remco test", "secret", [])["object_id"]
         store.pietje = rbac.add_user("pietje@test.nl", "pietje", "pietje test", "secret", [])["object_id"]
         store.truus = rbac.add_user("truus@test.nl", "truus", "truus test", "secret", [])["object_id"]
 
     def test_group_creation(self, rbac, store):
-        store.articles = rbac.add_group("articles@test.nl", "articles", [])["object_id"]
-        store.all = rbac.add_group("all@test.nl", "all", [])["object_id"]
-        store.users = rbac.add_group("users@test.nl", "users", [])["object_id"]
-        store.admins = rbac.add_group("admins@test.nl", "admins", [])["object_id"]
+        store.groups = rbac.add_group("groups@test.nl", "groups", [])["object_id"]
+
+        store.articles = rbac.add_group("articles@test.nl", "articles", [store.groups])["object_id"]
+        store.all = rbac.add_group("all@test.nl", "all", [store.groups])["object_id"]
+        store.users = rbac.add_group("users@test.nl", "users", [store.groups])["object_id"]
+        store.admins = rbac.add_group("admins@test.nl", "admins", [store.groups])["object_id"]
+
+        assert rbac.has_membership(store.admins, store.groups)
+        assert not rbac.has_membership(store.groups, store.admins)
 
     def test_item_creation(self, rbac, store):
         for name in "abcde":
             store[name] = rbac.add_user("article_" + name + "@test.nl", name, "article", "", [])["object_id"]
 
     def test_stash_users_in_groups(self, rbac, store):
         rbac.add_membership(store.remco, store.admins)
```

### Comparing `edwh_auth_rbac-0.2.3/pyproject.toml` & `edwh_auth_rbac-0.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "edwh",
     "edwh-migrate",
     "hatch",
     "python-semantic-release<8",
     "black",
     "su6[all]",
     "testcontainers",
+    "requests<2.32", # 2.32 breaks testcontainers
 ]
 
 [project.urls]
 Documentation = "https://github.com/educationwarehouse/edwh-auth-rbac#readme"
 Issues = "https://github.com/educationwarehouse/edwh-auth-rbac/issues"
 Source = "https://github.com/educationwarehouse/edwh-auth-rbac"
 
@@ -87,8 +88,8 @@
 [tool.isort]
 profile = "black"
 extend_skip_glob = ["venv*"]
 
 [tool.pytest.ini_options]
 pythonpath = [
     "src",
-]
+]
```

### Comparing `edwh_auth_rbac-0.2.3/PKG-INFO` & `edwh_auth_rbac-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: edwh-auth-rbac
-Version: 0.2.3
+Version: 0.2.4
 Summary: Recursive Memberships and Permissions for the Education Warehouse Authentication System
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-auth-rbac#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-auth-rbac/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-auth-rbac
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 Keywords: edwh,omgeving,whitelabel
@@ -18,14 +18,15 @@
 Requires-Dist: pydal
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: edwh; extra == 'dev'
 Requires-Dist: edwh-migrate; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: python-semantic-release<8; extra == 'dev'
+Requires-Dist: requests<2.32; extra == 'dev'
 Requires-Dist: su6[all]; extra == 'dev'
 Requires-Dist: testcontainers; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # EDWH Auth RBAC
 
 Role-Based Access Control with recursive memberships
```

