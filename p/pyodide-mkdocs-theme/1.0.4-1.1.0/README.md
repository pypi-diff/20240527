# Comparing `tmp/pyodide_mkdocs_theme-1.0.4.tar.gz` & `tmp/pyodide_mkdocs_theme-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-1.0.4.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-1.1.0.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-1.0.4.tar` & `pyodide_mkdocs_theme-1.1.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-1.0.4/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-1.0.4/README.md
--rw-r--r--   0        0        0     1347 2024-05-16 22:36:03.803644 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     2591 2024-05-15 21:11:56.281098 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-05-16 22:36:03.835644 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0     1322 2024-05-15 21:11:56.281098 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
--rw-r--r--   0        0        0     1063 2024-05-15 21:11:56.293098 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-05-12 18:52:50.335028 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     5919 2024-05-15 21:11:56.321099 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     2992 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py
--rw-r--r--   0        0        0        0 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6043 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0    11922 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/ide.py
--rw-r--r--   0        0        0    16534 2024-05-15 21:11:56.337099 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py
--rw-r--r--   0        0        0    21130 2024-05-15 21:11:56.369100 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py
--rw-r--r--   0        0        0     4850 2024-05-15 21:11:56.377100 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py
--rw-r--r--   0        0        0     3470 2024-05-15 21:11:56.377100 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py
--rw-r--r--   0        0        0     2435 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11591 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0    13668 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/messages.py
--rw-r--r--   0        0        0     7262 2024-05-16 18:56:03.280303 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0    16089 2024-05-16 22:32:28.181317 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4776 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0        0 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0    15211 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11391 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0     9693 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
--rw-r--r--   0        0        0     1603 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0     6652 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
--rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     9042 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0     1163 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     9640 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0     4229 2024-05-16 22:36:03.803644 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/scripts/custom_lang.py
--rw-r--r--   0        0        0     5487 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/scripts/mkdocs.yml
--rw-r--r--   0        0        0     3593 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/scripts/model.py
--rw-r--r--   0        0        0      823 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/README.md
--rw-r--r--   0        0        0        0 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     2857 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg
--rw-r--r--   0        0        0     1645 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png
--rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/hooks/libsAfter.html
--rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/hooks/libsBefore.html
--rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/hooks/scriptsAfter.html
--rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/hooks/scriptsBefore.html
--rw-r--r--   0        0        0     6093 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
--rw-r--r--   0        0        0    10642 2024-05-16 22:29:59.532956 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
--rw-r--r--   0        0        0     1770 2024-05-16 22:36:00.103535 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
--rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0     4361 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0    10814 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js
--rw-r--r--   0        0        0    14528 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js
--rw-r--r--   0        0        0     1183 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js
--rw-r--r--   0        0        0     8220 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js
--rw-r--r--   0        0        0    18519 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js
--rw-r--r--   0        0        0    12716 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js
--rw-r--r--   0        0        0     7231 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js
--rw-r--r--   0        0        0    11253 2024-05-15 21:11:56.481103 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js
--rw-r--r--   0        0        0     4455 2024-05-15 21:11:56.489103 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0     5341 2024-05-15 21:11:56.505103 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     2635 2024-05-15 21:11:56.505103 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     3831 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css
--rw-r--r--   0        0        0     1078 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css
--rw-r--r--   0        0        0     1947 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css
--rw-r--r--   0        0        0     3764 2024-05-16 18:56:03.284304 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css
--rw-r--r--   0        0        0     3904 2024-05-15 21:11:56.525104 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css
--rw-r--r--   0        0        0     1918 2024-05-15 21:11:56.525104 pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css
--rw-r--r--   0        0        0     1766 2024-05-16 22:36:00.147536 pyodide_mkdocs_theme-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-1.1.0/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-1.1.0/README.md
+-rw-r--r--   0        0        0     1347 2024-05-27 09:57:21.636930 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     2591 2024-05-15 21:11:56.281098 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-05-27 09:57:21.672931 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0     1322 2024-05-15 21:11:56.281098 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
+-rw-r--r--   0        0        0     1063 2024-05-15 21:11:56.293098 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-05-12 18:52:50.335028 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     5919 2024-05-15 21:11:56.321099 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     2996 2024-05-27 09:42:56.555664 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:11:56.329099 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6043 2024-04-27 20:26:40.306387 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0    17204 2024-05-27 09:42:56.575665 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py
+-rw-r--r--   0        0        0    13613 2024-05-27 09:42:56.591666 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_ide.py
+-rw-r--r--   0        0        0    19387 2024-05-27 09:42:56.591666 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py
+-rw-r--r--   0        0        0     4972 2024-05-27 09:42:56.607666 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py
+-rw-r--r--   0        0        0     3460 2024-05-27 09:42:56.607666 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py
+-rw-r--r--   0        0        0     2435 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11591 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0    13668 2024-05-15 21:11:56.389101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/messages.py
+-rw-r--r--   0        0        0     7422 2024-05-27 09:42:56.607666 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0    16171 2024-05-27 09:42:56.623666 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4776 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0    15211 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11391 2024-05-25 09:20:37.108858 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0     9693 2024-05-15 21:11:56.421101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py
+-rw-r--r--   0        0        0     1603 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0     6652 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py
+-rw-r--r--   0        0        0     2877 2024-04-24 20:11:56.666105 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     9042 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0     1163 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     9846 2024-05-27 09:42:56.639667 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0     3539 2024-05-27 09:57:21.636930 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/scripts/custom_lang.py
+-rw-r--r--   0        0        0     4776 2024-05-27 09:42:56.655667 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/scripts/mkdocs.yml
+-rw-r--r--   0        0        0     2902 2024-05-27 09:42:56.671668 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/scripts/model.py
+-rw-r--r--   0        0        0      823 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     2857 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg
+-rw-r--r--   0        0        0     1645 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-05-15 21:11:56.425101 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-05-15 21:11:56.429102 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png
+-rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/hooks/libsAfter.html
+-rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/hooks/libsBefore.html
+-rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/hooks/scriptsAfter.html
+-rw-r--r--   0        0        0        0 2024-05-16 21:25:14.310769 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/hooks/scriptsBefore.html
+-rw-r--r--   0        0        0     6123 2024-05-27 09:42:56.675668 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0    12332 2024-05-27 09:42:56.699669 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1770 2024-05-27 09:57:18.652840 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4361 2024-04-29 14:09:33.373857 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0    12029 2024-05-27 09:42:56.699669 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js
+-rw-r--r--   0        0        0    15301 2024-05-27 09:42:56.699669 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js
+-rw-r--r--   0        0        0     1157 2024-05-27 09:42:56.711669 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js
+-rw-r--r--   0        0        0     9056 2024-05-27 09:42:56.711669 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js
+-rw-r--r--   0        0        0    17296 2024-05-27 09:42:56.731670 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js
+-rw-r--r--   0        0        0    12716 2024-05-15 21:11:56.437102 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js
+-rw-r--r--   0        0        0     7237 2024-05-27 09:42:56.731670 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js
+-rw-r--r--   0        0        0    11465 2024-05-27 09:42:56.759670 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0     4455 2024-05-15 21:11:56.489103 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0     5341 2024-05-15 21:11:56.505103 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     2635 2024-05-15 21:11:56.505103 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     3831 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css
+-rw-r--r--   0        0        0     1078 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css
+-rw-r--r--   0        0        0     1947 2024-05-15 21:11:56.517104 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css
+-rw-r--r--   0        0        0     3764 2024-05-16 18:56:03.284304 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css
+-rw-r--r--   0        0        0     3904 2024-05-15 21:11:56.525104 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css
+-rw-r--r--   0        0        0     1918 2024-05-15 21:11:56.525104 pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css
+-rw-r--r--   0        0        0     1766 2024-05-27 09:57:18.684841 pyodide_mkdocs_theme-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-1.1.0/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-1.0.4/LICENSE` & `pyodide_mkdocs_theme-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/README.md` & `pyodide_mkdocs_theme-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/deprecation.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 from ..tools_and_constants import ScriptSection
 from ..parsing import build_code_fence
 from ..plugin.maestro_IDE import MaestroIDE
 from .ide_files_data import IdeFilesExtractor
 from .ide_manager import IdeManager
-from .ide import Ide
+from .ide_ide import Ide
 from .ide_terminal import Terminal
 from .ide_pybtn import PyBtn
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/ide.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_ide.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 # pylint: disable=unused-argument
 
 
 from itertools import compress
-from typing import ClassVar, Tuple
+from math import inf
+from typing import ClassVar, Tuple, Union
 from dataclasses import dataclass
 
 from .. import html_builder as Html
 from ..tools_and_constants import HtmlClass, IdeConstants, Prefix, ScriptKind
 from ..messages import Tip
-from ..parsing import build_code_fence
+from ..parsing import build_code_fence, items_comma_joiner
 from ..paths_utils import convert_url_to_utf8, to_uri
 
 from .ide_manager import IdeManager
 
 
 
 
