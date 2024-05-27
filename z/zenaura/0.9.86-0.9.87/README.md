# Comparing `tmp/zenaura-0.9.86.tar.gz` & `tmp/zenaura-0.9.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.86.tar", last modified: Sun May 26 21:29:08 2024, max compression
+gzip compressed data, was "zenaura-0.9.87.tar", last modified: Mon May 27 20:14:03 2024, max compression
```

## Comparing `zenaura-0.9.86.tar` & `zenaura-0.9.87.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 21:29:08.032090 zenaura-0.9.86/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.86/LICENSE
--rw-rw-rw-   0        0        0     2028 2024-05-26 21:29:08.031090 zenaura-0.9.86/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.86/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 21:29:08.032090 zenaura-0.9.86/setup.cfg
--rw-rw-rw-   0        0        0     1135 2024-05-26 21:29:01.000000 zenaura-0.9.86/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:29:07.983590 zenaura-0.9.86/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.86/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6591 2024-05-26 18:57:08.000000 zenaura-0.9.86/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.86/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.86/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.86/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.86/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.86/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.86/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.86/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.86/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.86/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:29:07.984589 zenaura-0.9.86/zenaura/
--rw-rw-rw-   0        0        0        0 2024-05-26 19:08:09.000000 zenaura-0.9.86/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:29:07.998088 zenaura-0.9.86/zenaura/client/
--rw-rw-rw-   0        0        0        0 2024-05-26 18:57:31.000000 zenaura-0.9.86/zenaura/client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:29:08.001089 zenaura-0.9.86/zenaura/client/algorithm/
--rw-rw-rw-   0        0        0       39 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/algorithm/__init__.py
--rw-rw-rw-   0        0        0      193 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/algorithm/algorithm.py
--rw-rw-rw-   0        0        0      972 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/algorithm/operations.py
--rw-rw-rw-   0        0        0     7166 2024-05-26 18:57:08.000000 zenaura-0.9.86/zenaura/client/algorithm/searcher.py
--rw-rw-rw-   0        0        0     2772 2024-05-26 18:57:08.000000 zenaura-0.9.86/zenaura/client/algorithm/updater.py
--rw-rw-rw-   0        0        0     8990 2024-05-26 18:57:08.000000 zenaura-0.9.86/zenaura/client/app.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:29:08.003589 zenaura-0.9.86/zenaura/client/compiler/
--rw-rw-rw-   0        0        0       53 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/compiler/__init__.py
--rw-rw-rw-   0        0        0     1403 2024-05-26 18:57:08.000000 zenaura-0.9.86/zenaura/client/compiler/attribute.py
--rw-rw-rw-   0        0        0     3471 2024-05-26 18:57:08.000000 zenaura-0.9.86/zenaura/client/compiler/compiler.py
--rw-rw-rw-   0        0        0     1132 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/compiler/sanitize.py
--rw-rw-rw-   0        0        0     4093 2024-05-26 18:57:08.000000 zenaura-0.9.86/zenaura/client/component.py
--rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/config.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:29:08.013091 zenaura-0.9.86/zenaura/client/dom/
--rw-rw-rw-   0        0        0       43 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/dom/__init__.py
--rw-rw-rw-   0        0        0      280 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/dom/dom.py
--rw-rw-rw-   0        0        0     1803 2024-05-26 18:57:08.000000 zenaura-0.9.86/zenaura/client/dom/error.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:29:08.014589 zenaura-0.9.86/zenaura/client/dom/lifecycles/
--rw-rw-rw-   0        0        0      437 2024-05-26 18:57:08.000000 zenaura-0.9.86/zenaura/client/dom/lifecycles/mount.py
--rw-rw-rw-   0        0        0      780 2024-05-26 18:57:08.000000 zenaura-0.9.86/zenaura/client/dom/lifecycles/render.py
--rw-rw-rw-   0        0        0     1852 2024-05-26 20:41:24.000000 zenaura-0.9.86/zenaura/client/dom/mount.py
--rw-rw-rw-   0        0        0     1883 2024-05-26 21:17:10.000000 zenaura-0.9.86/zenaura/client/dom/render.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:29:08.024588 zenaura-0.9.86/zenaura/client/hydrator/
--rw-rw-rw-   0        0        0      235 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/hydrator/__init__.py
--rw-rw-rw-   0        0        0     1895 2024-05-26 18:57:08.000000 zenaura-0.9.86/zenaura/client/hydrator/compiler_adapter.py
--rw-rw-rw-   0        0        0     1236 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/hydrator/hydrator.py
--rw-rw-rw-   0        0        0     1346 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/hydrator/lookup.py
--rw-rw-rw-   0        0        0     6602 2024-05-26 21:28:25.000000 zenaura-0.9.86/zenaura/client/hydrator/real_dom_adapter.py
--rw-rw-rw-   0        0        0     2264 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/hydrator/tasker.py
--rw-rw-rw-   0        0        0     1064 2024-05-26 18:57:08.000000 zenaura-0.9.86/zenaura/client/hydrator/virtual_dom_adapter.py
--rw-rw-rw-   0        0        0     2631 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/mocks.py
--rw-rw-rw-   0        0        0      896 2024-05-26 18:57:08.000000 zenaura-0.9.86/zenaura/client/mutator.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:29:08.026590 zenaura-0.9.86/zenaura/client/observer/
--rw-rw-rw-   0        0        0       60 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/observer/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/observer/observer.py
--rw-rw-rw-   0        0        0     1609 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/observer/subject.py
--rw-rw-rw-   0        0        0     2009 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/observer.py
--rw-rw-rw-   0        0        0      943 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/page.py
--rw-rw-rw-   0        0        0     2212 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/persistance.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:29:08.029091 zenaura-0.9.86/zenaura/client/tags/
--rw-rw-rw-   0        0        0      165 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/tags/__init__.py
--rw-rw-rw-   0        0        0      429 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/tags/attribute.py
--rw-rw-rw-   0        0        0     4666 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/tags/builder.py
--rw-rw-rw-   0        0        0      418 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/tags/data.py
--rw-rw-rw-   0        0        0      473 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/tags/html.py
--rw-rw-rw-   0        0        0    10231 2024-05-26 17:44:57.000000 zenaura-0.9.86/zenaura/client/tags/node.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:29:08.030088 zenaura-0.9.86/zenaura/server/
--rw-rw-rw-   0        0        0       33 2024-05-26 19:08:17.000000 zenaura-0.9.86/zenaura/server/__init__.py
--rw-rw-rw-   0        0        0     1173 2024-05-26 19:24:34.000000 zenaura-0.9.86/zenaura/server/server.py
-drwxrwxrwx   0        0        0        0 2024-05-26 21:29:08.030589 zenaura-0.9.86/zenaura.egg-info/
--rw-rw-rw-   0        0        0     2028 2024-05-26 21:29:07.000000 zenaura-0.9.86/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1867 2024-05-26 21:29:07.000000 zenaura-0.9.86/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 21:29:07.000000 zenaura-0.9.86/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 21:29:07.000000 zenaura-0.9.86/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 21:29:07.000000 zenaura-0.9.86/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 20:14:03.726630 zenaura-0.9.87/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.87/LICENSE
+-rw-rw-rw-   0        0        0     2028 2024-05-27 20:14:03.726130 zenaura-0.9.87/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.87/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-27 20:14:03.726630 zenaura-0.9.87/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2024-05-27 20:13:58.000000 zenaura-0.9.87/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:14:03.691314 zenaura-0.9.87/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.87/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6603 2024-05-27 19:33:16.000000 zenaura-0.9.87/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.87/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.87/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.87/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.87/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.87/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.87/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0     1201 2024-05-27 20:12:21.000000 zenaura-0.9.87/tests/test_server.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.87/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.87/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.87/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:14:03.691814 zenaura-0.9.87/zenaura/
+-rw-rw-rw-   0        0        0        0 2024-05-26 19:08:09.000000 zenaura-0.9.87/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:14:03.706228 zenaura-0.9.87/zenaura/client/
+-rw-rw-rw-   0        0        0        0 2024-05-26 18:57:31.000000 zenaura-0.9.87/zenaura/client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:14:03.709163 zenaura-0.9.87/zenaura/client/algorithm/
+-rw-rw-rw-   0        0        0       39 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/algorithm/__init__.py
+-rw-rw-rw-   0        0        0      193 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/algorithm/algorithm.py
+-rw-rw-rw-   0        0        0      972 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/algorithm/operations.py
+-rw-rw-rw-   0        0        0     7166 2024-05-26 18:57:08.000000 zenaura-0.9.87/zenaura/client/algorithm/searcher.py
+-rw-rw-rw-   0        0        0     2772 2024-05-26 18:57:08.000000 zenaura-0.9.87/zenaura/client/algorithm/updater.py
+-rw-rw-rw-   0        0        0    10263 2024-05-27 19:32:29.000000 zenaura-0.9.87/zenaura/client/app.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:14:03.711162 zenaura-0.9.87/zenaura/client/compiler/
+-rw-rw-rw-   0        0        0       53 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/compiler/__init__.py
+-rw-rw-rw-   0        0        0     1403 2024-05-26 18:57:08.000000 zenaura-0.9.87/zenaura/client/compiler/attribute.py
+-rw-rw-rw-   0        0        0     3471 2024-05-26 18:57:08.000000 zenaura-0.9.87/zenaura/client/compiler/compiler.py
+-rw-rw-rw-   0        0        0     1132 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/compiler/sanitize.py
+-rw-rw-rw-   0        0        0     4093 2024-05-26 18:57:08.000000 zenaura-0.9.87/zenaura/client/component.py
+-rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/config.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:14:03.713661 zenaura-0.9.87/zenaura/client/dom/
+-rw-rw-rw-   0        0        0       43 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/dom/__init__.py
+-rw-rw-rw-   0        0        0      280 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/dom/dom.py
+-rw-rw-rw-   0        0        0     1803 2024-05-26 18:57:08.000000 zenaura-0.9.87/zenaura/client/dom/error.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:14:03.715162 zenaura-0.9.87/zenaura/client/dom/lifecycles/
+-rw-rw-rw-   0        0        0      449 2024-05-27 19:25:39.000000 zenaura-0.9.87/zenaura/client/dom/lifecycles/mount.py
+-rw-rw-rw-   0        0        0      804 2024-05-27 19:26:03.000000 zenaura-0.9.87/zenaura/client/dom/lifecycles/render.py
+-rw-rw-rw-   0        0        0     1488 2024-05-27 19:25:23.000000 zenaura-0.9.87/zenaura/client/dom/mount.py
+-rw-rw-rw-   0        0        0     1883 2024-05-26 21:17:10.000000 zenaura-0.9.87/zenaura/client/dom/render.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:14:03.718626 zenaura-0.9.87/zenaura/client/hydrator/
+-rw-rw-rw-   0        0        0      235 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/hydrator/__init__.py
+-rw-rw-rw-   0        0        0     1895 2024-05-26 18:57:08.000000 zenaura-0.9.87/zenaura/client/hydrator/compiler_adapter.py
+-rw-rw-rw-   0        0        0     1236 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/hydrator/hydrator.py
+-rw-rw-rw-   0        0        0     1346 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/hydrator/lookup.py
+-rw-rw-rw-   0        0        0     7089 2024-05-27 19:20:18.000000 zenaura-0.9.87/zenaura/client/hydrator/real_dom_adapter.py
+-rw-rw-rw-   0        0        0     2264 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/hydrator/tasker.py
+-rw-rw-rw-   0        0        0     1064 2024-05-26 18:57:08.000000 zenaura-0.9.87/zenaura/client/hydrator/virtual_dom_adapter.py
+-rw-rw-rw-   0        0        0     2631 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/mocks.py
+-rw-rw-rw-   0        0        0      896 2024-05-26 18:57:08.000000 zenaura-0.9.87/zenaura/client/mutator.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:14:03.720129 zenaura-0.9.87/zenaura/client/observer/
+-rw-rw-rw-   0        0        0       60 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/observer/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/observer/observer.py
+-rw-rw-rw-   0        0        0     1609 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/observer/subject.py
+-rw-rw-rw-   0        0        0     2009 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/observer.py
+-rw-rw-rw-   0        0        0      810 2024-05-27 18:49:15.000000 zenaura-0.9.87/zenaura/client/page.py
+-rw-rw-rw-   0        0        0     2212 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/persistance.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:14:03.723630 zenaura-0.9.87/zenaura/client/tags/
+-rw-rw-rw-   0        0        0      165 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/tags/__init__.py
+-rw-rw-rw-   0        0        0      429 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/tags/attribute.py
+-rw-rw-rw-   0        0        0     4666 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/tags/builder.py
+-rw-rw-rw-   0        0        0      418 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/tags/data.py
+-rw-rw-rw-   0        0        0      473 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/tags/html.py
+-rw-rw-rw-   0        0        0    10231 2024-05-26 17:44:57.000000 zenaura-0.9.87/zenaura/client/tags/node.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:14:03.725129 zenaura-0.9.87/zenaura/server/
+-rw-rw-rw-   0        0        0       33 2024-05-26 19:08:17.000000 zenaura-0.9.87/zenaura/server/__init__.py
+-rw-rw-rw-   0        0        0     3316 2024-05-27 20:10:51.000000 zenaura-0.9.87/zenaura/server/server.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:14:03.725629 zenaura-0.9.87/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     2028 2024-05-27 20:14:03.000000 zenaura-0.9.87/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1888 2024-05-27 20:14:03.000000 zenaura-0.9.87/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 20:14:03.000000 zenaura-0.9.87/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-27 20:14:03.000000 zenaura-0.9.87/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 20:14:03.000000 zenaura-0.9.87/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.86/LICENSE` & `zenaura-0.9.87/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/PKG-INFO` & `zenaura-0.9.87/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.86
+Version: 0.9.87
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.86/README.md` & `zenaura-0.9.87/README.md`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/setup.py` & `zenaura-0.9.87/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='0.9.86',
+    version='0.9.87',
     description="Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
     packages=['zenaura', 'zenaura.server', 'zenaura.client', 'zenaura.client.algorithm', 'zenaura.client.compiler', 'zenaura.client.hydrator', 'zenaura.client.observer', 'zenaura.client.tags', 'zenaura.client.dom', 'zenaura.client.dom.lifecycles'],
     install_requires=[
         'bleach'
     ],
```

