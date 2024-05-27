# Comparing `tmp/drf_redesign-0.3.8.tar.gz` & `tmp/drf_redesign-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_redesign-0.3.8.tar", max compression
+gzip compressed data, was "drf_redesign-0.3.9.tar", max compression
```

## Comparing `drf_redesign-0.3.8.tar` & `drf_redesign-0.3.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1074 2024-05-18 17:42:51.803383 drf_redesign-0.3.8/LICENSE
--rw-r--r--   0        0        0     3571 2024-05-18 17:42:51.803383 drf_redesign-0.3.8/README.md
--rw-r--r--   0        0        0       91 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/__init__.py
--rw-r--r--   0        0        0      235 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/apps.py
--rw-r--r--   0        0        0    28239 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1884 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      684 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      585 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0     1004 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1762 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1636 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1617 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1398 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1433 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0     1006 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     1004 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/checkbox.html
--rw-r--r--   0        0        0     1766 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/form.html
--rw-r--r--   0        0        0     1307 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/input.html
--rw-r--r--   0        0        0      262 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/list_field.html
--rw-r--r--   0        0        0      330 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/radio.html
--rw-r--r--   0        0        0     1487 2024-05-18 17:42:51.807383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/select.html
--rw-r--r--   0        0        0     1411 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/select_multiple.html
--rw-r--r--   0        0        0     1054 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/textarea.html
--rw-r--r--   0        0        0     5226 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/login.html
--rw-r--r--   0        0        0     2051 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0     1272 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      296 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0     1004 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/checkbox.html
--rw-r--r--   0        0        0     1766 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/dict_field.html
--rw-r--r--   0        0        0      427 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/fieldset.html
--rw-r--r--   0        0        0      150 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/form.html
--rw-r--r--   0        0        0     1281 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/input.html
--rw-r--r--   0        0        0      262 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/list_field.html
--rw-r--r--   0        0        0      330 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/radio.html
--rw-r--r--   0        0        0     1461 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/select.html
--rw-r--r--   0        0        0     1474 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/select_multiple.html
--rw-r--r--   0        0        0     1051 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/textarea.html
--rw-r--r--   0        0        0       51 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templatetags/__init__.py
--rw-r--r--   0        0        0     1682 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/drf_redesign/templatetags/rest_framework_redesign.py
--rw-r--r--   0        0        0      576 2024-05-18 17:42:51.811383 drf_redesign-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     4454 1970-01-01 00:00:00.000000 drf_redesign-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-27 06:46:25.016999 drf_redesign-0.3.9/LICENSE
+-rw-r--r--   0        0        0     3571 2024-05-27 06:46:25.016999 drf_redesign-0.3.9/README.md
+-rw-r--r--   0        0        0       91 2024-05-27 06:46:25.016999 drf_redesign-0.3.9/drf_redesign/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-27 06:46:25.016999 drf_redesign-0.3.9/drf_redesign/apps.py
+-rw-r--r--   0        0        0    25884 2024-05-27 06:46:25.016999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1884 2024-05-27 06:46:25.016999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      684 2024-05-27 06:46:25.016999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      585 2024-05-27 06:46:25.016999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0     1004 2024-05-27 06:46:25.016999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1762 2024-05-27 06:46:25.016999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-27 06:46:25.016999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-27 06:46:25.016999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-27 06:46:25.016999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1636 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1617 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1398 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1433 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0     1006 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     1004 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/form.html
+-rw-r--r--   0        0        0     1307 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/input.html
+-rw-r--r--   0        0        0      262 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/radio.html
+-rw-r--r--   0        0        0     1487 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/select.html
+-rw-r--r--   0        0        0     1411 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/select_multiple.html
+-rw-r--r--   0        0        0     1054 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/textarea.html
+-rw-r--r--   0        0        0     5226 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     2051 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0     1272 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      296 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0     1004 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/form.html
+-rw-r--r--   0        0        0     1281 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/input.html
+-rw-r--r--   0        0        0      262 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/radio.html
+-rw-r--r--   0        0        0     1461 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/select.html
+-rw-r--r--   0        0        0     1474 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/select_multiple.html
+-rw-r--r--   0        0        0     1051 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/textarea.html
+-rw-r--r--   0        0        0       51 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templatetags/__init__.py
+-rw-r--r--   0        0        0     1860 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/drf_redesign/templatetags/rest_framework_redesign.py
+-rw-r--r--   0        0        0      576 2024-05-27 06:46:25.020999 drf_redesign-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4454 1970-01-01 00:00:00.000000 drf_redesign-0.3.9/PKG-INFO
```

### Comparing `drf_redesign-0.3.8/LICENSE` & `drf_redesign-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/README.md` & `drf_redesign-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/api.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/api.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,604 +1,621 @@
 {% extends "rest_framework/base.html" %}
 
 {% load i18n static rest_framework rest_framework_redesign %}
 
 {% block meta %}
-  {{ block.super }}
-  <meta name="viewport" content="width=device-width, initial-scale=1.0">
+{{ block.super }}
+<meta name="viewport" content="width=device-width, initial-scale=1.0">
 {% endblock %}
 
 {% block style %}
-  {% block bootstrap_theme %}
-    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"
-      integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
-    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@latest/font/bootstrap-icons.css">
-    <link id="hljs-theme" rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/a11y-dark.min.css">
-  {% endblock %}
+{% block bootstrap_theme %}
+<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"
+  integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
+<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@latest/font/bootstrap-icons.css">
+<link id="hljs-theme" rel="stylesheet"
+  href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/a11y-dark.min.css">
+{% endblock %}
 
-  <style>
-    {% if code_style %}
-      {{ code_style }}
-    {% endif %}
+<style>
+  {% if code_style %}
+    {{code_style }}
+  {% endif %}
+
+  .dropdown-toggle::after {
+    content: none;
+  }
+</style>
 
-    .dropdown-toggle::after {
-      content: none;
-    }
-  </style>
- 
-  <script>
+<script>
   /*!
     * Color mode toggler for Bootstrap's docs (https://getbootstrap.com/)
     * Copyright 2011-2023 The Bootstrap Authors
     * Licensed under the Creative Commons Attribution 3.0 Unported License.
     */
 
