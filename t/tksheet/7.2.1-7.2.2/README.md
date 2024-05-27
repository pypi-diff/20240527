# Comparing `tmp/tksheet-7.2.1.tar.gz` & `tmp/tksheet-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-7.2.1.tar", last modified: Wed May 22 17:26:31 2024, max compression
+gzip compressed data, was "tksheet-7.2.2.tar", last modified: Mon May 27 15:51:37 2024, max compression
```

## Comparing `tksheet-7.2.1.tar` & `tksheet-7.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-22 17:26:31.830066 tksheet-7.2.1/
--rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2024-01-20 17:50:45.000000 tksheet-7.2.1/LICENSE.txt
--rw-r--r--   0 rg        (1000) rg        (1000)     6145 2024-05-22 17:26:31.830066 tksheet-7.2.1/PKG-INFO
--rw-rw-r--   0 rg        (1000) rg        (1000)     4046 2024-05-15 18:18:34.000000 tksheet-7.2.1/README.md
--rw-rw-r--   0 rg        (1000) rg        (1000)     1099 2024-05-22 16:11:28.000000 tksheet-7.2.1/pyproject.toml
--rw-rw-r--   0 rg        (1000) rg        (1000)       38 2024-05-22 17:26:31.830066 tksheet-7.2.1/setup.cfg
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-22 17:26:31.830066 tksheet-7.2.1/tksheet/
--rw-rw-r--   0 rg        (1000) rg        (1000)     2124 2024-05-22 16:11:28.000000 tksheet-7.2.1/tksheet/__init__.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    51594 2024-01-25 08:44:04.000000 tksheet-7.2.1/tksheet/colors.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   101151 2024-05-22 17:16:45.000000 tksheet-7.2.1/tksheet/column_headers.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    10037 2024-01-25 08:44:04.000000 tksheet-7.2.1/tksheet/formatters.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    40835 2024-05-20 07:30:00.000000 tksheet-7.2.1/tksheet/functions.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   324259 2024-05-22 17:17:53.000000 tksheet-7.2.1/tksheet/main_table.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    13628 2024-05-17 10:30:02.000000 tksheet-7.2.1/tksheet/other_classes.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   107384 2024-05-22 17:16:16.000000 tksheet-7.2.1/tksheet/row_index.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   267749 2024-05-22 17:21:20.000000 tksheet-7.2.1/tksheet/sheet.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    12262 2024-05-20 09:45:04.000000 tksheet-7.2.1/tksheet/sheet_options.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     6548 2024-05-21 08:53:42.000000 tksheet-7.2.1/tksheet/text_editor.py
--rw-r--r--   0 rg        (1000) rg        (1000)    14474 2024-05-21 08:36:35.000000 tksheet-7.2.1/tksheet/themes.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     8356 2024-05-19 18:22:05.000000 tksheet-7.2.1/tksheet/top_left_rectangle.py
--rw-rw-r--   0 rg        (1000) rg        (1000)      340 2024-01-25 08:44:04.000000 tksheet-7.2.1/tksheet/types.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     3452 2024-05-20 09:29:16.000000 tksheet-7.2.1/tksheet/vars.py
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-22 17:26:31.830066 tksheet-7.2.1/tksheet.egg-info/
--rw-r--r--   0 rg        (1000) rg        (1000)     6145 2024-05-22 17:26:31.000000 tksheet-7.2.1/tksheet.egg-info/PKG-INFO
--rw-rw-r--   0 rg        (1000) rg        (1000)      481 2024-05-22 17:26:31.000000 tksheet-7.2.1/tksheet.egg-info/SOURCES.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        1 2024-05-22 17:26:31.000000 tksheet-7.2.1/tksheet.egg-info/dependency_links.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        8 2024-05-22 17:26:31.000000 tksheet-7.2.1/tksheet.egg-info/top_level.txt
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-27 15:51:37.406540 tksheet-7.2.2/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2024-01-20 17:50:45.000000 tksheet-7.2.2/LICENSE.txt
+-rw-r--r--   0 rg        (1000) rg        (1000)     6319 2024-05-27 15:51:37.406540 tksheet-7.2.2/PKG-INFO
+-rw-r--r--   0 rg        (1000) rg        (1000)     4222 2024-05-25 15:33:08.000000 tksheet-7.2.2/README.md
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1099 2024-05-22 17:27:00.000000 tksheet-7.2.2/pyproject.toml
+-rw-rw-r--   0 rg        (1000) rg        (1000)       38 2024-05-27 15:51:37.406540 tksheet-7.2.2/setup.cfg
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-27 15:51:37.402540 tksheet-7.2.2/tksheet/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     2124 2024-05-22 17:27:00.000000 tksheet-7.2.2/tksheet/__init__.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    51594 2024-01-25 08:44:04.000000 tksheet-7.2.2/tksheet/colors.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   102039 2024-05-27 15:41:38.000000 tksheet-7.2.2/tksheet/column_headers.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    10037 2024-01-25 08:44:04.000000 tksheet-7.2.2/tksheet/formatters.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    40835 2024-05-20 07:30:00.000000 tksheet-7.2.2/tksheet/functions.py
+-rw-r--r--   0 rg        (1000) rg        (1000)   324868 2024-05-27 15:41:21.000000 tksheet-7.2.2/tksheet/main_table.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    13628 2024-05-17 10:30:02.000000 tksheet-7.2.2/tksheet/other_classes.py
+-rw-r--r--   0 rg        (1000) rg        (1000)   108213 2024-05-27 15:41:55.000000 tksheet-7.2.2/tksheet/row_index.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   268309 2024-05-27 15:43:20.000000 tksheet-7.2.2/tksheet/sheet.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    12262 2024-05-20 09:45:04.000000 tksheet-7.2.2/tksheet/sheet_options.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     6548 2024-05-21 08:53:42.000000 tksheet-7.2.2/tksheet/text_editor.py
+-rw-r--r--   0 rg        (1000) rg        (1000)    14474 2024-05-21 08:36:35.000000 tksheet-7.2.2/tksheet/themes.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     8436 2024-05-26 07:23:05.000000 tksheet-7.2.2/tksheet/top_left_rectangle.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)      340 2024-01-25 08:44:04.000000 tksheet-7.2.2/tksheet/types.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     3452 2024-05-20 09:29:16.000000 tksheet-7.2.2/tksheet/vars.py
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-27 15:51:37.406540 tksheet-7.2.2/tksheet.egg-info/
+-rw-r--r--   0 rg        (1000) rg        (1000)     6319 2024-05-27 15:51:37.000000 tksheet-7.2.2/tksheet.egg-info/PKG-INFO
+-rw-rw-r--   0 rg        (1000) rg        (1000)      481 2024-05-27 15:51:37.000000 tksheet-7.2.2/tksheet.egg-info/SOURCES.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        1 2024-05-27 15:51:37.000000 tksheet-7.2.2/tksheet.egg-info/dependency_links.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        8 2024-05-27 15:51:37.000000 tksheet-7.2.2/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-7.2.1/LICENSE.txt` & `tksheet-7.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.1/PKG-INFO` & `tksheet-7.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tkinter table / sheet widget
 Author-email: ragardner <github@ragardner.simplelogin.com>
 License: Copyright (c) 2019 ragardner and open source contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -36,22 +36,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# tksheet