### Comparing `zenaura-0.9.86/tests/test_algorithm.py` & `zenaura-0.9.87/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/tests/test_app.py` & `zenaura-0.9.87/tests/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 import unittest
 from unittest.mock import MagicMock, patch
-from zenaura import Page
+from zenaura.client.page import Page
 
 
 
 sys.modules["pyscript"] = MagicMock()
 
 class TestApp(unittest.TestCase):
```

### Comparing `zenaura-0.9.86/tests/test_compiler.py` & `zenaura-0.9.87/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/tests/test_component_e2e.py` & `zenaura-0.9.87/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/tests/test_component_unit.py` & `zenaura-0.9.87/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/tests/test_node_properties.py` & `zenaura-0.9.87/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/tests/test_observer.py` & `zenaura-0.9.87/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/tests/test_rdom_adapter.py` & `zenaura-0.9.87/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/tests/test_tags.py` & `zenaura-0.9.87/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/tests/test_tasker.py` & `zenaura-0.9.87/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/tests/test_zenaura_dom.py` & `zenaura-0.9.87/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/algorithm/operations.py` & `zenaura-0.9.87/zenaura/client/algorithm/operations.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/algorithm/searcher.py` & `zenaura-0.9.87/zenaura/client/algorithm/searcher.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/algorithm/updater.py` & `zenaura-0.9.87/zenaura/client/algorithm/updater.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/app.py` & `zenaura-0.9.87/zenaura/client/app.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+import asyncio
 from dataclasses import dataclass
 from typing import List
 from zenaura.client.dom import zenaura_dom
 from zenaura.client.tags import Node
 from zenaura.client.component import Component, Reuseable
 from zenaura.client.page import Page
 from zenaura.client.mocks import MockWindow, MockDocument
