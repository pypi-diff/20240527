# Comparing `tmp/python_rebase-0.3.3.tar.gz` & `tmp/python_rebase-0.3.4.tar.gz`

## Comparing `python_rebase-0.3.3.tar` & `python_rebase-0.3.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 python_rebase-0.3.3/CHANGELOG.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 python_rebase-0.3.3/requirements.txt
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 python_rebase-0.3.3/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 python_rebase-0.3.3/examples/auth_example.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 python_rebase-0.3.3/examples/movement_example.py
--rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 python_rebase-0.3.3/examples/session_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rebase-0.3.3/src/python_rebase/__init__.py
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 python_rebase-0.3.3/src/python_rebase/api_response.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 python_rebase-0.3.3/src/python_rebase/mismatched_articulations_error.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 python_rebase-0.3.3/src/python_rebase/missing_attribute_error.py
--rw-r--r--   0        0        0     7592 2020-02-02 00:00:00.000000 python_rebase-0.3.3/src/python_rebase/movement.py
--rw-r--r--   0        0        0     9479 2020-02-02 00:00:00.000000 python_rebase-0.3.3/src/python_rebase/rebase_client.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 python_rebase-0.3.3/src/python_rebase/register.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 python_rebase-0.3.3/src/python_rebase/repeated_articulation_error.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 python_rebase-0.3.3/src/python_rebase/rotation.py
--rw-r--r--   0        0        0     8206 2020-02-02 00:00:00.000000 python_rebase-0.3.3/src/python_rebase/session.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 python_rebase-0.3.3/src/python_rebase/unauthorized_user_error.py
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 python_rebase-0.3.3/src/python_rebase/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rebase-0.3.3/tests/__init__.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 python_rebase-0.3.3/tests/exceptions_test.py
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 python_rebase-0.3.3/tests/movement_test.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 python_rebase-0.3.3/tests/rebase_client_test.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 python_rebase-0.3.3/tests/register_test.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 python_rebase-0.3.3/tests/rotation_test.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 python_rebase-0.3.3/tests/session_test.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 python_rebase-0.3.3/tests/util_test.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 python_rebase-0.3.3/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 python_rebase-0.3.3/LICENSE
--rw-r--r--   0        0        0    30070 2020-02-02 00:00:00.000000 python_rebase-0.3.3/README.md
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 python_rebase-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    30998 2020-02-02 00:00:00.000000 python_rebase-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 python_rebase-0.3.4/CHANGELOG.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 python_rebase-0.3.4/requirements.txt
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 python_rebase-0.3.4/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 python_rebase-0.3.4/examples/auth_example.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 python_rebase-0.3.4/examples/movement_example.py
+-rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 python_rebase-0.3.4/examples/session_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rebase-0.3.4/src/python_rebase/__init__.py
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 python_rebase-0.3.4/src/python_rebase/api_response.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 python_rebase-0.3.4/src/python_rebase/mismatched_articulations_error.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 python_rebase-0.3.4/src/python_rebase/missing_attribute_error.py
+-rw-r--r--   0        0        0     7592 2020-02-02 00:00:00.000000 python_rebase-0.3.4/src/python_rebase/movement.py
+-rw-r--r--   0        0        0     9481 2020-02-02 00:00:00.000000 python_rebase-0.3.4/src/python_rebase/rebase_client.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 python_rebase-0.3.4/src/python_rebase/register.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 python_rebase-0.3.4/src/python_rebase/repeated_articulation_error.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 python_rebase-0.3.4/src/python_rebase/rotation.py
+-rw-r--r--   0        0        0     8206 2020-02-02 00:00:00.000000 python_rebase-0.3.4/src/python_rebase/session.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 python_rebase-0.3.4/src/python_rebase/unauthorized_user_error.py
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 python_rebase-0.3.4/src/python_rebase/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_rebase-0.3.4/tests/__init__.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 python_rebase-0.3.4/tests/exceptions_test.py
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 python_rebase-0.3.4/tests/movement_test.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 python_rebase-0.3.4/tests/rebase_client_test.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 python_rebase-0.3.4/tests/register_test.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 python_rebase-0.3.4/tests/rotation_test.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 python_rebase-0.3.4/tests/session_test.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 python_rebase-0.3.4/tests/util_test.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 python_rebase-0.3.4/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 python_rebase-0.3.4/LICENSE
+-rw-r--r--   0        0        0    30070 2020-02-02 00:00:00.000000 python_rebase-0.3.4/README.md
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 python_rebase-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0    30998 2020-02-02 00:00:00.000000 python_rebase-0.3.4/PKG-INFO
```

### Comparing `python_rebase-0.3.3/CHANGELOG.md` & `python_rebase-0.3.4/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 
 Todas as mudanças notáveis deste projeto serão documentadas neste arquivo.
 
 Este formato é baseado em [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
 e este projeto adere ao [Versionamento Semântico](https://semver.org/spec/v2.0.0.html).
 
+## [0.3.4] - 2024-05-27
+
+### Alterado
+- Foi atualizada a versão da biblioteca `requests`
+
 ## [0.3.3] - 2024-02-22
 
 ### Adicionado
 - Método `authenticate` em `ReBaseClient`, que pode ser utilizado para tentar autenticar um usuário sem executar nenhuma operação sobre o banco de dados;
 - Parâmetro booleano `try_authenticate` no inicializador de `ReBaseClient`, por padrão `False`. Quando `True`, tenta autenticar no momento da inicialização e, caso falhe, levanta erro `UnauthorizedUserError`;
 - Erro `UnauthorizedUserError`, levantado na ocasião anteriormente mencionada.
```

### Comparing `python_rebase-0.3.3/.github/workflows/pylint.yml` & `python_rebase-0.3.4/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/examples/auth_example.py` & `python_rebase-0.3.4/examples/auth_example.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/examples/movement_example.py` & `python_rebase-0.3.4/examples/movement_example.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/examples/session_example.py` & `python_rebase-0.3.4/examples/session_example.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/src/python_rebase/api_response.py` & `python_rebase-0.3.4/src/python_rebase/api_response.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/src/python_rebase/mismatched_articulations_error.py` & `python_rebase-0.3.4/src/python_rebase/mismatched_articulations_error.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/src/python_rebase/missing_attribute_error.py` & `python_rebase-0.3.4/src/python_rebase/missing_attribute_error.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/src/python_rebase/movement.py` & `python_rebase-0.3.4/src/python_rebase/movement.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/src/python_rebase/rebase_client.py` & `python_rebase-0.3.4/src/python_rebase/rebase_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         try:
             if method == _Method.GET:
                 response = requests.get(url, headers=self._authentication_headers, params=params, timeout=30)
             elif method == _Method.POST:
                 response = requests.post(url, headers={ 'Content-Type': 'application/json', **self._authentication_headers }, params=params, data=data, timeout=30)
             elif method == _Method.PUT:
                 response = requests.put(url, headers={ 'Content-Type': 'application/json', **self._authentication_headers }, params=params, data=data, timeout=30)
-            elif method == _Method.DELETE:
+            else: # method == _Method.DELETE
                 response = requests.delete(url, headers=self._authentication_headers, params=params, timeout=30)
         except requests.exceptions.RequestException as e:
             return self.__new_api_error_response(str(e))
 
         return self.__parse_api_response(response, response_type)
 
     def __parse_api_response(self, response: requests.Response, response_type: APIResponse.ResponseType) -> APIResponse:
```

### Comparing `python_rebase-0.3.3/src/python_rebase/register.py` & `python_rebase-0.3.4/src/python_rebase/register.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/src/python_rebase/repeated_articulation_error.py` & `python_rebase-0.3.4/src/python_rebase/repeated_articulation_error.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/src/python_rebase/rotation.py` & `python_rebase-0.3.4/src/python_rebase/rotation.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/src/python_rebase/session.py` & `python_rebase-0.3.4/src/python_rebase/session.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/src/python_rebase/unauthorized_user_error.py` & `python_rebase-0.3.4/src/python_rebase/unauthorized_user_error.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/src/python_rebase/util.py` & `python_rebase-0.3.4/src/python_rebase/util.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/tests/exceptions_test.py` & `python_rebase-0.3.4/tests/exceptions_test.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/tests/movement_test.py` & `python_rebase-0.3.4/tests/movement_test.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/tests/rebase_client_test.py` & `python_rebase-0.3.4/tests/rebase_client_test.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/tests/register_test.py` & `python_rebase-0.3.4/tests/register_test.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/tests/rotation_test.py` & `python_rebase-0.3.4/tests/rotation_test.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/tests/session_test.py` & `python_rebase-0.3.4/tests/session_test.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/tests/util_test.py` & `python_rebase-0.3.4/tests/util_test.py`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/.gitignore` & `python_rebase-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/LICENSE` & `python_rebase-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_rebase-0.3.3/README.md` & `python_rebase-0.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Python ReBase [0.3.3]
+# Python ReBase [0.3.4]
 Este projeto é uma API escrita em Python para comunicação com o ReBase, um banco de dados de sessões de reabilitação física.
 
 ## Índice
-- [Python ReBase \[0.3.3\]](#python-rebase-033)
+- [Python ReBase \[0.3.4\]](#python-rebase-034)
   - [Índice](#índice)
   - [Visão Geral](#visão-geral)
     - [Sobre o ReBase](#sobre-o-rebase)
   - [Instalação](#instalação)
   - [Requisitos](#requisitos)
   - [Quick Start](#quick-start)
     - [Inicializando o ReBaseClient](#inicializando-o-rebaseclient)
```

### Comparing `python_rebase-0.3.3/pyproject.toml` & `python_rebase-0.3.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests>=2.31.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python-rebase"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Tiago Trotta", email="mrtrotta2010@gmail.com" },
 ]
 description = "Python implementation of the ReBase API"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_rebase-0.3.3/PKG-INFO` & `python_rebase-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: python-rebase
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python implementation of the ReBase API
 Project-URL: Repository, https://github.com/MrTrotta2010/python-rebase
 Project-URL: Changelog, https://github.com/MrTrotta2010/python-rebase/blob/main/CHANGELOG.md
 Author-email: Tiago Trotta <mrtrotta2010@gmail.com>
 License-File: LICENSE
 Keywords: database,databases,gesture tracking,medical,movement tracking
 Classifier: Development Status :: 4 - Beta
@@ -14,19 +14,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
-# Python ReBase [0.3.3]
+# Python ReBase [0.3.4]
 Este projeto é uma API escrita em Python para comunicação com o ReBase, um banco de dados de sessões de reabilitação física.
 
 ## Índice
-- [Python ReBase \[0.3.3\]](#python-rebase-033)
+- [Python ReBase \[0.3.4\]](#python-rebase-034)
   - [Índice](#índice)
   - [Visão Geral](#visão-geral)
     - [Sobre o ReBase](#sobre-o-rebase)
   - [Instalação](#instalação)
   - [Requisitos](#requisitos)
   - [Quick Start](#quick-start)
     - [Inicializando o ReBaseClient](#inicializando-o-rebaseclient)
```

