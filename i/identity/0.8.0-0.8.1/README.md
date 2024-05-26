# Comparing `tmp/identity-0.8.0.tar.gz` & `tmp/identity-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "identity-0.8.0.tar", last modified: Mon May 20 06:00:10 2024, max compression
+gzip compressed data, was "identity-0.8.1.tar", last modified: Sun May 26 22:38:32 2024, max compression
```

## Comparing `identity-0.8.0.tar` & `identity-0.8.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:00:10.009603 identity-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 06:00:05.000000 identity-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-20 06:00:10.009603 identity-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-20 06:00:05.000000 identity-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:00:10.005603 identity-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-20 06:00:05.000000 identity-0.8.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:00:10.005603 identity-0.8.0/identity/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-20 06:00:05.000000 identity-0.8.0/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-20 06:00:05.000000 identity-0.8.0/identity/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-20 06:00:05.000000 identity-0.8.0/identity/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-20 06:00:05.000000 identity-0.8.0/identity/quart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:00:10.001603 identity-0.8.0/identity/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:00:10.005603 identity-0.8.0/identity/templates/identity/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-20 06:00:05.000000 identity-0.8.0/identity/templates/identity/auth_error.html
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-20 06:00:05.000000 identity-0.8.0/identity/templates/identity/login.html
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-20 06:00:05.000000 identity-0.8.0/identity/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    23033 2024-05-20 06:00:05.000000 identity-0.8.0/identity/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:00:10.005603 identity-0.8.0/identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-20 06:00:09.000000 identity-0.8.0/identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-20 06:00:10.000000 identity-0.8.0/identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 06:00:09.000000 identity-0.8.0/identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-20 06:00:09.000000 identity-0.8.0/identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 06:00:09.000000 identity-0.8.0/identity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-20 06:00:05.000000 identity-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-20 06:00:10.009603 identity-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 06:00:05.000000 identity-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:00:10.005603 identity-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-20 06:00:05.000000 identity-0.8.0/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-20 06:00:05.000000 identity-0.8.0/tests/test_quart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:38:32.010685 identity-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-26 22:38:28.000000 identity-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-05-26 22:38:32.010685 identity-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-26 22:38:28.000000 identity-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:38:32.006685 identity-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-26 22:38:28.000000 identity-0.8.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:38:32.010685 identity-0.8.1/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-26 22:38:28.000000 identity-0.8.1/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-26 22:38:28.000000 identity-0.8.1/identity/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-26 22:38:28.000000 identity-0.8.1/identity/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-26 22:38:28.000000 identity-0.8.1/identity/quart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:38:32.006685 identity-0.8.1/identity/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:38:32.010685 identity-0.8.1/identity/templates/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-26 22:38:28.000000 identity-0.8.1/identity/templates/identity/auth_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-26 22:38:28.000000 identity-0.8.1/identity/templates/identity/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-26 22:38:28.000000 identity-0.8.1/identity/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23446 2024-05-26 22:38:28.000000 identity-0.8.1/identity/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:38:32.010685 identity-0.8.1/identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-05-26 22:38:31.000000 identity-0.8.1/identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-26 22:38:32.000000 identity-0.8.1/identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 22:38:31.000000 identity-0.8.1/identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-26 22:38:31.000000 identity-0.8.1/identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 22:38:31.000000 identity-0.8.1/identity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-26 22:38:28.000000 identity-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-26 22:38:32.010685 identity-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-26 22:38:28.000000 identity-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:38:32.010685 identity-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-26 22:38:28.000000 identity-0.8.1/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-26 22:38:28.000000 identity-0.8.1/tests/test_quart.py
```

### Comparing `identity-0.8.0/LICENSE` & `identity-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `identity-0.8.0/PKG-INFO` & `identity-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: identity
-Version: 0.8.0
+Version: 0.8.1
 Summary: This is an authentication/authorization library, currently optimized for web apps. It provides some higher level APIs built on top of Microsoft's MSAL Python.
 Home-page: https://github.com/rayluo/identity
 Author: Ray Luo
 Author-email: rayluo.mba@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/rayluo/identity/releases
 Project-URL: Documentation, https://identity-library.readthedocs.io/
@@ -103,15 +103,15 @@
 
 By using this library, it will automatically renew signed-in session when the ID token expires.
 
 * [Sample written in ![Django](https://raw.githubusercontent.com/rayluo/identity/dev/docs/django.webp)](https://github.com/Azure-Samples/ms-identity-python-webapp-django)
 * [Sample written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-python-webapp)
 * [Sample written in ![Quart](https://raw.githubusercontent.com/rayluo/identity/dev/docs/quart.webp)](https://github.com/rayluo/python-webapp-quart)
 * Need support for more web frameworks?
-  [Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues)
+  [Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues?q=is%3Aissue+is%3Aopen+sort%3Areactions-%2B1-desc)
 
 </td>
   </tr>
 
   <tr>
     <th>How to customize the login page</th>
     <td colspan=4>
@@ -157,16 +157,15 @@
 </td>
   </tr>
 
   <tr>
     <th>Other scenarios</th>
     <td colspan=4>
 
-[Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues)
-<!-- FastAPI, Streamlit, ... -->
+[Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues?q=is%3Aissue+is%3Aopen+sort%3Areactions-%2B1-desc)
 
 </td>
   </tr>
 
 </table>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: identity Version: 0.8.0 Summary: This is an
+Metadata-Version: 2.1 Name: identity Version: 0.8.1 Summary: This is an
 authentication/authorization library, currently optimized for web apps. It
 provides some higher level APIs built on top of Microsoft's MSAL Python. Home-
 page: https://github.com/rayluo/identity Author: Ray Luo Author-email:
 rayluo.mba@gmail.com License: MIT Project-URL: Changelog, https://github.com/
 rayluo/identity/releases Project-URL: Documentation, https://identity-
 library.readthedocs.io/ Keywords: identity,auth,authentication,authorization
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
@@ -68,15 +68,16 @@
 |            |/github.com/Azure-Samples/ms-identity-python-webapp-django) * [Sample   |
 |WWeebb AApppp SSiiggnn|written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/  |
 |IInn && SSiiggnn   |dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-     |
 |OOuutt         |python-webapp) * [Sample written in ![Quart](https://                   |
 |            |raw.githubusercontent.com/rayluo/identity/dev/docs/quart.webp)](https://|
 |            |github.com/rayluo/python-webapp-quart) * Need support for more web      |
 |            |frameworks? [Upvote existing feature request or create a new one](https:|
-|_ _ _ _ _ _ _ _ _ _ _ _ _|_/_/_g_i_t_h_u_b_._c_o_m_/_r_a_y_l_u_o_/_i_d_e_n_t_i_t_y_/_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
+|            |//github.com/rayluo/identity/                                           |
+|_ _ _ _ _ _ _ _ _ _ _ _ _|_i_s_s_u_e_s_?_q_=_i_s_%_3_A_i_s_s_u_e_+_i_s_%_3_A_o_p_e_n_+_s_o_r_t_%_3_A_r_e_a_c_t_i_o_n_s_-_%_2_B_1_-_d_e_s_c_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |HHooww ttoo      |The default login page will typically redirect users to your Identity   |
 |ccuussttoommiizzee   |Provider, so you don't have to customize it. But if the default login   |
 |tthhee llooggiinn   |page is shown in your browser, you can read its HTML source code, and   |
 |_pp_aa_gg_ee_ _ _ _ _ _ _ _ _|_f_i_n_d_ _t_h_e_ _h_o_w_-_t_o_ _i_n_s_t_r_u_c_t_i_o_n_s_ _t_h_e_r_e_._ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |WWeebb AApppp     |This library supports: + Incremental consent. If the user needs to      |
 |CCaallllss aa wweebb |consent to more permissions, the library will automatically redirect the|
 |AAPPII         |user to the consent page. + Automatically cache the access token and    |
@@ -87,15 +88,16 @@
 |AAPPII ((OOnn--    |                                                                        |
 |_bb_ee_hh_aa_ll_ff_--_oo_ff_))_ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |HHooww ttoo bbuuiilldd|                                                                        |
 |tthhee ssaammpplleess |Read our [docs here](https://identity-library.readthedocs.io/en/latest/)|
 |aabboovvee ffrroomm  |                                                                        |
 |_ss_cc_rr_aa_tt_cc_hh_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |OOtthheerr       |[Upvote existing feature request or create a new one](https://          |
-|_ss_cc_ee_nn_aa_rr_ii_oo_ss_ _ _ _|_g_i_t_h_u_b_._c_o_m_/_r_a_y_l_u_o_/_i_d_e_n_t_i_t_y_/_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
+|sscceennaarriiooss   |github.com/rayluo/identity/                                             |
+|_ _ _ _ _ _ _ _ _ _ _ _ _|_i_s_s_u_e_s_?_q_=_i_s_%_3_A_i_s_s_u_e_+_i_s_%_3_A_o_p_e_n_+_s_o_r_t_%_3_A_r_e_a_c_t_i_o_n_s_-_%_2_B_1_-_d_e_s_c_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 ## Installation This package is [available on PyPI](https://pypi.org/project/
 identity/). Choose the package declaration that matches your web framework: *
 Django: `pip install identity[django]` * Flask: `pip install identity[flask]` *
 Quart: `pip install identity[quart]` ## Versions This library follows [Semantic
 Versioning](http://semver.org/). Your project should declare `identity`
 dependency with proper lower and upper bound. You can find the changes for each
 version under [Releases](https://github.com/rayluo/identity/releases).
```

