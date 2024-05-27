# Comparing `tmp/infisical_python-2.2.0.tar.gz` & `tmp/infisical_python-2.2.1.tar.gz`

## Comparing `infisical_python-2.2.0.tar` & `infisical_python-2.2.1.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 infisical_python-2.2.0/local_dependencies/infisical/Cargo.toml
--rw-r--r--   0     1001      127     3901 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/aws_iam_login.rs
--rw-r--r--   0     1001      127     3895 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/gcp_iam_login.rs
--rw-r--r--   0     1001      127     1814 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/gcp_id_token_login.rs
--rw-r--r--   0     1001      127     1826 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/kubernetes_login.rs
--rw-r--r--   0     1001      127     3734 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/mod.rs
--rw-r--r--   0     1001      127     1807 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/universal_auth_login.rs
--rw-r--r--   0     1001      127     1943 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/mod.rs
--rw-r--r--   0     1001      127     2311 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/create_secret.rs
--rw-r--r--   0     1001      127     1907 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/delete_secret.rs
--rw-r--r--   0     1001      127     2590 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/get_secret.rs
--rw-r--r--   0     1001      127     3754 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/list_secrets.rs
--rw-r--r--   0     1001      127      111 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/mod.rs
--rw-r--r--   0     1001      127     1733 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/update_secret.rs
--rw-r--r--   0     1001      127      830 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/auth/authenticate.rs
--rw-r--r--   0     1001      127      125 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/auth/mod.rs
--rw-r--r--   0     1001      127     4966 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/cache.rs
--rw-r--r--   0     1001      127     8184 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/client/auth_method_settings.rs
--rw-r--r--   0     1001      127     1977 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/client/client.rs
--rw-r--r--   0     1001      127     2006 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/client/client_settings.rs
--rw-r--r--   0     1001      127       91 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/client/mod.rs
--rw-r--r--   0     1001      127     1135 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/constants.rs
--rw-r--r--   0     1001      127     5797 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/error.rs
--rw-r--r--   0     1001      127     8314 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/helper.rs
--rw-r--r--   0     1001      127      159 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/lib.rs
--rw-r--r--   0     1001      127     1144 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/client_cryptography.rs
--rw-r--r--   0     1001      127     1894 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/client_secrets.rs
--rw-r--r--   0     1001      127      708 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/cryptography/create_symmetric_key.rs
--rw-r--r--   0     1001      127     2519 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/cryptography/decrypt_symmetric.rs
--rw-r--r--   0     1001      127     2405 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/cryptography/encrypt_symmetric.rs
--rw-r--r--   0     1001      127      335 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/cryptography/mod.rs
--rw-r--r--   0     1001      127       93 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/mod.rs
--rw-r--r--   0     1001      127     1365 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/create.rs
--rw-r--r--   0     1001      127     1092 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/delete.rs
--rw-r--r--   0     1001      127      985 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/get.rs
--rw-r--r--   0     1001      127     1071 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/list.rs
--rw-r--r--   0     1001      127      979 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/mod.rs
--rw-r--r--   0     1001      127     1201 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/update.rs
--rw-r--r--   0     1001      127     4361 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/tests/cryptography.rs
--rw-r--r--   0     1001      127    11199 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical/tests/secrets.rs
--rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 infisical_python-2.2.0/local_dependencies/infisical-json/Cargo.toml
--rw-r--r--   0     1001      127     2314 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical-json/src/client.rs
--rw-r--r--   0     1001      127     1122 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical-json/src/command.rs
--rw-r--r--   0     1001      127       51 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical-json/src/lib.rs
--rw-r--r--   0     1001      127     1788 2024-05-25 17:01:55.000000 infisical_python-2.2.0/local_dependencies/infisical-json/src/response.rs
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 infisical_python-2.2.0/Cargo.toml
--rw-r--r--   0     1001      127     1053 2024-05-25 17:01:55.000000 infisical_python-2.2.0/LICENSE
--rw-r--r--   0     1001      127       43 2024-05-25 17:01:55.000000 infisical_python-2.2.0/MANIFEST.in
--rw-r--r--   0     1001      127      502 2024-05-25 17:01:55.000000 infisical_python-2.2.0/README.md
--rw-r--r--   0     1001      127      894 2024-05-25 17:01:55.000000 infisical_python-2.2.0/example.py
--rw-r--r--   0     1001      127     1198 2024-05-25 17:02:00.000000 infisical_python-2.2.0/infisical_client/__init__.py
--rw-r--r--   0     1001      127     3814 2024-05-25 17:01:55.000000 infisical_python-2.2.0/infisical_client/infisical_client.py
--rw-r--r--   0     1001      127     2123 2024-05-25 17:01:59.000000 infisical_python-2.2.0/pyproject.toml
--rw-r--r--   0     1001      127      938 2024-05-25 17:01:55.000000 infisical_python-2.2.0/src/client.rs
--rw-r--r--   0     1001      127      104 2024-05-25 17:01:55.000000 infisical_python-2.2.0/src/lib.rs
--rw-r--r--   0     1001      127      189 2024-05-25 17:01:55.000000 infisical_python-2.2.0/src/python_module.rs
--rw-r--r--   0        0        0    80967 2024-05-25 17:02:48.000000 infisical_python-2.2.0/Cargo.lock
--rw-r--r--   0     1001      127    47505 2024-05-25 17:02:01.000000 infisical_python-2.2.0/infisical_client/schemas.py
--rw-r--r--   0        0        0     1999 1970-01-01 00:00:00.000000 infisical_python-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 infisical_python-2.2.1/local_dependencies/infisical/Cargo.toml
+-rw-r--r--   0     1001      127     3901 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/api/auth/aws_iam_login.rs
+-rw-r--r--   0     1001      127     1762 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/api/auth/azure_login.rs
+-rw-r--r--   0     1001      127     3895 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/api/auth/gcp_iam_login.rs
+-rw-r--r--   0     1001      127     1814 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/api/auth/gcp_id_token_login.rs
+-rw-r--r--   0     1001      127     1826 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/api/auth/kubernetes_login.rs
+-rw-r--r--   0     1001      127     4532 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/api/auth/mod.rs
+-rw-r--r--   0     1001      127     1807 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/api/auth/universal_auth_login.rs
+-rw-r--r--   0     1001      127     1943 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/api/mod.rs
+-rw-r--r--   0     1001      127     2311 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/api/secrets/create_secret.rs
+-rw-r--r--   0     1001      127     1907 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/api/secrets/delete_secret.rs
+-rw-r--r--   0     1001      127     2590 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/api/secrets/get_secret.rs
+-rw-r--r--   0     1001      127     3754 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/api/secrets/list_secrets.rs
+-rw-r--r--   0     1001      127      111 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/api/secrets/mod.rs
+-rw-r--r--   0     1001      127     1733 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/api/secrets/update_secret.rs
+-rw-r--r--   0     1001      127      830 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/auth/authenticate.rs
+-rw-r--r--   0     1001      127      125 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/auth/mod.rs
+-rw-r--r--   0     1001      127     4966 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/cache.rs
+-rw-r--r--   0     1001      127     9377 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/client/auth_method_settings.rs
+-rw-r--r--   0     1001      127     1977 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/client/client.rs
+-rw-r--r--   0     1001      127     2006 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/client/client_settings.rs
+-rw-r--r--   0     1001      127       91 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/client/mod.rs
+-rw-r--r--   0     1001      127     1456 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/constants.rs
+-rw-r--r--   0     1001      127     5797 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/error.rs
+-rw-r--r--   0     1001      127     8224 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/helper.rs
+-rw-r--r--   0     1001      127      159 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/lib.rs
+-rw-r--r--   0     1001      127     1144 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/manager/client_cryptography.rs
+-rw-r--r--   0     1001      127     1894 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/manager/client_secrets.rs
+-rw-r--r--   0     1001      127      708 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/manager/cryptography/create_symmetric_key.rs
+-rw-r--r--   0     1001      127     2519 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/manager/cryptography/decrypt_symmetric.rs
+-rw-r--r--   0     1001      127     2405 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/manager/cryptography/encrypt_symmetric.rs
+-rw-r--r--   0     1001      127      335 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/manager/cryptography/mod.rs
+-rw-r--r--   0     1001      127       93 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/manager/mod.rs
+-rw-r--r--   0     1001      127     1365 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/manager/secrets/create.rs
+-rw-r--r--   0     1001      127     1092 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/manager/secrets/delete.rs
+-rw-r--r--   0     1001      127      985 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/manager/secrets/get.rs
+-rw-r--r--   0     1001      127     1071 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/manager/secrets/list.rs
+-rw-r--r--   0     1001      127      979 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/manager/secrets/mod.rs
+-rw-r--r--   0     1001      127     1201 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/src/manager/secrets/update.rs
+-rw-r--r--   0     1001      127     4386 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/tests/cryptography.rs
+-rw-r--r--   0     1001      127    11199 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical/tests/secrets.rs
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 infisical_python-2.2.1/local_dependencies/infisical-json/Cargo.toml
+-rw-r--r--   0     1001      127     2314 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical-json/src/client.rs
+-rw-r--r--   0     1001      127     1122 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical-json/src/command.rs
+-rw-r--r--   0     1001      127       51 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical-json/src/lib.rs
+-rw-r--r--   0     1001      127     1788 2024-05-27 16:54:53.000000 infisical_python-2.2.1/local_dependencies/infisical-json/src/response.rs
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 infisical_python-2.2.1/Cargo.toml
+-rw-r--r--   0     1001      127     1053 2024-05-27 16:54:53.000000 infisical_python-2.2.1/LICENSE
+-rw-r--r--   0     1001      127       43 2024-05-27 16:54:53.000000 infisical_python-2.2.1/MANIFEST.in
+-rw-r--r--   0     1001      127      502 2024-05-27 16:54:53.000000 infisical_python-2.2.1/README.md
+-rw-r--r--   0     1001      127      894 2024-05-27 16:54:53.000000 infisical_python-2.2.1/example.py
+-rw-r--r--   0     1001      127     1254 2024-05-27 16:54:55.000000 infisical_python-2.2.1/infisical_client/__init__.py
+-rw-r--r--   0     1001      127     3814 2024-05-27 16:54:53.000000 infisical_python-2.2.1/infisical_client/infisical_client.py
+-rw-r--r--   0     1001      127     2123 2024-05-27 16:54:55.000000 infisical_python-2.2.1/pyproject.toml
+-rw-r--r--   0     1001      127      938 2024-05-27 16:54:53.000000 infisical_python-2.2.1/src/client.rs
+-rw-r--r--   0     1001      127      104 2024-05-27 16:54:53.000000 infisical_python-2.2.1/src/lib.rs
+-rw-r--r--   0     1001      127      189 2024-05-27 16:54:53.000000 infisical_python-2.2.1/src/python_module.rs
+-rw-r--r--   0        0        0    80967 2024-05-27 16:55:40.000000 infisical_python-2.2.1/Cargo.lock
+-rw-r--r--   0     1001      127    48286 2024-05-27 16:54:56.000000 infisical_python-2.2.1/infisical_client/schemas.py
+-rw-r--r--   0        0        0     1999 1970-01-01 00:00:00.000000 infisical_python-2.2.1/PKG-INFO
```

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/Cargo.toml` & `infisical_python-2.2.1/local_dependencies/infisical/Cargo.toml`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/aws_iam_login.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/api/auth/aws_iam_login.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/gcp_iam_login.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/api/auth/gcp_iam_login.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/gcp_id_token_login.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/api/auth/gcp_id_token_login.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/kubernetes_login.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/api/auth/kubernetes_login.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/mod.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/api/auth/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 use crate::{
     error::{Error, Result},
     Client,
 };
 
 pub mod aws_iam_login;