-import asyncio
+from zenaura.client.hydrator import HydratorRealDomAdapter
+
+rdom_hyd = HydratorRealDomAdapter() 
+
 event_loop = asyncio.get_event_loop()
 
 # this is really nothing just to be able to mock 
 try :
     from pyscript import document, window
 except ImportError:
     document = MockDocument() 
@@ -87,15 +91,14 @@
 
         if not isinstance(page, Page):
             raise TypeError("Only a Page can be mounted on a route")
         self.middleware: Optional[Callable] = middleware  # For optional route-specific logic
 
 
 # router 
-
 class App:
     """
         Represents a router for managing routes and navigation.
 
         Methods
         -------
         __init__()
@@ -148,18 +151,23 @@
         # run middle ware #TODO test
         if callable(middleware):
             await middleware()
         
 
         [page, title, middleware, ssr] = self.routes[path]
         window.history.pushState(path, title, path) # Update browser history
-        if not ssr: # ignore mount step for ssr
-            await zenaura_dom.mount(page)  # Mount the page on root container
+        if not ssr: # ignore mount step for server side rendering pages.
+            rdom_hyd.hyd_rdom_toggle_pages_visibilty(page, self.history.current.page)
+            await zenaura_dom.mount(page)  # trigger attached lifecycle for each component within the page.
+        else: # trigger attached lifecycle method for the component.
+            await zenaura_dom.mount(page)
         self.history.visit(page)
-        document.title = title  # Update the title
+        document.title = title 
+
+
 
     async def handle_location(self) -> None:
         """
         Handles the current location by mounting the associated page and update title of document
         """
         path = window.location.pathname
         matched_route, params = self._match_route(path)
@@ -167,16 +175,20 @@
         if not matched_route:
             await self.not_found()
             return
         [page, title, middleware, ssr] = self.routes[path]
         window.history.pushState(path, title, path) # Update browser history
         if callable(middleware):
             await middleware()
-        if not ssr: # ignore mount for ssr 
+        if not ssr: # ignore mount step for server side rendering pages.
+            rdom_hyd.hyd_rdom_toggle_pages_visibilty(page, self.history.current.page)
+            await zenaura_dom.mount(page)  # trigger attached lifecycle for each component within the page.
+        else: # trigger attached lifecycle method for the component.
             await zenaura_dom.mount(page)
+        # TODO handle ssr in mount. 
         self.history.visit(page)
         document.title = title
 
 
 
 
     def add_route(self, route : Route) -> None:
@@ -188,24 +200,30 @@
         route : Route
             The route to be added to the router's configuration.
         """
         self.routes[route.path] = [route.page, route.title, route.middleware, route.ssr]
         self.paths.append(route.path)
     
     async def back(self) -> None:
-        page = self.history.back()
-        if self.history.current.page == page:
-            return # do not mount new page
-        await zenaura_dom.mount(page) # else mount new page
+        previous_page = self.history.current.page
+        curr_page = self.history.back()
+        if not curr_page.ssr: # ignore mount step for server side rendering pages.
+            rdom_hyd.hyd_rdom_toggle_pages_visibilty(previous_page, curr_page)
+            await zenaura_dom.mount(curr_page)  # trigger attached lifecycle for each component within the page.
+        else: # trigger attached lifecycle method for the component.
+            await zenaura_dom.mount(curr_page)
     
     async def forward(self) -> None:
-        page = self.history.forward()
-        if self.history.current.page == page:
-            return # do not mount new page
-        await zenaura_dom.mount(page) # else mount new page
+        previous_page = self.history.current.page
+        curr_page = self.history.forward()
+        if not curr_page.ssr: # ignore mount step for server side rendering pages.
+            rdom_hyd.hyd_rdom_toggle_pages_visibilty(previous_page, curr_page)
+            await zenaura_dom.mount(curr_page)  # trigger attached lifecycle for each component within the page.
+        else: # trigger attached lifecycle method for the component.
+            await zenaura_dom.mount(curr_page)
 
     def get_current_route(self) -> Optional[Tuple[Page, str]]:
             """Get the page and title of the current route, or None if not found."""
             path = window.location.pathname
             matched_route, info = self._match_route(path)
             return matched_route, info
