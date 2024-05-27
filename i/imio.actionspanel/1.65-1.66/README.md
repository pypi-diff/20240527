# Comparing `tmp/imio.actionspanel-1.65.tar.gz` & `tmp/imio.actionspanel-1.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.actionspanel-1.65.tar", last modified: Thu Feb  8 14:34:57 2024, max compression
+gzip compressed data, was "dist/imio.actionspanel-1.66.tar", last modified: Mon May 27 10:20:57 2024, max compression
```

## Comparing `imio.actionspanel-1.65.tar` & `imio.actionspanel-1.66.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio.actionspanel.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio.actionspanel.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio.actionspanel.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio.actionspanel.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio.actionspanel.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    30498 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio.actionspanel.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3560 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio.actionspanel.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio.actionspanel.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      122 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio.actionspanel.egg-info/requires.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/skins/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/skins/actionspanel_plone/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      144 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/skins/actionspanel_plone/rename_icon.gif
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1598 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/skins/actionspanel_plone/folder_position_typeaware.cpy
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      221 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/skins/actionspanel_plone/folder_position_typeaware.cpy.metadata
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      285 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/skins/actionspanel_plone/extedit_icon.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1529 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      813 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/adapters.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      734 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/locales/manual.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/locales/es/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/locales/es/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      665 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/locales/es/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4870 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/locales/es/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      628 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/locales/plone.pot
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3329 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/locales/imio.actionspanel.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      578 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4123 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/locales/fr/LC_MESSAGES/imio.actionspanel.po
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      271 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/profiles/default/browserlayer.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      234 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      125 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/profiles/default/registry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      453 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/profiles/default/skins.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      468 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/profiles/default/cssregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1020 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/profiles/default/actions.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      398 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/profiles/default/jsregistry.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      891 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/testing.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      781 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/interfaces.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3109 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/mk_sync_locales.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2254 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       24 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      171 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/testing.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/tests/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      311 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/static/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5846 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/static/actionspanel.js
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      684 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/static/arrowDown.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1007 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/static/actionspanel.css
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       63 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/static/notTriggerableTransition.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      621 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/static/history_last_event_has_comment.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      766 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/static/arrowBottom.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      674 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/static/arrowUp.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      707 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/static/arrowTop.png
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1003 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/static/history.gif
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2458 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_transitions.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1375 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_actions.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    33690 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/views.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4480 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/comments.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1989 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1933 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/comment_delete.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1055 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_folder_contents.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      367 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_viewlet.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2395 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_arrows.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      925 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_edit.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      877 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/viewlets.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3202 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/registry.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      662 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/jsvariables.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      997 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_own_delete_with_comments.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      624 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_add_content.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      634 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_history.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1259 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_own_delete.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      487 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       24 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      415 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_ext_edit.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1714 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/browser/comment_transition.pt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1147 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/actionspanel/upgrades.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/src/imio/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      516 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/dev.cfg
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/docs/LICENSE.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1662 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    30498 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      219 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    20679 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       46 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/CONTRIBUTORS.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      322 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/versions.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/base.cfg
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/.tx/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      274 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/.tx/config
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      171 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/sources.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3254 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      370 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/Makefile
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       47 2024-02-08 14:34:57.000000 imio.actionspanel-1.65/buildout.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio.actionspanel.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio.actionspanel.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio.actionspanel.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio.actionspanel.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        5 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio.actionspanel.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    30810 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio.actionspanel.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3592 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio.actionspanel.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio.actionspanel.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      122 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio.actionspanel.egg-info/requires.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/skins/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/skins/actionspanel_plone/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      144 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/skins/actionspanel_plone/rename_icon.gif
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1598 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/skins/actionspanel_plone/folder_position_typeaware.cpy
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      221 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/skins/actionspanel_plone/folder_position_typeaware.cpy.metadata
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      285 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/skins/actionspanel_plone/extedit_icon.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1848 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      736 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/adapters.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      734 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/locales/manual.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/locales/es/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/locales/es/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      665 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/locales/es/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4870 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/locales/es/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      628 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/locales/plone.pot
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3329 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/locales/imio.actionspanel.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      578 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4123 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/locales/fr/LC_MESSAGES/imio.actionspanel.po
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      271 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      234 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      125 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/profiles/default/registry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      453 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/profiles/default/skins.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      468 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/profiles/default/cssregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1020 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/profiles/default/actions.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      398 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/profiles/default/jsregistry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      891 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      901 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/interfaces.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3109 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/mk_sync_locales.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2254 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       24 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      704 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/events.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      171 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/testing.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      311 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/static/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5846 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/static/actionspanel.js
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      684 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/static/arrowDown.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1007 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/static/actionspanel.css
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       63 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/static/notTriggerableTransition.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      621 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/static/history_last_event_has_comment.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      766 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/static/arrowBottom.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      674 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/static/arrowUp.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      707 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/static/arrowTop.png
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1003 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/static/history.gif
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2458 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_transitions.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1375 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_actions.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    33690 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/views.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     4480 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/comments.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1989 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1933 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/comment_delete.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1055 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_folder_contents.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      367 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_viewlet.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2395 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_arrows.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      925 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_edit.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      877 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/viewlets.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3202 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/registry.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      662 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/jsvariables.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      997 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_own_delete_with_comments.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      624 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_add_content.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      634 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_history.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1259 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_own_delete.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      487 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       24 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      415 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_ext_edit.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1714 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/browser/comment_transition.pt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1147 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/actionspanel/upgrades.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/src/imio/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      516 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/dev.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/docs/LICENSE.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1662 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    30810 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      219 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    20927 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       46 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/CONTRIBUTORS.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      322 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/versions.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      750 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/base.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/.tx/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      274 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/.tx/config
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      171 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/sources.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3254 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      370 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/Makefile
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       47 2024-05-27 10:20:57.000000 imio.actionspanel-1.66/buildout.cfg
```

### Comparing `imio.actionspanel-1.65/src/imio.actionspanel.egg-info/PKG-INFO` & `imio.actionspanel-1.66/src/imio.actionspanel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.actionspanel
-Version: 1.65
+Version: 1.66
 Summary: Actions panel
 Home-page: https://github.com/imio/imio.actionspanel
 Author: IMIO
 Author-email: dev@imio.be
 License: GPL
 Download-URL: https://pypi.org/project/imio.actionspanel
 Description: imio.actionspanel
