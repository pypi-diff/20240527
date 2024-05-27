# Comparing `tmp/tkeasygui-0.2.68.tar.gz` & `tmp/tkeasygui-0.2.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkeasygui-0.2.68.tar", last modified: Sat May 11 02:55:57 2024, max compression
+gzip compressed data, was "tkeasygui-0.2.69.tar", last modified: Mon May 27 05:01:10 2024, max compression
```

## Comparing `tkeasygui-0.2.68.tar` & `tkeasygui-0.2.69.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-05-11 02:55:57.946493 tkeasygui-0.2.68/
--rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.68/LICENSE
--rw-r--r--   0 kujirahand   (501) staff       (20)     7181 2024-05-11 02:55:57.946254 tkeasygui-0.2.68/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)     4777 2024-04-27 14:17:16.000000 tkeasygui-0.2.68/README.md
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-05-11 02:55:57.944342 tkeasygui-0.2.68/TkEasyGUI/
--rw-r--r--   0 kujirahand   (501) staff       (20)      376 2024-04-20 12:19:46.000000 tkeasygui-0.2.68/TkEasyGUI/__init__.py
--rw-r--r--   0 kujirahand   (501) staff       (20)    28011 2024-04-27 13:34:47.000000 tkeasygui-0.2.68/TkEasyGUI/dialogs.py
--rw-r--r--   0 kujirahand   (501) staff       (20)     2545 2024-04-24 11:24:23.000000 tkeasygui-0.2.68/TkEasyGUI/locale_easy.py
--rw-r--r--   0 kujirahand   (501) staff       (20)     6538 2024-04-27 13:29:24.000000 tkeasygui-0.2.68/TkEasyGUI/utils.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-05-11 02:55:56.000000 tkeasygui-0.2.68/TkEasyGUI/version.py
--rw-r--r--   0 kujirahand   (501) staff       (20)   124495 2024-05-11 02:49:19.000000 tkeasygui-0.2.68/TkEasyGUI/widgets.py
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-05-11 02:55:57.945864 tkeasygui-0.2.68/TkEasyGUI.egg-info/
--rw-r--r--   0 kujirahand   (501) staff       (20)     7181 2024-05-11 02:55:57.000000 tkeasygui-0.2.68/TkEasyGUI.egg-info/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)      325 2024-05-11 02:55:57.000000 tkeasygui-0.2.68/TkEasyGUI.egg-info/SOURCES.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-05-11 02:55:57.000000 tkeasygui-0.2.68/TkEasyGUI.egg-info/dependency_links.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-05-11 02:55:57.000000 tkeasygui-0.2.68/TkEasyGUI.egg-info/requires.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-05-11 02:55:57.000000 tkeasygui-0.2.68/TkEasyGUI.egg-info/top_level.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)     1301 2024-05-11 02:50:51.000000 tkeasygui-0.2.68/pyproject.toml
--rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-05-11 02:55:57.946550 tkeasygui-0.2.68/setup.cfg
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-05-27 05:01:10.994899 tkeasygui-0.2.69/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.69/LICENSE
+-rw-r--r--   0 kujirahand   (501) staff       (20)     7347 2024-05-27 05:01:10.994616 tkeasygui-0.2.69/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)     4863 2024-05-27 04:59:03.000000 tkeasygui-0.2.69/README.md
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-05-27 05:01:10.992704 tkeasygui-0.2.69/TkEasyGUI/
+-rw-r--r--   0 kujirahand   (501) staff       (20)      376 2024-04-20 12:19:46.000000 tkeasygui-0.2.69/TkEasyGUI/__init__.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)    28613 2024-05-20 23:03:15.000000 tkeasygui-0.2.69/TkEasyGUI/dialogs.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)     2545 2024-04-24 11:24:23.000000 tkeasygui-0.2.69/TkEasyGUI/locale_easy.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)     6538 2024-04-27 13:29:24.000000 tkeasygui-0.2.69/TkEasyGUI/utils.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-05-27 05:01:08.000000 tkeasygui-0.2.69/TkEasyGUI/version.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)   131372 2024-05-21 02:27:16.000000 tkeasygui-0.2.69/TkEasyGUI/widgets.py
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-05-27 05:01:10.994133 tkeasygui-0.2.69/TkEasyGUI.egg-info/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     7347 2024-05-27 05:01:10.000000 tkeasygui-0.2.69/TkEasyGUI.egg-info/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)      325 2024-05-27 05:01:10.000000 tkeasygui-0.2.69/TkEasyGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-05-27 05:01:10.000000 tkeasygui-0.2.69/TkEasyGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-05-27 05:01:10.000000 tkeasygui-0.2.69/TkEasyGUI.egg-info/requires.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-05-27 05:01:10.000000 tkeasygui-0.2.69/TkEasyGUI.egg-info/top_level.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1371 2024-05-27 05:00:56.000000 tkeasygui-0.2.69/pyproject.toml
+-rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-05-27 05:01:10.994975 tkeasygui-0.2.69/setup.cfg
```

### Comparing `tkeasygui-0.2.68/LICENSE` & `tkeasygui-0.2.69/LICENSE`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.68/PKG-INFO` & `tkeasygui-0.2.69/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.68
+Version: 0.2.69
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
         
@@ -26,14 +26,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/kujirahand/tkeasygui-python
 Project-URL: Documentation, https://github.com/kujirahand/tkeasygui-python/blob/main/README.md
 Project-URL: Repository, https://github.com/kujirahand/tkeasygui-python/
 Project-URL: Issues, https://github.com/kujirahand/tkeasygui-python/issues
+Project-URL: Changelog, https://github.com/kujirahand/tkeasygui-python/releases
 Keywords: GUI,Tkinter,PySimpleGUI
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -44,20 +45,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Pillow
 Requires-Dist: pyperclip
 
 # TkEasyGUI
 
-`TkEasyGUI` is a Python library that allows for the easy and simple creation of GUI applications.
+`TkEasyGUI` is the easiest library for creating GUIs in Python.
 
 <img src="https://github.com/kujirahand/tkeasygui-python/raw/main/docs/image/logo-button.jpg" width="180" alt="TkEasyGUI Logo">
 
 - Python's standard UI library `Tkinter`, is often considered to have a high barrier to entry and to be difficult to use. By using this library, you can create GUI applications easily and intuitively.
 - In the event model, it is compatible with the well-known GUI library `PySimpleGUI`.
+- This package supports type hints, allowing property selection via code completion. `Python 3.9 or later` is required.
 - This project adopts the lenient MIT license. This license will not change in the future. Let's enjoy creating GUI programs.
 
 - [👉日本語](https://github.com/kujirahand/tkeasygui-python/blob/main/README-ja.md) / [👉中文](https://github.com/kujirahand/tkeasygui-python/blob/main/README-zh.md)
 
 
 ## Platform
```