+pub mod azure_login;
 pub mod gcp_iam_login;
 pub mod gcp_id_token_login;
 pub mod kubernetes_login;
 pub mod universal_auth_login;
 
 fn base64_encode(plain: String) -> String {
     return base64::engine::general_purpose::STANDARD.encode(plain);
@@ -51,14 +52,40 @@
             client.site_url.clone()
         ))
         .header(reqwest::header::ACCEPT, "application/json")
         .header(reqwest::header::USER_AGENT, client.user_agent.clone());
 
     let mut body = HashMap::new();
     body.insert("identityId", identity_id);
+    body.insert("jwt", jwt);
+
+    let response = request.form(&body).send().await?;
+
+    return Ok(response);
+}
+
+pub(self) async fn auth_infisical_azure(
+    client: &mut Client,
+    identity_id: Option<String>,
+    jwt: Option<String>,
+) -> Result<reqwest::Response> {
+    let request_client = reqwest::Client::builder()
+        .use_preconfigured_tls(rustls_platform_verifier::tls_config())
+        .build()?;
+
+    let request = request_client
+        .post(format!(
+            "{}/api/v1/auth/azure-auth/login",
+            client.site_url.clone()
+        ))
+        .header(reqwest::header::ACCEPT, "application/json")
+        .header(reqwest::header::USER_AGENT, client.user_agent.clone());
+
+    let mut body = HashMap::new();
+    body.insert("identityId", identity_id);
     body.insert("jwt", jwt);
 
     let response = request.form(&body).send().await?;
 
     return Ok(response);
 }
