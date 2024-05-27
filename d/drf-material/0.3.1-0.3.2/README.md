# Comparing `tmp/drf_material-0.3.1.tar.gz` & `tmp/drf_material-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_material-0.3.1.tar", max compression
+gzip compressed data, was "drf_material-0.3.2.tar", max compression
```

## Comparing `drf_material-0.3.1.tar` & `drf_material-0.3.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1074 2024-05-18 17:44:32.203850 drf_material-0.3.1/LICENSE
--rw-r--r--   0        0        0     3088 2024-05-18 17:44:32.203850 drf_material-0.3.1/README.md
--rw-r--r--   0        0        0       87 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/__init__.py
--rw-r--r--   0        0        0      235 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/apps.py
--rw-r--r--   0        0        0    24397 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1882 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      684 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      606 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0     1004 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1762 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1636 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1617 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1373 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1411 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      962 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     1004 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/checkbox.html
--rw-r--r--   0        0        0     1766 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/form.html
--rw-r--r--   0        0        0     1307 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/input.html
--rw-r--r--   0        0        0      262 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/list_field.html
--rw-r--r--   0        0        0      330 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/radio.html
--rw-r--r--   0        0        0     1481 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/select.html
--rw-r--r--   0        0        0     1411 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/select_multiple.html
--rw-r--r--   0        0        0     1077 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/inline/textarea.html
--rw-r--r--   0        0        0     3631 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1912 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0     1272 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      298 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0     1004 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/checkbox.html
--rw-r--r--   0        0        0     1766 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/form.html
--rw-r--r--   0        0        0     1281 2024-05-18 17:44:32.207850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/input.html
--rw-r--r--   0        0        0      262 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/list_field.html
--rw-r--r--   0        0        0      330 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/radio.html
--rw-r--r--   0        0        0     1455 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/select.html
--rw-r--r--   0        0        0     1473 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/select_multiple.html
--rw-r--r--   0        0        0     1051 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templates/rest_framework/vertical/textarea.html
--rw-r--r--   0        0        0       51 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templatetags/__init__.py
--rw-r--r--   0        0        0     1681 2024-05-18 17:44:32.211850 drf_material-0.3.1/drf_material/templatetags/rest_framework_material.py
--rw-r--r--   0        0        0      548 2024-05-18 17:44:32.211850 drf_material-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3943 1970-01-01 00:00:00.000000 drf_material-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-27 06:45:44.176651 drf_material-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3088 2024-05-27 06:45:44.176651 drf_material-0.3.2/README.md
+-rw-r--r--   0        0        0       87 2024-05-27 06:45:44.176651 drf_material-0.3.2/drf_material/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-27 06:45:44.176651 drf_material-0.3.2/drf_material/apps.py
+-rw-r--r--   0        0        0    24420 2024-05-27 06:45:44.176651 drf_material-0.3.2/drf_material/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1882 2024-05-27 06:45:44.176651 drf_material-0.3.2/drf_material/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      684 2024-05-27 06:45:44.176651 drf_material-0.3.2/drf_material/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      606 2024-05-27 06:45:44.176651 drf_material-0.3.2/drf_material/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0     1004 2024-05-27 06:45:44.176651 drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1762 2024-05-27 06:45:44.176651 drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-27 06:45:44.176651 drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-27 06:45:44.176651 drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1636 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1617 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1373 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1411 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      962 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     1004 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/inline/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/inline/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/inline/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/inline/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/inline/form.html
+-rw-r--r--   0        0        0     1307 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/inline/input.html
+-rw-r--r--   0        0        0      262 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/inline/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/inline/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/inline/radio.html
+-rw-r--r--   0        0        0     1481 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/inline/select.html
+-rw-r--r--   0        0        0     1411 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/inline/select_multiple.html
+-rw-r--r--   0        0        0     1077 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/inline/textarea.html
+-rw-r--r--   0        0        0     3631 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1912 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0     1272 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      298 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0     1004 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/vertical/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/vertical/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/vertical/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/vertical/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/vertical/form.html
+-rw-r--r--   0        0        0     1281 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/vertical/input.html
+-rw-r--r--   0        0        0      262 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/vertical/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/vertical/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/vertical/radio.html
+-rw-r--r--   0        0        0     1455 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/vertical/select.html
+-rw-r--r--   0        0        0     1473 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/vertical/select_multiple.html
+-rw-r--r--   0        0        0     1051 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templates/rest_framework/vertical/textarea.html
+-rw-r--r--   0        0        0       51 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templatetags/__init__.py
+-rw-r--r--   0        0        0     1860 2024-05-27 06:45:44.180651 drf_material-0.3.2/drf_material/templatetags/rest_framework_material.py
+-rw-r--r--   0        0        0      548 2024-05-27 06:45:44.180651 drf_material-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3943 1970-01-01 00:00:00.000000 drf_material-0.3.2/PKG-INFO
```

### Comparing `drf_material-0.3.1/LICENSE` & `drf_material-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/README.md` & `drf_material-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/api.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/api.html`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,17 @@
     <link href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap" rel="stylesheet" />
     <link href="https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/6.4.2/mdb.min.css" rel="stylesheet"/>
     <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@latest/font/bootstrap-icons.css">
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/a11y-light.min.css">
   {% endblock %}
 
   <style>
-    {% if code_style %}{{ code_style }}{% endif %}
+    {% if code_style %}
+      {{ code_style }}
+    {% endif %}
 
     .dropdown-toggle::after {
       content: none;
     }
   </style>
 {% endblock %}
 
@@ -110,15 +112,15 @@
                       <li>
                         <h5 class="dropdown-header">
                           {% translate 'Account' %}
                         </h5>
                       </li>
                       <li>
                         {% if user.is_authenticated %}
-                          {% optional_logout request user %}
+                          {% optional_logout request user csrf_token %}
                         {% else %}
                           {% optional_login request %}
                         {% endif %}
                       </li>
                     </ul>
                   </li>
                 </ul>
```