+<p align="center" width="100%">
+    <img width="33%" src="https://github.com/ragardner/tksheet/assets/26602401/4124c3ce-cf62-4925-9158-c5bdf712765b"> 
+</p>
+
+# <div align="center">tksheet - python tkinter table widget</div>
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.8|3.9|3.10|3.11|3.12-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt)
 
 [![GitHub Release Date](https://img.shields.io/github/release-date-pre/ragardner/tksheet.svg)](https://github.com/ragardner/tksheet/releases) [![Downloads](https://img.shields.io/pypi/dm/tksheet.svg)](https://pypi.org/project/tksheet/)
 
-### **A python tkinter table widget**
-
 |    **Help**       |                                                                  |
 |-------------------|------------------------------------------------------------------|
 | Versions 6.x.x -> | [Documentation Wiki](https://github.com/ragardner/tksheet/wiki/Version-6) | |
 | Versions 7.x.x -> | [Documentation Wiki](https://github.com/ragardner/tksheet/wiki/Version-7) | |
 | [Changelog](https://github.com/ragardner/tksheet/blob/master/docs/CHANGELOG.md) | |
 | [Questions](https://github.com/ragardner/tksheet/wiki/Version-7#asking-questions) | |
 | [Issues](https://github.com/ragardner/tksheet/wiki/Version-7#issues) | |
```

### Comparing `tksheet-7.2.1/README.md` & `tksheet-7.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# tksheet
+<p align="center" width="100%">
+    <img width="33%" src="https://github.com/ragardner/tksheet/assets/26602401/4124c3ce-cf62-4925-9158-c5bdf712765b"> 
+</p>
+
+# <div align="center">tksheet - python tkinter table widget</div>
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.8|3.9|3.10|3.11|3.12-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt)
 
 [![GitHub Release Date](https://img.shields.io/github/release-date-pre/ragardner/tksheet.svg)](https://github.com/ragardner/tksheet/releases) [![Downloads](https://img.shields.io/pypi/dm/tksheet.svg)](https://pypi.org/project/tksheet/)
 
-### **A python tkinter table widget**
-
 |    **Help**       |                                                                  |
 |-------------------|------------------------------------------------------------------|
 | Versions 6.x.x -> | [Documentation Wiki](https://github.com/ragardner/tksheet/wiki/Version-6) | |
 | Versions 7.x.x -> | [Documentation Wiki](https://github.com/ragardner/tksheet/wiki/Version-7) | |
 | [Changelog](https://github.com/ragardner/tksheet/blob/master/docs/CHANGELOG.md) | |
 | [Questions](https://github.com/ragardner/tksheet/wiki/Version-7#asking-questions) | |
 | [Issues](https://github.com/ragardner/tksheet/wiki/Version-7#issues) | |
```

### Comparing `tksheet-7.2.1/pyproject.toml` & `tksheet-7.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tksheet"
 description = "Tkinter table / sheet widget"
 readme = "README.md"
-version = "7.2.1"
+version = "7.2.2"
 authors = [{ name = "ragardner", email = "github@ragardner.simplelogin.com" }]
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["tkinter", "table", "widget", "sheet", "grid", "tk"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `tksheet-7.2.1/tksheet/__init__.py` & `tksheet-7.2.2/tksheet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ruff: noqa: F401
 
 """
 tksheet - A Python tkinter table widget
 """
 
-__version__ = "7.2.1"
+__version__ = "7.2.2"
 
 from .colors import (
     color_map,
 )
 from .column_headers import ColumnHeaders
 from .formatters import (
     Formatter,
```

### Comparing `tksheet-7.2.1/tksheet/colors.py` & `tksheet-7.2.2/tksheet/colors.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.1/tksheet/column_headers.py` & `tksheet-7.2.2/tksheet/column_headers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from __future__ import annotations
 
 import tkinter as tk
 from collections import defaultdict
 from collections.abc import (
     Callable,
+    Hashable,
     Sequence,
 )
 from functools import (
     partial,
 )
 from itertools import (
     cycle,
     islice,
+    repeat,
 )
 from math import ceil, floor
+from operator import (
+    itemgetter,
+)
 from typing import Literal
 
 from .colors import (
     color_map,
 )
 from .formatters import is_bool_like, try_to_bool
 from .functions import (
@@ -130,15 +135,15 @@
     def event_generate(self, *args, **kwargs) -> None:
         for arg in args:
             if self.MT and arg in self.MT.event_linker:
                 self.MT.event_linker[arg]()
             else:
                 super().event_generate(*args, **kwargs)
 
-    def basic_bindings(self, enable: bool = True):
+    def basic_bindings(self, enable: bool = True) -> None:
         if enable:
             self.bind("<Motion>", self.mouse_motion)
             self.bind("<ButtonPress-1>", self.b1_press)
             self.bind("<B1-Motion>", self.b1_motion)
             self.bind("<ButtonRelease-1>", self.b1_release)
             self.bind("<Double-Button-1>", self.double_b1)
             self.bind(rc_binding, self.rc)
@@ -154,30 +159,34 @@
             self.unbind("<Double-Button-1>")
             self.unbind(rc_binding)
             self.unbind("<MouseWheel>")
             if USER_OS == "linux":
                 self.unbind("<Button-4>")
                 self.unbind("<Button-5>")
 
-    def mousewheel(self, event: object):
-        maxlines = 0
+    def mousewheel(self, event: object) -> None:
         if isinstance(self.MT._headers, int):
-            if len(self.MT.data) > self.MT._headers:
-                maxlines = max(
+            maxlines = max(
+                (
                     len(
                         self.MT.get_valid_cell_data_as_str(self.MT._headers, datacn, get_displayed=True)
                         .rstrip()
                         .split("\n")
                     )
                     for datacn in range(len(self.MT.data[self.MT._headers]))
-                )
+                ),
+                default=0,
+            )
         elif isinstance(self.MT._headers, (list, tuple)):
             maxlines = max(
-                len(e.rstrip().split("\n")) if isinstance(e, str) else len(f"{e}".rstrip().split("\n"))
-                for e in self.MT._headers
+                (
+                    len(e.rstrip().split("\n")) if isinstance(e, str) else len(f"{e}".rstrip().split("\n"))
+                    for e in self.MT._headers
+                ),
+                default=0,
             )
         if maxlines == 1:
             maxlines = 0
         if self.lines_start_at > maxlines:
             self.lines_start_at = maxlines
         if (event.delta < 0 or event.num == 5) and self.lines_start_at < maxlines:
             self.lines_start_at += 1
@@ -386,15 +395,15 @@
                     if self.MT.current_cursor != "hand2":
                         self.config(cursor="hand2")
                         self.MT.current_cursor = "hand2"
             if not mouse_over_resize and not mouse_over_selected:
                 self.MT.reset_mouse_motion_creations()
         try_binding(self.extra_motion_func, event)
 
-    def double_b1(self, event: object):
+    def double_b1(self, event: object) -> None:
         self.mouseclick_outside_editor_or_dropdown_all_canvases(inside=True)
         self.focus_set()
         if (
             self.double_click_resizing_enabled
             and self.width_resizing_enabled
             and self.rsz_w is not None
             and not self.currently_resizing_width
@@ -426,15 +435,15 @@
                     or self.edit_cell_enabled
                 ):
                     self.open_cell(event)
         self.rsz_w = None
         self.mouse_motion(event)
         try_binding(self.extra_double_b1_func, event)
 
-    def b1_press(self, event: object):
+    def b1_press(self, event: object) -> None:
         self.MT.unbind("<MouseWheel>")
         self.focus_set()
         self.closed_dropdown = self.mouseclick_outside_editor_or_dropdown_all_canvases(inside=True)
         x = self.canvasx(event.x)
         y = self.canvasy(event.y)
         c = self.MT.identify_col(x=event.x)
         self.b1_pressed_loc = c
@@ -491,15 +500,15 @@
                     if self.MT.single_selection_enabled:
                         self.being_drawn_item = True
                         self.being_drawn_item = self.select_col(c, redraw=True)
                     elif self.MT.toggle_selection_enabled:
                         self.toggle_select_col(c, redraw=True)
         try_binding(self.extra_b1_press_func, event)
 
-    def b1_motion(self, event: object):
+    def b1_motion(self, event: object) -> None:
         x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
         if self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
             x = self.canvasx(event.x)
             size = x - self.MT.col_positions[self.rsz_w - 1]
             if size >= self.MT.min_column_width and size < self.MT.max_column_width:
                 self.hide_resize_and_ctrl_lines(ctrl_lines=False)
                 line2x = self.MT.col_positions[self.rsz_w - 1]
@@ -589,21 +598,21 @@
                         self.PAR.emit_event("<<SheetSelect>>", data=sel_event)
                 if self.scroll_if_event_offscreen(event):
                     need_redraw = True
             if need_redraw:
                 self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=False)
         try_binding(self.extra_b1_motion_func, event)
 
-    def get_b1_motion_box(self, start_col, end_col):
+    def get_b1_motion_box(self, start_col: int, end_col: int) -> tuple[int, int, int, int, Literal["columns"]]:
         if end_col >= start_col:
             return 0, start_col, len(self.MT.row_positions) - 1, end_col + 1, "columns"
         elif end_col < start_col:
             return 0, end_col, len(self.MT.row_positions) - 1, start_col + 1, "columns"
 
-    def ctrl_b1_motion(self, event: object):
+    def ctrl_b1_motion(self, event: object) -> None:
         x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
         if (
             self.drag_and_drop_enabled
             and self.col_selection_enabled
             and self.MT.anything_selected(exclude_cells=True, exclude_rows=True)
             and self.rsz_h is None
             and self.rsz_w is None
@@ -649,15 +658,15 @@
                 if self.scroll_if_event_offscreen(event):
                     need_redraw = True
             if need_redraw:
                 self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=False)
         elif not self.MT.ctrl_select_enabled:
             self.b1_motion(event)
 
-    def drag_and_drop_motion(self, event: object):
+    def drag_and_drop_motion(self, event: object) -> float:
         x = event.x
         wend = self.winfo_width()
         xcheck = self.xview()
         if x >= wend - 0 and len(xcheck) > 1 and xcheck[1] < 1:
             if x >= wend + 15:
                 self.MT.xview_scroll(2, "units")
                 self.xview_scroll(2, "units")
@@ -993,15 +1002,15 @@
 
     def hide_box(self, item: int) -> None:
         if isinstance(item, int):
             self.disp_boxes.discard(item)
             self.hidd_boxes.add(item)
             self.itemconfig(item, state="hidden")
 
-    def get_cell_dimensions(self, datacn):
+    def get_cell_dimensions(self, datacn: int) -> tuple[int, int]:
         txt = self.get_valid_cell_data_as_str(datacn, fix=False)
         if txt:
             self.MT.txt_measure_canvas.itemconfig(
                 self.MT.txt_measure_canvas_text, text=txt, font=self.PAR.ops.header_font
             )
             b = self.MT.txt_measure_canvas.bbox(self.MT.txt_measure_canvas_text)
             w = b[2] - b[0] + 7
@@ -1011,179 +1020,179 @@
             h = self.MT.min_header_height
         if datacn in self.cell_options and (
             self.get_cell_kwargs(datacn, key="dropdown") or self.get_cell_kwargs(datacn, key="checkbox")
         ):
             return w + self.MT.header_txt_height, h
         return w, h
 
-    def set_height_of_header_to_text(self, text=None, only_increase=False):
-        if (
-            text is None
-            and not self.MT._headers
-            and isinstance(self.MT._headers, list)
-            or isinstance(self.MT._headers, int)
-            and self.MT._headers >= len(self.MT.data)
+    def set_height_of_header_to_text(
+        self,
+        text: None | str = None,
+        only_if_too_small: bool = False,
+    ) -> int:
+        h = self.MT.min_header_height
+        if (text is None and not self.MT._headers and isinstance(self.MT._headers, list)) or (
+            isinstance(self.MT._headers, int) and self.MT._headers >= len(self.MT.data)
         ):
-            return
+            return h
+        self.fix_header()
         qconf = self.MT.txt_measure_canvas.itemconfig
         qbbox = self.MT.txt_measure_canvas.bbox
         qtxtm = self.MT.txt_measure_canvas_text
         qfont = self.PAR.ops.header_font
-        new_height = self.MT.min_header_height
         default_header_height = self.MT.get_default_header_height()
-        self.fix_header()
-        if text is not None:
-            if text:
-                qconf(qtxtm, text=text, font=qfont)
-                b = qbbox(qtxtm)
-                if (h := b[3] - b[1] + 5) > new_height:
-                    new_height = h
-        else:
+        if text is not None and text:
+            qconf(qtxtm, text=text, font=qfont)
+            b = qbbox(qtxtm)
+            if (th := b[3] - b[1] + 5) > h:
+                h = th
+        elif text is None:
             if self.MT.all_columns_displayed:
                 if isinstance(self.MT._headers, list):
                     iterable = range(len(self.MT._headers))
                 else:
                     iterable = range(len(self.MT.data[self.MT._headers]))
             else:
                 iterable = self.MT.displayed_columns
-            if isinstance(self.MT._headers, list):
-                for datacn in iterable:
-                    w_, h = self.get_cell_dimensions(datacn)
-                    if h < self.MT.min_header_height:
-                        h = int(self.MT.min_header_height)
-                    elif h > self.MT.max_header_height:
-                        h = int(self.MT.max_header_height)
-                    if h > new_height:
-                        new_height = h
+            if (
+                isinstance(self.MT._headers, list)
+                and (th := max(map(itemgetter(0), map(self.get_cell_dimensions, iterable)), default=h)) > h
+            ):
+                h = th
             elif isinstance(self.MT._headers, int):
                 datarn = self.MT._headers
                 for datacn in iterable:
-                    txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True)
-                    if txt:
+                    if txt := self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True):
                         qconf(qtxtm, text=txt, font=qfont)
                         b = qbbox(qtxtm)
-                        h = b[3] - b[1] + 5
+                        th = b[3] - b[1] + 5
                     else:
-                        h = default_header_height
-                    if h < self.MT.min_header_height:
-                        h = int(self.MT.min_header_height)
-                    elif h > self.MT.max_header_height:
-                        h = int(self.MT.max_header_height)
-                    if h > new_height:
-                        new_height = h
+                        th = default_header_height
+                    if th > h:
+                        h = th
         space_bot = self.MT.get_space_bot(0)
-        if new_height > space_bot and space_bot > self.MT.min_header_height:
-            new_height = space_bot
-        if not only_increase or (only_increase and new_height > self.current_height):
-            self.set_height(new_height, set_TL=True)
+        if h > space_bot and space_bot > self.MT.min_header_height:
+            h = space_bot
+        if h < self.MT.min_header_height:
+            h = int(self.MT.min_header_height)
+        elif h > self.MT.max_header_height:
+            h = int(self.MT.max_header_height)
+        if not only_if_too_small or (only_if_too_small and h > self.current_height):
+            self.set_height(h, set_TL=True)
             self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
-        return new_height
+        return h
 
-    def set_col_width(
+    def get_col_text_width(
         self,
-        col,
-        width=None,
-        only_set_if_too_small=False,
-        displayed_only=False,
-        recreate=True,
-        return_new_width=False,
-    ):
-        if col < 0:
-            return
-        qconf = self.MT.txt_measure_canvas.itemconfig
-        qbbox = self.MT.txt_measure_canvas.bbox
-        qtxtm = self.MT.txt_measure_canvas_text
-        qtxth = self.MT.table_txt_height
-        qfont = self.PAR.ops.table_font
+        col: int,
+        visible_only: bool = False,
+        only_if_too_small: bool = False,
+    ) -> int:
         self.fix_header()
-        if width is None:
-            w = self.MT.min_column_width
-            hw = self.MT.min_column_width
+        w = self.MT.min_column_width
+        datacn = col if self.MT.all_columns_displayed else self.MT.displayed_columns[col]
+        # header
+        hw, hh_ = self.get_cell_dimensions(datacn)
+        # table
+        if self.MT.data:
             if self.MT.all_rows_displayed:
-                if displayed_only:
-                    x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
-                    start_row, end_row = self.MT.get_visible_rows(y1, y2)
+                if visible_only:
+                    iterable = range(*self.MT.visible_text_rows)
                 else:
-                    start_row, end_row = 0, len(self.MT.data)
-                iterable = range(start_row, end_row)
+                    iterable = range(0, len(self.MT.data))
             else:
-                if displayed_only:
-                    x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
-                    start_row, end_row = self.MT.get_visible_rows(y1, y2)
+                if visible_only:
+                    start_row, end_row = self.MT.visible_text_rows
                 else:
                     start_row, end_row = 0, len(self.MT.displayed_rows)
                 iterable = self.MT.displayed_rows[start_row:end_row]
-            datacn = col if self.MT.all_columns_displayed else self.MT.displayed_columns[col]
-            # header
-            hw, hh_ = self.get_cell_dimensions(datacn)
-            # table
-            if self.MT.data:
-                for datarn in iterable:
-                    txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True)
-                    if txt:
-                        qconf(qtxtm, text=txt, font=qfont)
-                        b = qbbox(qtxtm)
-                        if self.MT.get_cell_kwargs(datarn, datacn, key="dropdown") or self.MT.get_cell_kwargs(
-                            datarn, datacn, key="checkbox"
-                        ):
-                            tw = b[2] - b[0] + qtxth + 7
-                        else:
-                            tw = b[2] - b[0] + 7
-                        if tw > w:
-                            w = tw
-            if w > hw:
-                new_width = w
-            else:
-                new_width = hw
-        else:
-            new_width = int(width)
-        if new_width <= self.MT.min_column_width:
-            new_width = int(self.MT.min_column_width)
-        elif new_width > self.MT.max_column_width:
-            new_width = int(self.MT.max_column_width)
-        if only_set_if_too_small:
-            if new_width <= self.MT.col_positions[col + 1] - self.MT.col_positions[col]:
-                return self.MT.col_positions[col + 1] - self.MT.col_positions[col]
-        if not return_new_width:
-            new_col_pos = self.MT.col_positions[col] + new_width
-            increment = new_col_pos - self.MT.col_positions[col + 1]
-            self.MT.col_positions[col + 2 :] = [
-                e + increment for e in islice(self.MT.col_positions, col + 2, len(self.MT.col_positions))
-            ]
-            self.MT.col_positions[col + 1] = new_col_pos
-            if recreate:
-                self.MT.recreate_all_selection_boxes()
-        return new_width
+            qconf = self.MT.txt_measure_canvas.itemconfig
+            qbbox = self.MT.txt_measure_canvas.bbox
+            qtxtm = self.MT.txt_measure_canvas_text
+            qtxth = self.MT.table_txt_height
+            qfont = self.PAR.ops.table_font
+            for datarn in iterable:
+                if txt := self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True):
+                    qconf(qtxtm, text=txt, font=qfont)
+                    b = qbbox(qtxtm)
+                    if (
+                        self.MT.get_cell_kwargs(datarn, datacn, key="dropdown")
+                        or self.MT.get_cell_kwargs(datarn, datacn, key="checkbox")
+                    ) and (tw := b[2] - b[0] + qtxth + 7) > w:
+                        w = tw
+                    elif (tw := b[2] - b[0] + 7) > w:
+                        w = tw
+        if hw > w:
+            w = hw
+        if only_if_too_small and w < self.MT.col_positions[col + 1] - self.MT.col_positions[col]:
+            w = self.MT.col_positions[col + 1] - self.MT.col_positions[col]
+        if w <= self.MT.min_column_width:
+            w = int(self.MT.min_column_width)
+        elif w > self.MT.max_column_width:
+            w = int(self.MT.max_column_width)
+        return w
 
-    def set_width_of_all_cols(self, width=None, only_set_if_too_small=False, recreate=True):
+    def set_col_width(
+        self,
+        col: int,
+        width: None | int = None,
+        only_if_too_small: bool = False,
+        visible_only: bool = False,
+        recreate: bool = True,
+    ) -> int:
+        if width is None:
+            width = self.get_col_text_width(col=col, visible_only=visible_only)
+        if width <= self.MT.min_column_width:
+            width = int(self.MT.min_column_width)
+        elif width > self.MT.max_column_width:
+            width = int(self.MT.max_column_width)
+        if only_if_too_small and width <= self.MT.col_positions[col + 1] - self.MT.col_positions[col]:
+            return self.MT.col_positions[col + 1] - self.MT.col_positions[col]
+        new_col_pos = self.MT.col_positions[col] + width
+        increment = new_col_pos - self.MT.col_positions[col + 1]
+        self.MT.col_positions[col + 2 :] = [
+            e + increment for e in islice(self.MT.col_positions, col + 2, len(self.MT.col_positions))
+        ]
+        self.MT.col_positions[col + 1] = new_col_pos
+        if recreate:
+            self.MT.recreate_all_selection_boxes()
+        return width
+
+    def set_width_of_all_cols(
+        self,
+        width: None | int = None,
+        only_if_too_small: bool = False,
+        recreate: bool = True,
+    ) -> None:
         if width is None:
             if self.MT.all_columns_displayed:
                 iterable = range(self.MT.total_data_cols())
             else:
                 iterable = range(len(self.MT.displayed_columns))
             self.MT.set_col_positions(
-                itr=(
-                    self.set_col_width(
-                        cn,
-                        only_set_if_too_small=only_set_if_too_small,
-                        recreate=False,
-                        return_new_width=True,
-                    )
-                    for cn in iterable
-                )
+                itr=(self.get_col_text_width(cn, only_if_too_small=only_if_too_small) for cn in iterable)
             )
         elif width is not None:
             if self.MT.all_columns_displayed:
-                self.MT.set_col_positions(itr=(width for cn in range(self.MT.total_data_cols())))
+                self.MT.set_col_positions(itr=repeat(width, self.MT.total_data_cols()))
             else:
-                self.MT.set_col_positions(itr=(width for cn in range(len(self.MT.displayed_columns))))
+                self.MT.set_col_positions(itr=repeat(width, len(self.MT.displayed_columns)))
         if recreate:
             self.MT.recreate_all_selection_boxes()
 
-    def redraw_highlight_get_text_fg(self, fc, sc, c, c_2, c_3, selections, datacn):
+    def redraw_highlight_get_text_fg(
+        self,
+        fc: float,
+        sc: float,
+        c: int,
+        c_2: str,
+        c_3: str,
+        selections: dict,
+        datacn: int,
+    ) -> tuple[str, bool]:
         redrawn = False
         kwargs = self.get_cell_kwargs(datacn, key="highlight")
         if kwargs:
             if kwargs[0] is not None:
                 c_1 = kwargs[0] if kwargs[0].startswith("#") else color_map[kwargs[0]]
             if "columns" in selections and c in selections["columns"]:
                 tf = (
@@ -1232,53 +1241,68 @@
                 tf = self.PAR.ops.header_selected_columns_fg
             elif "cells" in selections and c in selections["cells"]:
                 tf = self.PAR.ops.header_selected_cells_fg
             else:
                 tf = self.PAR.ops.header_fg
         return tf, redrawn
 
-    def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag):
+    def redraw_highlight(
+        self,
+        x1: float,
+        y1: float,
+        x2: float,
+        y2: float,
+        fill: str,
+        outline: str,
+        tag: str | tuple[str],
+    ) -> bool:
         coords = (x1, y1, x2, y2)
         if self.hidd_high:
             iid, showing = self.hidd_high.popitem()
             self.coords(iid, coords)
             if showing:
                 self.itemconfig(iid, fill=fill, outline=outline)
             else:
                 self.itemconfig(iid, fill=fill, outline=outline, tag=tag, state="normal")
         else:
             iid = self.create_rectangle(coords, fill=fill, outline=outline, tag=tag)
         self.disp_high[iid] = True
         return True
 
-    def redraw_gridline(self, points, fill, width, tag):
+    def redraw_gridline(
+        self,
+        points: Sequence[float],
+        fill: str,
+        width: int,
+        tag: str | tuple[str],
+    ) -> None:
         if self.hidd_grid:
             t, sh = self.hidd_grid.popitem()
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill=fill, width=width, tag=tag)
             else:
                 self.itemconfig(t, fill=fill, width=width, tag=tag, state="normal")
             self.disp_grid[t] = True
         else:
             self.disp_grid[self.create_line(points, fill=fill, width=width, tag=tag)] = True
 
     def redraw_dropdown(
         self,
-        x1,
-        y1,
-        x2,
-        y2,
-        fill,
-        outline,
-        tag,
-        draw_outline=True,
-        draw_arrow=True,
-        dd_is_open=False,
-    ):
+        x1: float,
+        y1: float,
+        x2: float,
+        y2: float,
+        fill: str,
+        outline: str,
+        tag: str | tuple[str],
+        draw_outline: bool = True,
+        draw_arrow: bool = True,
+        dd_is_open: bool = False,
+    ) -> None:
         if draw_outline and self.PAR.ops.show_dropdown_borders:
             self.redraw_highlight(x1 + 1, y1 + 1, x2, y2, fill="", outline=self.PAR.ops.header_fg, tag=tag)
         if draw_arrow:
             mod = (self.MT.header_txt_height - 1) if self.MT.header_txt_height % 2 else self.MT.header_txt_height
             half_mod = mod / 2
             qtr_mod = mod / 4
             mid_y = (
@@ -1314,15 +1338,25 @@
                 t = self.create_polygon(
                     points,
                     fill=fill,
                     tag=tag,
                 )
             self.disp_dropdown[t] = True
 
-    def redraw_checkbox(self, x1, y1, x2, y2, fill, outline, tag, draw_check=False):
+    def redraw_checkbox(
+        self,
+        x1: float,
+        y1: float,
+        x2: float,
+        y2: float,
+        fill: str,
+        outline: str,
+        tag: str | tuple[str],
+        draw_check: bool = False,
+    ) -> None:
         points = rounded_box_coords(x1, y1, x2, y2)
         if self.hidd_checkbox:
             t, sh = self.hidd_checkbox.popitem()
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill=outline, outline=fill)
             else:
@@ -1358,26 +1392,28 @@
                 last_col_line_pos + self.PAR.ops.empty_horizontal + 2,
                 self.current_height,
             )
         )
 
     def redraw_grid_and_text(
         self,
-        last_col_line_pos,
-        scrollpos_left,
-        x_stop,
-        start_col,
-        end_col,
-        scrollpos_right,
-        col_pos_exists,
-    ):
+        last_col_line_pos: float,
+        scrollpos_left: float,
+        x_stop: float,
+        grid_start_col: int,
+        grid_end_col: int,
+        text_start_col: int,
+        text_end_col: int,
+        scrollpos_right: float,
+        col_pos_exists: bool,
+    ) -> bool:
         try:
             self.configure_scrollregion(last_col_line_pos=last_col_line_pos)
         except Exception:
-            return
+            return False
         self.hidd_text.update(self.disp_text)
         self.disp_text = {}
         self.hidd_high.update(self.disp_high)
         self.disp_high = {}
         self.hidd_grid.update(self.disp_grid)
         self.disp_grid = {}
         self.hidd_dropdown.update(self.disp_dropdown)
@@ -1387,26 +1423,26 @@
         self.visible_col_dividers = {}
         self.col_height_resize_bbox = (
             scrollpos_left,
             self.current_height - 2,
             x_stop,
             self.current_height,
         )
-        draw_x = self.MT.col_positions[start_col]
+        draw_x = self.MT.col_positions[grid_start_col]
         yend = self.current_height - 5
         if (self.PAR.ops.show_vertical_grid or self.width_resizing_enabled) and col_pos_exists:
             points = [
                 x_stop - 1,
                 self.current_height - 1,
                 scrollpos_left - 1,
                 self.current_height - 1,
                 scrollpos_left - 1,
                 -1,
             ]
-            for c in range(start_col + 1, end_col):
+            for c in range(grid_start_col, grid_end_col):
                 draw_x = self.MT.col_positions[c]
                 if self.width_resizing_enabled:
                     self.visible_col_dividers[c] = (draw_x - 2, 1, draw_x + 2, yend)
                 points.extend(
                     (
                         draw_x,
                         -1,
@@ -1427,17 +1463,17 @@
         )
         c_3 = (
             self.PAR.ops.header_selected_columns_bg
             if self.PAR.ops.header_selected_columns_bg.startswith("#")
             else color_map[self.PAR.ops.header_selected_columns_bg]
         )
         font = self.PAR.ops.header_font
-        selections = self.get_redraw_selections(start_col, end_col)
+        selections = self.get_redraw_selections(text_start_col, grid_end_col)
         dd_coords = self.dropdown.get_coords()
-        for c in range(start_col, end_col - 1):
+        for c in range(text_start_col, text_end_col):
             draw_y = self.MT.header_first_ln_ins
             cleftgridln = self.MT.col_positions[c]
             crightgridln = self.MT.col_positions[c + 1]
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             fill, dd_drawn = self.redraw_highlight_get_text_fg(
                 cleftgridln, crightgridln, c, c_2, c_3, selections, datacn
             )
@@ -1625,15 +1661,15 @@
         for item, box in self.MT.get_selection_items():
             r1, c1, r2, c2 = box.coords
             for c in range(startc, endc):
                 if c1 <= c and c2 > c:
                     d[box.type_ if box.type_ != "rows" else "cells"].add(c)
         return d
 
-    def open_cell(self, event: object = None, ignore_existing_editor=False):
+    def open_cell(self, event: object = None, ignore_existing_editor: bool = False) -> None:
         if not self.MT.anything_selected() or (not ignore_existing_editor and self.text_editor.open):
             return
         if not self.MT.selected:
             return
         c = self.MT.selected.column
         datacn = self.MT.datacn(c)
         if self.get_cell_kwargs(datacn, key="readonly"):
@@ -1765,31 +1801,36 @@
             self.text_editor.tktext.focus_set()
             self.text_editor.window.scroll_to_bottom()
             self.text_editor.tktext.bind("<FocusOut>", self.close_text_editor)
         for key, func in self.MT.text_editor_user_bound_keys.items():
             self.text_editor.tktext.bind(key, func)
         return True
 
-    # displayed indexes                         #just here to receive text editor arg
-    def text_editor_has_wrapped(self, r=0, c=0, check_lines=None):
+    # displayed indexes
+    def text_editor_has_wrapped(
+        self,
+        r: int = 0,
+        c: int = 0,
+        check_lines: None = None,  # just here to receive text editor arg
+    ) -> None:
         if self.width_resizing_enabled:
             curr_width = self.text_editor.window.winfo_width()
             new_width = curr_width + (self.MT.header_txt_height * 2)
             if new_width != curr_width:
                 self.text_editor.window.config(width=new_width)
-                self.set_col_width_run_binding(c, width=new_width, only_set_if_too_small=False)
+                self.set_col_width_run_binding(c, width=new_width, only_if_too_small=False)
                 if self.dropdown.open and self.dropdown.get_coords() == c:
                     self.itemconfig(self.dropdown.canvas_id, width=new_width)
                     self.dropdown.window.update_idletasks()
                     self.dropdown.window._reselect()
                 self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=False, redraw_table=True)
                 self.coords(self.text_editor.canvas_id, self.MT.col_positions[c] + 1, 0)
 
     # displayed indexes
-    def text_editor_newline_binding(self, event: object = None, check_lines=True):
+    def text_editor_newline_binding(self, event: object = None, check_lines: bool = True) -> None:
         if not self.height_resizing_enabled:
             return
         curr_height = self.text_editor.window.winfo_height()
         if curr_height < self.MT.min_header_height:
             return
         if (
             not check_lines
@@ -1812,15 +1853,15 @@
                     self.coords(
                         self.dropdown.canvas_id,
                         self.MT.col_positions[c],
                         new_height - 1,
                     )
                     self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
 
-    def refresh_open_window_positions(self, zoom: Literal["in", "out"]):
+    def refresh_open_window_positions(self, zoom: Literal["in", "out"]) -> None:
         if self.text_editor.open:
             c = self.text_editor.column
             self.text_editor.window.config(
                 height=self.current_height,
                 width=self.MT.col_positions[c + 1] - self.MT.col_positions[c] + 1,
             )
             self.text_editor.tktext.config(font=self.PAR.ops.header_font)
@@ -1918,15 +1959,19 @@
             try_binding(self.extra_end_edit_cell_func, event_data)
         self.MT.recreate_all_selection_boxes()
         self.hide_text_editor_and_dropdown()
         if event.keysym != "FocusOut":
             self.focus_set()
         return "break"
 
-    def get_dropdown_height_anchor(self, c, text_editor_h=None):
+    def get_dropdown_height_anchor(
+        self,
+        c: int,
+        text_editor_h: None | int = None,
+    ) -> tuple[int, Literal["nw"]]:
         win_h = 5
         datacn = self.MT.datacn(c)
         for i, v in enumerate(self.get_cell_kwargs(datacn, key="dropdown")["values"]):
             v_numlines = len(v.split("\n") if isinstance(v, str) else f"{v}".split("\n"))
             if v_numlines > 1:
                 win_h += (
                     self.MT.header_first_ln_ins + (v_numlines * self.MT.header_xtra_lines_increment) + 5
@@ -1953,15 +1998,15 @@
         event: dict,
         modified_func: Callable | None,
     ) -> None:
         if modified_func:
             modified_func(event)
         dd_window.search_and_see(event)
 
-    def open_dropdown_window(self, c, event: object = None):
+    def open_dropdown_window(self, c: int, event: object = None) -> None:
         self.hide_text_editor("Escape")
         kwargs = self.get_cell_kwargs(self.MT.datacn(c), key="dropdown")
         if kwargs["state"] == "normal":
             if not self.open_text_editor(event=event, c=c, dropdown=True):
                 return
         win_h, anchor = self.get_dropdown_height_anchor(c)
         win_w = self.MT.col_positions[c + 1] - self.MT.col_positions[c] + 1
@@ -2026,15 +2071,20 @@
             self.update_idletasks()
             self.dropdown.window.focus_set()
             redraw = True
         self.dropdown.open = True
         if redraw:
             self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=False, redraw_table=False)
 
-    def close_dropdown_window(self, c=None, selection=None, redraw=True):
+    def close_dropdown_window(
+        self,
+        c: None | int = None,
+        selection: object = None,
+        redraw: bool = True,
+    ) -> None:
         if c is not None and selection is not None:
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             kwargs = self.get_cell_kwargs(datacn, key="dropdown")
             pre_edit_value = self.get_cell_data(datacn)
             edited = False
             event_data = event_dict(
                 name="end_edit_header",
@@ -2064,50 +2114,50 @@
 
     def hide_text_editor_and_dropdown(self, redraw: bool = True) -> None:
         self.hide_text_editor("Escape")
         self.hide_dropdown_window()
         if redraw:
             self.MT.refresh()
 
-    def mouseclick_outside_editor_or_dropdown(self, inside: bool = False):
+    def mouseclick_outside_editor_or_dropdown(self, inside: bool = False) -> int | None:
         closed_dd_coords = self.dropdown.get_coords()
         if self.text_editor.open:
             self.close_text_editor(new_tk_event("ButtonPress-1"))
         if closed_dd_coords is not None:
             self.hide_dropdown_window()
             if inside:
                 self.MT.main_table_redraw_grid_and_text(
                     redraw_header=True,
                     redraw_row_index=False,
                     redraw_table=False,
                 )
         return closed_dd_coords
 
-    def mouseclick_outside_editor_or_dropdown_all_canvases(self, inside: bool = False):
+    def mouseclick_outside_editor_or_dropdown_all_canvases(self, inside: bool = False) -> int | None:
         self.RI.mouseclick_outside_editor_or_dropdown()
         self.MT.mouseclick_outside_editor_or_dropdown()
         return self.mouseclick_outside_editor_or_dropdown(inside)
 
     def hide_dropdown_window(self) -> None:
         if self.dropdown.open:
             self.dropdown.window.unbind("<FocusOut>")
             self.itemconfig(self.dropdown.canvas_id, state="hidden")
             self.dropdown.open = False
 
     # internal event use
     def set_cell_data_undo(
         self,
-        c=0,
-        datacn=None,
-        value="",
-        cell_resize=True,
-        undo=True,
-        redraw=True,
-        check_input_valid=True,
-    ):
+        c: int = 0,
+        datacn: int | None = None,
+        value: object = "",
+        cell_resize: bool = True,
+        undo: bool = True,
+        redraw: bool = True,
+        check_input_valid: bool = True,
+    ) -> bool:
         if datacn is None:
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
         event_data = event_dict(
             name="edit_header",
             sheet=self.PAR.name,
             widget=self,
             cells_header={datacn: self.get_cell_data(datacn)},
@@ -2130,15 +2180,15 @@
             self.set_col_width_run_binding(c)
         if redraw:
             self.MT.refresh()
         if edited:
             self.MT.sheet_modified(event_data)
         return edited
 
-    def set_cell_data(self, datacn=None, value=""):
+    def set_cell_data(self, datacn: int | None = None, value: object = "") -> None:
         if isinstance(self.MT._headers, int):
             self.MT.set_cell_data(datarn=self.MT._headers, datacn=datacn, value=value)
         else:
             self.fix_header(datacn)
             if self.get_cell_kwargs(datacn, key="checkbox"):
                 self.MT._headers[datacn] = try_to_bool(value)
             else:
@@ -2152,42 +2202,42 @@
         if self.cell_equal_to(datacn, value):
             return False
         kwargs = self.get_cell_kwargs(datacn, key="dropdown")
         if kwargs and kwargs["validate_input"] and value not in kwargs["values"]:
             return False
         return True
 
-    def cell_equal_to(self, datacn, value):
+    def cell_equal_to(self, datacn: int, value: object) -> bool:
         self.fix_header(datacn)
         if isinstance(self.MT._headers, list):
             return self.MT._headers[datacn] == value
         elif isinstance(self.MT._headers, int):
             return self.MT.cell_equal_to(self.MT._headers, datacn, value)
 
     def get_cell_data(
         self,
-        datacn,
-        get_displayed=False,
-        none_to_empty_str=False,
-        redirect_int=False,
-    ):
+        datacn: int,
+        get_displayed: bool = False,
+        none_to_empty_str: bool = False,
+        redirect_int: bool = False,
+    ) -> object:
         if get_displayed:
             return self.get_valid_cell_data_as_str(datacn, fix=False)
         if redirect_int and isinstance(self.MT._headers, int):  # internal use
             return self.MT.get_cell_data(self.MT._headers, datacn, none_to_empty_str=True)
         if (
             isinstance(self.MT._headers, int)
             or not self.MT._headers
             or datacn >= len(self.MT._headers)
             or (self.MT._headers[datacn] is None and none_to_empty_str)
         ):
             return ""
         return self.MT._headers[datacn]
 
-    def get_valid_cell_data_as_str(self, datacn, fix=True) -> str:
+    def get_valid_cell_data_as_str(self, datacn: int, fix: bool = True) -> str:
         kwargs = self.get_cell_kwargs(datacn, key="dropdown")
         if kwargs:
             if kwargs["text"] is not None:
                 return f"{kwargs['text']}"
         else:
             kwargs = self.get_cell_kwargs(datacn, key="checkbox")
             if kwargs:
@@ -2200,58 +2250,54 @@
             value = "" if self.MT._headers[datacn] is None else f"{self.MT._headers[datacn]}"
         except Exception:
             value = ""
         if not value and self.PAR.ops.show_default_header_for_empty:
             value = get_n2a(datacn, self.default_header)
         return value
 
-    def get_value_for_empty_cell(self, datacn, c_ops=True):
+    def get_value_for_empty_cell(self, datacn: int, c_ops: bool = True) -> object:
         if self.get_cell_kwargs(datacn, key="checkbox", cell=c_ops):
             return False
         kwargs = self.get_cell_kwargs(datacn, key="dropdown", cell=c_ops)
         if kwargs and kwargs["validate_input"] and kwargs["values"]:
             return kwargs["values"][0]
         return ""
 
-    def get_empty_header_seq(self, end, start=0, c_ops=True):
+    def get_empty_header_seq(self, end: int, start: int = 0, c_ops: bool = True) -> list[object]:
         return [self.get_value_for_empty_cell(datacn, c_ops=c_ops) for datacn in range(start, end)]
 
-    def fix_header(self, datacn=None, fix_values=tuple()):
+    def fix_header(self, datacn: None | int = None) -> None:
         if isinstance(self.MT._headers, int):
             return
         if isinstance(self.MT._headers, float):
             self.MT._headers = int(self.MT._headers)
             return
         if not isinstance(self.MT._headers, list):
             try:
                 self.MT._headers = list(self.MT._headers)
             except Exception:
                 self.MT._headers = []
         if isinstance(datacn, int) and datacn >= len(self.MT._headers):
             self.MT._headers.extend(self.get_empty_header_seq(end=datacn + 1, start=len(self.MT._headers)))
-        if fix_values:
-            for cn, v in enumerate(islice(self.MT._headers, fix_values[0], fix_values[1])):
-                if not self.input_valid_for_cell(cn, v):
-                    self.MT._headers[cn] = self.get_value_for_empty_cell(cn)
 
     # displayed indexes
-    def set_col_width_run_binding(self, c, width=None, only_set_if_too_small=True):
+    def set_col_width_run_binding(self, c: int, width: int | None = None, only_if_too_small: bool = True) -> None:
         old_width = self.MT.col_positions[c + 1] - self.MT.col_positions[c]
-        new_width = self.set_col_width(c, width=width, only_set_if_too_small=only_set_if_too_small)
+        new_width = self.set_col_width(c, width=width, only_if_too_small=only_if_too_small)
         if self.column_width_resize_func is not None and old_width != new_width:
             self.column_width_resize_func(
                 event_dict(
                     name="resize",
                     sheet=self.PAR.name,
                     resized_columns={c: {"old_size": old_width, "new_size": new_width}},
                 )
             )
 
     # internal event use
-    def click_checkbox(self, c, datacn=None, undo=True, redraw=True):
+    def click_checkbox(self, c: int, datacn: int | None = None, undo: bool = True, redraw: bool = True) -> None:
         if datacn is None:
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
         kwargs = self.get_cell_kwargs(datacn, key="checkbox")
         if kwargs["state"] == "normal":
             pre_edit_value = self.get_cell_data(datacn)
             if isinstance(self.MT._headers, list):
                 value = not self.MT._headers[datacn] if isinstance(self.MT._headers[datacn], bool) else False
@@ -2278,11 +2324,11 @@
             )
             if kwargs["check_function"] is not None:
                 kwargs["check_function"](event_data)
             try_binding(self.extra_end_edit_cell_func, event_data)
         if redraw:
             self.MT.refresh()
 
-    def get_cell_kwargs(self, datacn, key="dropdown", cell=True):
+    def get_cell_kwargs(self, datacn: int, key: Hashable = "dropdown", cell: bool = True) -> dict:
         if cell and datacn in self.cell_options and key in self.cell_options[datacn]:
             return self.cell_options[datacn][key]
         return {}
```

### Comparing `tksheet-7.2.1/tksheet/formatters.py` & `tksheet-7.2.2/tksheet/formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.1/tksheet/functions.py` & `tksheet-7.2.2/tksheet/functions.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.1/tksheet/main_table.py` & `tksheet-7.2.2/tksheet/main_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -3638,15 +3638,15 @@
         else:
             w = self.min_column_width
             h = self.min_row_height
         if self.get_cell_kwargs(datarn, datacn, key="dropdown") or self.get_cell_kwargs(datarn, datacn, key="checkbox"):
             return w + self.table_txt_height, h
         return w, h
 
-    def set_cell_size_to_text(self, r, c, only_set_if_too_small=False, redraw: bool = True, run_binding=False):
+    def set_cell_size_to_text(self, r, c, only_if_too_small=False, redraw: bool = True, run_binding=False):
         min_column_width = int(self.min_column_width)
         min_rh = int(self.min_row_height)
         w = min_column_width
         h = min_rh
         datacn = self.datacn(c)
         datarn = self.datarn(r)
         tw, h = self.get_cell_dimensions(datarn, datacn)
@@ -3658,15 +3658,15 @@
             h = int(self.max_row_height)
         if w < min_column_width:
             w = int(min_column_width)
         elif w > self.max_column_width:
             w = int(self.max_column_width)
         cell_needs_resize_w = False
         cell_needs_resize_h = False
-        if only_set_if_too_small:
+        if only_if_too_small:
             if w > self.col_positions[c + 1] - self.col_positions[c]:
                 cell_needs_resize_w = True
             if h > self.row_positions[r + 1] - self.row_positions[r]:
                 cell_needs_resize_h = True
         else:
             if w != self.col_positions[c + 1] - self.col_positions[c]:
                 cell_needs_resize_w = True
@@ -3788,32 +3788,34 @@
         return self.row_positions, self.col_positions
 
     def set_col_positions(self, itr: Iterator[float]) -> None:
         self.col_positions = list(accumulate(chain([0], itr)))
 
     def reset_col_positions(self, ncols: int | None = None):
         colpos = self.PAR.ops.default_column_width
-        if self.all_columns_displayed:
-            self.set_col_positions(itr=(colpos for c in range(ncols if ncols is not None else self.total_data_cols())))
+        if isinstance(ncols, int):
+            self.set_col_positions(itr=repeat(colpos, ncols))
         else:
-            self.set_col_positions(
-                itr=(colpos for c in range(ncols if ncols is not None else len(self.displayed_columns)))
-            )
+            if self.all_columns_displayed:
+                self.set_col_positions(itr=repeat(colpos, self.total_data_cols()))
+            else:
+                self.set_col_positions(itr=repeat(colpos, len(self.displayed_columns)))
 
     def set_row_positions(self, itr: Iterator[float]) -> None:
         self.row_positions = list(accumulate(chain([0], itr)))
 
     def reset_row_positions(self, nrows: int | None = None):
         rowpos = self.get_default_row_height()
-        if self.all_rows_displayed:
-            self.set_row_positions(itr=(rowpos for r in range(nrows if nrows is not None else self.total_data_rows())))
+        if isinstance(nrows, int):
+            self.set_row_positions(itr=repeat(rowpos, nrows))
         else:
-            self.set_row_positions(
-                itr=(rowpos for r in range(nrows if nrows is not None else len(self.displayed_rows)))
-            )
+            if self.all_rows_displayed:
+                self.set_row_positions(itr=repeat(rowpos, self.total_data_rows()))
+            else:
+                self.set_row_positions(itr=repeat(rowpos, len(self.displayed_rows)))
 
     def del_col_position(self, idx: int, deselect_all: bool = False):
         if deselect_all:
             self.deselect("all", redraw=False)
         if idx == "end" or len(self.col_positions) <= idx + 1:
             del self.col_positions[-1]
         else:
@@ -4335,15 +4337,15 @@
                 self.data[rn].insert(cn, v)
         # if not hiding rows then we can extend row positions if necessary
         if add_row_positions and self.all_rows_displayed and maxrn + 1 > len(self.row_positions) - 1:
             default_row_height = self.get_default_row_height()
             self.set_row_positions(
                 itr=chain(
                     self.gen_row_heights(),
-                    (default_row_height for i in range(len(self.row_positions) - 1, maxrn + 1)),
+                    repeat(default_row_height, len(self.row_positions) - 1, maxrn + 1),
                 )
             )
         if isinstance(self._headers, list) and header:
             self._headers = insert_items(self._headers, header, self.CH.fix_header)
         if push_ops:
             self.adjust_options_post_add_columns(
                 cols=tuple(reversed(columns)),
@@ -4470,15 +4472,15 @@
         if isinstance(self._row_index, list) and index:
             self._row_index = insert_items(self._row_index, index, self.RI.fix_index)
         # if not hiding columns then we can extend col positions if necessary
         if add_col_positions and self.all_columns_displayed and maxcn + 1 > len(self.col_positions) - 1:
             self.set_col_positions(
                 itr=chain(
                     self.gen_column_widths(),
-                    (self.PAR.ops.default_column_width for i in range(len(self.col_positions) - 1, maxcn + 1)),
+                    repeat(self.PAR.ops.default_column_width, len(self.col_positions) - 1, maxcn + 1),
                 )
             )
         if push_ops:
             self.adjust_options_post_add_rows(
                 rows=tuple(reversed(rows)),
                 create_ops=create_ops,
             )
@@ -5011,27 +5013,29 @@
         return (
             self.canvasx(0),
             self.canvasy(0),
             self.canvasx(self.winfo_width()),
             self.canvasy(self.winfo_height()),
         )
 
-    def get_visible_rows(self, y1: int | float, y2: int | float) -> tuple[int, int]:
-        start_row = bisect_left(self.row_positions, y1)
-        end_row = bisect_right(self.row_positions, y2)
-        if not y2 >= self.row_positions[-1]:
-            end_row += 1
-        return start_row, end_row
-
-    def get_visible_columns(self, x1: int | float, x2: int | float) -> tuple[int, int]:
-        start_col = bisect_left(self.col_positions, x1)
-        end_col = bisect_right(self.col_positions, x2)
-        if not x2 >= self.col_positions[-1]:
-            end_col += 1
-        return start_col, end_col
+    @property
+    def visible_text_rows(self) -> tuple[int, int]:
+        start = bisect_left(self.row_positions, self.canvasy(0))
+        end = bisect_right(self.row_positions, self.canvasy(self.winfo_height()))
+        start = start - 1 if start else start
+        end = end - 1 if end == len(self.row_positions) else end
+        return start, end
+
+    @property
+    def visible_text_columns(self) -> tuple[int, int]:
+        start = bisect_left(self.col_positions, self.canvasx(0))
+        end = bisect_right(self.col_positions, self.canvasx(self.winfo_width()))
+        start = start - 1 if start else start
+        end = end - 1 if end == len(self.col_positions) else end
+        return start, end
 
     def redraw_highlight_get_text_fg(
         self,
         r: int,
         c: int,
         fc: int | float,
         fr: int | float,
@@ -5370,29 +5374,34 @@
         if setting_views or scrollregion != self.scrollregion:
             self.configure(scrollregion=scrollregion)
             self.scrollregion = scrollregion
             self.CH.configure_scrollregion(last_col_line_pos)
             self.RI.configure_scrollregion(last_row_line_pos)
             if setting_views:
                 return False
+        scrollpos_top = self.canvasy(0)
         scrollpos_bot = self.canvasy(can_height)
-        end_row = bisect_right(self.row_positions, scrollpos_bot)
-        if not scrollpos_bot >= self.row_positions[-1]:
-            end_row += 1
         scrollpos_left = self.canvasx(0)
-        scrollpos_top = self.canvasy(0)
         scrollpos_right = self.canvasx(can_width)
-        start_row = bisect_left(self.row_positions, scrollpos_top)
-        start_col = bisect_left(self.col_positions, scrollpos_left)
-        end_col = bisect_right(self.col_positions, scrollpos_right)
+
+        grid_start_row = bisect_left(self.row_positions, scrollpos_top)
+        grid_end_row = bisect_right(self.row_positions, scrollpos_bot)
+        grid_start_col = bisect_left(self.col_positions, scrollpos_left)
+        grid_end_col = bisect_right(self.col_positions, scrollpos_right)
+
+        text_start_row = grid_start_row - 1 if grid_start_row else grid_start_row
+        text_end_row = grid_end_row - 1 if grid_end_row == len(self.row_positions) else grid_end_row
+        text_start_col = grid_start_col - 1 if grid_start_col else grid_start_col
+        text_end_col = grid_end_col - 1 if grid_end_col == len(self.col_positions) else grid_end_col
+
         changed_w = False
         if self.PAR.ops.auto_resize_row_index and redraw_row_index and self.show_index:
             changed_w = self.RI.auto_set_index_width(
-                end_row=end_row - 1,
-                only_rows=[self.datarn(r) for r in range(start_row if not start_row else start_row - 1, end_row - 1)],
+                end_row=grid_end_row,
+                only_rows=[self.datarn(r) for r in range(text_start_row, text_end_row)],
             )
         if resized_cols or resized_rows or changed_w:
             self.recreate_all_selection_boxes()
             if changed_w:
                 self.update_idletasks()
                 self.RI.update_idletasks()
                 self.CH.update_idletasks()
@@ -5404,16 +5413,14 @@
         self.disp_high = {}
         self.hidd_grid.update(self.disp_grid)
         self.disp_grid = {}
         self.hidd_dropdown.update(self.disp_dropdown)
         self.disp_dropdown = {}
         self.hidd_checkbox.update(self.disp_checkbox)
         self.disp_checkbox = {}
-        if not scrollpos_right >= self.col_positions[-1]:
-            end_col += 1
         if last_col_line_pos > scrollpos_right:
             x_stop = scrollpos_right
         else:
             x_stop = last_col_line_pos
         if last_row_line_pos > scrollpos_bot:
             y_stop = scrollpos_bot
         else:
@@ -5435,15 +5442,15 @@
                             x_grid_stop,
                             self.row_positions[r],
                             self.canvasx(0) - 1,
                             self.row_positions[r],
                             self.canvasx(0) - 1,
                             self.row_positions[r + 1] if len(self.row_positions) - 1 > r else self.row_positions[r],
                         )
-                        for r in range(start_row - 1, end_row)
+                        for r in range(grid_start_row, grid_end_row)
                     ]
                 )
             )
             if points:
                 self.redraw_gridline(
                     points=points,
                     fill=self.PAR.ops.table_grid_fg,
@@ -5467,32 +5474,27 @@
                             self.col_positions[c],
                             y_grid_stop,
                             self.col_positions[c],
                             scrollpos_top - 1,
                             self.col_positions[c + 1] if len(self.col_positions) - 1 > c else self.col_positions[c],
                             scrollpos_top - 1,
                         )
-                        for c in range(start_col - 1, end_col)
+                        for c in range(grid_start_col, grid_end_col)
                     ]
                 )
             )
             if points:
                 self.redraw_gridline(
                     points=points,
                     fill=self.PAR.ops.table_grid_fg,
                     width=1,
                     tag="g",
                 )