```

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/api/auth/universal_auth_login.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/api/auth/universal_auth_login.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/api/mod.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/api/mod.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/create_secret.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/api/secrets/create_secret.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/delete_secret.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/api/secrets/delete_secret.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/get_secret.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/api/secrets/get_secret.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/list_secrets.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/api/secrets/list_secrets.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/api/secrets/update_secret.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/api/secrets/update_secret.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/auth/authenticate.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/auth/authenticate.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/cache.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/cache.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/client/auth_method_settings.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/client/auth_method_settings.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use log::debug;
 use schemars::JsonSchema;
 use serde::{Deserialize, Serialize};
 
 use crate::constants::{
-    INFISICAL_AWS_IAM_IDENTITY_ID_ENV_NAME, INFISICAL_GCP_AUTH_IDENTITY_ID_ENV_NAME,
+    INFISICAL_AWS_IAM_AUTH_IDENTITY_ID_ENV_NAME, INFISICAL_AZURE_AUTH_IDENTITY_ID_ENV_NAME,
+    INFISICAL_GCP_AUTH_IDENTITY_ID_ENV_NAME,
     INFISICAL_GCP_IAM_SERVICE_ACCOUNT_KEY_FILE_PATH_ENV_NAME,
     INFISICAL_KUBERNETES_IDENTITY_ID_ENV_NAME,
     INFISICAL_KUBERNETES_SERVICE_ACCOUNT_TOKEN_PATH_ENV_NAME,
     INFISICAL_UNIVERSAL_AUTH_CLIENT_ID_ENV_NAME, INFISICAL_UNIVERSAL_AUTH_CLIENT_SECRET_ENV_NAME,
 };
 
 fn default_kubernetes_service_account_token_path() -> Option<String> {
@@ -51,48 +52,60 @@
 pub struct KubernetesAuthMethod {
     #[schemars(
         description = "The Infisical Identity ID that you want to authenticate to Infisical with."
     )]
     pub identity_id: String,
 
     #[schemars(
-        description = "The path to the Kubernetes Service Account token file.\n\n This is usually located at /var/run/secrets/kubernetes.io/serviceaccount/token."
+        description = "The path to the Kubernetes Service Account token file.\n\nIf no path is provided, it will default to /var/run/secrets/kubernetes.io/serviceaccount/token."
     )]
     #[serde(default = "default_kubernetes_service_account_token_path")]
     pub service_account_token_path: Option<String>,
 }
 
 #[derive(Serialize, Deserialize, Debug, JsonSchema)]
+#[serde(rename_all = "camelCase")]
+pub struct AzureAuthMethod {
+    #[schemars(
+        description = "The Infisical Identity ID that you want to authenticate to Infisical with."
+    )]
+    pub identity_id: String,
+}
+
+#[derive(Serialize, Deserialize, Debug, JsonSchema)]
 #[serde(default, rename_all = "camelCase")]
 pub struct AuthenticationOptions {
     pub access_token: Option<String>,
     pub universal_auth: Option<UniversalAuthMethod>,
     pub kubernetes: Option<KubernetesAuthMethod>,
+    pub azure: Option<AzureAuthMethod>,
     pub gcp_id_token: Option<GCPIdTokenAuthMethod>,
     pub gcp_iam: Option<GCPIamAuthMethod>,
     pub aws_iam: Option<AWSIamAuthMethod>,
 }
 
 impl Default for AuthenticationOptions {
     fn default() -> Self {
         Self {
             access_token: None,
             universal_auth: None,
             gcp_id_token: None,
             gcp_iam: None,
             aws_iam: None,
             kubernetes: None,
+            azure: None,
         }
     }
 }
 
 #[derive(Debug)]
 pub enum AuthMethod {
     UniversalAuth,
     Kubernetes,
+    Azure,
     GcpIdToken,
     GcpIam,
     AwsIam,
 }
 
 // Custom validation to ensure that if universal_auth or gcp_auth are present, their fields are populated
 impl AuthenticationOptions {
@@ -128,38 +141,52 @@
         }
         // KUBERNETES AUTH:
         else if let Some(ref auth) = self.kubernetes {
             if !auth.identity_id.is_empty() {
                 return Ok(AuthMethod::Kubernetes);
             }
             return Err("kubernetes auth is present but identity_id is empty".into());
+
+        // AZURE AUTH:
+        } else if let Some(ref auth) = self.azure {
+            if !auth.identity_id.is_empty() {
+                return Ok(AuthMethod::Azure);
+            }
+            return Err("azure auth is present but identity_id is empty".into());
         } else {
             debug!("No authentication method is set. Checking environment variables.");
 
+            // universal auth env's
             let universal_auth_client_id_env =
                 std::env::var(INFISICAL_UNIVERSAL_AUTH_CLIENT_ID_ENV_NAME).unwrap_or_default();
             let universal_auth_client_secret_env =
                 std::env::var(INFISICAL_UNIVERSAL_AUTH_CLIENT_SECRET_ENV_NAME).unwrap_or_default();
 
+            // gcp auth env's
             let gcp_auth_identity_id_env =
                 std::env::var(INFISICAL_GCP_AUTH_IDENTITY_ID_ENV_NAME).unwrap_or_default();
-
             let gcp_iam_service_account_key_file_path_env =
                 std::env::var(INFISICAL_GCP_IAM_SERVICE_ACCOUNT_KEY_FILE_PATH_ENV_NAME)
                     .unwrap_or_default();
 
+            // aws iam auth env's
             let aws_iam_identity_id_env =
-                std::env::var(INFISICAL_AWS_IAM_IDENTITY_ID_ENV_NAME).unwrap_or_default();
+                std::env::var(INFISICAL_AWS_IAM_AUTH_IDENTITY_ID_ENV_NAME).unwrap_or_default();
 
+            // kubernetes auth env's
             let kubernetes_identity_id_env =
                 std::env::var(INFISICAL_KUBERNETES_IDENTITY_ID_ENV_NAME).unwrap_or_default();
             let kubernetes_service_account_token_path_env =
                 std::env::var(INFISICAL_KUBERNETES_SERVICE_ACCOUNT_TOKEN_PATH_ENV_NAME)
                     .unwrap_or_default();
 
+            // azure auth env's
+            let azure_auth_identity_id_env =
+                std::env::var(INFISICAL_AZURE_AUTH_IDENTITY_ID_ENV_NAME).unwrap_or_default();
+
             // universal auth env check
             if !universal_auth_client_id_env.is_empty()
                 && !universal_auth_client_secret_env.is_empty()
             {
                 self.universal_auth = Some(UniversalAuthMethod {
                     client_id: universal_auth_client_id_env,
                     client_secret: universal_auth_client_secret_env,
@@ -194,23 +221,30 @@
                     identity_id: gcp_auth_identity_id_env,
                 });
 
                 return Ok(AuthMethod::GcpIdToken);
             }
 
             // kubernetes auth env check
-            if !kubernetes_identity_id_env.is_empty()
-            // && !kubernetes_service_account_token_path_env.is_empty()
-            {
+            if !kubernetes_identity_id_env.is_empty() {
                 self.kubernetes = Some(KubernetesAuthMethod {
                     identity_id: kubernetes_identity_id_env,
                     service_account_token_path: Some(kubernetes_service_account_token_path_env)
                         .or(default_kubernetes_service_account_token_path()),
                 });
 
                 return Ok(AuthMethod::Kubernetes);
             }
 
+            // azure auth env check
+            if !azure_auth_identity_id_env.is_empty() {
+                self.azure = Some(AzureAuthMethod {
+                    identity_id: azure_auth_identity_id_env,
+                });
+
+                return Ok(AuthMethod::Azure);
+            }
+
             return Err("No authentication method is set.".into());
         }
     }
 }
```

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/client/client.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/client/client.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/client/client_settings.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/client/client_settings.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/constants.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/constants.rs`

 * *Files 19% similar despite different names*

```diff
@@ -5,20 +5,27 @@
 
 // GCP Auth:
 pub const INFISICAL_GCP_AUTH_IDENTITY_ID_ENV_NAME: &str = "INFISICAL_GCP_AUTH_IDENTITY_ID";
 pub const INFISICAL_GCP_IAM_SERVICE_ACCOUNT_KEY_FILE_PATH_ENV_NAME: &str =
     "INFISICAL_GCP_IAM_SERVICE_ACCOUNT_KEY_FILE_PATH";
 
 // AWS IAM Auth:
