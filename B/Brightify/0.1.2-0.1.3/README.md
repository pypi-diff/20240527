# Comparing `tmp/brightify-0.1.2.tar.gz` & `tmp/brightify-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightify-0.1.2.tar", last modified: Thu May 23 18:37:13 2024, max compression
+gzip compressed data, was "brightify-0.1.3.tar", last modified: Mon May 27 07:40:38 2024, max compression
```

## Comparing `brightify-0.1.2.tar` & `brightify-0.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.515554 brightify-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.515554 brightify-0.1.2/Brightify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-23 18:37:13.000000 brightify-0.1.2/Brightify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-23 18:37:13.000000 brightify-0.1.2/Brightify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:37:13.000000 brightify-0.1.2/Brightify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-23 18:37:13.000000 brightify-0.1.2/Brightify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 18:37:13.000000 brightify-0.1.2/Brightify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-23 18:37:08.000000 brightify-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-23 18:37:13.515554 brightify-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-23 18:37:08.000000 brightify-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.511554 brightify-0.1.2/brightify/
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/BaseApp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/Brightylog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/SensorComm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/UIConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.511554 brightify-0.1.2/brightify/linux/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/linux/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/log_config.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.511554 brightify-0.1.2/brightify/monitors/
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/monitors/MonitorBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/monitors/MonitorDDCCI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/monitors/MonitorGeneric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/monitors/MonitorUSB.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/monitors/m27q.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.511554 brightify-0.1.2/brightify/res/
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/res/icon_dark.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/res/icon_light.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.511554 brightify-0.1.2/brightify/sensor_firmware/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/sensor_firmware/platformio.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.511554 brightify-0.1.2/brightify/sensor_firmware/src/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/sensor_firmware/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:37:13.515554 brightify-0.1.2/brightify/windows/
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/windows/WindowsApp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/windows/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/windows/add_startup_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/windows/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 18:37:08.000000 brightify-0.1.2/brightify/windows/remove_startup_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-23 18:37:08.000000 brightify-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:37:13.515554 brightify-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.310752 brightify-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.310752 brightify-0.1.3/Brightify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-27 07:40:38.000000 brightify-0.1.3/Brightify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-27 07:40:38.000000 brightify-0.1.3/Brightify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:40:38.000000 brightify-0.1.3/Brightify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 07:40:38.000000 brightify-0.1.3/Brightify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 07:40:38.000000 brightify-0.1.3/Brightify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-27 07:40:30.000000 brightify-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-27 07:40:38.310752 brightify-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-27 07:40:30.000000 brightify-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.306752 brightify-0.1.3/brightify/
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/BaseApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/SensorComm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/brightylog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.306752 brightify-0.1.3/brightify/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/linux/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/log_config.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.306752 brightify-0.1.3/brightify/monitors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/monitors/MonitorBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/monitors/MonitorDDCCI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/monitors/MonitorUSB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/monitors/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/monitors/m27q.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.310752 brightify-0.1.3/brightify/res/
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/res/icon_dark.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/res/icon_light.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.310752 brightify-0.1.3/brightify/sensor_firmware/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/sensor_firmware/platformio.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.310752 brightify-0.1.3/brightify/sensor_firmware/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/sensor_firmware/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/ui_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:40:38.310752 brightify-0.1.3/brightify/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/windows/WindowsApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/windows/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/windows/add_startup_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/windows/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-27 07:40:30.000000 brightify-0.1.3/brightify/windows/remove_startup_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-27 07:40:30.000000 brightify-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:40:38.310752 brightify-0.1.3/setup.cfg
```

### Comparing `brightify-0.1.2/Brightify.egg-info/PKG-INFO` & `brightify-0.1.3/Brightify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Brightify
-Version: 0.1.2
+Version: 0.1.3
 Summary: Brightify is an OS-independent application that adjusts monitor brightness using the DDC/CI protocol and custom protocols for USB monitors, featuring a brightness sensor for automatic adjustments based on ambient light, and can be controlled via a taskbar icon.
 Author-email: "Robin S." <brightify@rs-web.net>
 Keywords: brightness,monitor,screen,control,tool
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: platformio
 Requires-Dist: pyserial
