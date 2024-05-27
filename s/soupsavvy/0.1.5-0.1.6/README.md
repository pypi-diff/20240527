# Comparing `tmp/soupsavvy-0.1.5.tar.gz` & `tmp/soupsavvy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soupsavvy-0.1.5.tar", last modified: Mon May 20 01:15:47 2024, max compression
+gzip compressed data, was "soupsavvy-0.1.6.tar", last modified: Mon May 27 20:58:38 2024, max compression
```

## Comparing `soupsavvy-0.1.5.tar` & `soupsavvy-0.1.6.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.131610 soupsavvy-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8448 2024-05-20 01:15:47.131610 soupsavvy-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:15:47.131610 soupsavvy-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.127611 soupsavvy-0.1.5/soupsavvy/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 01:15:35.000000 soupsavvy-0.1.5/soupsavvy/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-20 01:15:35.000000 soupsavvy-0.1.5/soupsavvy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.127611 soupsavvy-0.1.5/soupsavvy/tags/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20610 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17316 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/combinators.py
--rw-r--r--   0 runner    (1001) docker     (127)    15556 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.127611 soupsavvy-0.1.5/soupsavvy/tags/css/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/css/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/css/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18511 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/css/tag_selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/tags/tag_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.127611 soupsavvy-0.1.5/soupsavvy/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.131610 soupsavvy-0.1.5/soupsavvy/testing/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.131610 soupsavvy-0.1.5/soupsavvy/testing/generators/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/templates/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/templates/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/testing/generators/templates/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.131610 soupsavvy-0.1.5/soupsavvy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 01:15:31.000000 soupsavvy-0.1.5/soupsavvy/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:15:47.131610 soupsavvy-0.1.5/soupsavvy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8448 2024-05-20 01:15:47.000000 soupsavvy-0.1.5/soupsavvy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-20 01:15:47.000000 soupsavvy-0.1.5/soupsavvy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:15:47.000000 soupsavvy-0.1.5/soupsavvy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-20 01:15:47.000000 soupsavvy-0.1.5/soupsavvy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 01:15:47.000000 soupsavvy-0.1.5/soupsavvy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:38.722322 soupsavvy-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-27 20:58:38.722322 soupsavvy-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:58:38.722322 soupsavvy-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:38.714321 soupsavvy-0.1.6/soupsavvy/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 20:58:24.000000 soupsavvy-0.1.6/soupsavvy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-27 20:58:24.000000 soupsavvy-0.1.6/soupsavvy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:38.718321 soupsavvy-0.1.6/soupsavvy/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20610 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/tags/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/tags/combinators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19470 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/tags/components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:38.718321 soupsavvy-0.1.6/soupsavvy/tags/css/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/tags/css/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/tags/css/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/tags/css/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18511 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/tags/css/tag_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/tags/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/tags/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/tags/relative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/tags/tag_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:38.718321 soupsavvy-0.1.6/soupsavvy/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:38.718321 soupsavvy-0.1.6/soupsavvy/testing/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/testing/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/testing/generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/testing/generators/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/testing/generators/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/testing/generators/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:38.718321 soupsavvy-0.1.6/soupsavvy/testing/generators/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/testing/generators/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/testing/generators/templates/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/testing/generators/templates/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/testing/generators/templates/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:38.718321 soupsavvy-0.1.6/soupsavvy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-27 20:58:20.000000 soupsavvy-0.1.6/soupsavvy/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:38.718321 soupsavvy-0.1.6/soupsavvy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-27 20:58:38.000000 soupsavvy-0.1.6/soupsavvy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-27 20:58:38.000000 soupsavvy-0.1.6/soupsavvy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:58:38.000000 soupsavvy-0.1.6/soupsavvy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-27 20:58:38.000000 soupsavvy-0.1.6/soupsavvy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 20:58:38.000000 soupsavvy-0.1.6/soupsavvy.egg-info/top_level.txt
```

### Comparing `soupsavvy-0.1.5/LICENSE` & `soupsavvy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.5/PKG-INFO` & `soupsavvy-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soupsavvy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package for advanced web scraping
 Author: sewcio543
 License: MIT License
         
         Copyright (c) 2024 Wojciech Seweryn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,19 +48,18 @@
 Requires-Dist: coverage==7.2.2; extra == "dev"
 Requires-Dist: flake8==7.0.0; extra == "dev"
 Requires-Dist: mypy==1.7.0; extra == "dev"
 Requires-Dist: pre-commit==3.6.1; extra == "dev"
 Requires-Dist: pytest==7.1.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 
-# soupsavvy
+![SoupSavvy](resources/logo.png)
+========
 