-pub const INFISICAL_AWS_IAM_IDENTITY_ID_ENV_NAME: &str = "INFISICAL_AWS_IAM_AUTH_IDENTITY_ID";
+pub const INFISICAL_AWS_IAM_AUTH_IDENTITY_ID_ENV_NAME: &str = "INFISICAL_AWS_IAM_AUTH_IDENTITY_ID";
 
 // Kubernetes Auth:
 pub const INFISICAL_KUBERNETES_SERVICE_ACCOUNT_TOKEN_PATH_ENV_NAME: &str =
     //  /var/run/secrets/kubernetes.io/serviceaccount/token
     "INFISICAL_KUBERNETES_SERVICE_ACCOUNT_TOKEN_PATH";
 
+// Azure Auth:
+pub const INFISICAL_AZURE_AUTH_IDENTITY_ID_ENV_NAME: &str = "INFISICAL_AZURE_AUTH_IDENTITY_ID";
+
 pub const INFISICAL_KUBERNETES_IDENTITY_ID_ENV_NAME: &str = "INFISICAL_KUBERNETES_IDENTITY_ID";
 
 // AWS EC2 Metadata Service:
 pub const AWS_EC2_METADATA_TOKEN_URL: &str = "http://169.254.169.254/latest/api/token";
 pub const AWS_EC2_INSTANCE_IDENTITY_DOCUMENT_URL: &str =
     "http://169.254.169.254/latest/dynamic/instance-identity/document";
