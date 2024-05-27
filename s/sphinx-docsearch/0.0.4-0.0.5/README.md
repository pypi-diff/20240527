# Comparing `tmp/sphinx_docsearch-0.0.4.tar.gz` & `tmp/sphinx_docsearch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_docsearch-0.0.4.tar", max compression
+gzip compressed data, was "sphinx_docsearch-0.0.5.tar", max compression
```

## Comparing `sphinx_docsearch-0.0.4.tar` & `sphinx_docsearch-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2023-11-30 15:01:43.357858 sphinx_docsearch-0.0.4/LICENSE
--rw-r--r--   0        0        0     1579 2023-11-30 15:01:43.357858 sphinx_docsearch-0.0.4/README.md
--rw-r--r--   0        0        0     1766 2023-11-30 15:01:43.361858 sphinx_docsearch-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4533 2023-11-30 15:01:43.361858 sphinx_docsearch-0.0.4/src/sphinx_docsearch/__init__.py
--rw-r--r--   0        0        0        0 2023-11-30 15:01:43.361858 sphinx_docsearch-0.0.4/src/sphinx_docsearch/py.typed
--rw-r--r--   0        0        0      130 2023-11-30 15:01:43.361858 sphinx_docsearch-0.0.4/src/sphinx_docsearch/static/alabaster-docsearch-custom.css
--rw-r--r--   0        0        0    13261 2023-11-30 15:01:43.361858 sphinx_docsearch-0.0.4/src/sphinx_docsearch/static/docsearch.css
--rw-r--r--   0        0        0   127224 2023-11-30 15:01:43.361858 sphinx_docsearch-0.0.4/src/sphinx_docsearch/static/docsearch.js
--rw-r--r--   0        0        0      648 2023-11-30 15:01:43.361858 sphinx_docsearch-0.0.4/src/sphinx_docsearch/static/docsearch_config.js_t
--rw-r--r--   0        0        0     1782 2023-11-30 15:01:43.361858 sphinx_docsearch-0.0.4/src/sphinx_docsearch/static/furo-docsearch-custom.css
--rw-r--r--   0        0        0      167 2023-11-30 15:01:43.361858 sphinx_docsearch-0.0.4/src/sphinx_docsearch/static/rtd-docsearch-custom.css
--rw-r--r--   0        0        0      117 2023-11-30 15:01:43.361858 sphinx_docsearch-0.0.4/src/sphinx_docsearch/templates/searchbox.html
--rw-r--r--   0        0        0      117 2023-11-30 15:01:43.361858 sphinx_docsearch-0.0.4/src/sphinx_docsearch/templates/sidebar/search.html
--rw-r--r--   0        0        0     2613 1970-01-01 00:00:00.000000 sphinx_docsearch-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-27 15:09:03.022004 sphinx_docsearch-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1528 2024-05-27 15:09:03.022004 sphinx_docsearch-0.0.5/README.md
+-rw-r--r--   0        0        0     1860 2024-05-27 15:09:03.022004 sphinx_docsearch-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4628 2024-05-27 15:09:03.022004 sphinx_docsearch-0.0.5/src/sphinx_docsearch/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:09:03.022004 sphinx_docsearch-0.0.5/src/sphinx_docsearch/py.typed
+-rw-r--r--   0        0        0      130 2024-05-27 15:09:03.022004 sphinx_docsearch-0.0.5/src/sphinx_docsearch/static/alabaster-docsearch-custom.css
+-rw-r--r--   0        0        0    13762 2024-05-27 15:09:03.022004 sphinx_docsearch-0.0.5/src/sphinx_docsearch/static/docsearch.css
+-rw-r--r--   0        0        0   127820 2024-05-27 15:09:03.022004 sphinx_docsearch-0.0.5/src/sphinx_docsearch/static/docsearch.js
+-rw-r--r--   0        0        0      648 2024-05-27 15:09:03.022004 sphinx_docsearch-0.0.5/src/sphinx_docsearch/static/docsearch_config.js_t
+-rw-r--r--   0        0        0     1782 2024-05-27 15:09:03.022004 sphinx_docsearch-0.0.5/src/sphinx_docsearch/static/furo-docsearch-custom.css
+-rw-r--r--   0        0        0      167 2024-05-27 15:09:03.022004 sphinx_docsearch-0.0.5/src/sphinx_docsearch/static/rtd-docsearch-custom.css
+-rw-r--r--   0        0        0      117 2024-05-27 15:09:03.022004 sphinx_docsearch-0.0.5/src/sphinx_docsearch/templates/searchbox.html
+-rw-r--r--   0        0        0      117 2024-05-27 15:09:03.026003 sphinx_docsearch-0.0.5/src/sphinx_docsearch/templates/sidebar/search.html
+-rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 sphinx_docsearch-0.0.5/PKG-INFO
```

### Comparing `sphinx_docsearch-0.0.4/LICENSE` & `sphinx_docsearch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.4/README.md` & `sphinx_docsearch-0.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 replaces Sphinx's built-in search with Algolia DocSearch.
 
 ## Before you begin
 
 [**Apply for DocSearch**](https://docsearch.algolia.com/apply).
 You'll get an email with your Algolia credentials.
 
-This extension supports Python versions 3.8, 3.9, 3.10, and 3.11 and Sphinx versions 5 and later.
+This extension supports Python versions 3.8 and later and Sphinx versions 5 and later.
 
 ## Install
 
 Install the `sphinx-docsearch` package:
 
 ```sh
 pip install sphinx-docsearch
@@ -32,18 +32,18 @@
    ```python
    # conf.py
    docsearch_app_id = "<DOCSEARCH_APP_ID>"
    docsearch_api_key = "<DOCSEARCH_SEARCH_API_KEY>"
    docsearch_index_name = "<DOCSEARCH_INDEX_NAME>"
    ```
 
-   See also: [Configure DocSearch](https://sphinx-docsearch.readthedocs.io/en/latest/configuration.html).
+   See also: [Configure DocSearch](https://sphinx-docsearch.readthedocs.io/configuration.html).
 
 ## Customize
 
 To change what the crawler should extract from your pages, see [Record Extractor](https://docsearch.algolia.com/docs/record-extractor).
 
-You can add [custom templates](https://sphinx-docsearch.readthedocs.io/en/latest/customization.html#add-custom-templates),
-if your Sphinx HTML theme uses templates [not provided](https://sphinx-docsearch.readthedocs.io/en/latest/themes.html)
+You can add [custom templates](https://sphinx-docsearch.readthedocs.io/customization.html#add-custom-templates),
+if your Sphinx HTML theme uses templates [not provided](https://sphinx-docsearch.readthedocs.io/themes.html)
 by this extension.
 
-You can customize the look of the DocSearch UI by [adding your own CSS](https://sphinx-docsearch.readthedocs.io/en/latest/customization.html#add-custom-css).
+You can customize the look of the DocSearch UI by [adding your own CSS](https://sphinx-docsearch.readthedocs.io/customization.html#add-custom-css).
```

### Comparing `sphinx_docsearch-0.0.4/pyproject.toml` & `sphinx_docsearch-0.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "sphinx-docsearch"
-version = "0.0.4"
+version = "0.0.5"
 description = "A Sphinx extension for replacing the built-in search with Algolia DocSearch"
-authors = ["Algolia"]
+authors = ["Algolia <support@algolia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   {include = "sphinx_docsearch", from = "src"}
 ]
 classifiers = [
   'Programming Language :: Python',
@@ -17,63 +17,64 @@
   'Topic :: Software Development :: Documentation'
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 sphinx = [
   { version = "<7.2", python = ">=3.8,<3.9"},
-  { version = "^7.2,<7.3", python = ">=3.9,<=3.12"},
+  { version = "^7.2,<7.4", python = ">=3.9,<3.13"},
 ]
 
 [tool.poetry.group.lint.dependencies]
 ruff = "*"
-black = "*"
 
 [tool.poetry.group.docs.dependencies]
-sphinx-autobuild = "^2021.3.14"
+sphinx-autobuild = [
+  { version = "^2021.3.14", python = ">=3.8,<3.9" },
+  { version = "^2024.2.4", python = ">=3.9, <3.13"},
+]
 python-dotenv = "^1.0.0"
-furo = "^2023.5.20"
+furo = "^2024.1.29"
 myst-parser = "^2.0.0"
 sphinx_rtd_theme = "^2.0.0"
+sphinxawesome-theme = "^5.1"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.3.1"
+pytest = "^8"
 beautifulsoup4 = "^4.12.2"
-pytest-cov = "^4.0.0"
+pytest-cov = ">=4,<6"
 mypy = "^1.2.0"
 types-beautifulsoup4 = "^4.12.0.4"
-nox = "^2023.4.22"
-httpx = "^0.24.1"
+nox = "^2024.4.15"
+httpx = "^0.27.0"
+defusedxml = "^0.7"
 
 [tool.coverage.path]
 source = ["src"]
 
 [tool.coverage.run]
 branch = true
 source = ["sphinx_docsearch"]
 
 [tool.coverage.report]
 show_missing = true
-fail_under = 98
 
 [tool.mypy]
 show_error_codes = true
 show_error_context = true
 pretty = true
 strict = true
 show_column_numbers = true
 warn_unreachable = true
 warn_unused_ignores = true
 
-[tool.ruff]
+[tool.ruff.lint]
 select = ["E", "F", "B", "Q", "W", "I", "C90", "D", "UP", "YTT", "S", "ANN", "SIM", "N"]
 # Ignore conflicting rules
 ignore = ["D203", "D213", "E501"]
-target-version = "py38"
-extend-exclude = ["*.pyi"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = ["S101"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sphinx_docsearch-0.0.4/src/sphinx_docsearch/__init__.py` & `sphinx_docsearch-0.0.5/src/sphinx_docsearch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 """Add Algolia DocSearch to Sphinx.
 
 Replace Sphinx built-in search with Algolia DocSearch.
 
 :copyright: Kai Welke.
 :license: MIT, see LICENSE for details
 """
+
 from __future__ import annotations
 
 from importlib.metadata import PackageNotFoundError, version
 from pathlib import Path
 from typing import Any
 
 from sphinx.application import Config, Sphinx
 from sphinx.builders.dirhtml import DirectoryHTMLBuilder
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.locale import __
 from sphinx.util import logging
-from sphinx.util.display import progress_message
+
+try:
+    from sphinx.util.display import progress_message
+except ImportError:
+    # Sphinx < 7.0
+    from sphinx.util import progress_message
 
 logger = logging.getLogger(__name__)
 
 try:
     __version__ = version(__name__.replace(".", "-"))
 except PackageNotFoundError:  # pragma: nocover
     __version__ = "unknown"
```

### Comparing `sphinx_docsearch-0.0.4/src/sphinx_docsearch/static/docsearch.css` & `sphinx_docsearch-0.0.5/src/sphinx_docsearch/static/docsearch.css`

 * *Files 7% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-/*! @docsearch/css 3.5.2 | MIT License | © Algolia, Inc. and contributors | https://docsearch.algolia.com */
-:root{--docsearch-primary-color:#5468ff;--docsearch-text-color:#1c1e21;--docsearch-spacing:12px;--docsearch-icon-stroke-width:1.4;--docsearch-highlight-color:var(--docsearch-primary-color);--docsearch-muted-color:#969faf;--docsearch-container-background:rgba(101,108,133,0.8);--docsearch-logo-color:#5468ff;--docsearch-modal-width:560px;--docsearch-modal-height:600px;--docsearch-modal-background:#f5f6f7;--docsearch-modal-shadow:inset 1px 1px 0 0 hsla(0,0%,100%,0.5),0 3px 8px 0 #555a64;--docsearch-searchbox-height:56px;--docsearch-searchbox-background:#ebedf0;--docsearch-searchbox-focus-background:#fff;--docsearch-searchbox-shadow:inset 0 0 0 2px var(--docsearch-primary-color);--docsearch-hit-height:56px;--docsearch-hit-color:#444950;--docsearch-hit-active-color:#fff;--docsearch-hit-background:#fff;--docsearch-hit-shadow:0 1px 3px 0 #d4d9e1;--docsearch-key-gradient:linear-gradient(-225deg,#d5dbe4,#f8f8f8);--docsearch-key-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,0.4);--docsearch-footer-height:44px;--docsearch-footer-background:#fff;--docsearch-footer-shadow:0 -1px 0 0 #e0e3e8,0 -3px 6px 0 rgba(69,98,155,0.12)}html[data-theme=dark]{--docsearch-text-color:#f5f6f7;--docsearch-container-background:rgba(9,10,17,0.8);--docsearch-modal-background:#15172a;--docsearch-modal-shadow:inset 1px 1px 0 0 #2c2e40,0 3px 8px 0 #000309;--docsearch-searchbox-background:#090a11;--docsearch-searchbox-focus-background:#000;--docsearch-hit-color:#bec3c9;--docsearch-hit-shadow:none;--docsearch-hit-background:#090a11;--docsearch-key-gradient:linear-gradient(-26.5deg,#565872,#31355b);--docsearch-key-shadow:inset 0 -2px 0 0 #282d55,inset 0 0 1px 1px #51577d,0 2px 2px 0 rgba(3,4,9,0.3);--docsearch-footer-background:#1e2136;--docsearch-footer-shadow:inset 0 1px 0 0 rgba(73,76,106,0.5),0 -4px 8px 0 rgba(0,0,0,0.2);--docsearch-logo-color:#fff;--docsearch-muted-color:#7f8497}.DocSearch-Button{align-items:center;background:var(--docsearch-searchbox-background);border:0;border-radius:40px;color:var(--docsearch-muted-color);cursor:pointer;display:flex;font-weight:500;height:36px;justify-content:space-between;margin:0 0 0 16px;padding:0 8px;user-select:none}.DocSearch-Button:active,.DocSearch-Button:focus,.DocSearch-Button:hover{background:var(--docsearch-searchbox-focus-background);box-shadow:var(--docsearch-searchbox-shadow);color:var(--docsearch-text-color);outline:none}.DocSearch-Button-Container{align-items:center;display:flex}.DocSearch-Search-Icon{stroke-width:1.6}.DocSearch-Button .DocSearch-Search-Icon{color:var(--docsearch-text-color)}.DocSearch-Button-Placeholder{font-size:1rem;padding:0 12px 0 6px}.DocSearch-Button-Keys{display:flex;min-width:calc(40px + .8em)}.DocSearch-Button-Key{align-items:center;background:var(--docsearch-key-gradient);border-radius:3px;box-shadow:var(--docsearch-key-shadow);color:var(--docsearch-muted-color);display:flex;height:18px;justify-content:center;margin-right:.4em;position:relative;padding:0 0 2px;border:0;top:-1px;width:20px}@media (max-width:768px){.DocSearch-Button-Keys,.DocSearch-Button-Placeholder{display:none}}.DocSearch--active{overflow:hidden!important}.DocSearch-Container,.DocSearch-Container *{box-sizing:border-box}.DocSearch-Container{background-color:var(--docsearch-container-background);height:100vh;left:0;position:fixed;top:0;width:100vw;z-index:200}.DocSearch-Container a{text-decoration:none}.DocSearch-Link{appearance:none;background:none;border:0;color:var(--docsearch-highlight-color);cursor:pointer;font:inherit;margin:0;padding:0}.DocSearch-Modal{background:var(--docsearch-modal-background);border-radius:6px;box-shadow:var(--docsearch-modal-shadow);flex-direction:column;margin:60px auto auto;max-width:var(--docsearch-modal-width);position:relative}.DocSearch-SearchBar{display:flex;padding:var(--docsearch-spacing) var(--docsearch-spacing) 0}.DocSearch-Form{align-items:center;background:var(--docsearch-searchbox-focus-background);border-radius:4px;box-shadow:var(--docsearch-searchbox-shadow);display:flex;height:var(--docsearch-searchbox-height);margin:0;padding:0 var(--docsearch-spacing);position:relative;width:100%}.DocSearch-Input{appearance:none;background:transparent;border:0;color:var(--docsearch-text-color);flex:1;font:inherit;font-size:1.2em;height:100%;outline:none;padding:0 0 0 8px;width:80%}.DocSearch-Input::placeholder{color:var(--docsearch-muted-color);opacity:1}.DocSearch-Input::-webkit-search-cancel-button,.DocSearch-Input::-webkit-search-decoration,.DocSearch-Input::-webkit-search-results-button,.DocSearch-Input::-webkit-search-results-decoration{display:none}.DocSearch-LoadingIndicator,.DocSearch-MagnifierLabel,.DocSearch-Reset{margin:0;padding:0}.DocSearch-MagnifierLabel,.DocSearch-Reset{align-items:center;color:var(--docsearch-highlight-color);display:flex;justify-content:center}.DocSearch-Container--Stalled .DocSearch-MagnifierLabel,.DocSearch-LoadingIndicator{display:none}.DocSearch-Container--Stalled .DocSearch-LoadingIndicator{align-items:center;color:var(--docsearch-highlight-color);display:flex;justify-content:center}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Reset{animation:none;appearance:none;background:none;border:0;border-radius:50%;color:var(--docsearch-icon-color);cursor:pointer;right:0;stroke-width:var(--docsearch-icon-stroke-width)}}.DocSearch-Reset{animation:fade-in .1s ease-in forwards;appearance:none;background:none;border:0;border-radius:50%;color:var(--docsearch-icon-color);cursor:pointer;padding:2px;right:0;stroke-width:var(--docsearch-icon-stroke-width)}.DocSearch-Reset[hidden]{display:none}.DocSearch-Reset:hover{color:var(--docsearch-highlight-color)}.DocSearch-LoadingIndicator svg,.DocSearch-MagnifierLabel svg{height:24px;width:24px}.DocSearch-Cancel{display:none}.DocSearch-Dropdown{max-height:calc(var(--docsearch-modal-height) - var(--docsearch-searchbox-height) - var(--docsearch-spacing) - var(--docsearch-footer-height));min-height:var(--docsearch-spacing);overflow-y:auto;overflow-y:overlay;padding:0 var(--docsearch-spacing);scrollbar-color:var(--docsearch-muted-color) var(--docsearch-modal-background);scrollbar-width:thin}.DocSearch-Dropdown::-webkit-scrollbar{width:12px}.DocSearch-Dropdown::-webkit-scrollbar-track{background:transparent}.DocSearch-Dropdown::-webkit-scrollbar-thumb{background-color:var(--docsearch-muted-color);border:3px solid var(--docsearch-modal-background);border-radius:20px}.DocSearch-Dropdown ul{list-style:none;margin:0;padding:0}.DocSearch-Label{font-size:.75em;line-height:1.6em}.DocSearch-Help,.DocSearch-Label{color:var(--docsearch-muted-color)}.DocSearch-Help{font-size:.9em;margin:0;user-select:none}.DocSearch-Title{font-size:1.2em}.DocSearch-Logo a{display:flex}.DocSearch-Logo svg{color:var(--docsearch-logo-color);margin-left:8px}.DocSearch-Hits:last-of-type{margin-bottom:24px}.DocSearch-Hits mark{background:none;color:var(--docsearch-highlight-color)}.DocSearch-HitsFooter{color:var(--docsearch-muted-color);display:flex;font-size:.85em;justify-content:center;margin-bottom:var(--docsearch-spacing);padding:var(--docsearch-spacing)}.DocSearch-HitsFooter a{border-bottom:1px solid;color:inherit}.DocSearch-Hit{border-radius:4px;display:flex;padding-bottom:4px;position:relative}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit--deleting{transition:none}}.DocSearch-Hit--deleting{opacity:0;transition:all .25s linear}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit--favoriting{transition:none}}.DocSearch-Hit--favoriting{transform:scale(0);transform-origin:top center;transition:all .25s linear;transition-delay:.25s}.DocSearch-Hit a{background:var(--docsearch-hit-background);border-radius:4px;box-shadow:var(--docsearch-hit-shadow);display:block;padding-left:var(--docsearch-spacing);width:100%}.DocSearch-Hit-source{background:var(--docsearch-modal-background);color:var(--docsearch-highlight-color);font-size:.85em;font-weight:600;line-height:32px;margin:0 -4px;padding:8px 4px 0;position:sticky;top:0;z-index:10}.DocSearch-Hit-Tree{color:var(--docsearch-muted-color);height:var(--docsearch-hit-height);opacity:.5;stroke-width:var(--docsearch-icon-stroke-width);width:24px}.DocSearch-Hit[aria-selected=true] a{background-color:var(--docsearch-highlight-color)}.DocSearch-Hit[aria-selected=true] mark{text-decoration:underline}.DocSearch-Hit-Container{align-items:center;color:var(--docsearch-hit-color);display:flex;flex-direction:row;height:var(--docsearch-hit-height);padding:0 var(--docsearch-spacing) 0 0}.DocSearch-Hit-icon{height:20px;width:20px}.DocSearch-Hit-action,.DocSearch-Hit-icon{color:var(--docsearch-muted-color);stroke-width:var(--docsearch-icon-stroke-width)}.DocSearch-Hit-action{align-items:center;display:flex;height:22px;width:22px}.DocSearch-Hit-action svg{display:block;height:18px;width:18px}.DocSearch-Hit-action+.DocSearch-Hit-action{margin-left:6px}.DocSearch-Hit-action-button{appearance:none;background:none;border:0;border-radius:50%;color:inherit;cursor:pointer;padding:2px}svg.DocSearch-Hit-Select-Icon{display:none}.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-Select-Icon{display:block}.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{background:rgba(0,0,0,.2);transition:background-color .1s ease-in}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{transition:none}}.DocSearch-Hit-action-button:focus path,.DocSearch-Hit-action-button:hover path{fill:#fff}.DocSearch-Hit-content-wrapper{display:flex;flex:1 1 auto;flex-direction:column;font-weight:500;justify-content:center;line-height:1.2em;margin:0 8px;overflow-x:hidden;position:relative;text-overflow:ellipsis;white-space:nowrap;width:80%}.DocSearch-Hit-title{font-size:.9em}.DocSearch-Hit-path{color:var(--docsearch-muted-color);font-size:.75em}.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-action,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-icon,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-path,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-text,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-title,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-Tree,.DocSearch-Hit[aria-selected=true] mark{color:var(--docsearch-hit-active-color)!important}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{background:rgba(0,0,0,.2);transition:none}}.DocSearch-ErrorScreen,.DocSearch-NoResults,.DocSearch-StartScreen{font-size:.9em;margin:0 auto;padding:36px 0;text-align:center;width:80%}.DocSearch-Screen-Icon{color:var(--docsearch-muted-color);padding-bottom:12px}.DocSearch-NoResults-Prefill-List{display:inline-block;padding-bottom:24px;text-align:left}.DocSearch-NoResults-Prefill-List ul{display:inline-block;padding:8px 0 0}.DocSearch-NoResults-Prefill-List li{list-style-position:inside;list-style-type:"» "}.DocSearch-Prefill{appearance:none;background:none;border:0;border-radius:1em;color:var(--docsearch-highlight-color);cursor:pointer;display:inline-block;font-size:1em;font-weight:700;padding:0}.DocSearch-Prefill:focus,.DocSearch-Prefill:hover{outline:none;text-decoration:underline}.DocSearch-Footer{align-items:center;background:var(--docsearch-footer-background);border-radius:0 0 8px 8px;box-shadow:var(--docsearch-footer-shadow);display:flex;flex-direction:row-reverse;flex-shrink:0;height:var(--docsearch-footer-height);justify-content:space-between;padding:0 var(--docsearch-spacing);position:relative;user-select:none;width:100%;z-index:300}.DocSearch-Commands{color:var(--docsearch-muted-color);display:flex;list-style:none;margin:0;padding:0}.DocSearch-Commands li{align-items:center;display:flex}.DocSearch-Commands li:not(:last-of-type){margin-right:.8em}.DocSearch-Commands-Key{align-items:center;background:var(--docsearch-key-gradient);border-radius:2px;box-shadow:var(--docsearch-key-shadow);display:flex;height:18px;justify-content:center;margin-right:.4em;padding:0 0 1px;color:var(--docsearch-muted-color);border:0;width:20px}@media (max-width:768px){:root{--docsearch-spacing:10px;--docsearch-footer-height:40px}.DocSearch-Dropdown{height:100%}.DocSearch-Container{height:100vh;height:-webkit-fill-available;height:calc(var(--docsearch-vh, 1vh)*100);position:absolute}.DocSearch-Footer{border-radius:0;bottom:0;position:absolute}.DocSearch-Hit-content-wrapper{display:flex;position:relative;width:80%}.DocSearch-Modal{border-radius:0;box-shadow:none;height:100vh;height:-webkit-fill-available;height:calc(var(--docsearch-vh, 1vh)*100);margin:0;max-width:100%;width:100%}.DocSearch-Dropdown{max-height:calc(var(--docsearch-vh, 1vh)*100 - var(--docsearch-searchbox-height) - var(--docsearch-spacing) - var(--docsearch-footer-height))}.DocSearch-Cancel{appearance:none;background:none;border:0;color:var(--docsearch-highlight-color);cursor:pointer;display:inline-block;flex:none;font:inherit;font-size:1em;font-weight:500;margin-left:var(--docsearch-spacing);outline:none;overflow:hidden;padding:0;user-select:none;white-space:nowrap}.DocSearch-Commands,.DocSearch-Hit-Tree{display:none}}@keyframes fade-in{0%{opacity:0}to{opacity:1}}
+/*! @docsearch/css 3.6.0 | MIT License | © Algolia, Inc. and contributors | https://docsearch.algolia.com */
+:root{--docsearch-primary-color:#5468ff;--docsearch-text-color:#1c1e21;--docsearch-spacing:12px;--docsearch-icon-stroke-width:1.4;--docsearch-highlight-color:var(--docsearch-primary-color);--docsearch-muted-color:#969faf;--docsearch-container-background:rgba(101,108,133,0.8);--docsearch-logo-color:#5468ff;--docsearch-modal-width:560px;--docsearch-modal-height:600px;--docsearch-modal-background:#f5f6f7;--docsearch-modal-shadow:inset 1px 1px 0 0 hsla(0,0%,100%,0.5),0 3px 8px 0 #555a64;--docsearch-searchbox-height:56px;--docsearch-searchbox-background:#ebedf0;--docsearch-searchbox-focus-background:#fff;--docsearch-searchbox-shadow:inset 0 0 0 2px var(--docsearch-primary-color);--docsearch-hit-height:56px;--docsearch-hit-color:#444950;--docsearch-hit-active-color:#fff;--docsearch-hit-background:#fff;--docsearch-hit-shadow:0 1px 3px 0 #d4d9e1;--docsearch-key-gradient:linear-gradient(-225deg,#d5dbe4,#f8f8f8);--docsearch-key-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,0.4);--docsearch-key-pressed-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 1px 0 rgba(30,35,90,0.4);--docsearch-footer-height:44px;--docsearch-footer-background:#fff;--docsearch-footer-shadow:0 -1px 0 0 #e0e3e8,0 -3px 6px 0 rgba(69,98,155,0.12)}html[data-theme=dark]{--docsearch-text-color:#f5f6f7;--docsearch-container-background:rgba(9,10,17,0.8);--docsearch-modal-background:#15172a;--docsearch-modal-shadow:inset 1px 1px 0 0 #2c2e40,0 3px 8px 0 #000309;--docsearch-searchbox-background:#090a11;--docsearch-searchbox-focus-background:#000;--docsearch-hit-color:#bec3c9;--docsearch-hit-shadow:none;--docsearch-hit-background:#090a11;--docsearch-key-gradient:linear-gradient(-26.5deg,#565872,#31355b);--docsearch-key-shadow:inset 0 -2px 0 0 #282d55,inset 0 0 1px 1px #51577d,0 2px 2px 0 rgba(3,4,9,0.3);--docsearch-key-pressed-shadow:inset 0 -2px 0 0 #282d55,inset 0 0 1px 1px #51577d,0 1px 1px 0 rgba(3,4,9,0.30196078431372547);--docsearch-footer-background:#1e2136;--docsearch-footer-shadow:inset 0 1px 0 0 rgba(73,76,106,0.5),0 -4px 8px 0 rgba(0,0,0,0.2);--docsearch-logo-color:#fff;--docsearch-muted-color:#7f8497}.DocSearch-Button{align-items:center;background:var(--docsearch-searchbox-background);border:0;border-radius:40px;color:var(--docsearch-muted-color);cursor:pointer;display:flex;font-weight:500;height:36px;justify-content:space-between;margin:0 0 0 16px;padding:0 8px;user-select:none}.DocSearch-Button:active,.DocSearch-Button:focus,.DocSearch-Button:hover{background:var(--docsearch-searchbox-focus-background);box-shadow:var(--docsearch-searchbox-shadow);color:var(--docsearch-text-color);outline:none}.DocSearch-Button-Container{align-items:center;display:flex}.DocSearch-Search-Icon{stroke-width:1.6}.DocSearch-Button .DocSearch-Search-Icon{color:var(--docsearch-text-color)}.DocSearch-Button-Placeholder{font-size:1rem;padding:0 12px 0 6px}.DocSearch-Button-Keys{display:flex;min-width:calc(40px + .8em)}.DocSearch-Button-Key{align-items:center;background:var(--docsearch-key-gradient);border-radius:3px;box-shadow:var(--docsearch-key-shadow);color:var(--docsearch-muted-color);display:flex;height:18px;justify-content:center;margin-right:.4em;position:relative;padding:0 0 2px;border:0;top:-1px;width:20px}.DocSearch-Button-Key--pressed{transform:translate3d(0,1px,0);box-shadow:var(--docsearch-key-pressed-shadow)}@media (max-width:768px){.DocSearch-Button-Keys,.DocSearch-Button-Placeholder{display:none}}.DocSearch--active{overflow:hidden!important}.DocSearch-Container,.DocSearch-Container *{box-sizing:border-box}.DocSearch-Container{background-color:var(--docsearch-container-background);height:100vh;left:0;position:fixed;top:0;width:100vw;z-index:200}.DocSearch-Container a{text-decoration:none}.DocSearch-Link{appearance:none;background:none;border:0;color:var(--docsearch-highlight-color);cursor:pointer;font:inherit;margin:0;padding:0}.DocSearch-Modal{background:var(--docsearch-modal-background);border-radius:6px;box-shadow:var(--docsearch-modal-shadow);flex-direction:column;margin:60px auto auto;max-width:var(--docsearch-modal-width);position:relative}.DocSearch-SearchBar{display:flex;padding:var(--docsearch-spacing) var(--docsearch-spacing) 0}.DocSearch-Form{align-items:center;background:var(--docsearch-searchbox-focus-background);border-radius:4px;box-shadow:var(--docsearch-searchbox-shadow);display:flex;height:var(--docsearch-searchbox-height);margin:0;padding:0 var(--docsearch-spacing);position:relative;width:100%}.DocSearch-Input{appearance:none;background:transparent;border:0;color:var(--docsearch-text-color);flex:1;font:inherit;font-size:1.2em;height:100%;outline:none;padding:0 0 0 8px;width:80%}.DocSearch-Input::placeholder{color:var(--docsearch-muted-color);opacity:1}.DocSearch-Input::-webkit-search-cancel-button,.DocSearch-Input::-webkit-search-decoration,.DocSearch-Input::-webkit-search-results-button,.DocSearch-Input::-webkit-search-results-decoration{display:none}.DocSearch-LoadingIndicator,.DocSearch-MagnifierLabel,.DocSearch-Reset{margin:0;padding:0}.DocSearch-MagnifierLabel,.DocSearch-Reset{align-items:center;color:var(--docsearch-highlight-color);display:flex;justify-content:center}.DocSearch-Container--Stalled .DocSearch-MagnifierLabel,.DocSearch-LoadingIndicator{display:none}.DocSearch-Container--Stalled .DocSearch-LoadingIndicator{align-items:center;color:var(--docsearch-highlight-color);display:flex;justify-content:center}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Reset{animation:none;appearance:none;background:none;border:0;border-radius:50%;color:var(--docsearch-icon-color);cursor:pointer;right:0;stroke-width:var(--docsearch-icon-stroke-width)}}.DocSearch-Reset{animation:fade-in .1s ease-in forwards;appearance:none;background:none;border:0;border-radius:50%;color:var(--docsearch-icon-color);cursor:pointer;padding:2px;right:0;stroke-width:var(--docsearch-icon-stroke-width)}.DocSearch-Reset[hidden]{display:none}.DocSearch-Reset:hover{color:var(--docsearch-highlight-color)}.DocSearch-LoadingIndicator svg,.DocSearch-MagnifierLabel svg{height:24px;width:24px}.DocSearch-Cancel{display:none}.DocSearch-Dropdown{max-height:calc(var(--docsearch-modal-height) - var(--docsearch-searchbox-height) - var(--docsearch-spacing) - var(--docsearch-footer-height));min-height:var(--docsearch-spacing);overflow-y:auto;overflow-y:overlay;padding:0 var(--docsearch-spacing);scrollbar-color:var(--docsearch-muted-color) var(--docsearch-modal-background);scrollbar-width:thin}.DocSearch-Dropdown::-webkit-scrollbar{width:12px}.DocSearch-Dropdown::-webkit-scrollbar-track{background:transparent}.DocSearch-Dropdown::-webkit-scrollbar-thumb{background-color:var(--docsearch-muted-color);border:3px solid var(--docsearch-modal-background);border-radius:20px}.DocSearch-Dropdown ul{list-style:none;margin:0;padding:0}.DocSearch-Label{font-size:.75em;line-height:1.6em}.DocSearch-Help,.DocSearch-Label{color:var(--docsearch-muted-color)}.DocSearch-Help{font-size:.9em;margin:0;user-select:none}.DocSearch-Title{font-size:1.2em}.DocSearch-Logo a{display:flex}.DocSearch-Logo svg{color:var(--docsearch-logo-color);margin-left:8px}.DocSearch-Hits:last-of-type{margin-bottom:24px}.DocSearch-Hits mark{background:none;color:var(--docsearch-highlight-color)}.DocSearch-HitsFooter{color:var(--docsearch-muted-color);display:flex;font-size:.85em;justify-content:center;margin-bottom:var(--docsearch-spacing);padding:var(--docsearch-spacing)}.DocSearch-HitsFooter a{border-bottom:1px solid;color:inherit}.DocSearch-Hit{border-radius:4px;display:flex;padding-bottom:4px;position:relative}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit--deleting{transition:none}}.DocSearch-Hit--deleting{opacity:0;transition:all .25s linear}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit--favoriting{transition:none}}.DocSearch-Hit--favoriting{transform:scale(0);transform-origin:top center;transition:all .25s linear;transition-delay:.25s}.DocSearch-Hit a{background:var(--docsearch-hit-background);border-radius:4px;box-shadow:var(--docsearch-hit-shadow);display:block;padding-left:var(--docsearch-spacing);width:100%}.DocSearch-Hit-source{background:var(--docsearch-modal-background);color:var(--docsearch-highlight-color);font-size:.85em;font-weight:600;line-height:32px;margin:0 -4px;padding:8px 4px 0;position:sticky;top:0;z-index:10}.DocSearch-Hit-Tree{color:var(--docsearch-muted-color);height:var(--docsearch-hit-height);opacity:.5;stroke-width:var(--docsearch-icon-stroke-width);width:24px}.DocSearch-Hit[aria-selected=true] a{background-color:var(--docsearch-highlight-color)}.DocSearch-Hit[aria-selected=true] mark{text-decoration:underline}.DocSearch-Hit-Container{align-items:center;color:var(--docsearch-hit-color);display:flex;flex-direction:row;height:var(--docsearch-hit-height);padding:0 var(--docsearch-spacing) 0 0}.DocSearch-Hit-icon{height:20px;width:20px}.DocSearch-Hit-action,.DocSearch-Hit-icon{color:var(--docsearch-muted-color);stroke-width:var(--docsearch-icon-stroke-width)}.DocSearch-Hit-action{align-items:center;display:flex;height:22px;width:22px}.DocSearch-Hit-action svg{display:block;height:18px;width:18px}.DocSearch-Hit-action+.DocSearch-Hit-action{margin-left:6px}.DocSearch-Hit-action-button{appearance:none;background:none;border:0;border-radius:50%;color:inherit;cursor:pointer;padding:2px}svg.DocSearch-Hit-Select-Icon{display:none}.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-Select-Icon{display:block}.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{background:rgba(0,0,0,.2);transition:background-color .1s ease-in}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{transition:none}}.DocSearch-Hit-action-button:focus path,.DocSearch-Hit-action-button:hover path{fill:#fff}.DocSearch-Hit-content-wrapper{display:flex;flex:1 1 auto;flex-direction:column;font-weight:500;justify-content:center;line-height:1.2em;margin:0 8px;overflow-x:hidden;position:relative;text-overflow:ellipsis;white-space:nowrap;width:80%}.DocSearch-Hit-title{font-size:.9em}.DocSearch-Hit-path{color:var(--docsearch-muted-color);font-size:.75em}.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-action,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-icon,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-path,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-text,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-title,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-Tree,.DocSearch-Hit[aria-selected=true] mark{color:var(--docsearch-hit-active-color)!important}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{background:rgba(0,0,0,.2);transition:none}}.DocSearch-ErrorScreen,.DocSearch-NoResults,.DocSearch-StartScreen{font-size:.9em;margin:0 auto;padding:36px 0;text-align:center;width:80%}.DocSearch-Screen-Icon{color:var(--docsearch-muted-color);padding-bottom:12px}.DocSearch-NoResults-Prefill-List{display:inline-block;padding-bottom:24px;text-align:left}.DocSearch-NoResults-Prefill-List ul{display:inline-block;padding:8px 0 0}.DocSearch-NoResults-Prefill-List li{list-style-position:inside;list-style-type:"» "}.DocSearch-Prefill{appearance:none;background:none;border:0;border-radius:1em;color:var(--docsearch-highlight-color);cursor:pointer;display:inline-block;font-size:1em;font-weight:700;padding:0}.DocSearch-Prefill:focus,.DocSearch-Prefill:hover{outline:none;text-decoration:underline}.DocSearch-Footer{align-items:center;background:var(--docsearch-footer-background);border-radius:0 0 8px 8px;box-shadow:var(--docsearch-footer-shadow);display:flex;flex-direction:row-reverse;flex-shrink:0;height:var(--docsearch-footer-height);justify-content:space-between;padding:0 var(--docsearch-spacing);position:relative;user-select:none;width:100%;z-index:300}.DocSearch-Commands{color:var(--docsearch-muted-color);display:flex;list-style:none;margin:0;padding:0}.DocSearch-Commands li{align-items:center;display:flex}.DocSearch-Commands li:not(:last-of-type){margin-right:.8em}.DocSearch-Commands-Key{align-items:center;background:var(--docsearch-key-gradient);border-radius:2px;box-shadow:var(--docsearch-key-shadow);display:flex;height:18px;justify-content:center;margin-right:.4em;padding:0 0 1px;color:var(--docsearch-muted-color);border:0;width:20px}.DocSearch-VisuallyHiddenForAccessibility{clip:rect(0 0 0 0);clip-path:inset(50%);height:1px;overflow:hidden;position:absolute;white-space:nowrap;width:1px}@media (max-width:768px){:root{--docsearch-spacing:10px;--docsearch-footer-height:40px}.DocSearch-Dropdown{height:100%}.DocSearch-Container{height:100vh;height:-webkit-fill-available;height:calc(var(--docsearch-vh, 1vh)*100);position:absolute}.DocSearch-Footer{border-radius:0;bottom:0;position:absolute}.DocSearch-Hit-content-wrapper{display:flex;position:relative;width:80%}.DocSearch-Modal{border-radius:0;box-shadow:none;height:100vh;height:-webkit-fill-available;height:calc(var(--docsearch-vh, 1vh)*100);margin:0;max-width:100%;width:100%}.DocSearch-Dropdown{max-height:calc(var(--docsearch-vh, 1vh)*100 - var(--docsearch-searchbox-height) - var(--docsearch-spacing) - var(--docsearch-footer-height))}.DocSearch-Cancel{appearance:none;background:none;border:0;color:var(--docsearch-highlight-color);cursor:pointer;display:inline-block;flex:none;font:inherit;font-size:1em;font-weight:500;margin-left:var(--docsearch-spacing);outline:none;overflow:hidden;padding:0;user-select:none;white-space:nowrap}.DocSearch-Commands,.DocSearch-Hit-Tree{display:none}}@keyframes fade-in{0%{opacity:0}to{opacity:1}}
```

### Comparing `sphinx_docsearch-0.0.4/src/sphinx_docsearch/static/docsearch.js` & `sphinx_docsearch-0.0.5/src/sphinx_docsearch/static/docsearch.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! @docsearch/js 3.5.2 | MIT License | © Algolia, Inc. and contributors | https://docsearch.algolia.com */ ! function(e, t) {
+/*! @docsearch/js 3.6.0 | MIT License | © Algolia, Inc. and contributors | https://docsearch.algolia.com */ ! function(e, t) {
     "object" == typeof exports && "undefined" != typeof module ? module.exports = t() : "function" == typeof define && define.amd ? define(t) : (e = e || self).docsearch = t()
 }(this, (function() {
     "use strict";
 
     function e(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
@@ -162,23 +162,23 @@
         return null != s.vnode && s.vnode(i), i
     }
 
     function S(e) {
         return e.children
     }
 
-    function j(e, t) {
+    function w(e, t) {
         this.props = e, this.context = t
     }
 
-    function w(e, t) {
-        if (null == t) return e.__ ? w(e.__, e.__.__k.indexOf(e) + 1) : null;
+    function j(e, t) {
+        if (null == t) return e.__ ? j(e.__, e.__.__k.indexOf(e) + 1) : null;
         for (var n; t < e.__k.length; t++)
             if (null != (n = e.__k[t]) && null != n.__e) return n.__e;
-        return "function" == typeof e.type ? w(e) : null
+        return "function" == typeof e.type ? j(e) : null
     }
 
     function E(e) {
         var t, n;
         if (null != (e = e.__) && null != e.__c) {
             for (e.__e = e.__c.base = null, t = 0; t < e.__k.length; t++)
                 if (null != (n = e.__k[t]) && null != n.__e) {
@@ -193,15 +193,15 @@
     }
 
     function I() {
         for (var e; I.__r = f.length;) e = f.sort((function(e, t) {
             return e.__v.__b - t.__v.__b
         })), f = [], e.some((function(e) {
             var t, n, r, o, i, c;
-            e.__d && (i = (o = (t = e).__v).__e, (c = t.__P) && (n = [], (r = b({}, o)).__v = o.__v + 1, q(c, o, r, t.__n, void 0 !== c.ownerSVGElement, null != o.__h ? [i] : null, n, null == i ? w(o) : i, o.__h), L(n, o), o.__e != i && E(o)))
+            e.__d && (i = (o = (t = e).__v).__e, (c = t.__P) && (n = [], (r = b({}, o)).__v = o.__v + 1, q(c, o, r, t.__n, void 0 !== c.ownerSVGElement, null != o.__h ? [i] : null, n, null == i ? j(o) : i, o.__h), L(n, o), o.__e != i && E(o)))
         }))
     }
 
     function D(e, t, n, r, o, i, c, a, u, l) {
         var s, f, p, m, v, y, b, g = r && r.__k || h,
             _ = g.length;
         for (n.__k = [], s = 0; s < t.length; s++)
@@ -213,16 +213,16 @@
                     for (f = 0; f < _; f++) {
                         if ((p = g[f]) && m.key == p.key && m.type === p.type) {
                             g[f] = void 0;
                             break
                         }
                         p = null
                     }
-                q(e, m, p = p || d, o, i, c, a, u, l), v = m.__e, (f = m.ref) && p.ref != f && (b || (b = []), p.ref && b.push(p.ref, null, m), b.push(f, m.__c || v, m)), null != v ? (null == y && (y = v), "function" == typeof m.type && null != m.__k && m.__k === p.__k ? m.__d = u = k(m, u, e) : u = C(e, m, p, g, v, u), l || "option" !== n.type ? "function" == typeof n.type && (n.__d = u) : e.value = "") : u && p.__e == u && u.parentNode != e && (u = w(p))
-            } for (n.__e = y, s = _; s--;) null != g[s] && ("function" == typeof n.type && null != g[s].__e && g[s].__e == n.__d && (n.__d = w(r, s + 1)), U(g[s], g[s]));
+                q(e, m, p = p || d, o, i, c, a, u, l), v = m.__e, (f = m.ref) && p.ref != f && (b || (b = []), p.ref && b.push(p.ref, null, m), b.push(f, m.__c || v, m)), null != v ? (null == y && (y = v), "function" == typeof m.type && null != m.__k && m.__k === p.__k ? m.__d = u = k(m, u, e) : u = C(e, m, p, g, v, u), l || "option" !== n.type ? "function" == typeof n.type && (n.__d = u) : e.value = "") : u && p.__e == u && u.parentNode != e && (u = j(p))
+            } for (n.__e = y, s = _; s--;) null != g[s] && ("function" == typeof n.type && null != g[s].__e && g[s].__e == n.__d && (n.__d = j(r, s + 1)), U(g[s], g[s]));
         if (b)
             for (s = 0; s < b.length; s++) H(b[s], b[++s], b[++s])
     }
 
     function k(e, t, n) {
         var r, o;
         for (r = 0; r < e.__k.length; r++)(o = e.__k[r]) && (o.__ = e, t = "function" == typeof o.type ? k(o, t, n) : C(n, o, o, e.__k, o.__e, t));
@@ -277,22 +277,22 @@
     }
 
     function R(e) {
         this.l[e.type + !0](s.event ? s.event(e) : e)
     }
 
     function q(e, t, n, r, o, i, c, a, u) {
-        var l, f, p, m, v, d, h, y, g, _, O, w = t.type;
+        var l, f, p, m, v, d, h, y, g, _, O, j = t.type;
         if (void 0 !== t.constructor) return null;
         null != n.__h && (u = n.__h, a = t.__e = n.__e, t.__h = null, i = [a]), (l = s.__b) && l(t);
         try {
-            e: if ("function" == typeof w) {
-                if (y = t.props, g = (l = w.contextType) && r[l.__c], _ = l ? g ? g.props.value : l.__ : r, n.__c ? h = (f = t.__c = n.__c).__ = f.__E : ("prototype" in w && w.prototype.render ? t.__c = f = new w(y, _) : (t.__c = f = new j(y, _), f.constructor = w, f.render = F), g && g.sub(f), f.props = y, f.state || (f.state = {}), f.context = _, f.__n = r, p = f.__d = !0, f.__h = []), null == f.__s && (f.__s = f.state), null != w.getDerivedStateFromProps && (f.__s == f.state && (f.__s = b({}, f.__s)), b(f.__s, w.getDerivedStateFromProps(y, f.__s))), m = f.props, v = f.state, p) null == w.getDerivedStateFromProps && null != f.componentWillMount && f.componentWillMount(), null != f.componentDidMount && f.__h.push(f.componentDidMount);
+            e: if ("function" == typeof j) {
+                if (y = t.props, g = (l = j.contextType) && r[l.__c], _ = l ? g ? g.props.value : l.__ : r, n.__c ? h = (f = t.__c = n.__c).__ = f.__E : ("prototype" in j && j.prototype.render ? t.__c = f = new j(y, _) : (t.__c = f = new w(y, _), f.constructor = j, f.render = F), g && g.sub(f), f.props = y, f.state || (f.state = {}), f.context = _, f.__n = r, p = f.__d = !0, f.__h = []), null == f.__s && (f.__s = f.state), null != j.getDerivedStateFromProps && (f.__s == f.state && (f.__s = b({}, f.__s)), b(f.__s, j.getDerivedStateFromProps(y, f.__s))), m = f.props, v = f.state, p) null == j.getDerivedStateFromProps && null != f.componentWillMount && f.componentWillMount(), null != f.componentDidMount && f.__h.push(f.componentDidMount);
                 else {
-                    if (null == w.getDerivedStateFromProps && y !== m && null != f.componentWillReceiveProps && f.componentWillReceiveProps(y, _), !f.__e && null != f.shouldComponentUpdate && !1 === f.shouldComponentUpdate(y, f.__s, _) || t.__v === n.__v) {
+                    if (null == j.getDerivedStateFromProps && y !== m && null != f.componentWillReceiveProps && f.componentWillReceiveProps(y, _), !f.__e && null != f.shouldComponentUpdate && !1 === f.shouldComponentUpdate(y, f.__s, _) || t.__v === n.__v) {
                         f.props = y, f.state = f.__s, t.__v !== n.__v && (f.__d = !1), f.__v = t, t.__e = n.__e, t.__k = n.__k, f.__h.length && c.push(f);
                         break e
                     }
                     null != f.componentWillUpdate && f.componentWillUpdate(y, f.__s, _), null != f.componentDidUpdate && f.__h.push((function() {
                         f.componentDidUpdate(m, v, d)
                     }))
                 }
@@ -382,15 +382,15 @@
         s.__ && s.__(e, t), o = (r = "function" == typeof n) ? null : n && n.__k || t.__k, i = [], q(t, e = (!r && n || t).__k = _(S, null, [e]), o || d, d, void 0 !== t.ownerSVGElement, !r && n ? [n] : o ? null : t.firstChild ? h.slice.call(t.childNodes) : null, i, !r && n ? n : o ? o.__e : t.firstChild, r), L(i, e)
     }
 
     function V(e, t) {
         B(e, t, V)
     }
 
-    function W(e, t, n) {
+    function K(e, t, n) {
         var r, o, i, c = arguments,
             a = b({}, e.props);
         for (i in t) "key" == i ? r = t[i] : "ref" == i ? o = t[i] : a[i] = t[i];
         if (arguments.length > 3)
             for (n = [n], i = 3; i < arguments.length; i++) n.push(c[i]);
         return null != n && (a.children = n), O(e.type, a, r || e.key, o || e.ref, null)
     }
@@ -401,21 +401,21 @@
                     if ((r = n.constructor) && null != r.getDerivedStateFromError && (n.setState(r.getDerivedStateFromError(e)), o = n.__d), null != n.componentDidCatch && (n.componentDidCatch(e), o = n.__d), o) return n.__E = n
                 } catch (t) {
                     e = t
                 }
             throw e
         },
         __v: 0
-    }, j.prototype.setState = function(e, t) {
+    }, w.prototype.setState = function(e, t) {
         var n;
         n = null != this.__s && this.__s !== this.state ? this.__s : this.__s = b({}, this.state), "function" == typeof e && (e = e(b({}, n), this.props)), e && b(n, e), null != e && this.__v && (t && this.__h.push(t), P(this))
-    }, j.prototype.forceUpdate = function(e) {
+    }, w.prototype.forceUpdate = function(e) {
         this.__v && (this.__e = !0, e && this.__h.push(e), P(this))
-    }, j.prototype.render = S, f = [], p = "function" == typeof Promise ? Promise.prototype.then.bind(Promise.resolve()) : setTimeout, I.__r = 0, v = 0;
-    var K, z, J, $ = 0,
+    }, w.prototype.render = S, f = [], p = "function" == typeof Promise ? Promise.prototype.then.bind(Promise.resolve()) : setTimeout, I.__r = 0, v = 0;
+    var W, z, J, $ = 0,
         Q = [],
         Z = s.__b,
         Y = s.__r,
         G = s.diffed,
         X = s.__c,
         ee = s.unmount;
 
@@ -429,33 +429,33 @@
     }
 
     function ne(e) {
         return $ = 1, re(pe, e)
     }
 
     function re(e, t, n) {
-        var r = te(K++, 2);
+        var r = te(W++, 2);
         return r.t = e, r.__c || (r.__ = [n ? n(t) : pe(void 0, t), function(e) {
             var t = r.t(r.__[0], e);
             r.__[0] !== t && (r.__ = [t, r.__[1]], r.__c.setState({}))
         }], r.__c = z), r.__
     }
 
     function oe(e, t) {
-        var n = te(K++, 3);
+        var n = te(W++, 3);
         !s.__s && fe(n.__H, t) && (n.__ = e, n.__H = t, z.__H.__h.push(n))
     }
 
     function ie(e, t) {
-        var n = te(K++, 4);
+        var n = te(W++, 4);
         !s.__s && fe(n.__H, t) && (n.__ = e, n.__H = t, z.__h.push(n))
     }
 
     function ce(e, t) {
-        var n = te(K++, 7);
+        var n = te(W++, 7);
         return fe(n.__H, t) && (n.__ = e(), n.__H = t, n.__h = e), n.__
     }
 
     function ae() {
         Q.forEach((function(e) {
             if (e.__P) try {
                 e.__H.__h.forEach(le), e.__H.__h.forEach(se), e.__H.__h = []
@@ -463,15 +463,15 @@
                 e.__H.__h = [], s.__e(t, e.__v)
             }
         })), Q = []
     }
     s.__b = function(e) {
         z = null, Z && Z(e)
     }, s.__r = function(e) {
-        Y && Y(e), K = 0;
+        Y && Y(e), W = 0;
         var t = (z = e.__c).__H;
         t && (t.__h.forEach(le), t.__h.forEach(se), t.__h = [])
     }, s.diffed = function(e) {
         G && G(e);
         var t = e.__c;
         t && t.__H && t.__H.__h.length && (1 !== Q.push(t) && J === s.requestAnimationFrame || ((J = s.requestAnimationFrame) || function(e) {
             var t, n = function() {
@@ -534,15 +534,15 @@
         for (var r in t)
             if ("__source" !== r && e[r] !== t[r]) return !0;
         return !1
     }
 
     function de(e) {
         this.props = e
-    }(de.prototype = new j).isPureReactComponent = !0, de.prototype.shouldComponentUpdate = function(e, t) {
+    }(de.prototype = new w).isPureReactComponent = !0, de.prototype.shouldComponentUpdate = function(e, t) {
         return ve(this.props, e) || ve(this.state, t)
     };
     var he = s.__b;
     s.__b = function(e) {
         e.type && e.type.__f && e.ref && (e.props.ref = e.ref, e.ref = null), he && he(e)
     };
     var ye = "undefined" != typeof Symbol && Symbol.for && Symbol.for("react.forward_ref") || 3911;
@@ -569,23 +569,23 @@
     }
 
     function Se(e) {
         var t = e.__.__c;
         return t && t.__e && t.__e(e)
     }
 
-    function je() {
+    function we() {
         this.u = null, this.o = null
     }
     s.__e = function(e, t, n) {
         if (e.then)
             for (var r, o = t; o = o.__;)
                 if ((r = o.__c) && r.__c) return null == t.__e && (t.__e = n.__e, t.__k = n.__k), r.__c(e, t);
         _e(e, t, n)
-    }, (Oe.prototype = new j).__c = function(e, t) {
+    }, (Oe.prototype = new w).__c = function(e, t) {
         var n = t.__c,
             r = this;
         null == r.t && (r.t = []), r.t.push(n);
         var o = Se(r.__v),
             i = !1,
             c = function() {
                 i || (i = !0, n.componentWillUnmount = n.__c, o ? o(a) : a())
@@ -629,15 +629,15 @@
                 }(this.__b, n, r.__O = r.__P)
             }
             this.__b = null
         }
         var o = t.__e && _(S, null, e.fallback);
         return o && (o.__h = null), [_(S, null, t.__e ? null : e.children), o]
     };
-    var we = function(e, t, n) {
+    var je = function(e, t, n) {
         if (++n[1] === n[0] && e.o.delete(t), e.props.revealOrder && ("t" !== e.props.revealOrder[0] || !e.o.size))
             for (n = e.u; n;) {
                 for (; n.length > 3;) n.pop()();
                 if (n[1] < n[0]) break;
                 e.u = n = n[2]
             }
     };
@@ -672,48 +672,48 @@
     }
 
     function Ie(e, t) {
         return _(Pe, {
             __v: e,
             i: t
         })
-    }(je.prototype = new j).__e = function(e) {
+    }(we.prototype = new w).__e = function(e) {
         var t = this,
             n = Se(t.__v),
             r = t.o.get(e);
         return r[0]++,
             function(o) {
                 var i = function() {
-                    t.props.revealOrder ? (r.push(o), we(t, e, r)) : o()
+                    t.props.revealOrder ? (r.push(o), je(t, e, r)) : o()
                 };
                 n ? n(i) : i()
             }
-    }, je.prototype.render = function(e) {
+    }, we.prototype.render = function(e) {
         this.u = null, this.o = new Map;
         var t = A(e.children);
         e.revealOrder && "b" === e.revealOrder[0] && t.reverse();
         for (var n = t.length; n--;) this.o.set(t[n], this.u = [1, 0, this.u]);
         return e.children
-    }, je.prototype.componentDidUpdate = je.prototype.componentDidMount = function() {
+    }, we.prototype.componentDidUpdate = we.prototype.componentDidMount = function() {
         var e = this;
         this.o.forEach((function(t, n) {
-            we(e, n, t)
+            je(e, n, t)
         }))
     };
     var De = "undefined" != typeof Symbol && Symbol.for && Symbol.for("react.element") || 60103,
         ke = /^(?:accent|alignment|arabic|baseline|cap|clip(?!PathU)|color|fill|flood|font|glyph(?!R)|horiz|marker(?!H|W|U)|overline|paint|stop|strikethrough|stroke|text(?!L)|underline|unicode|units|v|vector|vert|word|writing|x(?!C))[A-Z]/,
         Ae = function(e) {
             return ("undefined" != typeof Symbol && "symbol" == n(Symbol()) ? /fil|che|rad/i : /fil|che|ra/i).test(e)
         };
 
     function Ce(e, t, n) {
         return null == t.__k && (t.textContent = ""), B(e, t), "function" == typeof n && n(), e ? e.__c : null
     }
-    j.prototype.isReactComponent = {}, ["componentWillMount", "componentWillReceiveProps", "componentWillUpdate"].forEach((function(e) {
-        Object.defineProperty(j.prototype, e, {
+    w.prototype.isReactComponent = {}, ["componentWillMount", "componentWillReceiveProps", "componentWillUpdate"].forEach((function(e) {
+        Object.defineProperty(w.prototype, e, {
             configurable: !0,
             get: function() {
                 return this["UNSAFE_" + e]
             },
             set: function(t) {
                 Object.defineProperty(this, e, {
                     configurable: !0,
@@ -800,15 +800,15 @@
         useCallback: function(e, t) {
             return $ = 8, ce((function() {
                 return e
             }), t)
         },
         useContext: function(e) {
             var t = z.context[e.__c],
-                n = te(K++, 9);
+                n = te(W++, 9);
             return n.__c = e, t ? (null == n.__ && (n.__ = !0, t.sub(z)), t.props.value) : e.__
         },
         useDebugValue: function(e, t) {
             s.useDebugValue && s.useDebugValue(t ? t(e) : e)
         },
         version: "16.8.0",
         Children: ge,
@@ -845,27 +845,27 @@
             };
             return n.Provider.__ = n.Consumer.contextType = n
         },
         createFactory: function(e) {
             return _.bind(null, e)
         },
         cloneElement: function(e) {
-            return Fe(e) ? W.apply(null, arguments) : e
+            return Fe(e) ? K.apply(null, arguments) : e
         },
         createRef: function() {
             return {
                 current: null
             }
         },
         Fragment: S,
         isValidElement: Fe,
         findDOMNode: function(e) {
             return e && (e.base || 1 === e.nodeType && e) || null
         },
-        Component: j,
+        Component: w,
         PureComponent: de,
         memo: function(e, t) {
             function n(e) {
                 var n = this.props.ref,
                     r = n == e.ref;
                 return !r && n && (n.call ? n(null) : n.current = null), t ? !t(this.props, e) || !r : ve(this.props, e)
             }
@@ -883,15 +883,15 @@
             return t.$$typeof = ye, t.render = t, t.prototype.isReactComponent = t.__f = !0, t.displayName = "ForwardRef(" + (e.displayName || e.name) + ")", t
         },
         unstable_batchedUpdates: function(e, t) {
             return e(t)
         },
         StrictMode: S,
         Suspense: Oe,
-        SuspenseList: je,
+        SuspenseList: we,
         lazy: function(e) {
             var t, n, r;
 
             function o(o) {
                 if (t || (t = e()).then((function(e) {
                         n = e.default || e
                     }), (function(e) {
@@ -915,30 +915,31 @@
             strokeWidth: "1.2",
             stroke: "currentColor",
             fill: "none",
             strokeLinecap: "square"
         }))
     }
 
-    function We() {
+    function Ke() {
         return Be.createElement("svg", {
             width: "20",
             height: "20",
             className: "DocSearch-Search-Icon",
-            viewBox: "0 0 20 20"
+            viewBox: "0 0 20 20",
+            "aria-hidden": "true"
         }, Be.createElement("path", {
             d: "M14.386 14.386l4.0877 4.0877-4.0877-4.0877c-2.9418 2.9419-7.7115 2.9419-10.6533 0-2.9419-2.9418-2.9419-7.7115 0-10.6533 2.9418-2.9419 7.7115-2.9419 10.6533 0 2.9419 2.9418 2.9419 7.7115 0 10.6533z",
             stroke: "currentColor",
             fill: "none",
             fillRule: "evenodd",
             strokeLinecap: "round",
             strokeLinejoin: "round"
         }))
     }
-    var Ke = ["translations"];
+    var We = ["translations"];
 
     function ze() {
         return ze = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
@@ -1000,15 +1001,15 @@
         }
         return o
     }
     var Ze = "Ctrl";
     var Ye = Be.forwardRef((function(e, t) {
         var n = e.translations,
             r = void 0 === n ? {} : n,
-            o = Qe(e, Ke),
+            o = Qe(e, We),
             i = r.buttonText,
             c = void 0 === i ? "Search" : i,
             a = r.buttonAriaLabel,
             u = void 0 === a ? "Search" : a,
             l = Je(ne(null), 2),
             s = l[0],
             f = l[1];
@@ -1018,84 +1019,108 @@
             type: "button",
             className: "DocSearch DocSearch-Button",
             "aria-label": u
         }, o, {
             ref: t
         }), Be.createElement("span", {
             className: "DocSearch-Button-Container"
-        }, Be.createElement(We, null), Be.createElement("span", {
+        }, Be.createElement(Ke, null), Be.createElement("span", {
             className: "DocSearch-Button-Placeholder"
         }, c)), Be.createElement("span", {
             className: "DocSearch-Button-Keys"
-        }, null !== s && Be.createElement(Be.Fragment, null, Be.createElement("kbd", {
-            className: "DocSearch-Button-Key"
-        }, s === Ze ? Be.createElement(Ve, null) : s), Be.createElement("kbd", {
-            className: "DocSearch-Button-Key"
+        }, null !== s && Be.createElement(Be.Fragment, null, Be.createElement(Ge, {
+            reactsToKey: s === Ze ? Ze : "Meta"
+        }, s === Ze ? Be.createElement(Ve, null) : s), Be.createElement(Ge, {
+            reactsToKey: "k"
         }, "K"))))
     }));
 
-    function Ge(e, t) {
+    function Ge(e) {
+        var t = e.reactsToKey,
+            n = e.children,
+            r = Je(ne(!1), 2),
+            o = r[0],
+            i = r[1];
+        return oe((function() {
+            if (t) return window.addEventListener("keydown", e), window.addEventListener("keyup", n),
+                function() {
+                    window.removeEventListener("keydown", e), window.removeEventListener("keyup", n)
+                };
+
+            function e(e) {
+                e.key === t && i(!0)
+            }
+
+            function n(e) {
+                e.key !== t && "Meta" !== e.key || i(!1)
+            }
+        }), [t]), Be.createElement("kbd", {
+            className: o ? "DocSearch-Button-Key DocSearch-Button-Key--pressed" : "DocSearch-Button-Key"
+        }, n)
+    }
+
+    function Xe(e, t) {
         var n = void 0;
         return function() {
             for (var r = arguments.length, o = new Array(r), i = 0; i < r; i++) o[i] = arguments[i];
             n && clearTimeout(n), n = setTimeout((function() {
                 return e.apply(void 0, o)
             }), t)
         }
     }
 
-    function Xe(e) {
+    function et(e) {
         return e.reduce((function(e, t) {
             return e.concat(t)
         }), [])
     }
-    var et = 0;
+    var tt = 0;
 
-    function tt(e) {
+    function nt(e) {
         return 0 === e.collections.length ? 0 : e.collections.reduce((function(e, t) {
             return e + t.items.length
         }), 0)
     }
 
-    function nt(e) {
+    function rt(e) {
         return e !== Object(e)
     }
 
-    function rt(e, t) {
+    function ot(e, t) {
         if (e === t) return !0;
-        if (nt(e) || nt(t) || "function" == typeof e || "function" == typeof t) return e === t;
+        if (rt(e) || rt(t) || "function" == typeof e || "function" == typeof t) return e === t;
         if (Object.keys(e).length !== Object.keys(t).length) return !1;
         for (var n = 0, r = Object.keys(e); n < r.length; n++) {
             var o = r[n];
             if (!(o in t)) return !1;
-            if (!rt(e[o], t[o])) return !1
+            if (!ot(e[o], t[o])) return !1
         }
         return !0
     }
-    var ot = function() {};
-    var it = [{
+    var it = function() {};
+    var ct = [{
         segment: "autocomplete-core",
         version: "1.9.3"
     }];
 
-    function ct(e) {
+    function at(e) {
         var t = e.item,
             n = e.items;
         return {
             index: t.__autocomplete_indexName,
             items: [t],
             positions: [1 + n.findIndex((function(e) {
                 return e.objectID === t.objectID
             }))],
             queryID: t.__autocomplete_queryID,
             algoliaSource: ["autocomplete"]
         }
     }
 
-    function at(e, t) {
+    function ut(e, t) {
         return function(e) {
             if (Array.isArray(e)) return e
         }(e) || function(e, t) {
             var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
             if (null != n) {
                 var r, o, i, c, a = [],
                     u = !0,
@@ -1115,64 +1140,64 @@
                         if (l) throw o
                     }
                 }
                 return a
             }
         }(e, t) || function(e, t) {
             if (!e) return;
-            if ("string" == typeof e) return ut(e, t);
+            if ("string" == typeof e) return lt(e, t);
             var n = Object.prototype.toString.call(e).slice(8, -1);
             "Object" === n && e.constructor && (n = e.constructor.name);
             if ("Map" === n || "Set" === n) return Array.from(e);
-            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return ut(e, t)
+            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return lt(e, t)
         }(e, t) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function ut(e, t) {
+    function lt(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
-    var lt = ["items"],
-        st = ["items"];
+    var st = ["items"],
+        ft = ["items"];
 
-    function ft(e) {
-        return ft = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function pt(e) {
+        return pt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-        }, ft(e)
+        }, pt(e)
     }
 
-    function pt(e) {
+    function mt(e) {
         return function(e) {
-            if (Array.isArray(e)) return mt(e)
+            if (Array.isArray(e)) return vt(e)
         }(e) || function(e) {
             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
         }(e) || function(e, t) {
             if (!e) return;
-            if ("string" == typeof e) return mt(e, t);
+            if ("string" == typeof e) return vt(e, t);
             var n = Object.prototype.toString.call(e).slice(8, -1);
             "Object" === n && e.constructor && (n = e.constructor.name);
             if ("Map" === n || "Set" === n) return Array.from(e);
-            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return mt(e, t)
+            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return vt(e, t)
         }(e) || function() {
             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function mt(e, t) {
+    function vt(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function vt(e, t) {
+    function dt(e, t) {
         if (null == e) return {};
         var n, r, o = function(e, t) {
             if (null == e) return {};
             var n, r, o = {},
                 i = Object.keys(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
             return o
@@ -1180,132 +1205,132 @@
         if (Object.getOwnPropertySymbols) {
             var i = Object.getOwnPropertySymbols(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
         }
         return o
     }
 
-    function dt(e, t) {
+    function ht(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function ht(e) {
+    function yt(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? dt(Object(n), !0).forEach((function(t) {
-                yt(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : dt(Object(n)).forEach((function(t) {
+            t % 2 ? ht(Object(n), !0).forEach((function(t) {
+                bt(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ht(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function yt(e, t, n) {
+    function bt(e, t, n) {
         return (t = function(e) {
             var t = function(e, t) {
-                if ("object" !== ft(e) || null === e) return e;
+                if ("object" !== pt(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, t || "default");
-                    if ("object" !== ft(r)) return r;
+                    if ("object" !== pt(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
-            return "symbol" === ft(t) ? t : String(t)
+            return "symbol" === pt(t) ? t : String(t)
         }(t)) in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function bt(e) {
-        for (var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 20, n = [], r = 0; r < e.objectIDs.length; r += t) n.push(ht(ht({}, e), {}, {
+    function gt(e) {
+        for (var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 20, n = [], r = 0; r < e.objectIDs.length; r += t) n.push(yt(yt({}, e), {}, {
             objectIDs: e.objectIDs.slice(r, r + t)
         }));
         return n
     }
 
-    function gt(e) {
+    function _t(e) {
         return e.map((function(e) {
             var t = e.items,
-                n = vt(e, lt);
-            return ht(ht({}, n), {}, {
+                n = dt(e, st);
+            return yt(yt({}, n), {}, {
                 objectIDs: (null == t ? void 0 : t.map((function(e) {
                     return e.objectID
                 }))) || n.objectIDs
             })
         }))
     }
 
-    function _t(e) {
-        var t, n, r, o = (t = at((e.version || "").split(".").map(Number), 2), n = t[0], r = t[1], n >= 3 || 2 === n && r >= 4 || 1 === n && r >= 10);
+    function Ot(e) {
+        var t, n, r, o = (t = ut((e.version || "").split(".").map(Number), 2), n = t[0], r = t[1], n >= 3 || 2 === n && r >= 4 || 1 === n && r >= 10);
 
         function i(t, n, r) {
             if (o && void 0 !== r) {
                 var i = r[0].__autocomplete_algoliaCredentials,
                     c = {
                         "X-Algolia-Application-Id": i.appId,
                         "X-Algolia-API-Key": i.apiKey
                     };
-                e.apply(void 0, [t].concat(pt(n), [{
+                e.apply(void 0, [t].concat(mt(n), [{
                     headers: c
                 }]))
-            } else e.apply(void 0, [t].concat(pt(n)))
+            } else e.apply(void 0, [t].concat(mt(n)))
         }
         return {
             init: function(t, n) {
                 e("init", {
                     appId: t,
                     apiKey: n
                 })
             },
             setUserToken: function(t) {
                 e("setUserToken", t)
             },
             clickedObjectIDsAfterSearch: function() {
                 for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-                t.length > 0 && i("clickedObjectIDsAfterSearch", gt(t), t[0].items)
+                t.length > 0 && i("clickedObjectIDsAfterSearch", _t(t), t[0].items)
             },
             clickedObjectIDs: function() {
                 for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-                t.length > 0 && i("clickedObjectIDs", gt(t), t[0].items)
+                t.length > 0 && i("clickedObjectIDs", _t(t), t[0].items)
             },
             clickedFilters: function() {
                 for (var t = arguments.length, n = new Array(t), r = 0; r < t; r++) n[r] = arguments[r];
                 n.length > 0 && e.apply(void 0, ["clickedFilters"].concat(n))
             },
             convertedObjectIDsAfterSearch: function() {
                 for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-                t.length > 0 && i("convertedObjectIDsAfterSearch", gt(t), t[0].items)
+                t.length > 0 && i("convertedObjectIDsAfterSearch", _t(t), t[0].items)
             },
             convertedObjectIDs: function() {
                 for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-                t.length > 0 && i("convertedObjectIDs", gt(t), t[0].items)
+                t.length > 0 && i("convertedObjectIDs", _t(t), t[0].items)
             },
             convertedFilters: function() {
                 for (var t = arguments.length, n = new Array(t), r = 0; r < t; r++) n[r] = arguments[r];
                 n.length > 0 && e.apply(void 0, ["convertedFilters"].concat(n))
             },
             viewedObjectIDs: function() {
                 for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
                 t.length > 0 && t.reduce((function(e, t) {
                     var n = t.items,
-                        r = vt(t, st);
-                    return [].concat(pt(e), pt(bt(ht(ht({}, r), {}, {
+                        r = dt(t, ft);
+                    return [].concat(mt(e), mt(gt(yt(yt({}, r), {}, {
                         objectIDs: (null == n ? void 0 : n.map((function(e) {
                             return e.objectID
                         }))) || r.objectIDs
                     })).map((function(e) {
                         return {
                             items: n,
                             payload: e
@@ -1319,87 +1344,87 @@
             viewedFilters: function() {
                 for (var t = arguments.length, n = new Array(t), r = 0; r < t; r++) n[r] = arguments[r];
                 n.length > 0 && e.apply(void 0, ["viewedFilters"].concat(n))
             }
         }
     }
 
-    function Ot(e) {
+    function St(e) {
         var t = e.items.reduce((function(e, t) {
             var n;
             return e[t.__autocomplete_indexName] = (null !== (n = e[t.__autocomplete_indexName]) && void 0 !== n ? n : []).concat(t), e
         }), {});
         return Object.keys(t).map((function(e) {
             return {
                 index: e,
                 items: t[e],
                 algoliaSource: ["autocomplete"]
             }
         }))
     }
 
-    function St(e) {
+    function wt(e) {
         return e.objectID && e.__autocomplete_indexName && e.__autocomplete_queryID
     }
 
     function jt(e) {
         return jt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         }, jt(e)
     }
 
-    function wt(e) {
+    function Et(e) {
         return function(e) {
-            if (Array.isArray(e)) return Et(e)
+            if (Array.isArray(e)) return Pt(e)
         }(e) || function(e) {
             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
         }(e) || function(e, t) {
             if (!e) return;
-            if ("string" == typeof e) return Et(e, t);
+            if ("string" == typeof e) return Pt(e, t);
             var n = Object.prototype.toString.call(e).slice(8, -1);
             "Object" === n && e.constructor && (n = e.constructor.name);
             if ("Map" === n || "Set" === n) return Array.from(e);
-            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Et(e, t)
+            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Pt(e, t)
         }(e) || function() {
             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function Et(e, t) {
+    function Pt(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function Pt(e, t) {
+    function It(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function It(e) {
+    function Dt(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Pt(Object(n), !0).forEach((function(t) {
-                Dt(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Pt(Object(n)).forEach((function(t) {
+            t % 2 ? It(Object(n), !0).forEach((function(t) {
+                kt(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : It(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Dt(e, t, n) {
+    function kt(e, t, n) {
         return (t = function(e) {
             var t = function(e, t) {
                 if ("object" !== jt(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, t || "default");
                     if ("object" !== jt(r)) return r;
@@ -1411,56 +1436,56 @@
         }(t)) in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
-    var kt = "2.6.0",
-        At = "https://cdn.jsdelivr.net/npm/search-insights@".concat(kt, "/dist/search-insights.min.js"),
-        Ct = Ge((function(e) {
+    var At = "2.6.0",
+        Ct = "https://cdn.jsdelivr.net/npm/search-insights@".concat(At, "/dist/search-insights.min.js"),
+        xt = Xe((function(e) {
             var t = e.onItemsChange,
                 n = e.items,
                 r = e.insights,
                 o = e.state;
             t({
                 insights: r,
-                insightsEvents: Ot({
+                insightsEvents: St({
                     items: n
                 }).map((function(e) {
-                    return It({
+                    return Dt({
                         eventName: "Items Viewed"
                     }, e)
                 })),
                 state: o
             })
         }), 400);
 
-    function xt(e) {
+    function Nt(e) {
         var t = function(e) {
-                return It({
+                return Dt({
                     onItemsChange: function(e) {
                         var t = e.insights,
                             n = e.insightsEvents;
-                        t.viewedObjectIDs.apply(t, wt(n.map((function(e) {
-                            return It(It({}, e), {}, {
-                                algoliaSource: [].concat(wt(e.algoliaSource || []), ["autocomplete-internal"])
+                        t.viewedObjectIDs.apply(t, Et(n.map((function(e) {
+                            return Dt(Dt({}, e), {}, {
+                                algoliaSource: [].concat(Et(e.algoliaSource || []), ["autocomplete-internal"])
                             })
                         }))))
                     },
                     onSelect: function(e) {
                         var t = e.insights,
                             n = e.insightsEvents;
-                        t.clickedObjectIDsAfterSearch.apply(t, wt(n.map((function(e) {
-                            return It(It({}, e), {}, {
-                                algoliaSource: [].concat(wt(e.algoliaSource || []), ["autocomplete-internal"])
+                        t.clickedObjectIDsAfterSearch.apply(t, Et(n.map((function(e) {
+                            return Dt(Dt({}, e), {}, {
+                                algoliaSource: [].concat(Et(e.algoliaSource || []), ["autocomplete-internal"])
                             })
                         }))))
                     },
-                    onActive: ot
+                    onActive: it
                 }, e)
             }(e),
             n = t.insightsClient,
             r = t.onItemsChange,
             o = t.onSelect,
             i = t.onActive,
             c = n;
@@ -1471,41 +1496,41 @@
         }((function(e) {
             var t = e.window,
                 n = t.AlgoliaAnalyticsObject || "aa";
             "string" == typeof n && (c = t[n]), c || (t.AlgoliaAnalyticsObject = n, t[n] || (t[n] = function() {
                 t[n].queue || (t[n].queue = []);
                 for (var e = arguments.length, r = new Array(e), o = 0; o < e; o++) r[o] = arguments[o];
                 t[n].queue.push(r)
-            }), t[n].version = kt, c = t[n], function(e) {
+            }), t[n].version = At, c = t[n], function(e) {
                 var t = "[Autocomplete]: Could not load search-insights.js. Please load it manually following https://alg.li/insights-autocomplete";
                 try {
                     var n = e.document.createElement("script");
-                    n.async = !0, n.src = At, n.onerror = function() {
+                    n.async = !0, n.src = Ct, n.onerror = function() {
                         console.error(t)
                     }, document.body.appendChild(n)
                 } catch (e) {
                     console.error(t)
                 }
             }(t))
         }));
-        var a = _t(c),
+        var a = Ot(c),
             u = {
                 current: []
             },
-            l = Ge((function(e) {
+            l = Xe((function(e) {
                 var t = e.state;
                 if (t.isOpen) {
                     var n = t.collections.reduce((function(e, t) {
-                        return [].concat(wt(e), wt(t.items))
-                    }), []).filter(St);
-                    rt(u.current.map((function(e) {
+                        return [].concat(Et(e), Et(t.items))
+                    }), []).filter(wt);
+                    ot(u.current.map((function(e) {
                         return e.objectID
                     })), n.map((function(e) {
                         return e.objectID
-                    }))) || (u.current = n, n.length > 0 && Ct({
+                    }))) || (u.current = n, n.length > 0 && xt({
                         onItemsChange: r,
                         items: n,
                         insights: a,
                         state: t
                     }))
                 }
             }), 0);
@@ -1522,38 +1547,38 @@
                         },
                         insights: a
                     }
                 }), n((function(e) {
                     var t = e.item,
                         n = e.state,
                         r = e.event;
-                    St(t) && o({
+                    wt(t) && o({
                         state: n,
                         event: r,
                         insights: a,
                         item: t,
-                        insightsEvents: [It({
+                        insightsEvents: [Dt({
                             eventName: "Item Selected"
-                        }, ct({
+                        }, at({
                             item: t,
                             items: u.current
                         }))]
                     })
                 })), r((function(e) {
                     var t = e.item,
                         n = e.state,
                         r = e.event;
-                    St(t) && i({
+                    wt(t) && i({
                         state: n,
                         event: r,
                         insights: a,
                         item: t,
-                        insightsEvents: [It({
+                        insightsEvents: [Dt({
                             eventName: "Item Active"
-                        }, ct({
+                        }, at({
                             item: t,
                             items: u.current
                         }))]
                     })
                 }))
             },
             onStateChange: function(e) {
@@ -1562,25 +1587,25 @@
                     state: t
                 })
             },
             __autocomplete_pluginOptions: e
         }
     }
 
-    function Nt(e, t) {
+    function Tt(e, t) {
         var n = t;
         return {
             then: function(t, r) {
-                return Nt(e.then(Rt(t, n, e), Rt(r, n, e)), n)
+                return Tt(e.then(qt(t, n, e), qt(r, n, e)), n)
             },
             catch: function(t) {
-                return Nt(e.catch(Rt(t, n, e)), n)
+                return Tt(e.catch(qt(t, n, e)), n)
             },
             finally: function(t) {
-                return t && n.onCancelList.push(t), Nt(e.finally(Rt(t && function() {
+                return t && n.onCancelList.push(t), Tt(e.finally(qt(t && function() {
                     return n.onCancelList = [], t()
                 }, n, e)), n)
             },
             cancel: function() {
                 n.isCanceled = !0;
                 var e = n.onCancelList;
                 n.onCancelList = [], e.forEach((function(e) {
@@ -1589,87 +1614,87 @@
             },
             isCanceled: function() {
                 return !0 === n.isCanceled
             }
         }
     }
 
-    function Tt(e) {
-        return Nt(e, {
+    function Rt(e) {
+        return Tt(e, {
             isCanceled: !1,
             onCancelList: []
         })
     }
 
-    function Rt(e, t, n) {
+    function qt(e, t, n) {
         return e ? function(n) {
             return t.isCanceled ? n : e(n)
         } : n
     }
 
-    function qt(e, t, n, r) {
+    function Lt(e, t, n, r) {
         if (!n) return null;
         if (e < 0 && (null === t || null !== r && 0 === t)) return n + e;
         var o = (null === t ? -1 : t) + e;
         return o <= -1 || o >= n ? null === r ? null : 0 : o
     }
 
-    function Lt(e, t) {
+    function Mt(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Mt(e) {
+    function Ht(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Lt(Object(n), !0).forEach((function(t) {
-                Ht(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Lt(Object(n)).forEach((function(t) {
+            t % 2 ? Mt(Object(n), !0).forEach((function(t) {
+                Ut(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Mt(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Ht(e, t, n) {
+    function Ut(e, t, n) {
         return (t = function(e) {
             var t = function(e, t) {
-                if ("object" !== Ut(e) || null === e) return e;
+                if ("object" !== Ft(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, t || "default");
-                    if ("object" !== Ut(r)) return r;
+                    if ("object" !== Ft(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
-            return "symbol" === Ut(t) ? t : String(t)
+            return "symbol" === Ft(t) ? t : String(t)
         }(t)) in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function Ut(e) {
-        return Ut = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function Ft(e) {
+        return Ft = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-        }, Ut(e)
+        }, Ft(e)
     }
 
-    function Ft(e) {
+    function Bt(e) {
         var t = function(e) {
             var t = e.collections.map((function(e) {
                 return e.items.length
             })).reduce((function(e, t, n) {
                 var r = (e[n - 1] || 0) + t;
                 return e.push(r), e
             }), []).reduce((function(t, n) {
@@ -1702,68 +1727,68 @@
             itemUrl: r.getItemUrl({
                 item: n,
                 state: e
             }),
             source: r
         }
     }
-    var Bt = /((gt|sm)-|galaxy nexus)|samsung[- ]|samsungbrowser/i;
+    var Vt = /((gt|sm)-|galaxy nexus)|samsung[- ]|samsungbrowser/i;
 
-    function Vt(e) {
-        return Vt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function Kt(e) {
+        return Kt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-        }, Vt(e)
+        }, Kt(e)
     }
 
     function Wt(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Kt(e, t, n) {
+    function zt(e, t, n) {
         return (t = function(e) {
             var t = function(e, t) {
-                if ("object" !== Vt(e) || null === e) return e;
+                if ("object" !== Kt(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, t || "default");
-                    if ("object" !== Vt(r)) return r;
+                    if ("object" !== Kt(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
-            return "symbol" === Vt(t) ? t : String(t)
+            return "symbol" === Kt(t) ? t : String(t)
         }(t)) in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function zt(e, t, n) {
+    function Jt(e, t, n) {
         var r, o = t.initialState;
         return {
             getState: function() {
                 return o
             },
             dispatch: function(r, i) {
                 var c = function(e) {
                     for (var t = 1; t < arguments.length; t++) {
                         var n = null != arguments[t] ? arguments[t] : {};
                         t % 2 ? Wt(Object(n), !0).forEach((function(t) {
-                            Kt(e, t, n[t])
+                            zt(e, t, n[t])
                         })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Wt(Object(n)).forEach((function(t) {
                             Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                         }))
                     }
                     return e
                 }({}, o);
                 o = e(o, {
@@ -1791,163 +1816,163 @@
                 isEmpty: function() {
                     return 0 === r.length
                 }
             })
         }
     }
 
-    function Jt(e) {
-        return Jt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function $t(e) {
+        return $t = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-        }, Jt(e)
+        }, $t(e)
     }
 
-    function $t(e, t) {
+    function Qt(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Qt(e) {
+    function Zt(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? $t(Object(n), !0).forEach((function(t) {
-                Zt(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : $t(Object(n)).forEach((function(t) {
+            t % 2 ? Qt(Object(n), !0).forEach((function(t) {
+                Yt(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Qt(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Zt(e, t, n) {
+    function Yt(e, t, n) {
         return (t = function(e) {
             var t = function(e, t) {
-                if ("object" !== Jt(e) || null === e) return e;
+                if ("object" !== $t(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, t || "default");
-                    if ("object" !== Jt(r)) return r;
+                    if ("object" !== $t(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
-            return "symbol" === Jt(t) ? t : String(t)
+            return "symbol" === $t(t) ? t : String(t)
         }(t)) in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function Yt(e) {
-        return Yt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function Gt(e) {
+        return Gt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-        }, Yt(e)
+        }, Gt(e)
     }
 
-    function Gt(e) {
+    function Xt(e) {
         return function(e) {
-            if (Array.isArray(e)) return Xt(e)
+            if (Array.isArray(e)) return en(e)
         }(e) || function(e) {
             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
         }(e) || function(e, t) {
             if (!e) return;
-            if ("string" == typeof e) return Xt(e, t);
+            if ("string" == typeof e) return en(e, t);
             var n = Object.prototype.toString.call(e).slice(8, -1);
             "Object" === n && e.constructor && (n = e.constructor.name);
             if ("Map" === n || "Set" === n) return Array.from(e);
-            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Xt(e, t)
+            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return en(e, t)
         }(e) || function() {
             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function Xt(e, t) {
+    function en(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function en(e, t) {
+    function tn(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function tn(e) {
+    function nn(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? en(Object(n), !0).forEach((function(t) {
-                nn(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : en(Object(n)).forEach((function(t) {
+            t % 2 ? tn(Object(n), !0).forEach((function(t) {
+                rn(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : tn(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function nn(e, t, n) {
+    function rn(e, t, n) {
         return (t = function(e) {
             var t = function(e, t) {
-                if ("object" !== Yt(e) || null === e) return e;
+                if ("object" !== Gt(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, t || "default");
-                    if ("object" !== Yt(r)) return r;
+                    if ("object" !== Gt(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
-            return "symbol" === Yt(t) ? t : String(t)
+            return "symbol" === Gt(t) ? t : String(t)
         }(t)) in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function rn(e, t) {
+    function on(e, t) {
         var n, r = "undefined" != typeof window ? window : {},
             o = e.plugins || [];
-        return tn(tn({
+        return nn(nn({
             debug: !1,
             openOnFocus: !1,
             placeholder: "",
             autoFocus: !1,
             defaultActiveItemId: null,
             stallThreshold: 300,
             insights: !1,
             environment: r,
             shouldPanelOpen: function(e) {
-                return tt(e.state) > 0
+                return nt(e.state) > 0
             },
             reshape: function(e) {
                 return e.sources
             }
         }, e), {}, {
-            id: null !== (n = e.id) && void 0 !== n ? n : "autocomplete-".concat(et++),
+            id: null !== (n = e.id) && void 0 !== n ? n : "autocomplete-".concat(tt++),
             plugins: o,
-            initialState: tn({
+            initialState: nn({
                 activeItemId: null,
                 query: "",
                 completion: null,
                 collections: [],
                 isOpen: !1,
                 status: "idle",
                 context: {}
@@ -1970,15 +1995,15 @@
                 var n;
                 null === (n = e.onReset) || void 0 === n || n.call(e, t), o.forEach((function(e) {
                     var n;
                     return null === (n = e.onReset) || void 0 === n ? void 0 : n.call(e, t)
                 }))
             },
             getSources: function(n) {
-                return Promise.all([].concat(Gt(o.map((function(e) {
+                return Promise.all([].concat(Xt(o.map((function(e) {
                     return e.getSources
                 }))), [e.getSources]).filter(Boolean).map((function(e) {
                     return function(e, t) {
                         var n = [];
                         return Promise.resolve(e(t)).then((function(e) {
                             return Promise.all(e.filter((function(e) {
                                 return Boolean(e)
@@ -1989,30 +2014,30 @@
                                     getItemInputValue: function(e) {
                                         return e.state.query
                                     },
                                     getItemUrl: function() {},
                                     onSelect: function(e) {
                                         (0, e.setIsOpen)(!1)
                                     },
-                                    onActive: ot,
-                                    onResolve: ot
+                                    onActive: it,
+                                    onResolve: it
                                 };
                                 Object.keys(t).forEach((function(e) {
                                     t[e].__default = !0
                                 }));
-                                var r = Mt(Mt({}, t), e);
+                                var r = Ht(Ht({}, t), e);
                                 return Promise.resolve(r)
                             })))
                         }))
                     }(e, n)
                 }))).then((function(e) {
-                    return Xe(e)
+                    return et(e)
                 })).then((function(e) {
                     return e.map((function(e) {
-                        return tn(tn({}, e), {}, {
+                        return nn(nn({}, e), {}, {
                             onSelect: function(n) {
                                 e.onSelect(n), t.forEach((function(e) {
                                     var t;
                                     return null === (t = e.onSelect) || void 0 === t ? void 0 : t.call(e, n)
                                 }))
                             },
                             onActive: function(n) {
@@ -2027,15 +2052,15 @@
                                     return null === (t = e.onResolve) || void 0 === t ? void 0 : t.call(e, n)
                                 }))
                             }
                         })
                     }))
                 }))
             },
-            navigator: tn({
+            navigator: nn({
                 navigate: function(e) {
                     var t = e.itemUrl;
                     r.location.assign(t)
                 },
                 navigateNewTab: function(e) {
                     var t = e.itemUrl,
                         n = r.open(t, "_blank", "noopener");
@@ -2045,209 +2070,209 @@
                     var t = e.itemUrl;
                     r.open(t, "_blank", "noopener")
                 }
             }, e.navigator)
         })
     }
 
-    function on(e) {
-        return on = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function cn(e) {
+        return cn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-        }, on(e)
+        }, cn(e)
     }
 
-    function cn(e, t) {
+    function an(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function an(e) {
+    function un(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? cn(Object(n), !0).forEach((function(t) {
-                un(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : cn(Object(n)).forEach((function(t) {
+            t % 2 ? an(Object(n), !0).forEach((function(t) {
+                ln(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : an(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function un(e, t, n) {
+    function ln(e, t, n) {
         return (t = function(e) {
             var t = function(e, t) {
-                if ("object" !== on(e) || null === e) return e;
+                if ("object" !== cn(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, t || "default");
-                    if ("object" !== on(r)) return r;
+                    if ("object" !== cn(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
-            return "symbol" === on(t) ? t : String(t)
+            return "symbol" === cn(t) ? t : String(t)
         }(t)) in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function ln(e) {
-        return ln = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function sn(e) {
+        return sn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-        }, ln(e)
+        }, sn(e)
     }
 
-    function sn(e, t) {
+    function fn(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function fn(e) {
+    function pn(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? sn(Object(n), !0).forEach((function(t) {
-                pn(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : sn(Object(n)).forEach((function(t) {
+            t % 2 ? fn(Object(n), !0).forEach((function(t) {
+                mn(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : fn(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function pn(e, t, n) {
+    function mn(e, t, n) {
         return (t = function(e) {
             var t = function(e, t) {
-                if ("object" !== ln(e) || null === e) return e;
+                if ("object" !== sn(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, t || "default");
-                    if ("object" !== ln(r)) return r;
+                    if ("object" !== sn(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
-            return "symbol" === ln(t) ? t : String(t)
+            return "symbol" === sn(t) ? t : String(t)
         }(t)) in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function mn(e) {
+    function vn(e) {
         return function(e) {
-            if (Array.isArray(e)) return vn(e)
+            if (Array.isArray(e)) return dn(e)
         }(e) || function(e) {
             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
         }(e) || function(e, t) {
             if (!e) return;
-            if ("string" == typeof e) return vn(e, t);
+            if ("string" == typeof e) return dn(e, t);
             var n = Object.prototype.toString.call(e).slice(8, -1);
             "Object" === n && e.constructor && (n = e.constructor.name);
             if ("Map" === n || "Set" === n) return Array.from(e);
-            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return vn(e, t)
+            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return dn(e, t)
         }(e) || function() {
             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function vn(e, t) {
+    function dn(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function dn(e) {
+    function hn(e) {
         return Boolean(e.execute)
     }
 
-    function hn(e, t, n) {
+    function yn(e, t, n) {
         if (o = e, Boolean(null == o ? void 0 : o.execute)) {
-            var r = "algolia" === e.requesterId ? Object.assign.apply(Object, [{}].concat(mn(Object.keys(n.context).map((function(e) {
+            var r = "algolia" === e.requesterId ? Object.assign.apply(Object, [{}].concat(vn(Object.keys(n.context).map((function(e) {
                 var t;
                 return null === (t = n.context[e]) || void 0 === t ? void 0 : t.__algoliaSearchParameters
             }))))) : {};
-            return fn(fn({}, e), {}, {
+            return pn(pn({}, e), {}, {
                 requests: e.queries.map((function(n) {
                     return {
-                        query: "algolia" === e.requesterId ? fn(fn({}, n), {}, {
-                            params: fn(fn({}, r), n.params)
+                        query: "algolia" === e.requesterId ? pn(pn({}, n), {}, {
+                            params: pn(pn({}, r), n.params)
                         }) : n,
                         sourceId: t,
                         transformResponse: e.transformResponse
                     }
                 }))
             })
         }
         var o;
         return {
             items: e,
             sourceId: t
         }
     }
 
-    function yn(e) {
+    function bn(e) {
         var t = e.reduce((function(e, t) {
-            if (!dn(t)) return e.push(t), e;
+            if (!hn(t)) return e.push(t), e;
             var n = t.searchClient,
                 r = t.execute,
                 o = t.requesterId,
                 i = t.requests,
                 c = e.find((function(e) {
-                    return dn(t) && dn(e) && e.searchClient === n && Boolean(o) && e.requesterId === o
+                    return hn(t) && hn(e) && e.searchClient === n && Boolean(o) && e.requesterId === o
                 }));
             if (c) {
                 var a;
-                (a = c.items).push.apply(a, mn(i))
+                (a = c.items).push.apply(a, vn(i))
             } else {
                 var u = {
                     execute: r,
                     requesterId: o,
                     items: i,
                     searchClient: n
                 };
                 e.push(u)
             }
             return e
         }), []).map((function(e) {
-            if (!dn(e)) return Promise.resolve(e);
+            if (!hn(e)) return Promise.resolve(e);
             var t = e,
                 n = t.execute,
                 r = t.items;
             return n({
                 searchClient: t.searchClient,
                 requests: r
             })
         }));
         return Promise.all(t).then((function(e) {
-            return Xe(e)
+            return et(e)
         }))
     }
 
-    function bn(e, t, n) {
+    function gn(e, t, n) {
         return t.map((function(t) {
             var r, o = e.filter((function(e) {
                     return e.sourceId === t.sourceId
                 })),
                 i = o.map((function(e) {
                     return e.items
                 })),
@@ -2280,156 +2305,156 @@
             }), a.every(Boolean), 'The `getItems` function from source "'.concat(t.sourceId, '" must return an array of items but returned ').concat(JSON.stringify(void 0), ".\n\nDid you forget to return items?\n\nSee: https://www.algolia.com/doc/ui-libraries/autocomplete/core-concepts/sources/#param-getitems"), {
                 source: t,
                 items: a
             }
         }))
     }
 
-    function gn(e) {
-        return gn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function _n(e) {
+        return _n = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-        }, gn(e)
+        }, _n(e)
     }
-    var _n = ["event", "nextState", "props", "query", "refresh", "store"];
+    var On = ["event", "nextState", "props", "query", "refresh", "store"];
 
-    function On(e, t) {
+    function Sn(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Sn(e) {
+    function wn(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? On(Object(n), !0).forEach((function(t) {
+            t % 2 ? Sn(Object(n), !0).forEach((function(t) {
                 jn(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : On(Object(n)).forEach((function(t) {
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Sn(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
     function jn(e, t, n) {
         return (t = function(e) {
             var t = function(e, t) {
-                if ("object" !== gn(e) || null === e) return e;
+                if ("object" !== _n(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, t || "default");
-                    if ("object" !== gn(r)) return r;
+                    if ("object" !== _n(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
-            return "symbol" === gn(t) ? t : String(t)
+            return "symbol" === _n(t) ? t : String(t)
         }(t)) in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function wn(e, t) {
+    function En(e, t) {
         if (null == e) return {};
         var n, r, o = function(e, t) {
             if (null == e) return {};
             var n, r, o = {},
                 i = Object.keys(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
             return o
         }(e, t);
         if (Object.getOwnPropertySymbols) {
             var i = Object.getOwnPropertySymbols(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
         }
         return o
     }
-    var En, Pn, In, Dn = null,
-        kn = (En = -1, Pn = -1, In = void 0, function(e) {
-            var t = ++En;
+    var Pn, In, Dn, kn = null,
+        An = (Pn = -1, In = -1, Dn = void 0, function(e) {
+            var t = ++Pn;
             return Promise.resolve(e).then((function(e) {
-                return In && t < Pn ? In : (Pn = t, In = e, e)
+                return Dn && t < In ? Dn : (In = t, Dn = e, e)
             }))
         });
 
-    function An(e) {
+    function Cn(e) {
         var t = e.event,
             n = e.nextState,
             r = void 0 === n ? {} : n,
             o = e.props,
             i = e.query,
             c = e.refresh,
             a = e.store,
-            u = wn(e, _n);
-        Dn && o.environment.clearTimeout(Dn);
+            u = En(e, On);
+        kn && o.environment.clearTimeout(kn);
         var l = u.setCollections,
             s = u.setIsOpen,
             f = u.setQuery,
             p = u.setActiveItemId,
             m = u.setStatus;
         if (f(i), p(o.defaultActiveItemId), !i && !1 === o.openOnFocus) {
             var v, d = a.getState().collections.map((function(e) {
-                return Sn(Sn({}, e), {}, {
+                return wn(wn({}, e), {}, {
                     items: []
                 })
             }));
             m("idle"), l(d), s(null !== (v = r.isOpen) && void 0 !== v ? v : o.shouldPanelOpen({
                 state: a.getState()
             }));
-            var h = Tt(kn(d).then((function() {
+            var h = Rt(An(d).then((function() {
                 return Promise.resolve()
             })));
             return a.pendingRequests.add(h)
         }
-        m("loading"), Dn = o.environment.setTimeout((function() {
+        m("loading"), kn = o.environment.setTimeout((function() {
             m("stalled")
         }), o.stallThreshold);
-        var y = Tt(kn(o.getSources(Sn({
+        var y = Rt(An(o.getSources(wn({
             query: i,
             refresh: c,
             state: a.getState()
         }, u)).then((function(e) {
             return Promise.all(e.map((function(e) {
-                return Promise.resolve(e.getItems(Sn({
+                return Promise.resolve(e.getItems(wn({
                     query: i,
                     refresh: c,
                     state: a.getState()
                 }, u))).then((function(t) {
-                    return hn(t, e.sourceId, a.getState())
+                    return yn(t, e.sourceId, a.getState())
                 }))
-            }))).then(yn).then((function(t) {
-                return bn(t, e, a)
+            }))).then(bn).then((function(t) {
+                return gn(t, e, a)
             })).then((function(e) {
                 return function(e) {
                     var t = e.collections,
                         n = e.props,
                         r = e.state,
                         o = t.reduce((function(e, t) {
-                            return an(an({}, e), {}, un({}, t.source.sourceId, an(an({}, t.source), {}, {
+                            return un(un({}, e), {}, ln({}, t.source.sourceId, un(un({}, t.source), {}, {
                                 getItems: function() {
-                                    return Xe(t.items)
+                                    return et(t.items)
                                 }
                             })))
                         }), {}),
                         i = n.plugins.reduce((function(e, t) {
                             return t.reshape ? t.reshape(e) : e
                         }), {
                             sourcesBySourceId: o,
                             state: r
                         }).sourcesBySourceId;
-                    return Xe(n.reshape({
+                    return et(n.reshape({
                         sourcesBySourceId: i,
                         sources: Object.values(i),
                         state: r
                     })).filter(Boolean).map((function(e) {
                         return {
                             source: e,
                             items: e.getItems()
@@ -2444,90 +2469,90 @@
         })))).then((function(e) {
             var n;
             m("idle"), l(e);
             var f = o.shouldPanelOpen({
                 state: a.getState()
             });
             s(null !== (n = r.isOpen) && void 0 !== n ? n : o.openOnFocus && !i && f || f);
-            var p = Ft(a.getState());
+            var p = Bt(a.getState());
             if (null !== a.getState().activeItemId && p) {
                 var v = p.item,
                     d = p.itemInputValue,
                     h = p.itemUrl,
                     y = p.source;
-                y.onActive(Sn({
+                y.onActive(wn({
                     event: t,
                     item: v,
                     itemInputValue: d,
                     itemUrl: h,
                     refresh: c,
                     source: y,
                     state: a.getState()
                 }, u))
             }
         })).finally((function() {
-            m("idle"), Dn && o.environment.clearTimeout(Dn)
+            m("idle"), kn && o.environment.clearTimeout(kn)
         }));
         return a.pendingRequests.add(y)
     }
 
-    function Cn(e) {
-        return Cn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function xn(e) {
+        return xn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-        }, Cn(e)
+        }, xn(e)
     }
-    var xn = ["event", "props", "refresh", "store"];
+    var Nn = ["event", "props", "refresh", "store"];
 
-    function Nn(e, t) {
+    function Tn(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Tn(e) {
+    function Rn(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Nn(Object(n), !0).forEach((function(t) {
-                Rn(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Nn(Object(n)).forEach((function(t) {
+            t % 2 ? Tn(Object(n), !0).forEach((function(t) {
+                qn(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Tn(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Rn(e, t, n) {
+    function qn(e, t, n) {
         return (t = function(e) {
             var t = function(e, t) {
-                if ("object" !== Cn(e) || null === e) return e;
+                if ("object" !== xn(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, t || "default");
-                    if ("object" !== Cn(r)) return r;
+                    if ("object" !== xn(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
-            return "symbol" === Cn(t) ? t : String(t)
+            return "symbol" === xn(t) ? t : String(t)
         }(t)) in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function qn(e, t) {
+    function Ln(e, t) {
         if (null == e) return {};
         var n, r, o = function(e, t) {
             if (null == e) return {};
             var n, r, o = {},
                 i = Object.keys(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
             return o
@@ -2535,74 +2560,74 @@
         if (Object.getOwnPropertySymbols) {
             var i = Object.getOwnPropertySymbols(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
         }
         return o
     }
 
-    function Ln(e) {
-        return Ln = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function Mn(e) {
+        return Mn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-        }, Ln(e)
+        }, Mn(e)
     }
-    var Mn = ["props", "refresh", "store"],
-        Hn = ["inputElement", "formElement", "panelElement"],
-        Un = ["inputElement"],
-        Fn = ["inputElement", "maxLength"],
-        Bn = ["sourceIndex"],
+    var Hn = ["props", "refresh", "store"],
+        Un = ["inputElement", "formElement", "panelElement"],
+        Fn = ["inputElement"],
+        Bn = ["inputElement", "maxLength"],
         Vn = ["sourceIndex"],
+        Kn = ["sourceIndex"],
         Wn = ["item", "source", "sourceIndex"];
 
-    function Kn(e, t) {
+    function zn(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function zn(e) {
+    function Jn(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Kn(Object(n), !0).forEach((function(t) {
-                Jn(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Kn(Object(n)).forEach((function(t) {
+            t % 2 ? zn(Object(n), !0).forEach((function(t) {
+                $n(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : zn(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Jn(e, t, n) {
+    function $n(e, t, n) {
         return (t = function(e) {
             var t = function(e, t) {
-                if ("object" !== Ln(e) || null === e) return e;
+                if ("object" !== Mn(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, t || "default");
-                    if ("object" !== Ln(r)) return r;
+                    if ("object" !== Mn(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
-            return "symbol" === Ln(t) ? t : String(t)
+            return "symbol" === Mn(t) ? t : String(t)
         }(t)) in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function $n(e, t) {
+    function Qn(e, t) {
         if (null == e) return {};
         var n, r, o = function(e, t) {
             if (null == e) return {};
             var n, r, o = {},
                 i = Object.keys(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
             return o
@@ -2610,19 +2635,19 @@
         if (Object.getOwnPropertySymbols) {
             var i = Object.getOwnPropertySymbols(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
         }
         return o
     }
 
-    function Qn(e) {
+    function Zn(e) {
         var t = e.props,
             n = e.refresh,
             r = e.store,
-            o = $n(e, Mn),
+            o = Qn(e, Hn),
             i = function(e, t) {
                 return void 0 !== t ? "".concat(e, "-").concat(t) : e
             };
         return {
             getEnvironmentProps: function(e) {
                 var n = e.inputElement,
                     o = e.formElement,
@@ -2630,86 +2655,86 @@
 
                 function c(e) {
                     !r.getState().isOpen && r.pendingRequests.isEmpty() || e.target === n || !1 === [o, i].some((function(t) {
                         return n = t, r = e.target, n === r || n.contains(r);
                         var n, r
                     })) && (r.dispatch("blur", null), t.debug || r.pendingRequests.cancelAll())
                 }
-                return zn({
+                return Jn({
                     onTouchStart: c,
                     onMouseDown: c,
                     onTouchMove: function(e) {
                         !1 !== r.getState().isOpen && n === t.environment.document.activeElement && e.target !== n && n.blur()
                     }
-                }, $n(e, Hn))
+                }, Qn(e, Un))
             },
             getRootProps: function(e) {
-                return zn({
+                return Jn({
                     role: "combobox",
                     "aria-expanded": r.getState().isOpen,
                     "aria-haspopup": "listbox",
                     "aria-owns": r.getState().isOpen ? "".concat(t.id, "-list") : void 0,
                     "aria-labelledby": "".concat(t.id, "-label")
                 }, e)
             },
             getFormProps: function(e) {
                 e.inputElement;
-                return zn({
+                return Jn({
                     action: "",
                     noValidate: !0,
                     role: "search",
                     onSubmit: function(i) {
                         var c;
-                        i.preventDefault(), t.onSubmit(zn({
+                        i.preventDefault(), t.onSubmit(Jn({
                             event: i,
                             refresh: n,
                             state: r.getState()
                         }, o)), r.dispatch("submit", null), null === (c = e.inputElement) || void 0 === c || c.blur()
                     },
                     onReset: function(i) {
                         var c;
-                        i.preventDefault(), t.onReset(zn({
+                        i.preventDefault(), t.onReset(Jn({
                             event: i,
                             refresh: n,
                             state: r.getState()
                         }, o)), r.dispatch("reset", null), null === (c = e.inputElement) || void 0 === c || c.focus()
                     }
-                }, $n(e, Un))
+                }, Qn(e, Fn))
             },
             getLabelProps: function(e) {
                 var n = e || {},
                     r = n.sourceIndex,
-                    o = $n(n, Bn);
-                return zn({
+                    o = Qn(n, Vn);
+                return Jn({
                     htmlFor: "".concat(i(t.id, r), "-input"),
                     id: "".concat(i(t.id, r), "-label")
                 }, o)
             },
             getInputProps: function(e) {
                 var i;
 
                 function c(e) {
-                    (t.openOnFocus || Boolean(r.getState().query)) && An(zn({
+                    (t.openOnFocus || Boolean(r.getState().query)) && Cn(Jn({
                         event: e,
                         props: t,
                         query: r.getState().completion || r.getState().query,
                         refresh: n,
                         store: r
                     }, o)), r.dispatch("focus", null)
                 }
                 var a = e || {},
                     u = (a.inputElement, a.maxLength),
                     l = void 0 === u ? 512 : u,
-                    s = $n(a, Fn),
-                    f = Ft(r.getState()),
+                    s = Qn(a, Bn),
+                    f = Bt(r.getState()),
                     p = function(e) {
-                        return Boolean(e && e.match(Bt))
+                        return Boolean(e && e.match(Vt))
                     }((null === (i = t.environment.navigator) || void 0 === i ? void 0 : i.userAgent) || ""),
                     m = null != f && f.itemUrl && !p ? "go" : "search";
-                return zn({
+                return Jn({
                     "aria-autocomplete": "both",
                     "aria-activedescendant": r.getState().isOpen && null !== r.getState().activeItemId ? "".concat(t.id, "-item-").concat(r.getState().activeItemId) : void 0,
                     "aria-controls": r.getState().isOpen ? "".concat(t.id, "-list") : void 0,
                     "aria-labelledby": "".concat(t.id, "-label"),
                     value: r.getState().completion || r.getState().query,
                     id: "".concat(t.id, "-input"),
                     autoComplete: "off",
@@ -2718,53 +2743,53 @@
                     enterKeyHint: m,
                     spellCheck: "false",
                     autoFocus: t.autoFocus,
                     placeholder: t.placeholder,
                     maxLength: l,
                     type: "search",
                     onChange: function(e) {
-                        An(zn({
+                        Cn(Jn({
                             event: e,
                             props: t,
                             query: e.currentTarget.value.slice(0, l),
                             refresh: n,
                             store: r
                         }, o))
                     },
                     onKeyDown: function(e) {
                         ! function(e) {
                             var t = e.event,
                                 n = e.props,
                                 r = e.refresh,
                                 o = e.store,
-                                i = qn(e, xn);
+                                i = Ln(e, Nn);
                             if ("ArrowUp" === t.key || "ArrowDown" === t.key) {
                                 var c = function() {
                                         var e = n.environment.document.getElementById("".concat(n.id, "-item-").concat(o.getState().activeItemId));
                                         e && (e.scrollIntoViewIfNeeded ? e.scrollIntoViewIfNeeded(!1) : e.scrollIntoView(!1))
                                     },
                                     a = function() {
-                                        var e = Ft(o.getState());
+                                        var e = Bt(o.getState());
                                         if (null !== o.getState().activeItemId && e) {
                                             var n = e.item,
                                                 c = e.itemInputValue,
                                                 a = e.itemUrl,
                                                 u = e.source;
-                                            u.onActive(Tn({
+                                            u.onActive(Rn({
                                                 event: t,
                                                 item: n,
                                                 itemInputValue: c,
                                                 itemUrl: a,
                                                 refresh: r,
                                                 source: u,
                                                 state: o.getState()
                                             }, i))
                                         }
                                     };
-                                t.preventDefault(), !1 === o.getState().isOpen && (n.openOnFocus || Boolean(o.getState().query)) ? An(Tn({
+                                t.preventDefault(), !1 === o.getState().isOpen && (n.openOnFocus || Boolean(o.getState().query)) ? Cn(Rn({
                                     event: t,
                                     props: n,
                                     query: o.getState().query,
                                     refresh: r,
                                     store: o
                                 }, i)).then((function() {
                                     o.dispatch(t.key, {
@@ -2774,135 +2799,135 @@
                             } else if ("Escape" === t.key) t.preventDefault(), o.dispatch(t.key, null), o.pendingRequests.cancelAll();
                             else if ("Tab" === t.key) o.dispatch("blur", null), o.pendingRequests.cancelAll();
                             else if ("Enter" === t.key) {
                                 if (null === o.getState().activeItemId || o.getState().collections.every((function(e) {
                                         return 0 === e.items.length
                                     }))) return void(n.debug || o.pendingRequests.cancelAll());
                                 t.preventDefault();
-                                var u = Ft(o.getState()),
+                                var u = Bt(o.getState()),
                                     l = u.item,
                                     s = u.itemInputValue,
                                     f = u.itemUrl,
                                     p = u.source;
-                                if (t.metaKey || t.ctrlKey) void 0 !== f && (p.onSelect(Tn({
+                                if (t.metaKey || t.ctrlKey) void 0 !== f && (p.onSelect(Rn({
                                     event: t,
                                     item: l,
                                     itemInputValue: s,
                                     itemUrl: f,
                                     refresh: r,
                                     source: p,
                                     state: o.getState()
                                 }, i)), n.navigator.navigateNewTab({
                                     itemUrl: f,
                                     item: l,
                                     state: o.getState()
                                 }));
-                                else if (t.shiftKey) void 0 !== f && (p.onSelect(Tn({
+                                else if (t.shiftKey) void 0 !== f && (p.onSelect(Rn({
                                     event: t,
                                     item: l,
                                     itemInputValue: s,
                                     itemUrl: f,
                                     refresh: r,
                                     source: p,
                                     state: o.getState()
                                 }, i)), n.navigator.navigateNewWindow({
                                     itemUrl: f,
                                     item: l,
                                     state: o.getState()
                                 }));
                                 else if (t.altKey);
                                 else {
-                                    if (void 0 !== f) return p.onSelect(Tn({
+                                    if (void 0 !== f) return p.onSelect(Rn({
                                         event: t,
                                         item: l,
                                         itemInputValue: s,
                                         itemUrl: f,
                                         refresh: r,
                                         source: p,
                                         state: o.getState()
                                     }, i)), void n.navigator.navigate({
                                         itemUrl: f,
                                         item: l,
                                         state: o.getState()
                                     });
-                                    An(Tn({
+                                    Cn(Rn({
                                         event: t,
                                         nextState: {
                                             isOpen: !1
                                         },
                                         props: n,
                                         query: s,
                                         refresh: r,
                                         store: o
                                     }, i)).then((function() {
-                                        p.onSelect(Tn({
+                                        p.onSelect(Rn({
                                             event: t,
                                             item: l,
                                             itemInputValue: s,
                                             itemUrl: f,
                                             refresh: r,
                                             source: p,
                                             state: o.getState()
                                         }, i))
                                     }))
                                 }
                             }
-                        }(zn({
+                        }(Jn({
                             event: e,
                             props: t,
                             refresh: n,
                             store: r
                         }, o))
                     },
                     onFocus: c,
-                    onBlur: ot,
+                    onBlur: it,
                     onClick: function(n) {
                         e.inputElement !== t.environment.document.activeElement || r.getState().isOpen || c(n)
                     }
                 }, s)
             },
             getPanelProps: function(e) {
-                return zn({
+                return Jn({
                     onMouseDown: function(e) {
                         e.preventDefault()
                     },
                     onMouseLeave: function() {
                         r.dispatch("mouseleave", null)
                     }
                 }, e)
             },
             getListProps: function(e) {
                 var n = e || {},
                     r = n.sourceIndex,
-                    o = $n(n, Vn);
-                return zn({
+                    o = Qn(n, Kn);
+                return Jn({
                     role: "listbox",
                     "aria-labelledby": "".concat(i(t.id, r), "-label"),
                     id: "".concat(i(t.id, r), "-list")
                 }, o)
             },
             getItemProps: function(e) {
                 var c = e.item,
                     a = e.source,
                     u = e.sourceIndex,
-                    l = $n(e, Wn);
-                return zn({
+                    l = Qn(e, Wn);
+                return Jn({
                     id: "".concat(i(t.id, u), "-item-").concat(c.__autocomplete_id),
                     role: "option",
                     "aria-selected": r.getState().activeItemId === c.__autocomplete_id,
                     onMouseMove: function(e) {
                         if (c.__autocomplete_id !== r.getState().activeItemId) {
                             r.dispatch("mousemove", c.__autocomplete_id);
-                            var t = Ft(r.getState());
+                            var t = Bt(r.getState());
                             if (null !== r.getState().activeItemId && t) {
                                 var i = t.item,
                                     a = t.itemInputValue,
                                     u = t.itemUrl,
                                     l = t.source;
-                                l.onActive(zn({
+                                l.onActive(Jn({
                                     event: e,
                                     item: i,
                                     itemInputValue: a,
                                     itemUrl: u,
                                     refresh: n,
                                     source: l,
                                     state: r.getState()
@@ -2918,25 +2943,25 @@
                                 item: c,
                                 state: r.getState()
                             }),
                             u = a.getItemUrl({
                                 item: c,
                                 state: r.getState()
                             });
-                        (u ? Promise.resolve() : An(zn({
+                        (u ? Promise.resolve() : Cn(Jn({
                             event: e,
                             nextState: {
                                 isOpen: !1
                             },
                             props: t,
                             query: i,
                             refresh: n,
                             store: r
                         }, o))).then((function() {
-                            a.onSelect(zn({
+                            a.onSelect(Jn({
                                 event: e,
                                 item: c,
                                 itemInputValue: i,
                                 itemUrl: u,
                                 refresh: n,
                                 source: a,
                                 state: r.getState()
@@ -2944,290 +2969,290 @@
                         }))
                     }
                 }, l)
             }
         }
     }
 
-    function Zn(e) {
-        return Zn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function Yn(e) {
+        return Yn = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-        }, Zn(e)
+        }, Yn(e)
     }
 
-    function Yn(e, t) {
+    function Gn(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Gn(e) {
+    function Xn(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Yn(Object(n), !0).forEach((function(t) {
-                Xn(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Yn(Object(n)).forEach((function(t) {
+            t % 2 ? Gn(Object(n), !0).forEach((function(t) {
+                er(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Gn(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Xn(e, t, n) {
+    function er(e, t, n) {
         return (t = function(e) {
             var t = function(e, t) {
-                if ("object" !== Zn(e) || null === e) return e;
+                if ("object" !== Yn(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, t || "default");
-                    if ("object" !== Zn(r)) return r;
+                    if ("object" !== Yn(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
-            return "symbol" === Zn(t) ? t : String(t)
+            return "symbol" === Yn(t) ? t : String(t)
         }(t)) in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function er(e) {
+    function tr(e) {
         var t, n, r, o, i = e.plugins,
             c = e.options,
             a = null === (t = ((null === (n = c.__autocomplete_metadata) || void 0 === n ? void 0 : n.userAgents) || [])[0]) || void 0 === t ? void 0 : t.segment,
-            u = a ? Xn({}, a, Object.keys((null === (r = c.__autocomplete_metadata) || void 0 === r ? void 0 : r.options) || {})) : {};
+            u = a ? er({}, a, Object.keys((null === (r = c.__autocomplete_metadata) || void 0 === r ? void 0 : r.options) || {})) : {};
         return {
             plugins: i.map((function(e) {
                 return {
                     name: e.name,
                     options: Object.keys(e.__autocomplete_pluginOptions || [])
                 }
             })),
-            options: Gn({
+            options: Xn({
                 "autocomplete-core": Object.keys(c)
             }, u),
-            ua: it.concat((null === (o = c.__autocomplete_metadata) || void 0 === o ? void 0 : o.userAgents) || [])
+            ua: ct.concat((null === (o = c.__autocomplete_metadata) || void 0 === o ? void 0 : o.userAgents) || [])
         }
     }
 
-    function tr(e) {
+    function nr(e) {
         var t, n = e.state;
-        return !1 === n.isOpen || null === n.activeItemId ? null : (null === (t = Ft(n)) || void 0 === t ? void 0 : t.itemInputValue) || null
+        return !1 === n.isOpen || null === n.activeItemId ? null : (null === (t = Bt(n)) || void 0 === t ? void 0 : t.itemInputValue) || null
     }
 
-    function nr(e) {
-        return nr = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function rr(e) {
+        return rr = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-        }, nr(e)
+        }, rr(e)
     }
 
-    function rr(e, t) {
+    function or(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function or(e) {
+    function ir(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? rr(Object(n), !0).forEach((function(t) {
-                ir(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : rr(Object(n)).forEach((function(t) {
+            t % 2 ? or(Object(n), !0).forEach((function(t) {
+                cr(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : or(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function ir(e, t, n) {
+    function cr(e, t, n) {
         return (t = function(e) {
             var t = function(e, t) {
-                if ("object" !== nr(e) || null === e) return e;
+                if ("object" !== rr(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, t || "default");
-                    if ("object" !== nr(r)) return r;
+                    if ("object" !== rr(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
-            return "symbol" === nr(t) ? t : String(t)
+            return "symbol" === rr(t) ? t : String(t)
         }(t)) in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
-    var cr = function(e, t) {
+    var ar = function(e, t) {
         switch (t.type) {
             case "setActiveItemId":
             case "mousemove":
-                return or(or({}, e), {}, {
+                return ir(ir({}, e), {}, {
                     activeItemId: t.payload
                 });
             case "setQuery":
-                return or(or({}, e), {}, {
+                return ir(ir({}, e), {}, {
                     query: t.payload,
                     completion: null
                 });
             case "setCollections":
-                return or(or({}, e), {}, {
+                return ir(ir({}, e), {}, {
                     collections: t.payload
                 });
             case "setIsOpen":
-                return or(or({}, e), {}, {
+                return ir(ir({}, e), {}, {
                     isOpen: t.payload
                 });
             case "setStatus":
-                return or(or({}, e), {}, {
+                return ir(ir({}, e), {}, {
                     status: t.payload
                 });
             case "setContext":
-                return or(or({}, e), {}, {
-                    context: or(or({}, e.context), t.payload)
+                return ir(ir({}, e), {}, {
+                    context: ir(ir({}, e.context), t.payload)
                 });
             case "ArrowDown":
-                var n = or(or({}, e), {}, {
-                    activeItemId: t.payload.hasOwnProperty("nextActiveItemId") ? t.payload.nextActiveItemId : qt(1, e.activeItemId, tt(e), t.props.defaultActiveItemId)
+                var n = ir(ir({}, e), {}, {
+                    activeItemId: t.payload.hasOwnProperty("nextActiveItemId") ? t.payload.nextActiveItemId : Lt(1, e.activeItemId, nt(e), t.props.defaultActiveItemId)
                 });
-                return or(or({}, n), {}, {
-                    completion: tr({
+                return ir(ir({}, n), {}, {
+                    completion: nr({
                         state: n
                     })
                 });
             case "ArrowUp":
-                var r = or(or({}, e), {}, {
-                    activeItemId: qt(-1, e.activeItemId, tt(e), t.props.defaultActiveItemId)
+                var r = ir(ir({}, e), {}, {
+                    activeItemId: Lt(-1, e.activeItemId, nt(e), t.props.defaultActiveItemId)
                 });
-                return or(or({}, r), {}, {
-                    completion: tr({
+                return ir(ir({}, r), {}, {
+                    completion: nr({
                         state: r
                     })
                 });
             case "Escape":
-                return e.isOpen ? or(or({}, e), {}, {
+                return e.isOpen ? ir(ir({}, e), {}, {
                     activeItemId: null,
                     isOpen: !1,
                     completion: null
-                }) : or(or({}, e), {}, {
+                }) : ir(ir({}, e), {}, {
                     activeItemId: null,
                     query: "",
                     status: "idle",
                     collections: []
                 });
             case "submit":
-                return or(or({}, e), {}, {
+                return ir(ir({}, e), {}, {
                     activeItemId: null,
                     isOpen: !1,
                     status: "idle"
                 });
             case "reset":
-                return or(or({}, e), {}, {
+                return ir(ir({}, e), {}, {
                     activeItemId: !0 === t.props.openOnFocus ? t.props.defaultActiveItemId : null,
                     status: "idle",
                     query: ""
                 });
             case "focus":
-                return or(or({}, e), {}, {
+                return ir(ir({}, e), {}, {
                     activeItemId: t.props.defaultActiveItemId,
                     isOpen: (t.props.openOnFocus || Boolean(e.query)) && t.props.shouldPanelOpen({
                         state: e
                     })
                 });
             case "blur":
-                return t.props.debug ? e : or(or({}, e), {}, {
+                return t.props.debug ? e : ir(ir({}, e), {}, {
                     isOpen: !1,
                     activeItemId: null
                 });
             case "mouseleave":
-                return or(or({}, e), {}, {
+                return ir(ir({}, e), {}, {
                     activeItemId: t.props.defaultActiveItemId
                 });
             default:
                 return "The reducer action ".concat(JSON.stringify(t.type), " is not supported."), e
         }
     };
 
-    function ar(e) {
-        return ar = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function ur(e) {
+        return ur = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-        }, ar(e)
+        }, ur(e)
     }
 
-    function ur(e, t) {
+    function lr(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function lr(e) {
+    function sr(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? ur(Object(n), !0).forEach((function(t) {
-                sr(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ur(Object(n)).forEach((function(t) {
+            t % 2 ? lr(Object(n), !0).forEach((function(t) {
+                fr(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : lr(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function sr(e, t, n) {
+    function fr(e, t, n) {
         return (t = function(e) {
             var t = function(e, t) {
-                if ("object" !== ar(e) || null === e) return e;
+                if ("object" !== ur(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, t || "default");
-                    if ("object" !== ar(r)) return r;
+                    if ("object" !== ur(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
-            return "symbol" === ar(t) ? t : String(t)
+            return "symbol" === ur(t) ? t : String(t)
         }(t)) in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function fr(e) {
+    function pr(e) {
         var t = [],
-            n = rn(e, t),
-            r = zt(cr, n, (function(e) {
+            n = on(e, t),
+            r = Jt(ar, n, (function(e) {
                 var t = e.prevState,
                     r = e.state;
-                n.onStateChange(lr({
+                n.onStateChange(sr({
                     prevState: t,
                     state: r,
                     refresh: c,
                     navigator: n.navigator
                 }, o))
             })),
             o = function(e) {
@@ -3238,17 +3263,17 @@
                     },
                     setQuery: function(e) {
                         t.dispatch("setQuery", e)
                     },
                     setCollections: function(e) {
                         var n = 0,
                             r = e.map((function(e) {
-                                return Qt(Qt({}, e), {}, {
-                                    items: Xe(e.items).map((function(e) {
-                                        return Qt(Qt({}, e), {}, {
+                                return Zt(Zt({}, e), {}, {
+                                    items: et(e.items).map((function(e) {
+                                        return Zt(Zt({}, e), {}, {
                                             __autocomplete_id: n++
                                         })
                                     }))
                                 })
                             }));
                         t.dispatch("setCollections", r)
                     },
@@ -3261,23 +3286,23 @@
                     setContext: function(e) {
                         t.dispatch("setContext", e)
                     }
                 }
             }({
                 store: r
             }),
-            i = Qn(lr({
+            i = Zn(sr({
                 props: n,
                 refresh: c,
                 store: r,
                 navigator: n.navigator
             }, o));
 
         function c() {
-            return An(lr({
+            return Cn(sr({
                 event: new Event("input"),
                 nextState: {
                     isOpen: r.getState().isOpen
                 },
                 props: n,
                 navigator: n.navigator,
                 query: r.getState().query,
@@ -3285,19 +3310,19 @@
                 store: r
             }, o))
         }
         if (e.insights && !n.plugins.some((function(e) {
                 return "aa.algoliaInsightsPlugin" === e.name
             }))) {
             var a = "boolean" == typeof e.insights ? {} : e.insights;
-            n.plugins.push(xt(a))
+            n.plugins.push(Nt(a))
         }
         return n.plugins.forEach((function(e) {
                 var r;
-                return null === (r = e.subscribe) || void 0 === r ? void 0 : r.call(e, lr(lr({}, o), {}, {
+                return null === (r = e.subscribe) || void 0 === r ? void 0 : r.call(e, sr(sr({}, o), {}, {
                     navigator: n.navigator,
                     refresh: c,
                     onSelect: function(e) {
                         t.push({
                             onSelect: e
                         })
                     },
@@ -3320,26 +3345,26 @@
                     var i = o.document.createElement("meta"),
                         c = o.document.querySelector("head");
                     i.name = "algolia:metadata", setTimeout((function() {
                         i.content = JSON.stringify(r), c.appendChild(i)
                     }), 0)
                 }
             }({
-                metadata: er({
+                metadata: tr({
                     plugins: n.plugins,
                     options: e
                 }),
                 environment: n.environment
-            }), lr(lr({
+            }), sr(sr({
                 refresh: c,
                 navigator: n.navigator
             }, i), o)
     }
 
-    function pr(e) {
+    function mr(e) {
         var t = e.translations,
             n = (void 0 === t ? {} : t).searchByText,
             r = void 0 === n ? "Search by" : n;
         return Be.createElement("a", {
             href: "https://www.algolia.com/ref/docsearch/?utm_source=".concat(window.location.hostname, "&utm_medium=referral&utm_content=powered_by&utm_campaign=docsearch"),
             target: "_blank",
             rel: "noopener noreferrer"
@@ -3384,30 +3409,30 @@
             d: "M1314.05,104.73h-49.33c-48.36,0-90.91,25.48-115.75,64.1-11.79,18.34-19.6,39.64-22.11,62.59-.58,5.3-.88,10.68-.88,16.14s.31,11.15,.93,16.59c4.28,38.09,23.14,71.61,50.66,94.52,2.93,2.6,6.05,4.98,9.31,7.14,12.86,8.49,28.11,13.47,44.52,13.47h0c17.99,0,34.61-5.93,48.16-15.97,16.29-11.58,28.88-28.54,34.48-47.75v50.26h-.11v11.08c0,21.84-5.71,38.27-17.34,49.36-11.61,11.08-31.04,16.63-58.25,16.63-11.12,0-28.79-.59-46.6-2.41-2.83-.29-5.46,1.5-6.27,4.22l-12.78,43.11c-1.02,3.46,1.27,7.02,4.83,7.53,21.52,3.08,42.52,4.68,54.65,4.68,48.91,0,85.16-10.75,108.89-32.21,21.48-19.41,33.15-48.89,35.2-88.52V110.63c0-3.26-2.64-5.9-5.9-5.9h-56.32Zm0,64.1s.65,139.13,0,143.36c-12.08,9.77-27.11,13.59-43.49,14.7-.16,.01-.33,.03-.49,.04-1.12,.07-2.24,.1-3.36,.1-1.32,0-2.63-.03-3.94-.1-40.41-2.11-74.52-37.26-74.52-79.38,0-10.25,1.96-20.01,5.42-28.98,11.22-29.12,38.77-49.74,71.06-49.74h49.33Z"
         }), Be.createElement("path", {
             className: "cls-1",
             d: "M249.83,0C113.3,0,2,110.09,.03,246.16c-2,138.19,110.12,252.7,248.33,253.5,42.68,.25,83.79-10.19,120.3-30.03,3.56-1.93,4.11-6.83,1.08-9.51l-23.38-20.72c-4.75-4.21-11.51-5.4-17.36-2.92-25.48,10.84-53.17,16.38-81.71,16.03-111.68-1.37-201.91-94.29-200.13-205.96,1.76-110.26,92-199.41,202.67-199.41h202.69V407.41l-115-102.18c-3.72-3.31-9.42-2.66-12.42,1.31-18.46,24.44-48.53,39.64-81.93,37.34-46.33-3.2-83.87-40.5-87.34-86.81-4.15-55.24,39.63-101.52,94-101.52,49.18,0,89.68,37.85,93.91,85.95,.38,4.28,2.31,8.27,5.52,11.12l29.95,26.55c3.4,3.01,8.79,1.17,9.63-3.3,2.16-11.55,2.92-23.58,2.07-35.92-4.82-70.34-61.8-126.93-132.17-131.26-80.68-4.97-148.13,58.14-150.27,137.25-2.09,77.1,61.08,143.56,138.19,145.26,32.19,.71,62.03-9.41,86.14-26.95l150.26,133.2c6.44,5.71,16.61,1.14,16.61-7.47V9.48C499.66,4.25,495.42,0,490.18,0H249.83Z"
         })))
     }
 
-    function mr(e) {
+    function vr(e) {
         return Be.createElement("svg", {
             width: "15",
             height: "15",
             "aria-label": e.ariaLabel,
             role: "img"
         }, Be.createElement("g", {
             fill: "none",
             stroke: "currentColor",
             strokeLinecap: "round",
             strokeLinejoin: "round",
             strokeWidth: "1.2"
         }, e.children))
     }
 
-    function vr(e) {
+    function dr(e) {
         var t = e.translations,
             n = void 0 === t ? {} : t,
             r = n.selectText,
             o = void 0 === r ? "to select" : r,
             i = n.selectKeyAriaLabel,
             c = void 0 === i ? "Enter key" : i,
             a = n.navigateText,
@@ -3420,62 +3445,62 @@
             v = void 0 === m ? "to close" : m,
             d = n.closeKeyAriaLabel,
             h = void 0 === d ? "Escape key" : d,
             y = n.searchByText,
             b = void 0 === y ? "Search by" : y;
         return Be.createElement(Be.Fragment, null, Be.createElement("div", {
             className: "DocSearch-Logo"
-        }, Be.createElement(pr, {
+        }, Be.createElement(mr, {
             translations: {
                 searchByText: b
             }
         })), Be.createElement("ul", {
             className: "DocSearch-Commands"
         }, Be.createElement("li", null, Be.createElement("kbd", {
             className: "DocSearch-Commands-Key"
-        }, Be.createElement(mr, {
+        }, Be.createElement(vr, {
             ariaLabel: c
         }, Be.createElement("path", {
             d: "M12 3.53088v3c0 1-1 2-2 2H4M7 11.53088l-3-3 3-3"
         }))), Be.createElement("span", {
             className: "DocSearch-Label"
         }, o)), Be.createElement("li", null, Be.createElement("kbd", {
             className: "DocSearch-Commands-Key"
-        }, Be.createElement(mr, {
+        }, Be.createElement(vr, {
             ariaLabel: p
         }, Be.createElement("path", {
             d: "M7.5 3.5v8M10.5 8.5l-3 3-3-3"
         }))), Be.createElement("kbd", {
             className: "DocSearch-Commands-Key"
-        }, Be.createElement(mr, {
+        }, Be.createElement(vr, {
             ariaLabel: s
         }, Be.createElement("path", {
             d: "M7.5 11.5v-8M10.5 6.5l-3-3-3 3"
         }))), Be.createElement("span", {
             className: "DocSearch-Label"
         }, u)), Be.createElement("li", null, Be.createElement("kbd", {
             className: "DocSearch-Commands-Key"
-        }, Be.createElement(mr, {
+        }, Be.createElement(vr, {
             ariaLabel: h
         }, Be.createElement("path", {
             d: "M13.6167 8.936c-.1065.3583-.6883.962-1.4875.962-.7993 0-1.653-.9165-1.653-2.1258v-.5678c0-1.2548.7896-2.1016 1.653-2.1016.8634 0 1.3601.4778 1.4875 1.0724M9 6c-.1352-.4735-.7506-.9219-1.46-.8972-.7092.0246-1.344.57-1.344 1.2166s.4198.8812 1.3445.9805C8.465 7.3992 8.968 7.9337 9 8.5c.032.5663-.454 1.398-1.4595 1.398C6.6593 9.898 6 9 5.963 8.4851m-1.4748.5368c-.2635.5941-.8099.876-1.5443.876s-1.7073-.6248-1.7073-2.204v-.4603c0-1.0416.721-2.131 1.7073-2.131.9864 0 1.6425 1.031 1.5443 2.2492h-2.956"
         }))), Be.createElement("span", {
             className: "DocSearch-Label"
         }, v))))
     }
 
-    function dr(e) {
+    function hr(e) {
         var t = e.hit,
             n = e.children;
         return Be.createElement("a", {
             href: t.url
         }, n)
     }
 
-    function hr() {
+    function yr() {
         return Be.createElement("svg", {
             viewBox: "0 0 38 38",
             stroke: "currentColor",
             strokeOpacity: ".5"
         }, Be.createElement("g", {
             fill: "none",
             fillRule: "evenodd"
@@ -3495,15 +3520,15 @@
             from: "0 18 18",
             to: "360 18 18",
             dur: "1s",
             repeatCount: "indefinite"
         })))))
     }
 
-    function yr() {
+    function br() {
         return Be.createElement("svg", {
             width: "20",
             height: "20",
             viewBox: "0 0 20 20"
         }, Be.createElement("g", {
             stroke: "currentColor",
             fill: "none",
@@ -3513,30 +3538,30 @@
         }, Be.createElement("path", {
             d: "M3.18 6.6a8.23 8.23 0 1112.93 9.94h0a8.23 8.23 0 01-11.63 0"
         }), Be.createElement("path", {
             d: "M6.44 7.25H2.55V3.36M10.45 6v5.6M10.45 11.6L13 13"
         })))
     }
 
-    function br() {
+    function gr() {
         return Be.createElement("svg", {
             width: "20",
             height: "20",
             viewBox: "0 0 20 20"
         }, Be.createElement("path", {
             d: "M10 10l5.09-5.09L10 10l5.09 5.09L10 10zm0 0L4.91 4.91 10 10l-5.09 5.09L10 10z",
             stroke: "currentColor",
             fill: "none",
             fillRule: "evenodd",
             strokeLinecap: "round",
             strokeLinejoin: "round"
         }))
     }
 
-    function gr() {
+    function _r() {
         return Be.createElement("svg", {
             className: "DocSearch-Hit-Select-Icon",
             width: "20",
             height: "20",
             viewBox: "0 0 20 20"
         }, Be.createElement("g", {
             stroke: "currentColor",
@@ -3546,40 +3571,40 @@
             strokeLinejoin: "round"
         }, Be.createElement("path", {
             d: "M18 3v4c0 2-2 4-4 4H2"
         }), Be.createElement("path", {
             d: "M8 17l-6-6 6-6"
         })))
     }
-    var _r = function() {
+    var Or = function() {
         return Be.createElement("svg", {
             width: "20",
             height: "20",
             viewBox: "0 0 20 20"
         }, Be.createElement("path", {
             d: "M17 6v12c0 .52-.2 1-1 1H4c-.7 0-1-.33-1-1V2c0-.55.42-1 1-1h8l5 5zM14 8h-3.13c-.51 0-.87-.34-.87-.87V4",
             stroke: "currentColor",
             fill: "none",
             fillRule: "evenodd",
             strokeLinejoin: "round"
         }))
     };
 
-    function Or(e) {
+    function Sr(e) {
         switch (e.type) {
             case "lvl1":
-                return Be.createElement(_r, null);
+                return Be.createElement(Or, null);
             case "content":
                 return Be.createElement(jr, null);
             default:
-                return Be.createElement(Sr, null)
+                return Be.createElement(wr, null)
         }
     }
 
-    function Sr() {
+    function wr() {
         return Be.createElement("svg", {
             width: "20",
             height: "20",
             viewBox: "0 0 20 20"
         }, Be.createElement("path", {
             d: "M13 13h4-4V8H7v5h6v4-4H7V8H3h4V3v5h6V3v5h4-4v5zm-6 0v4-4H3h4z",
             stroke: "currentColor",
@@ -3600,101 +3625,101 @@
             stroke: "currentColor",
             fill: "none",
             fillRule: "evenodd",
             strokeLinejoin: "round"
         }))
     }
 
-    function wr() {
+    function Er() {
         return Be.createElement("svg", {
             width: "20",
             height: "20",
             viewBox: "0 0 20 20"
         }, Be.createElement("path", {
             d: "M10 14.2L5 17l1-5.6-4-4 5.5-.7 2.5-5 2.5 5 5.6.8-4 4 .9 5.5z",
             stroke: "currentColor",
             fill: "none",
             fillRule: "evenodd",
             strokeLinejoin: "round"
         }))
     }
 
-    function Er() {
+    function Pr() {
         return Be.createElement("svg", {
             width: "40",
             height: "40",
             viewBox: "0 0 20 20",
             fill: "none",
             fillRule: "evenodd",
             stroke: "currentColor",
             strokeLinecap: "round",
             strokeLinejoin: "round"
         }, Be.createElement("path", {
             d: "M19 4.8a16 16 0 00-2-1.2m-3.3-1.2A16 16 0 001.1 4.7M16.7 8a12 12 0 00-2.8-1.4M10 6a12 12 0 00-6.7 2M12.3 14.7a4 4 0 00-4.5 0M14.5 11.4A8 8 0 0010 10M3 16L18 2M10 18h0"
         }))
     }
 
-    function Pr() {
+    function Ir() {
         return Be.createElement("svg", {
             width: "40",
             height: "40",
             viewBox: "0 0 20 20",
             fill: "none",
             fillRule: "evenodd",
             stroke: "currentColor",
             strokeLinecap: "round",
             strokeLinejoin: "round"
         }, Be.createElement("path", {
             d: "M15.5 4.8c2 3 1.7 7-1 9.7h0l4.3 4.3-4.3-4.3a7.8 7.8 0 01-9.8 1m-2.2-2.2A7.8 7.8 0 0113.2 2.4M2 18L18 2"
         }))
     }
 
-    function Ir(e) {
+    function Dr(e) {
         var t = e.translations,
             n = void 0 === t ? {} : t,
             r = n.titleText,
             o = void 0 === r ? "Unable to fetch results" : r,
             i = n.helpText,
             c = void 0 === i ? "You might want to check your network connection." : i;
         return Be.createElement("div", {
             className: "DocSearch-ErrorScreen"
         }, Be.createElement("div", {
             className: "DocSearch-Screen-Icon"
-        }, Be.createElement(Er, null)), Be.createElement("p", {
+        }, Be.createElement(Pr, null)), Be.createElement("p", {
             className: "DocSearch-Title"
         }, o), Be.createElement("p", {
             className: "DocSearch-Help"
         }, c))
     }
-    var Dr = ["translations"];
+    var kr = ["translations"];
 
-    function kr(e) {
+    function Ar(e) {
         return function(e) {
-            if (Array.isArray(e)) return Ar(e)
+            if (Array.isArray(e)) return Cr(e)
         }(e) || function(e) {
             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
         }(e) || function(e, t) {
             if (!e) return;
-            if ("string" == typeof e) return Ar(e, t);
+            if ("string" == typeof e) return Cr(e, t);
             var n = Object.prototype.toString.call(e).slice(8, -1);
             "Object" === n && e.constructor && (n = e.constructor.name);
             if ("Map" === n || "Set" === n) return Array.from(e);
-            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Ar(e, t)
+            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Cr(e, t)
         }(e) || function() {
             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function Ar(e, t) {
+    function Cr(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function Cr(e, t) {
+    function xr(e, t) {
         if (null == e) return {};
         var n, r, o = function(e, t) {
             if (null == e) return {};
             var n, r, o = {},
                 i = Object.keys(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
             return o
@@ -3702,39 +3727,39 @@
         if (Object.getOwnPropertySymbols) {
             var i = Object.getOwnPropertySymbols(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
         }
         return o
     }
 
-    function xr(e) {
+    function Nr(e) {
         var t = e.translations,
             n = void 0 === t ? {} : t,
-            r = Cr(e, Dr),
+            r = xr(e, kr),
             o = n.noResultsText,
             i = void 0 === o ? "No results for" : o,
             c = n.suggestedQueryText,
             a = void 0 === c ? "Try searching for" : c,
             u = n.reportMissingResultsText,
             l = void 0 === u ? "Believe this query should return results?" : u,
             s = n.reportMissingResultsLinkText,
             f = void 0 === s ? "Let us know." : s,
             p = r.state.context.searchSuggestions;
         return Be.createElement("div", {
             className: "DocSearch-NoResults"
         }, Be.createElement("div", {
             className: "DocSearch-Screen-Icon"
-        }, Be.createElement(Pr, null)), Be.createElement("p", {
+        }, Be.createElement(Ir, null)), Be.createElement("p", {
             className: "DocSearch-Title"
         }, i, ' "', Be.createElement("strong", null, r.state.query), '"'), p && p.length > 0 && Be.createElement("div", {
             className: "DocSearch-NoResults-Prefill-List"
         }, Be.createElement("p", {
             className: "DocSearch-Help"
         }, a, ":"), Be.createElement("ul", null, p.slice(0, 3).reduce((function(e, t) {
-            return [].concat(kr(e), [Be.createElement("li", {
+            return [].concat(Ar(e), [Be.createElement("li", {
                 key: t
             }, Be.createElement("button", {
                 className: "DocSearch-Prefill",
                 key: t,
                 type: "button",
                 onClick: function() {
                     r.setQuery(t.toLowerCase() + " "), r.refresh(), r.inputRef.current.focus()
@@ -3746,49 +3771,49 @@
             href: r.getMissingResultsUrl({
                 query: r.state.query
             }),
             target: "_blank",
             rel: "noopener noreferrer"
         }, f)))
     }
-    var Nr = ["hit", "attribute", "tagName"];
+    var Tr = ["hit", "attribute", "tagName"];
 
-    function Tr(e, t) {
+    function Rr(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Rr(e) {
+    function qr(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Tr(Object(n), !0).forEach((function(t) {
-                qr(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Tr(Object(n)).forEach((function(t) {
+            t % 2 ? Rr(Object(n), !0).forEach((function(t) {
+                Lr(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Rr(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function qr(e, t, n) {
+    function Lr(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function Lr(e, t) {
+    function Mr(e, t) {
         if (null == e) return {};
         var n, r, o = function(e, t) {
             if (null == e) return {};
             var n, r, o = {},
                 i = Object.keys(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
             return o
@@ -3796,32 +3821,32 @@
         if (Object.getOwnPropertySymbols) {
             var i = Object.getOwnPropertySymbols(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
         }
         return o
     }
 
-    function Mr(e, t) {
+    function Hr(e, t) {
         return t.split(".").reduce((function(e, t) {
             return null != e && e[t] ? e[t] : null
         }), e)
     }
 
-    function Hr(e) {
+    function Ur(e) {
         var t = e.hit,
             n = e.attribute,
             r = e.tagName;
-        return _(void 0 === r ? "span" : r, Rr(Rr({}, Lr(e, Nr)), {}, {
+        return _(void 0 === r ? "span" : r, qr(qr({}, Mr(e, Tr)), {}, {
             dangerouslySetInnerHTML: {
-                __html: Mr(t, "_snippetResult.".concat(n, ".value")) || Mr(t, n)
+                __html: Hr(t, "_snippetResult.".concat(n, ".value")) || Hr(t, n)
             }
         }))
     }
 
-    function Ur(e, t) {
+    function Fr(e, t) {
         return function(e) {
             if (Array.isArray(e)) return e
         }(e) || function(e, t) {
             var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
             if (null == n) return;
             var r, o, i = [],
                 c = !0,
@@ -3836,47 +3861,47 @@
                 } finally {
                     if (a) throw o
                 }
             }
             return i
         }(e, t) || function(e, t) {
             if (!e) return;
-            if ("string" == typeof e) return Fr(e, t);
+            if ("string" == typeof e) return Br(e, t);
             var n = Object.prototype.toString.call(e).slice(8, -1);
             "Object" === n && e.constructor && (n = e.constructor.name);
             if ("Map" === n || "Set" === n) return Array.from(e);
-            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Fr(e, t)
+            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Br(e, t)
         }(e, t) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function Fr(e, t) {
+    function Br(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function Br() {
-        return Br = Object.assign || function(e) {
+    function Vr() {
+        return Vr = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, Br.apply(this, arguments)
+        }, Vr.apply(this, arguments)
     }
 
-    function Vr(e) {
+    function Kr(e) {
         return e.collection && 0 !== e.collection.items.length ? Be.createElement("section", {
             className: "DocSearch-Hits"
         }, Be.createElement("div", {
             className: "DocSearch-Hit-source"
         }, e.title), Be.createElement("ul", e.getListProps(), e.collection.items.map((function(t, n) {
-            return Be.createElement(Wr, Br({
+            return Be.createElement(Wr, Vr({
                 key: [e.title, t.objectID].join(":"),
                 item: t,
                 index: n
             }, e))
         })))) : null
     }
 
@@ -3885,23 +3910,23 @@
             n = e.index,
             r = e.renderIcon,
             o = e.renderAction,
             i = e.getItemProps,
             c = e.onItemClick,
             a = e.collection,
             u = e.hitComponent,
-            l = Ur(Be.useState(!1), 2),
+            l = Fr(Be.useState(!1), 2),
             s = l[0],
             f = l[1],
-            p = Ur(Be.useState(!1), 2),
+            p = Fr(Be.useState(!1), 2),
             m = p[0],
             v = p[1],
             d = Be.useRef(null),
             h = u;
-        return Be.createElement("li", Br({
+        return Be.createElement("li", Vr({
             className: ["DocSearch-Hit", t.__docsearch_parent && "DocSearch-Hit--Child", s && "DocSearch-Hit--deleting", m && "DocSearch-Hit--favoriting"].filter(Boolean).join(" "),
             onTransitionEnd: function() {
                 d.current && d.current()
             }
         }, i({
             item: t,
             source: a.source,
@@ -3913,96 +3938,96 @@
         }, Be.createElement("div", {
             className: "DocSearch-Hit-Container"
         }, r({
             item: t,
             index: n
         }), t.hierarchy[t.type] && "lvl1" === t.type && Be.createElement("div", {
             className: "DocSearch-Hit-content-wrapper"
-        }, Be.createElement(Hr, {
+        }, Be.createElement(Ur, {
             className: "DocSearch-Hit-title",
             hit: t,
             attribute: "hierarchy.lvl1"
-        }), t.content && Be.createElement(Hr, {
+        }), t.content && Be.createElement(Ur, {
             className: "DocSearch-Hit-path",
             hit: t,
             attribute: "content"
         })), t.hierarchy[t.type] && ("lvl2" === t.type || "lvl3" === t.type || "lvl4" === t.type || "lvl5" === t.type || "lvl6" === t.type) && Be.createElement("div", {
             className: "DocSearch-Hit-content-wrapper"
-        }, Be.createElement(Hr, {
+        }, Be.createElement(Ur, {
             className: "DocSearch-Hit-title",
             hit: t,
             attribute: "hierarchy.".concat(t.type)
-        }), Be.createElement(Hr, {
+        }), Be.createElement(Ur, {
             className: "DocSearch-Hit-path",
             hit: t,
             attribute: "hierarchy.lvl1"
         })), "content" === t.type && Be.createElement("div", {
             className: "DocSearch-Hit-content-wrapper"
-        }, Be.createElement(Hr, {
+        }, Be.createElement(Ur, {
             className: "DocSearch-Hit-title",
             hit: t,
             attribute: "content"
-        }), Be.createElement(Hr, {
+        }), Be.createElement(Ur, {
             className: "DocSearch-Hit-path",
             hit: t,
             attribute: "hierarchy.lvl1"
         })), o({
             item: t,
             runDeleteTransition: function(e) {
                 f(!0), d.current = e
             },
             runFavoriteTransition: function(e) {
                 v(!0), d.current = e
             }
         }))))
     }
 
-    function Kr(e, t, n) {
+    function zr(e, t, n) {
         return e.reduce((function(e, r) {
             var o = t(r);
             return e.hasOwnProperty(o) || (e[o] = []), e[o].length < (n || 5) && e[o].push(r), e
         }), {})
     }
 
-    function zr(e) {
+    function Jr(e) {
         return e
     }
 
-    function Jr(e) {
+    function $r(e) {
         return 1 === e.button || e.altKey || e.ctrlKey || e.metaKey || e.shiftKey
     }
 
-    function $r() {}
-    var Qr = /(<mark>|<\/mark>)/g,
-        Zr = RegExp(Qr.source);
+    function Qr() {}
+    var Zr = /(<mark>|<\/mark>)/g,
+        Yr = RegExp(Zr.source);
 
-    function Yr(e) {
+    function Gr(e) {
         var t, n, r = e;
         if (!r.__docsearch_parent && !e._highlightResult) return e.hierarchy.lvl0;
         var o = ((r.__docsearch_parent ? null === (t = r.__docsearch_parent) || void 0 === t || null === (t = t._highlightResult) || void 0 === t || null === (t = t.hierarchy) || void 0 === t ? void 0 : t.lvl0 : null === (n = e._highlightResult) || void 0 === n || null === (n = n.hierarchy) || void 0 === n ? void 0 : n.lvl0) || {}).value;
-        return o && Zr.test(o) ? o.replace(Qr, "") : o
+        return o && Yr.test(o) ? o.replace(Zr, "") : o
     }
 
-    function Gr() {
-        return Gr = Object.assign || function(e) {
+    function Xr() {
+        return Xr = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, Gr.apply(this, arguments)
+        }, Xr.apply(this, arguments)
     }
 
-    function Xr(e) {
+    function eo(e) {
         return Be.createElement("div", {
             className: "DocSearch-Dropdown-Container"
         }, e.state.collections.map((function(t) {
             if (0 === t.items.length) return null;
-            var n = Yr(t.items[0]);
-            return Be.createElement(Vr, Gr({}, e, {
+            var n = Gr(t.items[0]);
+            return Be.createElement(Kr, Xr({}, e, {
                 key: t.source.sourceId,
                 title: n,
                 collection: t,
                 renderIcon: function(e) {
                     var n, r = e.item,
                         o = e.index;
                     return Be.createElement(Be.Fragment, null, r.__docsearch_parent && Be.createElement("svg", {
@@ -4016,43 +4041,43 @@
                         strokeLinejoin: "round"
                     }, r.__docsearch_parent !== (null === (n = t.items[o + 1]) || void 0 === n ? void 0 : n.__docsearch_parent) ? Be.createElement("path", {
                         d: "M8 6v21M20 27H8.3"
                     }) : Be.createElement("path", {
                         d: "M8 6v42M20 27H8.3"
                     }))), Be.createElement("div", {
                         className: "DocSearch-Hit-icon"
-                    }, Be.createElement(Or, {
+                    }, Be.createElement(Sr, {
                         type: r.type
                     })))
                 },
                 renderAction: function() {
                     return Be.createElement("div", {
                         className: "DocSearch-Hit-action"
-                    }, Be.createElement(gr, null))
+                    }, Be.createElement(_r, null))
                 }
             }))
         })), e.resultsFooterComponent && Be.createElement("section", {
             className: "DocSearch-HitsFooter"
         }, Be.createElement(e.resultsFooterComponent, {
             state: e.state
         })))
     }
-    var eo = ["translations"];
+    var to = ["translations"];
 
-    function to() {
-        return to = Object.assign || function(e) {
+    function no() {
+        return no = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, to.apply(this, arguments)
+        }, no.apply(this, arguments)
     }
 
-    function no(e, t) {
+    function ro(e, t) {
         if (null == e) return {};
         var n, r, o = function(e, t) {
             if (null == e) return {};
             var n, r, o = {},
                 i = Object.keys(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
             return o
@@ -4060,18 +4085,18 @@
         if (Object.getOwnPropertySymbols) {
             var i = Object.getOwnPropertySymbols(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
         }
         return o
     }
 
-    function ro(e) {
+    function oo(e) {
         var t = e.translations,
             n = void 0 === t ? {} : t,
-            r = no(e, eo),
+            r = ro(e, to),
             o = n.recentSearchesTitle,
             i = void 0 === o ? "Recent" : o,
             c = n.noRecentSearchesText,
             a = void 0 === c ? "No recent searches" : c,
             u = n.saveRecentSearchButtonTitle,
             l = void 0 === u ? "Save this search" : u,
             s = n.removeRecentSearchButtonTitle,
@@ -4082,21 +4107,21 @@
             d = void 0 === v ? "Remove this search from favorites" : v;
         return "idle" === r.state.status && !1 === r.hasCollections ? r.disableUserPersonalization ? null : Be.createElement("div", {
             className: "DocSearch-StartScreen"
         }, Be.createElement("p", {
             className: "DocSearch-Help"
         }, a)) : !1 === r.hasCollections ? null : Be.createElement("div", {
             className: "DocSearch-Dropdown-Container"
-        }, Be.createElement(Vr, to({}, r, {
+        }, Be.createElement(Kr, no({}, r, {
             title: i,
             collection: r.state.collections[0],
             renderIcon: function() {
                 return Be.createElement("div", {
                     className: "DocSearch-Hit-icon"
-                }, Be.createElement(yr, null))
+                }, Be.createElement(br, null))
             },
             renderAction: function(e) {
                 var t = e.item,
                     n = e.runFavoriteTransition,
                     o = e.runDeleteTransition;
                 return Be.createElement(Be.Fragment, null, Be.createElement("div", {
                     className: "DocSearch-Hit-action"
@@ -4105,34 +4130,34 @@
                     title: l,
                     type: "submit",
                     onClick: function(e) {
                         e.preventDefault(), e.stopPropagation(), n((function() {
                             r.favoriteSearches.add(t), r.recentSearches.remove(t), r.refresh()
                         }))
                     }
-                }, Be.createElement(wr, null))), Be.createElement("div", {
+                }, Be.createElement(Er, null))), Be.createElement("div", {
                     className: "DocSearch-Hit-action"
                 }, Be.createElement("button", {
                     className: "DocSearch-Hit-action-button",
                     title: f,
                     type: "submit",
                     onClick: function(e) {
                         e.preventDefault(), e.stopPropagation(), o((function() {
                             r.recentSearches.remove(t), r.refresh()
                         }))
                     }
-                }, Be.createElement(br, null))))
+                }, Be.createElement(gr, null))))
             }
-        })), Be.createElement(Vr, to({}, r, {
+        })), Be.createElement(Kr, no({}, r, {
             title: m,
             collection: r.state.collections[1],
             renderIcon: function() {
                 return Be.createElement("div", {
                     className: "DocSearch-Hit-icon"
-                }, Be.createElement(wr, null))
+                }, Be.createElement(Er, null))
             },
             renderAction: function(e) {
                 var t = e.item,
                     n = e.runDeleteTransition;
                 return Be.createElement("div", {
                     className: "DocSearch-Hit-action"
                 }, Be.createElement("button", {
@@ -4140,77 +4165,77 @@
                     title: d,
                     type: "submit",
                     onClick: function(e) {
                         e.preventDefault(), e.stopPropagation(), n((function() {
                             r.favoriteSearches.remove(t), r.refresh()
                         }))
                     }
-                }, Be.createElement(br, null)))
+                }, Be.createElement(gr, null)))
             }
         })))
     }
-    var oo = ["translations"];
+    var io = ["translations"];
 
-    function io() {
-        return io = Object.assign || function(e) {
+    function co() {
+        return co = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, io.apply(this, arguments)
+        }, co.apply(this, arguments)
     }
 
-    function co(e, t) {
+    function ao(e, t) {
         if (null == e) return {};
         var n, r, o = function(e, t) {
             if (null == e) return {};
             var n, r, o = {},
                 i = Object.keys(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
             return o
         }(e, t);
         if (Object.getOwnPropertySymbols) {
             var i = Object.getOwnPropertySymbols(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
         }
         return o
     }
-    var ao = Be.memo((function(e) {
+    var uo = Be.memo((function(e) {
             var t = e.translations,
                 n = void 0 === t ? {} : t,
-                r = co(e, oo);
-            if ("error" === r.state.status) return Be.createElement(Ir, {
+                r = ao(e, io);
+            if ("error" === r.state.status) return Be.createElement(Dr, {
                 translations: null == n ? void 0 : n.errorScreen
             });
             var o = r.state.collections.some((function(e) {
                 return e.items.length > 0
             }));
-            return r.state.query ? !1 === o ? Be.createElement(xr, io({}, r, {
+            return r.state.query ? !1 === o ? Be.createElement(Nr, co({}, r, {
                 translations: null == n ? void 0 : n.noResultsScreen
-            })) : Be.createElement(Xr, r) : Be.createElement(ro, io({}, r, {
+            })) : Be.createElement(eo, r) : Be.createElement(oo, co({}, r, {
                 hasCollections: o,
                 translations: null == n ? void 0 : n.startScreen
             }))
         }), (function(e, t) {
             return "loading" === t.state.status || "stalled" === t.state.status
         })),
-        uo = ["translations"];
+        lo = ["translations"];
 
-    function lo() {
-        return lo = Object.assign || function(e) {
+    function so() {
+        return so = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, lo.apply(this, arguments)
+        }, so.apply(this, arguments)
     }
 
-    function so(e, t) {
+    function fo(e, t) {
         if (null == e) return {};
         var n, r, o = function(e, t) {
             if (null == e) return {};
             var n, r, o = {},
                 i = Object.keys(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
             return o
@@ -4218,66 +4243,70 @@
         if (Object.getOwnPropertySymbols) {
             var i = Object.getOwnPropertySymbols(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
         }
         return o
     }
 
-    function fo(e) {
+    function po(e) {
         var t = e.translations,
             n = void 0 === t ? {} : t,
-            r = so(e, uo),
+            r = fo(e, lo),
             o = n.resetButtonTitle,
             i = void 0 === o ? "Clear the query" : o,
             c = n.resetButtonAriaLabel,
             a = void 0 === c ? "Clear the query" : c,
             u = n.cancelButtonText,
             l = void 0 === u ? "Cancel" : u,
             s = n.cancelButtonAriaLabel,
             f = void 0 === s ? "Cancel" : s,
-            p = r.getFormProps({
+            p = n.searchInputLabel,
+            m = void 0 === p ? "Search" : p,
+            v = r.getFormProps({
                 inputElement: r.inputRef.current
             }).onReset;
         return Be.useEffect((function() {
             r.autoFocus && r.inputRef.current && r.inputRef.current.focus()
         }), [r.autoFocus, r.inputRef]), Be.useEffect((function() {
             r.isFromSelection && r.inputRef.current && r.inputRef.current.select()
         }), [r.isFromSelection, r.inputRef]), Be.createElement(Be.Fragment, null, Be.createElement("form", {
             className: "DocSearch-Form",
             onSubmit: function(e) {
                 e.preventDefault()
             },
-            onReset: p
-        }, Be.createElement("label", lo({
+            onReset: v
+        }, Be.createElement("label", so({
             className: "DocSearch-MagnifierLabel"
-        }, r.getLabelProps()), Be.createElement(We, null)), Be.createElement("div", {
+        }, r.getLabelProps()), Be.createElement(Ke, null), Be.createElement("span", {
+            className: "DocSearch-VisuallyHiddenForAccessibility"
+        }, m)), Be.createElement("div", {
             className: "DocSearch-LoadingIndicator"
-        }, Be.createElement(hr, null)), Be.createElement("input", lo({
+        }, Be.createElement(yr, null)), Be.createElement("input", so({
             className: "DocSearch-Input",
             ref: r.inputRef
         }, r.getInputProps({
             inputElement: r.inputRef.current,
             autoFocus: r.autoFocus,
             maxLength: 64
         }))), Be.createElement("button", {
             type: "reset",
             title: i,
             className: "DocSearch-Reset",
             "aria-label": a,
             hidden: !r.state.query
-        }, Be.createElement(br, null))), Be.createElement("button", {
+        }, Be.createElement(gr, null))), Be.createElement("button", {
             className: "DocSearch-Cancel",
             type: "reset",
             "aria-label": f,
             onClick: r.onClose
         }, l))
     }
-    var po = ["_highlightResult", "_snippetResult"];
+    var mo = ["_highlightResult", "_snippetResult"];
 
-    function mo(e, t) {
+    function vo(e, t) {
         if (null == e) return {};
         var n, r, o = function(e, t) {
             if (null == e) return {};
             var n, r, o = {},
                 i = Object.keys(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
             return o
@@ -4285,15 +4314,15 @@
         if (Object.getOwnPropertySymbols) {
             var i = Object.getOwnPropertySymbols(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
         }
         return o
     }
 
-    function vo(e) {
+    function ho(e) {
         return !1 === function() {
             var e = "__TEST_KEY__";
             try {
                 return localStorage.setItem(e, ""), localStorage.removeItem(e), !0
             } catch (e) {
                 return !1
             }
@@ -4309,24 +4338,24 @@
             getItem: function() {
                 var t = window.localStorage.getItem(e);
                 return t ? JSON.parse(t) : []
             }
         }
     }
 
-    function ho(e) {
+    function yo(e) {
         var t = e.key,
             n = e.limit,
             r = void 0 === n ? 5 : n,
-            o = vo(t),
+            o = ho(t),
             i = o.getItem().slice(0, r);
         return {
             add: function(e) {
                 var t = e,
-                    n = (t._highlightResult, t._snippetResult, mo(t, po)),
+                    n = (t._highlightResult, t._snippetResult, vo(t, mo)),
                     c = i.findIndex((function(e) {
                         return e.objectID === n.objectID
                     }));
                 c > -1 && i.splice(c, 1), i.unshift(n), i = i.slice(0, r), o.setItem(i)
             },
             remove: function(e) {
                 i = i.filter((function(t) {
@@ -4334,17 +4363,17 @@
                 })), o.setItem(i)
             },
             getAll: function() {
                 return i
             }
         }
     }
-    var yo = ["facetName", "facetQuery"];
+    var bo = ["facetName", "facetQuery"];
 
-    function bo(e) {
+    function go(e) {
         var t, n = "algoliasearch-client-js-".concat(e.key),
             r = function() {
                 return void 0 === t && (t = e.localStorage || window.localStorage), t
             },
             o = function() {
                 return JSON.parse(r().getItem(n) || "{}")
             },
@@ -4407,15 +4436,15 @@
                 return Promise.resolve().then((function() {
                     r().removeItem(n)
                 }))
             }
         }
     }
 
-    function go(e) {
+    function _o(e) {
         var t = a(e.caches),
             n = t.shift();
         return void 0 === n ? {
             get: function(e, t) {
                 var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {
                     miss: function() {
                         return Promise.resolve()
@@ -4440,44 +4469,44 @@
             get: function(e, r) {
                 var o = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {
                     miss: function() {
                         return Promise.resolve()
                     }
                 };
                 return n.get(e, r, o).catch((function() {
-                    return go({
+                    return _o({
                         caches: t
                     }).get(e, r, o)
                 }))
             },
             set: function(e, r) {
                 return n.set(e, r).catch((function() {
-                    return go({
+                    return _o({
                         caches: t
                     }).set(e, r)
                 }))
             },
             delete: function(e) {
                 return n.delete(e).catch((function() {
-                    return go({
+                    return _o({
                         caches: t
                     }).delete(e)
                 }))
             },
             clear: function() {
                 return n.clear().catch((function() {
-                    return go({
+                    return _o({
                         caches: t
                     }).clear()
                 }))
             }
         }
     }
 
-    function _o() {
+    function Oo() {
         var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {
                 serializable: !0
             },
             t = {};
         return {
             get: function(n, r) {
                 var o = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {
@@ -4505,148 +4534,148 @@
             },
             clear: function() {
                 return t = {}, Promise.resolve()
             }
         }
     }
 
-    function Oo(e) {
+    function So(e) {
         for (var t = e.length - 1; t > 0; t--) {
             var n = Math.floor(Math.random() * (t + 1)),
                 r = e[t];
             e[t] = e[n], e[n] = r
         }
         return e
     }
 
-    function So(e, t) {
+    function wo(e, t) {
         return t ? (Object.keys(t).forEach((function(n) {
             e[n] = t[n](e)
         })), e) : e
     }
 
     function jo(e) {
         for (var t = arguments.length, n = new Array(t > 1 ? t - 1 : 0), r = 1; r < t; r++) n[r - 1] = arguments[r];
         var o = 0;
         return e.replace(/%s/g, (function() {
             return encodeURIComponent(n[o++])
         }))
     }
-    var wo = "4.19.1",
-        Eo = {
+    var Eo = "4.19.1",
+        Po = {
             WithinQueryParameters: 0,
             WithinHeaders: 1
         };
 
-    function Po(e, t) {
+    function Io(e, t) {
         var n = e || {},
             r = n.data || {};
         return Object.keys(n).forEach((function(e) {
             -1 === ["timeout", "headers", "queryParameters", "data", "cacheable"].indexOf(e) && (r[e] = n[e])
         })), {
             data: Object.entries(r).length > 0 ? r : void 0,
             timeout: n.timeout || t,
             headers: n.headers || {},
             queryParameters: n.queryParameters || {},
             cacheable: n.cacheable
         }
     }
-    var Io = {
+    var Do = {
             Read: 1,
             Write: 2,
             Any: 3
         },
-        Do = 1,
-        ko = 2,
-        Ao = 3,
-        Co = 12e4;
+        ko = 1,
+        Ao = 2,
+        Co = 3,
+        xo = 12e4;
 
-    function xo(e) {
-        var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Do;
+    function No(e) {
+        var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : ko;
         return t(t({}, e), {}, {
             status: n,
             lastUpdate: Date.now()
         })
     }
 
-    function No(e) {
+    function To(e) {
         return "string" == typeof e ? {
             protocol: "https",
             url: e,
-            accept: Io.Any
+            accept: Do.Any
         } : {
             protocol: e.protocol || "https",
             url: e.url,
-            accept: e.accept || Io.Any
+            accept: e.accept || Do.Any
         }
     }
-    var To = "GET",
-        Ro = "POST";
+    var Ro = "GET",
+        qo = "POST";
 
-    function qo(e, t) {
+    function Lo(e, t) {
         return Promise.all(t.map((function(t) {
             return e.get(t, (function() {
-                return Promise.resolve(xo(t))
+                return Promise.resolve(No(t))
             }))
         }))).then((function(e) {
             var n = e.filter((function(e) {
                     return function(e) {
-                        return e.status === Do || Date.now() - e.lastUpdate > Co
+                        return e.status === ko || Date.now() - e.lastUpdate > xo
                     }(e)
                 })),
                 r = e.filter((function(e) {
                     return function(e) {
-                        return e.status === Ao && Date.now() - e.lastUpdate <= Co
+                        return e.status === Co && Date.now() - e.lastUpdate <= xo
                     }(e)
                 })),
                 o = [].concat(a(n), a(r));
             return {
                 getTimeout: function(e, t) {
                     return (0 === r.length && 0 === e ? 1 : r.length + 3 + e) * t
                 },
                 statelessHosts: o.length > 0 ? o.map((function(e) {
-                    return No(e)
+                    return To(e)
                 })) : t
             }
         }))
     }
 
-    function Lo(e, n, r, o) {
+    function Mo(e, n, r, o) {
         var i = [],
             c = function(e, n) {
-                if (e.method === To || void 0 === e.data && void 0 === n.data) return;
+                if (e.method === Ro || void 0 === e.data && void 0 === n.data) return;
                 var r = Array.isArray(e.data) ? e.data : t(t({}, e.data), n.data);
                 return JSON.stringify(r)
             }(r, o),
             u = function(e, n) {
                 var r = t(t({}, e.headers), n.headers),
                     o = {};
                 return Object.keys(r).forEach((function(e) {
                     var t = r[e];
                     o[e.toLowerCase()] = t
                 })), o
             }(e, o),
             l = r.method,
-            s = r.method !== To ? {} : t(t({}, r.data), o.data),
+            s = r.method !== Ro ? {} : t(t({}, r.data), o.data),
             f = t(t(t({
                 "x-algolia-agent": e.userAgent.value
             }, e.queryParameters), s), o.queryParameters),
             p = 0,
             m = function t(n, a) {
                 var s = n.pop();
                 if (void 0 === s) throw {
                     name: "RetryError",
                     message: "Unreachable hosts - your application id may be incorrect. If the error persists, contact support@algolia.com.",
-                    transporterStackTrace: Fo(i)
+                    transporterStackTrace: Bo(i)
                 };
                 var m = {
                         data: c,
                         headers: u,
                         method: l,
-                        url: Ho(s, r.path, f),
+                        url: Uo(s, r.path, f),
                         connectTimeout: a(p, e.timeouts.connect),
                         responseTimeout: a(p, o.timeout)
                     },
                     v = function(e) {
                         var t = {
                             request: m,
                             response: e,
@@ -4669,15 +4698,15 @@
                                         }
                                     }(t.message, e)
                                 }
                             }(e)
                         },
                         onRetry: function(r) {
                             var o = v(r);
-                            return r.isTimedOut && p++, Promise.all([e.logger.info("Retryable failure", Bo(o)), e.hostsCache.set(s, xo(s, r.isTimedOut ? Ao : ko))]).then((function() {
+                            return r.isTimedOut && p++, Promise.all([e.logger.info("Retryable failure", Vo(o)), e.hostsCache.set(s, No(s, r.isTimedOut ? Co : Ao))]).then((function() {
                                 return t(n, a)
                             }))
                         },
                         onFail: function(e) {
                             throw v(e),
                                 function(e, t) {
                                     var n = e.content,
@@ -4690,15 +4719,15 @@
                                         return {
                                             name: "ApiError",
                                             message: e,
                                             status: t,
                                             transporterStackTrace: n
                                         }
                                     }(o, r, t)
-                                }(e, Fo(i))
+                                }(e, Bo(i))
                         }
                     };
                 return e.requester.send(m).then((function(e) {
                     return function(e, t) {
                         return function(e) {
                             var t = e.status;
                             return e.isTimedOut || function(e) {
@@ -4706,75 +4735,75 @@
                                     n = e.status;
                                 return !t && 0 == ~~n
                             }(e) || 2 != ~~(t / 100) && 4 != ~~(t / 100)
                         }(e) ? t.onRetry(e) : 2 == ~~(e.status / 100) ? t.onSuccess(e) : t.onFail(e)
                     }(e, d)
                 }))
             };
-        return qo(e.hostsCache, n).then((function(e) {
+        return Lo(e.hostsCache, n).then((function(e) {
             return m(a(e.statelessHosts).reverse(), e.getTimeout)
         }))
     }
 
-    function Mo(e) {
+    function Ho(e) {
         var t = {
             value: "Algolia for JavaScript (".concat(e, ")"),
             add: function(e) {
                 var n = "; ".concat(e.segment).concat(void 0 !== e.version ? " (".concat(e.version, ")") : "");
                 return -1 === t.value.indexOf(n) && (t.value = "".concat(t.value).concat(n)), t
             }
         };
         return t
     }
 
-    function Ho(e, t, n) {
-        var r = Uo(n),
+    function Uo(e, t, n) {
+        var r = Fo(n),
             o = "".concat(e.protocol, "://").concat(e.url, "/").concat("/" === t.charAt(0) ? t.substr(1) : t);
         return r.length && (o += "?".concat(r)), o
     }
 
-    function Uo(e) {
+    function Fo(e) {
         return Object.keys(e).map((function(t) {
             return jo("%s=%s", t, (n = e[t], "[object Object]" === Object.prototype.toString.call(n) || "[object Array]" === Object.prototype.toString.call(n) ? JSON.stringify(e[t]) : e[t]));
             var n
         })).join("&")
     }
 
-    function Fo(e) {
+    function Bo(e) {
         return e.map((function(e) {
-            return Bo(e)
+            return Vo(e)
         }))
     }
 
-    function Bo(e) {
+    function Vo(e) {
         var n = e.request.headers["x-algolia-api-key"] ? {
             "x-algolia-api-key": "*****"
         } : {};
         return t(t({}, e), {}, {
             request: t(t({}, e.request), {}, {
                 headers: t(t({}, e.request.headers), n)
             })
         })
     }
-    var Vo = function(e) {
+    var Ko = function(e) {
             var n = e.appId,
                 r = function(e, t, n) {
                     var r = {
                         "x-algolia-api-key": n,
                         "x-algolia-application-id": t
                     };
                     return {
                         headers: function() {
-                            return e === Eo.WithinHeaders ? r : {}
+                            return e === Po.WithinHeaders ? r : {}
                         },
                         queryParameters: function() {
-                            return e === Eo.WithinQueryParameters ? r : {}
+                            return e === Po.WithinQueryParameters ? r : {}
                         }
                     }
-                }(void 0 !== e.authMode ? e.authMode : Eo.WithinHeaders, n, e.apiKey),
+                }(void 0 !== e.authMode ? e.authMode : Po.WithinHeaders, n, e.apiKey),
                 o = function(e) {
                     var t = e.hostsCache,
                         n = e.logger,
                         r = e.requester,
                         o = e.requestsCache,
                         i = e.responsesCache,
                         a = e.timeouts,
@@ -4788,21 +4817,21 @@
                             requestsCache: o,
                             responsesCache: i,
                             timeouts: a,
                             userAgent: u,
                             headers: e.headers,
                             queryParameters: s,
                             hosts: l.map((function(e) {
-                                return No(e)
+                                return To(e)
                             })),
                             read: function(e, t) {
-                                var n = Po(t, f.timeouts.read),
+                                var n = Io(t, f.timeouts.read),
                                     r = function() {
-                                        return Lo(f, f.hosts.filter((function(e) {
-                                            return 0 != (e.accept & Io.Read)
+                                        return Mo(f, f.hosts.filter((function(e) {
+                                            return 0 != (e.accept & Do.Read)
                                         })), e, n)
                                     };
                                 if (!0 !== (void 0 !== n.cacheable ? n.cacheable : e.cacheable)) return r();
                                 var o = {
                                     request: e,
                                     mappedRequestOptions: n,
                                     transporter: {
@@ -4824,28 +4853,28 @@
                                 }), {
                                     miss: function(e) {
                                         return f.responsesCache.set(o, e)
                                     }
                                 })
                             },
                             write: function(e, t) {
-                                return Lo(f, f.hosts.filter((function(e) {
-                                    return 0 != (e.accept & Io.Write)
-                                })), e, Po(t, f.timeouts.write))
+                                return Mo(f, f.hosts.filter((function(e) {
+                                    return 0 != (e.accept & Do.Write)
+                                })), e, Io(t, f.timeouts.write))
                             }
                         };
                     return f
                 }(t(t({
                     hosts: [{
                         url: "".concat(n, "-dsn.algolia.net"),
-                        accept: Io.Read
+                        accept: Do.Read
                     }, {
                         url: "".concat(n, ".algolia.net"),
-                        accept: Io.Write
-                    }].concat(Oo([{
+                        accept: Do.Write
+                    }].concat(So([{
                         url: "".concat(n, "-1.algolianet.com")
                     }, {
                         url: "".concat(n, "-2.algolianet.com")
                     }, {
                         url: "".concat(n, "-3.algolianet.com")
                     }]))
                 }, e), {}, {
@@ -4863,106 +4892,106 @@
                             version: t
                         })
                     },
                     clearCache: function() {
                         return Promise.all([o.requestsCache.clear(), o.responsesCache.clear()]).then((function() {}))
                     }
                 };
-            return So(i, e.methods)
+            return wo(i, e.methods)
         },
         Wo = function(e) {
             return function(t, n) {
-                return t.method === To ? e.transporter.read(t, n) : e.transporter.write(t, n)
+                return t.method === Ro ? e.transporter.read(t, n) : e.transporter.write(t, n)
             }
         },
-        Ko = function(e) {
+        zo = function(e) {
             return function(t) {
                 var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {},
                     r = {
                         transporter: e.transporter,
                         appId: e.appId,
                         indexName: t
                     };
-                return So(r, n.methods)
+                return wo(r, n.methods)
             }
         },
-        zo = function(e) {
+        Jo = function(e) {
             return function(n, r) {
                 var o = n.map((function(e) {
                     return t(t({}, e), {}, {
-                        params: Uo(e.params || {})
+                        params: Fo(e.params || {})
                     })
                 }));
                 return e.transporter.read({
-                    method: Ro,
+                    method: qo,
                     path: "1/indexes/*/queries",
                     data: {
                         requests: o
                     },
                     cacheable: !0
                 }, r)
             }
         },
-        Jo = function(e) {
+        $o = function(e) {
             return function(n, r) {
                 return Promise.all(n.map((function(n) {
                     var o = n.params,
                         c = o.facetName,
                         a = o.facetQuery,
-                        u = i(o, yo);
-                    return Ko(e)(n.indexName, {
+                        u = i(o, bo);
+                    return zo(e)(n.indexName, {
                         methods: {
-                            searchForFacetValues: Zo
+                            searchForFacetValues: Yo
                         }
                     }).searchForFacetValues(c, a, t(t({}, r), u))
                 })))
             }
         },
-        $o = function(e) {
+        Qo = function(e) {
             return function(t, n, r) {
                 return e.transporter.read({
-                    method: Ro,
+                    method: qo,
                     path: jo("1/answers/%s/prediction", e.indexName),
                     data: {
                         query: t,
                         queryLanguages: n
                     },
                     cacheable: !0
                 }, r)
             }
         },
-        Qo = function(e) {
+        Zo = function(e) {
             return function(t, n) {
                 return e.transporter.read({
-                    method: Ro,
+                    method: qo,
                     path: jo("1/indexes/%s/query", e.indexName),
                     data: {
                         query: t
                     },
                     cacheable: !0
                 }, n)
             }
         },
-        Zo = function(e) {
+        Yo = function(e) {
             return function(t, n, r) {
                 return e.transporter.read({
-                    method: Ro,
+                    method: qo,
                     path: jo("1/indexes/%s/facets/%s/query", e.indexName, t),
                     data: {
                         facetQuery: n
                     },
                     cacheable: !0
                 }, r)
             }
         },
-        Yo = 1,
-        Go = 2,
-        Xo = 3;
+        Go = 1,
+        Xo = 2,
+        ei = 3;
 
-    function ei(e, n, r) {
+    function ti(e, n, r) {
         var o, i = {
             appId: e,
             apiKey: n,
             timeouts: {
                 connect: 1,
                 read: 2,
                 write: 30
@@ -4998,108 +5027,108 @@
                                 status: n.status,
                                 isTimedOut: !1
                             })
                         }, n.send(e.data)
                     }))
                 }
             },
-            logger: (o = Xo, {
+            logger: (o = ei, {
                 debug: function(e, t) {
-                    return Yo >= o && console.debug(e, t), Promise.resolve()
+                    return Go >= o && console.debug(e, t), Promise.resolve()
                 },
                 info: function(e, t) {
-                    return Go >= o && console.info(e, t), Promise.resolve()
+                    return Xo >= o && console.info(e, t), Promise.resolve()
                 },
                 error: function(e, t) {
                     return console.error(e, t), Promise.resolve()
                 }
             }),
-            responsesCache: _o(),
-            requestsCache: _o({
+            responsesCache: Oo(),
+            requestsCache: Oo({
                 serializable: !1
             }),
-            hostsCache: go({
-                caches: [bo({
-                    key: "".concat(wo, "-").concat(e)
-                }), _o()]
+            hostsCache: _o({
+                caches: [go({
+                    key: "".concat(Eo, "-").concat(e)
+                }), Oo()]
             }),
-            userAgent: Mo(wo).add({
+            userAgent: Ho(Eo).add({
                 segment: "Browser",
                 version: "lite"
             }),
-            authMode: Eo.WithinQueryParameters
+            authMode: Po.WithinQueryParameters
         };
-        return Vo(t(t(t({}, i), r), {}, {
+        return Ko(t(t(t({}, i), r), {}, {
             methods: {
-                search: zo,
-                searchForFacetValues: Jo,
-                multipleQueries: zo,
-                multipleSearchForFacetValues: Jo,
+                search: Jo,
+                searchForFacetValues: $o,
+                multipleQueries: Jo,
+                multipleSearchForFacetValues: $o,
                 customRequest: Wo,
                 initIndex: function(e) {
                     return function(t) {
-                        return Ko(e)(t, {
+                        return zo(e)(t, {
                             methods: {
-                                search: Qo,
-                                searchForFacetValues: Zo,
-                                findAnswers: $o
+                                search: Zo,
+                                searchForFacetValues: Yo,
+                                findAnswers: Qo
                             }
                         })
                     }
                 }
             }
         }))
     }
-    ei.version = wo;
-    var ti = "3.5.2";
-    var ni = ["footer", "searchBox"];
+    ti.version = Eo;
+    var ni = "3.6.0";
+    var ri = ["footer", "searchBox"];
 
-    function ri() {
-        return ri = Object.assign || function(e) {
+    function oi() {
+        return oi = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, ri.apply(this, arguments)
+        }, oi.apply(this, arguments)
     }
 
-    function oi(e, t) {
+    function ii(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function ii(e) {
+    function ci(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? oi(Object(n), !0).forEach((function(t) {
-                ci(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : oi(Object(n)).forEach((function(t) {
+            t % 2 ? ii(Object(n), !0).forEach((function(t) {
+                ai(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ii(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function ci(e, t, n) {
+    function ai(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function ai(e, t) {
+    function ui(e, t) {
         return function(e) {
             if (Array.isArray(e)) return e
         }(e) || function(e, t) {
             var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
             if (null == n) return;
             var r, o, i = [],
                 c = !0,
@@ -5114,31 +5143,31 @@
                 } finally {
                     if (a) throw o
                 }
             }
             return i
         }(e, t) || function(e, t) {
             if (!e) return;
-            if ("string" == typeof e) return ui(e, t);
+            if ("string" == typeof e) return li(e, t);
             var n = Object.prototype.toString.call(e).slice(8, -1);
             "Object" === n && e.constructor && (n = e.constructor.name);
             if ("Map" === n || "Set" === n) return Array.from(e);
-            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return ui(e, t)
+            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return li(e, t)
         }(e, t) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function ui(e, t) {
+    function li(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function li(e, t) {
+    function si(e, t) {
         if (null == e) return {};
         var n, r, o = function(e, t) {
             if (null == e) return {};
             var n, r, o = {},
                 i = Object.keys(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
             return o
@@ -5146,50 +5175,50 @@
         if (Object.getOwnPropertySymbols) {
             var i = Object.getOwnPropertySymbols(e);
             for (r = 0; r < i.length; r++) n = i[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
         }
         return o
     }
 
-    function si(e) {
+    function fi(e) {
         var t = e.appId,
             n = e.apiKey,
             r = e.indexName,
             o = e.placeholder,
             i = void 0 === o ? "Search docs" : o,
             c = e.searchParameters,
             a = e.maxResultsPerGroup,
             u = e.onClose,
-            l = void 0 === u ? $r : u,
+            l = void 0 === u ? Qr : u,
             s = e.transformItems,
-            f = void 0 === s ? zr : s,
+            f = void 0 === s ? Jr : s,
             p = e.hitComponent,
-            m = void 0 === p ? dr : p,
+            m = void 0 === p ? hr : p,
             v = e.resultsFooterComponent,
             d = void 0 === v ? function() {
                 return null
             } : v,
             h = e.navigator,
             y = e.initialScrollY,
             b = void 0 === y ? 0 : y,
             g = e.transformSearchClient,
-            _ = void 0 === g ? zr : g,
+            _ = void 0 === g ? Jr : g,
             O = e.disableUserPersonalization,
             S = void 0 !== O && O,
-            j = e.initialQuery,
-            w = void 0 === j ? "" : j,
+            w = e.initialQuery,
+            j = void 0 === w ? "" : w,
             E = e.translations,
             P = void 0 === E ? {} : E,
             I = e.getMissingResultsUrl,
             D = e.insights,
             k = void 0 !== D && D,
             A = P.footer,
             C = P.searchBox,
-            x = li(P, ni),
-            N = ai(Be.useState({
+            x = si(P, ri),
+            N = ui(Be.useState({
                 query: "",
                 collections: [],
                 completion: null,
                 context: {},
                 isOpen: !1,
                 activeItemId: null,
                 status: "idle"
@@ -5199,52 +5228,52 @@
             q = Be.useRef(null),
             L = Be.useRef(null),
             M = Be.useRef(null),
             H = Be.useRef(null),
             U = Be.useRef(null),
             F = Be.useRef(10),
             B = Be.useRef("undefined" != typeof window ? window.getSelection().toString().slice(0, 64) : "").current,
-            V = Be.useRef(w || B).current,
-            W = function(e, t, n) {
+            V = Be.useRef(j || B).current,
+            K = function(e, t, n) {
                 return Be.useMemo((function() {
-                    var r = ei(e, t);
-                    return r.addAlgoliaAgent("docsearch", ti), !1 === /docsearch.js \(.*\)/.test(r.transporter.userAgent.value) && r.addAlgoliaAgent("docsearch-react", ti), n(r)
+                    var r = ti(e, t);
+                    return r.addAlgoliaAgent("docsearch", ni), !1 === /docsearch.js \(.*\)/.test(r.transporter.userAgent.value) && r.addAlgoliaAgent("docsearch-react", ni), n(r)
                 }), [e, t, n])
             }(t, n, _),
-            K = Be.useRef(ho({
+            W = Be.useRef(yo({
                 key: "__DOCSEARCH_FAVORITE_SEARCHES__".concat(r),
                 limit: 10
             })).current,
-            z = Be.useRef(ho({
+            z = Be.useRef(yo({
                 key: "__DOCSEARCH_RECENT_SEARCHES__".concat(r),
-                limit: 0 === K.getAll().length ? 7 : 4
+                limit: 0 === W.getAll().length ? 7 : 4
             })).current,
             J = Be.useCallback((function(e) {
                 if (!S) {
                     var t = "content" === e.type ? e.__docsearch_parent : e;
-                    t && -1 === K.getAll().findIndex((function(e) {
+                    t && -1 === W.getAll().findIndex((function(e) {
                         return e.objectID === t.objectID
                     })) && z.add(t)
                 }
-            }), [K, z, S]),
+            }), [W, z, S]),
             $ = Be.useCallback((function(e) {
                 if (T.context.algoliaInsightsPlugin && e.__autocomplete_id) {
                     var t = e,
                         n = {
                             eventName: "Item Selected",
                             index: t.__autocomplete_indexName,
                             items: [t],
                             positions: [e.__autocomplete_id],
                             queryID: t.__autocomplete_queryID
                         };
                     T.context.algoliaInsightsPlugin.insights.clickedObjectIDsAfterSearch(n)
                 }
             }), [T.context.algoliaInsightsPlugin]),
             Q = Be.useMemo((function() {
-                return fr({
+                return pr({
                     id: "docsearch",
                     defaultActiveItemId: 0,
                     placeholder: i,
                     openOnFocus: !0,
                     initialState: {
                         query: V,
                         context: {
@@ -5262,57 +5291,57 @@
                             u = e.setContext,
                             s = e.setStatus;
                         if (!o) return S ? [] : [{
                             sourceId: "recentSearches",
                             onSelect: function(e) {
                                 var t = e.item,
                                     n = e.event;
-                                J(t), Jr(n) || l()
+                                J(t), $r(n) || l()
                             },
                             getItemUrl: function(e) {
                                 return e.item.url
                             },
                             getItems: function() {
                                 return z.getAll()
                             }
                         }, {
                             sourceId: "favoriteSearches",
                             onSelect: function(e) {
                                 var t = e.item,
                                     n = e.event;
-                                J(t), Jr(n) || l()
+                                J(t), $r(n) || l()
                             },
                             getItemUrl: function(e) {
                                 return e.item.url
                             },
                             getItems: function() {
-                                return K.getAll()
+                                return W.getAll()
                             }
                         }];
                         var p = Boolean(k);
-                        return W.search([{
+                        return K.search([{
                             query: o,
                             indexName: r,
-                            params: ii({
+                            params: ci({
                                 attributesToRetrieve: ["hierarchy.lvl0", "hierarchy.lvl1", "hierarchy.lvl2", "hierarchy.lvl3", "hierarchy.lvl4", "hierarchy.lvl5", "hierarchy.lvl6", "content", "type", "url"],
                                 attributesToSnippet: ["hierarchy.lvl1:".concat(F.current), "hierarchy.lvl2:".concat(F.current), "hierarchy.lvl3:".concat(F.current), "hierarchy.lvl4:".concat(F.current), "hierarchy.lvl5:".concat(F.current), "hierarchy.lvl6:".concat(F.current), "content:".concat(F.current)],
                                 snippetEllipsisText: "…",
                                 highlightPreTag: "<mark>",
                                 highlightPostTag: "</mark>",
                                 hitsPerPage: 20,
                                 clickAnalytics: p
                             }, c)
                         }]).catch((function(e) {
                             throw "RetryError" === e.name && s("error"), e
                         })).then((function(e) {
                             var o = e.results[0],
                                 c = o.hits,
                                 s = o.nbHits,
-                                m = Kr(c, (function(e) {
-                                    return Yr(e)
+                                m = zr(c, (function(e) {
+                                    return Gr(e)
                                 }), a);
                             i.context.searchSuggestions.length < Object.keys(m).length && u({
                                 searchSuggestions: Object.keys(m)
                             }), u({
                                 nbHits: s
                             });
                             var v = {};
@@ -5325,40 +5354,40 @@
                                 }
                             }), Object.values(m).map((function(e, t) {
                                 return {
                                     sourceId: "hits".concat(t),
                                     onSelect: function(e) {
                                         var t = e.item,
                                             n = e.event;
-                                        J(t), Jr(n) || l()
+                                        J(t), $r(n) || l()
                                     },
                                     getItemUrl: function(e) {
                                         return e.item.url
                                     },
                                     getItems: function() {
-                                        return Object.values(Kr(e, (function(e) {
+                                        return Object.values(zr(e, (function(e) {
                                             return e.hierarchy.lvl1
                                         }), a)).map(f).map((function(e) {
                                             return e.map((function(t) {
                                                 var n = null,
                                                     r = e.find((function(e) {
                                                         return "lvl1" === e.type && e.hierarchy.lvl1 === t.hierarchy.lvl1
                                                     }));
-                                                return "lvl1" !== t.type && r && (n = r), ii(ii({}, t), {}, {
+                                                return "lvl1" !== t.type && r && (n = r), ci(ci({}, t), {}, {
                                                     __docsearch_parent: n
                                                 }, v)
                                             }))
                                         })).flat()
                                     }
                                 }
                             }))
                         }))
                     }
                 })
-            }), [r, c, a, W, l, z, K, J, V, i, h, f, S, k, t, n]),
+            }), [r, c, a, K, l, z, W, J, V, i, h, f, S, k, t, n]),
             Z = Q.getEnvironmentProps,
             Y = Q.getRootProps,
             G = Q.refresh;
         return function(e) {
                 var t = e.getEnvironmentProps,
                     n = e.panelElement,
                     r = e.formElement,
@@ -5422,15 +5451,15 @@
                         L.current.style.setProperty("--docsearch-vh", "".concat(e, "px"))
                     }
                 }
                 return e(), window.addEventListener("resize", e),
                     function() {
                         window.removeEventListener("resize", e)
                     }
-            }), []), Be.createElement("div", ri({
+            }), []), Be.createElement("div", oi({
                 ref: q
             }, Y({
                 "aria-expanded": !0
             }), {
                 className: ["DocSearch", "DocSearch-Container", "stalled" === T.status && "DocSearch-Container--Stalled", "error" === T.status && "DocSearch-Container--Errored"].filter(Boolean).join(" "),
                 role: "button",
                 tabIndex: 0,
@@ -5439,56 +5468,56 @@
                 }
             }), Be.createElement("div", {
                 className: "DocSearch-Modal",
                 ref: L
             }, Be.createElement("header", {
                 className: "DocSearch-SearchBar",
                 ref: M
-            }, Be.createElement(fo, ri({}, Q, {
+            }, Be.createElement(po, oi({}, Q, {
                 state: T,
                 autoFocus: 0 === V.length,
                 inputRef: U,
                 isFromSelection: Boolean(V) && V === B,
                 translations: C,
                 onClose: l
             }))), Be.createElement("div", {
                 className: "DocSearch-Dropdown",
                 ref: H
-            }, Be.createElement(ao, ri({}, Q, {
+            }, Be.createElement(uo, oi({}, Q, {
                 indexName: r,
                 state: T,
                 hitComponent: m,
                 resultsFooterComponent: d,
                 disableUserPersonalization: S,
                 recentSearches: z,
-                favoriteSearches: K,
+                favoriteSearches: W,
                 inputRef: U,
                 translations: x,
                 getMissingResultsUrl: I,
                 onItemClick: function(e, t) {
-                    $(e), J(e), Jr(t) || l()
+                    $(e), J(e), $r(t) || l()
                 }
             }))), Be.createElement("footer", {
                 className: "DocSearch-Footer"
-            }, Be.createElement(vr, {
+            }, Be.createElement(dr, {
                 translations: A
             }))))
     }
 
-    function fi() {
-        return fi = Object.assign || function(e) {
+    function pi() {
+        return pi = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, fi.apply(this, arguments)
+        }, pi.apply(this, arguments)
     }
 
-    function pi(e, t) {
+    function mi(e, t) {
         return function(e) {
             if (Array.isArray(e)) return e
         }(e) || function(e, t) {
             var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
             if (null == n) return;
             var r, o, i = [],
                 c = !0,
@@ -5503,36 +5532,36 @@
                 } finally {
                     if (a) throw o
                 }
             }
             return i
         }(e, t) || function(e, t) {
             if (!e) return;
-            if ("string" == typeof e) return mi(e, t);
+            if ("string" == typeof e) return vi(e, t);
             var n = Object.prototype.toString.call(e).slice(8, -1);
             "Object" === n && e.constructor && (n = e.constructor.name);
             if ("Map" === n || "Set" === n) return Array.from(e);
-            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return mi(e, t)
+            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return vi(e, t)
         }(e, t) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function mi(e, t) {
+    function vi(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function vi(e) {
+    function di(e) {
         var t, n, r = Be.useRef(null),
-            o = pi(Be.useState(!1), 2),
+            o = mi(Be.useState(!1), 2),
             i = o[0],
             c = o[1],
-            a = pi(Be.useState((null == e ? void 0 : e.initialQuery) || void 0), 2),
+            a = mi(Be.useState((null == e ? void 0 : e.initialQuery) || void 0), 2),
             u = a[0],
             l = a[1],
             s = Be.useCallback((function() {
                 c(!0)
             }), [c]),
             f = Be.useCallback((function() {
                 c(!1)
@@ -5565,25 +5594,25 @@
                 c(!0), l(e.key)
             }), [c, l]),
             searchButtonRef: r
         }), Be.createElement(Be.Fragment, null, Be.createElement(Ye, {
             ref: r,
             translations: null == e || null === (t = e.translations) || void 0 === t ? void 0 : t.button,
             onClick: s
-        }), i && Ie(Be.createElement(si, fi({}, e, {
+        }), i && Ie(Be.createElement(fi, pi({}, e, {
             initialScrollY: window.scrollY,
             initialQuery: u,
             translations: null == e || null === (n = e.translations) || void 0 === n ? void 0 : n.modal,
             onClose: f
         })), document.body))
     }
     return function(e) {
-        Ce(Be.createElement(vi, o({}, e, {
+        Ce(Be.createElement(di, o({}, e, {
             transformSearchClient: function(t) {
-                return t.addAlgoliaAgent("docsearch.js", ti), e.transformSearchClient ? e.transformSearchClient(t) : t
+                return t.addAlgoliaAgent("docsearch.js", ni), e.transformSearchClient ? e.transformSearchClient(t) : t
             }
         })), function(e) {
             var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : window;
             return "string" == typeof e ? t.document.querySelector(e) : e
         }(e.container, e.environment))
     }
 }));
```

### Comparing `sphinx_docsearch-0.0.4/src/sphinx_docsearch/static/docsearch_config.js_t` & `sphinx_docsearch-0.0.5/src/sphinx_docsearch/static/docsearch_config.js_t`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.4/src/sphinx_docsearch/static/furo-docsearch-custom.css` & `sphinx_docsearch-0.0.5/src/sphinx_docsearch/static/furo-docsearch-custom.css`

 * *Files identical despite different names*

### Comparing `sphinx_docsearch-0.0.4/PKG-INFO` & `sphinx_docsearch-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: sphinx-docsearch
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Sphinx extension for replacing the built-in search with Algolia DocSearch
 License: MIT
 Author: Algolia
+Author-email: support@algolia.com
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -15,28 +16,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
 Requires-Dist: sphinx (<7.2) ; python_version >= "3.8" and python_version < "3.9"
-Requires-Dist: sphinx (>=7.2,<7.3) ; python_version >= "3.9" and python_full_version <= "3.12.0"
+Requires-Dist: sphinx (>=7.2,<7.4) ; python_version >= "3.9" and python_version < "3.13"
 Description-Content-Type: text/markdown
 
 # Algolia DocSearch for Sphinx
 
 This extension for the [Sphinx](https://www.sphinx-doc.org/en/master/) documentation generator
 replaces Sphinx's built-in search with Algolia DocSearch.
 
 ## Before you begin
 
 [**Apply for DocSearch**](https://docsearch.algolia.com/apply).
 You'll get an email with your Algolia credentials.
 
-This extension supports Python versions 3.8, 3.9, 3.10, and 3.11 and Sphinx versions 5 and later.
+This extension supports Python versions 3.8 and later and Sphinx versions 5 and later.
 
 ## Install
 
 Install the `sphinx-docsearch` package:
 
 ```sh
 pip install sphinx-docsearch
@@ -56,19 +57,19 @@
    ```python
    # conf.py
    docsearch_app_id = "<DOCSEARCH_APP_ID>"
    docsearch_api_key = "<DOCSEARCH_SEARCH_API_KEY>"
    docsearch_index_name = "<DOCSEARCH_INDEX_NAME>"
    ```
 
-   See also: [Configure DocSearch](https://sphinx-docsearch.readthedocs.io/en/latest/configuration.html).
+   See also: [Configure DocSearch](https://sphinx-docsearch.readthedocs.io/configuration.html).
 
 ## Customize
 
 To change what the crawler should extract from your pages, see [Record Extractor](https://docsearch.algolia.com/docs/record-extractor).
 
-You can add [custom templates](https://sphinx-docsearch.readthedocs.io/en/latest/customization.html#add-custom-templates),
-if your Sphinx HTML theme uses templates [not provided](https://sphinx-docsearch.readthedocs.io/en/latest/themes.html)
+You can add [custom templates](https://sphinx-docsearch.readthedocs.io/customization.html#add-custom-templates),
+if your Sphinx HTML theme uses templates [not provided](https://sphinx-docsearch.readthedocs.io/themes.html)
 by this extension.
 
-You can customize the look of the DocSearch UI by [adding your own CSS](https://sphinx-docsearch.readthedocs.io/en/latest/customization.html#add-custom-css).
+You can customize the look of the DocSearch UI by [adding your own CSS](https://sphinx-docsearch.readthedocs.io/customization.html#add-custom-css).
```

