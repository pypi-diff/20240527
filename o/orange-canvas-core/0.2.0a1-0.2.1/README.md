# Comparing `tmp/orange-canvas-core-0.2.0a1.tar.gz` & `tmp/orange-canvas-core-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orange-canvas-core-0.2.0a1.tar", last modified: Mon Nov 27 12:50:41 2023, max compression
+gzip compressed data, was "orange-canvas-core-0.2.1.tar", last modified: Mon May 27 11:53:49 2024, max compression
```

## Comparing `orange-canvas-core-0.2.0a1.tar` & `orange-canvas-core-0.2.1.tar`

### file list

```diff
@@ -1,295 +1,295 @@
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.531905 orange-canvas-core-0.2.0a1/
--rw-r--r--   0 ales      (1000) ales      (1000)    35147 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/LICENSE.txt
--rw-r--r--   0 ales      (1000) ales      (1000)       57 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/MANIFEST.in
--rw-r--r--   0 ales      (1000) ales      (1000)     1602 2023-11-27 12:50:41.531905 orange-canvas-core-0.2.0a1/PKG-INFO
--rw-r--r--   0 ales      (1000) ales      (1000)     1027 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/README.rst
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.508572 orange-canvas-core-0.2.0a1/docs/
--rw-r--r--   0 ales      (1000) ales      (1000)     7273 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/make.bat
--rw-r--r--   0 ales      (1000) ales      (1000)      347 2023-10-30 14:24:58.000000 orange-canvas-core-0.2.0a1/docs/requirements-rtd.txt
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.511905 orange-canvas-core-0.2.0a1/docs/source/
--rw-r--r--   0 ales      (1000) ales      (1000)     9735 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/docs/source/conf.py
--rw-r--r--   0 ales      (1000) ales      (1000)      506 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/index.rst
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.511905 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/
--rw-r--r--   0 ales      (1000) ales      (1000)      603 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/application.canvasmain.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      235 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/application.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      632 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/application.welcomedialog.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      478 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/canvas.items.annotationitem.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      237 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/canvas.items.linkitem.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      827 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/canvas.items.nodeitem.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      211 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/canvas.rst
--rw-r--r--   0 ales      (1000) ales      (1000)     1153 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/canvas.scene.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      932 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/document.interactions.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      491 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/document.quickmenu.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      197 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/document.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      735 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/document.schemeedit.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      343 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/gui.dock.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      272 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/gui.dropshadow.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      315 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/gui.framelesswindow.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      480 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/gui.lineedit.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      240 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/gui.quickhelp.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      311 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/gui.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      267 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/gui.splashscreen.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      662 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/gui.stackedwidget.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      235 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/gui.toolbar.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      358 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/gui.toolbox.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      510 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/gui.toolgrid.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      462 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/gui.tooltree.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      186 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/index.rst
--rw-r--r--   0 ales      (1000) ales      (1000)     2094 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/overview.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      763 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/registry.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      688 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.annotation.rst
--rw-r--r--   0 ales      (1000) ales      (1000)     2285 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.events.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      395 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.link.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      536 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.node.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      193 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.readwrite.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      279 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.rst
--rw-r--r--   0 ales      (1000) ales      (1000)     1456 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.scheme.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      584 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.signalmanager.rst
--rw-r--r--   0 ales      (1000) ales      (1000)      618 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.widgetmanager.rst
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.515238 orange-canvas-core-0.2.0a1/orange_canvas_core.egg-info/
--rw-r--r--   0 ales      (1000) ales      (1000)     1602 2023-11-27 12:50:41.000000 orange-canvas-core-0.2.0a1/orange_canvas_core.egg-info/PKG-INFO
--rw-r--r--   0 ales      (1000) ales      (1000)     9906 2023-11-27 12:50:41.000000 orange-canvas-core-0.2.0a1/orange_canvas_core.egg-info/SOURCES.txt
--rw-r--r--   0 ales      (1000) ales      (1000)        1 2023-11-27 12:50:41.000000 orange-canvas-core-0.2.0a1/orange_canvas_core.egg-info/dependency_links.txt
--rw-r--r--   0 ales      (1000) ales      (1000)      246 2023-11-27 12:50:41.000000 orange-canvas-core-0.2.0a1/orange_canvas_core.egg-info/requires.txt
--rw-r--r--   0 ales      (1000) ales      (1000)       13 2023-11-27 12:50:41.000000 orange-canvas-core-0.2.0a1/orange_canvas_core.egg-info/top_level.txt
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.515238 orange-canvas-core-0.2.0a1/orangecanvas/
--rw-r--r--   0 ales      (1000) ales      (1000)        0 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)      104 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/__main__.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.515238 orange-canvas-core-0.2.0a1/orangecanvas/application/
--rw-r--r--   0 ales      (1000) ales      (1000)       64 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1420 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/aboutdialog.py
--rw-r--r--   0 ales      (1000) ales      (1000)    35535 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/addons.py
--rw-r--r--   0 ales      (1000) ales      (1000)     9537 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/application.py
--rw-r--r--   0 ales      (1000) ales      (1000)    97137 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/canvasmain.py
--rw-r--r--   0 ales      (1000) ales      (1000)    23902 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/canvastooldock.py
--rw-r--r--   0 ales      (1000) ales      (1000)     3493 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/examples.py
--rw-r--r--   0 ales      (1000) ales      (1000)    14596 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/outputview.py
--rw-r--r--   0 ales      (1000) ales      (1000)     5951 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/schemeinfo.py
--rw-r--r--   0 ales      (1000) ales      (1000)    24523 2023-06-05 09:22:03.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/settings.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.515238 orange-canvas-core-0.2.0a1/orangecanvas/application/tests/
--rw-r--r--   0 ales      (1000) ales      (1000)        0 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/tests/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     7022 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_addons.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4178 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_addons_utils.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1798 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_application.py
--rw-r--r--   0 ales      (1000) ales      (1000)     3386 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_canvastooldock.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4586 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_main.py
--rw-r--r--   0 ales      (1000) ales      (1000)    12606 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_mainwindow.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4829 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_outputview.py
--rw-r--r--   0 ales      (1000) ales      (1000)      639 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_schemeinfo.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1821 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_settings.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1137 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_welcomedialog.py
--rw-r--r--   0 ales      (1000) ales      (1000)     3094 2023-10-18 10:31:35.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_widgettoolbox.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.515238 orange-canvas-core-0.2.0a1/orangecanvas/application/utils/
--rw-r--r--   0 ales      (1000) ales      (1000)        0 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/utils/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)    20539 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/utils/addons.py
--rw-r--r--   0 ales      (1000) ales      (1000)     9599 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/welcomedialog.py
--rw-r--r--   0 ales      (1000) ales      (1000)    19895 2023-10-18 10:31:35.000000 orange-canvas-core-0.2.0a1/orangecanvas/application/widgettoolbox.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.515238 orange-canvas-core-0.2.0a1/orangecanvas/canvas/
--rw-r--r--   0 ales      (1000) ales      (1000)      313 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/__init__.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.518572 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/
--rw-r--r--   0 ales      (1000) ales      (1000)      288 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)    26237 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/annotationitem.py
--rw-r--r--   0 ales      (1000) ales      (1000)    16390 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/controlpoints.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4065 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/graphicspathobject.py
--rw-r--r--   0 ales      (1000) ales      (1000)    19389 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/graphicstextitem.py
--rw-r--r--   0 ales      (1000) ales      (1000)    27045 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/linkitem.py
--rw-r--r--   0 ales      (1000) ales      (1000)    61492 2023-10-12 12:27:47.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/nodeitem.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.518572 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/
--rw-r--r--   0 ales      (1000) ales      (1000)      738 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2077 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/test_annotationitem.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1843 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/test_controlpoints.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2029 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/test_graphicspathobject.py
--rw-r--r--   0 ales      (1000) ales      (1000)     3214 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/test_graphicstextitem.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4033 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/test_linkitem.py
--rw-r--r--   0 ales      (1000) ales      (1000)     7044 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/test_nodeitem.py
--rw-r--r--   0 ales      (1000) ales      (1000)     3800 2023-05-23 09:45:47.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/test_utils.py
--rw-r--r--   0 ales      (1000) ales      (1000)    10662 2023-05-23 09:45:47.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/utils.py
--rw-r--r--   0 ales      (1000) ales      (1000)     5792 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/layout.py
--rw-r--r--   0 ales      (1000) ales      (1000)    33048 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/scene.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.518572 orange-canvas-core-0.2.0a1/orangecanvas/canvas/tests/
--rw-r--r--   0 ales      (1000) ales      (1000)        0 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/tests/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2653 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/tests/test_layout.py
--rw-r--r--   0 ales      (1000) ales      (1000)     9026 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/tests/test_scene.py
--rw-r--r--   0 ales      (1000) ales      (1000)      871 2023-10-26 11:00:28.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/tests/test_view.py
--rw-r--r--   0 ales      (1000) ales      (1000)    10270 2023-10-26 11:00:28.000000 orange-canvas-core-0.2.0a1/orangecanvas/canvas/view.py
--rw-r--r--   0 ales      (1000) ales      (1000)    16942 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/config.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.518572 orange-canvas-core-0.2.0a1/orangecanvas/document/
--rw-r--r--   0 ales      (1000) ales      (1000)      400 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/document/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)    12087 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/document/commands.py
--rw-r--r--   0 ales      (1000) ales      (1000)    33848 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/document/editlinksdialog.py
--rw-r--r--   0 ales      (1000) ales      (1000)    77825 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/document/interactions.py
--rw-r--r--   0 ales      (1000) ales      (1000)    62110 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/document/quickmenu.py
--rw-r--r--   0 ales      (1000) ales      (1000)    93560 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/document/schemeedit.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4195 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/document/suggestions.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.518572 orange-canvas-core-0.2.0a1/orangecanvas/document/tests/
--rw-r--r--   0 ales      (1000) ales      (1000)        0 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/document/tests/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     3868 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/document/tests/test_editlinksdialog.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2839 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/document/tests/test_quickmenu.py
--rw-r--r--   0 ales      (1000) ales      (1000)    24293 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/document/tests/test_schemeedit.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1729 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/document/tests/test_usagestatistics.py
--rw-r--r--   0 ales      (1000) ales      (1000)    13623 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/document/usagestatistics.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.521905 orange-canvas-core-0.2.0a1/orangecanvas/gui/
--rw-r--r--   0 ales      (1000) ales      (1000)      163 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     9124 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/dock.py
--rw-r--r--   0 ales      (1000) ales      (1000)    11138 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/dropshadow.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2617 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/framelesswindow.py
--rw-r--r--   0 ales      (1000) ales      (1000)     6002 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/iconengine.py
--rw-r--r--   0 ales      (1000) ales      (1000)     3426 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/iconview.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1574 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/itemmodels.py
--rw-r--r--   0 ales      (1000) ales      (1000)     7557 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/lineedit.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4683 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/quickhelp.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4979 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/splashscreen.py
--rw-r--r--   0 ales      (1000) ales      (1000)    11878 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/stackedwidget.py
--rw-r--r--   0 ales      (1000) ales      (1000)    11038 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/svgiconengine.py
--rw-r--r--   0 ales      (1000) ales      (1000)     5523 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/test.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.521905 orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/
--rw-r--r--   0 ales      (1000) ales      (1000)       31 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1611 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_dock.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2966 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_dropshadow.py
--rw-r--r--   0 ales      (1000) ales      (1000)      500 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_framelesswindow.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1162 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_iconengine.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1470 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_lineedit.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1276 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_splashscreen.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2197 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_stackedwidget.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1186 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_toolbar.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2220 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_toolbox.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2933 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_toolgrid.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2600 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_tooltree.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2972 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/textlabel.py
--rw-r--r--   0 ales      (1000) ales      (1000)     3518 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/toolbar.py
--rw-r--r--   0 ales      (1000) ales      (1000)    22011 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/toolbox.py
--rw-r--r--   0 ales      (1000) ales      (1000)    17493 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/toolgrid.py
--rw-r--r--   0 ales      (1000) ales      (1000)    13310 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/tooltree.py
--rw-r--r--   0 ales      (1000) ales      (1000)    23585 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/utils.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4084 2023-10-26 11:00:28.000000 orange-canvas-core-0.2.0a1/orangecanvas/gui/windowlistmanager.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.521905 orange-canvas-core-0.2.0a1/orangecanvas/help/
--rw-r--r--   0 ales      (1000) ales      (1000)       68 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/help/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2262 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/help/intersphinx.py
--rw-r--r--   0 ales      (1000) ales      (1000)    10508 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/help/manager.py
--rw-r--r--   0 ales      (1000) ales      (1000)    13159 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/help/provider.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.521905 orange-canvas-core-0.2.0a1/orangecanvas/help/tests/
--rw-r--r--   0 ales      (1000) ales      (1000)        0 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/help/tests/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1568 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/help/tests/test_manager.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2920 2023-11-06 10:17:13.000000 orange-canvas-core-0.2.0a1/orangecanvas/help/tests/test_provider.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.525238 orange-canvas-core-0.2.0a1/orangecanvas/icons/
--rw-r--r--   0 ales      (1000) ales      (1000)      777 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Arrow.svg
--rw-r--r--   0 ales      (1000) ales      (1000)      854 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Back.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     1352 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Document Info.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     2081 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Documentation.svg
--rw-r--r--   0 ales      (1000) ales      (1000)      714 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Dropdown.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     3237 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Examples.svg
--rw-r--r--   0 ales      (1000) ales      (1000)    11315 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Get Started.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     1509 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Grid.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     1597 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Info.svg
--rw-r--r--   0 ales      (1000) ales      (1000)      771 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Maximize Toolbar.svg
--rw-r--r--   0 ales      (1000) ales      (1000)      769 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Minimize Toolbar.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     1301 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/New.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     1680 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Open.svg
--rw-r--r--   0 ales      (1000) ales      (1000)      755 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Pause.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     1297 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Recent.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     1791 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Search.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     1044 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Text Size.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     1593 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/Tutorials.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     2081 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/YouTube.svg
--rw-r--r--   0 ales      (1000) ales      (1000)      600 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/arrow-right.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     1010 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/default-category.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     1031 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/default-widget.svg
--rw-r--r--   0 ales      (1000) ales      (1000)      243 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/orange-canvas-core-splash.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     9836 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/orange-canvas.svg
--rw-r--r--   0 ales      (1000) ales      (1000)    35907 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/icons/orange-splash-screen.png
--rw-r--r--   0 ales      (1000) ales      (1000)    17708 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/main.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.525238 orange-canvas-core-0.2.0a1/orangecanvas/preview/
--rw-r--r--   0 ales      (1000) ales      (1000)       92 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/preview/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     9381 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/preview/previewbrowser.py
--rw-r--r--   0 ales      (1000) ales      (1000)     3876 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/preview/previewdialog.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4867 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/preview/previewmodel.py
--rw-r--r--   0 ales      (1000) ales      (1000)     5125 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/preview/scanner.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.525238 orange-canvas-core-0.2.0a1/orangecanvas/preview/tests/
--rw-r--r--   0 ales      (1000) ales      (1000)        0 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/preview/tests/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1052 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/preview/tests/test_previewbrowser.py
--rw-r--r--   0 ales      (1000) ales      (1000)      798 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/preview/tests/test_previewdialog.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1456 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/preview/tests/test_scanner.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.525238 orange-canvas-core-0.2.0a1/orangecanvas/registry/
--rw-r--r--   0 ales      (1000) ales      (1000)     2737 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/registry/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     7065 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/registry/base.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1558 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/registry/cache.py
--rw-r--r--   0 ales      (1000) ales      (1000)    15411 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/registry/description.py
--rw-r--r--   0 ales      (1000) ales      (1000)    17564 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/registry/discovery.py
--rw-r--r--   0 ales      (1000) ales      (1000)    12489 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/registry/qt.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.525238 orange-canvas-core-0.2.0a1/orangecanvas/registry/tests/
--rw-r--r--   0 ales      (1000) ales      (1000)     6301 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/registry/tests/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4573 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/registry/tests/test_base.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2953 2023-11-24 11:08:33.000000 orange-canvas-core-0.2.0a1/orangecanvas/registry/tests/test_discovery.py
--rw-r--r--   0 ales      (1000) ales      (1000)     6071 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/registry/utils.py
--rw-r--r--   0 ales      (1000) ales      (1000)     7051 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/resources.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.528572 orange-canvas-core-0.2.0a1/orangecanvas/scheme/
--rw-r--r--   0 ales      (1000) ales      (1000)     1008 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     7632 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/annotations.py
--rw-r--r--   0 ales      (1000) ales      (1000)      612 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/errors.py
--rw-r--r--   0 ales      (1000) ales      (1000)     8382 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/events.py
--rw-r--r--   0 ales      (1000) ales      (1000)    13665 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/link.py
--rw-r--r--   0 ales      (1000) ales      (1000)    11750 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/node.py
--rw-r--r--   0 ales      (1000) ales      (1000)    28793 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/readwrite.py
--rw-r--r--   0 ales      (1000) ales      (1000)    27759 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/scheme.py
--rw-r--r--   0 ales      (1000) ales      (1000)    46448 2023-10-12 11:54:22.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/signalmanager.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.528572 orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/
--rw-r--r--   0 ales      (1000) ales      (1000)     2699 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1407 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/test_annotations.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2785 2023-04-18 11:24:24.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/test_links.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1754 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/test_nodes.py
--rw-r--r--   0 ales      (1000) ales      (1000)     6967 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/test_readwrite.py
--rw-r--r--   0 ales      (1000) ales      (1000)     5688 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/test_scheme.py
--rw-r--r--   0 ales      (1000) ales      (1000)    14841 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/test_signalmanager.py
--rw-r--r--   0 ales      (1000) ales      (1000)    10788 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/test_widgetmanager.py
--rw-r--r--   0 ales      (1000) ales      (1000)    25408 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/scheme/widgetmanager.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.528572 orange-canvas-core-0.2.0a1/orangecanvas/styles/
--rw-r--r--   0 ales      (1000) ales      (1000)     5773 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/styles/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)      235 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/styles/darkorange.qss
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.528572 orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/
--rw-r--r--   0 ales      (1000) ales      (1000)     1991 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Arrow.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     3321 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Document Info.svg
--rw-r--r--   0 ales      (1000) ales      (1000)      538 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Dropdown.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     2251 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Grid.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     1420 2022-01-13 14:33:46.000000 orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Info.svg
--rw-r--r--   0 ales      (1000) ales      (1000)      573 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Pause.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     4870 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Search.svg
--rw-r--r--   0 ales      (1000) ales      (1000)      862 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Text Size.svg
--rw-r--r--   0 ales      (1000) ales      (1000)     8255 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/styles/orange.qss
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.528572 orange-canvas-core-0.2.0a1/orangecanvas/utils/
--rw-r--r--   0 ales      (1000) ales      (1000)     8778 2023-11-16 11:21:06.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2763 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/after_exit.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1598 2023-10-18 10:31:35.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/asyncutils.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2455 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/graph.py
--rw-r--r--   0 ales      (1000) ales      (1000)     3408 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/image.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.528572 orange-canvas-core-0.2.0a1/orangecanvas/utils/localization/
--rw-r--r--   0 ales      (1000) ales      (1000)     1012 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/localization/__init__.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.528572 orange-canvas-core-0.2.0a1/orangecanvas/utils/localization/tests/
--rw-r--r--   0 ales      (1000) ales      (1000)        0 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/localization/tests/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)      816 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/localization/tests/test_localization.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2296 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/markup.py
--rw-r--r--   0 ales      (1000) ales      (1000)    27821 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/overlay.py
--rw-r--r--   0 ales      (1000) ales      (1000)     2924 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/pickle.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4290 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/pkgmeta.py
--rw-r--r--   0 ales      (1000) ales      (1000)    10082 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/propertybindings.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4870 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/qinvoke.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4767 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/qobjref.py
--rw-r--r--   0 ales      (1000) ales      (1000)      683 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/qtcompat.py
--rw-r--r--   0 ales      (1000) ales      (1000)      193 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/redirect.py
--rw-r--r--   0 ales      (1000) ales      (1000)    12397 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/settings.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4151 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/shtools.py
-drwxr-xr-x   0 ales      (1000) ales      (1000)        0 2023-11-27 12:50:41.531905 orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/
--rw-r--r--   0 ales      (1000) ales      (1000)        0 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/__init__.py
--rw-r--r--   0 ales      (1000) ales      (1000)      838 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_after_exit.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1584 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_graph.py
--rw-r--r--   0 ales      (1000) ales      (1000)      761 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_markup.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4345 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_overlay.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1168 2023-11-24 10:01:39.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_pkgmeta.py
--rw-r--r--   0 ales      (1000) ales      (1000)     6295 2023-03-21 11:42:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_propertybindings.py
--rw-r--r--   0 ales      (1000) ales      (1000)     5947 2023-09-19 10:41:54.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_qinvoke.py
--rw-r--r--   0 ales      (1000) ales      (1000)     1696 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_qobjref.py
--rw-r--r--   0 ales      (1000) ales      (1000)      754 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_resources.py
--rw-r--r--   0 ales      (1000) ales      (1000)     4637 2021-08-20 16:07:42.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_settings.py
--rw-r--r--   0 ales      (1000) ales      (1000)      776 2023-01-10 12:51:36.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_shtools.py
--rw-r--r--   0 ales      (1000) ales      (1000)      523 2023-09-19 11:19:30.000000 orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_utils.py
--rw-r--r--   0 ales      (1000) ales      (1000)      316 2023-11-27 12:50:41.531905 orange-canvas-core-0.2.0a1/setup.cfg
--rwxr-xr-x   0 ales      (1000) ales      (1000)     2246 2023-11-27 12:49:19.000000 orange-canvas-core-0.2.0a1/setup.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.808581 orange-canvas-core-0.2.1/
+-rw-rw-r--   0 marko     (1000) marko     (1000)    35147 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/LICENSE.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)       57 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/MANIFEST.in
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1600 2024-05-27 11:53:49.808581 orange-canvas-core-0.2.1/PKG-INFO
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1027 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/README.rst
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.764581 orange-canvas-core-0.2.1/docs/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7273 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/make.bat
+-rw-rw-r--   0 marko     (1000) marko     (1000)      347 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/requirements-rtd.txt
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.764581 orange-canvas-core-0.2.1/docs/source/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9735 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/conf.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      506 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/index.rst
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.768581 orange-canvas-core-0.2.1/docs/source/orangecanvas/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      603 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/application.canvasmain.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      235 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/application.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      632 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/application.welcomedialog.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      478 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/canvas.items.annotationitem.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      237 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/canvas.items.linkitem.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      827 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/canvas.items.nodeitem.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      211 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/canvas.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1153 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/canvas.scene.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      932 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/document.interactions.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      491 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/document.quickmenu.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      197 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/document.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      735 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/document.schemeedit.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      343 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/gui.dock.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      272 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/gui.dropshadow.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      315 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/gui.framelesswindow.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      480 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/gui.lineedit.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      240 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/gui.quickhelp.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      311 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/gui.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      267 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/gui.splashscreen.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      662 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/gui.stackedwidget.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      235 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/gui.toolbar.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      358 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/gui.toolbox.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      510 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/gui.toolgrid.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      462 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/gui.tooltree.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      186 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/index.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2094 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/overview.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      763 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/registry.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      688 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.annotation.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2285 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.events.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      395 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.link.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      536 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.node.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      193 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.readwrite.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      279 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1456 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.scheme.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      584 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.signalmanager.rst
+-rw-rw-r--   0 marko     (1000) marko     (1000)      618 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.widgetmanager.rst
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.772581 orange-canvas-core-0.2.1/orange_canvas_core.egg-info/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1600 2024-05-27 11:53:49.000000 orange-canvas-core-0.2.1/orange_canvas_core.egg-info/PKG-INFO
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9906 2024-05-27 11:53:49.000000 orange-canvas-core-0.2.1/orange_canvas_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)        1 2024-05-27 11:53:49.000000 orange-canvas-core-0.2.1/orange_canvas_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)      246 2024-05-27 11:53:49.000000 orange-canvas-core-0.2.1/orange_canvas_core.egg-info/requires.txt
+-rw-rw-r--   0 marko     (1000) marko     (1000)       13 2024-05-27 11:53:49.000000 orange-canvas-core-0.2.1/orange_canvas_core.egg-info/top_level.txt
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.772581 orange-canvas-core-0.2.1/orangecanvas/
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      104 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/__main__.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.776581 orange-canvas-core-0.2.1/orangecanvas/application/
+-rw-rw-r--   0 marko     (1000) marko     (1000)       64 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1420 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/aboutdialog.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    35535 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/addons.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9695 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/application.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)   100430 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/canvasmain.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    23902 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/canvastooldock.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3493 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/examples.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    14596 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/outputview.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5951 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/schemeinfo.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    24523 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/settings.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.776581 orange-canvas-core-0.2.1/orangecanvas/application/tests/
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/tests/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7022 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/tests/test_addons.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4178 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/tests/test_addons_utils.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2047 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/tests/test_application.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3386 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/tests/test_canvastooldock.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5178 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/tests/test_main.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    13466 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/tests/test_mainwindow.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4829 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/tests/test_outputview.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      639 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/tests/test_schemeinfo.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1821 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/tests/test_settings.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1137 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/tests/test_welcomedialog.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3094 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/tests/test_widgettoolbox.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.780581 orange-canvas-core-0.2.1/orangecanvas/application/utils/
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/utils/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    20539 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/utils/addons.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9599 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/welcomedialog.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    19895 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/application/widgettoolbox.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.780581 orange-canvas-core-0.2.1/orangecanvas/canvas/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      313 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/__init__.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.780581 orange-canvas-core-0.2.1/orangecanvas/canvas/items/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      288 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    26237 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/annotationitem.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    16390 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/controlpoints.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4065 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/graphicspathobject.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    19389 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/graphicstextitem.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    27045 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/linkitem.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    61492 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/nodeitem.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.784581 orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      738 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2077 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/test_annotationitem.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1843 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/test_controlpoints.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2029 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/test_graphicspathobject.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3214 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/test_graphicstextitem.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4033 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/test_linkitem.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7044 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/test_nodeitem.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3800 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/test_utils.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    10662 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/items/utils.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5792 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/layout.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    33228 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/scene.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.784581 orange-canvas-core-0.2.1/orangecanvas/canvas/tests/
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/tests/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2653 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/tests/test_layout.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9026 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/tests/test_scene.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      871 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/tests/test_view.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    10270 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/canvas/view.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    16942 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/config.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.788581 orange-canvas-core-0.2.1/orangecanvas/document/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      400 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/document/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    12087 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/document/commands.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    33848 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/document/editlinksdialog.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    78366 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/document/interactions.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    62110 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/document/quickmenu.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    93560 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/document/schemeedit.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4195 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/document/suggestions.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.788581 orange-canvas-core-0.2.1/orangecanvas/document/tests/
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/document/tests/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3868 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/document/tests/test_editlinksdialog.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2839 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/document/tests/test_quickmenu.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    24293 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/document/tests/test_schemeedit.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1729 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/document/tests/test_usagestatistics.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    13623 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/document/usagestatistics.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.792581 orange-canvas-core-0.2.1/orangecanvas/gui/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      163 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9124 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/dock.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    11138 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/dropshadow.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2617 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/framelesswindow.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     6002 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/iconengine.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3426 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/iconview.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1574 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/itemmodels.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7557 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/lineedit.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4683 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/quickhelp.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4979 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/splashscreen.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    11878 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/stackedwidget.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    11038 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/svgiconengine.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5523 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/test.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.792581 orange-canvas-core-0.2.1/orangecanvas/gui/tests/
+-rw-rw-r--   0 marko     (1000) marko     (1000)       31 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/tests/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1611 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_dock.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2966 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_dropshadow.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      500 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_framelesswindow.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1162 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_iconengine.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1470 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_lineedit.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1276 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_splashscreen.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2197 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_stackedwidget.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1186 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_toolbar.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2220 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_toolbox.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2933 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_toolgrid.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2600 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_tooltree.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2972 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/textlabel.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3518 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/toolbar.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    22011 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/toolbox.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    17493 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/toolgrid.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    13310 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/tooltree.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    23585 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/utils.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4084 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/gui/windowlistmanager.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.792581 orange-canvas-core-0.2.1/orangecanvas/help/
+-rw-rw-r--   0 marko     (1000) marko     (1000)       68 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/help/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2262 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/help/intersphinx.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    10508 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/help/manager.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    13159 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/help/provider.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.792581 orange-canvas-core-0.2.1/orangecanvas/help/tests/
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/help/tests/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1568 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/help/tests/test_manager.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2920 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/help/tests/test_provider.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.796581 orange-canvas-core-0.2.1/orangecanvas/icons/
+-rw-rw-r--   0 marko     (1000) marko     (1000)      777 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Arrow.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      854 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Back.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1352 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Document Info.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2081 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Documentation.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      714 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Dropdown.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3237 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Examples.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)    11315 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Get Started.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1509 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Grid.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1597 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Info.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      771 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Maximize Toolbar.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      769 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Minimize Toolbar.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1301 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/New.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1680 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Open.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      755 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Pause.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1297 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Recent.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1791 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Search.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1044 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Text Size.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1593 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/Tutorials.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2081 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/YouTube.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      600 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/arrow-right.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1010 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/default-category.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1031 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/default-widget.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      243 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/orange-canvas-core-splash.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9836 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/orange-canvas.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)    35907 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/icons/orange-splash-screen.png
+-rw-rw-r--   0 marko     (1000) marko     (1000)    18213 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/main.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.796581 orange-canvas-core-0.2.1/orangecanvas/preview/
+-rw-rw-r--   0 marko     (1000) marko     (1000)       92 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/preview/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     9381 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/preview/previewbrowser.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3876 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/preview/previewdialog.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4867 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/preview/previewmodel.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5125 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/preview/scanner.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.796581 orange-canvas-core-0.2.1/orangecanvas/preview/tests/
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/preview/tests/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1052 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/preview/tests/test_previewbrowser.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      798 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/preview/tests/test_previewdialog.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1456 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/preview/tests/test_scanner.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.800581 orange-canvas-core-0.2.1/orangecanvas/registry/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2737 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/registry/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7065 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/registry/base.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1558 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/registry/cache.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    15411 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/registry/description.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    17564 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/registry/discovery.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    12489 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/registry/qt.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.800581 orange-canvas-core-0.2.1/orangecanvas/registry/tests/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     6301 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/registry/tests/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4573 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/registry/tests/test_base.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2953 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/registry/tests/test_discovery.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     6071 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/registry/utils.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7051 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/resources.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.800581 orange-canvas-core-0.2.1/orangecanvas/scheme/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1008 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     7632 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/annotations.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      612 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/errors.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     8382 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/events.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    13665 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/link.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    11750 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/node.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    28793 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/readwrite.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    27759 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/scheme.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    46448 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/signalmanager.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.800581 orange-canvas-core-0.2.1/orangecanvas/scheme/tests/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2699 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/tests/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1407 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/tests/test_annotations.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2785 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/tests/test_links.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1754 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/tests/test_nodes.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     6967 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/tests/test_readwrite.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5688 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/tests/test_scheme.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    14841 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/tests/test_signalmanager.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    10788 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/tests/test_widgetmanager.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    25408 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/scheme/widgetmanager.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.804581 orange-canvas-core-0.2.1/orangecanvas/styles/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5773 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/styles/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      235 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/styles/darkorange.qss
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.804581 orange-canvas-core-0.2.1/orangecanvas/styles/orange/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1991 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/styles/orange/Arrow.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3321 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/styles/orange/Document Info.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      538 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/styles/orange/Dropdown.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2251 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/styles/orange/Grid.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1420 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/styles/orange/Info.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      573 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/styles/orange/Pause.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4870 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/styles/orange/Search.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)      862 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/styles/orange/Text Size.svg
+-rw-rw-r--   0 marko     (1000) marko     (1000)     8255 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/styles/orange.qss
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.804581 orange-canvas-core-0.2.1/orangecanvas/utils/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     8778 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2763 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/after_exit.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1598 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/asyncutils.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2455 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/graph.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     3408 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/image.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.804581 orange-canvas-core-0.2.1/orangecanvas/utils/localization/
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1012 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/localization/__init__.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.808581 orange-canvas-core-0.2.1/orangecanvas/utils/localization/tests/
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/localization/tests/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      816 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/localization/tests/test_localization.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2296 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/markup.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    27821 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/overlay.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     2924 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/pickle.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4290 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/pkgmeta.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    10082 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/propertybindings.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4870 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/qinvoke.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4767 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/qobjref.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      683 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/qtcompat.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      193 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/redirect.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)    12397 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/settings.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4151 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/shtools.py
+drwxrwxr-x   0 marko     (1000) marko     (1000)        0 2024-05-27 11:53:49.808581 orange-canvas-core-0.2.1/orangecanvas/utils/tests/
+-rw-rw-r--   0 marko     (1000) marko     (1000)        0 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/tests/__init__.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      838 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_after_exit.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1584 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_graph.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      761 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_markup.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4382 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_overlay.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1168 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_pkgmeta.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     6295 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_propertybindings.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     5947 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_qinvoke.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     1696 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_qobjref.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      754 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_resources.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)     4637 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_settings.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      776 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_shtools.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      523 2024-05-27 11:49:53.000000 orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_utils.py
+-rw-rw-r--   0 marko     (1000) marko     (1000)      316 2024-05-27 11:53:49.808581 orange-canvas-core-0.2.1/setup.cfg
+-rwxrwxr-x   0 marko     (1000) marko     (1000)     2244 2024-05-27 11:51:43.000000 orange-canvas-core-0.2.1/setup.py
```

### Comparing `orange-canvas-core-0.2.0a1/LICENSE.txt` & `orange-canvas-core-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/PKG-INFO` & `orange-canvas-core-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange-canvas-core
-Version: 0.2.0a1
+Version: 0.2.1
 Summary: Core component of Orange Canvas
 Home-page: http://orange.biolab.si/
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: contact@orange.biolab.si
 License: GPLv3
 Project-URL: Bug Reports, https://github.com/biolab/orange-canvas-core/issues
 Project-URL: Source, https://github.com/biolab/orange-canvas-core/