+
+// Azure Metadata Service:
+pub const AZURE_METADATA_SERVICE_URL: &str =
+    "http://169.254.169.254/metadata/identity/oauth2/token?api-version=2018-02-01&resource=https%3A%2F%2Fmanagement.azure.com%2F";
```

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/error.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/error.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/helper.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/helper.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use std::borrow::Cow;
 
 use crate::{
     api::auth::{
-        aws_iam_login::aws_iam_login, gcp_iam_login::gcp_iam_login,
+        aws_iam_login::aws_iam_login, azure_login::azure_login, gcp_iam_login::gcp_iam_login,
         gcp_id_token_login::gcp_id_token_login, kubernetes_login::kubernetes_login,
         universal_auth_login::universal_auth_login,
     },
     client::auth_method_settings::AuthMethod,
     constants::{AWS_EC2_INSTANCE_IDENTITY_DOCUMENT_URL, AWS_EC2_METADATA_TOKEN_URL},
     error::{Error, Result},
     manager::secrets::Secret,
@@ -31,53 +31,54 @@
         };
 
         return Err(err);
     };
     debug!("Auth validation passed");
 
     let auth_method = validation_result.unwrap_or(AuthMethod::UniversalAuth);
-    let access_token;
+
+    let result;
 
     match auth_method {
         AuthMethod::UniversalAuth => {
             debug!("Auth method is Universal Auth");
-            let result = universal_auth_login(client).await?;
-            access_token = result.access_token;
+            result = universal_auth_login(client).await?;
         }
         AuthMethod::GcpIdToken => {
             debug!("Auth method is GCP ID Token");
-            let result = gcp_id_token_login(client).await?;
-            access_token = result.access_token;
+            result = gcp_id_token_login(client).await?;
         }
         AuthMethod::GcpIam => {
             debug!("Auth method is GCP IAM");
-            let result = gcp_iam_login(client).await?;
-            access_token = result.access_token;
+            result = gcp_iam_login(client).await?;
         }
 
         AuthMethod::AwsIam => {
             debug!("Auth method is AWS IAM");
-            let result = aws_iam_login(client).await?;
-            access_token = result.access_token;
+            result = aws_iam_login(client).await?;
         }
 
         AuthMethod::Kubernetes => {
             debug!("Auth method is Kubernetes");
-            let result = kubernetes_login(client).await?;
-            access_token = result.access_token;
+            result = kubernetes_login(client).await?;
+        }
+
+        AuthMethod::Azure => {
+            debug!("Auth method is Azure");
+            result = azure_login(client).await?;
         }
     }
 
-    if access_token.is_empty() {
+    if result.access_token.is_empty() {
         debug!("No access token obtained");
         return Err(Error::NoAccessTokenObtained);
     }
 
     debug!("Setting access token");
-    client.set_access_token(access_token);
+    client.set_access_token(result.access_token);
     Ok(())
 }
 
 pub fn ensure_unique_secrets_by_key(secrets: &mut Vec<Secret>) {
     let mut secret_map = std::collections::HashMap::new();
 
     // Use the entry API to check and insert if the key does not exist
```

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/manager/client_cryptography.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/manager/client_cryptography.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/manager/client_secrets.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/manager/client_secrets.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/manager/cryptography/create_symmetric_key.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/manager/cryptography/create_symmetric_key.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/manager/cryptography/decrypt_symmetric.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/manager/cryptography/decrypt_symmetric.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/manager/cryptography/encrypt_symmetric.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/manager/cryptography/encrypt_symmetric.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/create.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/manager/secrets/create.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/delete.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/manager/secrets/delete.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/get.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/manager/secrets/get.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/list.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/manager/secrets/list.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/mod.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/manager/secrets/mod.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/src/manager/secrets/update.rs` & `infisical_python-2.2.1/local_dependencies/infisical/src/manager/secrets/update.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/tests/cryptography.rs` & `infisical_python-2.2.1/local_dependencies/infisical/tests/cryptography.rs`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         // These fields are deprecated. If they are populated, they will be backfilled into the new auth object.
         client_id: None,
         client_secret: None,
         access_token: None,
 
         auth: AuthenticationOptions {
             gcp_iam: None,
+            azure: None,
             gcp_id_token: None,
             kubernetes: None,
             aws_iam: None,
             access_token: None,
             universal_auth: Some(UniversalAuthMethod {
                 client_id: environment.client_id,
                 client_secret: environment.client_secret,
```