@@ -73,14 +74,56 @@
         auto_log_assert
         corr_rems_mask
         has_check_btn
     '''.split())
 
 
 
+    def _validate_files_config(self, max_attempts: Union[int,float] ):
+        msg = prop = None
+
+        if (not msg and self.env.forbid_secrets_without_corr_or_REMs
+            and self.has_secrets and not self.has_any_corr_rem
+        ):
+            msg,prop = (
+                "A `secrets` section exist but there are no `corr` section, REM or VIS_REM file.",
+                "forbid_secrets_without_corr_or_REMs"
+            )
+
+        elements = [*filter(bool,(
+            "a correction"   * (not self.has_corr),
+            "a REM file"     * (not self.has_rem),
+            "a VIS_REM file" * (not self.has_vis_rem),
+        ))]
+        elt_msg = items_comma_joiner(elements, 'and')
+        single  = len(elements)==1
+        elt_msg = f"{ elt_msg } exist{ 's' * (single)}".capitalize()
+
+        if (not msg and self.env.forbid_hidden_corr_and_REMs_without_secrets
+            and self.has_any_corr_rem and not self.has_secrets
+        ):
+            msg,prop = (
+                f"{ elt_msg }, but there is no `secrets` section.",
+                'forbid_hidden_corr_and_REMs_without_secrets'
+            )
+
+        if (not msg and self.env.forbid_corr_and_REMs_with_infinite_attempts
+            and max_attempts==inf and self.has_any_corr_rem
+        ):
+            subject = "it" if single else "they"
+            msg,prop = (
+                f"{ elt_msg }, but {subject} will never be visible because the number of "
+                "attempts is set to infinity.",
+                'forbid_corr_and_REMs_with_infinite_attempts'
+            )
+
+        self._validation_outcome(msg,prop)
+
+
+
 
     def generate_id(self):
         """
         Generate an id number for the current IDE (editor+terminal), as a "prefix_hash(32bits)".
 
         This id must be:
             - Unique to every IDE used throughout the whole website.
@@ -290,15 +333,15 @@
         """
         Build all buttons below an "ide" (editor+terminal).
         """
         buttons = ''.join([
             self.create_button("play"),
             self.create_button("check", btn_kind="validate") if self.has_check_btn else "",
             self.create_button("download", margin_left=1 ),
-            self.create_upload_button(margin_right=1),
+            self.create_button("upload", margin_right=1 ),
             self.create_button("restart"),
             self.create_button("save"),
         ])
 
         cnt_txt      = self.env.lang.attempts_left.msg
         cnt_txt_span = Html.span(cnt_txt + " : ", kls=HtmlClass.compteur_txt)
         cnt_or_inf   = self.max_attempts_symbol
@@ -309,26 +352,26 @@
             Html.div(buttons, kls=HtmlClass.ide_buttons_div)
             + Html.div(compteur, kls=HtmlClass.compteur_wrapper),
             kls = HtmlClass.ide_buttons_div_wrapper
         )
         return buttons_div
 
 
-    def create_upload_button(self, margin_right:float = 1) -> str:
-        """
-        @brief : Create upload button for an IDE number {id_ide}.
-        @details : Use an HTML input to upload a file from user. The user clicks on the button to
-        fire a JS event that triggers the hidden input.
-        """
-
-        input_button_controller = Html.input(
-            id = f"{ Prefix.input_ }{ self.editor_name }",
-            kls = HtmlClass.py_mk_hidden,
-            type = 'file',
-            name = 'file',
-            enctype = "multipart/form-data",
-        )
-        button = self.create_button(
-            "upload",
-            margin_right = margin_right,
-        )
-        return button + input_button_controller
+    # def create_upload_button(self, margin_right:float = 1) -> str:
+    #     """
+    #     @brief : Create upload button for an IDE number {id_ide}.
+    #     @details : Use an HTML input to upload a file from user. The user clicks on the button to
+    #     fire a JS event that triggers the hidden input.
+    #     """
+
+    #     input_button_controller = Html.input(
+    #         id = f"{ Prefix.input_ }{ self.editor_name }",
+    #         kls = HtmlClass.py_mk_hidden,
+    #         type = 'file',
+    #         name = 'file',
+    #         enctype = "multipart/form-data",
+    #     )
+    #     button = self.create_button(
+    #         "upload",
+    #         margin_right = margin_right,
+    #     )
+    #     return button + input_button_controller
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_files_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,26 +108,32 @@
     """ Bit mask giving the configuration for correction and/or remark data
         mask&1 represent the presence of correction, mask&2 is for REM.
     """
 
     env_content: str = ""
     """ Python header code content (run async) """
 
+    env_term_content: str = ""
+    """ Run unconditionally, only before a command of a terminal is run. """
+
     user_content:str = ""
     """ Python user code (only) """
 
     corr_content: str = ""
     """ Python solution code """
 
     public_tests: str = ""
     """ Public tests (only) """
 
     secret_tests:str = ""
     """ Code for the private tests """
 
+    post_term_content: str = ""
+    """ Run unconditionally, only after a command of a terminal was run. """
+
     post_content: str = ""
     """ Code for post executions (teardown / run async).
         Always run, even in case of failures in users or tests code, but NOT if an error
         occurred in the ENV section.
     """
 
 
@@ -142,20 +148,22 @@
 
 
     SECTION_TOKEN: ClassVar[re.Pattern] = re.compile(
         r'^(# *-+ *PYODIDE *: *\w+ *-+ *#)$', flags=re.MULTILINE
     )
 
     SECTION_TO_PROP: ClassVar[Dict[str,str]] = {
-        ScriptSection.env:     "env_content",
-        ScriptSection.user:    "user_content",
-        ScriptSection.corr:    "corr_content",
-        ScriptSection.tests:   "public_tests",
-        ScriptSection.secrets: "secret_tests",
-        ScriptSection.post:    "post_content",
+        ScriptSection.env:          "env_content",
+        ScriptSection.env_term:     "env_term_content",
+        ScriptSection.user:         "user_content",
+        ScriptSection.corr:         "corr_content",
+        ScriptSection.tests:        "public_tests",
+        ScriptSection.secrets:      "secret_tests",
+        ScriptSection.post_term:    "post_term_content",
+        ScriptSection.post:         "post_content",
     }
 
 
     @property
     def has_env(self):
         return bool(self.env_content)
     @property
@@ -206,14 +214,23 @@
         # if not self.skip_check and self.env.check_python_files:
         #     self.check_python()
 
         # self._fuuuuuusion()
         # self._cleanup_tests()
 
 
+    def get_sections_data(self, with_corr=True):
+        """ Returns an generator of tuples (property, content) for all sections. """
+        return (
+            (prop, getattr(self, prop))
+            for prop in self.SECTION_TO_PROP.values()
+            if with_corr or prop != "corr_content"
+        )
+
+
 
     def get_path_and_existence(self, tail:str):
         """
         Return a pair (Path|None, str).
         The path|None is the built path, relative to the CWD, or None if no file is found.
         The string is the file content (empty string if no file)
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -170,14 +170,19 @@
     """ Must be overridden in the child class """
 
     NEED_INDENTS: ClassVar[bool] = False
     """
     Specify the macro had adding multiline content (so it _will_ consume one indentation data).
     """
 
+    NEEDED_KINDS: ClassVar[Tuple[ScriptKind]] = ScriptKind.pyodide,
+    """
+    Register the kind of js scripts that must be added to the page, for the current object.
+    """
+
     KW_TO_TRANSFER: ClassVar[Tuple[ Union[str, Tuple[str,str]]] ]  = ()
     """
     Configuration of the keywords that should be extracted if given in the constructor.
     This is an Iterable of  (argument, property) pairs.
     If an element is a string, it will be used as (value, value.lower())
     """
 
@@ -186,39 +191,31 @@
     Configuration of the properties that should extract a global default value, if it's still
     set to None after the extra arguments have been handled.
     This is an Iterable of  (argument, property) pairs.
     """
 
     JS_EXPORTED_GENERICS: ClassVar[set] = set('''
         py_name
-        env_content
-        user_content
-        public_tests
-        secret_tests
-        post_content
         excluded
         excluded_methods
         rec_limit
         white_list
-    '''.split())
+    '''.split() + [
+        prop for prop in IdeFilesExtractor.SECTION_TO_PROP.values() if prop !="corr_content"
+    ])
     """
     Values that are always exported to JS, whatever the tool.
     """
 
     JS_EXPORTED_VALUES: ClassVar[set] = None
     """
     If defined, gives the names of all the properties that should be exported to JS.
     HAS TO BE OVERRIDDEN by the subclasses.
     """
 
-    NEEDED_KINDS: ClassVar[Tuple[ScriptKind]] = ScriptKind.pyodide,
-    """
-    Register the kind of js scripts that must be added to the page, for the current object.
-    """
-
 
     #-------------------------
 
 
     @property               # pylint: disable-next=all
     def has_corr(self):     return self.files_data.has_corr
     @property               # pylint: disable-next=all