```

### Comparing `brightify-0.1.2/PKG-INFO` & `brightify-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Brightify
-Version: 0.1.2
+Version: 0.1.3
 Summary: Brightify is an OS-independent application that adjusts monitor brightness using the DDC/CI protocol and custom protocols for USB monitors, featuring a brightness sensor for automatic adjustments based on ambient light, and can be controlled via a taskbar icon.
 Author-email: "Robin S." <brightify@rs-web.net>
 Keywords: brightness,monitor,screen,control,tool
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: platformio
 Requires-Dist: pyserial
```

### Comparing `brightify-0.1.2/README.md` & `brightify-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `brightify-0.1.2/brightify/BaseApp.py` & `brightify-0.1.3/brightify/BaseApp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,112 +1,46 @@
+import logging
 import threading
-from typing import List, Tuple, Type, Callable, Generator, Optional, Literal, Dict, Any
+from typing import List, Tuple, Type, Callable, Generator, Literal, Any
 
 from PyQt6 import QtCore
-from PyQt6.QtCore import QPoint, Qt, QRect, QPropertyAnimation, QTimer, QThread
-from PyQt6.QtGui import QFocusEvent, QCursor, QRegion, QPainterPath
-from PyQt6.QtWidgets import QMainWindow, QWidget, QVBoxLayout
+from PyQt6.QtCore import QPoint, Qt, QRect, QPropertyAnimation, QTimer, QThread, QObject, QEvent, QEasingCurve
+from PyQt6.QtGui import QFocusEvent, QCursor
+from PyQt6.QtWidgets import QMainWindow, QWidget, QVBoxLayout, QApplication, QLabel, QPushButton
 
 from brightify import app_name, root_dir
 from brightify.SensorComm import SensorComm
-from brightify.UIConfig import UIConfig, Theme
-from brightify.UIConfig import MonitorRow
-
-import logging
-
+from brightify.monitors.finder import get_supported_monitors
+from brightify.ui_config import MonitorRow
+from brightify.ui_config import UIConfig, Theme
 from brightify.monitors.MonitorBase import MonitorBase
 from brightify.monitors.MonitorDDCCI import MonitorDDCCI
 from brightify.monitors.MonitorUSB import MonitorUSB
 
 # use global logger
 logger = logging.getLogger(app_name)
 
 
-def _supported_usb_impls() -> List[Type[MonitorUSB]]:
-    """
-    Finds all user implemented MonitorUSB classes in the monitors directory.
-    :return: a list of all MonitorUSB implementations
-    """
-    import os, importlib, inspect
-    monitor_impls = set()
-    directory = "monitors"
-    for filename in os.listdir(root_dir / directory):
-        if not filename.endswith(".py"):
-            continue
-        module_name = filename.replace(".py", "")
-        full_module_name = f"{__package__}.{directory}.{module_name}"
-        try:
-            module = importlib.import_module(full_module_name)
-            for name, obj in inspect.getmembers(module):
-                if inspect.isclass(obj) and issubclass(obj, MonitorUSB) and obj is not MonitorUSB:
-                    monitor_impls.add(obj)
-        except ImportError:
-            pass
-    return list(monitor_impls)
-
-
-def _usb_monitors(monitor_impls: List[Type[MonitorUSB]]) -> List[MonitorUSB]:
-    """
-    Finds all USB devices connected to the system and instantiates the corresponding MonitorUSB classes.
-    :param monitor_impls: a list of all MonitorUSB implementations
-    :return: a list of all MonitorUSB implementations with a connected USB device
-    """
-    import usb1
-    context = usb1.USBContext()
-    devices = context.getDeviceList(skip_on_error=True)
-    monitor_inst: List[Tuple[Type[MonitorUSB], usb1.USBDevice]] = []
-    for dev in devices:
-        for impl in monitor_impls:
-            if impl.vid() == dev.getVendorID() and impl.pid() == dev.getProductID():
-                monitor_inst.append((impl, dev))
-                break
-
-    return [impl(dev) for impl, dev in monitor_inst]
-
-
-def _ddcci_monitors() -> List[MonitorDDCCI]:
-    """
-    Finds all monitors connected to the system and instantiates the MonitorDDCCI class.
-    :return: a list of all MonitorDDCCI implementations
-    """
-    import monitorcontrol
-    monitors = monitorcontrol.get_monitors()
-    return [MonitorDDCCI(monitor) for monitor in monitors]
-
-
-def get_supported_monitors() -> List[MonitorBase]:
-    """
-    Finds all user implemented MonitorUSB classes and instantiates them with the corresponding USB device.
-    If a monitor without a USB device is found or an implementation is missing, we try to connect to the monitor via DDC-CI.
-    :return: a list of all MonitorBase implementations
-    """
-    monitor_impls = _supported_usb_impls()
-    usb_monitors = _usb_monitors(monitor_impls)
-    logger.info(f"Found {len(usb_monitors)} USB monitor(s) with implementation: {[m.name() for m in usb_monitors]}")
-    ddcci_monitors = _ddcci_monitors()
-    logger.info(f"Found {len(ddcci_monitors)} DDCCI monitor(s)")
-    return usb_monitors + ddcci_monitors
-
-
 class BaseApp(QMainWindow):
     """
     The main application window that contains all MonitorRows.
     """
 
     def __init__(self, theme_cb: Callable[[], Theme], parent=None):
         super(BaseApp, self).__init__(parent, Qt.WindowType.Tool)
 
         # The rows contain one MonitorRow for each supported Monitor connected
         self.rows: QVBoxLayout = QVBoxLayout()
         self.central_widget = QWidget(self)
         self.central_widget.setLayout(self.rows)
         self.setCentralWidget(self.central_widget)
 
+        # Lock for animations, rapid clicks can cause multiple animations to run at the same time
         self.__anim_lock: threading.Lock = threading.Lock()
-        # Store the top left corner given by the OS
+        # Store the top left corner given by the OS to be used to position the window
         self.__top_left: QPoint | None = None
         self.__get_theme = theme_cb
         self.__ui_config: UIConfig = UIConfig()
         self.__sensor_comm = SensorComm()
 
         # Start timer that reads sensor data every 500ms
         self.__sensor_thread = QThread()
@@ -123,14 +57,17 @@
         self.fade_up_animation.finished.connect(self.setFocus)
 
         self.fade_down_animation = QPropertyAnimation(self, b"geometry")
         self.fade_down_animation.finished.connect(self.__anim_lock.release)
         self.fade_down_animation.finished.connect(self.clearFocus)
         self.fade_down_animation.finished.connect(self.hide)
 
+        # Install event filter on the application to detect when the window loses focus
+        QApplication.instance().installEventFilter(self)
+
     @property
     def top_left(self) -> QPoint | None:
         return self.__top_left
 
     @top_left.setter
     def top_left(self, value: QPoint | Tuple[int, int] | Any):
         if isinstance(value, tuple):
@@ -142,17 +79,17 @@
     @property
     def ui_config(self) -> UIConfig:
         return self.__ui_config
 
     def __config_layout(self):
         self.setWindowTitle(app_name)
         self.setWindowFlags(self.windowFlags() | QtCore.Qt.WindowType.FramelessWindowHint)
-        self.rows.setContentsMargins(self.ui_config.pad_horizontal, self.ui_config.pad_vertical,
-                                     self.ui_config.pad_horizontal, self.ui_config.pad_vertical)
-        self.rows.setSpacing(self.ui_config.pad_horizontal)
+        self.rows.setContentsMargins(self.ui_config.pad, self.ui_config.pad,
+                                     self.ui_config.pad, self.ui_config.pad)
+        self.rows.setSpacing(self.ui_config.pad)
 
     @staticmethod
     def __config_slider(row: MonitorRow):
         def on_change(value):
             row.brightness_label.setText(f"{value}%")
 
         row.slider.valueChanged.connect(lambda value: on_change(value))
@@ -206,26 +143,45 @@
 
     def clear_rows(self):
         while self.rows.count():
             widget = self.rows.takeAt(0).widget()
             if isinstance(widget, MonitorRow):
                 if widget.monitor is not None:
                     widget.monitor.__del__()  # delete the monitor object
-            if widget is not None:
-                widget.deleteLater()
+                self.rows.removeWidget(widget)
+                widget.hide()  # hide the widget
+                widget.deleteLater()  # schedule the widget for deletion
+
+    def run_once(self, animation: QPropertyAnimation, finished: Callable[[], Any]):
+        def run_and_disconnect():
+            finished()
+            animation.finished.disconnect(run_and_disconnect)
+
+        animation.finished.connect(run_and_disconnect)
+
+    def __add_reload_button(self):
+
+        # add a reload button to the top of self.rows
+        reload_button = QPushButton("Reload", self)
+        reload_button.clicked.connect(lambda: self.change_state("hide"))
+        reload_button.clicked.connect(lambda: self.run_once(self.fade_down_animation, self.redraw))
+        reload_button.setStyleSheet(self.ui_config.button_style)
+        self.rows.addWidget(reload_button)
 
     def __load_rows(self):
         self.clear_rows()
         max_name_width = 0
         max_type_width = 0
         monitors: List[MonitorBase] = get_supported_monitors()
         if not monitors:
             logger.warning("No monitors were found - try to reconnect the monitor")
             return
 
+        self.__add_reload_button()
+
         for m in monitors:
             logger.info(f"Adding monitor: {m.name()}")
             row = MonitorRow(self.ui_config.theme, parent=self)
             row.slider.setRange(m.min_brightness, m.max_brightness)
             row.name_label.setText(m.name())
             self.__config_slider(row)
             self.__connect_monitor(row, m)
@@ -244,40 +200,39 @@
         if self.ui_config.theme == theme:
             logger.debug("No theme update needed")
             return
         self.ui_config.theme = theme
         logger.debug(f"Theme updated to: {theme}")
 
     def redraw(self):
+        if self.top_left is None:
+            logger.warning("Top left corner not set, cannot position the window. Using default position.")
+            screen = QApplication.primaryScreen().availableGeometry()
+            self.top_left = QPoint(screen.width() // 2, screen.height() // 2)
         logger.debug("Redrawing the app")
-        self.change_state("hide")
         self.__update_theme()
         self.__config_layout()
         self.setStyleSheet(self.ui_config.style_sheet)
         self.__load_rows()
-        # The OS must set the top left corner, and invoke this function
         self.move(self.top_left)
         # start the sensor thread if it is not running
         if not self.__sensor_thread.isRunning():
             logger.debug("Starting sensor thread")
             self.__sensor_thread.start()
         # start the sensor timer if it is not running
         if not self.__sensor_timer.isActive():
             logger.debug("Starting sensor timer")
             self.__sensor_timer.start(250)
 
-    # catch outside clicks, which should change the state of the window to hide
-    def focusOutEvent(self, event: QFocusEvent):
-        # get the position of the cursor and check if it is outside the window
-        if event.lostFocus():
-            if not self.geometry().contains(QCursor.pos()):
-                self.change_state("hide")
-                return
-
-        super().focusOutEvent(event)
+    def eventFilter(self, obj: QObject, event: QEvent) -> bool:
+        if event.type() == QEvent.Type.WindowDeactivate and obj is self:
+            # The application window has lost focus
+            self.change_state("hide")
+            return True  # Event was handled
+        return super().eventFilter(obj, event)
 
     def change_state(self, new_state: Literal["show", "hide", "invert"] = "invert"):
         if self.top_left is None:
             logger.error("Top left corner not set")
             return
         # prevent multiple animations
         if self.__anim_lock.locked():
@@ -302,10 +257,7 @@
             self.fade_up_animation.start()
         else:
             logger.debug(f"Hiding window")
             self.ui_config.config_fade_animation(self.fade_down_animation, up, down)
             self.fade_down_animation.start()
 
         self.updateGeometry()
-
-    def show(self):
-        super().show()
```