### Comparing `infisical_python-2.2.0/local_dependencies/infisical/tests/secrets.rs` & `infisical_python-2.2.1/local_dependencies/infisical/tests/secrets.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical-json/src/client.rs` & `infisical_python-2.2.1/local_dependencies/infisical-json/src/client.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical-json/src/command.rs` & `infisical_python-2.2.1/local_dependencies/infisical-json/src/command.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/local_dependencies/infisical-json/src/response.rs` & `infisical_python-2.2.1/local_dependencies/infisical-json/src/response.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/Cargo.toml` & `infisical_python-2.2.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "infisical-py"
-version = "2.2.0"
+version = "2.2.1"
 edition = "2021"
 rust-version = "1.57"
 
 [lib]
 name = "infisical_py"
 crate-type = ["cdylib"]
```

### Comparing `infisical_python-2.2.0/LICENSE` & `infisical_python-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/example.py` & `infisical_python-2.2.1/example.py`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/infisical_client/__init__.py` & `infisical_python-2.2.1/infisical_client/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.2.0"
+__version__ = "2.2.1"
 
 from .infisical_client import InfisicalClient as InfisicalClient
 
 from .infisical_py import InfisicalClient as RustInfisicalClient
 
 from .schemas import GetSecretOptions as GetSecretOptions
 from .schemas import UpdateSecretOptions as UpdateSecretOptions
@@ -21,8 +21,9 @@
 
 # Auth related
 from .schemas import AuthenticationOptions as AuthenticationOptions
 
 from .schemas import AWSIamAuthMethod as AWSIamAuthMethod
 from .schemas import GCPIamAuthMethod as GCPIamAuthMethod
 from .schemas import GCPIDTokenAuthMethod as GCPIDTokenAuthMethod
-from .schemas import UniversalAuthMethod as UniversalAuthMethod
+from .schemas import UniversalAuthMethod as UniversalAuthMethod
+from .schemas import AzureAuthMethod as AzureAuthMethod
```