------------------
-
-## Python package that makes web-scraping more manageable
+## Python package that makes web-scraping better than ever
 
 | | |
 | --- | --- |
 | Package | ![Deployment PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/production_release.yml/badge.svg) [![GitHub](https://img.shields.io/badge/GitHub-sewcio543-181717.svg?style=flat&logo=github)](https://github.com/sewcio543) [![PyPI](https://img.shields.io/pypi/v/soupsavvy?color=orange)](https://pypi.org/project/soupsavvy/) [![Python Versions](https://img.shields.io/pypi/pyversions/soupsavvy)](https://www.python.org/)|
 | Testing | ![Tests](https://github.com/sewcio543/soupsavvy/actions/workflows/tests.yml/badge.svg) [![Codecov](https://codecov.io/gh/sewcio543/soupsavvy/graph/badge.svg?token=RZ51VS3QLB)](https://codecov.io/gh/sewcio543/soupsavvy)|
 | Code Quality | ![Build](https://github.com/sewcio543/soupsavvy/actions/workflows/build_package.yml/badge.svg) ![Linting](https://github.com/sewcio543/soupsavvy/actions/workflows/linting.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sewcio543/soupsavvy/main.svg)](https://results.pre-commit.ci/latest/github/sewcio543/soupsavvy/main)|
 | Documentation | [![readthedocs](https://img.shields.io/readthedocs/pip?logo=readthedocs)](https://github.com/sewcio543/soupsavvy/actions/workflows/documentation.yml/badge.svg) [![Docs link](https://img.shields.io/badge/docs-check_out-blue)](https://sewcio543.github.io/soupsavvy/)|
@@ -70,15 +69,14 @@
 - [About](#about)
 - [Key features](#key-features)
 - [Instalation](#installation)
 - [Usage](#usage)
 - [Contributing](#contributing)
 - [License](#license)
 - [Acknowledgements](#acknowledgements)
-- [In the future](#in-the-future)
 
 ## About
 
 **soupsavvy** is a library designed to make web scraping tasks more efficient and manageable. Automating web scraping can be a thankless and time-consuming job. It builds around [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) library enabling developers to create more complex workflows and advanced searches with ease.
 
 ## Key Features
 
@@ -138,42 +136,47 @@
 ```
 
 with savvier version:
 
 ```python
 import re
 
-from soupsavvy import AttributeTag, ElementTag, PatternElementTag, StepsElementTag
+from soupsavvy import (
+    AttributeSelector,
+    DescendantCombinator,
+    PatternSelector,
+    TagSelector,
+)
 
-# define your complex tag once
-tag = StepsElementTag(
-    ElementTag(
+# define your complex selector once
+selector = DescendantCombinator(
+    TagSelector(
         "div",
         attributes=[
-            AttributeTag(name="class", value="menu"),
-            AttributeTag(name="role", value="search"),
+            AttributeSelector(name="class", value="menu"),
+            AttributeSelector(name="role", value="search"),
         ],
     ),
-    PatternElementTag(
-        tag=ElementTag(
+    PatternSelector(
+        tag=TagSelector(
             "a",
             attributes=[
-                AttributeTag(name="class", value="option"),
-                AttributeTag(name="href", value="github.com", re=True),
+                AttributeSelector(name="class", value="option"),
+                AttributeSelector(name="href", value="github.com", re=True),
             ],
         ),
         pattern="Github",
         re=True,
     ),
 )
 # reuse it in any place to search for tag in any markup, if not found, strict mode raises exception
-a = tag.find(markup, strict=True)
+element = selector.find(markup, strict=True)
 ```
 
-This streamlined soupsavvy approach and encapsulating complex tag(s) into single objects transforms web scraping tasks from a potential 'soup sandwich'🥪 into a 'duck soup' 🦆 scenario.
+This streamlined soupsavvy approach and encapsulating complex selector(s) into single objects.
 
 With soupsavvy's robust features, developers can avoid common problems encountered in web scraping, such as exception handling or integration with type checkers.
 
 Full documentation can be found at **[soupsavvy Docs](https://sewcio543.github.io/soupsavvy/)**
 
 ## Contributing
 
@@ -188,14 +191,7 @@
 
 Soupsavvy is built upon the foundation of excellent BeautifulSoup. We extend our gratitude to the developers and contributors of this projects for their invaluable contributions to the Python community and making our life a lot easier!
 
 -----------------
 
 **Let's soap this soup!**  
 **Happy scraping!** ✨
-
-## In the future
-
-- Scraping workflows from soup to nuts
-- New Tag components
-- Enhanced CI pipeline
-- Documentation
```

### Comparing `soupsavvy-0.1.5/README.md` & `soupsavvy-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# soupsavvy
+![SoupSavvy](resources/logo.png)
+========
 
------------------
-
-## Python package that makes web-scraping more manageable
+## Python package that makes web-scraping better than ever
 
 | | |
 | --- | --- |
 | Package | ![Deployment PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/production_release.yml/badge.svg) [![GitHub](https://img.shields.io/badge/GitHub-sewcio543-181717.svg?style=flat&logo=github)](https://github.com/sewcio543) [![PyPI](https://img.shields.io/pypi/v/soupsavvy?color=orange)](https://pypi.org/project/soupsavvy/) [![Python Versions](https://img.shields.io/pypi/pyversions/soupsavvy)](https://www.python.org/)|
 | Testing | ![Tests](https://github.com/sewcio543/soupsavvy/actions/workflows/tests.yml/badge.svg) [![Codecov](https://codecov.io/gh/sewcio543/soupsavvy/graph/badge.svg?token=RZ51VS3QLB)](https://codecov.io/gh/sewcio543/soupsavvy)|
 | Code Quality | ![Build](https://github.com/sewcio543/soupsavvy/actions/workflows/build_package.yml/badge.svg) ![Linting](https://github.com/sewcio543/soupsavvy/actions/workflows/linting.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sewcio543/soupsavvy/main.svg)](https://results.pre-commit.ci/latest/github/sewcio543/soupsavvy/main)|
 | Documentation | [![readthedocs](https://img.shields.io/readthedocs/pip?logo=readthedocs)](https://github.com/sewcio543/soupsavvy/actions/workflows/documentation.yml/badge.svg) [![Docs link](https://img.shields.io/badge/docs-check_out-blue)](https://sewcio543.github.io/soupsavvy/)|
@@ -16,15 +15,14 @@
 - [About](#about)
 - [Key features](#key-features)
 - [Instalation](#installation)
 - [Usage](#usage)
 - [Contributing](#contributing)
 - [License](#license)
 - [Acknowledgements](#acknowledgements)
-- [In the future](#in-the-future)
 
 ## About
 
 **soupsavvy** is a library designed to make web scraping tasks more efficient and manageable. Automating web scraping can be a thankless and time-consuming job. It builds around [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) library enabling developers to create more complex workflows and advanced searches with ease.
 
 ## Key Features
 
@@ -84,42 +82,47 @@
 ```
 
 with savvier version:
 
 ```python
 import re
 
-from soupsavvy import AttributeTag, ElementTag, PatternElementTag, StepsElementTag
+from soupsavvy import (
+    AttributeSelector,
+    DescendantCombinator,
+    PatternSelector,
+    TagSelector,
+)
 
-# define your complex tag once
-tag = StepsElementTag(
-    ElementTag(
+# define your complex selector once
+selector = DescendantCombinator(
+    TagSelector(
         "div",
         attributes=[
-            AttributeTag(name="class", value="menu"),
-            AttributeTag(name="role", value="search"),
+            AttributeSelector(name="class", value="menu"),
+            AttributeSelector(name="role", value="search"),
         ],
     ),
-    PatternElementTag(
-        tag=ElementTag(
+    PatternSelector(
+        tag=TagSelector(
             "a",
             attributes=[
-                AttributeTag(name="class", value="option"),
-                AttributeTag(name="href", value="github.com", re=True),
+                AttributeSelector(name="class", value="option"),
+                AttributeSelector(name="href", value="github.com", re=True),
             ],
         ),
         pattern="Github",
         re=True,
     ),
 )
 # reuse it in any place to search for tag in any markup, if not found, strict mode raises exception
-a = tag.find(markup, strict=True)
+element = selector.find(markup, strict=True)
 ```
 
-This streamlined soupsavvy approach and encapsulating complex tag(s) into single objects transforms web scraping tasks from a potential 'soup sandwich'🥪 into a 'duck soup' 🦆 scenario.
+This streamlined soupsavvy approach and encapsulating complex selector(s) into single objects.
 
 With soupsavvy's robust features, developers can avoid common problems encountered in web scraping, such as exception handling or integration with type checkers.
 
 Full documentation can be found at **[soupsavvy Docs](https://sewcio543.github.io/soupsavvy/)**
 
 ## Contributing
 
@@ -134,14 +137,7 @@
 
 Soupsavvy is built upon the foundation of excellent BeautifulSoup. We extend our gratitude to the developers and contributors of this projects for their invaluable contributions to the Python community and making our life a lot easier!
 
 -----------------
 
 **Let's soap this soup!**  
 **Happy scraping!** ✨
-
-## In the future
-
-- Scraping workflows from soup to nuts
-- New Tag components
-- Enhanced CI pipeline
-- Documentation
```

### Comparing `soupsavvy-0.1.5/pyproject.toml` & `soupsavvy-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.5/soupsavvy/tags/__init__.py` & `soupsavvy-0.1.6/soupsavvy/tags/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 from .combinators import SubsequentSiblingCombinator
 from .components import AndSelector
 from .components import AndSelector as AndElementTag
 from .components import AnyTagSelector
 from .components import AnyTagSelector as AnyTag
 from .components import AttributeSelector
 from .components import AttributeSelector as AttributeTag
+from .components import HasSelector
 from .components import NotSelector
 from .components import NotSelector as NotElementTag
 from .components import PatternSelector
 from .components import PatternSelector as PatternElementTag
 from .components import TagSelector
 from .components import TagSelector as ElementTag
+from .relative import Anchor
 
 __all__ = [
     "AnyTagSelector",
     "AttributeSelector",
     "TagSelector",
     "PatternSelector",
     "SelectorList",
@@ -34,8 +36,10 @@
     "StepElementTag",
     "AndElementTag",
     "NotElementTag",
     "AnyTag",
     "AttributeTag",
     "ElementTag",
     "PatternElementTag",
+    "HasSelector",
+    "Anchor",
 ]
```

### Comparing `soupsavvy-0.1.5/soupsavvy/tags/base.py` & `soupsavvy-0.1.6/soupsavvy/tags/base.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.5/soupsavvy/tags/combinators.py` & `soupsavvy-0.1.6/soupsavvy/tags/combinators.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,28 +17,127 @@
 
 Notes
 -----
 For more information on CSS combinators see:
 https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors/Combinators
 """
 
+from abc import abstractmethod
 from dataclasses import dataclass
 from functools import reduce
-from itertools import chain, product
-from typing import Optional
+from typing import Optional, Type
 
 from bs4 import Tag
 
 from soupsavvy.tags.base import IterableSoup, SelectableSoup
 from soupsavvy.tags.namespace import FindResult
-from soupsavvy.tags.tag_utils import UniqueTag
+from soupsavvy.tags.relative import (
+    RelativeChild,
+    RelativeDescendant,
+    RelativeNextSibling,
+    RelativeSelector,
+    RelativeSubsequentSibling,
+)
+from soupsavvy.tags.tag_utils import TagResultSet
+
+
+class BaseCombinator(SelectableSoup, IterableSoup):
+    def __init__(
+        self,
+        selector1: SelectableSoup,
+        selector2: SelectableSoup,
+        /,
+        *selectors: SelectableSoup,
+    ) -> None:
+        """
+        Initializes Combinator object with provided positional arguments.
+        At least two SelectableSoup object are required to create Combinator.
+
+        Parameters
+        ----------
+        selectors: SelectableSoup
+            SelectableSoup objects to match accepted as positional arguments.
+
+        Notes
+        -----
+        Object can be initialized with more than two SelectableSoup objects,
+        which would be equal to chaining multiple combinators of the same type.
+
+        For example, chaining child combinator in css:
+
+        Example
+        -------
+        >>> div > a > span
+
+        translated to soupsavvy would be:
+
+        Example
+        -------
+        >>> ChildCombinator(ElementTag("div"), ElementTag("a"), ElementTag("span"))
+
+        Raises
+        ------
+        NotSelectableSoupException
+            If any of provided parameters is not an instance of SelectableSoup.
+        """
+        super().__init__([selector1, selector2, *selectors])
+
+    @property
+    @abstractmethod
+    def _selector(self) -> Type[RelativeSelector]:
+        """
+        Returns type of the relative selector that is used
+        to perform a single step search in the combinator selector.
+
+        Returns
+        -------
+        Type[RelativeSelector]
+            Type of the relative selector that is used in the combinator.
+            Selector instance of this type is initialized
+            with each step in the combinator.
+        """
+        raise NotImplementedError(
+            f"{self.__class__.__name__} is a base class "
+            "and does not implement '_selector' property."
+        )
+
+    def find_all(
+        self,
+        tag: Tag,
+        recursive: bool = True,
+        limit: Optional[int] = None,
+    ) -> list[Tag]:
+        elements: list[Tag] = []
+
+        for i, step in enumerate(self.steps):
+            if i == 0:
+                # only first step follows recursive rule
+                elements = step.find_all(tag, recursive=recursive)
+                continue
+
+            if not elements:
+                break
+
+            selector = self._selector(step)
+            results = TagResultSet(
+                reduce(
+                    list.__add__,
+                    # each relative selector has defined recursive behavior
+                    (selector.find_all(element) for element in elements),
+                )
+            )
+
+            n = limit if i + 1 == len(self.steps) else None
+            elements = results.fetch(n)
+
+        return elements
 
 
 @dataclass(init=False)
-class ChildCombinator(SelectableSoup, IterableSoup):
+class ChildCombinator(BaseCombinator):
     """
     Class representing a child combinator in CSS selectors.
 
     Example
     -------
     >>> ChildCombinator(ElementTag("div"), ElementTag("a"))
 
@@ -79,80 +178,21 @@
 
     Notes
     -----
     For more information on child combinator see:
     https://developer.mozilla.org/en-US/docs/Web/CSS/Child_combinator
     """
 
-    def __init__(
-        self,
-        tag1: SelectableSoup,
-        tag2: SelectableSoup,
-        /,
-        *tags: SelectableSoup,
-    ) -> None:
-        """
-        Initializes ChildCombinator object with provided positional arguments as tags.
-        At least two SelectableSoup objects are required to create ChildCombinator.
-
-        Parameters
-        ----------
-        tags: SelectableSoup
-            SelectableSoup objects to match accepted as positional arguments.
-            At least two SelectableSoup objects are required to create ChildCombinator.
-
-        Notes
-        -----
-        Object can be initialized with more than two SelectableSoup objects,
-        which would be equal to chaining multiple child combinators.
-
-        Example
-        -------
-        >>> div > a > span
-
-        translates to soupsavvy would be:
-
-        Example
-        -------
-        >>> ChildCombinator(ElementTag("div"), ElementTag("a"), ElementTag("span"))
-
-        Raises
-        ------
-        NotSelectableSoupException
-            If any of provided parameters is not an instance of SelectableSoup.
-        """
-        super().__init__([tag1, tag2, *tags])
-
-    def find_all(
-        self,
-        tag: Tag,
-        recursive: bool = True,
-        limit: Optional[int] = None,
-    ) -> list[Tag]:
-        elements = [tag]
-
-        for i, step in enumerate(self.steps):
-            # only first step follows recursive rule, the rest are not recursive
-            # to match only direct children
-            recursive_ = recursive if i == 0 else False
-
-            elements = reduce(
-                list.__add__,
-                (step.find_all(element, recursive=recursive_) for element in elements),
-            )
-
-            # break if no elements were found in the step
-            if not elements:
-                break
-
-        return elements[:limit]
+    @property
+    def _selector(self) -> Type[RelativeSelector]:
+        return RelativeChild
 
 
 @dataclass(init=False)
-class NextSiblingCombinator(SelectableSoup, IterableSoup):
+class NextSiblingCombinator(BaseCombinator):
     """
     Class representing a next sibling combinator in CSS selectors.
 
     Example
     -------
     >>> NextSiblingCombinator(ElementTag("div"), ElementTag("a"))
 
@@ -183,86 +223,21 @@
     -----
     For more information on next sibling combinator see:
     https://developer.mozilla.org/en-US/docs/Web/CSS/Next-sibling_combinator
 
     This is also known as the adjacent sibling combinator.
     """
 
-    def __init__(
-        self,
-        tag1: SelectableSoup,
-        tag2: SelectableSoup,
-        /,
-        *tags: SelectableSoup,
-    ) -> None:
-        """
-        Initializes SubsequentSiblingCombinator object with provided
-        positional arguments as tags. At least two SelectableSoup object are required
-        to create SubsequentSiblingCombinator.
-
-        Parameters
-        ----------
-        tags: SelectableSoup
-            SelectableSoup objects to match accepted as positional arguments.
-            At least two SelectableSoup objects are required
-            to create SubsequentSiblingCombinator.
-
-        Raises
-        ------
-        NotSelectableSoupException
-            If any of provided parameters is not an instance of SelectableSoup.
-        """
-        super().__init__([tag1, tag2, *tags])
-
-    def find_all(
-        self,
-        tag: Tag,
-        recursive: bool = True,
-        limit: Optional[int] = None,
-    ) -> list[Tag]:
-
-        elements = [tag]
-
-        for i, step in enumerate(self.steps):
-            if i == 0:
-                # only first step follows recursive rule
-                elements = step.find_all(elements[0], recursive=recursive)
-                continue
-
-            matching = {
-                UniqueTag(element)
-                for tag in elements
-                for element in step.find_all(tag.parent or tag, recursive=False)
-            }
-
-            next_siblings = [
-                UniqueTag(tag.find_next_sibling()) for tag in elements  # type: ignore
-            ]
-
-            matches: list[UniqueTag] = []
-            last_step = i + 1 == len(self.steps)
-
-            for element in next_siblings:
-                if element in matching and element not in matches:
-                    matches.append(element)
-
-                    if len(matches) == limit and last_step:
-                        break
-
-            elements = [element.tag for element in matches]
-
-            # break if no elements were found in the step
-            if not elements:
-                break
-
-        return elements
+    @property
+    def _selector(self) -> Type[RelativeSelector]:
+        return RelativeNextSibling
 
 
 @dataclass(init=False)
-class SubsequentSiblingCombinator(SelectableSoup, IterableSoup):
+class SubsequentSiblingCombinator(BaseCombinator):
     """
     Class representing a subsequent sibling combinator in CSS selectors.
     Subsequent sibling combinator separates two selectors
     and matches all instances of the second element that follow the first element
     (not necessarily immediately) and share the same parent element.
 
     Example
@@ -297,88 +272,21 @@
     -----
     For more information on subsequent sibling combinator see:
     https://developer.mozilla.org/en-US/docs/Web/CSS/Subsequent-sibling_combinator
 
     This is also known as the general sibling combinator.
     """
 
-    def __init__(
-        self,
-        tag1: SelectableSoup,
-        tag2: SelectableSoup,
-        /,
-        *tags: SelectableSoup,
-    ) -> None:
-        """
-        Initializes SubsequentSiblingCombinator object with provided
-        positional arguments as tags. At least two SelectableSoup object are required
-        to create SubsequentSiblingCombinator.
-
-        Parameters
-        ----------
-        tags: SelectableSoup
-            SelectableSoup objects to match accepted as positional arguments.
-            At least two SelectableSoup objects are required
-            to create SubsequentSiblingCombinator.
-
-        Raises
-        ------
-        NotSelectableSoupException
-            If any of provided parameters is not an instance of SelectableSoup.
-        """
-        super().__init__([tag1, tag2, *tags])
-
-    def find_all(
-        self,
-        tag: Tag,
-        recursive: bool = True,
-        limit: Optional[int] = None,
-    ) -> list[Tag]:
-
-        elements = [tag]
-
-        for i, step in enumerate(self.steps):
-            if i == 0:
-                # only first step follows recursive rule
-                elements = step.find_all(elements[0], recursive=recursive)
-                continue
-
-            matching = {
-                UniqueTag(element)
-                for tag in elements
-                for element in step.find_all(tag.parent or tag, recursive=False)
-            }
-
-            next_siblings = [
-                UniqueTag(sibling)  # type: ignore
-                for tag in elements
-                for sibling in tag.find_next_siblings()
-            ]
-
-            matches: list[UniqueTag] = []
-            last_step = i + 1 == len(self.steps)
-
-            for element in next_siblings:
-                if element in matching and element not in matches:
-                    matches.append(element)
-
-                    if len(matches) == limit and last_step:
-                        break
-
-            elements = [element.tag for element in matches]
-
-            # break if no elements were found in the step
-            if not elements:
-                break
-
-        return elements
+    @property
+    def _selector(self) -> Type[RelativeSelector]:
+        return RelativeSubsequentSibling
 
 
 @dataclass(init=False)
-class DescendantCombinator(SelectableSoup, IterableSoup):
+class DescendantCombinator(BaseCombinator):
     """
     Class representing a descent combinator in CSS selectors.
     Descent combinator separates two selectors and matches all instances
     of the second element that are descendants of the first element.
 
     Two SelectableSoup objects are required to create DescentCombinator,
     but more can be provided as positional arguments, which binds them
@@ -419,59 +327,17 @@
 
     Notes
     -----
     For more information on subsequent sibling combinator see:
     https://developer.mozilla.org/en-US/docs/Web/CSS/Descendant_combinator
     """
 
-    def __init__(
-        self,
-        tag1: SelectableSoup,
-        tag2: SelectableSoup,
-        /,
-        *tags: SelectableSoup,
-    ) -> None:
-        """
-        Initializes DescentCombinator object with provided positional arguments as tags.
-        At least two SelectableSoup object required to create DescentCombinator.
-
-        Parameters
-        ----------
-        tags: SelectableSoup
-            SelectableSoup objects to match accepted as positional arguments.
-            At least two SelectableSoup objects are required to create DescentCombinator.
-
-        Raises
-        ------
-        NotSelectableSoupException
-            If any of provided parameters is not an instance of SelectableSoup.
-        """
-        super().__init__([tag1, tag2, *tags])
-
-    def find_all(
-        self,
-        tag: Tag,
-        recursive: bool = True,
-        limit: Optional[int] = None,
-    ) -> list[Tag]:
-        elements = [tag]
-
-        for i, step in enumerate(self.steps):
-            # only first step follows recursive rule
-            recursive_ = recursive if i == 0 else True
-
-            elements = reduce(
-                list.__add__,
-                (step.find_all(element, recursive=recursive_) for element in elements),
-            )
-            # break if no elements were found in the step
-            if not elements:
-                break
-
-        return elements[:limit]
+    @property
+    def _selector(self) -> Type[RelativeSelector]:
+        return RelativeDescendant
 
 
 @dataclass(init=False)
 class SelectorList(SelectableSoup, IterableSoup):
     """
     Class representing a list of selectors in CSS,
     a selector list is a comma-separated list of selectors,
@@ -519,54 +385,64 @@
     -------
     >>> ElementTag(tag="a") | ElementTag("div", [AttributeTag(name="class", value="widget")])
 
     Which is equivalent to the first example.
 
     Notes
     -----
+    This Combinator does not inherit from BaseCombinator,
+    as its logic differs from other combinators.
+
     For more information on selector list see:
     https://developer.mozilla.org/en-US/docs/Web/CSS/Selector_list
     """
 
     def __init__(
         self,
-        tag1: SelectableSoup,
-        tag2: SelectableSoup,
+        selector1: SelectableSoup,
+        selector2: SelectableSoup,
         /,
-        *tags: SelectableSoup,
+        *selectors: SelectableSoup,
     ) -> None:
         """
-        Initializes SelectorList object with provided positional arguments as tags.
+        Initializes SelectorList object with provided positional arguments.
         At least two SelectableSoup objects are required to create SelectorList.
 
         Parameters
         ----------
-        tags: SelectableSoup
+        selectors: SelectableSoup
             SelectableSoup objects to match accepted as positional arguments.
 
         Raises
         ------
         NotSelectableSoupException
             If any of provided parameters is not an instance of SelectableSoup.
         """
-        super().__init__([tag1, tag2, *tags])
+        super().__init__([selector1, selector2, *selectors])
 
     def _find(self, tag: Tag, recursive: bool = True) -> FindResult:
         # iterates all tags and returns first element that matches
-        for _tag_ in self.steps:
-            result = _tag_.find(tag, recursive=recursive)
+        for selector in self.steps:
+            result = selector.find(tag, recursive=recursive)
 
             if result is not None:
                 return result
 
         return None
 
     def find_all(
         self,
         tag: Tag,
         recursive: bool = True,
         limit: Optional[int] = None,
     ) -> list[Tag]:
-        return reduce(
-            list.__add__,
-            (_tag_.find_all(tag, recursive=recursive) for _tag_ in self.steps),
-        )[:limit]
+        results = TagResultSet()
+
+        for selector in self.steps:
+            results |= TagResultSet(
+                selector.find_all(tag, recursive=recursive),
+            )
+
+            if limit and len(results) >= limit:
+                break
+
+        return results.fetch(limit)
```

### Comparing `soupsavvy-0.1.5/soupsavvy/tags/components.py` & `soupsavvy-0.1.6/soupsavvy/tags/components.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from soupsavvy.tags.base import (
     IterableSoup,
     SelectableCSS,
     SelectableSoup,
     SingleSelectableSoup,
 )
 from soupsavvy.tags.exceptions import WildcardTagException
+from soupsavvy.tags.relative import RelativeSelector
 from soupsavvy.tags.tag_utils import TagIterator, UniqueTag
 
 
 @dataclass
 class AttributeSelector(SingleSelectableSoup, SelectableCSS):
     """
     Class representing attribute of the HTML element.
@@ -347,15 +348,15 @@
         self,
         tag: SelectableSoup,
         /,
         *tags: SelectableSoup,
     ) -> None:
         """
         Initializes NotSelectors object with provided positional arguments as tags.
-        At least one SelectableSoup object is required to create NotSelectors.
+        At least one SelectableSoup object is required to create NotSelector.
 
         Parameters
         ----------
         tags: SelectableSoup
             SelectableSoup objects to negate match accepted as positional arguments.
 
         Raises
@@ -451,15 +452,15 @@
         tag1: SelectableSoup,
         tag2: SelectableSoup,
         /,
         *tags: SelectableSoup,
     ) -> None:
         """
         Initializes AndTagSelector object with provided positional arguments as tags.
-        At least two SelectableSoup objects are required to create AndTagSelector.
+        At least two SelectableSoup objects are required to create AndSelector.
 
         Parameters
         ----------
         tags: SelectableSoup
             SelectableSoup objects to match accepted as positional arguments.
 
         Raises
@@ -486,7 +487,130 @@
             step_elements = [
                 UniqueTag(element)
                 for element in step.find_all(tag, recursive=recursive)
             ]
             matching = [element for element in matching if element in step_elements]
 
         return [element.tag for element in matching][:limit]
+
+
+@dataclass(init=False)
+class HasSelector(SelectableSoup, IterableSoup):
+    """
+    Class representing elements selected with respect to matching reference elements.
+    Element is selected if any of the provided selectors matched reference element.
+
+    Example
+    -------
+    >>> HasSelector(TagSelector(tag="div"))
+
+    matches all elements that have any descendant with "div" tag name.
+    It uses default combinator of relative selector, which is descendant.
+
+    Example
+    -------
+    >>> <span><div>Hello World</div></span> ✔️
+    >>> <span><a>Hello World</a></span> ❌
+
+    Other relative selectors can be used with Anchor element.
+
+    Example
+    -------
+    >>> from soupsavvy.tags.relative import Anchor
+    >>> HasSelector(Anchor > TagSelector("div"))
+    >>> HasSelector(Anchor + TagSelector("div"))
+
+    or by using RelativeSelector components directly:
+
+    Example
+    -------
+    >>> from soupsavvy.tags.relative import RelativeChild, RelativeNextSibling
+    >>> HasSelector(RelativeChild(TagSelector("div")))
+    >>> HasSelector(RelativeNextSibling(TagSelector("div"))
+
+    Example
+    -------
+    >>> <span><div>Hello World</div></span> ✔️
+    >>> <span><a><div>Hello World</div></a></span> ❌
+
+    In this case, HasSelector is anchored against any element, and matches only elements
+    that have "div" tag name as a child.
+
+    Object can be initialized with multiple selectors as well, in which case
+    at least one selector must match for element to be included in the result.
+
+    This is an equivalent of CSS :has() pseudo-class,
+    that represents elements if any of the relative selectors that are passed as an argument
+    match at least one element when anchored against this element.
+
+    Example
+    -------
+    >>> :has(div, a) { color: red; }
+    >>> :has(+ div, > a) { color: red; }
+
+    These examples translated to soupsavvy would be:
+
+    Example
+    -------
+    >>> from soupsavvy.tags.relative import Anchor
+    >>> HasSelector(TagSelector("div"), TagSelector("a"))
+    >>> HasSelector(Anchor + TagSelector("div"), Anchor > TagSelector("a"))
+
+    Notes
+    -----
+    Passing RelativeDescendant selector into HasSelector is equivalent to using
+    its selector directly, as descendant combinator is default option.
+
+    Example
+    -------
+    >>> HasSelector(RelativeDescendant(TagSelector("div")))
+    >>> HasSelector(Anchor > TagSelector("div"))
+    >>> HasSelector(TagSelector("div"))
+
+    Three of the above examples are equivalent.
+
+    For more information on :has() pseudo-class see:
+    https://developer.mozilla.org/en-US/docs/Web/CSS/:has
+    """
+
+    def __init__(
+        self,
+        selector: SelectableSoup,
+        /,
+        *selectors: SelectableSoup,
+    ) -> None:
+        """
+        Initializes AndTagSelector object with provided positional arguments as tags.
+        At least two SelectableSoup objects are required to create HasSelector.
+
+        Parameters
+        ----------
+        tags: SelectableSoup
+            SelectableSoup objects to match accepted as positional arguments.
+            At least one selector is required to create HasSelector.
+
+        Raises
+        ------
+        NotSelectableSoupException
+            If any of provided parameters is not an instance of SelectableSoup.
+        """
+        super().__init__([selector, *selectors])
+
+    def find_all(
+        self,
+        tag: Tag,
+        recursive: bool = True,
+        limit: Optional[int] = None,
+    ) -> list[Tag]:
+
+        elements = TagIterator(tag, recursive=recursive)
+        matching: list[Tag] = []
+
+        for element in elements:
+            # we only care if anything matching was found
+            if any(step.find(element) for step in self.steps):
+                matching.append(element)
+
+                if len(matching) == limit:
+                    break
+
+        return matching
```

### Comparing `soupsavvy-0.1.5/soupsavvy/tags/css/tag_selectors.py` & `soupsavvy-0.1.6/soupsavvy/tags/css/tag_selectors.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.5/soupsavvy/tags/exceptions.py` & `soupsavvy-0.1.6/soupsavvy/tags/exceptions.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.5/soupsavvy/tags/namespace.py` & `soupsavvy-0.1.6/soupsavvy/tags/namespace.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.5/soupsavvy/testing/generators/base.py` & `soupsavvy-0.1.6/soupsavvy/testing/generators/base.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.5/soupsavvy/testing/generators/exceptions.py` & `soupsavvy-0.1.6/soupsavvy/testing/generators/exceptions.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.5/soupsavvy/testing/generators/generators.py` & `soupsavvy-0.1.6/soupsavvy/testing/generators/generators.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.5/soupsavvy/testing/generators/templates/base.py` & `soupsavvy-0.1.6/soupsavvy/testing/generators/templates/base.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.5/soupsavvy/testing/generators/templates/templates.py` & `soupsavvy-0.1.6/soupsavvy/testing/generators/templates/templates.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.5/soupsavvy/utils/deprecation.py` & `soupsavvy-0.1.6/soupsavvy/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `soupsavvy-0.1.5/soupsavvy.egg-info/PKG-INFO` & `soupsavvy-0.1.6/soupsavvy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soupsavvy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package for advanced web scraping
 Author: sewcio543
 License: MIT License
         
         Copyright (c) 2024 Wojciech Seweryn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,19 +48,18 @@
 Requires-Dist: coverage==7.2.2; extra == "dev"
 Requires-Dist: flake8==7.0.0; extra == "dev"
 Requires-Dist: mypy==1.7.0; extra == "dev"
 Requires-Dist: pre-commit==3.6.1; extra == "dev"
 Requires-Dist: pytest==7.1.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 
-# soupsavvy
+![SoupSavvy](resources/logo.png)
+========
 
------------------
-
-## Python package that makes web-scraping more manageable
+## Python package that makes web-scraping better than ever
 
 | | |
 | --- | --- |
 | Package | ![Deployment PyPI](https://github.com/sewcio543/soupsavvy/actions/workflows/production_release.yml/badge.svg) [![GitHub](https://img.shields.io/badge/GitHub-sewcio543-181717.svg?style=flat&logo=github)](https://github.com/sewcio543) [![PyPI](https://img.shields.io/pypi/v/soupsavvy?color=orange)](https://pypi.org/project/soupsavvy/) [![Python Versions](https://img.shields.io/pypi/pyversions/soupsavvy)](https://www.python.org/)|
 | Testing | ![Tests](https://github.com/sewcio543/soupsavvy/actions/workflows/tests.yml/badge.svg) [![Codecov](https://codecov.io/gh/sewcio543/soupsavvy/graph/badge.svg?token=RZ51VS3QLB)](https://codecov.io/gh/sewcio543/soupsavvy)|
 | Code Quality | ![Build](https://github.com/sewcio543/soupsavvy/actions/workflows/build_package.yml/badge.svg) ![Linting](https://github.com/sewcio543/soupsavvy/actions/workflows/linting.yml/badge.svg) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sewcio543/soupsavvy/main.svg)](https://results.pre-commit.ci/latest/github/sewcio543/soupsavvy/main)|
 | Documentation | [![readthedocs](https://img.shields.io/readthedocs/pip?logo=readthedocs)](https://github.com/sewcio543/soupsavvy/actions/workflows/documentation.yml/badge.svg) [![Docs link](https://img.shields.io/badge/docs-check_out-blue)](https://sewcio543.github.io/soupsavvy/)|
@@ -70,15 +69,14 @@
 - [About](#about)
 - [Key features](#key-features)
 - [Instalation](#installation)
 - [Usage](#usage)
 - [Contributing](#contributing)
 - [License](#license)
 - [Acknowledgements](#acknowledgements)
-- [In the future](#in-the-future)
 
 ## About
 
 **soupsavvy** is a library designed to make web scraping tasks more efficient and manageable. Automating web scraping can be a thankless and time-consuming job. It builds around [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) library enabling developers to create more complex workflows and advanced searches with ease.
 
 ## Key Features
 
@@ -138,42 +136,47 @@
 ```
 
 with savvier version:
 
 ```python
 import re
 
-from soupsavvy import AttributeTag, ElementTag, PatternElementTag, StepsElementTag
+from soupsavvy import (
+    AttributeSelector,
+    DescendantCombinator,
+    PatternSelector,
+    TagSelector,
+)
 
-# define your complex tag once
-tag = StepsElementTag(
-    ElementTag(
+# define your complex selector once
+selector = DescendantCombinator(
+    TagSelector(
         "div",
         attributes=[
-            AttributeTag(name="class", value="menu"),
-            AttributeTag(name="role", value="search"),
+            AttributeSelector(name="class", value="menu"),
+            AttributeSelector(name="role", value="search"),
         ],
     ),
-    PatternElementTag(
-        tag=ElementTag(
+    PatternSelector(
+        tag=TagSelector(
             "a",
             attributes=[
-                AttributeTag(name="class", value="option"),
-                AttributeTag(name="href", value="github.com", re=True),
+                AttributeSelector(name="class", value="option"),
+                AttributeSelector(name="href", value="github.com", re=True),
             ],
         ),
         pattern="Github",
         re=True,
     ),
 )
 # reuse it in any place to search for tag in any markup, if not found, strict mode raises exception
-a = tag.find(markup, strict=True)
+element = selector.find(markup, strict=True)
 ```
 
-This streamlined soupsavvy approach and encapsulating complex tag(s) into single objects transforms web scraping tasks from a potential 'soup sandwich'🥪 into a 'duck soup' 🦆 scenario.
+This streamlined soupsavvy approach and encapsulating complex selector(s) into single objects.
 
 With soupsavvy's robust features, developers can avoid common problems encountered in web scraping, such as exception handling or integration with type checkers.
 
 Full documentation can be found at **[soupsavvy Docs](https://sewcio543.github.io/soupsavvy/)**
 
 ## Contributing
 
@@ -188,14 +191,7 @@
 
 Soupsavvy is built upon the foundation of excellent BeautifulSoup. We extend our gratitude to the developers and contributors of this projects for their invaluable contributions to the Python community and making our life a lot easier!
 
 -----------------
 
 **Let's soap this soup!**  
 **Happy scraping!** ✨
-
-## In the future
-
-- Scraping workflows from soup to nuts
-- New Tag components
-- Enhanced CI pipeline
-- Documentation
```

### Comparing `soupsavvy-0.1.5/soupsavvy.egg-info/SOURCES.txt` & `soupsavvy-0.1.6/soupsavvy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 soupsavvy.egg-info/top_level.txt
 soupsavvy/tags/__init__.py
 soupsavvy/tags/base.py
 soupsavvy/tags/combinators.py
 soupsavvy/tags/components.py
 soupsavvy/tags/exceptions.py
 soupsavvy/tags/namespace.py
+soupsavvy/tags/relative.py
 soupsavvy/tags/tag_utils.py
 soupsavvy/tags/css/__init__.py
+soupsavvy/tags/css/api.py
 soupsavvy/tags/css/exceptions.py
 soupsavvy/tags/css/tag_selectors.py
 soupsavvy/testing/__init__.py
 soupsavvy/testing/generators/__init__.py
 soupsavvy/testing/generators/base.py
 soupsavvy/testing/generators/exceptions.py
 soupsavvy/testing/generators/generators.py
```