@@ -77,14 +77,22 @@
         
         You can contribute for any message missing or other new languages, join us at `PloneGov iMiO Team <https://www.transifex.com/plone/plonegov-imio/>`_ into *Transifex.net* service with all world Plone translators community.
         
         
         Changelog
         =========
         
+        1.66 (2024-05-27)
+        -----------------
+        
+        - Added `onObjWillBeRemoved` event handler (ZCML disabled by default)
+          that will check for an `IContentDeletable.mayDelete` adapter upon
+          any deletion.  Enable it when using `IContentDeletable`.
+          [gbastien]
+        
         1.65 (2024-02-08)
         -----------------
         
         - Use `typeInfo.Title()` to get portal_type's title instead
           translating the `typeInfo.title`.
           [gbastien]
```

### Comparing `imio.actionspanel-1.65/src/imio.actionspanel.egg-info/SOURCES.txt` & `imio.actionspanel-1.66/src/imio.actionspanel.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 src/imio.actionspanel.egg-info/not-zip-safe
 src/imio.actionspanel.egg-info/requires.txt
 src/imio.actionspanel.egg-info/top_level.txt
 src/imio/actionspanel/__init__.py
 src/imio/actionspanel/adapters.py
 src/imio/actionspanel/config.py
 src/imio/actionspanel/configure.zcml
+src/imio/actionspanel/events.py
 src/imio/actionspanel/interfaces.py
 src/imio/actionspanel/mk_sync_locales.sh
 src/imio/actionspanel/testing.py
 src/imio/actionspanel/testing.zcml
 src/imio/actionspanel/upgrades.zcml
 src/imio/actionspanel/utils.py
 src/imio/actionspanel/browser/__init__.py