```

### Comparing `orange-canvas-core-0.2.0a1/README.rst` & `orange-canvas-core-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/make.bat` & `orange-canvas-core-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/conf.py` & `orange-canvas-core-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/application.canvasmain.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/application.canvasmain.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/application.welcomedialog.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/application.welcomedialog.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/canvas.items.nodeitem.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/canvas.items.nodeitem.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/canvas.scene.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/canvas.scene.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/document.interactions.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/document.interactions.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/document.schemeedit.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/document.schemeedit.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/gui.stackedwidget.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/gui.stackedwidget.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/overview.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/overview.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/registry.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/registry.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.annotation.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.annotation.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.events.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.events.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.node.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.node.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.scheme.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.scheme.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.signalmanager.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.signalmanager.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/docs/source/orangecanvas/scheme.widgetmanager.rst` & `orange-canvas-core-0.2.1/docs/source/orangecanvas/scheme.widgetmanager.rst`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orange_canvas_core.egg-info/PKG-INFO` & `orange-canvas-core-0.2.1/orange_canvas_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange-canvas-core
-Version: 0.2.0a1
+Version: 0.2.1
 Summary: Core component of Orange Canvas
 Home-page: http://orange.biolab.si/
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: contact@orange.biolab.si
 License: GPLv3
 Project-URL: Bug Reports, https://github.com/biolab/orange-canvas-core/issues
 Project-URL: Source, https://github.com/biolab/orange-canvas-core/
```