#### html2text {}

```diff
@@ -7,16 +7,16 @@
     * _{{_%%_ _tt_rr_aa_nn_ss_ll_aa_tt_ee_ _""_HH_oo_mm_ee_""_ _%%_}}
     * _{{_%%_ _tt_rr_aa_nn_ss_ll_aa_tt_ee_ _""_TT_uu_tt_oo_rr_ii_aa_ll_""_ _%%_}}
     * _{{_%%_ _tt_rr_aa_nn_ss_ll_aa_tt_ee_ _""_GG_ii_tt_hh_uu_bb_""_ _%%_}}
     * _{{_%%_ _tt_rr_aa_nn_ss_ll_aa_tt_ee_ _""_MM_aa_tt_ee_rr_ii_aa_ll_""_ _%%_}}
     * _{{_%%_ _ii_ff_ _uu_ss_ee_rr_.._ii_ss____aa_uu_tt_hh_ee_nn_tt_ii_cc_aa_tt_ee_dd_ _%%_}}_ _{{_{{_ _rr_ee_qq_uu_ee_ss_tt_.._uu_ss_ee_rr_||_cc_aa_pp_ff_ii_rr_ss_tt_ _}}_}}_ _{{_%%_ _ee_ll_ss_ee_ _%%_}}_ _{{_%%
       _tt_rr_aa_nn_ss_ll_aa_tt_ee_ _""_AA_cc_cc_oo_uu_nn_tt_""_ _%%_}}_ _{{_%%_ _ee_nn_dd_ii_ff_ _%%_}}
           o **** {{%% ttrraannssllaattee ''AAccccoouunntt'' %%}} ****
-          o {% if user.is_authenticated %} {% optional_logout request user %}
-            {% else %} {% optional_login request %} {% endif %}
+          o {% if user.is_authenticated %} {% optional_logout request user
+            csrf_token %} {% else %} {% optional_login request %} {% endif %}
 {% endblock %} {% block breadcrumbs %}
    1. {% for breadcrumb_name, breadcrumb_url in breadcrumblist %} {% if
       forloop.last %}
    2. {{ breadcrumb_name }}
    3. {% else %}
    4. _{_{_ _b_r_e_a_d_c_r_u_m_b___n_a_m_e_ _}_}
    5. {% endif %} {% empty %} {% block breadcrummdb_empty %}&nmdbp;{% endblock
```

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/filters/base.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/filters/ordering.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/filters/search.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/checkbox.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/checkbox_multiple.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/input.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/radio.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/select.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/select_multiple.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/horizontal/textarea.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/inline/checkbox.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/inline/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/inline/checkbox_multiple.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/inline/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/inline/input.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/inline/input.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/inline/radio.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/inline/radio.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/inline/select.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/inline/select.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/inline/select_multiple.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/inline/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/inline/textarea.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/inline/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/login.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/login.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/pagination/numbers.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/pagination/previous_and_next.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/vertical/checkbox.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/vertical/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/vertical/checkbox_multiple.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/vertical/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/vertical/input.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/vertical/input.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/vertical/radio.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/vertical/radio.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/vertical/select.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/vertical/select.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/vertical/select_multiple.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/vertical/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templates/rest_framework/vertical/textarea.html` & `drf_material-0.3.2/drf_material/templates/rest_framework/vertical/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_material-0.3.1/drf_material/templatetags/rest_framework_material.py` & `drf_material-0.3.2/drf_material/templatetags/rest_framework_material.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,54 +12,63 @@
 
 @register.simple_tag
 def optional_login(request):
     """Include a login snippet if REST framework's login view is in the URLconf."""
 
     try:
         login_url = reverse("rest_framework:login")
