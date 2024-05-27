# Comparing `tmp/nebari_jupyterhub_theme-2023.4.1.tar.gz` & `tmp/nebari_jupyterhub_theme-2024.5.1.tar.gz`

## Comparing `nebari_jupyterhub_theme-2023.4.1.tar` & `nebari_jupyterhub_theme-2024.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/__init__.py
--rw-r--r--   0        0        0    54444 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Bold.ttf
--rw-r--r--   0        0        0    53504 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Regular.ttf
--rw-r--r--   0        0        0   153944 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/Poppins-Bold.ttf
--rw-r--r--   0        0        0   158240 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/Poppins-Regular.ttf
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/images/Nebari-Logo-Horizontal-Lockup-White-text.svg
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/images/Nebari-logo-square.svg
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/templates/login.html
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/templates/page.html
--rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/templates/style.css
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/LICENSE
--rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/README.md
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/pyproject.toml
--rw-r--r--   0        0        0    13236 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2023.4.1/PKG-INFO
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/__init__.py
+-rw-r--r--   0        0        0    54444 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Bold.ttf
+-rw-r--r--   0        0        0    53504 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Regular.ttf
+-rw-r--r--   0        0        0   153944 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/custom/css/Poppins-Bold.ttf
+-rw-r--r--   0        0        0   158240 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/custom/css/Poppins-Regular.ttf
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/custom/images/Nebari-Logo-Horizontal-Lockup-White-text.svg
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/custom/images/Nebari-logo-square.svg
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/templates/login.html
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/templates/page.html
+-rw-r--r--   0        0        0     8629 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/templates/style.css
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/LICENSE
+-rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/README.md
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/pyproject.toml
+-rw-r--r--   0        0        0    13243 2020-02-02 00:00:00.000000 nebari_jupyterhub_theme-2024.5.1/PKG-INFO
```

### Comparing `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Bold.ttf` & `nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Bold.ttf`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Regular.ttf` & `nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/custom/css/AtkinsonHyperlegible-Regular.ttf`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/Poppins-Bold.ttf` & `nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/custom/css/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/css/Poppins-Regular.ttf` & `nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/custom/css/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/images/Nebari-Logo-Horizontal-Lockup-White-text.svg` & `nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/custom/images/Nebari-Logo-Horizontal-Lockup-White-text.svg`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/custom/images/Nebari-logo-square.svg` & `nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/custom/images/Nebari-logo-square.svg`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/templates/login.html` & `nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/templates/login.html`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/templates/page.html` & `nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/templates/page.html`

 * *Files 26% similar despite different names*

```diff
@@ -2,44 +2,62 @@
 <!-- Distributed under the terms of the Modified BSD License. -->
 
 {% extends "templates/page.html" %}
 
 {% block nav_bar_left_items %}
 
 <!-- Default nav bar items -->
-<li><a href="{{base_url}}home {% if cdsdashboards_restricted %}-cds{% endif %}">Home</a></li>
-<li><a href="{{base_url}}token">Token</a></li>
+<li class="nav-item"><a class="nav-link" href="{{base_url}}home {% if cdsdashboards_restricted %}-cds{% endif %}">Home</a></li>
+<li class="nav-item"><a class="nav-link" href="{{base_url}}token">Token</a></li>
 
 <!-- Access to admin dashboard -->
 {% if user.admin %}
-<li><a href="{{base_url}}admin">Admin</a></li>
+<li class="nav-item"><a class="nav-link" href="{{base_url}}admin">Admin</a></li>
 {% endif %}
 
 {% if services %}
-<li class="dropdown">
+<li class="nav-item dropdown">
     <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">Services<span class="caret"></span></a>
     <ul class="dropdown-menu">
     {% for service in services %}
     <li><a class="dropdown-item" href="{{service.prefix}}">{{service.name}}</a></li>
     {% endfor %}
     </ul>
 </li>
 {% endif %}
 
 <!-- Custom integrations-->
-<li><a href="/auth/admin/nebari/console/">User Management</a></li>
-<li><a href="/argo">Argo Workflows</a></li>
+<li class="nav-item"><a class="nav-link" href="/auth/admin/nebari/console/">User Management</a></li>
+<li class="nav-item"><a class="nav-link" href="/argo">Argo Workflows</a></li>
 {% if cdsdashboards_enabled %}
-    <li><a href="{{ base_url }}dashboards">Dashboards</a></li>
+    <li class="nav-item"><a class="nav-link" href="{{ base_url }}dashboards">Dashboards</a></li>
 {% endif %}
-<li><a href="/conda-store">Environment Management</a></li>
-<li><a href="/monitoring">Monitoring</a></li>
+<li class="nav-item"><a class="nav-link" href="/conda-store">Environment Management</a></li>
+<li class="nav-item"><a class="nav-link" href="/monitoring">Monitoring</a></li>
 
 {% endblock nav_bar_left_items %}
 
+<!-- Switch login button to light -->
+{% block login_widget %}
+<span id="login_widget">
+  {% if user %}
+    <span class="navbar-text me-1">{{ user.name }}</span>
+    <a id="logout"
+       role="button"
+       class="btn btn-sm btn-outline-light"
+       href="{{ logout_url }}"> <i aria-hidden="true" class="fa fa-sign-out"></i> Logout</a>
+  {% else %}
+    <a id="login"
+       role="button"
+       class="btn btn-sm btn-outline-light"
+       href="{{ login_url }}">Login</a>
+  {% endif %}
+</span>
+{% endblock login_widget %}
+
 {% block footer %}
 {% if display_version %}
 <div class="version">
   {{ version or 'v0.0.1'}}
 </div>
 {% endif %}
 {% endblock footer%}
```