### Comparing `orange-canvas-core-0.2.0a1/orange_canvas_core.egg-info/SOURCES.txt` & `orange-canvas-core-0.2.1/orange_canvas_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/aboutdialog.py` & `orange-canvas-core-0.2.1/orangecanvas/application/aboutdialog.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/addons.py` & `orange-canvas-core-0.2.1/orangecanvas/application/addons.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/application.py` & `orange-canvas-core-0.2.1/orangecanvas/application/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
     }
 else:
     HighDpiScaleFactorRoundingPolicyLookup = {}
 
 
 class CanvasApplication(QApplication):
     fileOpenRequest = Signal(QUrl)
+    applicationPaletteChanged = Signal()
 
     __args = None
 
     def __init__(self, argv):
         CanvasApplication.__args, argv_ = self.parseArguments(argv)
         ns = CanvasApplication.__args
         fix_qt_plugins_path()
@@ -156,14 +157,16 @@
         if event.type() == QEvent.FileOpen:
             if not self.__in_exec:
                 self.__fileOpenUrls.append(event.url())
             else:
                 self.fileOpenRequest.emit(event.url())
         elif event.type() == QEvent.PolishRequest:
             self.configureStyle()
+        elif event.type() == QEvent.Type.ApplicationPaletteChange:
+            self.applicationPaletteChanged.emit()
         return super().event(event)
 
     def exec(self) -> int:
         while self.__fileOpenUrls:
             self.fileOpenRequest.emit(self.__fileOpenUrls.pop(0))
         self.__in_exec = True
         try:
```

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/canvasmain.py` & `orange-canvas-core-0.2.1/orangecanvas/application/canvasmain.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import sys
 import logging
 import operator
 import io
 import traceback
 from concurrent import futures
+from contextlib import contextmanager
 
 from xml.sax.saxutils import escape
 from functools import partial, reduce
 from types import SimpleNamespace
 from typing import (
     Optional, List, Union, Any, cast, Dict, Callable, IO, Sequence, Iterable,
     Tuple, TypeVar, Awaitable,
@@ -82,14 +83,15 @@
 from ..utils.qobjref import qobjref
 from . import welcomedialog
 from . import addons
 from ..preview import previewdialog, previewmodel
 from .. import config
 from . import examples
 from ..resources import load_styled_svg_icon
+from ..canvas import scene
 
 log = logging.getLogger(__name__)
 
 
 def user_documents_path():
     """
     Return the users 'Documents' folder path.
@@ -423,14 +425,20 @@
         self.save_as_action = QAction(
             self.tr("Save As ..."), self,
             objectName="action-save-as",
             toolTip=self.tr("Save current workflow as."),
             triggered=self.save_scheme_as,
             shortcut=QKeySequence.SaveAs,
         )
+        self.save_as_svg_action = QAction(
+            self.tr("Save Workflow Image as SVG ..."), self,
+            objectName="action-save-to-svg.",
+            toolTip=self.tr("Save workflow image as SVG."),
+            triggered=self.save_as_svg,
+        )
         self.quit_action = QAction(
             self.tr("Quit"), self,
             objectName="quit-action",
             triggered=QApplication.closeAllWindows,
             menuRole=QAction.QuitRole,
             shortcut=QKeySequence.Quit,
         )
@@ -642,14 +650,15 @@
         file_menu.addAction(sep)
 
         file_menu.addAction(self.close_window_action)
         sep = file_menu.addSeparator()
         sep.setObjectName("close-window-actions-separator")
         file_menu.addAction(self.save_action)
         file_menu.addAction(self.save_as_action)
+        file_menu.addAction(self.save_as_svg_action)
         sep = file_menu.addSeparator()
         sep.setObjectName("save-actions-separator")
         file_menu.addAction(self.show_properties_action)
         file_menu.addAction(self.quit_action)
 
         self.recent_menu.addAction(self.recent_action)
 
@@ -1487,32 +1496,40 @@
         `QFileDialog.Accepted` if the scheme was saved successfully and
         `QFileDialog.Rejected` if not.
         """
         document = self.current_document()
         curr_scheme = document.scheme()
         assert curr_scheme is not None
         title = self.__title_for_scheme(curr_scheme)
-        settings = QSettings()
-        settings.beginGroup("mainwindow")
+        settings = self._settings()
 
         if document.path():
             start_dir = document.path()
         else:
             start_dir = settings.value("last-scheme-dir", "", type=str)
             if not os.path.isdir(start_dir):
                 start_dir = user_documents_path()
 
             start_dir = os.path.join(start_dir, title + ".ows")
 
-        filename, _ = QFileDialog.getSaveFileName(
-            self, self.tr("Save Orange Workflow File"),
-            start_dir, self.tr("Orange Workflow (*.ows)")
-        )
-
-        if filename:
+        dialog = QFileDialog(
+            self,
+            windowTitle=self.tr("Save Orange Workflow File"),
+            directory=start_dir,
+            fileMode=QFileDialog.AnyFile,
+            acceptMode=QFileDialog.AcceptSave,
+            windowModality=Qt.WindowModal,
+            objectName="save-as-ows-filedialog",
+        )
+        dialog.setNameFilter(self.tr("Orange Workflow (*.ows)"))
+        dialog.exec()
+        files = dialog.selectedFiles()
+        dialog.deleteLater()
+        if files:
+            filename = files[0]
             settings.setValue("last-scheme-dir", os.path.dirname(filename))
             if self.save_scheme_to(curr_scheme, filename):
                 document.setPath(filename)
                 document.setModified(False)
                 self.add_recent_scheme(curr_scheme.title, document.path())
 
                 return QFileDialog.Accepted
@@ -1794,14 +1811,87 @@
         commands = properties_and_commands[1]
         for c in commands:
             undoStack.push(c)
 
         properties = properties_and_commands[0]
         document.restoreProperties(properties)
 
+    def _settings(self) -> QSettings:
+        s = QSettings()
+        s.beginGroup("mainwindow")
+        return s
+
+    def save_as_svg(self):
+        settings = self._settings()
+        settings.beginGroup("save-as-svg-filedialog")
+        path = settings.value("path", defaultValue="", type=str)
+        if path:
+            directory = os.path.dirname(path)
+        else:
+            directory = user_documents_path()
+        document_path = self.current_document().path()
+        if document_path:
+            document_basename = os.path.basename(document_path)
+            basename, _ = os.path.splitext(document_basename)
+            basename = basename + ".svg"
+        else:
+            basename = self.tr("untitled.svg")
+        dialog = QFileDialog(
+            self,
+            acceptMode=QFileDialog.AcceptSave,
+            fileMode=QFileDialog.AnyFile,
+            directory=directory,
+            windowModality=Qt.WindowModal,
+            objectName="save-as-svg-filedialog",
+        )
+        dialog.setAttribute(Qt.WA_DeleteOnClose)
+        dialog.setNameFilter(self.tr("Scalable Vector Graphics (*.svg)"))
+        dialog.selectFile(os.path.join(directory, basename))
+
+        def save():
+            files = dialog.selectedFiles()
+            if files:
+                self.__save_as_svg(files[0])
+                settings.setValue("path", files[0])
+
+        dialog.accepted.connect(save)
+        dialog.exec()
+
+    def __save_as_svg(self, path):
+        doc = self.current_document()
+        content = scene.grab_svg(doc.scene())
+        with self._handle_os_write_error():
+            with open(path, "wt", encoding="utf-8") as f:
+                f.write(content)
+
+    @contextmanager
+    def _handle_os_write_error(self):
+        try:
+            yield
+        except PermissionError as ex:
+            log.error("Write error", exc_info=True)
+            message_warning(
+                self.tr('"%(path)s" could not be saved. You do not '
+                        'have write permissions (%(strerror)s).') %
+                {"path": ex.filename, "strerror": ex.strerror},
+                title="",
+                informative_text=self.tr(
+                    "Change the file system permissions or choose "
+                    "another location."),
+                parent=self
+            )
+        except OSError as ex:
+            log.error("Write error", exc_info=True)
+            message_warning(
+                self.tr('"%(path)s" could not be saved.') %
+                {"path": ex.filename},
+                title="",
+                informative_text=ex.strerror
+            )
+
     def recent_scheme(self):
         # type: () -> int
         """
         Browse recent schemes.
 
         Return QDialog.Rejected if the user canceled the operation and
         QDialog.Accepted otherwise.
```

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/canvastooldock.py` & `orange-canvas-core-0.2.1/orangecanvas/application/canvastooldock.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/examples.py` & `orange-canvas-core-0.2.1/orangecanvas/application/examples.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/outputview.py` & `orange-canvas-core-0.2.1/orangecanvas/application/outputview.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/schemeinfo.py` & `orange-canvas-core-0.2.1/orangecanvas/application/schemeinfo.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/settings.py` & `orange-canvas-core-0.2.1/orangecanvas/application/settings.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_addons.py` & `orange-canvas-core-0.2.1/orangecanvas/application/tests/test_addons.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_addons_utils.py` & `orange-canvas-core-0.2.1/orangecanvas/application/tests/test_addons_utils.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_application.py` & `orange-canvas-core-0.2.1/orangecanvas/application/tests/test_application.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 import os
 import sys
 import time
 import unittest
 