```

### Comparing `zenaura-0.9.86/zenaura/client/compiler/attribute.py` & `zenaura-0.9.87/zenaura/client/compiler/attribute.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/compiler/compiler.py` & `zenaura-0.9.87/zenaura/client/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/compiler/sanitize.py` & `zenaura-0.9.87/zenaura/client/compiler/sanitize.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/component.py` & `zenaura-0.9.87/zenaura/client/component.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/config.py` & `zenaura-0.9.87/zenaura/client/config.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/dom/error.py` & `zenaura-0.9.87/zenaura/client/dom/error.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/dom/lifecycles/render.py` & `zenaura-0.9.87/zenaura/client/dom/lifecycles/render.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 class RenderLifeCycle:
-    def on_mutation(self, comp) -> None:
+    async def on_mutation(self, comp) -> None:
         """
         Method called after the component is updated in the DOM and re-rendered.
 
         Parameters:
         - comp: An instance of the Component class.
 
         Returns:
         None
         """
         # Perform operations before updating
         if hasattr(comp, 'on_mutation'):
-            comp.on_mutation()
+            await comp.on_mutation()
 
-    def on_settled(self, comp) -> None:
+    async def on_settled(self, comp) -> None:
         """
         Method called after the component is updated in the DOM and re-rendered.
 
         Parameters:
         - comp: An instance of the Component class.
 
         Returns:
         None
         """
         # Perform operations after updating
         if hasattr(comp, 'on_settled'):