+
     except NoReverseMatch:
         return ""
 
     snippet = """
     <a class="dropdown-item" href="{href}?next={next}">
-        <strong class="d-flex align-items-center gap-3">
-            <i class="bi bi-box-arrow-in-right"></i>
-            Login
-        </strong>
+      <strong class="d-flex align-items-center gap-3">
+        <i class="bi bi-box-arrow-in-right"></i>
+        Login
+      </strong>
     </a>"""
+
     snippet = format_html(
         snippet,
         href=login_url,
         next=escape(request.path),
     )
 
     return mark_safe(snippet)
 
 
 @register.simple_tag
-def optional_logout(request, user):
+def optional_logout(request, user, csrf_token):
     """Include a logout snippet if REST framework's logout view is in the URLconf."""
 
     try:
         logout_url = reverse("rest_framework:logout")
+
     except NoReverseMatch:
         snippet = format_html(
             '<li class="dropdown-item">{user}</li>',
             user=escape(user),
         )
         return mark_safe(snippet)
 
     snippet = """
-    <a class="dropdown-item" href="{href}?next={next}">
+    <form method="post" action="{href}?next={next}">
+      <input type="hidden" name="csrfmiddlewaretoken" value="{csrf_token}">
+    
+      <button type="submit" class="dropdown-item">
         <strong class="d-flex align-items-center gap-3">
-            <i class="bi bi-box-arrow-right"></i>
-            Logout
+          <i class="bi bi-box-arrow-right"></i>
+          Logout
         </strong>
-    </a>"""
+      </button>
+    </form>"""
+
     snippet = format_html(
         snippet,
         user=escape(user),
         href=logout_url,
         next=escape(request.path),
+        csrf_token=csrf_token,
     )
 
     return mark_safe(snippet)
```

### Comparing `drf_material-0.3.1/pyproject.toml` & `drf_material-0.3.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-material"
-version = "0.3.1"
+version = "0.3.2"
 description = "Material design for Django REST Framework API"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "drf_material"}]
 homepage = "https://github.com/youzarsiph/drf-material/"
 repository = "https://github.com/youzarsiph/drf-material/"
```

### Comparing `drf_material-0.3.1/PKG-INFO` & `drf_material-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-material
-Version: 0.3.1
+Version: 0.3.2
 Summary: Material design for Django REST Framework API
 Home-page: https://github.com/youzarsiph/drf-material/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