@@ -285,24 +282,19 @@
         py_name = f"{root_name}-{py_path}".strip('-') or 'unknown'
 
         # Prepare the dump of configuration to JS:
         to_register: List[Tuple[str,Any]] = [
             #-----------------------------------------------------
             # Generic properties (always exported, but may be useless depending on the actual class)
             ('py_name',             py_name+'.py'),
-            ('env_content',         self.files_data.env_content),
-            ('user_content',        self.files_data.user_content),
-            ('public_tests',        self.files_data.public_tests),
-            ('secret_tests',        self.files_data.secret_tests),
-            ('post_content',        self.files_data.post_content),
-
             ("excluded",            excluded),
             ("excluded_methods",    excluded_methods),
             ("rec_limit",           self.rec_limit),
             ("white_list",          white_list),
+            *self.files_data.get_sections_data(with_corr=False),
 
             #-----------------------------------------------------
             # Specific to some concrete class
 
             # IDEs:
             ('attempts_left',       max_attempts),
             ("auto_log_assert",     self.auto_log_assert),
@@ -388,52 +380,15 @@
 
         max_attempts = inf if is_inf else int(max_ide)
         return max_attempts
 
 
 
     def _validate_files_config(self, max_attempts: Union[int,float] ):
-        msg = None,None
-
-        if (not msg and self.env.forbid_secrets_without_corr_or_REMs
-            and self.has_secrets and not self.has_any_corr_rem
-        ):
-            msg = (
-                "A `secrets` section exist but there are no `corr` section, REM or VIS_REM file.",
-                "forbid_secrets_without_corr_or_REMs"
-            )
-
-        elements = [*filter(bool,(
-            "a correction"   * (not self.has_corr),
-            "a REM file"     * (not self.has_rem),
-            "a VIS_REM file" * (not self.has_vis_rem),
-        ))]
-        elt_msg = items_comma_joiner(elements, 'and')
-        single  = len(elements)==1
-        elt_msg = f"{ elt_msg } exist{ 's' * (single)}".capitalize()
-
-        if (not msg and self.env.forbid_hidden_corr_and_REMs_without_secrets
-            and self.has_any_corr_rem and not self.has_secrets
-        ):
-            msg = (
-                f"{ elt_msg }, but there is no `secrets` section.",
-                'forbid_hidden_corr_and_REMs_without_secrets'
-            )
-
-        if (not msg and self.env.forbid_corr_and_REMs_with_infinite_attempts
-            and max_attempts==inf and self.has_any_corr_rem
-        ):
-            subject = "it" if single else "they"
-            msg = (
-                f"{ elt_msg }, but {subject} will never be visible because the number of "
-                "attempts is set to infinity.",
-                'forbid_corr_and_REMs_with_infinite_attempts'
-            )
-
-        self._validation_outcome(*msg)
+        raise NotImplementedError()
 
 
 
     def _validation_outcome(self, msg:Optional[str], config_opt:Optional[str]=None):
         if not msg:
             return
 
@@ -441,15 +396,15 @@
         if config_opt:
             msg += (
                 "\n    You can deactivate this check by setting plugins.pyodide_macros."
                 f"build.{config_opt} to false in `mkdocs.yml`."
             )
 
         if self.env._dev_mode:       # pylint: disable=protected-access
-            logger.error("DEV_MODE (expected x3) - " + msg)
+            logger.error("DEV_MODE (expected x5) - " + msg)
         else:
             raise BuildError(msg)
 
 
 
     def _compute_exclusions_and_white_list(self, prop:str):
         """
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_pybtn.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,20 +64,22 @@
     KW_TO_TRANSFER: ClassVar[Tuple[ Union[str, Tuple[str,str]]] ] = (
         'WRAPPER',
         'HEIGHT', 'SIZE', 'WIDTH', 'ICON',
         'TIP', 'TIP_SHIFT', 'TIP_WIDTH',
     )
 
 
-    def _validate_files_config(self, max_attempts: Union[int,float], msg=None):
+    def _validate_files_config(self, _: Union[int,float]):
 
         forbidden = [*filter(bool,(
+            "env_term code"  * bool(self.files_data.env_term_content),
             "user code"      * self.files_data.has_code,
             "public tests"   * self.files_data.has_tests,
             "secret tests"   * self.files_data.has_secrets,
+            "post_term code" * bool(self.files_data.post_term_content),
             "post code"      * self.files_data.has_post,
             "a correction"   * self.has_corr,
             "a REM file"     * self.has_rem,
             "a VIS_REM file" * self.has_vis_rem,
         ))]
 
         if forbidden:
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/ide_terminal.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         if 'FILL' not in self.extra_kw:
             self.extra_kw['FILL'] = ''
 
         super().handle_extra_args()
 
 
-    def _validate_files_config(self, _: Union[int,float], msg=None):
+    def _validate_files_config(self, _: Union[int,float]):
 
         forbidden = [*filter(bool,(
             "user code"      * self.files_data.has_code,
             "public tests"   * self.files_data.has_tests,
             "secret tests"   * self.files_data.has_secrets,
             "a correction"   * self.has_corr,
             "a REM file"     * self.has_rem,
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/messages.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/messages.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,18 +48,20 @@
     global variable specific to each page.
 
     Always instantiated without arguments, and items are updated when needed.
     """
 
     py_name:      str = ""          # name to use for downloaded file
     env_content:  str = ""          # HDR part of "exo.py"
+    env_term_content:  str = ""     # HDR part for terminal commands only
     user_content: str = ""          # Non-HDR part of "exo.py" (initial code)
     #corr_content: str = ""         # not exported to JS!
     public_tests: str = ""          # test part of "exo.py" (initial code)
     secret_tests: str = ""          # Content of "exo_test.py" (private tests)
+    post_term_content: str = ""     # Content to run after for terminal commands only
     post_content: str = ""          # Content to run after executions are done
 
     excluded: List[str] = None      # List of forbidden instructions (functions or packages)
     excluded_methods: List[str] = None # List of forbidden methods accesses
     rec_limit: int = None           # recursion depth to use at runtime, if defined (-1 otherwise).
     white_list: List[str] = None    # White list of packages to preload at runtime
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,17 +380,18 @@
 #     return out
 
 
 
 
 
 
-TOME_BASE = re.sub(r'[ <>"\[\]\\]', '', printable)[:-5]
+TOME_BASE = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!#$%'()*+,-./:;=?@^_`{|}~"
 """ Removed:
         - "<>" because could generate tags
+        - "&" because of &lt; stuff
         - "[]" because could be seen as md links syntaxe by mkdocs-addresses
 """
 BASE_TOME = {c:i for i,c in enumerate(TOME_BASE)}
 BASE      = len(TOME_BASE)
 
 
 @lru_cache(None)
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_indent.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,18 +264,20 @@
 
 
 class ScriptSection:
     """ Name of each possible section used in a "monolithic" python file """
     ignore  = AutoDescriptor()
 
     env = AutoDescriptor()
+    env_term = AutoDescriptor()
     user = AutoDescriptor("code")
     corr = AutoDescriptor()
     tests = AutoDescriptor()
     secrets = AutoDescriptor()
+    post_term = AutoDescriptor()
     post = AutoDescriptor()
 
 
 
 
 
 
@@ -333,13 +335,20 @@
 
 BLOCKS_KINDS = set('content libs scripts extrahead'.split())
 INSERTIONS_KINDS = {s for s in dir(ScriptKind) if not s.startswith('_')
                                                and not callable(getattr(ScriptKind, s)) }
 PAGES_KINDS = INSERTIONS_KINDS - BLOCKS_KINDS
 
 
+
+
+
 class DebugConfig(Namespace):
 
     check_decode = False
     """ If True, decode any LZW encoded string to check consistency """
 
     shuffle = True
+    """
+    If True, the alphabet built from the complete set of characters of the messages to
+    compress with LZW is shuffled.
+    """
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/scripts/custom_lang.py` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/scripts/custom_lang.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-"""
-pyodide-mkdocs-theme
-Copyleft GNU GPLv3 🄯 2024 Frédéric Zinelli
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
-See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.
-If not, see <https://www.gnu.org/licenses/>.
-"""
-
 
 from pyodide_mkdocs_theme.pyodide_macros import (
     PyodideMacrosPlugin,
     Msg, MsgPlural, TestsToken, Tip,
 )
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/scripts/mkdocs.yml` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/scripts/mkdocs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-# pyodide-mkdocs-theme
-# Copyleft GNU GPLv3 🄯 2024 Frédéric Zinelli
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
-# See the GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.
-# If not, see <https://www.gnu.org/licenses/>.
-
 # Voici un exemple presque complet de configuration pour un fichier
 # mkdocs.yml utilisant pyodide-mkdocs-theme.
 
 site_url: "{>> L'adresse de votre site web ici <<}"
 site_name: "{>> Titre pour votre site <<}"
 # site_description: "(optionnel)"
 # repo_url: "(optionnel)"
```

#### html2text {}

```diff
@@ -1,20 +1,11 @@
-# pyodide-mkdocs-theme # Copyleft GNU GPLv3 ð¯ 2024 FrÃ©dÃ©ric Zinelli # #
-This program is free software: you can redistribute it and/or modify # it under
-the terms of the GNU General Public License as published by # the Free Software
-Foundation, either version 3 of the License, or # (at your option) any later
-version. # # This program is distributed in the hope that it will be useful, #
-but WITHOUT ANY WARRANTY; without even the implied warranty of #
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. # See the GNU General
-Public License for more details. # # You should have received a copy of the GNU
-General Public License # along with this program. # If not, see
-www.gnu.org/licenses/>. # Voici un exemple presque complet de configuration
-pour un fichier # mkdocs.yml utilisant pyodide-mkdocs-theme. site_url: "{>>
-L'adresse de votre site web ici <<}" site_name: "{>> Titre pour votre site <<}"
-# site_description: "(optionnel)" # repo_url: "(optionnel)" # edit_uri: "
+# Voici un exemple presque complet de configuration pour un fichier #
+mkdocs.yml utilisant pyodide-mkdocs-theme. site_url: "{>> L'adresse de votre
+site web ici <<}" site_name: "{>> Titre pour votre site <<}" #
+site_description: "(optionnel)" # repo_url: "(optionnel)" # edit_uri: "
 (optionnel)" # Copyright "CC BY-NC-SA" copyright: |
 Partage ou adaptation possible selon les conditions de la licence _C_C_ _B_Y_-_N_C_-_S_A
 _4_._0_[_h_t_t_p_s_:_/_/_m_i_r_r_o_r_s_._c_r_e_a_t_i_v_e_c_o_m_m_o_n_s_._o_r_g_/_p_r_e_s_s_k_i_t_/_i_c_o_n_s_/_c_c_._s_v_g_?_r_e_f_=_c_h_o_o_s_e_r_-_v_1_]
 _[_h_t_t_p_s_:_/_/_m_i_r_r_o_r_s_._c_r_e_a_t_i_v_e_c_o_m_m_o_n_s_._o_r_g_/_p_r_e_s_s_k_i_t_/_i_c_o_n_s_/_b_y_._s_v_g_?_r_e_f_=_c_h_o_o_s_e_r_-_v_1_]
 _[_h_t_t_p_s_:_/_/_m_i_r_r_o_r_s_._c_r_e_a_t_i_v_e_c_o_m_m_o_n_s_._o_r_g_/_p_r_e_s_s_k_i_t_/_i_c_o_n_s_/_n_c_._s_v_g_?_r_e_f_=_c_h_o_o_s_e_r_-_v_1_]
 _[_h_t_t_p_s_:_/_/_m_i_r_r_o_r_s_._c_r_e_a_t_i_v_e_c_o_m_m_o_n_s_._o_r_g_/_p_r_e_s_s_k_i_t_/_i_c_o_n_s_/_s_a_._s_v_g_?_r_e_f_=_c_h_o_o_s_e_r_-_v_1_]
 docs_dir: docs nav: - "Accueil": index.md # - ... # Pour supprimer certains
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/README.md` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/assets/images/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/assets/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/assets/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/assets/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/assets/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/assets/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/assets/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -152,17 +152,17 @@
     // JS <-> python property names tracker
 
     cutFeedback: true,
     joinTerminalLines: false,
 
     // HDR_TOKEN_PATTERN:   /#\s*-[\s-]*HDR\s*-[\s-]*#/i,           // not used anymore
     COMMENTED_PATTERN: /(^\s*)(\S)(.?)/,
-    MODULE_REG: /File "<(env|post|exec|console)>", line (\d+)($|, in (?!await_fut))/,
-    TRACE_REG: /  File "<(env|post|exec|console)>"/,
-    TRACE_NUM_LINE: /File "<(?:env|post|exec|console)>", line (\d+)/,
+    MODULE_REG: /File "<(env[^>]*|post[^>]*|exec|console)>", line (\d+)($|, in (?!await_fut))/,
+    TRACE_REG: /  File "<(env[^>]*|post[^>]*|exec|console)>"/,
+    TRACE_NUM_LINE: /File "<(?:env[^>]*|post[^>]*|exec|console)>", line (\d+)/,
 
     ESCAPE_SQ_B: /\[|\]/g,
     UNESCAPE_SQ_B: new RegExp(`[${ SqBs.L }${ SqBs.R }]`, 'g'),
 
     ACE_COLOR_THEME: {
         customTheme: undefined,
         customThemeDefaultKey: "",
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -191,21 +191,25 @@
 let info = (content) => richTextFormat(content, "i", "grey");
 let italic = (content) => richTextFormat(content, "i");
 let success = (content) => richTextFormat(content, "ib", "green");
 let failure = (content) => richTextFormat(content, "ib", "orange");
 
 
 // Update CONFIG strings on the fly:
-'successMsg runScript installStart installDone'
-.split(' ').forEach(
+'successMsg runScript installStart installDone'.split(' ').forEach(
     prop => CONFIG.lang[prop].msg = info(CONFIG.lang[prop].msg)
 )
 
 
 
+function toSnake(msg) {
+    return msg.replace(/[A-Z]/g, m => '_' + m.toLowerCase())
+}
+
+
 
 /**Takes a string and cut the "middle chunk" of them if it is considered too long (length > 1750),
  * shortening it in the following way:
  *   - keep the 500 first and 300 last chars
  *   - replace the middle with a message
  * */
 function textShortener(text) {
@@ -251,40 +255,34 @@
         throw new Error("Cannot pick from an empty array")
     }
     const i = Math.random() * arr.length | 0
     return arr[i]
 }
 
 
-/**Applique c ^ key à chaque nombre de text
- * (Nota: 43960 = 0b1010101010101010)
- * */
-const decrypt_string = (text, key = 43960) => {
-    if (!CONFIG.encryptCorrectionsAndRems) return text
-    return text.split('.').map(c => String.fromCodePoint(key ^ +c)).join('')
-}
 
-const ALPHA = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!#$%&'()*+,-./:;=?@^_`{|}~"
+
+const ALPHA = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!#$%'()*+,-./:;=?@^_`{|}~"
 const TOME_B = [...ALPHA].reduce((o, c, i) => (o[c] = i, o), {})
 
 const unBase = s => [...s].reduce((v, c) => v * ALPHA.length + TOME_B[c], 0)
 
 /**@txt: CONFIG.LZW separated lines, with:
- *      1. dot separated unicode char codes
+ *      1. A dot + dots separated unicode codePoints
  *      2. regular alpha
  *      3. compressed data, size 2
  *      4. ..., size 3,
  *      5. ...
  */
 const decompressLZW = (compressed) => {
 
     const [bigs, smalls, ...chunks] = compressed.trim().split(CONFIG.LZW)
     const tome = [
         [...'><'],
-        bigs == '.' ? [] : bigs.slice(1) // no initial dot
+        bigs == '.' ? [] : bigs.slice(1)
         .split('.')
         .map(n => String.fromCodePoint(+n)),
         [...smalls],
     ].flat()
 
     let txt = [],
         size = 1,
@@ -330,8 +328,71 @@
     if (window.getSelection) {
         text = window.getSelection().toString();
 
     } else if (document.selection && document.selection.type != "Control") {
         text = document.selection.createRange().text;
     }
     return text;
-}
+}
+
+
+
+
+
+
+/**Apply a "download" action, given the content, name and type of the file to download.
+ * */
+function downloader(content, filename, type = "text/plain") {
+    let blob = new Blob([content], {
+        type
+    })
+    let link = document.createElement("a")
+    link.href = URL.createObjectURL(blob)
+    link.download = filename
+    link.click()
+    URL.revokeObjectURL(link.href)
+    link.remove()
+}
+
+
+/**Routine reusing the very same input[type=file] element (hidden in <head>) to upload content.
+ * It must receive a callback that will handle the action to do with the content of the uploaded
+ * file.
+ * Returns a curried event executor: (cbk)=>[event executor function}
+ * */
+var [uploader, uploaderAsync] = (function() {
+
+    const jInput = $('<input id="pyodide-file-uploader" name="file-uploader" type="file" enctype="multipart/form-data">')
+    $(document.head).append(jInput)
+
+    let contentHandler = null // Replaced on the fly at runtime
+
+    jInput[0].addEventListener("change", function(changeEvent) {
+            let file = changeEvent.target.files[0]
+            let reader = new FileReader();
+            reader.onload = function(event) {
+                contentHandler(event.target.result)
+                contentHandler = null // to spot end of execution in async way
+            }
+            reader.readAsText(file)
+        },
+        false
+    )
+
+    const uploader = (cbk) => _ => {
+        contentHandler = cbk
+        jInput.click()
+        console.log()
+        // This is ABSOLUTELY NEEDED, otherwise "Le sélecteur <input> a été bloqué faute
+        // d’activation par l’utilisateur." when used from pyodide... XD
+    }
+
+    const uploaderAsync = (cbk) => async _ => {
+        uploader(cbk)()
+        // Wait until the upload is done, so that the uploaded content is usable in pyodide
+        while (contentHandler) {
+            await sleep(200)
+        }
+    }
+
+    return [uploader, uploaderAsync]
+})()
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-per-pages/0_genericPythonSnippets-pyodide.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -51,68 +51,112 @@
 
 const terminalFeatureCode = (option) => {
 
     switch (option) {
 
         case "inputPrompt":
             return `
-def _hack():
+def _hack_3():
     if not getattr(__builtins__, '__js_input__',None):
         import js
         __builtins__.__js_input__ = js.inputWithPrompt
     __builtins__.input = __js_input__
-_hack()
-del _hack
+_hack_3()
+del _hack_3
 `
 
 
         case "version":
             return `
 def version():
     print("pyodide-mkdocs-theme v${ CONFIG.version }")`
 
 
 
         case "exclusionsTools":
             return `
-def _hack():
+def _hack_4():
 
     def __move_forward__(stuff):
         treasure = __builtins__.__builtins___
         if type(stuff) is str and stuff in treasure:
             return treasure[stuff][0]
 
     class ExclusionError(Exception):
         @staticmethod
         def throw(that:str):
             raise ExclusionError(f"${ CONFIG.MSG.exclusionMarker }: don't use {that}")
 
     __builtins__.__move_forward__ = __move_forward__
     __builtins__.ExclusionError = ExclusionError
 
-_hack()
-del _hack
+_hack_4()
+del _hack_4
 `
 
         case "refresher":
             return `
-def _hack():
+def _hack_5():
     def clear_scope(skip=()):
         keeper = set(skip) | {
             '__name__', '__doc__', '__package__', '__loader__', '__spec__',
             '__annotations__', '__builtins__', '_pyodide_core', 'version'
         }
         g_dct = globals()
         for k in list(globals()):
             if k not in keeper:
                 del g_dct[k]
 
     __builtins__.clear_scope = clear_scope
-_hack()
-del _hack
+_hack_5()
+del _hack_5
+`
+
+        case "upDownLoader":
+            return `
+def _hack_A():
+
+    import js
+    from pyodide.ffi import create_proxy
+    from typing import Callable, Any as AnyType
+
+
+    def wrapping(cbk):
+
+        def wrapper(content:str):
+            nonlocal out
+            out = cbk(content)
+            proxy_cbk.destroy()
+
+        proxy_cbk = create_proxy(wrapper)    # Does NOT work when using pyodide.ffi.create_once_callable
+        out = None
+
+        return proxy_cbk, lambda:out
+
+
+    async def pyodide_uploader_async(cbk:Callable[[str],AnyType]) -> AnyType:
+        proxy_cbk, out_getter = wrapping(cbk)
+        await js.uploaderAsync(proxy_cbk)()
+        return out_getter()
+
+    def pyodide_uploader(cbk:Callable[[str],None]) -> None:
+        proxy_cbk, _ = wrapping(cbk)
+        js.uploader(proxy_cbk)()
+
+
+    def pyodide_downloader(content:str, filename:str, type="text/plain"):
+        js.downloader(content, filename, type)
+
+
+    __builtins__.pyodide_uploader_async = pyodide_uploader_async
+    __builtins__.pyodide_uploader       = pyodide_uploader
+    __builtins__.pyodide_downloader     = pyodide_downloader
+
+_hack_A()
+del _hack_A
 `
         default:
             throw new Error(`Unknown feature: ${option}`)
     }
 }
 
 