#### html2text {}

```diff
@@ -12,15 +12,19 @@
 _U_s_e_r_ _M_a_n_a_g_e_m_e_n_t
 _A_r_g_o_ _W_o_r_k_f_l_o_w_s
 {% if cdsdashboards_enabled %}
 _D_a_s_h_b_o_a_r_d_s
 {% endif %}
 _E_n_v_i_r_o_n_m_e_n_t_ _M_a_n_a_g_e_m_e_n_t
 _M_o_n_i_t_o_r_i_n_g
-{% endblock nav_bar_left_items %} {% block footer %} {% if display_version %}
+{% endblock nav_bar_left_items %} {% block login_widget %} {% if user %} {
+{ user.name }}
+_L_o_g_o_u_t
+ {% else %} _L_o_g_i_n {% endif %} {% endblock login_widget %} {% block footer %} {%
+if display_version %}
 {{ version or 'v0.0.1'}}
 {% endif %} {% endblock footer%} {% block stylesheet %}
 }" type="text/css"/>
 {% if cdsdashboards_enabled %}
 {% endif %} {% set jsurls = nebari_theme_extra_js_urls | default([]) %} {% for
 jsurl in jsurls %}
 {% endfor %} {% endblock stylesheet %} {% block logo %} _[_J_u_p_y_t_e_r_H_u_b_ _l_o_g_o_ _-
```

### Comparing `nebari_jupyterhub_theme-2023.4.1/nebari_jupyterhub_theme/templates/style.css` & `nebari_jupyterhub_theme-2024.5.1/nebari_jupyterhub_theme/templates/style.css`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     --h4-font-size: 1rem;
     --h5-font-size: 0.875rem;
     --h6-font-size: 0.85rem;
 
     /*  Colors */
     --heading-color: {{ h1_color | default("#0f1015") }};
     --text-color: {{ text_color | default("#1c1d26") }};
-    --link-text-color: {{ text_color | default("#1c1d26") }};
+    --link-text-color: {{ text_color | default("#20b1a8") }};
     --primary-color: {{ primary_color | default("#9e17b7") }};
     --primary-color-dark: #79158a;
     --secondary-color: {{ secondary_color | default("#2bd1c5") }};
     --secondary-color-dark: #20b1a8;
     --accent-color: {{ accent_color | default("#eda61d") }};
     --accent-color-dark: #a16d14;
     --navbar-background-color: {{ navbar_color | default("#1c1d26") }};
@@ -85,51 +85,59 @@
 
 label {
     font-family: var(--base-font-family);
 }
 
 a{
     color: var(--link-text-color);
+    text-decoration: underline;
     text-decoration-color: CurrentColor;
     text-underline-offset: 1px;
 }
 
 /* Navbar  */
-.nav{
+.navbar-nav {
     margin-left:10px;
 }
 
-.navbar.navbar-default {
-    background: var(--navbar-background-color);
+.navbar.bg-body-tertiary {
+    background: var(--navbar-background-color)!important;
     box-shadow: 0px 1.5px 3px 0px rgba(72, 74, 94, 0.16);
     border: None;
 }
 
-.navbar.navbar-default .navbar-nav>li>a,
-.navbar.navbar-default .navbar-text {
+.navbar.bg-body-tertiary .navbar-nav>li>a,
+.navbar.bg-body-tertiary .navbar-text {
     color: var(--navbar-text-color);
     text-decoration: none;
 }
 
+/* Spawner form */
+
+#kubespawner-profiles-list > label.profile {
+  margin-bottom: 12px;
+  padding-bottom: 0;
+}
+
 /* Authenticator form */
 #login-main .auth-form-header {
     background: var(--accent-color) !important;
     color: {{ accent_text_color | default("#1c1d26") }} ;
     font-family: var(--base-font-family);
 }
 
 #login-main .service-login {
     vertical-align: top !important;
     padding-top: 60px;
 }
 
 /* Focus states */
 