### Comparing `tkeasygui-0.2.68/README.md` & `tkeasygui-0.2.69/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # TkEasyGUI
 
-`TkEasyGUI` is a Python library that allows for the easy and simple creation of GUI applications.
+`TkEasyGUI` is the easiest library for creating GUIs in Python.
 
 <img src="https://github.com/kujirahand/tkeasygui-python/raw/main/docs/image/logo-button.jpg" width="180" alt="TkEasyGUI Logo">
 
 - Python's standard UI library `Tkinter`, is often considered to have a high barrier to entry and to be difficult to use. By using this library, you can create GUI applications easily and intuitively.
 - In the event model, it is compatible with the well-known GUI library `PySimpleGUI`.
+- This package supports type hints, allowing property selection via code completion. `Python 3.9 or later` is required.
 - This project adopts the lenient MIT license. This license will not change in the future. Let's enjoy creating GUI programs.
 
 - [👉日本語](https://github.com/kujirahand/tkeasygui-python/blob/main/README-ja.md) / [👉中文](https://github.com/kujirahand/tkeasygui-python/blob/main/README-zh.md)
 
 
 ## Platform
```

### Comparing `tkeasygui-0.2.68/TkEasyGUI/dialogs.py` & `tkeasygui-0.2.69/TkEasyGUI/dialogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,14 +274,31 @@
         multiple_files: bool = False, # can select multiple files
         file_types: tuple[tuple[str, str]] = (("All Files", "*.*"),),
         no_window: Union[bool, None] = None, # for compatibility
         **kw) -> Union[str, tuple[str], None]:
     """Popup a file selection dialog. Return the file selected."""
     if title is None:
         title = message
+    if file_types is not None:
+        # check file types
+        new_types = []
+        for ft in file_types:
+            if len(ft) != 2:
+                ft = (ft, ft)
+            # fix file types for mac (#52)
+            # like ("Image Files", *.jpg;*.jpeg;*.jpe;*.heic")
+            if is_mac():
+                if ";" in ft[1]:
+                    desc = ft[0]
+                    exts = ft[1].split(";")
+                    for ext in exts:
+                        new_types.append((desc, ext))
+                    continue
+            new_types.append(ft)
+        file_types = tuple(new_types)
     if save_as:
         result = filedialog.asksaveasfilename(
             title=title,
             initialdir=initial_folder,
             filetypes=file_types,
             **kw)
     else:
```

### Comparing `tkeasygui-0.2.68/TkEasyGUI/locale_easy.py` & `tkeasygui-0.2.69/TkEasyGUI/locale_easy.py`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.68/TkEasyGUI/utils.py` & `tkeasygui-0.2.69/TkEasyGUI/utils.py`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.68/TkEasyGUI/widgets.py` & `tkeasygui-0.2.69/TkEasyGUI/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     OrientationType,
     PadType,
     PointType,
     ReliefType,
     TextAlign,
     TextVAlign,
     # Window,
-        _window_count,
+    _window_count,
     _window_parent,
     _window_pop,
     _window_push,
     generate_element_id,
     generate_element_style_key,
     get_current_theme,
     get_root_window,
@@ -132,15 +132,15 @@
         self.enable_key_events: bool = enable_key_events
         self.return_keyboard_events: bool = return_keyboard_events
         self.font_size_average: tuple[int, int] = (12, 10)
         self.row_padding: int = row_padding
         self.center_window: bool = center_window
         self.padding_x: int = padding_x
         self.padding_y: int = padding_y
-        self.show_scrollbar = show_scrollbar
+        self.show_scrollbar = show_scrollbar  # (experimental)
         # Canvas
         self.canvas: Union[tk.Canvas, None] = None
         if show_scrollbar:
             self.canvas = tk.Canvas(self.window)
             self.canvas.pack(
                 side=tk.LEFT, fill=tk.BOTH, expand=True,
                 padx=padding_x, pady=padding_y
@@ -298,19 +298,21 @@
             for elem in widgets:
                 elem.prepare_create(self)
         # create widgets
         self.need_focus_widget: tk.Widget|None = None
         for row_no, widgets in enumerate(layout):
             bgcolor = None
             if parent is not None:
-                bgcolor = parent.cget("background")
-            frame_prop = {
-                "name": f"tkeasygui_frame_row_{row_no}",
-                "background": bgcolor
-            }
+                try:
+                    bgcolor = parent.cget("background")
+                except Exception:
+                    pass
+            frame_prop = {"name": f"tkeasygui_frame_row_{row_no}"}
+            if bgcolor is not None:
+                frame_prop["background"] = bgcolor
             frame_row = tk.Frame(parent, **frame_prop)
             # columns
             prev_element: Element|None = None
             row_pack_prop: dict[str, Any] = {
                 "expand": False,
                 "fill": "x",
                 "side": valign,
@@ -330,15 +332,18 @@
                 # set prev_element and next_element
                 elem.prev_element = prev_element # set prev_element
                 if prev_element is not None:
                     prev_element.next_element = elem
                 prev_element = elem
                 # create widget
                 try:
-                    widget: tk.Widget = elem.create(self, frame_row)
+                    elem_parent = frame_row
+                    if type(parent) == ttk.Notebook:
+                        elem_parent = parent
+                    widget: tk.Widget = elem.create(self, elem_parent)
                     widget.__tkeasygui = elem # type : ignore
                 except Exception as e:
                     print(e.__traceback__, file=sys.stderr)
                     raise TkEasyError(
                         f"Window._create_widget.Failed `{elem.element_type}` key=`{elem.get_name()}` {elem.props} reason:{e}"
                     ) from e
                 # check key
@@ -364,14 +369,26 @@
                 elem.post_create(self, frame_row)
                 # bind event (before create)
                 for event_name, handle_t in elem._bind_dict.items():
                     self.bind(elem, event_name, handle_t[0], handle_t[1], handle_t[2])
                 # menu ?
                 if isinstance(elem, Menu):
                     continue
+                # Tab?
+                if isinstance(parent, ttk.Notebook):
+                    # print("@@@@ TabGroup", type(parent), type(elem.widget), elem.get())
+                    parent.add(elem.widget, text=elem.get())
+                    if isinstance(elem, Tab):
+                        group:TabGroup = parent.__tkeasygui
+                        tab: Tab = elem
+                        if group.max_rows > tab.rows:
+                            tab.rows = group.max_rows
+                        if group.max_cols > tab.cols:
+                            tab.cols = group.max_cols
+                    continue
                 # pack widget
                 fill_props = elem._get_pack_props(align, valign)
                 widget.pack(**fill_props)
                 # expand_y?
                 if elem.expand_y:
                     row_pack_prop["expand"] = True
                     row_pack_prop["fill"] = "both"
@@ -1235,14 +1252,182 @@
     
     def __getattr__(self, name):
         """Get unknown attribute."""
         if name in ["Widget"]:
             return self.widget
         return super().__getattr__(name)
 
+class Tab(Element):
+    """
+    (experimental) Tab element - Tab is used together with TabGroup.
+    **Example:**
+    ```py
+    import TkEasyGUI as sg
+    # Tab's Layout
+    tab1_layout = [[sg.Text("Tab1")], [sg.Input(key="input1")], [sg.Button("Read1")]]
+    tab2_layout = [[sg.Text("Tab2")], [sg.Input(key="input2")], [sg.Button("Read2")]]
+    # Main Layout
+    layout = [[
+        sg.TabGroup([[
+            sg.Tab("Tab title1", tab1_layout),
+            sg.Tab("Tab title2", tab2_layout),
+        ]])],
+        [sg.Button("Quit")]]
+    # create window and event loop
+    with sg.Window("Tab Demo", layout) as window:
+        for event, values in window:
+            pass
+    ```
+    """
+    def __init__(
+        self,
+        title: str,
+        layout: list[list[Element]],
+        key: str = "",
+        background_color: Union[str, None] = None,
+        vertical_alignment: TextVAlign = "top",
+        size: Union[tuple[int, int], None] = None,
+        # text props
+        text_align: Union[TextAlign, None] = "left",  # text align
+        # pack props
+        expand_x: bool = False,
+        expand_y: bool = False,
+        pad: Union[PadType, None] = None,
+        # other
+        metadata: Union[dict[str, Any], None] = None,
+        **kw,
+    ) -> None:
+        super().__init__("Tab", "Frame", key, False, metadata, **kw)
+        self.has_children = True
+        self.title = title
+        self.layout = layout
+        self.text_align = text_align
+        self.vertical_alignment = vertical_alignment
+        self.has_font_prop = False
+        self.use_ttk = False
+        self.rows = len(layout)
+        self.cols = 0
+        for row in layout:
+            self.cols = max(self.cols, len(row))
+        self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
+        if size is not None:
+            self.props["size"] = size
+        if background_color is not None:
+            self.props["background_color"] = background_color
+        if text_align is not None:
+            self.props["anchor"] = self._justify_to_anchor(text_align)
+
+    def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
+        self.widget = tk.Frame(parent, **self.props)
+        return self.widget
+
+    def get(self) -> Any:
+        """Return Widget title"""
+        return self.title
+
+    def update(self, *args, **kw) -> None:
+        """Update the widget."""
+        self._widget_update(**kw)
+
+    def __getattr__(self, name):
+        """Get unknown attribute."""
+        if name in ["Widget"]:
+            return self.widget
+        return super().__getattr__(name)
+
+
+class TabGroup(Element):
+    """
+    (experimental) TabGroup element - Specify the Tab element for the child elements.
+
+    **Example:**
+    ```py
+    import TkEasyGUI as sg
+    # Tab's Layout
+    tab1_layout = [[sg.Text("Tab1")], [sg.Input(key="input1")], [sg.Button("Read1")]]
+    tab2_layout = [[sg.Text("Tab2")], [sg.Input(key="input2")], [sg.Button("Read2")]]
+    # Main Layout
+    layout = [[
+        sg.TabGroup([[
+            sg.Tab("Tab title1", tab1_layout),
+            sg.Tab("Tab title2", tab2_layout),
+        ]])],
+        [sg.Button("Quit")]]
+    # create window and event loop
+    with sg.Window("Tab Demo", layout) as window:
+        for event, values in window:
+            pass
+    ```
+    """
+    def __init__(
+        self,
+        layout: Union[list[list["TabGroup"]], list["TabGroup"]],
+        key: str = "",
+        background_color: Union[str, None] = None,
+        vertical_alignment: TextVAlign = "top",
+        size: Union[tuple[int, int], None] = None,
+        # text props
+        text_align: Union[TextAlign, None] = "left",  # text align
+        # pack props
+        expand_x: bool = True,
+        expand_y: bool = True,
+        pad: Union[PadType, None] = None,
+        # other
+        metadata: Union[dict[str, Any], None] = None,
+        **kw,
+    ) -> None:
+        super().__init__("TabGroup", "Notebook", key, False, metadata, **kw)
+        self.has_children = True
+        # check layout type
+        if layout is None:
+            layout = []
+        if len(layout) > 0:
+            if not isinstance(layout[0], list):
+                layout = [layout]
+            if not isinstance(layout[0][0], Tab):
+                raise ValueError("TabGroup layout should be list of Tab")
+        self.layout = layout
+        self.text_align = text_align
+        self.vertical_alignment = vertical_alignment
+        self.has_font_prop = False
+        self.use_ttk = True
+        self.background_color = background_color
+        self.max_rows = 3
+        self.max_cols = 3
+        self.window = None
+        self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
+        if text_align is not None:
+            self.props["anchor"] = self._justify_to_anchor(text_align)
+
+    def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
+        self.window = win
+        self.widget = ttk.Notebook(parent, **self.props)
+        return self.widget
+    
+    def post_create(self, win: Window, parent: tk.Widget) -> None:
+        if win.size is None:
+            win.set_size((600, 400))
+        return super().post_create(win, parent)
+
+    def get(self) -> Any:
+        """Return Widget"""
+        return self.widget
+
+    def update(self, *args, **kw) -> None:
+        """Update the widget."""
+        self._widget_update(**kw)
+
+    def __getattr__(self, name):
+        """Get unknown attribute."""
+        if name in ["Widget"]:
+            return self.widget
+        return super().__getattr__(name)
+
+
+
 class Text(Element):
     """Text element."""
     def __init__(
                 self,
                 text: str = "",
                 key: Union[str, None] = None,
                 enable_events: bool=False, # enabled events (click)
@@ -1400,15 +1585,29 @@
     def update(self, text: Union[str, None] = None, *args, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.set_text(text)
         self._widget_update(**kw)
 
 class Button(Element):
-    """Button element."""
+    """
+        Button element
+
+        **Example**
+        The program below changes the button's label to "Pushed" when the button is pressed.
+        ```python
+        import TkEasyGUI as eg
+        button:eg.Button = eg.Button("Push me")
+        with eg.Window("Title", layout=[[button]]) as window:
+            for event, values in window.event_iter():
+                if event == button.get_text():
+                    button.set_text("Pushed")
+                    break
+        ```
+    """
     def __init__(
         self,
         button_text: str = "",
         key: Union[str, None] = None,
         disabled: bool = None,
         size: Union[tuple[int, int], None] = None,
         tooltip: Union[str, None] = None,  # (TODO) tooltip
```

### Comparing `tkeasygui-0.2.68/TkEasyGUI.egg-info/PKG-INFO` & `tkeasygui-0.2.69/TkEasyGUI.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.68
+Version: 0.2.69
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
         
@@ -26,14 +26,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/kujirahand/tkeasygui-python
 Project-URL: Documentation, https://github.com/kujirahand/tkeasygui-python/blob/main/README.md
 Project-URL: Repository, https://github.com/kujirahand/tkeasygui-python/
 Project-URL: Issues, https://github.com/kujirahand/tkeasygui-python/issues
+Project-URL: Changelog, https://github.com/kujirahand/tkeasygui-python/releases
 Keywords: GUI,Tkinter,PySimpleGUI
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -44,20 +45,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Pillow
 Requires-Dist: pyperclip
 
 # TkEasyGUI
 
-`TkEasyGUI` is a Python library that allows for the easy and simple creation of GUI applications.
+`TkEasyGUI` is the easiest library for creating GUIs in Python.
 
 <img src="https://github.com/kujirahand/tkeasygui-python/raw/main/docs/image/logo-button.jpg" width="180" alt="TkEasyGUI Logo">
 
 - Python's standard UI library `Tkinter`, is often considered to have a high barrier to entry and to be difficult to use. By using this library, you can create GUI applications easily and intuitively.
 - In the event model, it is compatible with the well-known GUI library `PySimpleGUI`.
+- This package supports type hints, allowing property selection via code completion. `Python 3.9 or later` is required.
 - This project adopts the lenient MIT license. This license will not change in the future. Let's enjoy creating GUI programs.
 
 - [👉日本語](https://github.com/kujirahand/tkeasygui-python/blob/main/README-ja.md) / [👉中文](https://github.com/kujirahand/tkeasygui-python/blob/main/README-zh.md)
 
 
 ## Platform
```

### Comparing `tkeasygui-0.2.68/pyproject.toml` & `tkeasygui-0.2.69/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TkEasyGUI"
-version = "0.2.68"
+version = "0.2.69"
 dependencies = [
   "Pillow",
   "pyperclip",
 ]
 requires-python = ">=3.9"
 authors = [
   { name="kujirahand", email="web@kujirahand.com" },
@@ -33,11 +33,12 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/kujirahand/tkeasygui-python"
 Documentation = "https://github.com/kujirahand/tkeasygui-python/blob/main/README.md"
 Repository = "https://github.com/kujirahand/tkeasygui-python/"
 Issues = "https://github.com/kujirahand/tkeasygui-python/issues"
+Changelog = "https://github.com/kujirahand/tkeasygui-python/releases"
 
 [tool.ruff.lint]
 select = ["E", "F", "I"]
 ignore = ["E501"]
```