-            comp.on_settled()
+            await comp.on_settled()
```

### Comparing `zenaura-0.9.86/zenaura/client/dom/mount.py` & `zenaura-0.9.87/zenaura/client/hydrator/lookup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,35 @@
+from collections import defaultdict
 
-from .lifecycles.mount import MountLifeCycles
-from .error import GracefulDegenerationLifeCycleWrapper
-from zenaura.client.page import Page
-from zenaura.client.hydrator import HydratorRealDomAdapter
-import traceback
-
-rdom_hyd = HydratorRealDomAdapter()
-
-class Mount(
-    GracefulDegenerationLifeCycleWrapper,
-    MountLifeCycles,
-    ):
-    async def mount(self, page: Page  ) -> None:
-        """
-            Mount only Page instance to the DOM.
-            Only one page instance can be mounted at a time.
-            Lifecycle:
-            2. in-time compile html for the page components.
-            3. attach compiled html to the DOM.
-            4. trigger attached for page components.
-            5. update state in vdom for each component.
-            6. cleanup vdom from unmounted components.
-            try : 
-                - mount the component.
-            except:
-                - call componentDidCatchError method.
-            Parameters:
-            - comp: An instance of the Component class.
-
-            Returns:
-            None
-        """
-
-        try :
-            # wait for DOMContent to be loaded 
-            await rdom_hyd.hyd_rdom_wait_for_dom_content_loaded()
-
-            compiled_html = self.hyd_comp_compile_page(page)
-
-            self.hyd_rdom_attach_to_root(compiled_html)
-            # trigger attached for page components
-            
-            # clean up perviously mounted components :
-            self.zen_dom_table.clear()
-
-            for comp in page.children:
-                # trigger attached for page components
-                self.attached(comp)
-                # update state in vdom
-                self.hyd_vdom_update(comp)
-
-        except Exception as e:
-            self.componentDidCatchError(page.children[0], traceback.format_exc())
+class VDomLookupTable:
+    """
+        1. zen_dom_table :
+        - Optimizing general tree structure
+        - each component unique id
+        - each child of the component has ZENAURA_DOM_ATTRIBUTE
+        this allows for:
+        - searching for mounted component prev state : O(1)
+        - deleting unmounted components : O(1)
+        - inserting mounted components : O(1)
+        now same time complexity applies on tree structure:
+        - search O(n)
+        - insert O(n)
+        - delete O(n)
+        - update O(n)
+        aslo allows for effecient management of memory
+        since in zenaura one page and each page is a dummy node
+        of children components
+        then once the page unmounted all the components are deleted
+
+        2. zenaura prev_page_instance:
+        - once page is mounted we store the prev_page_instance
+        - zenaura mount single page at a time or " route path "
+        - this allow for effecient memory management
+        - once new page is mounted:
+            - get the prev page instance
+            - iterage over the prev page components
+            - delete the prev page component from zen_dom_table
+
+    """
+    zen_dom_table = defaultdict(str)
+    prev_page_instance = None
+    zen_pre_compiled = defaultdict(str)
```

### Comparing `zenaura-0.9.86/zenaura/client/dom/render.py` & `zenaura-0.9.87/zenaura/client/dom/render.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/hydrator/compiler_adapter.py` & `zenaura-0.9.87/zenaura/client/hydrator/compiler_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/hydrator/hydrator.py` & `zenaura-0.9.87/zenaura/client/hydrator/hydrator.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/hydrator/real_dom_adapter.py` & `zenaura-0.9.87/zenaura/client/hydrator/real_dom_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio 
 from zenaura.client.tags import Node, HTMLElement, Attribute