@@ -131,33 +175,33 @@
 */
 
 
 /**Rely on pyodide to analyze the code content and find the imports the user is trying to use.
  * */
 const getUserImportedModules = (code) => {
     return pyodide.runPython(`
-    def _hack():
+    def _hack_6():
         from pyodide.code import find_imports
         __builtins__.imported_modules = find_imports(${JSON.stringify(code)})
-    _hack()
-    del _hack
+    _hack_6()
+    del _hack_6
     __builtins__.imported_modules
     `);
 }
 
 
 /**Extract all the packages names currently available in pyodide.
  * */
 const getAvailablePackages = () => {
     return new Set(pyodide.runPython(`
-    def _hack():
+    def _hack_7():
         import sys
         __builtins__.loaded_modules = " ".join(sys.modules.keys())
-    _hack()
-    del _hack
+    _hack_7()
+    del _hack_7
     __builtins__.loaded_modules
     `).split(' '))
 }
 
 
 
 
@@ -171,31 +215,31 @@
 ------------------------------------------------------------------
 */
 
 
 /**Use a StringIO stdout, so that the full content can be extracted later
  * */
 const setupStdIO = _ => pyodide.runPython(`
-    def _hack():
+    def _hack_8():
         import sys, io
         __builtins__.src_stdout = sys.stdout
         sys.stdout = io.StringIO()
-    _hack()
-    del _hack
+    _hack_8()
+    del _hack_8
 `)
 
 const getFullStdIO = _ => escapeSquareBrackets(pyodide.runPython(`
-    def _hack():
+    def _hack_9():
         import sys
         __builtins__._stdout = sys.stdout.getvalue()
         sys.stdout.close()
         sys.stdout = __builtins__.src_stdout
         del __builtins__.src_stdout
-    _hack()
-    del _hack
+    _hack_9()
+    del _hack_9
     __builtins__._stdout
 `) || '')
 
 
 
 
 