-        if start_row > 0:
-            start_row -= 1
-        if start_col > 0:
-            start_col -= 1
-        end_row -= 1
         if redraw_table:
-            selections = self.get_redraw_selections(start_row, end_row, start_col, end_col)
+            selections = self.get_redraw_selections(text_start_row, grid_end_row, text_start_col, grid_end_col)
             c_2 = (
                 self.PAR.ops.table_selected_cells_bg
                 if self.PAR.ops.table_selected_cells_bg.startswith("#")
                 else color_map[self.PAR.ops.table_selected_cells_bg]
             )
             c_2_ = (int(c_2[1:3], 16), int(c_2[3:5], 16), int(c_2[5:], 16))
             c_3 = (
@@ -5503,18 +5505,18 @@
             c_3_ = (int(c_3[1:3], 16), int(c_3[3:5], 16), int(c_3[5:], 16))
             c_4 = (
                 self.PAR.ops.table_selected_rows_bg
                 if self.PAR.ops.table_selected_rows_bg.startswith("#")
                 else color_map[self.PAR.ops.table_selected_rows_bg]
             )
             c_4_ = (int(c_4[1:3], 16), int(c_4[3:5], 16), int(c_4[5:], 16))
-            rows_ = tuple(range(start_row, end_row))
+            rows_ = tuple(range(text_start_row, text_end_row))
             font = self.PAR.ops.table_font
             dd_coords = self.dropdown.get_coords()
-            for c in range(start_col, end_col - 1):
+            for c in range(text_start_col, text_end_col):
                 for r in rows_:
                     rtopgridln = self.row_positions[r]
                     rbotgridln = self.row_positions[r + 1]
                     if rbotgridln - rtopgridln < self.table_txt_height:
                         continue
                     cleftgridln = self.col_positions[c]
                     crightgridln = self.col_positions[c + 1]
@@ -5714,31 +5716,35 @@
                 for iid, box in self.selection_boxes.items():
                     if box.bd_iid:
                         self.tag_raise(box.bd_iid)
                 if self.selected:
                     self.tag_raise(self.selected.iid)
         if redraw_header and self.show_header:
             self.CH.redraw_grid_and_text(
-                last_col_line_pos,
-                scrollpos_left,
-                x_stop,
-                start_col,
-                end_col,
-                scrollpos_right,
-                col_pos_exists,
+                last_col_line_pos=last_col_line_pos,
+                scrollpos_left=scrollpos_left,
+                x_stop=x_stop,
+                grid_start_col=grid_start_col,
+                grid_end_col=grid_end_col,
+                text_start_col=text_start_col,
+                text_end_col=text_end_col,
+                scrollpos_right=scrollpos_right,
+                col_pos_exists=col_pos_exists,
             )
         if redraw_row_index and self.show_index:
             self.RI.redraw_grid_and_text(
-                last_row_line_pos,
-                scrollpos_top,
-                y_stop,
-                start_row,
-                end_row + 1,
-                scrollpos_bot,
-                row_pos_exists,
+                last_row_line_pos=last_row_line_pos,
+                scrollpos_top=scrollpos_top,
+                y_stop=y_stop,
+                grid_start_row=grid_start_row,
+                grid_end_row=grid_end_row,
+                text_start_row=text_start_row,
+                text_end_row=text_end_row,
+                scrollpos_bot=scrollpos_bot,
+                row_pos_exists=row_pos_exists,
             )
         event_data = {"sheetname": "", "header": redraw_header, "row_index": redraw_row_index, "table": redraw_table}
         self.PAR.emit_event("<<SheetRedrawn>>", data=event_data)
         return True
 
     def get_selection_items(
         self,
@@ -6485,15 +6491,15 @@
                 return False
             if text is None:
                 return False
             else:
                 text = text if isinstance(text, str) else f"{text}"
         text = "" if text is None else text
         if self.PAR.ops.cell_auto_resize_enabled:
-            self.set_cell_size_to_text(r, c, only_set_if_too_small=True, redraw=True, run_binding=True)
+            self.set_cell_size_to_text(r, c, only_if_too_small=True, redraw=True, run_binding=True)
         if self.text_editor.open and (r, c) == self.text_editor.coords:
             self.text_editor.window.set_text(self.text_editor.get() + "" if not isinstance(text, str) else text)
             return
         if self.text_editor.open:
             self.hide_text_editor()
         if not self.see(r=r, c=c, check_cell_visibility=True):
             self.refresh()
@@ -7102,15 +7108,15 @@
             selected=self.selected,
         )
         if not check_input_valid or self.input_valid_for_cell(datarn, datacn, value):
             if self.undo_enabled and undo:
                 self.undo_stack.append(pickled_event_dict(event_data))
             self.set_cell_data(datarn, datacn, value)
             if cell_resize and self.PAR.ops.cell_auto_resize_enabled:
-                self.set_cell_size_to_text(r, c, only_set_if_too_small=True, redraw=redraw, run_binding=True)
+                self.set_cell_size_to_text(r, c, only_if_too_small=True, redraw=redraw, run_binding=True)
             self.sheet_modified(event_data)
             return True
         return False
 
     def set_cell_data(
         self,
         datarn: int,
```

### Comparing `tksheet-7.2.1/tksheet/other_classes.py` & `tksheet-7.2.2/tksheet/other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.1/tksheet/row_index.py` & `tksheet-7.2.2/tksheet/row_index.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from __future__ import annotations
 
 import tkinter as tk
 from collections import defaultdict
 from collections.abc import (
     Callable,
     Generator,
+    Hashable,
+    Iterator,
+    Sequence,
 )
 from functools import (
     partial,
 )
 from itertools import (
     chain,
     cycle,
     islice,
+    repeat,
 )
 from math import (
     ceil,
     floor,
 )
+from operator import (
+    itemgetter,
+)
 from typing import Literal
 
 from .colors import (
     color_map,
 )
 from .formatters import (
     is_bool_like,
@@ -591,21 +598,21 @@
                         self.PAR.emit_event("<<SheetSelect>>", data=sel_event)
                 if self.scroll_if_event_offscreen(event):
                     need_redraw = True
             if need_redraw:
                 self.MT.main_table_redraw_grid_and_text(redraw_header=False, redraw_row_index=True)
         try_binding(self.extra_b1_motion_func, event)
 
-    def get_b1_motion_box(self, start_row, end_row):
+    def get_b1_motion_box(self, start_row: int, end_row: int) -> tuple[int, int, int, int, Literal["rows"]]:
         if end_row >= start_row:
             return start_row, 0, end_row + 1, len(self.MT.col_positions) - 1, "rows"
         elif end_row < start_row:
             return end_row, 0, start_row + 1, len(self.MT.col_positions) - 1, "rows"
 
-    def ctrl_b1_motion(self, event: object):
+    def ctrl_b1_motion(self, event: object) -> None:
         x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
         if (
             self.drag_and_drop_enabled
             and self.row_selection_enabled
             and self.rsz_h is None
             and self.rsz_w is None
             and self.dragged_row is not None
@@ -651,15 +658,15 @@
                 if self.scroll_if_event_offscreen(event):
                     need_redraw = True
             if need_redraw:
                 self.MT.main_table_redraw_grid_and_text(redraw_header=False, redraw_row_index=True)
         elif not self.MT.ctrl_select_enabled:
             self.b1_motion(event)
 
-    def drag_and_drop_motion(self, event: object):
+    def drag_and_drop_motion(self, event: object) -> float:
         y = event.y
         hend = self.winfo_height()
         ycheck = self.yview()
         if y >= hend - 0 and len(ycheck) > 1 and ycheck[1] < 1:
             if y >= hend + 15:
                 self.MT.yview_scroll(2, "units")
                 self.yview_scroll(2, "units")
@@ -688,19 +695,19 @@
             return self.MT.row_positions[row]
         elif row > self.dragged_row.to_move[-1]:
             return self.MT.row_positions[row + 1]
         return self.MT.row_positions[row]
 
     def show_drag_and_drop_indicators(
         self,
-        ypos,
-        x1,
-        x2,
-        rows,
-    ):
+        ypos: float,
+        x1: float,
+        x2: float,
+        rows: Sequence[int],
+    ) -> None:
         self.hide_resize_and_ctrl_lines()
         self.create_resize_line(
             0,
             ypos,
             self.current_width,
             ypos,
             width=3,
@@ -713,21 +720,21 @@
                 start_cell=(0, chunk[0]),
                 end_cell=(len(self.MT.col_positions) - 1, chunk[-1] + 1),
                 dash=(),
                 outline=self.PAR.ops.drag_and_drop_bg,
                 delete_on_timer=False,
             )
 
-    def hide_resize_and_ctrl_lines(self, ctrl_lines=True):
+    def hide_resize_and_ctrl_lines(self, ctrl_lines: bool = True) -> None:
         self.delete_resize_lines()
         self.MT.delete_resize_lines()
         if ctrl_lines:
             self.MT.delete_ctrl_outlines()
 
-    def scroll_if_event_offscreen(self, event: object):
+    def scroll_if_event_offscreen(self, event: object) -> bool:
         ycheck = self.yview()
         need_redraw = False
         if event.y > self.winfo_height() and len(ycheck) > 1 and ycheck[1] < 1:
             try:
                 self.MT.yview_scroll(1, "units")
                 self.yview_scroll(1, "units")
             except Exception:
@@ -742,15 +749,15 @@
             except Exception:
                 pass
             self.fix_yview()
             self.MT.y_move_synced_scrolls("moveto", self.MT.yview()[0])
             need_redraw = True
         return need_redraw
 
-    def fix_yview(self):
+    def fix_yview(self) -> None:
         ycheck = self.yview()
         if ycheck and ycheck[0] < 0:
             self.MT.set_yviews("moveto", 0)
         if len(ycheck) > 1 and ycheck[1] > 1:
             self.MT.set_yviews("moveto", 1)
 
     def event_over_dropdown(self, r: int, datarn: int, event: object, canvasy: float) -> bool:
@@ -1038,192 +1045,195 @@
             else:
                 align = self.align
             if align == "w":
                 w += self.MT.index_txt_height
             w += self.get_treeview_indent(self.MT._row_index[datarn].iid) + 5
         return w, h
 
-    def set_row_height(
+    def get_row_text_height(
         self,
         row: int,
-        height: None | int = None,
-        only_set_if_too_small: bool = False,
-        recreate: bool = True,
-        return_new_height: bool = False,
-        displayed_only: bool = False,
+        visible_only: bool = False,
+        only_if_too_small: bool = False,
     ) -> int:
-        r_norm = row + 1
-        r_extra = row + 2
-        min_rh = self.MT.min_row_height
+        h = self.MT.min_row_height
         datarn = row if self.MT.all_rows_displayed else self.MT.displayed_rows[row]
-        if height is None:
+        # index
+        _w, ih = self.get_cell_dimensions(datarn)
+        # table
+        if self.MT.data:
             if self.MT.all_columns_displayed:
-                if displayed_only:
-                    x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
-                    start_col, end_col = self.MT.get_visible_columns(x1, x2)
+                if visible_only:
+                    iterable = range(*self.MT.visible_text_columns)
                 else:
                     if not self.MT.data or datarn >= len(self.MT.data):
                         iterable = range(0, 0)
                     else:
                         iterable = range(0, len(self.MT.data[datarn]))
             else:
-                if displayed_only:
-                    x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
-                    start_col, end_col = self.MT.get_visible_columns(x1, x2)
+                if visible_only:
+                    start_col, end_col = self.MT.visible_text_columns
                 else:
                     start_col, end_col = 0, len(self.MT.displayed_columns)
                 iterable = self.MT.displayed_columns[start_col:end_col]
-            new_height = int(min_rh)
-            w_, h = self.get_cell_dimensions(datarn)
-            if h < min_rh:
-                h = int(min_rh)
-            elif h > self.MT.max_row_height:
-                h = int(self.MT.max_row_height)
-            if h > new_height:
-                new_height = h
-            if self.MT.data:
-                for datacn in iterable:
-                    txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True)
-                    if txt:
-                        h = self.MT.get_txt_h(txt) + 5
-                    else:
-                        h = min_rh
-                    if h < min_rh:
-                        h = int(min_rh)
-                    elif h > self.MT.max_row_height:
-                        h = int(self.MT.max_row_height)
-                    if h > new_height:
-                        new_height = h
-        else:
-            new_height = int(height)
-        if new_height < min_rh:
-            new_height = int(min_rh)
-        elif new_height > self.MT.max_row_height:
-            new_height = int(self.MT.max_row_height)
-        if only_set_if_too_small and new_height <= self.MT.row_positions[row + 1] - self.MT.row_positions[row]:
+            for datacn in iterable:
+                if (txt := self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True)) and (
+                    th := self.MT.get_txt_h(txt) + 5
+                ) > h:
+                    h = th
+        if ih > h:
+            h = ih
+        if only_if_too_small and h < self.MT.row_positions[row + 1] - self.MT.row_positions[row]:
             return self.MT.row_positions[row + 1] - self.MT.row_positions[row]
-        if not return_new_height:
-            new_row_pos = self.MT.row_positions[row] + new_height
-            increment = new_row_pos - self.MT.row_positions[r_norm]
-            self.MT.row_positions[r_extra:] = [
-                e + increment for e in islice(self.MT.row_positions, r_extra, len(self.MT.row_positions))
-            ]
-            self.MT.row_positions[r_norm] = new_row_pos
-            if recreate:
-                self.MT.recreate_all_selection_boxes()
-        return new_height
+        if h < self.MT.min_row_height:
+            h = int(self.MT.min_row_height)
+        elif h > self.MT.max_row_height:
+            h = int(self.MT.max_row_height)
+        return h
 
-    def set_width_of_index_to_text(
+    def set_row_height(
         self,
-        text: None | str = None,
-        only_rows: list = [],
-        set_width: bool = True,
-    ) -> None | int:
-        if (
-            text is None
-            and not self.MT._row_index
-            and isinstance(self.MT._row_index, list)
-            or isinstance(self.MT._row_index, int)
-            and self.MT._row_index >= len(self.MT.data)
+        row: int,
+        height: None | int = None,
+        only_if_too_small: bool = False,
+        visible_only: bool = False,
+        recreate: bool = True,
+    ) -> int:
+        if height is None:
+            height = self.get_row_text_height(row=row, visible_only=visible_only)
+        if height < self.MT.min_row_height:
+            height = int(self.MT.min_row_height)
+        elif height > self.MT.max_row_height:
+            height = int(self.MT.max_row_height)
+        if only_if_too_small and height <= self.MT.row_positions[row + 1] - self.MT.row_positions[row]:
+            return self.MT.row_positions[row + 1] - self.MT.row_positions[row]
+        new_row_pos = self.MT.row_positions[row] + height
+        increment = new_row_pos - self.MT.row_positions[row + 1]
+        self.MT.row_positions[row + 2 :] = [
+            e + increment for e in islice(self.MT.row_positions, row + 2, len(self.MT.row_positions))
+        ]
+        self.MT.row_positions[row + 1] = new_row_pos
+        if recreate:
+            self.MT.recreate_all_selection_boxes()
+        return height
+
+    def get_index_text_width(
+        self,
+        only_rows: Iterator[int] | None = None,
+    ) -> int:
+        self.fix_index()
+        w = self.PAR.ops.default_row_index_width
+        if (not self.MT._row_index and isinstance(self.MT._row_index, list)) or (
+            isinstance(self.MT._row_index, int) and self.MT._row_index >= len(self.MT.data)
         ):
-            return
+            return w
         qconf = self.MT.txt_measure_canvas.itemconfig
         qbbox = self.MT.txt_measure_canvas.bbox
         qtxtm = self.MT.txt_measure_canvas_text
-        new_width = int(self.MT.min_column_width)
-        self.fix_index()
-        if text is not None:
-            if text:
-                qconf(qtxtm, text=text)
-                b = qbbox(qtxtm)
-                w = b[2] - b[0] + 10
-                if w > new_width:
-                    new_width = w
-            else:
-                w = self.PAR.ops.default_row_index_width
-        else:
-            if only_rows:
-                iterable = only_rows
-            elif self.MT.all_rows_displayed:
-                if isinstance(self.MT._row_index, list):
-                    iterable = range(len(self.MT._row_index))
-                else:
-                    iterable = range(len(self.MT.data))
-            else:
-                iterable = self.MT.displayed_rows
+        if only_rows:
+            iterable = only_rows
+        elif self.MT.all_rows_displayed:
             if isinstance(self.MT._row_index, list):
-                for datarn in iterable:
-                    w, h_ = self.get_cell_dimensions(datarn)
-                    if w < self.MT.min_column_width:
-                        w = int(self.MT.min_column_width)
-                    elif w > self.MT.max_index_width:
-                        w = int(self.MT.max_index_width)
-                    if w > new_width:
-                        new_width = w
-            elif isinstance(self.MT._row_index, int):
-                datacn = self.MT._row_index
-                for datarn in iterable:
-                    txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True)
-                    if txt:
-                        qconf(qtxtm, text=txt)
-                        b = qbbox(qtxtm)
-                        w = b[2] - b[0] + 10
-                    else:
-                        w = self.PAR.ops.default_row_index_width
-                    if w < self.MT.min_column_width:
-                        w = int(self.MT.min_column_width)
-                    elif w > self.MT.max_index_width:
-                        w = int(self.MT.max_index_width)
-                    if w > new_width:
-                        new_width = w
-        if new_width == self.MT.min_column_width:
-            new_width = self.MT.min_column_width + 10
-        if set_width:
-            self.set_width(new_width, set_TL=True)
-            self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
-        return new_width
+                iterable = range(len(self.MT._row_index))
+            else:
+                iterable = range(len(self.MT.data))
+        else:
+            iterable = self.MT.displayed_rows
+        if (
+            isinstance(self.MT._row_index, list)
+            and (tw := max(map(itemgetter(0), map(self.get_cell_dimensions, iterable)), default=w)) > w
+        ):
+            w = tw
+        elif isinstance(self.MT._row_index, int):
+            datacn = self.MT._row_index
+            for datarn in iterable:
+                if txt := self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True):
+                    qconf(qtxtm, text=txt)
+                    b = qbbox(qtxtm)
+                    if (tw := b[2] - b[0] + 10) > w:
+                        w = tw
+        if w > self.MT.max_index_width:
+            w = int(self.MT.max_index_width)
+        return w
 
-    def set_height_of_all_rows(self, height=None, only_set_if_too_small=False, recreate=True):
+    def set_width_of_index_to_text(
+        self,
+        text: None | str = None,
+        only_rows: list = [],
+    ) -> int:
+        self.fix_index()
+        w = self.PAR.ops.default_row_index_width
+        if (text is None and isinstance(self.MT._row_index, list) and not self.MT._row_index) or (
+            isinstance(self.MT._row_index, int) and self.MT._row_index >= len(self.MT.data)
+        ):
+            return w
+        if text is not None and text:
+            self.MT.txt_measure_canvas.itemconfig(self.MT.txt_measure_canvas_text, text=text)
+            b = self.MT.txt_measure_canvas.bbox(self.MT.txt_measure_canvas_text)
+            if (tw := b[2] - b[0] + 10) > w:
+                w = tw
+        elif text is None:
+            w = self.get_index_text_width(only_rows=only_rows)
+        if w > self.MT.max_index_width:
+            w = int(self.MT.max_index_width)
+        self.set_width(w, set_TL=True)
+        self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
+        return w
+
+    def set_height_of_all_rows(
+        self,
+        height: int | None = None,
+        only_if_too_small: bool = False,
+        recreate: bool = True,
+    ) -> None:
         if height is None:
+            if self.MT.all_columns_displayed:
+                iterable = range(self.MT.total_data_rows())
+            else:
+                iterable = range(len(self.MT.displayed_rows))
             self.MT.set_row_positions(
-                itr=(
-                    self.set_row_height(
-                        rn,
-                        only_set_if_too_small=only_set_if_too_small,
-                        recreate=False,
-                        return_new_height=True,
-                    )
-                    for rn in range(len(self.MT.data))
-                )
+                itr=(self.get_row_text_height(rn, only_if_too_small=only_if_too_small) for rn in iterable)
             )
-        else:
-            self.MT.set_row_positions(itr=(height for r in range(len(self.MT.data))))
+        elif height is not None:
+            if self.MT.all_rows_displayed:
+                self.MT.set_row_positions(itr=repeat(height, len(self.MT.data)))
+            else:
+                self.MT.set_row_positions(itr=repeat(height, len(self.MT.displayed_rows)))
         if recreate:
             self.MT.recreate_all_selection_boxes()
 
     def auto_set_index_width(self, end_row: int, only_rows: list) -> bool:
         if not isinstance(self.MT._row_index, int) and not self.MT._row_index:
             if self.default_index == "letters":
                 new_w = self.MT.get_txt_w(f"{num2alpha(end_row)}") + 20
             elif self.default_index == "numbers":
                 new_w = self.MT.get_txt_w(f"{end_row}") + 20
             elif self.default_index == "both":
                 new_w = self.MT.get_txt_w(f"{end_row + 1} {num2alpha(end_row)}") + 20
         elif self.PAR.ops.auto_resize_row_index is True:
-            new_w = self.set_width_of_index_to_text(only_rows=only_rows, set_width=False)
+            new_w = self.get_index_text_width(only_rows=only_rows)
         else:
             new_w = None
         if new_w is not None and (sheet_w_x := floor(self.PAR.winfo_width() * 0.7)) < new_w:
             new_w = sheet_w_x
         if new_w and (self.current_width - new_w > 20 or new_w - self.current_width > 3):
             self.set_width(new_w, set_TL=True, recreate_selection_boxes=False)
             return True
         return False
 
-    def redraw_highlight_get_text_fg(self, fr, sr, r, c_2, c_3, selections, datarn):
+    def redraw_highlight_get_text_fg(
+        self,
+        fr: float,
+        sr: float,
+        r: int,
+        c_2: str,
+        c_3: str,
+        selections: dict,
+        datarn: int,
+    ) -> tuple[str, str, bool]:
         redrawn = False
         kwargs = self.get_cell_kwargs(datarn, key="highlight")
         if kwargs:
             if kwargs[0] is not None:
                 c_1 = kwargs[0] if kwargs[0].startswith("#") else color_map[kwargs[0]]
             if "rows" in selections and r in selections["rows"]:
                 txtfg = (
@@ -1276,47 +1286,62 @@
                 txtfg = self.PAR.ops.index_selected_cells_fg
                 tree_arrow_fg = self.PAR.ops.selected_cells_tree_arrow_fg
             else:
                 txtfg = self.PAR.ops.index_fg
                 tree_arrow_fg = self.PAR.ops.tree_arrow_fg
         return txtfg, tree_arrow_fg, redrawn
 
-    def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag):
+    def redraw_highlight(
+        self,
+        x1: float,
+        y1: float,
+        x2: float,
+        y2: float,
+        fill: str,
+        outline: str,
+        tag: str | tuple[str],
+    ) -> bool:
         coords = (x1, y1, x2, y2)
         if self.hidd_high:
             iid, showing = self.hidd_high.popitem()
             self.coords(iid, coords)
             if showing:
                 self.itemconfig(iid, fill=fill, outline=outline)
             else:
                 self.itemconfig(iid, fill=fill, outline=outline, tag=tag, state="normal")
         else:
             iid = self.create_rectangle(coords, fill=fill, outline=outline, tag=tag)
         self.disp_high[iid] = True
         return True
 
-    def redraw_gridline(self, points, fill, width, tag):
+    def redraw_gridline(
+        self,
+        points: tuple[float],
+        fill: str,
+        width: int,
+        tag: str | tuple[str],
+    ) -> None:
         if self.hidd_grid:
             t, sh = self.hidd_grid.popitem()
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill=fill, width=width, tag=tag)
             else:
                 self.itemconfig(t, fill=fill, width=width, tag=tag, state="normal")
             self.disp_grid[t] = True
         else:
             self.disp_grid[self.create_line(points, fill=fill, width=width, tag=tag)] = True
 
     def redraw_tree_arrow(
         self,
-        x1,
-        y1,
-        r,
-        fill,
-        tag,
+        x1: float,
+        y1: float,
+        r: int,
+        fill: str,
+        tag: str | tuple[str],
         indent: float,
         open_: bool = False,
     ) -> None:
         mod = (self.MT.index_txt_height - 1) if self.MT.index_txt_height % 2 else self.MT.index_txt_height
         half_mod = mod / 2
         qtr_mod = mod / 4
         small_mod = int(half_mod / 4) - 1