```

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/skins/actionspanel_plone/folder_position_typeaware.cpy` & `imio.actionspanel-1.66/src/imio/actionspanel/skins/actionspanel_plone/folder_position_typeaware.cpy`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/configure.zcml` & `imio.actionspanel-1.66/src/imio/actionspanel/configure.zcml`

 * *Files 15% similar despite different names*

```diff
@@ -32,11 +32,15 @@
   <cmf:registerDirectory name="actionspanel_plone"/>
 
   <genericsetup:registerProfile
       name="default"
       title="imio.actionspanel"
       directory="profiles/default"
       description="Extension profile for imio.actionspanel."
-      provides="Products.GenericSetup.interfaces.EXTENSION"
-      />
+      provides="Products.GenericSetup.interfaces.EXTENSION" />
 
+  <!-- Enable this if using IContentDeletable adapters or this will
+       not be checked by Plone upon default deletion (manage_deleteObjects) -->
+  <!--subscriber for="OFS.interfaces.IItem
+                   OFS.interfaces.IObjectWillBeRemovedEvent"
+              handler="imio.actionspanel.events.onObjWillBeRemoved" /-->
 </configure>
```

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/adapters.py` & `imio.actionspanel-1.66/src/imio/actionspanel/adapters.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 # -*- coding: utf-8 -*-
 #
-# File: adapters.py
-#
-# Copyright (c) 2014 by Imio.be
-#
 # GNU General Public License (GPL)
 #
 
 from imio.history.adapters import BaseImioHistoryAdapter
-from plone import api
 from Products.CMFCore.permissions import DeleteObjects
+from Products.CMFCore.utils import _checkPermission
 
 
 class ContentDeletableAdapter(object):
     """
       Manage the mayDelete on every objects.
     """
 
     def __init__(self, context):
         self.context = context
 
     def mayDelete(self, **kwargs):
         '''See docstring in interfaces.py'''
-        member = api.user.get_current()
-        return bool(member.has_permission(DeleteObjects, self.context))
+        return _checkPermission(DeleteObjects, self.context)
 
 
 class DeletedChildrenHistoryAdapter(BaseImioHistoryAdapter):
     """ """
 
     history_type = 'deleted_children'
     history_attr_name = 'deleted_children_history'
```

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/locales/manual.pot` & `imio.actionspanel-1.66/src/imio/actionspanel/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/locales/es/LC_MESSAGES/plone.po` & `imio.actionspanel-1.66/src/imio/actionspanel/locales/es/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/locales/es/LC_MESSAGES/imio.actionspanel.po` & `imio.actionspanel-1.66/src/imio/actionspanel/locales/es/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/locales/plone.pot` & `imio.actionspanel-1.66/src/imio/actionspanel/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/locales/imio.actionspanel.pot` & `imio.actionspanel-1.66/src/imio/actionspanel/locales/imio.actionspanel.pot`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/locales/fr/LC_MESSAGES/plone.po` & `imio.actionspanel-1.66/src/imio/actionspanel/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/locales/fr/LC_MESSAGES/imio.actionspanel.po` & `imio.actionspanel-1.66/src/imio/actionspanel/locales/fr/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/profiles/default/actions.xml` & `imio.actionspanel-1.66/src/imio/actionspanel/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/testing.py` & `imio.actionspanel-1.66/src/imio/actionspanel/testing.py`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/interfaces.py` & `imio.actionspanel-1.66/src/imio/actionspanel/interfaces.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     """
 
     def mayDelete(context):
         """
           This method returns True if current context is deletable.
           The default implementation does the work for checking 'Delete objects' on the
           object we want to delete, not that permission on the parent.