@@ -208,15 +252,15 @@
 ------------------------------------------------------------------
 */
 
 
 /**Put in place code exclusions. Are handled:
  *   - builtin function calls
  *   - imports
- *   - method calls (done through a simple string check in the code, in runPythonCodeWithOptions)
+ *   - method calls (done through a simple string check in the code, in runPythonCodeWithOptionsIfNoStdErr)
  *
  *
  * ## RATIONALS:
  *
  * To forbid the use of some functions or packages, replace them in the global scope by "functions"
  * that look "more or less the same", but will raise an error when called, or when used in the
  * wrong way (imports).
@@ -272,15 +316,15 @@
      *  Keep in mind that the code of the Raiser instances will run "in context".
      *  This means it will be subject to existing exclusions, so it must never use a function that
      *  could be forbidden. Possibly...
      *  Force this reason, copies of all the builtins used in the Raiser code are stored locally,
      *  to be sure the Raiser won't use Raiser instances... XD
      * */
     const code = `
-    def _hack():
+    def _hack_10():
 
         class Raiser:
             __name__ = __qualname__ = 'function'
 
             def __init__(self, key):  self.key = key
 
             def __repr__(self): return f"<built-in function {self.key}>"
@@ -325,27 +369,27 @@
 
         for key,lst in dct.items():
             stuff = lst[0]
             if callable(stuff) and key!='__import__':       # import already handled
                 globals()[key] = lst[1] = Raiser(key)
                 # store the reference to the raiser, to check against it later
 
-    _hack()
-    del _hack `
+    _hack_10()
+    del _hack_10 `
 
     pyodide.runPython(code)
 }
 
 
 
 /**Cancel the code exclusions (done as soon as possible, to restore pyodide's normal behaviors).
  * */
 const restoreOriginalFunctions = exclusions => {
     pyodide.runPython(`
-    def _hack():
+    def _hack_11():
         G = globals()
 
         not_ok = any(
             key for key,(func,raiser) in __builtins___.items()
                 if raiser is not None and key!='__import__' and raiser is not G.get(key)
         )
         if not_ok:
@@ -356,11 +400,11 @@
             if key == '__import__':
                 __builtins__.__import__ = func
 
             elif func is not None:
                 G[key] = func
                 if key == 'setrecursionlimit':
                     func(1000)