+from AnyQt.QtGui import QPalette
+from AnyQt.QtTest import QSignalSpy
+
 from orangecanvas.utils import shtools as sh
 from orangecanvas.application import application as appmod
 from orangecanvas.utils.shtools import temp_named_file
 
 
 def application_test_helper():
     app = appmod.CanvasApplication([])
+    p = app.palette()
+    spy = QSignalSpy(app.applicationPaletteChanged)
+    p.setColor(QPalette.Base, p.color(QPalette.Text))
+    app.setPalette(p)
+    assert list(spy) == [[]]
     app.quit()
     return
 
 
 class TestApplication(unittest.TestCase):
     def test_application(self):
         res = sh.python_run([
```

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_canvastooldock.py` & `orange-canvas-core-0.2.1/orangecanvas/application/tests/test_canvastooldock.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_main.py` & `orange-canvas-core-0.2.1/orangecanvas/application/tests/test_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
 import unittest
 from contextlib import contextmanager
 from functools import wraps
 from typing import Iterable
 from unittest.mock import patch, Mock
 
+from AnyQt.QtCore import Qt
+from AnyQt.QtGui import QPalette
+
 from orangecanvas import config
 from orangecanvas.application.canvasmain import CanvasMainWindow
 from orangecanvas.config import Config
 from orangecanvas.gui.test import QAppTestCase
 from orangecanvas.main import Main
 from orangecanvas.registry import WidgetDiscovery
 from orangecanvas.registry.tests import set_up_modules, tear_down_modules
@@ -131,7 +134,23 @@
         m = Main()
         with patch.object(self.app, "exec", lambda: 42), \
              patch.object(CanvasMainWindow, "open_scheme_file", Mock()), \
              temp_named_file('<scheme version="2.0"></scheme>') as fname:
             res = m.run(["-", "--no-welcome", "--no-splash", fname])
             CanvasMainWindow.open_scheme_file.assert_called_with(fname)
         self.assertEqual(res, 42)
+
+    @with_patched_main_application
+    def test_run_stylesheet_reconfigure(self):
+        m = Main()
+        m.parse_arguments(["-", "--config", f"{__name__}.TestConfig"])
+        m.window = m.create_main_window()
+        m.application = self.app
+
+        def setpalette(color):
+            self.app.setPalette(QPalette(color))
+            m._Main__reconfigure_stylesheet()
+
+        setpalette(Qt.white)
+        sheet = m.window.styleSheet()
+        setpalette(Qt.black)
+        self.assertNotEqual(sheet, m.window.styleSheet())
```

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_mainwindow.py` & `orange-canvas-core-0.2.1/orangecanvas/application/tests/test_mainwindow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import io
 import os
 import tempfile
 from unittest.mock import patch
 
 from AnyQt.QtGui import QWhatsThisClickedEvent
-from AnyQt.QtWidgets import QToolButton, QDialog, QMessageBox, QApplication
+from AnyQt.QtWidgets import (
+    QToolButton, QDialog, QMessageBox, QApplication, QFileDialog
+)
 
 from .. import addons
 from ..outputview import TextStream
 from ..utils.addons import _QueryResult, Installable
 from ...scheme import SchemeTextAnnotation, SchemeLink
 from ...gui.quickhelp import QuickHelpTipEvent, QuickHelp
 from ...utils.shtools import temp_named_file
@@ -169,18 +172,39 @@
         w = self.w
         w.current_document().setPath(self.filename)
         with patch.object(w, "save_scheme_as") as f:
             w.save_scheme()
             f.assert_not_called()
 
         w.current_document().setPath("")
-        with patch("AnyQt.QtWidgets.QFileDialog.getSaveFileName",
-                   return_value=(self.filename, "")) as f:
+
+        def exec(myself):
+            myself.setOption(QFileDialog.DontUseNativeDialog)
+            myself.setOption(QFileDialog.DontConfirmOverwrite)
+            myself.selectFile(self.filename)
+            myself.accept()
+
+        with patch("AnyQt.QtWidgets.QFileDialog.exec", exec):
             w.save_scheme()
-            self.assertEqual(w.current_document().path(), self.filename)
+            self.assertTrue(os.path.samefile(w.current_document().path(), self.filename))
+
+    def test_save_svg_image(self):
+        w = self.w
+        scheme = w.current_document().scheme()
+        scheme.load_from(io.BytesIO(TEST_OWS), registry=w.widget_registry)
+        with patch("AnyQt.QtWidgets.QFileDialog.exec"):
+            w.save_as_svg()
+            dialog = w.findChild(QFileDialog, "save-as-svg-filedialog")
+            dialog.setOption(QFileDialog.DontUseNativeDialog)
+            dialog.setOption(QFileDialog.DontConfirmOverwrite)
+            dialog.selectFile(self.filename)
+            dialog.accept()
+        with open(self.filename, "rb") as f:
+            contents = f.read()
+        self.assertIn(b"<svg", contents)
 
     def test_save_swp(self):
         w = self.w
         swpname = swp_name(w)
 
         with patch.object(w, "save_swp_to") as f:
             w.save_swp()
```

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_outputview.py` & `orange-canvas-core-0.2.1/orangecanvas/application/tests/test_outputview.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_schemeinfo.py` & `orange-canvas-core-0.2.1/orangecanvas/application/tests/test_schemeinfo.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_settings.py` & `orange-canvas-core-0.2.1/orangecanvas/application/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_welcomedialog.py` & `orange-canvas-core-0.2.1/orangecanvas/application/tests/test_welcomedialog.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/tests/test_widgettoolbox.py` & `orange-canvas-core-0.2.1/orangecanvas/application/tests/test_widgettoolbox.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/utils/addons.py` & `orange-canvas-core-0.2.1/orangecanvas/application/utils/addons.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/welcomedialog.py` & `orange-canvas-core-0.2.1/orangecanvas/application/welcomedialog.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/application/widgettoolbox.py` & `orange-canvas-core-0.2.1/orangecanvas/application/widgettoolbox.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/annotationitem.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/annotationitem.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/controlpoints.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/controlpoints.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/graphicspathobject.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/graphicspathobject.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/graphicstextitem.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/graphicstextitem.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/linkitem.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/linkitem.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/nodeitem.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/nodeitem.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/__init__.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/test_annotationitem.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/test_annotationitem.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/test_controlpoints.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/test_controlpoints.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/test_graphicspathobject.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/test_graphicspathobject.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/test_graphicstextitem.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/test_graphicstextitem.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/test_linkitem.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/test_linkitem.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/test_nodeitem.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/test_nodeitem.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/tests/test_utils.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/items/utils.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/items/utils.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/layout.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/layout.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/scene.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -946,26 +946,31 @@
             else:
                 return super().metric(metric)
 
 else:
     _QSvgGenerator = QSvgGenerator  # type: ignore
 
 
-def grab_svg(scene):
-    # type: (QGraphicsScene) -> str
+def grab_svg(scene: QGraphicsScene) -> str:
     """
     Return a SVG rendering of the scene contents.
 
     Parameters
     ----------
     scene : :class:`CanvasScene`
 
     """
     svg_buffer = QBuffer()
     gen = _QSvgGenerator()
+    views = scene.views()
+    if views:
+        screen = views[0].screen()
+        if screen is not None:
+            res = screen.physicalDotsPerInch()
+            gen.setResolution(int(res))
     gen.setOutputDevice(svg_buffer)
 
     items_rect = scene.itemsBoundingRect().adjusted(-10, -10, 10, 10)
 
     if items_rect.isNull():
         items_rect = QRectF(0, 0, 10, 10)
```

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/tests/test_layout.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/tests/test_scene.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/tests/test_scene.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/tests/test_view.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/canvas/view.py` & `orange-canvas-core-0.2.1/orangecanvas/canvas/view.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/config.py` & `orange-canvas-core-0.2.1/orangecanvas/config.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/document/commands.py` & `orange-canvas-core-0.2.1/orangecanvas/document/commands.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/document/editlinksdialog.py` & `orange-canvas-core-0.2.1/orangecanvas/document/editlinksdialog.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/document/interactions.py` & `orange-canvas-core-0.2.1/orangecanvas/document/interactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import abc
 import logging
 from functools import reduce
 
 from AnyQt.QtWidgets import (
     QApplication, QGraphicsRectItem, QGraphicsSceneMouseEvent,
     QGraphicsSceneContextMenuEvent, QWidget, QGraphicsItem,
-    QGraphicsSceneDragDropEvent, QMenu, QAction
+    QGraphicsSceneDragDropEvent, QMenu, QAction, QWidgetAction, QLabel
 )
 from AnyQt.QtGui import QPen, QBrush, QColor, QFontMetrics, QKeyEvent, QFont
 from AnyQt.QtCore import (
     Qt, QObject, QCoreApplication, QSizeF, QPointF, QRect, QRectF, QLineF,
     QPoint, QMimeData,
 )
 from AnyQt.QtCore import pyqtSignal as Signal
@@ -185,14 +185,26 @@
     def cancelReason(self):
         # type: () -> int
         """
         Return the reason the interaction was canceled.
         """
         return self.__cancelReason
 
+    def postQuickTip(self, contents: str) -> None:
+        """
+        Post a QuickHelpTipEvent with rich text `contents` to the document
+        editor.
+        """
+        hevent = QuickHelpTipEvent("", contents)
+        QApplication.postEvent(self.document, hevent)
+
+    def clearQuickTip(self):
+        """Clear the quick tip help event."""
+        self.postQuickTip("")
+
     def mousePressEvent(self, event):
         # type: (QGraphicsSceneMouseEvent) -> bool
         """
         Handle a `QGraphicsScene.mousePressEvent`.
         """
         return False
 
@@ -444,27 +456,24 @@
             self.from_item = anchor_item.parentNodeItem()
             if isinstance(anchor_item, items.SourceAnchorItem):
                 self.direction = NewLinkAction.FROM_SOURCE
             else:
                 self.direction = NewLinkAction.FROM_SINK
 
             event.accept()
-
-            helpevent = QuickHelpTipEvent(
-                self.tr("Create a new link"),
+            self.postQuickTip(
                 self.tr('<h3>Create new link</h3>'
                         '<p>Drag a link to an existing node or release on '
                         'an empty spot to create a new node.</p>'
                         '<p>Hold Shift when releasing the mouse button to '
                         'edit connections.</p>'
 #                        '<a href="help://orange-canvas/create-new-links">'
 #                        'More ...</a>'
                         )
             )
-            QCoreApplication.postEvent(self.document, helpevent)
             return True
         else:
             # Whoever put us in charge did not know what he was doing.
             self.cancel(self.ErrorReason)
             return False
 
     def mouseMoveEvent(self, event):
@@ -871,16 +880,15 @@
 
     def end(self):
         # type: () -> None
         self.cleanup()
         self.reset_open_anchor()
         # Remove the help tip set in mousePressEvent
         self.macro = None
-        helpevent = QuickHelpTipEvent("", "")
-        QCoreApplication.postEvent(self.document, helpevent)
+        self.clearQuickTip()
         super().end()
 
     def cancel(self, reason=UserInteraction.OtherReason):
         # type: (int) -> None
         self.cleanup()
         self.reset_open_anchor()
         super().cancel(reason)
@@ -1336,25 +1344,21 @@
         self.annotation = None  # type: Optional[scheme.SchemeArrowAnnotation]
         self.color = "red"
         self.cancelOnEsc = True
 
     def start(self):
         # type: () -> None
         self.document.view().setCursor(Qt.CrossCursor)
-
-        helpevent = QuickHelpTipEvent(
-            self.tr("Click and drag to create a new arrow"),
+        self.postQuickTip(
             self.tr('<h3>New arrow annotation</h3>'
                     '<p>Click and drag to create a new arrow annotation</p>'
 #                    '<a href="help://orange-canvas/arrow-annotations>'
 #                    'More ...</a>'
                     )
         )
-        QCoreApplication.postEvent(self.document, helpevent)
-
         super().start()
 
     def setColor(self, color):
         """
         Set the color for the new arrow.
         """
         self.color = color
@@ -1424,19 +1428,15 @@
 
     def end(self):
         # type: () -> None
         self.down_pos = None
         self.arrow_item = None
         self.annotation = None
         self.document.view().setCursor(Qt.ArrowCursor)
-
-        # Clear the help tip
-        helpevent = QuickHelpTipEvent("", "")
-        QCoreApplication.postEvent(self.document, helpevent)
-
+        self.clearQuickTip()
         super().end()
 
 
 def rect_to_tuple(rect):
     # type: (QRectF) -> Tuple[float, float, float, float]
     """
     Convert a QRectF into a (x, y, width, height) tuple.
@@ -1461,26 +1461,24 @@
     def setFont(self, font):
         # type: (QFont) -> None
         self.font = QFont(font)
 
     def start(self):
         # type: () -> None
         self.document.view().setCursor(Qt.CrossCursor)
-
-        helpevent = QuickHelpTipEvent(
-            self.tr("Click to create a new text annotation"),
+        self.postQuickTip(
             self.tr('<h3>New text annotation</h3>'
                     '<p>Click (and drag to resize) on the canvas to create '
                     'a new text annotation item.</p>'
+                    '<p>Right click on the annotation to change how it is '
+                    'rendered (Markdown, HTML, ...).</p>'
 #                    '<a href="help://orange-canvas/text-annotations">'
 #                    'More ...</a>'
                     )
         )
-        QCoreApplication.postEvent(self.document, helpevent)
-
         super().start()
 
     def createNewAnnotation(self, rect):
         # type: (QRectF) -> None
         """
         Create a new TextAnnotation at with `rect` as the geometry.
         """
@@ -1586,19 +1584,15 @@
             self.scene.removeItem(self.control)
 
         self.control = None
         self.down_pos = None
         self.annotation_item = None
         self.annotation = None
         self.document.view().setCursor(Qt.ArrowCursor)
-
-        # Clear the help tip
-        helpevent = QuickHelpTipEvent("", "")
-        QCoreApplication.postEvent(self.document, helpevent)
-
+        self.clearQuickTip()
         super().end()
 
 
 class ResizeTextAnnotation(UserInteraction):
     """
     Resize a Text Annotation interaction handler.
     """
@@ -1672,14 +1666,23 @@
     def __on_textGeometryChanged(self):
         # type: () -> None
         assert self.control is not None and self.item is not None
         if not self.control.isControlActive():
             rect = self.item.geometry()
             self.control.setRect(rect)
 
+    def start(self) -> None:
+        super().start()
+        self.postQuickTip(
+            self.tr('<h3>Edit Text Annotation</h3>'
+                    '<p>Drag control points to resize the annotation.</p>'
+                    '<p>Right click on the annotation to change how it is '
+                    'rendered (Markdown, HTML, ...).</p>')
+        )
+
     def cancel(self, reason=UserInteraction.OtherReason):
         # type: (int) -> None
         log.debug("ResizeTextAnnotation.cancel(%s)", reason)
         if self.item is not None and self.savedRect is not None:
             self.item.setGeometry(self.savedRect)
         super().cancel(reason)
 
@@ -1690,15 +1693,15 @@
 
         if self.item is not None and self.savedFramePen is not None:
             self.item.setFramePen(self.savedFramePen)
 
         self.item = None
         self.annotation = None
         self.control = None
-
+        self.clearQuickTip()
         super().end()
 
 
 class ResizeArrowAnnotation(UserInteraction):
     """
     Resize an Arrow Annotation interaction handler.
     """
@@ -2080,15 +2083,23 @@
         In case there are multiple handlers that accepted the event, a menu
         is used to select the handler.
         """
         handler: Optional[DropHandler] = None
         if len(self.__accepts) == 1:
             ep, handler = self.__accepts[0]
         elif len(self.__accepts) > 1:
+            class Title(QWidgetAction):
+                def createWidget(self, parent):
+                    return QLabel("<b>Select a widget</b>", parent, margin=2)
+
             menu = QMenu(event.widget())
+            menu.addAction(Title(menu))
+            separator = QAction()
+            separator.setSeparator(True)
+            menu.addAction(separator)
             for ep_, handler_ in self.__accepts:
                 ac = action_for_handler(handler_, document, event)
                 if ac is None:
                     ac = menu.addAction(ep_.name, )
                 else:
                     menu.addAction(ac)
                     ac.setParent(menu)
```

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/document/quickmenu.py` & `orange-canvas-core-0.2.1/orangecanvas/document/quickmenu.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/document/schemeedit.py` & `orange-canvas-core-0.2.1/orangecanvas/document/schemeedit.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/document/suggestions.py` & `orange-canvas-core-0.2.1/orangecanvas/document/suggestions.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/document/tests/test_editlinksdialog.py` & `orange-canvas-core-0.2.1/orangecanvas/document/tests/test_editlinksdialog.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/document/tests/test_quickmenu.py` & `orange-canvas-core-0.2.1/orangecanvas/document/tests/test_quickmenu.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/document/tests/test_schemeedit.py` & `orange-canvas-core-0.2.1/orangecanvas/document/tests/test_schemeedit.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/document/tests/test_usagestatistics.py` & `orange-canvas-core-0.2.1/orangecanvas/document/tests/test_usagestatistics.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/document/usagestatistics.py` & `orange-canvas-core-0.2.1/orangecanvas/document/usagestatistics.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/dock.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/dock.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/dropshadow.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/dropshadow.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/framelesswindow.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/framelesswindow.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/iconengine.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/iconengine.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/iconview.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/iconview.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/itemmodels.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/itemmodels.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/lineedit.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/lineedit.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/quickhelp.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/quickhelp.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/splashscreen.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/splashscreen.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/stackedwidget.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/stackedwidget.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/svgiconengine.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/svgiconengine.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/test.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/test.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_dock.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_dock.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_dropshadow.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_dropshadow.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_iconengine.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_iconengine.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_lineedit.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_lineedit.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_splashscreen.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_splashscreen.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_stackedwidget.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_stackedwidget.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_toolbar.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_toolbar.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_toolbox.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_toolbox.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_toolgrid.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_toolgrid.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/tests/test_tooltree.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/tests/test_tooltree.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/textlabel.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/textlabel.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/toolbar.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/toolbar.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/toolbox.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/toolbox.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/toolgrid.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/toolgrid.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/tooltree.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/tooltree.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/utils.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/utils.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/gui/windowlistmanager.py` & `orange-canvas-core-0.2.1/orangecanvas/gui/windowlistmanager.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/help/intersphinx.py` & `orange-canvas-core-0.2.1/orangecanvas/help/intersphinx.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/help/manager.py` & `orange-canvas-core-0.2.1/orangecanvas/help/manager.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/help/provider.py` & `orange-canvas-core-0.2.1/orangecanvas/help/provider.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/help/tests/test_manager.py` & `orange-canvas-core-0.2.1/orangecanvas/help/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/help/tests/test_provider.py` & `orange-canvas-core-0.2.1/orangecanvas/help/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Arrow.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Arrow.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Back.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Back.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Document Info.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Document Info.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Documentation.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Documentation.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Dropdown.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Dropdown.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Examples.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Examples.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Get Started.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Get Started.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Grid.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Grid.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Info.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Info.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Maximize Toolbar.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Maximize Toolbar.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Minimize Toolbar.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Minimize Toolbar.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/New.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/New.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Open.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Open.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Pause.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Pause.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Recent.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Recent.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Search.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Search.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Text Size.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Text Size.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/Tutorials.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/Tutorials.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/YouTube.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/YouTube.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/arrow-right.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/arrow-right.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/default-category.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/default-category.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/default-widget.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/default-widget.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/orange-canvas.svg` & `orange-canvas-core-0.2.1/orangecanvas/icons/orange-canvas.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/icons/orange-splash-screen.png` & `orange-canvas-core-0.2.1/orangecanvas/icons/orange-splash-screen.png`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/main.py` & `orange-canvas-core-0.2.1/orangecanvas/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 """
 import argparse
-
 import os
 import sys
 import gc
 import logging
 import pickle
 import shlex
 import warnings
-from typing import List, Optional, IO, Any
+from typing import List, Optional, IO, Any, Iterable
 
 from urllib.request import getproxies
 from contextlib import ExitStack, closing
 
 from AnyQt.QtGui import QFont, QColor, QPalette
 from AnyQt.QtCore import Qt, QSettings, QTimer, QUrl, QDir
 
@@ -172,14 +171,15 @@
         self.close_splash_screen()
         return widget_registry
 
     def setup_application(self):
         # sys.argv[0] must be in QApplication's argv list.
         self.application = CanvasApplication(sys.argv[:1] + self.arguments)
         self.application.setWindowIcon(self.config.application_icon())
+        self.application.applicationPaletteChanged.connect(self.__reconfigure_stylesheet)
         # Update the arguments
         self.arguments = self.application.arguments()[1:]
         fix_set_proxy_env()
 
     def tear_down_application(self):
         gc.collect()
         self.application.processEvents()
@@ -285,15 +285,15 @@
     def tear_down_logging(self):
         pass
 
     def create_main_window(self) -> CanvasMainWindow:
         """Create the (initial) main window."""
         return CanvasMainWindow()
 
-    window: CanvasMainWindow
+    window: Optional[CanvasMainWindow] = None
 
     def setup_main_window(self):
         stylesheet = self.main_window_stylesheet()
         self.window = window = self.create_main_window()
         if sys.platform != "darwin":  # on macOS transient document views do not have an icon.
             window.setWindowIcon(self.config.application_icon())
         window.setStyleSheet(stylesheet)
@@ -373,14 +373,24 @@
         if self.__excepthook__ is not None:
             sys.excepthook = self.__excepthook__
         if self.__stderr__ is not None:
             sys.stderr = self.__stderr__
         if self.__stdout__ is not None:
             sys.stdout = self.__stdout__
 
+    def _main_windows(self) -> Iterable[CanvasMainWindow]:
+        first = self.window
+        return (*((first,) if first else ()), *CanvasMainWindow._instances)
+
+    def __reconfigure_stylesheet(self) -> None:
+        ssheet = self.main_window_stylesheet()
+        for inst in self._main_windows():
+            if inst.styleSheet() != ssheet:
+                inst.setStyleSheet(ssheet)
+
 
 def fix_win_pythonw_std_stream():
     """
     On windows when running without a console (using pythonw.exe without I/O
     redirection) the std[err|out] file descriptors are invalid
     (`http://bugs.python.org/issue706263`_). We `fix` this by setting the
     stdout/stderr to `os.devnull`.
```

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/preview/previewbrowser.py` & `orange-canvas-core-0.2.1/orangecanvas/preview/previewbrowser.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/preview/previewdialog.py` & `orange-canvas-core-0.2.1/orangecanvas/preview/previewdialog.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/preview/previewmodel.py` & `orange-canvas-core-0.2.1/orangecanvas/preview/previewmodel.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/preview/scanner.py` & `orange-canvas-core-0.2.1/orangecanvas/preview/scanner.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/preview/tests/test_previewbrowser.py` & `orange-canvas-core-0.2.1/orangecanvas/preview/tests/test_previewbrowser.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/preview/tests/test_previewdialog.py` & `orange-canvas-core-0.2.1/orangecanvas/preview/tests/test_previewdialog.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/preview/tests/test_scanner.py` & `orange-canvas-core-0.2.1/orangecanvas/preview/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/registry/__init__.py` & `orange-canvas-core-0.2.1/orangecanvas/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/registry/base.py` & `orange-canvas-core-0.2.1/orangecanvas/registry/base.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/registry/cache.py` & `orange-canvas-core-0.2.1/orangecanvas/registry/cache.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/registry/description.py` & `orange-canvas-core-0.2.1/orangecanvas/registry/description.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/registry/discovery.py` & `orange-canvas-core-0.2.1/orangecanvas/registry/discovery.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/registry/qt.py` & `orange-canvas-core-0.2.1/orangecanvas/registry/qt.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/registry/tests/__init__.py` & `orange-canvas-core-0.2.1/orangecanvas/registry/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/registry/tests/test_base.py` & `orange-canvas-core-0.2.1/orangecanvas/registry/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/registry/tests/test_discovery.py` & `orange-canvas-core-0.2.1/orangecanvas/registry/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/registry/utils.py` & `orange-canvas-core-0.2.1/orangecanvas/registry/utils.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/resources.py` & `orange-canvas-core-0.2.1/orangecanvas/resources.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/__init__.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/annotations.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/annotations.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/errors.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/errors.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/events.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/events.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/link.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/link.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/node.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/node.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/readwrite.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/readwrite.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/scheme.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/scheme.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/signalmanager.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/signalmanager.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/__init__.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/test_annotations.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/test_links.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/test_nodes.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/test_readwrite.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/tests/test_readwrite.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/test_scheme.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/tests/test_scheme.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/test_signalmanager.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/tests/test_signalmanager.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/tests/test_widgetmanager.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/tests/test_widgetmanager.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/scheme/widgetmanager.py` & `orange-canvas-core-0.2.1/orangecanvas/scheme/widgetmanager.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/styles/__init__.py` & `orange-canvas-core-0.2.1/orangecanvas/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Arrow.svg` & `orange-canvas-core-0.2.1/orangecanvas/styles/orange/Arrow.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Document Info.svg` & `orange-canvas-core-0.2.1/orangecanvas/styles/orange/Document Info.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Dropdown.svg` & `orange-canvas-core-0.2.1/orangecanvas/styles/orange/Dropdown.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Grid.svg` & `orange-canvas-core-0.2.1/orangecanvas/styles/orange/Grid.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Info.svg` & `orange-canvas-core-0.2.1/orangecanvas/styles/orange/Info.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Pause.svg` & `orange-canvas-core-0.2.1/orangecanvas/styles/orange/Pause.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Search.svg` & `orange-canvas-core-0.2.1/orangecanvas/styles/orange/Search.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/styles/orange/Text Size.svg` & `orange-canvas-core-0.2.1/orangecanvas/styles/orange/Text Size.svg`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/styles/orange.qss` & `orange-canvas-core-0.2.1/orangecanvas/styles/orange.qss`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/__init__.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/after_exit.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/after_exit.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/asyncutils.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/asyncutils.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/graph.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/graph.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/image.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/image.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/localization/__init__.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/localization/__init__.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/localization/tests/test_localization.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/localization/tests/test_localization.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/markup.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/markup.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/overlay.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/overlay.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/pickle.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/pickle.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/pkgmeta.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/pkgmeta.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/propertybindings.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/propertybindings.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/qinvoke.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/qinvoke.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/qobjref.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/qobjref.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/qtcompat.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/qtcompat.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/settings.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/settings.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/shtools.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/shtools.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_after_exit.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_after_exit.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_graph.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_markup.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_markup.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_overlay.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_overlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # pylint: disable=protected-access
 
 import unittest.mock
 
 from AnyQt.QtCore import Qt, QEvent
-from AnyQt.QtTest import QTest
+from AnyQt.QtTest import QTest, QSignalSpy
 from AnyQt.QtWidgets import QWidget, QApplication
 
 from orangecanvas.gui.test import QAppTestCase
 from orangecanvas.utils.overlay import NotificationWidget, NotificationOverlay, Notification, \
     NotificationServer
 
 
 class TestOverlay(QAppTestCase):
     def setUp(self) -> None:
+        super().setUp()
         self.container = QWidget()
         self.overlay = NotificationOverlay(self.container)
         self.server = NotificationServer()
 
         self.server.newNotification.connect(self.overlay.addNotification)
         self.server.nextNotification.connect(self.overlay.nextWidget)
 
@@ -26,14 +27,15 @@
                                   accept_button_label="Ok")
 
     def tearDown(self) -> None:
         self.container = None
         self.overlay = None
         self.notif = None
         self.server = None
+        super().tearDown()
 
     def test_notification_widget(self):
         stdb = NotificationWidget.Ok | NotificationWidget.Close
         notifw = NotificationWidget(self.overlay,
                                     title="Titl",
                                     text="Tixt",
                                     standardButtons=stdb)
@@ -73,16 +75,15 @@
     def test_two_overlays(self):
         container2 = QWidget()
         overlay2 = NotificationOverlay(container2)
 
         self.server.newNotification.connect(overlay2.addNotification)
         self.server.nextNotification.connect(overlay2.nextWidget)
 
-        mock = unittest.mock.MagicMock()
-        self.notif.accepted.connect(mock)
+        spy = QSignalSpy(self.notif.accepted)
 
         self.server.registerNotification(self.notif)
 
         self.container.show()
         container2.show()
 
         w1 = self.overlay.currentWidget()
@@ -90,15 +91,15 @@
 
         self.assertTrue(w1.isVisible())
         self.assertTrue(w2.isVisible())
 
         button = w2.button(NotificationWidget.Ok)
         QTest.mouseClick(button, Qt.LeftButton)
 
-        mock.assert_called_once_with()
+        self.assertSequenceEqual(list(spy), [[]])
 
         self.assertFalse(w1.isVisible())
         self.assertFalse(w2.isVisible())
 
     def test_queued_notifications(self):
         notif2 = Notification(title="Hello universe!",
                               text="I'm another notif! I'm about to queue behind my older brother.")
```

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_pkgmeta.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_pkgmeta.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_propertybindings.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_propertybindings.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_qinvoke.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_qinvoke.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_qobjref.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_qobjref.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_resources.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_settings.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_shtools.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_shtools.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/orangecanvas/utils/tests/test_utils.py` & `orange-canvas-core-0.2.1/orangecanvas/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `orange-canvas-core-0.2.0a1/setup.py` & `orange-canvas-core-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 from setuptools import setup, find_packages
 
 NAME = "orange-canvas-core"
-VERSION = "0.2.0a1"
+VERSION = "0.2.1"
 DESCRIPTION = "Core component of Orange Canvas"
 
 with open("README.rst", "rt", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 URL = "http://orange.biolab.si/"
 AUTHOR = "Bioinformatics Laboratory, FRI UL"
```