+from zenaura.client.page import Page 
 from zenaura.client.component import Component
 from zenaura.client.config import ZENAURA_DOM_ATTRIBUTE
 from zenaura.client.mocks import MockDocument, MockWindow
 try :
     from pyscript import document, window
     from pyodide.ffi import create_proxy
     in_browser = True
@@ -171,8 +172,16 @@
     async def hyd_rdom_wait_for_dom_content_loaded(self):
         if not in_browser:
             return 
         while True:
             await asyncio.sleep(0.001)
             if document.readyState=="complete":
                 break
-        
+        
+
+    def hyd_rdom_toggle_pages_visibilty(self, current_page : Page , previous_page : Page):
+        p_page = document.querySelector(f'[{ZENAURA_DOM_ATTRIBUTE}="{previous_page.id}"]')
+        if p_page:
+            p_page.setAttribute("hidden", "true")
+        curr_page = document.querySelector(f'[{ZENAURA_DOM_ATTRIBUTE}="{current_page.id}"]')
+        if curr_page:
+            curr_page.setAttribute("hidden", "false") # Update the title
```

### Comparing `zenaura-0.9.86/zenaura/client/hydrator/tasker.py` & `zenaura-0.9.87/zenaura/client/hydrator/tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/hydrator/virtual_dom_adapter.py` & `zenaura-0.9.87/zenaura/client/hydrator/virtual_dom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/mocks.py` & `zenaura-0.9.87/zenaura/client/mocks.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/mutator.py` & `zenaura-0.9.87/zenaura/client/mutator.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/observer/subject.py` & `zenaura-0.9.87/zenaura/client/observer/subject.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/observer.py` & `zenaura-0.9.87/zenaura/client/observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/page.py` & `zenaura-0.9.87/zenaura/client/page.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,22 @@
+import uuid 
+import itertools
 from .component import Component, UUIDManager
 from typing import List
-import uuid 
+
 
 class Page:
     """
         a class representing a page in zenaura application
     """
-    def __init_subclass__(cls):
-        """
-        Initialize a new subclass of Page.
-
-        This method generates a unique id for each subclass using uuid.
-
-        Args:
-        cls: The subclass being initialized.
-
-        Returns:
-        None
-        """
+    _page_count = itertools.count(0)
 
-        super().__init_subclass__()
-        UUIDManager.persist_uuid(cls)
+    def __init_subclass__(cls, **kwargs):
+        cls.count = next(cls._component_count)
+        cls.id = UUIDManager.generate_uuid(cls.__name__, cls.count)
 
     def __init__(self, children : List[Component]):
         self.children = children
         self.pageId = uuid.uuid4().hex
         if not isinstance(self.children, list):
             raise TypeError("children must be a list")
```

### Comparing `zenaura-0.9.86/zenaura/client/persistance.py` & `zenaura-0.9.87/zenaura/client/persistance.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/tags/builder.py` & `zenaura-0.9.87/zenaura/client/tags/builder.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura/client/tags/node.py` & `zenaura-0.9.87/zenaura/client/tags/node.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.86/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.87/zenaura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.86
+Version: 0.9.87
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.86/zenaura.egg-info/SOURCES.txt` & `zenaura-0.9.87/zenaura.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 tests/test_app.py
 tests/test_compiler.py
 tests/test_component_e2e.py
 tests/test_component_unit.py
 tests/test_node_properties.py
 tests/test_observer.py
 tests/test_rdom_adapter.py
+tests/test_server.py
 tests/test_tags.py
 tests/test_tasker.py
 tests/test_zenaura_dom.py
 zenaura/__init__.py
 zenaura.egg-info/PKG-INFO
 zenaura.egg-info/SOURCES.txt
 zenaura.egg-info/dependency_links.txt
```