-    _hack()
-    del _hack
+    _hack_11()
+    del _hack_11
     `)
 }
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-per-pages/1_pyodideSectionsRunner-pyodide.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -34,26 +34,32 @@
     }
     get corrRemsMask() {
         return this.no_undefined('corrRemsMask')(this.data.corr_rems_mask)
     }
     get envContent() {
         return this.no_undefined('envContent')(this.data.env_content)
     }
+    get envTermContent() {
+        return this.no_undefined('envTermContent')(this.data.env_term_content)
+    }
     get excluded() {
         return this.no_undefined('excluded')(this.data.excluded)
     }
     get excludedMethods() {
         return this.no_undefined('excludedMethods')(this.data.excluded_methods)
     }
     get hasCheckBtn() {
         return this.no_undefined('hasCheckBtn')(this.data.has_check_btn)
     }
     get postContent() {
         return this.no_undefined('postContent')(this.data.post_content)
     }
+    get postTermContent() {
+        return this.no_undefined('postTermContent')(this.data.post_term_content)
+    }
     get prefillTerm() {
         return this.no_undefined('prefillTerm')(this.data.prefill_term)
     }
     get publicTests() {
         return this.no_undefined('publicTests')(this.data.public_tests)
     }
     get pyName() {
@@ -69,25 +75,28 @@
         return this.no_undefined('userContent')(this.data.user_content)
     }
     get whiteList() {
         return this.no_undefined('whiteList')(this.data.white_list)
     }
     //JS_CONFIG_DUMP
 
+
     constructor(id) {
         this.id = id
         this.decompressPagesIfNeeded()
         this.data = PAGE_IDES_CONFIG[id]
         if (CONFIG._devMode)
             CONFIG.objs[this.id] = this
         else {
             delete PAGE_IDES_CONFIG[id]
         }
+        this.alreadyRanEnv = false
     }
 
+
     decompressPagesIfNeeded() {
         if (typeof(PAGE_IDES_CONFIG) != 'string') return;
         const decompressed = decompressLZW(PAGE_IDES_CONFIG)
         PAGE_IDES_CONFIG = JSON.parse(
             decompressed, (key, val) => key == 'attempts_left' && val == "Infinity" ? Infinity : val
         )
     }
@@ -131,15 +140,15 @@
     }
 
 
 
 
 
     /**Given an editorName, automatically build the default options to pass as argument to the
-     * runPythonCodeWithOptions function.
+     * runPythonCodeWithOptionsIfNoStdErr function.
      *
      * The content of the config optional argument will override any basic option, except for
      * the packagesAliases object, where the config.packagesAliases entries will be added.
      *
      * @returns: an options object, described as follow:
      *     @options :
      *          .autoLogAssert:   (boolean) If true, will automatically add the code of a failing
@@ -154,80 +163,88 @@
      *          .withStdOut:      (boolean) Display the content of the stdOut or not.
      *          .whiteList:       (Array of strings) list of modules to import before the code
      *                            restrictions are put in place for the user's code.
      *
      * WARNING: If the editorName argument isn't given or is falsy, the fields excluded, whiteList
      *          and recLimit are not included.
      * */
-    buildOptionsForPyodideRun(config = {}) {
+    buildRunConfig(config = {}) {
         return {
+            // --- Python logistic related ---
             autoLogAssert: true, // default for the PUBLIC tests...
             excluded: this.excluded,
             excludedMethods: this.excludedMethods,
             isPublic: true,
             recLimit: this.recLimit,
             runCodeAsync: async (code) => pyodide.runPython(code),
             whiteList: this.whiteList,
             withStdOut: true, // default for the PUBLIC tests...
             ...config,
-            packagesAliases: {
-                // turtle: "pyo_js_turtle",         // this never got finished => unusable.
+            packagesAliases: { // useless so far...
+                // turtle: "pyo_js_turtle",     // this never got finished => unusable.
                 ...config.packagesAliases || {}
             },
+
+            // --- Runtime logistic related ---
+            stdErr: "", // First encountered error message
+            finalMsg: CONFIG.lang.successMsg.msg,
+            isAssertErr: false, // is the error an assertion error
+            envCrash: false, // true if error other than "assert" during any "env" step
         }
     }
 
 
 
 
 
     /**Extract the content of an environment code, and run its content into pyodide environment.
      *    - Stdout will be visible if an interface is available.
      *    - StdErr will be visible if an interface is available, and if none, an alert will be
      *      used (because environment code should never fail...)
      * */
     async runEnvironmentAsync(options, name) {
-        const prop = `${name}Content`
-        const content = this[prop].trim()
-
-        let stdErr = '',
-            isAssertErr = false
-        setupStdIO()
-        try {
-            if (content) {
+        const prop = `${ name }Content`
+        const content = name && this[prop].trim()
+        if (content && name && !options.envCrash) {
+            setupStdIO()
+            let localErr = ""
+            try {
                 // make sure packages are installed
                 await this.installAndImportMissingModules(content, options)
 
                 // run env/post content
                 await pyodide.runPythonAsync(content, {
-                    filename: `<${name}>`
+                    filename: `<${ toSnake(name) }>`
                 })
-            }
 
-            // If an error occurred, give feedback in the console, with stdout teardown on the way,
-            // then stop everything :
-        } catch (err) {
-            ;
-            [stdErr, isAssertErr] = generateErrorLog(err, "", false)
-        } finally {
-            this.giveFeedback(getFullStdIO(), stdErr, true)
+                // If an error occurred, give feedback in the console, with stdout teardown on the way,
+                // then stop everything :
+            } catch (err) {
+                ;
+                [options.stdErr, options.isAssertErr] = generateErrorLog(err, "", false)
+                localErr = options.stdErr
+                if (!options.isAssertErr && name.startsWith('env')) {
+                    options.envCrash = true
+                }
+            } finally {
+                this.giveFeedback(getFullStdIO(), localErr, true)
+            }
         }
-        return [stdErr, isAssertErr]
     }
 
 
 
 
 
     /**Explore the user's code to find missing modules to install. If some are found, load micropip
      * (if not done yet), then install all the missing modules.
      * Also import all the packages present in options.whiteList.
      *
      * @code : the python code to run.
-     * @options :Same as `buildOptionsForPyodideRun`.
+     * @options :Same as `buildRunConfig`.
      * */
     async installAndImportMissingModules(code, options) {
 
 
         const installedModules = getAvailablePackages()
         const wantedModules = getUserImportedModules(code)
 
@@ -246,35 +263,33 @@
         // Things to import whatever happens:
         const preImport = whiteList.map(name => 'import ' + name)
 
         if (missing.length || needPyLibs.length) {
             this.giveFeedback(CONFIG.lang.installStart.msg)
 
             for (const lib of needPyLibs) {
-                try {
-                    const archive = `${ CONFIG.baseUrl }/${ lib }.zip`
-                    const zipResponse = await fetch(archive)
-                    const zipBinary = await zipResponse.arrayBuffer()
-                    pyodide.unpackArchive(zipBinary, "zip", {
-                        extractDir: lib
-                    })
-                } catch (_) {}
+                const archive = `${ CONFIG.baseUrl }/${ lib }.zip`
+                const zipResponse = await fetch(archive)
+                const zipBinary = await zipResponse.arrayBuffer()
+                pyodide.unpackArchive(zipBinary, "zip", {
+                    extractDir: lib
+                })
             }
 
             if (missing.length) {
                 await pyodide.loadPackage("micropip");
                 let micropip = pyodide.pyimport("micropip");
 
-                for (let name of missing) {
-                    if (name in pkgReplacements) {
-                        preImport.push(`import ${ pkgReplacements[name] } as ${ name }`)
-                        name = pkgReplacements[name]
+                for (let lib of missing) {
+                    if (lib in pkgReplacements) {
+                        preImport.push(`import ${ pkgReplacements[lib] } as ${ lib }`)
+                        lib = pkgReplacements[lib]
                     }
-                    jsLogger("[Micropip] - Install", name)
-                    await micropip.install(name);
+                    jsLogger("[Micropip] - Install", lib)
+                    await micropip.install(lib);
                 }
             }
 
             this.giveFeedback(CONFIG.lang.installDone.msg)
         }
 
         // Import everything that is needed (either because module aliasing or because the code
@@ -300,27 +315,26 @@
     async setupRuntime() {
 
         Object.entries({
             exclusionsTools: true,
             inputPrompt: true,
             version: true,
             refresher: true,
+            upDownLoader: true,
         }).forEach(([opt, todo]) => {
             jsLogger("[Feature (re-/load)] -", opt)
             if (todo) pyodide.runPython(terminalFeatureCode(opt))
         })
 
         // Build the default configuration options to use to run the user's code:
-        const options = this.buildOptionsForPyodideRun()
-        const [stdErr, isAssertErr] = await this.runEnvironmentAsync(options, 'env')
-        return {
-            options,
-            stdErr,
-            isAssertErr
-        }
+        const options = this.buildRunConfig()
+        await this.runEnvironmentAsync(options, 'env')
+        this.alreadyRanEnv = true
+        if (options.stdErr && !options.isAssertErr) options.envCrash = true
+        return options
     }
 
 
 
     /**Takes a code as argument, and run it in the pyodide environment, using various options:
      *
      * @throws: Any JS runtime Error, if something went very wrong... (python errors are swallowed
@@ -334,18 +348,18 @@
      *    - Pyodide itself is using eval, so replacing globally the builtin will cause a lot of
      *      troubles and just won't work.
      *    - This function doesn't take in charge the pyodide environment setup, (preparation,
      *      rebuilding the setup, ...).
      *    - On the other hand it DOES take in charge installation of missing modules/packages
      *      in the user's/given code.
      */
-    async runPythonCodeWithOptions(code, options) {
+    async runPythonCodeWithOptionsIfNoStdErr(code, options) {
 
         // Do nothing if nothing to do...!
-        if (!code.trim()) return ""
+        if (options.stdErr || !code.trim()) return;
 
         try {
             // Do first the methods exclusions check, to gain some time (avoids loading modules if
             // the error would show up anyway after loading them)
             const nope = options.excludedMethods.filter(methodCall => code.includes(methodCall))
             if (nope.length) {
                 const plural = nope.length > 1 ? "s" : ""
@@ -354,30 +368,31 @@
                 throw new PythonError(msg)
             }
 
             // Detect possible user imports and install the packages to allow their imports:
             await this.installAndImportMissingModules(code, options)
 
         } catch (err) {
-            const [strErr, _] = generateErrorLog(err, code, false, !options.isPublic)
-            return this.giveFeedback("", strErr)
+            ;
+            [options.stdErr, ] = generateErrorLog(err, code, false, !options.isPublic)
+            this.giveFeedback("", options.stdErr)
+            return
         }
 
         const withExclusions = options.excluded.length > 0 || options.recLimit > 0
 
         // Setup stdout capture. WARNING: this must always be done even if it's not shown to the user.
         // If not done, a previous execution might have close the StringIO and if ever the user prints
         // something, it would result in an error without that:
         setupStdIO()
 
         // Setup code/imports exclusions if any (later id better)
         if (withExclusions) setupExclusions(options.excluded, options.recLimit)
 
-        let stdErr = "",
-            stdOut = "",
+        let stdOut = "",
             delayedErr, _ // "_" to avoid loosing lodash...
         try {
             await options.runCodeAsync(code)
         } catch (err) {
             // Since generateErrorLog might run python code, the exclusions must be removed _before_
             // the function is called, so store the error for later use.
             delayedErr = err
@@ -388,45 +403,41 @@
             // try/catch/finally construct:
             try {
                 if (withExclusions) restoreOriginalFunctions(options.excluded)
 
                 // Now only, compute the error message if needed.
                 if (delayedErr) {
                     ;
-                    [stdErr, _] = generateErrorLog(delayedErr, code, options.autoLogAssert, !options.isPublic)
+                    [options.stdErr, _] = generateErrorLog(delayedErr, code, options.autoLogAssert, !options.isPublic)
                 }
 
                 // Always extract the stdout and close the buffer (avoid memory leaks)
                 let captured = getFullStdIO()
 
                 // Send stdout feedback to the user only if allowed:
                 if (options.withStdOut) {
                     stdOut = textShortener(captured)
                 }
 
             } catch (err) {
                 // This second catch is there so that the user can see the JS error in the terminal.
                 // (Note: maybe I should actually throw them again...?)
                 ;
-                [stdErr, _] = generateErrorLog(err, code, true)
+                [options.stdErr, _] = generateErrorLog(err, code, true)
 
             } finally {
                 // Use a finally clause, in case something went wrong in generateErrorLog...
                 // (the message probably won't be accurate, but at least, something will be visible)
-                this.giveFeedback(stdOut, stdErr)
+                this.giveFeedback(stdOut, options.stdErr)
             }
-            return stdErr
         }
     }
 
 
 
 
-    async teardownRuntime(options, _gotError, _finalMsg = "") {
+    async teardownRuntime(options) {
         jsLogger("[Teardown] - PyodideRunner")
-
-        const out = await this.runEnvironmentAsync(options, 'post')
+        await this.runEnvironmentAsync(options, 'post')
         this.globalTearDown()
-        return out
     }
-
 }
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-per-pages/2_btnRunner-pyodide.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -30,16 +30,12 @@
 
 
     playFactory() {
         return withPyodideAsyncLock('playBtn', async (e) => {
             jsLogger("[playBtn]")
             if (e && e.preventDefault) e.preventDefault() // Useless for buttons, but keep it anyway...
 
-            let {
-                options,
-                stdErr,
-                _
-            } = await this.setupRuntime()
-            await this.teardownRuntime(options, stdErr, false)
+            const options = await this.setupRuntime()
+            await this.teardownRuntime(options)
         })
     }
 }
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-per-pages/2_terminalRunner-terms.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -22,14 +22,15 @@
 
 class _TerminalHandler extends PyodideSectionsRunner {
 
     constructor(id) {
         super(id)
         this.terminal = null
         this.termEnabled = false
+        this.alreadyRanPost = false
     }
 
     addResizer() {
         // Add resize listener (throttled):
         const topDiv = this.terminal.closest(".py_mk_wrapper")
         window.addEventListener('resize', _.throttle(_ => {
             const wWrapper = topDiv.width()
@@ -132,30 +133,31 @@
             }
         })
     }
 
     getAsyncPythonExecutor() {
         throw new Error('Should be overridden in the child class.')
     }
-}
 
 
+    prefillTermIfAllowed() {
+        if (this.prefillTerm) this.terminal.set_command(this.prefillTerm)
+    }
+
+}
 
 
 
 
 
 
 
-class TerminalRunner extends _TerminalHandler {
 
-    prefillTermIfAllowed() {
-        if (this.prefillTerm) this.terminal.set_command(this.prefillTerm)
-    }
 
+class TerminalRunner extends _TerminalHandler {
 
 
     /**When a terminal is available, display stdout and errors if any
      * */
     giveFeedback(stdout, stdErr = "", _) {
         if (stdErr) stdErr = error(stdErr)
         const msg = (stdout + stdErr).trim()
@@ -177,31 +179,34 @@
      * Using super calls, because one only wants the setup specific to terminal here, while "this"
      * could be an IdeRunner object. Ine that case, this.setupRuntime would run the setup for the
      * code in the editor, and not the command typed in the terminal.
      * This also way work with TerminalRunners, because the generic setupRuntime is _NOT_ on the
      * TerminalRunner class, but actually on the PythonSectionRunner one.
      *
      * For the very same kind of reasons, the `options` used cannot be the ones returned as usual
-     * by this.runPythonCodeWithOptions, because the terminal commands are run async, so store
+     * by this.runPythonCodeWithOptionsIfNoStdErr, because the terminal commands are run async, so store
      * locally the needed version.
      */
     getAsyncPythonExecutor() {
         const commandsBuffer = []
 
         return withPyodideAsyncLock('terminal', async (command) => {
 
             commandsBuffer.push(command)
             this.storeUserCodeInPython('__USER_CMD__', commandsBuffer.join('\n'))
             this.terminal.pause()
 
-            let outcome
+            let options
             try {
-                outcome = await super.setupRuntime()
-                /* HAS to be done before the pyconsole.push, otherwise, because of async loop
-                   scheduling, the environment is setup AFTER the user command has been run...
+                const needEnv = !this.alreadyRanEnv && this.envContent
+                options = needEnv ? await super.setupRuntime() : this.buildRunConfig()
+                await this.runEnvironmentAsync(options, 'envTerm')
+                /* The ASYNC potential calls to setupRuntime HAVE to be done before the pyconsole.push,
+                   otherwise, because of async loop scheduling, the environment is setup AFTER the user
+                   command has been run...
                    Because of this, need the commandBuffer to update the __USER_CMD__ variable, and
                    _also_ because of this, the env section will also run on incomplete commands...
                 */
 
                 // multiline commands should be split (useful when pasting)
                 for (let c of command.split("\n")) {
 
@@ -211,18 +216,24 @@
                     const isIncompleteExpr = future.syntax_check == "incomplete"
                     const headLine = isIncompleteExpr ? CONFIG.MSG.promptWait : CONFIG.MSG.promptStart
                     this.terminal.set_prompt(headLine);
 
                     switch (future.syntax_check) {
                         case "complete":
                             try {
-                                outcome.options.runCodeAsync = async _ => {
+                                /* NOTE: nothing can be awaited in between the future "creation" and the
+                                   execution of options.runCodeAsync, otherwise the loop event will actually
+                                   compute the result of the python command (which is already stored in the
+                                   loop event, now) before the restrictions are put in place in the environment
+                                   (everything is synch up to this...).
+                                 */
+                                options.runCodeAsync = async _ => {
                                     await pyFuncs.await_fut(future)
                                 }
-                                if (!outcome.stdErr) await this.runPythonCodeWithOptions(command, outcome.options)
+                                await this.runPythonCodeWithOptionsIfNoStdErr(command, options)
                             } finally {
                                 commandsBuffer.length = 0
                                 future.destroy() // to destroy only if it got awaited first
                                 await sleep() // Enforce GUI update, going through the next tick
                             }
                         case "incomplete":
                             continue // complete also goes there...
@@ -234,13 +245,19 @@
                         default:
                             commandsBuffer.length = 0
                             throw new Error(`Unexpected state ${future.syntax_check}`);
                     }
                 }
 
             } finally {
-                super.teardownRuntime(outcome.options) // Will Release the terminal to the user
+
+                await this.runEnvironmentAsync(options, 'postTerm')
+                if (this.alreadyRanEnv && !this.alreadyRanPost) {
+                    this.alreadyRanPost = true
+                    await this.runEnvironmentAsync(options, 'post')
+                }
+                this.globalTearDown()
                 this.storeUserCodeInPython('__USER_CMD__', "")
             }
         })
     }
 }
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-per-pages/3_ideRunner-ides.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -28,15 +28,15 @@
         this.commentIdH = "#comment_" + editorId
         this.globalIdH = "#global_" + editorId
         this.inputIdH = "#input_" + editorId
         this.counterH = "#compteur_" + editorId
         this.maxIdeSize = 0
         this.isV = false
         this.resized = true
-        this.corrHidden = true
+        this.hiddenDivContent = true
         this.editorCode = ""
     }
 
 
 
     // @Override
     build() {
@@ -47,30 +47,18 @@
         if (this.isV) this.resized = false
 
         this.setupAceEditor() // Create and define this.editor
 
         // Bind the ### "button":
         $(this.commentIdH).on("click", this.toggleComments.bind(this))
 
-        // Bind the input file, for downloads:
-        const uploadInput = $(this.inputIdH)
-
-        document // Note: doesn't want to work with jQuery... Dunno why
-            .getElementById(this.inputIdH.slice(1))
-            .addEventListener("change", function(changeEvent) {
-                    let reader = new FileReader();
-                    reader.onload = function(event) {
-                        ideThis.editor.getSession().setValue(event.target.result);
-                    };
-                    let file = changeEvent.target.files[0];
-                    reader.readAsText(file);
-                    ideThis.focusEditor()
-                },
-                false
-            )
+        const ideLoader = txt => {
+            this.applyCodeToEditorAndSave(txt)
+            this.focusEditor()
+        }
 
         // Bind all buttons below the IDE
         $(this.globalIdH).find("button").each(function() {
             const btn = $(this)
             const kind = btn.attr('btn_kind')
             let callback
             switch (kind) {
@@ -81,15 +69,15 @@
                     callback = ideThis.validateFactory();
                     break
 
                 case 'download':
                     callback = _ => ideThis.download();
                     break
                 case 'upload':
-                    callback = _ => uploadInput.click();
+                    callback = uploader(ideLoader);
                     break
 
                 case 'restart':
                     callback = _ => ideThis.restart();
                     break
                 case 'save':
                     callback = _ => {
@@ -319,25 +307,15 @@
 
     /**Download the current content of the editor to the download folder of the user.
      * */
     download() {
         jsLogger("[Download]")
 
         let ideContent = this.getCurrentEditorCode() + "" // enforce stringification in any case
-        let blob = new Blob([ideContent], {
-            type: "text/plain"
-        })
-        let link = document.createElement("a")
-        link.href = URL.createObjectURL(blob)
-        link.download = this.pyName
-
-        link.click()
-        URL.revokeObjectURL(link.href)
-        link.remove()
-
+        downloader(ideContent, this.pyName)
         this.focusEditor()
     }
 
 
     /**Reset the content of the editor to its initial content, and reset the localStorage for
      * this editor on the way.
      * */
@@ -412,55 +390,49 @@
         await sleep(200)
 
         return super.setupRuntime()
     }
 
 
 
-    async teardownRuntime(options, gotError, gotFinal) {
-        jsLogger("[Teardown] - IdeRunner -", JSON.stringify(gotError))
+    async teardownRuntime(options) {
+        jsLogger("[Teardown] - IdeRunner -", JSON.stringify(options.stdErr))
 
-        if (!gotError && !gotFinal) {
-            this.giveFeedback(CONFIG.lang.successMsg.msg)
+        if (!options.stdErr) {
+            this.giveFeedback(options.finalMsg)
         }
-        await super.teardownRuntime(options, gotError, gotFinal)
+        await super.teardownRuntime(options)
         this.storeUserCodeInPython('__USER_CODE__', "")
-        this.focusEditor()
     }
 
 
 
-    prefillTermIfAllowed() {
-        // do nothing, but forbid the action on the parent class, which would raise an error
-        // because prefillTerm is undefined, for IDEs.
-    }
+    /**Does nothing, but catch any call on the parent class, which would raise an error
+     * because prefillTerm is undefined, for IDEs.
+     * */
+    prefillTermIfAllowed() {}
 
 
 
     //--------------------------------------------------------------------
 
 
 
 
     playFactory() {
         return withPyodideAsyncLock('play', async (e) => {
             jsLogger("[Play]")
             if (e && e.preventDefault) e.preventDefault()
             this.resizeVerticalTerm() // needed in case the first click is on a button
 
-            let {
-                options,
-                stdErr,
-                _
-            } = await this.setupRuntime()
-            if (stdErr) return;
+            const options = await this.setupRuntime()
             try {
-                stdErr = await this.runPythonCodeWithOptions(this.editorCode, options)
+                await this.runPythonCodeWithOptionsIfNoStdErr(this.editorCode, options)
             } finally {
-                await this.teardownRuntime(options, stdErr, false)
+                await this.teardownRuntime(options)
             }
         })
     }
 
 
 
 
@@ -469,107 +441,100 @@
 
 
 
     validateFactory(e) {
         return withPyodideAsyncLock('Validate', async (e) => {
             jsLogger("[Validate]")
             if (e && e.preventDefault) e.preventDefault()
-            this.resizeVerticalTerm() // needed in case the first click is on a button
 
+            this.resizeVerticalTerm() // needed in case the first click is on a button
 
-            let {
-                options,
-                stdErr,
-                isAssertErr
-            } = await this.setupRuntime()
+            const options = await this.setupRuntime()
             let decrease_count = CONFIG.decreaseAttemptsOnUserCodeFailure
-            let gotFinal = false
+
 
             // If an error, stop everything...
-            if (stdErr) {
+            if (options.stdErr) {
                 // ... but decrease the number attempts and run teardown if this was AssertionError.
-                if (isAssertErr) {
-                    gotFinal = this.handleRunOutcome(false, decrease_count)
-                    this.teardownRuntime(options, stdErr, gotFinal)
+                if (options.isAssertErr) {
+                    this.handleRunOutcome(options, decrease_count)
                 }
+                this.teardownRuntime(options)
                 return // jail break...  x)
             }
 
+
             try {
                 // Define the user's code in the environment and run the public tests (if any)
-                stdErr = stdErr || await this.runPythonCodeWithOptions(this.editorCode, options)
-                decrease_count &&= !!stdErr
+                await this.runPythonCodeWithOptionsIfNoStdErr(this.editorCode, options)
+                decrease_count &&= Boolean(options.stdErr)
 
                 // Run the validation tests only if the user's code succeeded at the previous step
-                if (!stdErr) {
-                    /*
-                    Quit if no secret tests, ignoring any public tests.
-                    This is so that the behavior for Ctrl+Enter is compliant with the GUI: the
-                    validation button is present only if secret tests are present.
-                    */
-                    if (!this.secretTests) return // NOTE: should never happen anymore...
-
+                if (!options.stdErr) {
                     // If still running, run the original public tests and the secret ones...
                     const fullTests = `${ this.publicTests }\n\n${ this.secretTests }`.trim()
                     options.withStdOut = !CONFIG.deactivateStdoutForSecrets
                     options.isPublic = !CONFIG.showOnlyAssertionErrorsForSecrets
                     options.autoLogAssert = this.autoLogAssert !== null ? this.autoLogAssert :
                         CONFIG.showAssertionCodeOnFailedTest
 
-                    decrease_count = stdErr = await this.runPythonCodeWithOptions(fullTests, options)
+                    await this.runPythonCodeWithOptionsIfNoStdErr(fullTests, options)
+                    decrease_count = options.stdErr
                 }
 
                 /* Reveal solution and REMs on success, or if the counter reached 0 and the sol&REMs
                   content is still encrypted.
                   Prepare an appropriate revelation message if needed (`finalMsg`).
                 */
-
-                gotFinal = this.handleRunOutcome(!stdErr, decrease_count)
+                this.handleRunOutcome(options, decrease_count)
 
             } catch (e) {
                 // If something didn't get caught, it's very wrong... so dump everything to the console
-                // NOTE: nothing is thrown anymore, because everything is started async, now ! x/
                 this.terminal.echo(youAreInTroubles(e))
+                throw e
 
             } finally {
-                await this.teardownRuntime(options, stdErr, gotFinal)
+                await this.teardownRuntime(options)
             }
         })
     }
 
 
 
 
-    /**
+    /**Do not forget that all error feedback is already printed to the console. So when it comes to
+     * feedback, this method is only there to spot any final message needed.
+     *
      * @returns true if a final message is given (means, no "finished without error")
      * */
-    handleRunOutcome(success, allowCountDecrease) {
+    handleRunOutcome(options, allowCountDecrease) {
+        const success = !options.stdErr
 
         if (!success && allowCountDecrease) {
             this.decreaseIdeCounter()
         }
-        if (this.revealSolutionAndRemsIfNeeded(success)) {
-            const finalMsg = success ? this._buildSuccessMessage() :
-                this._getSolRemTxt(false)
-            if (finalMsg) {
-                this.giveFeedback(finalMsg)
-                return true
-            }
+
+        if (!this.corrRemsMask) {
+            if (success) options.finalMsg = this._buildSuccessMessage()
+
+        } else if (this.hiddenDivContent && (success || this.attemptsLeft == 0)) {
+            this.revealSolutionAndRemsIfNeeded()
+            options.finalMsg = success ? this._buildSuccessMessage() : this._getSolRemTxt(false)
+            this.hiddenDivContent = false // Forbid coming back here
         }
-        return false
     }
 
 
     /**Decrease the number of tries left, unless:
      *    - The solution is already revealed
      *    - The number of tries is infinite
      *    - There no attempts left (redundant with revelation condition, but hey...)
      */
     decreaseIdeCounter() {
-        if (!this.corrHidden) return // already revealed => nothing to change.
+        if (!this.hiddenDivContent) return // already revealed => nothing to change.
 
         // Allow going below 0 so that triggers once only for failure.
         const nAttempts = Math.max(-1, this.attemptsLeft - 1)
         this.data.attempts_left = nAttempts
 
         // Update the GUI counter if needed (check for encryption in case
         // the user already solved the problem)
@@ -585,26 +550,20 @@
      * Revelation occurs if:
      *    - Sol&REMs are still hidden,
      *    - Some Sol&REMs actually exist,
      *    - The run is successful or all attempts have been consumed.
      *
      * @returns: boolean, telling if the revelation occurred or not.
      */
-    revealSolutionAndRemsIfNeeded(success) {
-        const someToReveal = this.corrHidden && this.corrRemsMask && (success || this.attemptsLeft == 0)
-        if (someToReveal) {
-            const sol_div = $("#solution_" + this.id)
-            const compressed = sol_div.text()
-            const content = decompressLZW(compressed)
-            sol_div.html(content).attr('class', '') // update + unhide
-            mathJaxUpdate() // Enforce formatting, if ever...
-            this.corrHidden = false // Forbid coming back here
-            return true
-        }
-        return false
+    revealSolutionAndRemsIfNeeded() {
+        const sol_div = $("#solution_" + this.id)
+        const compressed = sol_div.text()
+        const content = decompressLZW(compressed)
+        sol_div.html(content).attr('class', '') // update + unhide
+        mathJaxUpdate() // Enforce formatting, if ever...
     }
 
 
     _buildSuccessMessage() {
         const emo = choice(CONFIG.MSG.successEmojis)
         let info = this._getSolRemTxt(true)
         return `${ success(CONFIG.lang.successHead.msg) } ${ emo } ${ CONFIG.lang.successHeadExtra.msg }${ info }`
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-per-pages/qcms-qcm.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-per-pages/start-pyodide.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -81,15 +81,15 @@
  * */
 function setupPyodideEnvironmentTools() {
 
     const routines = "pyconsole, await_fut, clear_console"
 
     // Indentation does matter a bit: 1 extra indent is ok, but 2 fails (whatever... :rolleyes: )
     const pythonRoutinesExtractionCode = `