@@ -1358,21 +1383,21 @@
                 capstyle=tk.ROUND,
                 joinstyle=tk.BEVEL,
             )
         self.disp_tree_arrow[t] = True
 
     def redraw_dropdown(
         self,
-        x1,
-        y1,
-        x2,
-        y2,
-        fill,
-        outline,
-        tag,
+        x1: float,
+        y1: float,
+        x2: float,
+        y2: float,
+        fill: str,
+        outline: str,
+        tag: str | tuple[str],
         draw_outline: bool = True,
         draw_arrow: bool = True,
         open_: bool = False,
     ) -> None:
         if draw_outline and self.PAR.ops.show_dropdown_borders:
             self.redraw_highlight(x1 + 1, y1 + 1, x2, y2, fill="", outline=self.PAR.ops.index_fg, tag=tag)
         if draw_arrow:
@@ -1410,15 +1435,25 @@
                 t = self.create_polygon(
                     points,
                     fill=fill,
                     tag=tag,
                 )
             self.disp_dropdown[t] = True
 
-    def redraw_checkbox(self, x1, y1, x2, y2, fill, outline, tag, draw_check=False):
+    def redraw_checkbox(
+        self,
+        x1: float,
+        y1: float,
+        x2: float,
+        y2: float,
+        fill: str,
+        outline: str,
+        tag: str | tuple[str],
+        draw_check: bool = False,
+    ) -> None:
         points = rounded_box_coords(x1, y1, x2, y2)
         if self.hidd_checkbox:
             t, sh = self.hidd_checkbox.popitem()
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill=outline, outline=fill)
             else:
@@ -1457,16 +1492,18 @@
         )
 
     def redraw_grid_and_text(
         self,
         last_row_line_pos: float,
         scrollpos_top: int,
         y_stop: int,
-        start_row: int,
-        end_row: int,
+        grid_start_row: int,
+        grid_end_row: int,
+        text_start_row: int,
+        text_end_row: int,
         scrollpos_bot: int,
         row_pos_exists: bool,
     ) -> None:
         try:
             self.configure_scrollregion(last_row_line_pos=last_row_line_pos)
         except Exception:
             return
@@ -1479,15 +1516,15 @@
         self.hidd_dropdown.update(self.disp_dropdown)
         self.disp_dropdown = {}
         self.hidd_checkbox.update(self.disp_checkbox)
         self.disp_checkbox = {}
         self.hidd_tree_arrow.update(self.disp_tree_arrow)
         self.disp_tree_arrow = {}
         self.visible_row_dividers = {}
-        draw_y = self.MT.row_positions[start_row]
+        draw_y = self.MT.row_positions[grid_start_row]
         xend = self.current_width - 6
         self.row_width_resize_bbox = (
             self.current_width - 2,
             scrollpos_top,
             self.current_width,
             scrollpos_bot,
         )
@@ -1496,15 +1533,15 @@
                 self.current_width - 1,
                 y_stop - 1,
                 self.current_width - 1,
                 scrollpos_top - 1,
                 -1,
                 scrollpos_top - 1,
             ]