### Comparing `infisical_python-2.2.0/infisical_client/infisical_client.py` & `infisical_python-2.2.1/infisical_client/infisical_client.py`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/pyproject.toml` & `infisical_python-2.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [tool.poetry]
 name = "infisical-python"
-version = "2.2.0"
+version = "2.2.1"
 description = 'Official Infisical SDK for Python (New)'
 authors = ["Daniel Hougaard <daniel@infisical.com>"]
 
 [tool.poetry_bumpversion.file."infisical_client/__init__.py"]
 search = '__version__ = "{current_version}"'
 replace = '__version__ = "{new_version}"'
```

### Comparing `infisical_python-2.2.0/src/client.rs` & `infisical_python-2.2.1/src/client.rs`

 * *Files identical despite different names*

### Comparing `infisical_python-2.2.0/Cargo.lock` & `infisical_python-2.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1358,15 +1358,15 @@
  "napi",
  "napi-build",
  "napi-derive",
 ]
 
 [[package]]
 name = "infisical-py"
-version = "2.2.0"
+version = "2.2.1"
 dependencies = [
  "env_logger 0.9.3",
  "infisical-json",
  "log",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-build-config",
@@ -1860,17 +1860,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.83"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
@@ -2363,26 +2363,26 @@
 name = "semver"
 version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
 
 [[package]]
 name = "serde"
-version = "1.0.202"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "226b61a0d411b2ba5ff6d7f73a476ac4f8bb900373459cd00fab8512828ba395"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.202"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.66",
 ]
 
 [[package]]
@@ -3279,10 +3279,10 @@
  "tokio",
  "tower-service",
  "url 2.5.0",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.7.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
+checksum = "ced3678a2879b30306d323f4542626697a464a97c0a07c9aebf7ebca65cd4dde"
```

### Comparing `infisical_python-2.2.0/infisical_client/schemas.py` & `infisical_python-2.2.1/infisical_client/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,31 @@
     def to_dict(self) -> dict:
         result: dict = {}
         result["identityId"] = from_str(self.identity_id)
         return result
 
 
 @dataclass
+class AzureAuthMethod:
+    identity_id: str
+    """The Infisical Identity ID that you want to authenticate to Infisical with."""
+
+    @staticmethod
+    def from_dict(obj: Any) -> 'AzureAuthMethod':
+        assert isinstance(obj, dict)
+        identity_id = from_str(obj.get("identityId"))
+        return AzureAuthMethod(identity_id)
+
+    def to_dict(self) -> dict:
+        result: dict = {}
+        result["identityId"] = from_str(self.identity_id)
+        return result
+
+
+@dataclass
 class GCPIamAuthMethod:
     identity_id: str
     service_account_key_file_path: str
     """The path to the GCP Service Account key file.
     
     You can generate this key file by going to the GCP Console -> IAM & Admin -> Service
     Accounts -> *Select your service account* -> Keys tab -> Add key.
@@ -105,15 +122,16 @@
 @dataclass
 class KubernetesAuthMethod:
     identity_id: str
     """The Infisical Identity ID that you want to authenticate to Infisical with."""
     service_account_token_path: Optional[str] = None
     """The path to the Kubernetes Service Account token file.
     