-    def _hack():
+    def _hack_2():
         import js
         import __main__
         from pyodide.console import PyodideConsole, repr_shorten
 
         pyconsole = PyodideConsole(__main__.__dict__)
 
         async def await_fut(fut):
@@ -104,16 +104,16 @@
             print(res, end='')
 
         def clear_console():            # Useless...?
             pyconsole.buffer = []
 
         return ${ routines }
 
-    ${ routines } = _hack()
-    del _hack`
+    ${ routines } = _hack_2()
+    del _hack_2`
 
     const namespace = pyodide.globals.get("dict")();
     pyodide.runPython(pythonRoutinesExtractionCode, {
         globals: namespace
     });
 
     const outRoutines = {}
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-scripts/error-logs-generator-scripts.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -130,19 +130,19 @@
     negative lookahead CANNOT start just after the number or the await_fut thing is matched
     when the line number has more than 1 digit..., so must use another strategy).
     */
     const iModule = errLines.findIndex(s => CONFIG.MODULE_REG.test(s))
 
     /*
     Python errors may sometimes be coming from side effects of restrictions: those may not come
-    from the execution of the user's code and the stacktrace, may then not content the desired
+    from the execution of the user's code and then, the stacktrace may not contain the desired
     pattern, aka, the "file" may be neither exec nor console. (this happens for example with a
     recursion limit set too low: the error is raised when extracting stdout only).
     */