### Comparing `brightify-0.1.2/brightify/Brightylog.py` & `brightify-0.1.3/brightify/brightylog.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.2/brightify/SensorComm.py` & `brightify-0.1.3/brightify/SensorComm.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.2/brightify/UIConfig.py` & `brightify-0.1.3/brightify/ui_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,16 +107,15 @@
 
 @dataclasses.dataclass
 class UIConfig:
     # Theme
     theme: Theme = dataclasses.field(default_factory=Theme)
 
     # Layout:
-    pad_horizontal: int = 5
-    pad_vertical: int = 25
+    pad: int = 5
 
     # The maximum width of the label in the MonitorRow, or -1 if unbounded
     max_label_width: int = -1
 
     # Icon
     _icon_path: Path = dataclasses.field(default=icon_light)
 
@@ -129,14 +128,27 @@
     @property
     def style_sheet(self):
         return f"""
             background-color: {self.theme.bg_color};
             color: {self.theme.text_color};
         """
 
+    @property
+    def button_style(self):
+        return f"""
+            QPushButton {{
+                background-color: {self.theme.accent_color};
+                color: {self.theme.text_color}; 
+                font-family: {self.theme.font};
+                font-size: {self.theme.font_size}px;
+                border: 1px solid {self.theme.accent_color};
+                border-radius: 5px;
+                padding: 5px;
+            }}
+        """
     def config_fade_animation(self, fa: QPropertyAnimation,
                               start_geometry: QtCore.QRect,
                               end_geometry: QtCore.QRect):
         fa.setDuration(self.animation_duration)
         fa.setEasingCurve(QEasingCurve.Type.Linear)
         fa.setStartValue(start_geometry)
         fa.setEndValue(end_geometry)