-.navbar.navbar-default .navbar-nav>li>a:focus,
-.navbar.navbar-default .navbar-nav>.open>a:focus,
+.navbar.bg-body-tertiary .navbar-nav>li>a:focus,
+.navbar.bg-body-tertiary .navbar-nav>.open>a:focus,
 a:focus {
     color: var(--text-color);
     background-color: var(--accent-color);
     box-shadow: 0 -2px var(--accent-color), 0 2px var(--text-color);
     text-decoration: none;
     outline: none;
     outline-offset: none;
@@ -187,22 +195,22 @@
 /* Hover states */
 a:hover{
     color: var(--link-hover-color);
     text-decoration: underline;
     text-decoration-thickness: var(--text-decoration-thickness);
 }
 
-.navbar.navbar-default .navbar-nav>li>a:hover {
+.navbar.bg-body-tertiary .navbar-nav>li>a:hover {
     color: var(--text-color);
     background-color: var(--navbar-hover-color);
     text-decoration: underline;
 }
 
-.navbar.navbar-default .navbar-nav>.open>a,
-.navbar.navbar-default .navbar-nav>.open>a:hover{
+.navbar.bg-body-tertiary .navbar-nav>.open>a,
+.navbar.bg-body-tertiary .navbar-nav>.open>a:hover{
     background-color: {{ navbar_hover_color | default("#00a3b0") }};
 }
 
 
 .btn:hover{
     box-shadow: var(--button-hover-shadow);
 }
```

### Comparing `nebari_jupyterhub_theme-2023.4.1/LICENSE` & `nebari_jupyterhub_theme-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.4.1/README.md` & `nebari_jupyterhub_theme-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nebari_jupyterhub_theme-2023.4.1/pyproject.toml` & `nebari_jupyterhub_theme-2024.5.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 # Distributed under the terms of the Modified BSD License.
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nebari-jupyterhub-theme"
-version = "2023.4.1"
+version = "2024.5.1"
 description = "Nebari JupyterHub theme"
 readme = "README.md"
 license = "BSD-3-Clause"
 requires-python = ">=3.8"
 maintainers = [{ name = "Nebari development team" }]
 keywords = ["jupyterhub", "theme"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Topic :: Software Development :: Build Tools",
     "Operating System :: OS Independent",
 ]
-dependencies = ["jupyterhub"]
+dependencies = ["jupyterhub>=5.0.0"]
 
 [project.urls]
 "Bug Reports" = "https://github.com/nebari-dev/nebari-jupyterhub-theme/issues"
 Homepage = "https://nebari.dev"
 "Source code" = "https://github.com/nebari-dev/nebari-jupyterhub-theme"
 
 [tool.hatch.build.targets.sdist]
```

### Comparing `nebari_jupyterhub_theme-2023.4.1/PKG-INFO` & `nebari_jupyterhub_theme-2024.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: nebari-jupyterhub-theme
-Version: 2023.4.1
+Version: 2024.5.1
 Summary: Nebari JupyterHub theme
 Project-URL: Bug Reports, https://github.com/nebari-dev/nebari-jupyterhub-theme/issues
 Project-URL: Homepage, https://nebari.dev
 Project-URL: Source code, https://github.com/nebari-dev/nebari-jupyterhub-theme
 Maintainer: Nebari development team
 License-Expression: BSD-3-Clause
 License-File: LICENSE
@@ -12,15 +12,15 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.8
-Requires-Dist: jupyterhub
+Requires-Dist: jupyterhub>=5.0.0
 Description-Content-Type: text/markdown
 
 <p align="center">
 <picture>
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/nebari-dev/nebari-design/main/logo-mark/horizontal/Nebari-Logo-Horizontal-Lockup.svg">
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/nebari-dev/nebari-design/main/logo-mark/horizontal/Nebari-Logo-Horizontal-Lockup-White-text.svg">
   <img alt="Nebari logo mark - text will be black in light color mode and white in dark color mode." src="https://raw.githubusercontent.com/nebari-dev/nebari-design/main/logo-mark/horizontal/Nebari-Logo-Horizontal-Lockup-White-text.svg" width="50%"/>
```