-            for r in range(start_row + 1, end_row):
+            for r in range(grid_start_row, grid_end_row):
                 draw_y = self.MT.row_positions[r]
                 if self.height_resizing_enabled:
                     self.visible_row_dividers[r] = (1, draw_y - 2, xend, draw_y + 2)
                 points.extend(
                     (
                         -1,
                         draw_y,
@@ -1524,19 +1561,19 @@
         )
         c_3 = (
             self.PAR.ops.index_selected_rows_bg
             if self.PAR.ops.index_selected_rows_bg.startswith("#")
             else color_map[self.PAR.ops.index_selected_rows_bg]
         )
         font = self.PAR.ops.index_font
-        selections = self.get_redraw_selections(start_row, end_row)
+        selections = self.get_redraw_selections(text_start_row, grid_end_row)
         dd_coords = self.dropdown.get_coords()
         treeview = self.PAR.ops.treeview
 
-        for r in range(start_row, end_row - 1):
+        for r in range(text_start_row, text_end_row):
             rtopgridln = self.MT.row_positions[r]
             rbotgridln = self.MT.row_positions[r + 1]
             if rbotgridln - rtopgridln < self.MT.index_txt_height:
                 continue
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
             fill, tree_arrow_fg, dd_drawn = self.redraw_highlight_get_text_fg(
                 rtopgridln,
@@ -1754,15 +1791,15 @@
         for item, box in self.MT.get_selection_items():
             r1, c1, r2, c2 = box.coords
             for r in range(startr, endr):
                 if r1 <= r and r2 > r:
                     d[box.type_ if box.type_ != "columns" else "cells"].add(r)
         return d
 
-    def open_cell(self, event: object = None, ignore_existing_editor=False):
+    def open_cell(self, event: object = None, ignore_existing_editor: bool = False) -> None:
         if not self.MT.anything_selected() or (not ignore_existing_editor and self.text_editor.open):
             return
         if not self.MT.selected:
             return
         r = self.MT.selected.row
         datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
         if self.get_cell_kwargs(datarn, key="readonly"):
@@ -1773,31 +1810,31 @@
                     self.open_dropdown_window(r, event=event)
                 elif self.get_cell_kwargs(datarn, key="checkbox"):
                     self.click_checkbox(r, datarn)
         elif self.edit_cell_enabled:
             self.open_text_editor(event=event, r=r, dropdown=False)
 
     # displayed indexes
-    def get_cell_align(self, r):
+    def get_cell_align(self, r: int) -> str:
         datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
         if datarn in self.cell_options and "align" in self.cell_options[datarn]:
             align = self.cell_options[datarn]["align"]
         else:
             align = self.align
         return align
 
     # r is displayed row
     def open_text_editor(
         self,
         event: object = None,
-        r=0,
-        text=None,
-        state="normal",
-        dropdown=False,
-    ):
+        r: int = 0,
+        text: None | str = None,
+        state: str = "normal",
+        dropdown: bool = False,
+    ) -> bool:
         text = None
         extra_func_key = "??"
         if event is None or self.MT.event_opens_dropdown_or_checkbox(event):
             if event is not None:
                 if hasattr(event, "keysym") and event.keysym == "Return":
                     extra_func_key = "Return"
                 elif hasattr(event, "keysym") and event.keysym == "F2":
@@ -1892,15 +1929,15 @@
             self.text_editor.tktext.focus_set()
             self.text_editor.window.scroll_to_bottom()
             self.text_editor.tktext.bind("<FocusOut>", self.close_text_editor)
         for key, func in self.MT.text_editor_user_bound_keys.items():
             self.text_editor.tktext.bind(key, func)
         return True
 
-    def text_editor_newline_binding(self, event: object = None, check_lines=True):
+    def text_editor_newline_binding(self, event: object = None, check_lines: bool = True) -> None:
         if not self.height_resizing_enabled:
             return
         curr_height = self.text_editor.window.winfo_height()
         if curr_height < self.MT.min_row_height:
             return
         if (
             not check_lines
@@ -1934,15 +1971,15 @@
                         self.coords(
                             self.dropdown.canvas_id,
                             0,
                             self.MT.row_positions[r],
                         )
                         self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
 
-    def refresh_open_window_positions(self, zoom: Literal["in", "out"]):
+    def refresh_open_window_positions(self, zoom: Literal["in", "out"]) -> None:
         if self.text_editor.open:
             r = self.text_editor.row
             self.text_editor.window.config(height=self.MT.row_positions[r + 1] - self.MT.row_positions[r])
             self.text_editor.tktext.config(font=self.PAR.ops.index_font)
             self.coords(
                 self.text_editor.canvas_id,
                 0,
@@ -2036,15 +2073,15 @@
             try_binding(self.extra_end_edit_cell_func, event_data)
         self.MT.recreate_all_selection_boxes()
         self.hide_text_editor_and_dropdown()
         if event.keysym != "FocusOut":
             self.focus_set()
         return "break"
 
-    def get_dropdown_height_anchor(self, r, text_editor_h=None):
+    def get_dropdown_height_anchor(self, r: int, text_editor_h: None | int = None) -> tuple[int, str]:
         win_h = 5
         datarn = self.MT.datarn(r)
         for i, v in enumerate(self.get_cell_kwargs(datarn, key="dropdown")["values"]):
             v_numlines = len(v.split("\n") if isinstance(v, str) else f"{v}".split("\n"))
             if v_numlines > 1:
                 win_h += (
                     self.MT.index_first_ln_ins + (v_numlines * self.MT.index_xtra_lines_increment) + 5
@@ -2079,15 +2116,15 @@
         modified_func: Callable | None,
     ) -> None:
         if modified_func:
             modified_func(event)
         dd_window.search_and_see(event)
 
     # r is displayed row
-    def open_dropdown_window(self, r, event: object = None):
+    def open_dropdown_window(self, r: int, event: object = None) -> None:
         self.hide_text_editor("Escape")
         kwargs = self.get_cell_kwargs(self.MT.datarn(r), key="dropdown")
         if kwargs["state"] == "normal":
             if not self.open_text_editor(event=event, r=r, dropdown=True):
                 return
         win_h, anchor = self.get_dropdown_height_anchor(r)
         win_w = self.current_width + 1
@@ -2160,15 +2197,20 @@
             self.dropdown.window.focus_set()
             redraw = True
         self.dropdown.open = True
         if redraw:
             self.MT.main_table_redraw_grid_and_text(redraw_header=False, redraw_row_index=True, redraw_table=False)
 
     # r is displayed row
-    def close_dropdown_window(self, r=None, selection=None, redraw=True):
+    def close_dropdown_window(
+        self,
+        r: int | None = None,
+        selection: object = None,
+        redraw: bool = True,
+    ) -> None:
         if r is not None and selection is not None:
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
             kwargs = self.get_cell_kwargs(datarn, key="dropdown")
             pre_edit_value = self.get_cell_data(datarn)
             edited = False
             event_data = event_dict(
                 name="end_edit_index",
@@ -2198,29 +2240,29 @@
 
     def hide_text_editor_and_dropdown(self, redraw: bool = True) -> None:
         self.hide_text_editor("Escape")
         self.hide_dropdown_window()
         if redraw:
             self.MT.refresh()
 
-    def mouseclick_outside_editor_or_dropdown(self, inside: bool = False):
+    def mouseclick_outside_editor_or_dropdown(self, inside: bool = False) -> int | None:
         closed_dd_coords = self.dropdown.get_coords()
         if self.text_editor.open:
             self.close_text_editor(new_tk_event("ButtonPress-1"))
         if closed_dd_coords is not None:
             self.hide_dropdown_window()
             if inside:
                 self.MT.main_table_redraw_grid_and_text(
                     redraw_header=False,
                     redraw_row_index=True,
                     redraw_table=False,
                 )
         return closed_dd_coords
 
-    def mouseclick_outside_editor_or_dropdown_all_canvases(self, inside: bool = False):
+    def mouseclick_outside_editor_or_dropdown_all_canvases(self, inside: bool = False) -> int | None:
         self.CH.mouseclick_outside_editor_or_dropdown()
         self.MT.mouseclick_outside_editor_or_dropdown()
         return self.mouseclick_outside_editor_or_dropdown(inside)
 
     def hide_dropdown_window(self) -> None:
         if self.dropdown.open:
             self.dropdown.window.unbind("<FocusOut>")
@@ -2255,22 +2297,22 @@
             self.fix_index(datarn)
             if not check_input_valid or self.input_valid_for_cell(datarn, value):
                 if self.MT.undo_enabled and undo:
                     self.MT.undo_stack.append(pickled_event_dict(event_data))
                 self.set_cell_data(datarn=datarn, value=value)
                 edited = True
         if edited and cell_resize and self.PAR.ops.cell_auto_resize_enabled:
-            self.set_row_height_run_binding(r, only_set_if_too_small=False)
+            self.set_row_height_run_binding(r, only_if_too_small=False)
         if redraw:
             self.MT.refresh()
         if edited:
             self.MT.sheet_modified(event_data)
         return edited
 
-    def set_cell_data(self, datarn=None, value=""):
+    def set_cell_data(self, datarn: int | None = None, value: object = "") -> None:
         if isinstance(self.MT._row_index, int):
             self.MT.set_cell_data(datarn=datarn, datacn=self.MT._row_index, value=value)
         else:
             self.fix_index(datarn)
             if self.get_cell_kwargs(datarn, key="checkbox"):
                 self.MT._row_index[datarn] = try_to_bool(value)
             else:
@@ -2284,42 +2326,42 @@
         if self.cell_equal_to(datarn, value):
             return False
         kwargs = self.get_cell_kwargs(datarn, key="dropdown")
         if kwargs and kwargs["validate_input"] and value not in kwargs["values"]:
             return False
         return True
 
-    def cell_equal_to(self, datarn, value):
+    def cell_equal_to(self, datarn: int, value: object) -> bool:
         self.fix_index(datarn)
         if isinstance(self.MT._row_index, list):
             return self.MT._row_index[datarn] == value
         elif isinstance(self.MT._row_index, int):
             return self.MT.cell_equal_to(datarn, self.MT._row_index, value)
 
     def get_cell_data(
         self,
-        datarn,
-        get_displayed=False,
-        none_to_empty_str=False,
-        redirect_int=False,
-    ):
+        datarn: int,
+        get_displayed: bool = False,
+        none_to_empty_str: bool = False,
+        redirect_int: bool = False,
+    ) -> object:
         if get_displayed:
             return self.get_valid_cell_data_as_str(datarn, fix=False)
         if redirect_int and isinstance(self.MT._row_index, int):  # internal use
             return self.MT.get_cell_data(datarn, self.MT._row_index, none_to_empty_str=True)
         if (
             isinstance(self.MT._row_index, int)
             or not self.MT._row_index
             or datarn >= len(self.MT._row_index)
             or (self.MT._row_index[datarn] is None and none_to_empty_str)
         ):
             return ""
         return self.MT._row_index[datarn]
 
-    def get_valid_cell_data_as_str(self, datarn, fix=True) -> str:
+    def get_valid_cell_data_as_str(self, datarn: int, fix: bool = True) -> str:
         kwargs = self.get_cell_kwargs(datarn, key="dropdown")
         if kwargs:
             if kwargs["text"] is not None:
                 return f"{kwargs['text']}"
         else:
             kwargs = self.get_cell_kwargs(datarn, key="checkbox")
             if kwargs:
@@ -2332,57 +2374,53 @@
             value = "" if self.MT._row_index[datarn] is None else f"{self.MT._row_index[datarn]}"
         except Exception:
             value = ""
         if not value and self.PAR.ops.show_default_index_for_empty:
             value = get_n2a(datarn, self.default_index)
         return value
 
-    def get_value_for_empty_cell(self, datarn, r_ops=True):
+    def get_value_for_empty_cell(self, datarn: int, r_ops: bool = True) -> object:
         if self.get_cell_kwargs(datarn, key="checkbox", cell=r_ops):
             return False
         kwargs = self.get_cell_kwargs(datarn, key="dropdown", cell=r_ops)
         if kwargs and kwargs["validate_input"] and kwargs["values"]:
             return kwargs["values"][0]
         return ""
 
-    def get_empty_index_seq(self, end, start=0, r_ops=True):
+    def get_empty_index_seq(self, end: int, start: int = 0, r_ops: bool = True) -> list[object]:
         return [self.get_value_for_empty_cell(datarn, r_ops=r_ops) for datarn in range(start, end)]
 
-    def fix_index(self, datarn=None, fix_values=tuple()):
+    def fix_index(self, datarn: int | None = None) -> None:
         if isinstance(self.MT._row_index, int):
             return
         if isinstance(self.MT._row_index, float):
             self.MT._row_index = int(self.MT._row_index)
             return
         if not isinstance(self.MT._row_index, list):
             try:
                 self.MT._row_index = list(self.MT._row_index)
             except Exception:
                 self.MT._row_index = []
         if isinstance(datarn, int) and datarn >= len(self.MT._row_index):
             self.MT._row_index.extend(self.get_empty_index_seq(end=datarn + 1, start=len(self.MT._row_index)))
-        if fix_values:
-            for rn, v in enumerate(islice(self.MT._row_index, fix_values[0], fix_values[1])):
-                if not self.input_valid_for_cell(rn, v):
-                    self.MT._row_index[rn] = self.get_value_for_empty_cell(rn)
 
-    def set_row_height_run_binding(self, r, only_set_if_too_small=True):
+    def set_row_height_run_binding(self, r: int, only_if_too_small: bool = True) -> None:
         old_height = self.MT.row_positions[r + 1] - self.MT.row_positions[r]
-        new_height = self.set_row_height(r, only_set_if_too_small=only_set_if_too_small)
+        new_height = self.set_row_height(r, only_if_too_small=only_if_too_small)
         if self.row_height_resize_func is not None and old_height != new_height:
             self.row_height_resize_func(
                 event_dict(
                     name="resize",
                     sheet=self.PAR.name,
                     resized_rows={r: {"old_size": old_height, "new_size": new_height}},
                 )
             )
 
     # internal event use
-    def click_checkbox(self, r, datarn=None, undo=True, redraw=True):
+    def click_checkbox(self, r: int, datarn: int | None = None, undo: bool = True, redraw: bool = True) -> None:
         if datarn is None:
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
         kwargs = self.get_cell_kwargs(datarn, key="checkbox")
         if kwargs["state"] == "normal":
             pre_edit_value = self.get_cell_data(datarn)
             if isinstance(self.MT._row_index, list):
                 value = not self.MT._row_index[datarn] if isinstance(self.MT._row_index[datarn], bool) else False
@@ -2409,15 +2447,15 @@
             )
             if kwargs["check_function"] is not None:
                 kwargs["check_function"](event_data)
             try_binding(self.extra_end_edit_cell_func, event_data)
         if redraw:
             self.MT.refresh()
 
-    def get_cell_kwargs(self, datarn, key="dropdown", cell=True, entire=True):
+    def get_cell_kwargs(self, datarn: int, key: Hashable = "dropdown", cell: bool = True) -> dict:
         if cell and datarn in self.cell_options and key in self.cell_options[datarn]:
             return self.cell_options[datarn][key]
         return {}
 
     # Treeview Mode
 
     def get_node_level(self, node: Node, level: int = 0) -> Generator[int]:
```

### Comparing `tksheet-7.2.1/tksheet/sheet.py` & `tksheet-7.2.2/tksheet/sheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import tkinter as tk
 from bisect import bisect_left
 from collections import defaultdict, deque
 from collections.abc import Callable, Generator, Iterator, Sequence
-from itertools import accumulate, chain, islice, product
+from itertools import accumulate, chain, islice, product, repeat
 from timeit import default_timer
 from tkinter import ttk
 from typing import Literal
 
 from .column_headers import ColumnHeaders
 from .functions import (
     add_highlight,
@@ -588,15 +588,15 @@
 
     # Bindings and Functionality
 
     def enable_bindings(self, *bindings: str) -> Sheet:
         self.MT.enable_bindings(bindings)
         return self
 
-    def disable_bindings(self, *bindings) -> Sheet:
+    def disable_bindings(self, *bindings: str) -> Sheet:
         self.MT.disable_bindings(bindings)
         return self
 
     def extra_bindings(
         self,
         bindings: str | list | tuple | None = None,
         func: Callable | None = None,
@@ -1077,16 +1077,19 @@
         self,
     ) -> bool:
         """
         Check if any Sheet widgets have focus
         Includes child widgets such as scroll bars
         Returns bool
         """
-        widget = self.focus_get()
-        return widget == self or any(widget == c for c in self.children.values())
+        try:
+            widget = self.focus_get()
+            return widget == self or any(widget == c for c in self.children.values())
+        except Exception:
+            return False
 
     def focus_set(
         self,
         canvas: Literal[
             "table",
             "header",
             "row_index",
@@ -1285,16 +1288,14 @@
             totalcols=self.MT.total_data_cols,
         )
 
     def get_data(
         self,
         *key: CreateSpanTypes,
     ) -> object:
-        span = self.span_from_key(*key)
-        rows, cols = self.ranges_from_span(span)
         """
         e.g. retrieves entire table as pandas dataframe
         sheet["A1"].expand().options(pandas.DataFrame).data
 
         must deal with
         - format
         - transpose
@@ -1346,14 +1347,16 @@
         - if True gets displayed header values instead of actual data
 
         convert
         - instead of returning data normally it returns
           convert(data) - sends the data to an optional convert function
 
         """
+        span = self.span_from_key(*key)
+        rows, cols = self.ranges_from_span(span)
         tdisp, idisp, hdisp = span.tdisp, span.idisp, span.hdisp
         table, index, header = span.table, span.index, span.header
         fmt_kw = span.kwargs if span.type_ == "format" and span.kwargs else None
         quick_tdata, quick_idata, quick_hdata = self.MT.get_cell_data, self.RI.get_cell_data, self.CH.get_cell_data
         res = []
         if span.transposed:
             if index:
@@ -1542,24 +1545,20 @@
         self,
         *key: CreateSpanTypes,
         data: object = None,
         undo: bool | None = None,
         emit_event: bool | None = None,
         redraw: bool = True,
     ) -> EventDataDict:
-        span = self.span_from_key(*key)
-        if data is None:
-            data = []
         """
         e.g.
         df = pandas.DataFrame([[1, 2, 3], [4, 5, 6]])
         sheet["A1"] = df.values.tolist()
 
-        can't use slices or expand
-        just uses the from_r, from_c values
+        just uses the spans from_r, from_c values
 
         'data' parameter could be:
         - list of lists
         - list of values
         - not a list or tuple
             - can have all three of the below set at the same time
             or just one or two:
@@ -1595,14 +1594,17 @@
 
         in the table comments below -
         - t stands for table
         - i stands for index
         - h stands for header
 
         """
+        span = self.span_from_key(*key)
+        if data is None:
+            data = []
         startr, startc = span_froms(span)
         table, index, header = span.table, span.index, span.header
         fmt_kw = span.kwargs if span.type_ == "format" and span.kwargs else None
         transposed = span.transposed
         maxr, maxc = startr, startc
         event_data = event_dict(
             name="edit_table",
@@ -2262,24 +2264,22 @@
 
     def total_rows(
         self,
         number: int | None = None,
         mod_positions: bool = True,
         mod_data: bool = True,
     ) -> int | Sheet:
+        total_rows = self.MT.total_data_rows()
         if number is None:
-            return self.MT.total_data_rows()
+            return total_rows
         if not isinstance(number, int) or number < 0:
             raise ValueError("number argument must be integer and > 0")
-        if number > len(self.MT.data):
-            if mod_positions:
-                height = self.MT.get_default_row_height()
-                for r in range(number - len(self.MT.data)):
-                    self.MT.insert_row_position("end", height)
-        elif number < len(self.MT.data):
+        if number > total_rows and mod_positions:
+            self.MT.insert_row_positions(heights=number - total_rows)
+        elif number < total_rows:
             if not self.MT.all_rows_displayed:
                 self.MT.display_rows(enable=False, reset_row_positions=False, deselect_all=True)
             self.MT.row_positions[number + 1 :] = []
         if mod_data:
             self.MT.data_dimensions(total_rows=number)
         return self
 
@@ -2290,19 +2290,16 @@
         mod_data: bool = True,
     ) -> int | Sheet:
         total_cols = self.MT.total_data_cols()
         if number is None:
             return total_cols
         if not isinstance(number, int) or number < 0:
             raise ValueError("number argument must be integer and > 0")
-        if number > total_cols:
-            if mod_positions:
-                width = self.ops.default_column_width
-                for c in range(number - total_cols):
-                    self.MT.insert_col_position("end", width)
+        if number > total_cols and mod_positions:
+            self.MT.insert_col_positions(widths=number - total_cols)
         elif number < total_cols:
             if not self.MT.all_columns_displayed:
                 self.MT.display_columns(enable=False, reset_col_positions=False, deselect_all=True)
             self.MT.col_positions[number + 1 :] = []
         if mod_data:
             self.MT.data_dimensions(total_columns=number)
         return self
@@ -3330,15 +3327,15 @@
     def set_cell_size_to_text(
         self,
         row: int,
         column: int,
         only_set_if_too_small: bool = False,
         redraw: bool = True,
     ) -> Sheet:
-        self.MT.set_cell_size_to_text(r=row, c=column, only_set_if_too_small=only_set_if_too_small)
+        self.MT.set_cell_size_to_text(r=row, c=column, only_if_too_small=only_set_if_too_small)
         return self.set_refresh_timer(redraw)
 
     def set_all_cell_sizes_to_text(
         self,
         redraw: bool = True,
         width: int | None = None,
         slim: bool = False,
@@ -3352,113 +3349,135 @@
         width: int | None = None,
         only_set_if_too_small: bool = False,
         redraw: bool = True,
         recreate_selection_boxes: bool = True,
     ) -> Sheet:
         self.CH.set_width_of_all_cols(
             width=width,
-            only_set_if_too_small=only_set_if_too_small,
+            only_if_too_small=only_set_if_too_small,
             recreate=recreate_selection_boxes,
         )
         return self.set_refresh_timer(redraw)
 
     def set_all_row_heights(
         self,
         height: int | None = None,
         only_set_if_too_small: bool = False,
         redraw: bool = True,
         recreate_selection_boxes: bool = True,
     ) -> Sheet:
         self.RI.set_height_of_all_rows(
             height=height,
-            only_set_if_too_small=only_set_if_too_small,
+            only_if_too_small=only_set_if_too_small,
             recreate=recreate_selection_boxes,
         )
         return self.set_refresh_timer(redraw)
 
     def column_width(
         self,
         column: int | Literal["all", "displayed"] | None = None,
         width: int | Literal["default", "text"] | None = None,
         only_set_if_too_small: bool = False,
         redraw: bool = True,
     ) -> Sheet | int:
         if column == "all" and width == "default":
             self.MT.reset_col_positions()
         elif column == "displayed" and width == "text":
-            sc, ec = self.MT.get_visible_columns(self.MT.canvasx(0), self.MT.canvasx(self.winfo_width()))
-            for c in range(sc, ec - 1):
+            for c in range(*self.MT.visible_text_columns):
                 self.CH.set_col_width(c)
         elif width == "text" and isinstance(column, int):
-            self.CH.set_col_width(col=column, width=None, only_set_if_too_small=only_set_if_too_small)
+            self.CH.set_col_width(col=column, width=None, only_if_too_small=only_set_if_too_small)
         elif isinstance(width, int) and isinstance(column, int):
-            self.CH.set_col_width(col=column, width=width, only_set_if_too_small=only_set_if_too_small)
+            self.CH.set_col_width(col=column, width=width, only_if_too_small=only_set_if_too_small)
         elif isinstance(column, int):
             return int(self.MT.col_positions[column + 1] - self.MT.col_positions[column])
         return self.set_refresh_timer(redraw)
 
     def row_height(
         self,
         row: int | Literal["all", "displayed"] | None = None,
         height: int | Literal["default", "text"] | None = None,
         only_set_if_too_small: bool = False,
         redraw: bool = True,
     ) -> Sheet | int:
         if row == "all" and height == "default":
             self.MT.reset_row_positions()
         elif row == "displayed" and height == "text":
-            sr, er = self.MT.get_visible_rows(self.MT.canvasy(0), self.MT.canvasy(self.winfo_width()))
-            for r in range(sr, er - 1):
+            for r in range(*self.MT.visible_text_rows):
                 self.RI.set_row_height(r)
         elif height == "text" and isinstance(row, int):
-            self.RI.set_row_height(row=row, height=None, only_set_if_too_small=only_set_if_too_small)
+            self.RI.set_row_height(row=row, height=None, only_if_too_small=only_set_if_too_small)
         elif isinstance(height, int) and isinstance(row, int):
-            self.RI.set_row_height(row=row, height=height, only_set_if_too_small=only_set_if_too_small)
+            self.RI.set_row_height(row=row, height=height, only_if_too_small=only_set_if_too_small)
         elif isinstance(row, int):
             return int(self.MT.row_positions[row + 1] - self.MT.row_positions[row])
         return self.set_refresh_timer(redraw)
 
     def get_column_widths(self, canvas_positions: bool = False) -> list[float]:
         if canvas_positions:
             return self.MT.col_positions
         return self.MT.get_column_widths()
 
     def get_row_heights(self, canvas_positions: bool = False) -> list[float]:
         if canvas_positions:
             return self.MT.row_positions
         return self.MT.get_row_heights()
 
+    def get_row_text_height(
+        self,
+        row: int,
+        visible_only: bool = False,
+        only_if_too_small: bool = False,
+    ) -> int:
+        return self.RI.get_row_text_height(
+            row=row,
+            visible_only=visible_only,
+            only_if_too_small=only_if_too_small,
+        )
+
+    def get_column_text_width(
+        self,
+        column: int,
+        visible_only: bool = False,
+        only_if_too_small: bool = False,
+    ) -> int:
+        return self.CH.get_col_text_width(
+            col=column,
+            visible_only=visible_only,
+            only_if_too_small=only_if_too_small,
+        )
+
     def set_column_widths(
         self,
-        column_widths: Iterator[int, float] | None = None,
+        column_widths: Iterator[float] | None = None,
         canvas_positions: bool = False,
         reset: bool = False,
     ) -> Sheet:
         if reset or column_widths is None:
             self.MT.reset_col_positions()
         elif is_iterable(column_widths):
             if canvas_positions and isinstance(column_widths, list):
                 self.MT.col_positions = column_widths
             else:
-                self.MT.col_positions = list(accumulate(chain([0], (width for width in column_widths))))
+                self.MT.col_positions = list(accumulate(chain([0], column_widths)))
         return self
 
     def set_row_heights(
         self,
-        row_heights: Iterator[int, float] | None = None,
+        row_heights: Iterator[float] | None = None,
         canvas_positions: bool = False,
         reset: bool = False,
     ) -> Sheet:
         if reset or row_heights is None:
             self.MT.reset_row_positions()
         elif is_iterable(row_heights):
             if canvas_positions and isinstance(row_heights, list):
                 self.MT.row_positions = row_heights
             else:
-                self.MT.row_positions = list(accumulate(chain([0], (height for height in row_heights))))
+                self.MT.row_positions = list(accumulate(chain([0], row_heights)))
         return self
 
     def set_width_of_index_to_text(self, text: None | str = None, *args, **kwargs) -> Sheet:
         self.RI.set_width_of_index_to_text(text=text)
         return self
 
     def set_index_width(self, pixels: int, redraw: bool = True) -> Sheet:
@@ -3552,61 +3571,61 @@
         total_rows: int | None = None,
         total_columns: int | None = None,
     ) -> tuple[int, int] | Sheet:
         if total_rows is None and total_columns is None:
             return len(self.MT.row_positions) - 1, len(self.MT.col_positions) - 1
         if isinstance(total_rows, int):
             height = self.MT.get_default_row_height()
-            self.MT.row_positions = list(accumulate(chain([0], (height for row in range(total_rows)))))
+            self.MT.row_positions = list(accumulate(chain([0], repeat(height, total_rows))))
         if isinstance(total_columns, int):
             width = self.ops.default_column_width
-            self.MT.col_positions = list(accumulate(chain([0], (width for column in range(total_columns)))))
+            self.MT.col_positions = list(accumulate(chain([0], repeat(width, total_columns))))
         return self
 
     def move_row_position(self, row: int, moveto: int) -> Sheet:
         self.MT.move_row_position(row, moveto)
         return self
 
     def move_column_position(self, column: int, moveto: int) -> Sheet:
         self.MT.move_col_position(column, moveto)
         return self
 
     def get_example_canvas_column_widths(self, total_cols: int | None = None) -> list[float]:
         colpos = int(self.ops.default_column_width)
         if isinstance(total_cols, int):
-            return list(accumulate(chain([0], (colpos for c in range(total_cols)))))
-        return list(accumulate(chain([0], (colpos for c in range(len(self.MT.col_positions) - 1)))))
+            return list(accumulate(chain([0], repeat(colpos, total_cols))))
+        return list(accumulate(chain([0], repeat(colpos, len(self.MT.col_positions) - 1))))
 
     def get_example_canvas_row_heights(self, total_rows: int | None = None) -> list[float]:
         rowpos = self.MT.get_default_row_height()
         if isinstance(total_rows, int):
-            return list(accumulate(chain([0], (rowpos for c in range(total_rows)))))
-        return list(accumulate(chain([0], (rowpos for c in range(len(self.MT.row_positions) - 1)))))
+            return list(accumulate(chain([0], repeat(rowpos, total_rows))))
+        return list(accumulate(chain([0], repeat(rowpos, len(self.MT.row_positions) - 1))))
 
     def verify_row_heights(self, row_heights: list[float], canvas_positions: bool = False) -> bool:
         if not isinstance(row_heights, list):
             return False
         if canvas_positions:
             if row_heights[0] != 0:
                 return False
             return not any(
                 x - z < self.MT.min_row_height or not isinstance(x, int) or isinstance(x, bool)
-                for z, x in zip(islice(row_heights, 0, None), islice(row_heights, 1, None))
+                for z, x in zip(row_heights, islice(row_heights, 1, None))
             )
         return not any(z < self.MT.min_row_height or not isinstance(z, int) or isinstance(z, bool) for z in row_heights)
 
     def verify_column_widths(self, column_widths: list[float], canvas_positions: bool = False) -> bool:
         if not isinstance(column_widths, list):
             return False
         if canvas_positions:
             if column_widths[0] != 0:
                 return False
             return not any(
                 x - z < self.MT.min_column_width or not isinstance(x, int) or isinstance(x, bool)
-                for z, x in zip(islice(column_widths, 0, None), islice(column_widths, 1, None))
+                for z, x in zip(column_widths, islice(column_widths, 1, None))
             )
         return not any(
             z < self.MT.min_column_width or not isinstance(z, int) or isinstance(z, bool) for z in column_widths
         )
 
     def valid_row_height(self, height: int) -> int:
         if height < self.MT.min_row_height:
@@ -3618,14 +3637,28 @@
     def valid_column_width(self, width: int) -> int:
         if width < self.MT.min_column_width:
             return self.MT.min_column_width
         elif width > self.MT.max_column_width:
             return self.MT.max_column_width
         return width
 
+    @property
+    def visible_rows(self) -> tuple[int, int]:
+        """
+        returns: tuple[visible start row int, visible end row int]
+        """
+        return self.MT.visible_text_rows
+
+    @property
+    def visible_columns(self) -> tuple[int, int]:
+        """
+        returns: tuple[visible start column int, visible end column int]
+        """
+        return self.MT.visible_text_columns
+
     # Identifying Bound Event Mouse Position
 
     def identify_region(self, event: object) -> Literal["table", "index", "header", "top left"]:
         if event.widget == self.MT:
             return "table"
         elif event.widget == self.RI:
             return "index"
```

### Comparing `tksheet-7.2.1/tksheet/sheet_options.py` & `tksheet-7.2.2/tksheet/sheet_options.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.1/tksheet/text_editor.py` & `tksheet-7.2.2/tksheet/text_editor.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.1/tksheet/themes.py` & `tksheet-7.2.2/tksheet/themes.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.1/tksheet/top_left_rectangle.py` & `tksheet-7.2.2/tksheet/top_left_rectangle.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
     def sa_leave(self, event: object = None) -> None:
         self.itemconfig(
             self.select_all_tri,
             fill=self.PAR.ops.top_left_fg,
         )
 
-    def basic_bindings(self, enable=True) -> None:
+    def basic_bindings(self, enable: bool = True) -> None:
         if enable:
             self.bind("<Motion>", self.mouse_motion)
             self.bind("<ButtonPress-1>", self.b1_press)
             self.bind("<B1-Motion>", self.b1_motion)
             self.bind("<ButtonRelease-1>", self.b1_release)
             self.bind("<Double-Button-1>", self.double_b1)
             self.bind(rc_binding, self.rc)
@@ -152,15 +152,20 @@
             self.unbind("<Motion>")
             self.unbind("<ButtonPress-1>")
             self.unbind("<B1-Motion>")
             self.unbind("<ButtonRelease-1>")
             self.unbind("<Double-Button-1>")
             self.unbind(rc_binding)
 
-    def set_dimensions(self, new_w=None, new_h=None, recreate_selection_boxes: bool = True) -> None:
+    def set_dimensions(
+        self,
+        new_w: None | int = None,
+        new_h: None | int = None,
+        recreate_selection_boxes: bool = True,
+    ) -> None:
         try:
             if new_h is None:
                 h = self.winfo_height()
             if new_w is None:
                 w = self.winfo_width()
             if new_w:
                 self.config(width=new_w)
```

### Comparing `tksheet-7.2.1/tksheet/vars.py` & `tksheet-7.2.2/tksheet/vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.2.1/tksheet.egg-info/PKG-INFO` & `tksheet-7.2.2/tksheet.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tkinter table / sheet widget
 Author-email: ragardner <github@ragardner.simplelogin.com>
 License: Copyright (c) 2019 ragardner and open source contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -36,22 +36,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# tksheet
+<p align="center" width="100%">
+    <img width="33%" src="https://github.com/ragardner/tksheet/assets/26602401/4124c3ce-cf62-4925-9158-c5bdf712765b"> 
+</p>
+
+# <div align="center">tksheet - python tkinter table widget</div>
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.8|3.9|3.10|3.11|3.12-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt)
 
 [![GitHub Release Date](https://img.shields.io/github/release-date-pre/ragardner/tksheet.svg)](https://github.com/ragardner/tksheet/releases) [![Downloads](https://img.shields.io/pypi/dm/tksheet.svg)](https://pypi.org/project/tksheet/)
 
-### **A python tkinter table widget**
-
 |    **Help**       |                                                                  |
 |-------------------|------------------------------------------------------------------|
 | Versions 6.x.x -> | [Documentation Wiki](https://github.com/ragardner/tksheet/wiki/Version-6) | |
 | Versions 7.x.x -> | [Documentation Wiki](https://github.com/ragardner/tksheet/wiki/Version-7) | |
 | [Changelog](https://github.com/ragardner/tksheet/blob/master/docs/CHANGELOG.md) | |
 | [Questions](https://github.com/ragardner/tksheet/wiki/Version-7#asking-questions) | |
 | [Issues](https://github.com/ragardner/tksheet/wiki/Version-7#issues) | |
```