### Comparing `identity-0.8.0/README.md` & `identity-0.8.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 By using this library, it will automatically renew signed-in session when the ID token expires.
 
 * [Sample written in ![Django](https://raw.githubusercontent.com/rayluo/identity/dev/docs/django.webp)](https://github.com/Azure-Samples/ms-identity-python-webapp-django)
 * [Sample written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-python-webapp)
 * [Sample written in ![Quart](https://raw.githubusercontent.com/rayluo/identity/dev/docs/quart.webp)](https://github.com/rayluo/python-webapp-quart)
 * Need support for more web frameworks?
-  [Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues)
+  [Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues?q=is%3Aissue+is%3Aopen+sort%3Areactions-%2B1-desc)
 
 </td>
   </tr>
 
   <tr>
     <th>How to customize the login page</th>
     <td colspan=4>
@@ -115,16 +115,15 @@
 </td>
   </tr>
 
   <tr>
     <th>Other scenarios</th>
     <td colspan=4>
 
-[Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues)
-<!-- FastAPI, Streamlit, ... -->
+[Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues?q=is%3Aissue+is%3Aopen+sort%3Areactions-%2B1-desc)
 
 </td>
   </tr>
 
 </table>
```

#### html2text {}

```diff
@@ -44,15 +44,16 @@
 |            |/github.com/Azure-Samples/ms-identity-python-webapp-django) * [Sample   |
 |WWeebb AApppp SSiiggnn|written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/  |
 |IInn && SSiiggnn   |dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-     |
 |OOuutt         |python-webapp) * [Sample written in ![Quart](https://                   |
 |            |raw.githubusercontent.com/rayluo/identity/dev/docs/quart.webp)](https://|
 |            |github.com/rayluo/python-webapp-quart) * Need support for more web      |
 |            |frameworks? [Upvote existing feature request or create a new one](https:|
-|_ _ _ _ _ _ _ _ _ _ _ _ _|_/_/_g_i_t_h_u_b_._c_o_m_/_r_a_y_l_u_o_/_i_d_e_n_t_i_t_y_/_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
+|            |//github.com/rayluo/identity/                                           |
+|_ _ _ _ _ _ _ _ _ _ _ _ _|_i_s_s_u_e_s_?_q_=_i_s_%_3_A_i_s_s_u_e_+_i_s_%_3_A_o_p_e_n_+_s_o_r_t_%_3_A_r_e_a_c_t_i_o_n_s_-_%_2_B_1_-_d_e_s_c_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |HHooww ttoo      |The default login page will typically redirect users to your Identity   |
 |ccuussttoommiizzee   |Provider, so you don't have to customize it. But if the default login   |
 |tthhee llooggiinn   |page is shown in your browser, you can read its HTML source code, and   |
 |_pp_aa_gg_ee_ _ _ _ _ _ _ _ _|_f_i_n_d_ _t_h_e_ _h_o_w_-_t_o_ _i_n_s_t_r_u_c_t_i_o_n_s_ _t_h_e_r_e_._ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |WWeebb AApppp     |This library supports: + Incremental consent. If the user needs to      |
 |CCaallllss aa wweebb |consent to more permissions, the library will automatically redirect the|
 |AAPPII         |user to the consent page. + Automatically cache the access token and    |
@@ -63,15 +64,16 @@
 |AAPPII ((OOnn--    |                                                                        |
 |_bb_ee_hh_aa_ll_ff_--_oo_ff_))_ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |HHooww ttoo bbuuiilldd|                                                                        |
 |tthhee ssaammpplleess |Read our [docs here](https://identity-library.readthedocs.io/en/latest/)|
 |aabboovvee ffrroomm  |                                                                        |
 |_ss_cc_rr_aa_tt_cc_hh_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |OOtthheerr       |[Upvote existing feature request or create a new one](https://          |
-|_ss_cc_ee_nn_aa_rr_ii_oo_ss_ _ _ _|_g_i_t_h_u_b_._c_o_m_/_r_a_y_l_u_o_/_i_d_e_n_t_i_t_y_/_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
+|sscceennaarriiooss   |github.com/rayluo/identity/                                             |
+|_ _ _ _ _ _ _ _ _ _ _ _ _|_i_s_s_u_e_s_?_q_=_i_s_%_3_A_i_s_s_u_e_+_i_s_%_3_A_o_p_e_n_+_s_o_r_t_%_3_A_r_e_a_c_t_i_o_n_s_-_%_2_B_1_-_d_e_s_c_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 ## Installation This package is [available on PyPI](https://pypi.org/project/
 identity/). Choose the package declaration that matches your web framework: *
 Django: `pip install identity[django]` * Flask: `pip install identity[flask]` *
 Quart: `pip install identity[quart]` ## Versions This library follows [Semantic
 Versioning](http://semver.org/). Your project should declare `identity`
 dependency with proper lower and upper bound. You can find the changes for each
 version under [Releases](https://github.com/rayluo/identity/releases).
```

### Comparing `identity-0.8.0/docs/conf.py` & `identity-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `identity-0.8.0/identity/django.py` & `identity-0.8.1/identity/django.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,21 @@
 
     Afterwards, all you need to do is to insert ``auth.urlpattern`` into
     your project's ``urlpatterns`` list in ``your_project/urls.py``.
     """
 
     def __init__(self, *args, **kwargs):
         super(Auth, self).__init__(*args, **kwargs)
-        route, self._redirect_view = _parse_redirect_uri(self._redirect_uri)
+        route, redirect_view = _parse_redirect_uri(self._redirect_uri)
         self.urlpattern = path(route, include([
             # Note: path(..., view, ...) does not accept classmethod
             path('login', self.login),
             path('logout', self.logout, name=f"identity.logout"),
             path(
-                self._redirect_view or 'auth_response',  # The latter is used by device code flow
+                redirect_view or 'auth_response',  # The latter is used by device code flow
                 self.auth_response,
             ),
         ]))
 
     def login(
         self,
         request,
@@ -59,23 +59,17 @@
         # by calling ``return redirect(auth.login)``.
         # But a better approach is to use the ``@login_required`` decorator
         # which will implicitly call this login view when needed.
         config_error = self._get_configuration_error()
         if config_error:
             return self._render_auth_error(
                 request, error="configuration_error", error_description=config_error)
-        redirect_uri = request.build_absolute_uri(
-            self._redirect_view) if self._redirect_view else None
-        if redirect_uri != self._redirect_uri:
-            logger.warning(
-                "redirect_uri mismatch: configured = %s, calculated = %s",
-                self._redirect_uri, redirect_uri)
         log_in_result = self._build_auth(request.session).log_in(
             scopes=scopes,  # Have user consent to scopes (if any) during log-in
-            redirect_uri=redirect_uri,  # Optional. If present, this absolute URL must match your app's redirect_uri registered in Azure Portal
+            redirect_uri=self._redirect_uri,  # Optional. If present, this absolute URL must match your app's redirect_uri registered in Azure Portal
             prompt="select_account",  # Optional. More values defined in  https://openid.net/specs/openid-connect-core-1_0.html#AuthRequest
             next_link=next_link,
             )
         if "error" in log_in_result:
             return self._render_auth_error(
                 request,
                 error=log_in_result["error"],
```

### Comparing `identity-0.8.0/identity/flask.py` & `identity-0.8.1/identity/flask.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         if config_error:
             return self._render_auth_error(
                 error="configuration_error", error_description=config_error)
         log_in_result = self._auth.log_in(
             scopes=scopes,  # Have user consent to scopes (if any) during log-in
             redirect_uri=self._redirect_uri,
             prompt="select_account",  # Optional. More values defined in  https://openid.net/specs/openid-connect-core-1_0.html#AuthRequest
+            next_link=next_link,
             )
         if "error" in log_in_result:
             return self._render_auth_error(
                 error=log_in_result["error"],
                 error_description=log_in_result.get("error_description"),
                 )
         return render_template("identity/login.html", **dict(
```

### Comparing `identity-0.8.0/identity/quart.py` & `identity-0.8.1/identity/quart.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         if config_error:
             return await self._render_auth_error(
                 error="configuration_error", error_description=config_error)
         log_in_result = self._auth.log_in(
             scopes=scopes,  # Have user consent to scopes (if any) during log-in
             redirect_uri=self._redirect_uri,
             prompt="select_account",  # Optional. More values defined in  https://openid.net/specs/openid-connect-core-1_0.html#AuthRequest
+            next_link=next_link,
             )
         if "error" in log_in_result:
             return await self._render_auth_error(
                 error=log_in_result["error"],
                 error_description=log_in_result.get("error_description"),
                 )
         return await render_template("identity/login.html", **dict(
```

### Comparing `identity-0.8.0/identity/templates/identity/auth_error.html` & `identity-0.8.1/identity/templates/identity/auth_error.html`

 * *Files identical despite different names*

### Comparing `identity-0.8.0/identity/templates/identity/login.html` & `identity-0.8.1/identity/templates/identity/login.html`

 * *Files identical despite different names*

### Comparing `identity-0.8.0/identity/web.py` & `identity-0.8.1/identity/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,23 @@
         app = self._build_msal_app()  # Only need a PCA at this moment
         if redirect_uri:
             flow = app.initiate_auth_code_flow(
                 _scopes, redirect_uri=redirect_uri, state=state, prompt=prompt)
         else:
             if state:
                 logger.warning("state only works in redirect_uri mode")
-            flow = app.initiate_device_flow(_scopes)
+            try:
+                flow = app.initiate_device_flow(_scopes)
+            except ValueError:  # Either Device Code endpoint unavailable or JsonDecodeError
+                return {
+                    "error": "configuration_error",
+                    "error_description":
+                        "This authority does not support device code flow. "
+                        "Please configure a redirect_uri to use auth code flow.",
+                    }
         if "error" in flow:
             return flow
         flow[self._EXPLICITLY_REQUESTED_SCOPES] = _scopes  # Can be different than the flow["scope"] which is possibly injected by OIDC library
         flow[self.__NEXT_LINK] = next_link
         self._session[self._AUTH_FLOW] = flow
         if redirect_uri:
             return {
```

### Comparing `identity-0.8.0/identity.egg-info/PKG-INFO` & `identity-0.8.1/identity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: identity
-Version: 0.8.0
+Version: 0.8.1
 Summary: This is an authentication/authorization library, currently optimized for web apps. It provides some higher level APIs built on top of Microsoft's MSAL Python.
 Home-page: https://github.com/rayluo/identity
 Author: Ray Luo
 Author-email: rayluo.mba@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/rayluo/identity/releases
 Project-URL: Documentation, https://identity-library.readthedocs.io/
@@ -103,15 +103,15 @@
 
 By using this library, it will automatically renew signed-in session when the ID token expires.
 
 * [Sample written in ![Django](https://raw.githubusercontent.com/rayluo/identity/dev/docs/django.webp)](https://github.com/Azure-Samples/ms-identity-python-webapp-django)
 * [Sample written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-python-webapp)
 * [Sample written in ![Quart](https://raw.githubusercontent.com/rayluo/identity/dev/docs/quart.webp)](https://github.com/rayluo/python-webapp-quart)
 * Need support for more web frameworks?
-  [Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues)
+  [Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues?q=is%3Aissue+is%3Aopen+sort%3Areactions-%2B1-desc)
 
 </td>
   </tr>
 
   <tr>
     <th>How to customize the login page</th>
     <td colspan=4>
@@ -157,16 +157,15 @@
 </td>
   </tr>
 
   <tr>
     <th>Other scenarios</th>
     <td colspan=4>
 
-[Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues)
-<!-- FastAPI, Streamlit, ... -->
+[Upvote existing feature request or create a new one](https://github.com/rayluo/identity/issues?q=is%3Aissue+is%3Aopen+sort%3Areactions-%2B1-desc)
 
 </td>
   </tr>
 
 </table>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: identity Version: 0.8.0 Summary: This is an
+Metadata-Version: 2.1 Name: identity Version: 0.8.1 Summary: This is an
 authentication/authorization library, currently optimized for web apps. It
 provides some higher level APIs built on top of Microsoft's MSAL Python. Home-
 page: https://github.com/rayluo/identity Author: Ray Luo Author-email:
 rayluo.mba@gmail.com License: MIT Project-URL: Changelog, https://github.com/
 rayluo/identity/releases Project-URL: Documentation, https://identity-
 library.readthedocs.io/ Keywords: identity,auth,authentication,authorization
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
@@ -68,15 +68,16 @@
 |            |/github.com/Azure-Samples/ms-identity-python-webapp-django) * [Sample   |
 |WWeebb AApppp SSiiggnn|written in ![Flask](https://raw.githubusercontent.com/rayluo/identity/  |
 |IInn && SSiiggnn   |dev/docs/flask.webp)](https://github.com/Azure-Samples/ms-identity-     |
 |OOuutt         |python-webapp) * [Sample written in ![Quart](https://                   |
 |            |raw.githubusercontent.com/rayluo/identity/dev/docs/quart.webp)](https://|
 |            |github.com/rayluo/python-webapp-quart) * Need support for more web      |
 |            |frameworks? [Upvote existing feature request or create a new one](https:|
-|_ _ _ _ _ _ _ _ _ _ _ _ _|_/_/_g_i_t_h_u_b_._c_o_m_/_r_a_y_l_u_o_/_i_d_e_n_t_i_t_y_/_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
+|            |//github.com/rayluo/identity/                                           |
+|_ _ _ _ _ _ _ _ _ _ _ _ _|_i_s_s_u_e_s_?_q_=_i_s_%_3_A_i_s_s_u_e_+_i_s_%_3_A_o_p_e_n_+_s_o_r_t_%_3_A_r_e_a_c_t_i_o_n_s_-_%_2_B_1_-_d_e_s_c_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |HHooww ttoo      |The default login page will typically redirect users to your Identity   |
 |ccuussttoommiizzee   |Provider, so you don't have to customize it. But if the default login   |
 |tthhee llooggiinn   |page is shown in your browser, you can read its HTML source code, and   |
 |_pp_aa_gg_ee_ _ _ _ _ _ _ _ _|_f_i_n_d_ _t_h_e_ _h_o_w_-_t_o_ _i_n_s_t_r_u_c_t_i_o_n_s_ _t_h_e_r_e_._ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |WWeebb AApppp     |This library supports: + Incremental consent. If the user needs to      |
 |CCaallllss aa wweebb |consent to more permissions, the library will automatically redirect the|
 |AAPPII         |user to the consent page. + Automatically cache the access token and    |
@@ -87,15 +88,16 @@
 |AAPPII ((OOnn--    |                                                                        |
 |_bb_ee_hh_aa_ll_ff_--_oo_ff_))_ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |HHooww ttoo bbuuiilldd|                                                                        |
 |tthhee ssaammpplleess |Read our [docs here](https://identity-library.readthedocs.io/en/latest/)|
 |aabboovvee ffrroomm  |                                                                        |
 |_ss_cc_rr_aa_tt_cc_hh_ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |OOtthheerr       |[Upvote existing feature request or create a new one](https://          |
-|_ss_cc_ee_nn_aa_rr_ii_oo_ss_ _ _ _|_g_i_t_h_u_b_._c_o_m_/_r_a_y_l_u_o_/_i_d_e_n_t_i_t_y_/_i_s_s_u_e_s_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
+|sscceennaarriiooss   |github.com/rayluo/identity/                                             |
+|_ _ _ _ _ _ _ _ _ _ _ _ _|_i_s_s_u_e_s_?_q_=_i_s_%_3_A_i_s_s_u_e_+_i_s_%_3_A_o_p_e_n_+_s_o_r_t_%_3_A_r_e_a_c_t_i_o_n_s_-_%_2_B_1_-_d_e_s_c_)_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 ## Installation This package is [available on PyPI](https://pypi.org/project/
 identity/). Choose the package declaration that matches your web framework: *
 Django: `pip install identity[django]` * Flask: `pip install identity[flask]` *
 Quart: `pip install identity[quart]` ## Versions This library follows [Semantic
 Versioning](http://semver.org/). Your project should declare `identity`
 dependency with proper lower and upper bound. You can find the changes for each
 version under [Releases](https://github.com/rayluo/identity/releases).
```

### Comparing `identity-0.8.0/setup.cfg` & `identity-0.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `identity-0.8.0/tests/test_django.py` & `identity-0.8.1/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `identity-0.8.0/tests/test_quart.py` & `identity-0.8.1/tests/test_quart.py`

 * *Files identical despite different names*