```

### Comparing `brightify-0.1.2/brightify/__main__.py` & `brightify-0.1.3/brightify/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import argparse
 from pathlib import Path
 
 from PyQt6.QtWidgets import QApplication
 
 from brightify import app_name, host_os, root_dir
 from brightify.BaseApp import BaseApp
-from brightify.Brightylog import configure_logging, start_logging
+from brightify.brightylog import configure_logging, start_logging
 
 # use global logger
 logger = logging.getLogger(app_name)
 
 
 def excepthook(exc_type, exc_value, exc_tb):
     if exc_type is KeyboardInterrupt:
@@ -43,14 +43,15 @@
     base_app.top_left = (0, 0)
     base_app.redraw()
     base_app.show()
     ret_code = app.exec()
     logger.info(f"Exiting with code {ret_code}")
     exit(ret_code)
 
+
 def main_darwin():
     raise NotImplementedError("MacOS not supported yet")
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description=app_name)
     subparsers = parser.add_subparsers(dest="command", help="The command to run. Defaults to 'run' if not specified.")
```

### Comparing `brightify-0.1.2/brightify/linux/helpers.py` & `brightify-0.1.3/brightify/linux/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 from typing import Literal
 
 from brightify import host_os
-from brightify.UIConfig import Theme
+from brightify.ui_config import Theme
 
 # Use OS specific logger
 logger = logging.getLogger("Linux")
 
 if host_os != "Linux":
     raise RuntimeError("This code is designed to run on Linux only")