+          You can return a appy.gen.No instance to be able to display a message
+          why element is not deletable.
         """
 
 
 class IFolderContentsShowableMarker(Interface):
     """
         Marker that can be used to show folder_contents action
     """
```

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/mk_sync_locales.sh` & `imio.actionspanel-1.66/src/imio/actionspanel/mk_sync_locales.sh`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/utils.py` & `imio.actionspanel-1.66/src/imio/actionspanel/utils.py`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/static/actionspanel.js` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/static/actionspanel.js`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/static/arrowDown.png` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/static/arrowDown.png`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/static/actionspanel.css` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/static/actionspanel.css`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/static/history_last_event_has_comment.gif` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/static/history_last_event_has_comment.gif`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/static/arrowBottom.png` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/static/arrowBottom.png`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/static/arrowUp.png` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/static/arrowUp.png`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/static/arrowTop.png` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/static/arrowTop.png`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/static/history.gif` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/static/history.gif`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_transitions.pt` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_transitions.pt`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_actions.pt` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_actions.pt`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/views.py` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/views.py`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/comments.py` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/comments.py`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/configure.zcml` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/comment_delete.pt` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/comment_delete.pt`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_folder_contents.pt` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_folder_contents.pt`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_arrows.pt` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_arrows.pt`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_edit.pt` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_edit.pt`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/viewlets.py` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/registry.py` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/registry.py`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/jsvariables.py` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/jsvariables.py`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_own_delete_with_comments.pt` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_own_delete_with_comments.pt`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_add_content.pt` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_add_content.pt`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_history.pt` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_history.pt`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/actions_panel_own_delete.pt` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/actions_panel_own_delete.pt`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/browser/comment_transition.pt` & `imio.actionspanel-1.66/src/imio/actionspanel/browser/comment_transition.pt`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/src/imio/actionspanel/upgrades.zcml` & `imio.actionspanel-1.66/src/imio/actionspanel/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/dev.cfg` & `imio.actionspanel-1.66/dev.cfg`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/docs/LICENSE.rst` & `imio.actionspanel-1.66/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/docs/LICENSE.GPL` & `imio.actionspanel-1.66/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/setup.py` & `imio.actionspanel-1.66/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 long_description = (
     open('README.rst').read() + '\n' + open('CHANGES.rst').read() + '\n')
 
 setup(
     name='imio.actionspanel',
-    version='1.65',
+    version='1.66',
     description="Actions panel",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `imio.actionspanel-1.65/PKG-INFO` & `imio.actionspanel-1.66/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.actionspanel
-Version: 1.65
+Version: 1.66
 Summary: Actions panel
 Home-page: https://github.com/imio/imio.actionspanel
 Author: IMIO
 Author-email: dev@imio.be
 License: GPL
 Download-URL: https://pypi.org/project/imio.actionspanel
 Description: imio.actionspanel
@@ -77,14 +77,22 @@
         
         You can contribute for any message missing or other new languages, join us at `PloneGov iMiO Team <https://www.transifex.com/plone/plonegov-imio/>`_ into *Transifex.net* service with all world Plone translators community.
         
         
         Changelog
         =========
         
+        1.66 (2024-05-27)
+        -----------------
+        
+        - Added `onObjWillBeRemoved` event handler (ZCML disabled by default)
+          that will check for an `IContentDeletable.mayDelete` adapter upon
+          any deletion.  Enable it when using `IContentDeletable`.
+          [gbastien]
+        
         1.65 (2024-02-08)
         -----------------
         
         - Use `typeInfo.Title()` to get portal_type's title instead
           translating the `typeInfo.title`.
           [gbastien]
```

### Comparing `imio.actionspanel-1.65/CHANGES.rst` & `imio.actionspanel-1.66/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+1.66 (2024-05-27)
+-----------------
+
+- Added `onObjWillBeRemoved` event handler (ZCML disabled by default)
+  that will check for an `IContentDeletable.mayDelete` adapter upon
+  any deletion.  Enable it when using `IContentDeletable`.
+  [gbastien]
+
 1.65 (2024-02-08)
 -----------------
 
 - Use `typeInfo.Title()` to get portal_type's title instead
   translating the `typeInfo.title`.
   [gbastien]
```

### Comparing `imio.actionspanel-1.65/base.cfg` & `imio.actionspanel-1.66/base.cfg`

 * *Files identical despite different names*

### Comparing `imio.actionspanel-1.65/README.rst` & `imio.actionspanel-1.66/README.rst`

 * *Files identical despite different names*