-    const isFromUserCode = iModule > 0
+    // const isFromUserCode = iModule > 0
 
     const [iError, isAssertErr] = getErrorKindInfos(errLines)
 
     // If ExclusionError, just throw the last line without anything else:
     if (errLines[iError].includes(CONFIG.MSG.exclusionMarker)) {
         const msg = errLines.slice(iError).join('\n')
         const i = msg.indexOf(CONFIG.MSG.exclusionMarker)
@@ -166,22 +166,24 @@
         errLines.splice(iError, errLines.length)
         errLines.push(`${errKind} has been raised.`)
     }
 
     // Shorten the error code section (if multiline assertion message), and then the stacktrace.
     shortenArrSection('err', errLines, iError, errLines.length - 1, iModule, purgeErr)
 
+    // Remove pyodide related information from the stacktrace (the user doesn't need to know)
+    shortenArrSection('trace', errLines, iModule, iError - 1, iModule, purgeErr)
+
     // Remove pyodide related information from the stacktrace (the user doesn't need to know) if
     // it's the user's code that is run, otherwise, keep the full stack trace to ease debugging:
-    if (isFromUserCode) {
-        shortenArrSection('trace', errLines, iModule, iError - 1, iModule, purgeErr)
-
-    } else {
-        errLines.push(CONFIG.MSG.bigFail)
-    }
+    // if(isFromUserCode){
+    //   shortenArrSection('trace', errLines, iModule, iError-1, iModule, purgeErr)
+    // }else{
+    //   errLines.push(CONFIG.MSG.bigFail)
+    // }
     return [errLines.join('\n'), isAssertErr]
 }
 
 
 
 /**Mutate the content of the given array, if the section identified by the original `from` and
  * `to` indices is considered too long.
@@ -269,26 +271,27 @@
     }
 
     // The double quotes are all escaped to make sure no multiline string will cause troubles
     const escapedCode = code.replace(/"/g, '\\"')
     const lineNo = +numMatch[1]
     const astExplorer = `
 
-def _hack___________():
+def _hack_1():
     import ast
     code = """${ escapedCode }"""
     tree = ast.parse(code)
     assertNode = next( node for node in ast.walk(tree)
-                            if isinstance(node, ast.Assert) and node.lineno==${ lineNo } )
+                            if isinstance(node, ast.Assert)
+                               and node.lineno <= ${ lineNo } <= node.end_lineno )
 
     i,j = assertNode.lineno-1, assertNode.end_lineno
     return '\\n'.join(code.splitlines()[i:j])
 
-_ = _hack___________()
-del _hack___________
+_ = _hack_1()
+del _hack_1
 _`
     let assertion
     try {
         assertion = pyodide.runPython(astExplorer)
     } catch (e) {
         // Any error here must be caught and returned, otherwise it will just
         // be swallowed (somehow...)
```

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/js-scripts/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/main.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/pyodide-css/0_generic-tooltips-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/pyodide-css/header-btns-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/pyodide-css/hourglass-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/pyodide-css/ide-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/pyodide-css/qcm-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css` & `pyodide_mkdocs_theme-1.1.0/pyodide_mkdocs_theme/templates/pyodide-css/terminal-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-1.0.4/pyproject.toml` & `pyodide_mkdocs_theme-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "1.0.4"
+version = "1.1.0"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
```

### Comparing `pyodide_mkdocs_theme-1.0.4/PKG-INFO` & `pyodide_mkdocs_theme-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 1.0.4
+Version: 1.1.0
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