```

### Comparing `brightify-0.1.2/brightify/log_config.toml` & `brightify-0.1.3/brightify/log_config.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 version = 1
 disable_existing_loggers = false
 
 [filters.warning_and_above]
-"()" = "brightify.Brightylog.WarningAndAbove"
+"()" = "brightify.brightylog.WarningAndAbove"
 
 [filters.info_and_below]
-"()" = "brightify.Brightylog.InfoAndBelow"
+"()" = "brightify.brightylog.InfoAndBelow"
 
 [formatters.console]
 format = "[%(levelname)s]: %(message)s [%(name)s @ %(asctime)s]"
 
 [formatters.json]
-"()" = "brightify.Brightylog.Brightylog"
+"()" = "brightify.brightylog.Brightylog"
 
 [formatters.json.fmt_keys]
 level = "levelname"
 message = "message"
 timestamp = "timestamp"
 logger = "name"
 module = "module"
@@ -42,15 +42,15 @@
 filters = ["info_and_below"]  # Don't log Info and below in file
 filename = "brightify.log.jsonl"
 maxBytes = 10485760 # 10MB
 backupCount = 5
 
 
 [handlers.queue_handler]
-class = "brightify.Brightylog.BrightyQueueHandler"
+class = "brightify.brightylog.BrightyQueueHandler"
 handlers = ["jsonfile", "stdout", "stderr"]
 respect_handler_level = true
 
 
 [loggers.root]
 level = "DEBUG"  # progate everything to root
 handlers = ["queue_handler"]