-    (() => {
-      'use strict'
-
-      const getStoredTheme = () => localStorage.getItem('theme')
-      const setStoredTheme = theme => localStorage.setItem('theme', theme)
+  (() => {
+    'use strict'
 
-      const getPreferredTheme = () => {
-        const storedTheme = getStoredTheme()
-        if (storedTheme) {
-          return storedTheme
-        }
+    const getStoredTheme = () => localStorage.getItem('theme')
+    const setStoredTheme = theme => localStorage.setItem('theme', theme)
 
-        return window.matchMedia('(prefers-color-scheme: dark)').matches ? 'dark' : 'light'
+    const getPreferredTheme = () => {
+      const storedTheme = getStoredTheme()
+      if (storedTheme) {
+        return storedTheme
       }
 
-      const setTheme = theme => {
-        if (theme === 'auto' && window.matchMedia('(prefers-color-scheme: dark)').matches) {
-          document.documentElement.setAttribute('data-bs-theme', 'dark')
-          document.getElementById('hljs-theme').setAttribute('href', 'https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/a11y-dark.min.css')
+      return window.matchMedia('(prefers-color-scheme: dark)').matches ? 'dark' : 'light'
+    }
+
+    const setTheme = theme => {
+      if (theme === 'auto' && window.matchMedia('(prefers-color-scheme: dark)').matches) {
+        document.documentElement.setAttribute('data-bs-theme', 'dark')
+        document.getElementById('hljs-theme').setAttribute('href', 'https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/a11y-dark.min.css')
+      } else {
+        document.documentElement.setAttribute('data-bs-theme', theme)
+        if (theme === 'light') {
+          document.getElementById('hljs-theme').setAttribute('href', 'https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/a11y-light.min.css')
         } else {
-          document.documentElement.setAttribute('data-bs-theme', theme)
-          if (theme === 'light') {
-            document.getElementById('hljs-theme').setAttribute('href', 'https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/a11y-light.min.css')
-          } else {
-            document.getElementById('hljs-theme').setAttribute('href', 'https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/a11y-dark.min.css')
-          }
+          document.getElementById('hljs-theme').setAttribute('href', 'https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/a11y-dark.min.css')
         }
       }
+    }
 
-      setTheme(getPreferredTheme())
+    setTheme(getPreferredTheme())
 
-      window.matchMedia('(prefers-color-scheme: dark)').addEventListener('change', () => {
-        const storedTheme = getStoredTheme()
-        if (storedTheme !== 'light' && storedTheme !== 'dark') {
-          setTheme(getPreferredTheme())
-        }
-      })
+    window.matchMedia('(prefers-color-scheme: dark)').addEventListener('change', () => {
+      const storedTheme = getStoredTheme()
+      if (storedTheme !== 'light' && storedTheme !== 'dark') {
+        setTheme(getPreferredTheme())
+      }
+    })
 
-      window.addEventListener('DOMContentLoaded', () => {
-        document.querySelectorAll('[data-bs-theme-value]')
-          .forEach(toggle => {
-            toggle.addEventListener('click', () => {
-              const theme = toggle.getAttribute('data-bs-theme-value')
-              setStoredTheme(theme)
-              setTheme(theme)
-            })
+    window.addEventListener('DOMContentLoaded', () => {
+      document.querySelectorAll('[data-bs-theme-value]')
+        .forEach(toggle => {
+          toggle.addEventListener('click', () => {
+            const theme = toggle.getAttribute('data-bs-theme-value')
+            setStoredTheme(theme)
+            setTheme(theme)
           })
-      })
-    })()
+        })
+    })
+  })()
 </script>
 {% endblock %}
 
 
 {% block navbar %}
-  <header class="fixed-top p-1 p-md-2">
-    <div class="bg-danger px-2 px-md-3 shadow-sm rounded-4 border border-danger">
-      <div class="bg-dark px-2 px-md-3 rounded-4 shadow-sm">
-        <div class="bg-danger px-2 px-md-3 rounded-4 shadow-sm">
-          <nav class="navbar navbar-expand-lg navbar-dark bg-dark rounded-4 shadow-sm {% block bootstrap_navbar_variant %}{% endblock %}"
-            role="navigation" aria-label="{% translate 'navbar' %}">
-            <div class="container-fluid">
-              {% block branding %}
-                <a class="navbar-brand d-flex align-item-center justify-content-center gap-1 bg-white rounded-4 px-2 shadow-sm" rel="nofollow"
-                  href="https://www.django-rest-framework.org/">
-                  <span class="fw-bold text-danger">[</span>
-                  <span class="fw-bold text-dark">{</span>
-                  <strong class="text-dark d-flex align-item-center justify-content-center">
-                    <abbr title="Django Rest Framework" data-bs-toggle="tooltip" class="text-decoration-none">
-                      {% translate 'DRF' %}
-                    </abbr>
-                  </strong>
-                  <span class="fw-bold text-dark">}</span>
-                  <span class="fw-bold text-danger">]</span>
-                </a>
-              {% endblock %}
-    
-              <button type="button" class="navbar-toggler" data-bs-toggle="collapse"
-                data-bs-target="#navbar" aria-controls="navbar" aria-expanded="false"
-                aria-label="Toggle navigation">
-                <span class="navbar-toggler-icon"></span>
-              </button>
-    
-              <div class="collapse navbar-collapse" id="navbar">
-                <ul class="navbar-nav me-auto">
-                  <li class="nav-item">
-                    <a href="https://www.django-rest-framework.org/" class="nav-link d-flex align-items-center gap-3">
-                      <i class="bi bi-house-fill"></i>
-                      {% translate "Home" %}
-                    </a>
-                  </li>
-                  <li class="nav-item">
-                    <a href="https://www.django-rest-framework.org/tutorial/quickstart/" class="nav-link d-flex align-items-center gap-3">
-                      <i class="bi bi-journal-code"></i>
-                      {% translate "Tutorial" %}
-                    </a>
-                  </li>
-                  <li class="nav-item">
-                    <a href="https://github.com/encode/django-rest-framework/" class="nav-link d-flex align-items-center gap-3">
-                      <i class="bi bi-github"></i>
-                      {% translate "Github" %}
-                    </a>
-                  </li>
-                  <li class="nav-item">
-                    <a href="https://github.com/youzarsiph/rest-framework-redesign/" class="nav-link d-flex align-items-center gap-3">
-                      <i class="bi bi-code-slash"></i>
-                      {% translate "Redesign" %}
-                    </a>
-                  </li>
-                </ul>
-                <ul class="navbar-nav gap-lg-4">
-                  <li class="nav-item dropdown">
-                    <a href="#" class="nav-link d-flex align-items-center justify-content-between gap-3" data-bs-toggle="dropdown">
-                      <span class="d-flex align-item-center gap-3">
-                        <i class="bi bi-person-fill"></i>
-                        {% if user.is_authenticated %}
-                          {{ request.user|capfirst }}
-                        {% else %}
-                          {% translate "Account" %}
-                        {% endif %}
-                      </span>
-                      <i class="bi bi-chevron-down"></i>
-                    </a>
-                    <ul class="dropdown-menu dropdown-menu-end rounded-4 shadow-sm pb-3-sm pb-3">
-                      <li>
-                        <h2 class="dropdown-header">
-                          {% translate 'Account' %}
-                        </h2>
-                      </li>
-                      <li>
-                        {% if user.is_authenticated %}
-                          {% optional_logout request user %}
-                        {% else %}
-                          {% optional_login request %}
-                        {% endif %}
-                      </li>
-                    </ul>
-                  </li>
-                  <li class="nav-item dropdown">
-                    <a href="#" class="nav-link d-flex align-item-center justify-content-between gap-3" data-bs-toggle="dropdown">
-                      <span class="d-flex align-item-center gap-3">
-                        <i class="bi bi-palette"></i>
+<header class="fixed-top p-1 p-md-2">
+  <div class="bg-danger px-2 px-md-3 shadow-sm rounded-4 border border-danger">
+    <div class="bg-dark px-2 px-md-3 rounded-4 shadow-sm">
+      <div class="bg-danger px-2 px-md-3 rounded-4 shadow-sm">
+        <nav
+          class="navbar navbar-expand-lg navbar-dark bg-dark rounded-4 shadow-sm {% block bootstrap_navbar_variant %}{% endblock %}"
+          role="navigation" aria-label="{% translate 'navbar' %}">
+          <div class="container-fluid">
+            {% block branding %}
+            <a class="navbar-brand d-flex align-item-center justify-content-center gap-1 bg-white rounded-4 px-2 shadow-sm"
+              rel="nofollow" href="https://www.django-rest-framework.org/">
+              <span class="fw-bold text-danger">[</span>
+              <span class="fw-bold text-dark">{</span>
+              <strong class="text-dark d-flex align-item-center justify-content-center">
+                <abbr title="Django Rest Framework" data-bs-toggle="tooltip" class="text-decoration-none">
+                  {% translate 'DRF' %}
+                </abbr>
+              </strong>
+              <span class="fw-bold text-dark">}</span>
+              <span class="fw-bold text-danger">]</span>
+            </a>
+            {% endblock %}
+
+            <button type="button" class="navbar-toggler" data-bs-toggle="collapse" data-bs-target="#navbar"
+              aria-controls="navbar" aria-expanded="false" aria-label="Toggle navigation">
+              <span class="navbar-toggler-icon"></span>
+            </button>
+
+            <div class="collapse navbar-collapse" id="navbar">
+              <ul class="navbar-nav me-auto">
+                <li class="nav-item">
+                  <a href="https://www.django-rest-framework.org/" class="nav-link d-flex align-items-center gap-3">
+                    <i class="bi bi-house-fill"></i>
+                    {% translate "Home" %}
+                  </a>
+                </li>
+                <li class="nav-item">
+                  <a href="https://www.django-rest-framework.org/tutorial/quickstart/"
+                    class="nav-link d-flex align-items-center gap-3">
+                    <i class="bi bi-journal-code"></i>
+                    {% translate "Tutorial" %}
+                  </a>
+                </li>
+                <li class="nav-item">
+                  <a href="https://github.com/encode/django-rest-framework/"
+                    class="nav-link d-flex align-items-center gap-3">
+                    <i class="bi bi-github"></i>
+                    {% translate "Github" %}
+                  </a>
+                </li>
+                <li class="nav-item">
+                  <a href="https://github.com/youzarsiph/rest-framework-redesign/"
+                    class="nav-link d-flex align-items-center gap-3">
+                    <i class="bi bi-code-slash"></i>
+                    {% translate "Redesign" %}
+                  </a>
+                </li>
+              </ul>
+              <ul class="navbar-nav gap-lg-4">
+                <li class="nav-item dropdown">
+                  <a href="#" class="nav-link d-flex align-items-center justify-content-between gap-3"
+                    data-bs-toggle="dropdown">
+                    <span class="d-flex align-item-center gap-3">
+                      <i class="bi bi-person-fill"></i>
+                      {% if user.is_authenticated %}
+                      {{ request.user|capfirst }}
+                      {% else %}
+                      {% translate "Account" %}
+                      {% endif %}
+                    </span>
+                    <i class="bi bi-chevron-down"></i>
+                  </a>
+                  <ul class="dropdown-menu dropdown-menu-end rounded-4 shadow-sm pb-3-sm pb-3">
+                    <li>
+                      <h2 class="dropdown-header">
+                        {% translate 'Account' %}
+                      </h2>
+                    </li>
+                    <li>
+                      {% if user.is_authenticated %}
+                      {% optional_logout request user csrf_token %}
+                      {% else %}
+                      {% optional_login request %}
+                      {% endif %}
+                    </li>
+                  </ul>
+                </li>
+                <li class="nav-item dropdown">
+                  <a href="#" class="nav-link d-flex align-item-center justify-content-between gap-3"
+                    data-bs-toggle="dropdown">
+                    <span class="d-flex align-item-center gap-3">
+                      <i class="bi bi-palette"></i>
+                      {% translate 'Theme' %}
+                    </span>
+                    <i class="bi bi-chevron-down"></i>
+                  </a>
+                  <ul class="dropdown-menu dropdown-menu-end rounded-4 shadow-sm pb-3">
+                    <li>
+                      <h2 class="dropdown-header">
                         {% translate 'Theme' %}
-                      </span>
-                      <i class="bi bi-chevron-down"></i>
-                    </a>
-                    <ul class="dropdown-menu dropdown-menu-end rounded-4 shadow-sm pb-3">
-                      <li>
-                        <h2 class="dropdown-header">
-                          {% translate 'Theme' %}
-                        </h2>
-                      </li>
-                      <li>
-                        <a class="dropdown-item px-4 d-flex align-items-center gap-4" href="#" data-bs-theme-value="auto">
-                          <i class="bi bi-circle-half"></i>
-                          {% translate 'Auto' %}
-                        </a>
-                      </li>
-                      <li>
-                        <a class="dropdown-item px-4 d-flex align-items-center gap-4" href="#" data-bs-theme-value="light">
-                          <i class="bi bi-sun"></i>
-                          {% translate 'Light' %}
-                        </a>
-                      </li>
-                      <li>
-                        <a class="dropdown-item px-4 d-flex align-items-center gap-4" href="#" data-bs-theme-value="dark">
-                          <i class="bi bi-moon-stars-fill"></i>
-                          {% translate 'Dark' %}
-                        </a>
-                      </li>
-                    </ul>
-                  </li>
-                </ul>
-              </div>
+                      </h2>
+                    </li>
+                    <li>
+                      <a class="dropdown-item px-4 d-flex align-items-center gap-4" href="#" data-bs-theme-value="auto">
+                        <i class="bi bi-circle-half"></i>
+                        {% translate 'Auto' %}
+                      </a>
+                    </li>
+                    <li>
+                      <a class="dropdown-item px-4 d-flex align-items-center gap-4" href="#"
+                        data-bs-theme-value="light">
+                        <i class="bi bi-sun"></i>
+                        {% translate 'Light' %}
+                      </a>
+                    </li>
+                    <li>
+                      <a class="dropdown-item px-4 d-flex align-items-center gap-4" href="#" data-bs-theme-value="dark">
+                        <i class="bi bi-moon-stars-fill"></i>
+                        {% translate 'Dark' %}
+                      </a>
+                    </li>
+                  </ul>
+                </li>
+              </ul>
             </div>
-          </nav>
-        </div>
+          </div>
+        </nav>
       </div>
     </div>
-  </header>
+  </div>
+</header>
 {% endblock %}
 
 
 {% block breadcrumbs %}
-  <div class="pt-5">
-    <nav aria-label="breadcrumb" class="card card-body shadow-sm rounded-4 mb-4 mt-5 p-4">
-      <ol class="breadcrumb mb-0">
-        {% for breadcrumb_name, breadcrumb_url in breadcrumblist %}
-            {% if forloop.last %}
-              <li class="breadcrumb-item active" aria-current="page">
-                {{ breadcrumb_name }}
-              </li>
-            {% else %}
-              <li class="breadcrumb-item">
-                <a href="{{ breadcrumb_url }}">{{ breadcrumb_name }}</a>
-              </li>
-            {% endif %}
-          {% empty %}
-            {% block breadcrumbs_empty %}&nbsp;{% endblock breadcrumbs_empty %}
-        {% endfor %}
-      </ol>
-    </nav>
-  </div>
+<div class="pt-5">
+  <nav aria-label="breadcrumb" class="card card-body shadow-sm rounded-4 mb-4 mt-5 p-4">
+    <ol class="breadcrumb mb-0">
+      {% for breadcrumb_name, breadcrumb_url in breadcrumblist %}
+      {% if forloop.last %}
+      <li class="breadcrumb-item active" aria-current="page">
+        {{ breadcrumb_name }}
+      </li>
+      {% else %}
+      <li class="breadcrumb-item">
+        <a href="{{ breadcrumb_url }}">{{ breadcrumb_name }}</a>
+      </li>
+      {% endif %}
+      {% empty %}
+      {% block breadcrumbs_empty %}&nbsp;{% endblock breadcrumbs_empty %}
+      {% endfor %}
+    </ol>
+  </nav>
+</div>
 {% endblock %}
 
 {% block content %}
-  <main>
-    <section title="{% translate 'Page Header' %}">
-      <div class="page-header">
-        <h1 class="display-4">{{ name }}</h1>
-      </div>
-      <div class="lead">
-        {% block description %}
-          {{ description }}
-        {% endblock %}
-      </div>
-    </section>
-
-    {% block request_forms %}
-      <section class="d-grid d-md-flex align-items-lg-center justify-content-lg-end gap-4 mb-4" aria-label="{% translate 'Request form' %}">
-        {% if 'GET' in allowed_methods %}
-          <form id="get-form">
-            <fieldset>
-              {% if api_settings.URL_FORMAT_OVERRIDE %}
-                <div class="btn-group w-100" role="group">
-                  <a class="btn btn-primary w-100 shadow-sm" href="{{ request.get_full_path }}" rel="nofollow"
-                    title="Make a GET request on the {{ name }} resource" data-bs-toggle="tooltip">
-                    <span class="d-flex align-items-center justify-content-center gap-4">
-                      <i class="bi bi-arrow-clockwise"></i>
-                      {% translate "GET" %}
-                    </span>
-                  </a>
-                  <button class="btn btn-outline-primary dropdown-toggle shadow-sm" type="button" id="dropdownMenuButton"
-                    data-bs-toggle="dropdown" aria-expanded="false">
-                    <i class="bi bi-chevron-down"></i>
-                  </button>
-                  <div class="dropdown">
-                    <ul class="dropdown-menu dropdown-menu-end rounded-4 shadow-sm pb-3 w-100" aria-labelledby="dropdownMenuButton">
-                      <li>
-                        <h6 class="dropdown-header">
-                          {% translate 'Select a format' %}
-                        </h6>
-                      </li>
-                      {% for format in available_formats %}
-                      <li>
-                        <a class="dropdown-item" data-bs-toggle="tooltip"
-                          href="{% add_query_param request api_settings.URL_FORMAT_OVERRIDE format %}" rel="nofollow"
-                          title="Make a GET request on the {{ name }} resource with the format set to `{{ format|upper }}`">
-                          {{ format|upper }}
-                        </a>
-                      </li>
-                      {% endfor %}
-                    </ul>
-                  </div>
-                </div>
-              {% else %}
-                <a class="btn btn-primary shadow-sm" href="{{ request.get_full_path }}" rel="nofollow"
-                  title="Make a GET request on the {{ name }} resource" data-bs-toggle="tooltip">
-                  <span class="d-flex align-items-center justify-content-center gap-4">
-                    <i class="bi bi-arrow-clockwise"></i>
-                    {% translate "GET" %}
-                  </span>
-                </a>
-              {% endif %}
-            </fieldset>
-          </form>
-        {% endif %}
-
-        {% if options_form %}
-          <form class="button-form" action="{{ request.get_full_path }}" data-method="OPTIONS">
-            <button type="submit" class="btn btn-info w-100 shadow-sm" title="Make an OPTIONS request on the {{ name }} resource" data-bs-toggle="tooltip">
-              <span class="d-flex align-items-center justify-content-center gap-4">
-                <i class="bi bi-info-square"></i>
-                {% translate "OPTIONS" %}
-              </span>
-            </button>
-          </form>
-        {% endif %}
-
-        {% if delete_form %}
-          <div>
-            <button type="button" class="btn btn-danger w-100 shadow-sm" data-bs-toggle="modal" data-bs-target="#deleteModal"
-              title="Make a DELETE request on the {{ name }} resource">
-              <span class="d-flex align-items-center justify-content-center gap-4">
-                <i class="bi bi-trash"></i>
-                {% translate "DELETE" %}
-              </span>
-            </button>
-          </div>
-
-          <div class="modal fade" id="deleteModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
-            <div class="modal-dialog modal-dialog-centered">
-              <div class="modal-content p-md-3 p-lg-4 rounded-4 shadow">
-                <div class="modal-header border-bottom-0">
-                  <h3 class="modal-title" id="exampleModalLabel">
-                    {% translate 'Delete' %} {{ name }}
-                  </h3>
-                  <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
-                </div>
-                <div class="modal-body">
-                  <p class="mb-4">
-                    {% translate "Are you sure you want to delete this" %} {{ name }}?
-                  </p>
-                  <div class="d-grid d-lg-flex align-items-lg-center gap-4">
-                    <form class="button-form w-100" action="{{ request.get_full_path }}" data-method="DELETE">
-                      <button class="btn btn-danger w-100 shadow-sm">
-                        <span class="d-flex align-item-center justify-content-center gap-4">
-                          <i class="bi bi-trash"></i>
-                          {% translate "Delete" %}
-                        </span>
-                      </button>
-                    </form>
-                    <button type="button" class="btn btn-outline-secondary w-100 shadow-sm" data-bs-dismiss="modal">
-                      <span class="d-flex align-item-center justify-content-center gap-4">
-                        <i class="bi bi-x-lg"></i>
-                        {% translate "Cancel" %}
-                      </span>
-                    </button>
-                  </div>
-                </div>
-              </div>
-            </div>
-          </div>
-        {% endif %}
+<main>
+  <section title="{% translate 'Page Header' %}">
+    <div class="page-header">
+      <h1 class="display-4">{{ name }}</h1>
+    </div>
+    <div class="lead">
+      {% block description %}
+      {{ description }}
+      {% endblock %}
+    </div>
+  </section>
 
-        {% if extra_actions %}
+  {% block request_forms %}
+  <section class="d-grid d-md-flex align-items-lg-center justify-content-lg-end gap-4 mb-4"
+    aria-label="{% translate 'Request form' %}">
+    {% if 'GET' in allowed_methods %}
+    <form id="get-form">
+      <fieldset>
+        {% if api_settings.URL_FORMAT_OVERRIDE %}
+        <div class="btn-group w-100" role="group">
+          <a class="btn btn-primary w-100 shadow-sm" href="{{ request.get_full_path }}" rel="nofollow"
+            title="Make a GET request on the {{ name }} resource" data-bs-toggle="tooltip">
+            <span class="d-flex align-items-center justify-content-center gap-4">
+              <i class="bi bi-arrow-clockwise"></i>
+              {% translate "GET" %}
+            </span>
+          </a>
+          <button class="btn btn-outline-primary dropdown-toggle shadow-sm" type="button" id="dropdownMenuButton"
+            data-bs-toggle="dropdown" aria-expanded="false">
+            <i class="bi bi-chevron-down"></i>
+          </button>
           <div class="dropdown">
-            <button class="btn btn-warning w-100 shadow-sm" id="extra-actions-menu" data-bs-toggle="dropdown" aria-haspopup="true"
-              aria-expanded="true">
-              <span class="d-flex align-items-center justify-content-center gap-4">
-                {% translate "Extra Actions" %}
-                <i class="bi bi-chevron-down"></i>
-              </span>
-            </button>
-            <ul class="dropdown-menu rounded-4 shadow-sm pb-3 w-100" aria-labelledby="extra-actions-menu">
+            <ul class="dropdown-menu dropdown-menu-end rounded-4 shadow-sm pb-3 w-100"
+              aria-labelledby="dropdownMenuButton">
               <li>
-                <h3 class="dropdown-header">
-                  {% translate 'Select an action' %}
-                </h3>
+                <h6 class="dropdown-header">
+                  {% translate 'Select a format' %}
+                </h6>
+              </li>
+              {% for format in available_formats %}
+              <li>
+                <a class="dropdown-item" data-bs-toggle="tooltip"
+                  href="{% add_query_param request api_settings.URL_FORMAT_OVERRIDE format %}" rel="nofollow"
+                  title="Make a GET request on the {{ name }} resource with the format set to `{{ format|upper }}`">
+                  {{ format|upper }}
+                </a>
               </li>
-              {% for action_name, url in extra_actions|items %}
-                <li>
-                  <a class="dropdown-item" href="{{ url }}">
-                    {{ action_name }}
-                  </a>
-                </li>
               {% endfor %}
             </ul>
           </div>
+        </div>
+        {% else %}
+        <a class="btn btn-primary shadow-sm" href="{{ request.get_full_path }}" rel="nofollow"
+          title="Make a GET request on the {{ name }} resource" data-bs-toggle="tooltip">
+          <span class="d-flex align-items-center justify-content-center gap-4">
+            <i class="bi bi-arrow-clockwise"></i>
+            {% translate "GET" %}
+          </span>
+        </a>
         {% endif %}
+      </fieldset>
+    </form>
+    {% endif %}
 
-        {% if filter_form %}
-          <button data-bs-toggle="modal" data-bs-target="#filtersModal" class="btn btn-success shadow-sm">
-            <span class="d-flex align-items-center justify-content-center gap-4">
-              <i class="bi bi-filter"></i>
-              {% translate "Filters" %}
-            </span>
-          </button>
-        {% endif %}
-      </section>
-    {% endblock %}
-
-    {% if paginator %}
-      <section title="{% translate 'Pagination' %}" class="d-flex align-item-center justify-content-end mb-4">
-        {% get_pagination_html paginator %}
-      </section>
+    {% if options_form %}
+    <form class="button-form" action="{{ request.get_full_path }}" data-method="OPTIONS">
+      <button type="submit" class="btn btn-info w-100 shadow-sm"
+        title="Make an OPTIONS request on the {{ name }} resource" data-bs-toggle="tooltip">
+        <span class="d-flex align-items-center justify-content-center gap-4">
+          <i class="bi bi-info-square"></i>
+          {% translate "OPTIONS" %}
+        </span>
+      </button>
+    </form>
     {% endif %}
 
-    <div class="row g-4 mb-4" aria-label="{% translate 'Main content' %}">
-      <section class="col-12 col-lg-8 order-last order-lg-first" role="main" aria-label="{% translate 'Main content' %}">
-        <div class="card card-body rounded-4 p-4 shadow-sm">
-          <div class="request-info" aria-label="{% translate 'Request info' %}">
-            <pre class="prettyprint"><code class="language-http" style="padding: 0; background-color: transparent;">{{ request.method }} {{ request.get_full_path }}</code></pre>
+    {% if delete_form %}
+    <div>
+      <button type="button" class="btn btn-danger w-100 shadow-sm" data-bs-toggle="modal" data-bs-target="#deleteModal"
+        title="Make a DELETE request on the {{ name }} resource">
+        <span class="d-flex align-items-center justify-content-center gap-4">
+          <i class="bi bi-trash"></i>
+          {% translate "DELETE" %}
+        </span>
+      </button>
+    </div>
+
+    <div class="modal fade" id="deleteModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
+      <div class="modal-dialog modal-dialog-centered">
+        <div class="modal-content p-md-3 p-lg-4 rounded-4 shadow">
+          <div class="modal-header border-bottom-0">
+            <h3 class="modal-title" id="exampleModalLabel">
+              {% translate 'Delete' %} {{ name }}
+            </h3>
+            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
           </div>
+          <div class="modal-body">
+            <p class="mb-4">
+              {% translate "Are you sure you want to delete this" %} {{ name }}?
+            </p>
+            <div class="d-grid d-lg-flex align-items-lg-center gap-4">
+              <form class="button-form w-100" action="{{ request.get_full_path }}" data-method="DELETE">
+                <button class="btn btn-danger w-100 shadow-sm">
+                  <span class="d-flex align-item-center justify-content-center gap-4">
+                    <i class="bi bi-trash"></i>
+                    {% translate "Delete" %}
+                  </span>
+                </button>
+              </form>
+              <button type="button" class="btn btn-outline-secondary w-100 shadow-sm" data-bs-dismiss="modal">
+                <span class="d-flex align-item-center justify-content-center gap-4">
+                  <i class="bi bi-x-lg"></i>
+                  {% translate "Cancel" %}
+                </span>
+              </button>
+            </div>
+          </div>
+        </div>
+      </div>
+    </div>
+    {% endif %}
+
+    {% if extra_actions %}
+    <div class="dropdown">
+      <button class="btn btn-warning w-100 shadow-sm" id="extra-actions-menu" data-bs-toggle="dropdown"
+        aria-haspopup="true" aria-expanded="true">
+        <span class="d-flex align-items-center justify-content-center gap-4">
+          {% translate "Extra Actions" %}
+          <i class="bi bi-chevron-down"></i>
+        </span>
+      </button>
+      <ul class="dropdown-menu rounded-4 shadow-sm pb-3 w-100" aria-labelledby="extra-actions-menu">
+        <li>
+          <h3 class="dropdown-header">
+            {% translate 'Select an action' %}
+          </h3>
+        </li>
+        {% for action_name, url in extra_actions|items %}
+        <li>
+          <a class="dropdown-item" href="{{ url }}">
+            {{ action_name }}
+          </a>
+        </li>
+        {% endfor %}
+      </ul>
+    </div>
+    {% endif %}
+
+    {% if filter_form %}
+    <button data-bs-toggle="modal" data-bs-target="#filtersModal" class="btn btn-success shadow-sm">
+      <span class="d-flex align-items-center justify-content-center gap-4">
+        <i class="bi bi-filter"></i>
+        {% translate "Filters" %}
+      </span>
+    </button>
+    {% endif %}
+  </section>
+  {% endblock %}
+
+  {% if paginator %}
+  <section title="{% translate 'Pagination' %}" class="d-flex align-item-center justify-content-end mb-4">
+    {% get_pagination_html paginator %}
+  </section>
+  {% endif %}
+
+  <div class="row g-4 mb-4" aria-label="{% translate 'Main content' %}">
+    <section class="col-12 col-lg-8 order-last order-lg-first" role="main" aria-label="{% translate 'Main content' %}">
+      <div class="card card-body rounded-4 p-4 shadow-sm">
+        <div class="request-info" aria-label="{% translate 'Request info' %}">
+          <pre
+            class="prettyprint"><code class="language-http" style="padding: 0; background-color: transparent;">{{ request.method }} {{ request.get_full_path }}</code></pre>
+        </div>
 
-          <div class="response-info" aria-label="{% translate 'response info' %}">
-<pre class="prettyprint d-grid">
+        <div class="response-info" aria-label="{% translate 'response info' %}">
+          <pre class="prettyprint d-grid">
 <code class="language-http" style="padding: 0; background-color: transparent;">HTTP {{ response.status_code }} {{ response.status_text }}
 {% for key, val in response_headers|items %}{{ key }}: {{ val|break_long_headers|urlize }}
 {% endfor %}</code>
 <code class="language-json" style="padding: 0; background-color: transparent;">{{ content|urlize }}</code>
 </pre>
-          </div>
         </div>
-      </section>
+      </div>
+    </section>
 
-      <section class="col-12 col-lg-4">
-        {% if display_edit_forms %}
-          {% if post_form or raw_data_post_form %}
-            <div {% if post_form %}class="card card-body rounded-4 p-4 shadow-sm" {% endif %}>
-              {% if post_form %}
-                <ul class="nav nav-pills nav-fill gap-4 p-1 rounded-5 border mb-4 shadow-sm" role="tablist">
-                  <li class="nav-item" role="presentation">
-                    <button class="nav-link active rounded-5" id="form-tab" data-bs-toggle="tab" data-bs-target="#form"
-                      type="button" role="tab" aria-controls="form" aria-selected="true">
-                      <span class="d-flex align-items-center justify-content-center gap-4">
-                        <i class="bi bi-filetype-html"></i>
-                        {% translate 'HTML form' %}
-                      </span>
-                    </button>
-                  </li>
-                  <li class="nav-item" role="presentation">
-                    <button class="nav-link rounded-5" id="raw-tab" data-bs-toggle="tab" data-bs-target="#raw"
-                      type="button" role="tab" aria-controls="raw" aria-selected="false">
-                      <span class="d-flex align-items-center justify-content-center gap-4">
-                        <i class="bi bi-filetype-json"></i>
-                        {% translate 'Raw data' %}
-                      </span>
-                    </button>
-                  </li>
-                </ul>
-              {% endif %}
-
-              <div class="tab-content">
-                {% if post_form %}
-                  <div class="tab-pane active" id="form" role="tabpanel" aria-labelledby="form-tab" tabindex="0">
-                    {% with form=post_form %}
-                      <form action="{{ request.get_full_path }}" method="POST" enctype="multipart/form-data" class="form-horizontal">
-                        <fieldset>
-                          {% csrf_token %}
-                          {{ post_form }}
-                          <div class="form-actions">
-                            <button class="btn btn-primary w-100 shadow-sm" title="Make a POST request on the {{ name }} resource" data-bs-toggle="tooltip">
-                              <span class="d-flex align-items-center justify-content-center gap-4">
-                                <i class="bi bi-send-fill"></i>
-                                {% translate "POST" %}
-                              </span>
-                            </button>
-                          </div>
-                        </fieldset>
-                      </form>
-                    {% endwith %}
-                  </div>
-                {% endif %}
-
-                <div class="tab-pane" id="raw" role="tabpanel" aria-labelledby="raw-tab" tabindex="0">
-                  {% with form=raw_data_post_form %}
-                    <form action="{{ request.get_full_path }}" method="POST" class="form-horizontal">
-                      <fieldset>
-                        {% include "rest_framework/raw_data_form.html" %}
-                        <div class="form-actions">
-                          <button class="btn btn-primary w-100 shadow-sm" title="Make a POST request on the {{ name }} resource" data-bs-toggle="tooltip">
-                            <span class="d-flex align-items-center justify-content-center gap-4">
-                              <i class="bi bi-send-fill"></i>
-                              {% translate "POST" %}
-                            </span>
-                          </button>
-                        </div>
-                      </fieldset>
-                    </form>
-                  {% endwith %}
-                </div>
-              </div>
+    <section class="col-12 col-lg-4">
+      {% if display_edit_forms %}
+      {% if post_form or raw_data_post_form %}
+      <div {% if post_form %}class="card card-body rounded-4 p-4 shadow-sm" {% endif %}>
+        {% if post_form %}
+        <ul class="nav nav-pills nav-fill gap-4 p-1 rounded-5 border mb-4 shadow-sm" role="tablist">
+          <li class="nav-item" role="presentation">
+            <button class="nav-link active rounded-5" id="form-tab" data-bs-toggle="tab" data-bs-target="#form"
+              type="button" role="tab" aria-controls="form" aria-selected="true">
+              <span class="d-flex align-items-center justify-content-center gap-4">
+                <i class="bi bi-filetype-html"></i>
+                {% translate 'HTML form' %}
+              </span>
+            </button>
+          </li>
+          <li class="nav-item" role="presentation">
+            <button class="nav-link rounded-5" id="raw-tab" data-bs-toggle="tab" data-bs-target="#raw" type="button"
+              role="tab" aria-controls="raw" aria-selected="false">
+              <span class="d-flex align-items-center justify-content-center gap-4">
+                <i class="bi bi-filetype-json"></i>
+                {% translate 'Raw data' %}
+              </span>
+            </button>
+          </li>
+        </ul>
+        {% endif %}
 
-              <p class="small mt-4 mb-0">
-                <span class="text-danger">*</span> Indicates Required
-              </p>
-            </div>
+        <div class="tab-content">
+          {% if post_form %}
+          <div class="tab-pane active" id="form" role="tabpanel" aria-labelledby="form-tab" tabindex="0">
+            {% with form=post_form %}
+            <form action="{{ request.get_full_path }}" method="POST" enctype="multipart/form-data"
+              class="form-horizontal">
+              <fieldset>
+                {% csrf_token %}
+                {{ post_form }}
+                <div class="form-actions">
+                  <button class="btn btn-primary w-100 shadow-sm" title="Make a POST request on the {{ name }} resource"
+                    data-bs-toggle="tooltip">
+                    <span class="d-flex align-items-center justify-content-center gap-4">
+                      <i class="bi bi-send-fill"></i>
+                      {% translate "POST" %}
+                    </span>
+                  </button>
+                </div>
+              </fieldset>
+            </form>
+            {% endwith %}
+          </div>
           {% endif %}
 
-          {% if put_form or raw_data_put_form or raw_data_patch_form %}
-            <div {% if put_form %}class="card card-body rounded-4 p-4 shadow-sm"{% endif %}>
-              {% if put_form %}
-                <ul class="nav nav-pills nav-fill gap-4 p-1 rounded-5 border mb-4 shadow-sm" role="tablist">
-                  <li class="nav-item" role="presentation">
-                    <button class="nav-link active rounded-5" id="form-tab" data-bs-toggle="tab" data-bs-target="#put-object-form"
-                      type="button" role="tab" aria-controls="form" aria-selected="true">
-                      <span class="d-flex align-items-center justify-content-center gap-4">
-                        <i class="bi bi-filetype-html"></i>
-                        {% translate 'HTML form' %}
-                      </span>
-                    </button>
-                  </li>
-                  <li class="nav-item" role="presentation">
-                    <button class="nav-link rounded-5" id="raw-tab" data-bs-toggle="tab" data-bs-target="#put-generic-content-form"
-                      type="button" role="tab" aria-controls="raw" aria-selected="false">
-                      <span class="d-flex align-items-center justify-content-center gap-4">
-                        <i class="bi bi-filetype-json"></i>
-                        {% translate 'Raw data' %}
-                      </span>
-                    </button>
-                  </li>
-                </ul>
-              {% endif %}
-
-              <div class="tab-content">
-                {% if put_form %}
-                  <div class="tab-pane active" id="put-object-form">
-                    <form action="{{ request.get_full_path }}" data-method="PUT" enctype="multipart/form-data" class="form-horizontal">
-                      <fieldset>
-                        {{ put_form }}
-                        <div class="form-actions">
-                          <button class="btn btn-primary w-100 shadow-sm" title="Make a PUT request on the {{ name }} resource" data-bs-toggle="tooltip">
-                            <span class="d-flex align-items-center justify-content-center gap-4">
-                              <i class="bi bi-send-fill"></i>
-                              {% translate "PUT" %}
-                            </span>
-                          </button>
-                        </div>
-                      </fieldset>
-                    </form>
-                  </div>
-                {% endif %}
-
-                <div {% if put_form %}class="tab-pane"{% endif %} id="put-generic-content-form">
-                  {% with form=raw_data_put_or_patch_form %}
-                    <form action="{{ request.get_full_path }}" data-method="PUT" class="form-horizontal">
-                      <fieldset>
-                        {% include "rest_framework/raw_data_form.html" %}
-                        <div class="form-actions">
-                          {% if raw_data_put_form %}
-                            <button class="btn btn-primary w-100 shadow-sm"
-                              title="Make a PUT request on the {{ name }} resource" data-bs-toggle="tooltip">
-                              <span class="d-flex align-items-center justify-content-center gap-4">
-                                <i class="bi bi-send-fill"></i>
-                                {% translate "PUT" %}
-                              </span>
-                            </button>
-                          {% endif %}
-                          {% if raw_data_patch_form %}
-                            <button data-method="PATCH" class="btn btn-outline-primary w-100 mt-4 shadow-sm"
-                              title="Make a PATCH request on the {{ name }} resource" data-bs-toggle="tooltip">
-                              <span class="d-flex align-items-center justify-content-center gap-4">
-                                <i class="bi bi-send-fill"></i>
-                                {% translate "PATCH" %}
-                              </span>
-                            </button>
-                          {% endif %}
-                        </div>
-                      </fieldset>
-                    </form>
-                  {% endwith %}
+          <div class="tab-pane" id="raw" role="tabpanel" aria-labelledby="raw-tab" tabindex="0">
+            {% with form=raw_data_post_form %}
+            <form action="{{ request.get_full_path }}" method="POST" class="form-horizontal">
+              <fieldset>
+                {% include "rest_framework/raw_data_form.html" %}
+                <div class="form-actions">
+                  <button class="btn btn-primary w-100 shadow-sm" title="Make a POST request on the {{ name }} resource"
+                    data-bs-toggle="tooltip">
+                    <span class="d-flex align-items-center justify-content-center gap-4">
+                      <i class="bi bi-send-fill"></i>
+                      {% translate "POST" %}
+                    </span>
+                  </button>
                 </div>
-              </div>
+              </fieldset>
+            </form>
+            {% endwith %}
+          </div>
+        </div>
 
-              <p class="small mt-4 mb-0">
-                <span class="text-danger">*</span> Indicates Required
-              </p>
-            </div>
-          {% endif %}
+        <p class="small mt-4 mb-0">
+          <span class="text-danger">*</span> Indicates Required
+        </p>
+      </div>
+      {% endif %}
+
+      {% if put_form or raw_data_put_form or raw_data_patch_form %}
+      <div {% if put_form %}class="card card-body rounded-4 p-4 shadow-sm" {% endif %}>
+        {% if put_form %}
+        <ul class="nav nav-pills nav-fill gap-4 p-1 rounded-5 border mb-4 shadow-sm" role="tablist">
+          <li class="nav-item" role="presentation">
+            <button class="nav-link active rounded-5" id="form-tab" data-bs-toggle="tab"
+              data-bs-target="#put-object-form" type="button" role="tab" aria-controls="form" aria-selected="true">
+              <span class="d-flex align-items-center justify-content-center gap-4">
+                <i class="bi bi-filetype-html"></i>
+                {% translate 'HTML form' %}
+              </span>
+            </button>
+          </li>
+          <li class="nav-item" role="presentation">
+            <button class="nav-link rounded-5" id="raw-tab" data-bs-toggle="tab"
+              data-bs-target="#put-generic-content-form" type="button" role="tab" aria-controls="raw"
+              aria-selected="false">
+              <span class="d-flex align-items-center justify-content-center gap-4">
+                <i class="bi bi-filetype-json"></i>
+                {% translate 'Raw data' %}
+              </span>
+            </button>
+          </li>
+        </ul>
         {% endif %}
-      </section>
-    </div>
-  </main>
+
+        <div class="tab-content">
+          {% if put_form %}
+          <div class="tab-pane active" id="put-object-form">
+            <form action="{{ request.get_full_path }}" data-method="PUT" enctype="multipart/form-data"
+              class="form-horizontal">
+              <fieldset>
+                {{ put_form }}
+                <div class="form-actions">
+                  <button class="btn btn-primary w-100 shadow-sm" title="Make a PUT request on the {{ name }} resource"
+                    data-bs-toggle="tooltip">
+                    <span class="d-flex align-items-center justify-content-center gap-4">
+                      <i class="bi bi-send-fill"></i>
+                      {% translate "PUT" %}
+                    </span>
+                  </button>
+                </div>
+              </fieldset>
+            </form>
+          </div>
+          {% endif %}
+
+          <div {% if put_form %}class="tab-pane" {% endif %} id="put-generic-content-form">
+            {% with form=raw_data_put_or_patch_form %}
+            <form action="{{ request.get_full_path }}" data-method="PUT" class="form-horizontal">
+              <fieldset>
+                {% include "rest_framework/raw_data_form.html" %}
+                <div class="form-actions">
+                  {% if raw_data_put_form %}
+                  <button class="btn btn-primary w-100 shadow-sm" title="Make a PUT request on the {{ name }} resource"
+                    data-bs-toggle="tooltip">
+                    <span class="d-flex align-items-center justify-content-center gap-4">
+                      <i class="bi bi-send-fill"></i>
+                      {% translate "PUT" %}
+                    </span>
+                  </button>
+                  {% endif %}
+                  {% if raw_data_patch_form %}
+                  <button data-method="PATCH" class="btn btn-outline-primary w-100 mt-4 shadow-sm"
+                    title="Make a PATCH request on the {{ name }} resource" data-bs-toggle="tooltip">
+                    <span class="d-flex align-items-center justify-content-center gap-4">
+                      <i class="bi bi-send-fill"></i>
+                      {% translate "PATCH" %}
+                    </span>
+                  </button>
+                  {% endif %}
+                </div>
+              </fieldset>
+            </form>
+            {% endwith %}
+          </div>
+        </div>
+
+        <p class="small mt-4 mb-0">
+          <span class="text-danger">*</span> Indicates Required
+        </p>
+      </div>
+      {% endif %}
+      {% endif %}
+    </section>
+  </div>
+</main>
 {% endblock %}
 
 {% if filter_form %}
-  {{ filter_form }}
+{{ filter_form }}
 {% endif %}
 
 {% block script %}
-  {{ block.super }}
-  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
-    integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
-  <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/highlight.min.js"></script>
-  <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/languages/http.min.js"></script>
-  <script>hljs.highlightAll()</script>
-  <script>
-    // Make all links in response section clickable
-    setTimeout(() =>
-      document.querySelectorAll('.response-info .language-json .hljs-string .str').forEach(e => {
-        if (e.innerHTML.startsWith('"http')) {
-          e.innerHTML = `<a href="${e.innerHTML.slice(1, e.innerHTML.length - 1)}">${e.innerHTML}</a>`
-        }
-      }), 100);
-  </script>
-  <script>
-    const tooltipTriggerList = document.querySelectorAll('[data-bs-toggle="tooltip"]')
-    const tooltipList = [...tooltipTriggerList].map(tooltipTriggerEl => new bootstrap.Tooltip(tooltipTriggerEl))
-  </script>
+{{ block.super }}
+<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
+  integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
+<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/highlight.min.js"></script>
+<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/languages/http.min.js"></script>
+<script>hljs.highlightAll()</script>
+<script>
+  // Make all links in response section clickable
+  setTimeout(() =>
+    document.querySelectorAll('.response-info .language-json .hljs-string .str').forEach(e => {
+      if (e.innerHTML.startsWith('"http')) {
+        e.innerHTML = `<a href="${e.innerHTML.slice(1, e.innerHTML.length - 1)}">${e.innerHTML}</a>`
+      }
+    }), 100);
+</script>
+<script>
+  const tooltipTriggerList = document.querySelectorAll('[data-bs-toggle="tooltip"]')
+  const tooltipList = [...tooltipTriggerList].map(tooltipTriggerEl => new bootstrap.Tooltip(tooltipTriggerEl))
+</script>
 {% endblock %}
```

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/filters/base.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/filters/ordering.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/filters/search.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/checkbox.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/input.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/radio.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/select.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/select_multiple.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/horizontal/textarea.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/checkbox.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/input.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/radio.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/select.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/select_multiple.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/inline/textarea.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/inline/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/login.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/login.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/pagination/numbers.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/pagination/previous_and_next.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/checkbox.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/input.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/radio.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/select.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/select_multiple.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templates/rest_framework/vertical/textarea.html` & `drf_redesign-0.3.9/drf_redesign/templates/rest_framework/vertical/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.8/drf_redesign/templatetags/rest_framework_redesign.py` & `drf_redesign-0.3.9/drf_redesign/templatetags/rest_framework_redesign.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ Customizes template tags from DRF """
 
-
 from django.template import Library
 from django.urls import NoReverseMatch, reverse
 from django.utils.html import escape, format_html
 from django.utils.safestring import mark_safe
 
 
 # Create your tags here.
@@ -13,54 +12,63 @@
 
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

### Comparing `drf_redesign-0.3.8/pyproject.toml` & `drf_redesign-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-redesign"
-version = "0.3.8"
+version = "0.3.9"
 description = "Redesign of the browse-able api of Django REST Framework with Bootstrap 5"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "drf_redesign"}]
 homepage = "https://github.com/youzarsiph/drf-redesign/"
 repository = "https://github.com/youzarsiph/drf-redesign/"
```

### Comparing `drf_redesign-0.3.8/PKG-INFO` & `drf_redesign-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-redesign
-Version: 0.3.8
+Version: 0.3.9
 Summary: Redesign of the browse-able api of Django REST Framework with Bootstrap 5
 Home-page: https://github.com/youzarsiph/drf-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