-    This is usually located at /var/run/secrets/kubernetes.io/serviceaccount/token.
+    If no path is provided, it will default to
+    /var/run/secrets/kubernetes.io/serviceaccount/token.
     """
 
     @staticmethod
     def from_dict(obj: Any) -> 'KubernetesAuthMethod':
         assert isinstance(obj, dict)
         identity_id = from_str(obj.get("identityId"))
         service_account_token_path = from_union([from_none, from_str], obj.get("serviceAccountTokenPath"))
@@ -150,36 +168,40 @@
 class AuthenticationOptions:
     """Configure the authentication method to use.
     
     Make sure to only set one one method at a time to avoid conflicts and unexpected behavior.
     """
     access_token: Optional[str] = None
     aws_iam: Optional[AWSIamAuthMethod] = None
+    azure: Optional[AzureAuthMethod] = None
     gcp_iam: Optional[GCPIamAuthMethod] = None
     gcp_id_token: Optional[GCPIDTokenAuthMethod] = None
     kubernetes: Optional[KubernetesAuthMethod] = None
     universal_auth: Optional[UniversalAuthMethod] = None
 
     @staticmethod
     def from_dict(obj: Any) -> 'AuthenticationOptions':
         assert isinstance(obj, dict)
         access_token = from_union([from_none, from_str], obj.get("accessToken"))
         aws_iam = from_union([AWSIamAuthMethod.from_dict, from_none], obj.get("awsIam"))
+        azure = from_union([AzureAuthMethod.from_dict, from_none], obj.get("azure"))
         gcp_iam = from_union([GCPIamAuthMethod.from_dict, from_none], obj.get("gcpIam"))
         gcp_id_token = from_union([GCPIDTokenAuthMethod.from_dict, from_none], obj.get("gcpIdToken"))
         kubernetes = from_union([KubernetesAuthMethod.from_dict, from_none], obj.get("kubernetes"))
         universal_auth = from_union([UniversalAuthMethod.from_dict, from_none], obj.get("universalAuth"))
-        return AuthenticationOptions(access_token, aws_iam, gcp_iam, gcp_id_token, kubernetes, universal_auth)
+        return AuthenticationOptions(access_token, aws_iam, azure, gcp_iam, gcp_id_token, kubernetes, universal_auth)
 
     def to_dict(self) -> dict:
         result: dict = {}
         if self.access_token is not None:
             result["accessToken"] = from_union([from_none, from_str], self.access_token)
         if self.aws_iam is not None:
             result["awsIam"] = from_union([lambda x: to_class(AWSIamAuthMethod, x), from_none], self.aws_iam)
+        if self.azure is not None:
+            result["azure"] = from_union([lambda x: to_class(AzureAuthMethod, x), from_none], self.azure)
         if self.gcp_iam is not None:
             result["gcpIam"] = from_union([lambda x: to_class(GCPIamAuthMethod, x), from_none], self.gcp_iam)
         if self.gcp_id_token is not None:
             result["gcpIdToken"] = from_union([lambda x: to_class(GCPIDTokenAuthMethod, x), from_none], self.gcp_id_token)
         if self.kubernetes is not None:
             result["kubernetes"] = from_union([lambda x: to_class(KubernetesAuthMethod, x), from_none], self.kubernetes)
         if self.universal_auth is not None:
```

### Comparing `infisical_python-2.2.0/PKG-INFO` & `infisical_python-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infisical-python
-Version: 2.2.0
+Version: 2.2.1
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
@@ -20,17 +20,17 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Official Infisical SDK for Python (New)
 Maintainer-email: Daniel Hougaard <daniel@infisical.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Documentation, https://github.com/Infisical/sdk/tree/main/crates/infisical-py#readme
-Project-URL: Source, https://github.com/infisical/sdk
 Project-URL: Issues, https://github.com/infisical/sdk/issues
+Project-URL: Source, https://github.com/infisical/sdk
+Project-URL: Documentation, https://github.com/Infisical/sdk/tree/main/crates/infisical-py#readme
 
 <h1 align="center">
     <a href="https://github.com/Infisical/infisical">
         <img width="300" src="https://raw.githubusercontent.com/Infisical/infisical-node/main/img/logoname-white.svg#gh-dark-mode-only" alt="infisical">
     </a>
 </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: infisical-python Version: 2.2.0 Classifier:
+Metadata-Version: 2.1 Name: infisical-python Version: 2.2.1 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Operating System :: OS
 Independent Classifier: Topic :: Software Development :: Libraries ::
 Application Frameworks Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development Classifier: Typing :: Typed
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -11,16 +11,16 @@
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy License-File: LICENSE Summary: Official Infisical SDK
 for Python (New) Maintainer-email: Daniel Hougaard
 infisical.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Project-URL: Documentation, https://github.com/
-Infisical/sdk/tree/main/crates/infisical-py#readme Project-URL: Source, https:/
-/github.com/infisical/sdk Project-URL: Issues, https://github.com/infisical/
-sdk/issues
+charset=UTF-8; variant=GFM Project-URL: Issues, https://github.com/infisical/
+sdk/issues Project-URL: Source, https://github.com/infisical/sdk Project-URL:
+Documentation, https://github.com/Infisical/sdk/tree/main/crates/infisical-
+py#readme
                            ************ _[[_ii_nn_ff_ii_ss_ii_cc_aa_ll_]] ************
   Open-source, end-to-end encrypted tool to manage secrets and configs across
                          your team and infrastructure.
 # Documentation [You can find the documentation here](https://infisical.com/
 docs/sdks/languages/python)
```