```

### Comparing `brightify-0.1.2/brightify/monitors/MonitorBase.py` & `brightify-0.1.3/brightify/monitors/MonitorBase.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.2/brightify/monitors/MonitorDDCCI.py` & `brightify-0.1.3/brightify/monitors/MonitorDDCCI.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.2/brightify/monitors/MonitorUSB.py` & `brightify-0.1.3/brightify/monitors/MonitorUSB.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,19 +3,16 @@
 import time
 from abc import abstractmethod
 from typing import Optional
 
 import usb1
 import atexit
 
-from brightify import app_name
 from brightify.monitors.MonitorBase import MonitorBase
-
-
-logger = logging.getLogger(app_name)
+from brightify.monitors.MonitorBase import logger
 
 
 class MonitorUSB(MonitorBase):
     def __init__(self, device: usb1.USBDevice, usb_delay_ms: Optional[float] = 25):
 
         if device.getProductID() != self.pid() or device.getVendorID() != self.vid():
             logger.warning("The device passed is not this monitor!")
```

### Comparing `brightify-0.1.2/brightify/monitors/m27q.py` & `brightify-0.1.3/brightify/monitors/m27q.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.2/brightify/res/icon_dark.ico` & `brightify-0.1.3/brightify/res/icon_dark.ico`

 * *Files identical despite different names*

### Comparing `brightify-0.1.2/brightify/res/icon_light.ico` & `brightify-0.1.3/brightify/res/icon_light.ico`

 * *Files identical despite different names*

### Comparing `brightify-0.1.2/brightify/windows/WindowsApp.py` & `brightify-0.1.3/brightify/windows/WindowsApp.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.2/brightify/windows/actions.py` & `brightify-0.1.3/brightify/windows/actions.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.2/brightify/windows/add_startup_task.py` & `brightify-0.1.3/brightify/windows/add_startup_task.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.2/brightify/windows/helpers.py` & `brightify-0.1.3/brightify/windows/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import Literal
 
 from brightify import host_os
-from brightify.UIConfig import Theme
+from brightify.ui_config import Theme
 
 if host_os != "Windows":
     raise RuntimeError("This code is designed to run on Windows only")
 try:
     import win32con, win32api, win32gui, win32ui, winerror, winreg
 except ModuleNotFoundError:
     raise RuntimeError("This code is designed to run with pywin32")
```

### Comparing `brightify-0.1.2/brightify/windows/remove_startup_task.py` & `brightify-0.1.3/brightify/windows/remove_startup_task.py`

 * *Files identical despite different names*

### Comparing `brightify-0.1.2/pyproject.toml` & `brightify-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Brightify"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name = "Robin S.", email = "brightify@rs-web.net" }
 ]
 description = "Brightify is an OS-independent application that adjusts monitor brightness using the DDC/CI protocol and custom protocols for USB monitors, featuring a brightness sensor for automatic adjustments based on ambient light, and can be controlled via a taskbar icon."
 
 requires-python = ">= 3.11"
```

