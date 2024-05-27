# Comparing `tmp/tabswitcher-0.0.8.tar.gz` & `tmp/tabswitcher-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabswitcher-0.0.8.tar", last modified: Sat May 25 21:40:28 2024, max compression
+gzip compressed data, was "tabswitcher-0.1.0.tar", last modified: Mon May 27 00:42:31 2024, max compression
```

## Comparing `tabswitcher-0.0.8.tar` & `tabswitcher-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:40:28.908347 tabswitcher-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-25 21:40:28.908347 tabswitcher-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 21:40:28.908347 tabswitcher-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:40:28.904347 tabswitcher-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:40:28.904347 tabswitcher-0.0.8/src/tabswitcher/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/NetworkImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/SearchInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/TabList.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:40:28.908347 tabswitcher-0.0.8/src/tabswitcher/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/assets/Icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/assets/brotab_service.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/assets/install.bat
--rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/assets/sans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/assets/searchIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/assets/tabswitcher_service.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/brotab.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/fuzzySearch.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/loadBookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-25 21:40:24.000000 tabswitcher-0.0.8/src/tabswitcher/logTabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:40:28.908347 tabswitcher-0.0.8/tabswitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-25 21:40:28.000000 tabswitcher-0.0.8/tabswitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-25 21:40:28.000000 tabswitcher-0.0.8/tabswitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 21:40:28.000000 tabswitcher-0.0.8/tabswitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-25 21:40:28.000000 tabswitcher-0.0.8/tabswitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-25 21:40:28.000000 tabswitcher-0.0.8/tabswitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 21:40:28.000000 tabswitcher-0.0.8/tabswitcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:42:31.548689 tabswitcher-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-27 00:42:31.548689 tabswitcher-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 00:42:31.548689 tabswitcher-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:42:31.544689 tabswitcher-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:42:31.544689 tabswitcher-0.1.0/src/tabswitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/NetworkImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/SearchInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/TabList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/VisibilityChecker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:42:31.548689 tabswitcher-0.1.0/src/tabswitcher/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/assets/Icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/assets/install.bat
+-rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/assets/sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/assets/searchIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/assets/tabswitcher_service.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/brotab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/focusWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/fuzzySearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/loadBookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/logTabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 00:42:27.000000 tabswitcher-0.1.0/src/tabswitcher/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:42:31.548689 tabswitcher-0.1.0/tabswitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-27 00:42:31.000000 tabswitcher-0.1.0/tabswitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-27 00:42:31.000000 tabswitcher-0.1.0/tabswitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 00:42:31.000000 tabswitcher-0.1.0/tabswitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-27 00:42:31.000000 tabswitcher-0.1.0/tabswitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 00:42:31.000000 tabswitcher-0.1.0/tabswitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 00:42:31.000000 tabswitcher-0.1.0/tabswitcher.egg-info/top_level.txt
```

### Comparing `tabswitcher-0.0.8/LICENCE` & `tabswitcher-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.8/setup.py` & `tabswitcher-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tabswitcher',
-    version='0.0.8',
+    version='0.1.0',
     packages=['tabswitcher'],
     package_dir={'tabswitcher': 'src/tabswitcher'},
     package_data={'tabswitcher': ['assets/*']},
     description="A tool for efficient browser tab switching outside the browser",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='YukiGasai',
@@ -19,15 +19,14 @@
     },
     license='AGPL-3.0',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Operating System :: Microsoft :: Windows'
     ],
```

### Comparing `tabswitcher-0.0.8/src/tabswitcher/SearchInput.py` & `tabswitcher-0.1.0/src/tabswitcher/SearchInput.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.8/src/tabswitcher/Settings.py` & `tabswitcher-0.1.0/src/tabswitcher/Settings.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.8/src/tabswitcher/Tab.py` & `tabswitcher-0.1.0/src/tabswitcher/Tab.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,19 @@
 class Tab:
     def __init__(self, id, title, url, manager):
         self.id = id
         self.title = title
         self.url = url
         self.icon = f"https://t0.gstatic.com/faviconV2?client=SOCIAL&type=FAVICON&fallback_opts=TYPE,SIZE,URL&url={get_domain(url)}&size=64"
         self.item = QListWidgetItem(self.title)
-        self.networkImage = NetworkImage(manager)
-        self.networkImage.download(self.icon, self.item)
-        self.item.setData(Qt.UserRole, self.id)
+        self.item.setData(Qt.UserRole, (self.id, self.title, self.url))
+        try:
+            self.networkImage = NetworkImage(manager)
+            self.networkImage.download(self.icon, self.item)
+        except Exception as e:
+            print(f"Error creating bookmark: {self.icon}, error: {e}")
 
     def __str__(self):
         return f"{self.id} - {self.title} - {self.url}"
 
     def __repr__(self):
         return f"{self.id} - {self.title} - {self.url}"
```

### Comparing `tabswitcher-0.0.8/src/tabswitcher/TabList.py` & `tabswitcher-0.1.0/src/tabswitcher/TabList.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from PyQt5.QtCore import Qt
 from PyQt5.QtWidgets import QListWidget
 
+from tabswitcher.actions import activate_tab
+
 from .colors import getBackgroundColor, getSelectedColor, getTextColor
 
 
 class TabList(QListWidget):
     def __init__(self, parent=None):
         super(TabList, self).__init__(parent)
 
         self.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
         self.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
         # Connect the itemClicked signal to the parent's activate_tab method
-        self.itemClicked.connect(parent.activate_tab)
+        self.itemClicked.connect(lambda item: activate_tab(parent, item))
         self.setStyleSheet("""
     QListWidget {
         border: none;
         font-size: 18px;
         color: %s;
         background: transparent;       
         height: 500px;
```

### Comparing `tabswitcher-0.0.8/src/tabswitcher/__main__.py` & `tabswitcher-0.1.0/src/tabswitcher/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import os
 import pickle
 
 import sys
-import time
-from PyQt5.QtGui import QFont, QCursor, QKeySequence, QDesktopServices, QIcon
-from PyQt5.QtCore import Qt, QUrl, QThread, pyqtSignal
-from PyQt5.QtWidgets import QApplication, QWidget, QVBoxLayout, QShortcut
+from PyQt5.QtGui import QFont, QCursor, QDesktopServices, QIcon
+from PyQt5.QtCore import Qt, QUrl
+from PyQt5.QtWidgets import QApplication, QWidget, QVBoxLayout
 from PyQt5.QtNetwork import QNetworkAccessManager
 import subprocess
 
+import pkg_resources
+
+from tabswitcher.Tab import Tab
+from tabswitcher.VisibilityChecker import VisibilityChecker
+from tabswitcher.actions import activate_tab, open_settings, openFirstGoogleResult, searchGoogeInNewTab
+from tabswitcher.loadBookmarks import load_bookmarks
+from tabswitcher.shortcuts import setup_shortcuts
+
 from .SearchInput import SearchInput
 from .Settings import Settings
 from .TabList import TabList
-from .brotab import delete_tab, get_tabs, seach_tab, switch_tab
+from .brotab import delete_tab, get_tabs, seach_tab
 from .colors import getWindowBackgroundColor
 from .fuzzySearch import fuzzy_search_cmd, fuzzy_search_py
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 settings = Settings()
 
 config_dir = os.path.expanduser('~/.tabswitcher')
@@ -26,212 +33,254 @@
 
     @property
     def tabs(self):
         if not hasattr(self, '_tabs'):
             self._tabs = get_tabs(self.manager)
         return self._tabs
     
+    @property
+    def bookmarks(self):
+        if not hasattr(self, '_bookmarks'):
+            self._bookmarks = self.load_bookmarks_items()
+        return self._bookmarks
+    
+    @property
+    def recent_tabs(self):
+        if not hasattr(self, '_recent_tabs'):
+            self._recent_tabs = self.get_last_active_tabs(self.manager)
+        return self._recent_tabs
+
+    
     @tabs.setter
     def tabs(self, value):
         self._tabs = value
 
+    @bookmarks.setter
+    def bookmarks(self, value):
+        self._bookamarks = value
+
+    @recent_tabs.setter
+    def recent_tabs(self, value):
+        self._recent_tabs = value
+
     def checkFocus(self, old, new):
         # If the new focus widget is not this widget or a child of this widget
         if new is not self and not self.isAncestorOf(new):
             self.close()
 
-    def open_recent_tab(self, i):
-        if i <= len(self.recent_tabs):
-            tab_id = self.recent_tabs[i-1]
-            switch_tab(tab_id)
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Open on monitor with mouse
         screen_number = QApplication.desktop().screenNumber(QCursor.pos())
         screen_geometry = QApplication.desktop().screenGeometry(screen_number)
         self.move(screen_geometry.center() - self.rect().center())
         self.setWindowModality(Qt.ApplicationModal)
-        self.recent_tabs = self.get_last_active_tabs()
 
-        # Open settings with Ctrl+,
-        shortcut = QShortcut(QKeySequence("Ctrl+,"), self)
-        shortcut.activated.connect(self.open_settings)
-
-        for i in range(1, 6):
-            shortcut = QShortcut(QKeySequence("Ctrl+" + str(i)), self)
-            shortcut.activated.connect(lambda i=i: self.open_recent_tab(i))
+
+        self.visibility_checker = VisibilityChecker(self)
+        self.visibility_checker.start()
       
         self.setWindowTitle('TabSwitcher')
         icon_path = os.path.join(script_dir, 'assets', "Icon.ico")
         self.setWindowIcon(QIcon(icon_path))
         self.setWindowFlags(Qt.FramelessWindowHint | Qt.WindowStaysOnTopHint )
         self.settings = Settings()
         if self.settings.get_show_background() == False:
             self.setAttribute(Qt.WA_TranslucentBackground)
         else:
             self.setAutoFillBackground( True );
         QApplication.instance().focusChanged.connect(self.checkFocus)
         self.manager = QNetworkAccessManager()
 
         self.tabs = get_tabs(self.manager)
+        self.bookmarks = self.load_bookmarks_items()
+        self.recent_tabs = self.get_last_active_tabs()
+
         self.layout = QVBoxLayout()
 
         self.resize(700, 500)
         font_path = os.path.join(script_dir, 'assets', "sans.ttf")
         font = QFont(font_path, 10)  # adjust the size as needed
         self.setFont(font)
         # Create a QLineEdit
         self.input = SearchInput()
         self.list = TabList(self)
-
         self.layout.addWidget(self.input)
         self.layout.addWidget(self.list)
         self.setLayout(self.layout)
         self.input.textChanged.connect(self.update_list)
-        self.list.itemActivated.connect(self.activate_tab)
+        self.list.itemActivated.connect(lambda item: activate_tab(self, item))
         self.update_list("")
+        self.input.setFocus()
+        
+        setup_shortcuts(self)
+
+
         self.setStyleSheet("""
         QWidget {
             background: %s;
         }
     """ % (getWindowBackgroundColor())
         )
-    
-    def open_settings(self):
-        # Open the configuration file in the default text editor
-        QDesktopServices.openUrl(QUrl.fromLocalFile(self.settings.config_file))
 
     def checkFocus(self, old, new):
         # If the new focus widget is not this widget or a child of this widget
         if new is not self and not self.isAncestorOf(new):
             self.close()
 
-    def searchGoogeInNewTab(self, text):
-        text = text[1:].strip()
-        text = text.replace(" ", "+")
-        url = "https://www.google.com/search?q=" + text
-        QDesktopServices.openUrl(QUrl(url))
-
-    def openFirstGoogleResult(self, text):
-        text = text[1:].strip()
-        text = text.replace(" ", "+")
-        url = f'https://www.google.com/search?q={text}&btnI=&sourceid=navclient&gfns=1'
-        QDesktopServices.openUrl(QUrl(url))
-
     def filterByPageContent(self, text):
         tabs = seach_tab(self.manager, text[1:].strip())
         for tab in tabs:
             self.list.addItem(tab.item)
 
     def keyPressEvent(self, event):
-        if event.key() == Qt.Key_Escape:
-            self.close()
-        elif event.key() == Qt.Key_Down and not self.list.hasFocus():
+        if event.key() == Qt.Key_Down and not self.list.hasFocus():
             self.list.setFocus()
             self.list.setCurrentRow(0)
         elif event.key() == Qt.Key_Return and self.input.hasFocus():
             inputText = self.input.text()
 
             if inputText.startswith("?"): 
-                self.searchGoogeInNewTab(inputText)
+                searchGoogeInNewTab(inputText)
             elif inputText.startswith("!"):
-                self.openFirstGoogleResult(inputText)
+                openFirstGoogleResult(inputText)
             elif inputText.startswith(">"):
                 self.filterByPageContent(inputText)
             
             elif self.list.count() > 0:
-                self.activate_tab(self.list.item(0))
+                activate_tab(self, self.list.item(0))
 
         elif event.key() == Qt.Key_Backspace and self.list.hasFocus():
             # Get the current focuses item
             tab_title = self.list.currentItem().text()
             tab = self.tabs[tab_title]
             delete_tab(tab.id)
             current_index = self.list.currentRow()
 
-            del self.tabs[tab_title]
+            if tab_title in self.tabs:
+                del self.tabs[tab_title]
+            
+            if tab_title in self.recent_tabs:
+                del self.recent_tabs[tab_title]
+            
             # Remember the current index
             if current_index >= self.list.count() - 1:
                 current_index = self.list.count() - 2
             self.update_list(self.input.text())
             # Set the focus to the next item
             self.list.setCurrentRow(current_index)
             self.list.setFocus()
 
         else:
             super().keyPressEvent(event)
     
 
+    def load_bookmarks_items(self):
+        bookmarks = load_bookmarks()
+        ar = {}
+        # Ensure that there are no duplicate bookmarks
+        seen_titles = set()
+        seen_urls = set()
+        for bookmark in bookmarks:
+            title, url = bookmark[0], bookmark[1]
+            if title not in seen_titles and url not in seen_urls:
+                ar[title] = Tab(-1, title, url, self.manager)
+                seen_titles.add(title)
+                seen_urls.add(url)
+        return ar
+
     def get_last_active_tabs(self):
         try:
             with open(tab_history_path, 'rb') as f:
-                return pickle.load(f)
+                tab_ids = pickle.load(f)
+                tabs = {}
+                for tab_id in tab_ids:
+                    for _, tab in self.tabs.items():
+                        if tab.id == tab_id:
+                            tabs[tab.title] = tab
+                return tabs
+            
         except FileNotFoundError:
             return []
 
     def get_last_active_tab(self, index):
         tabs = self.get_last_active_tabs()
         if index < len(tabs):
             return tabs[index]
         return None
          
     def update_list(self, text):
+
+        tabs_to_display = []
+        tabs_to_filter = {}
+
+
         # Clear the list before inserting new items
         # remove items from the list without deleting them to keep the netowork images loaded
         for i in reversed(range(self.list.count())): 
             self.list.takeItem(i)
-        if text.startswith('>'):
-            return
 
-        # Show the last 10 open tabs 
-        if text == "" and settings.get_enable_tab_logging():
-            tabIds = self.get_last_active_tabs()
-            tabs = []
-            for tabId in tabIds:
-                for _, tab in self.tabs.items():
-                    if tab.id == tabId:
-                        tabs.append(tab)
-                        break
+        # For commands to show any items
+        if text.startswith(('>', '!', '?')):
+            return
 
-        elif text == "":
-            tabs = self.tabs.values()
+        # Load the bookmarks if the user types #
+        if text.startswith('#'):
+            text = text[1:].strip()
+            tabs_to_filter = self.bookmarks
+        # If there is no text, show the last active tabs
+        elif text == "" and settings.get_enable_tab_logging():
+            tabs_to_filter = self.recent_tabs
+        else:
+            tabs_to_filter = self.tabs
+        
+    
+        # Filter out None keys
+        filtered_keys = [key for key in tabs_to_filter.keys() if key is not None]
 
+        if text == "":
+            tabs_to_display = list(tabs_to_filter.values())
         else:
             if self.settings.get_use_fzf():
-                tabMatches = fuzzy_search_cmd(text, self.tabs.keys())
+                tabMatches = fuzzy_search_cmd(text, filtered_keys)
             else:
-                tabMatches = fuzzy_search_py(text, self.tabs.keys())
+                tabMatches = fuzzy_search_py(text, filtered_keys)
             if not tabMatches:
                 return
-            tabs = [self.tabs[tabName] for tabName in tabMatches if tabName in self.tabs]
+            tabs_to_display = [tabs_to_filter[tabName] for tabName in tabMatches if tabName in tabs_to_filter]
 
-        for tab in tabs:
+        for tab in tabs_to_display:
             self.list.addItem(tab.item)
 
-    def activate_tab(self, item):
-        tab_id = item.data(Qt.UserRole)
-        switch_tab(tab_id)
-        self.close()
-
-
-
 def open_tabswitcher():
     app = QApplication(sys.argv)
     window = MainWindow()
     window.show()
+    window.activateWindow()
+    window.raise_()
     sys.exit(app.exec_())
 
 def main():
     if len(sys.argv) > 1 and sys.argv[1] == "--startlogger":
         from .logTabs import start_logging
         start_logging()
     elif len(sys.argv) > 1 and sys.argv[1] == "--install":
         batch_script = os.path.join(script_dir, "assets", "install.bat")
         subprocess.run(["cmd", "/c", batch_script])
+    elif len(sys.argv) > 1 and sys.argv[1] == "--version":
+        version = pkg_resources.get_distribution("tabswitcher").version
+        print(f"Version: {version}")
+    elif len(sys.argv) > 1 and sys.argv[1] == "--settings":
+        open_settings()
+    elif len(sys.argv) > 1 and sys.argv[1] == "--help":
+        print("tabswitcher: No arguments will just open the switcher window")
+        print("--startlogger\tRun the tab logger that will save the currenlty active tab")
+        print("--install\tWill make sure the logger is startet on system start")
+        print("--version\tGet the version number")
+        print("--help\t\tSee this page")
     else:
         open_tabswitcher()
 
 if __name__ == "__main__":
     main()
```

### Comparing `tabswitcher-0.0.8/src/tabswitcher/assets/Icon.ico` & `tabswitcher-0.1.0/src/tabswitcher/assets/Icon.ico`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.8/src/tabswitcher/assets/brotab_service.xml` & `tabswitcher-0.1.0/src/tabswitcher/assets/tabswitcher_service.xml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 ﻿<?xml version="1.0" encoding="UTF-16"?>
 <Task version="1.2" xmlns="http://schemas.microsoft.com/windows/2004/02/mit/task">
   <RegistrationInfo>
-    <Description>Make sure mediator is installed an running</Description>
-    <URI>\BroTab Service</URI>
+    <Description>Will Log the active tabs</Description>
+    <URI>\Tabswitcher Logger</URI>
   </RegistrationInfo>
   <Triggers>
     <LogonTrigger>
       <Enabled>true</Enabled>
     </LogonTrigger>
   </Triggers>
+  <Principals>
+    <Principal id="Author">
+      <UserId>S-1-5-21-41810631-4193613094-1123250322-1001</UserId>
+      <LogonType>S4U</LogonType>
+      <RunLevel>LeastPrivilege</RunLevel>
+    </Principal>
+  </Principals>
   <Settings>
     <MultipleInstancesPolicy>IgnoreNew</MultipleInstancesPolicy>
     <DisallowStartIfOnBatteries>false</DisallowStartIfOnBatteries>
     <StopIfGoingOnBatteries>false</StopIfGoingOnBatteries>
     <AllowHardTerminate>true</AllowHardTerminate>
     <StartWhenAvailable>true</StartWhenAvailable>
     <RunOnlyIfNetworkAvailable>false</RunOnlyIfNetworkAvailable>
@@ -26,11 +33,12 @@
     <RunOnlyIfIdle>false</RunOnlyIfIdle>
     <WakeToRun>false</WakeToRun>
     <ExecutionTimeLimit>PT0S</ExecutionTimeLimit>
     <Priority>7</Priority>
   </Settings>
   <Actions Context="Author">
     <Exec>
-      <Command>bt_mediator</Command>
+      <Command>C:\Users\Richard\.pyenv\pyenv-win\shims\tabswitcher.bat</Command>
+      <Arguments>--startlogger</Arguments>
     </Exec>
   </Actions>
 </Task>
```

### Comparing `tabswitcher-0.0.8/src/tabswitcher/assets/sans.ttf` & `tabswitcher-0.1.0/src/tabswitcher/assets/sans.ttf`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.8/src/tabswitcher/brotab.py` & `tabswitcher-0.1.0/src/tabswitcher/brotab.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,99 +1,128 @@
 
+import os
 import subprocess
 import chardet
 
+from PyQt5.QtCore import Qt
+from PyQt5.QtGui import QGuiApplication
+
+from tabswitcher.focusWindow import focus_window
+
 from .Settings import Settings
 from .Tab import Tab
 
 settings = Settings()
+script_dir = os.path.dirname(os.path.realpath(__file__))
 
 def get_url():
     mediator_port = settings.get_mediator_port()
     if mediator_port == 0:
         return None
     elif mediator_port not in range(4625, 4627):
         raise ValueError("Mediator port must be between 4625 and 4626 or 0 for automatic selection.")
     return f'127.0.0.1:{mediator_port}'
 
 def get_tabs(manager):
-    url = get_url()
-    if url is None:
-        output = subprocess.check_output(['bt', 'list']).decode()
-    else:
-        output = subprocess.check_output(['bt', '--target', url, 'list']).decode()
+    try:
+        url = get_url()
+        if url is None:
+            output = subprocess.check_output(['bt', 'list'], timeout=5).decode()
+        else:
+            output = subprocess.check_output(['bt', '--target', url, 'list'], timeout=5).decode()
+
+        lines = output.strip().split('\n')
+        lines = [line for line in lines if len(line)]
+        
+        titles = [line.split('\t')[1] for line in lines]
+
+        # Check if there are duplicate titles 
+        duplicate_titles = set(title for title in titles if titles.count(title) > 1)
+
+        tabs = {}
+        for line in lines:
+            id, title, url = line.split('\t')
+            # To prevent the same key add the id to dublicate titles 
+            if title in duplicate_titles:
+                title = f"{id} : {title}"
+            tab = Tab(id, title, url, manager)
+            tabs[title] = tab
+        
+        return tabs
+    except:
+        return {}
 
-    lines = output.strip().split('\n')
-    lines = [line for line in lines if len(line)]
-    
-    titles = [line.split('\t')[1] for line in lines]
+def switch_tab(tab_id, tab_title=None):
+    url = get_url()
 
-    # Check if there are duplicate titles 
-    duplicate_titles = set(title for title in titles if titles.count(title) > 1)
+    app = QGuiApplication.instance()
+    modifiers = app.queryKeyboardModifiers()
 
-    tabs = {}
-    for line in lines:
-        id, title, url = line.split('\t')
-        # To prevent the same key add the id to dublicate titles 
-        if title in duplicate_titles:
-            title = f"{id} : {title}"
-        tab = Tab(id, title, url, manager)
-        tabs[title] = tab
-    
-    return tabs
+    if modifiers & Qt.ShiftModifier:
+        if url is None:
+            subprocess.call(['bt', 'activate', tab_id, '--focused'])
+        else:
+            subprocess.call(['bt', '--target', url, 'activate', tab_id, '--focused'])
+        if tab_title is not None:
+            focus_window(tab_title)
 
-def switch_tab(tab_id):
-    url = get_url()
-    if url is None:
-        subprocess.call(['bt', 'activate', tab_id])
     else:
-        subprocess.call(['bt', '--target', url, 'activate', tab_id])
+        if url is None:
+            subprocess.call(['bt', 'activate', tab_id])
+        else:
+            subprocess.call(['bt', '--target', url, 'activate', tab_id])
+
 
 def delete_tab(tab_id):
     url = get_url()
     if url is None:
         subprocess.call(['bt', 'close', tab_id])
     else:
         subprocess.call(['bt', '--target', url, 'close', tab_id])
 
 
 def seach_tab(manager, text):
-
-    url = get_url()
-    if url is None:
-        _ = subprocess.check_output(['bt', 'index']).decode()
-        output_bytes = subprocess.check_output(['bt', 'search', text])
-    else:
-        _ = subprocess.check_output(['bt', '--target', url, 'index']).decode()
-        output_bytes = subprocess.check_output(['bt', '--target', url, 'search', text])
- 
-    if not output_bytes:
-        return []
-    
-    encoding = chardet.detect(output_bytes)['encoding']
-    output = output_bytes.decode(encoding)
-
-    lines = output.strip().split('\n')
-    lines = [line for line in lines if len(line)]
+    try:
+        url = get_url()
+        if url is None:
+            _ = subprocess.check_output(['bt', 'index'], timeout=20).decode()
+            output_bytes = subprocess.check_output(['bt', 'search', text], timeout=20)
+        else:
+            _ = subprocess.check_output(['bt', '--target', url, 'index'], timeout=20).decode()
+            output_bytes = subprocess.check_output(['bt', '--target', url, 'search', text], timeout=20)
     
-    tabs = []
-    for line in lines:
-        id, title, content = line.split("\t")
-        tab = Tab(id, title, "", manager)
-        tabs.append(tab)
-    return tabs
+        if not output_bytes:
+            return []
+        
+        encoding = chardet.detect(output_bytes)['encoding']
+        output = output_bytes.decode(encoding)
+
+        lines = output.strip().split('\n')
+        lines = [line for line in lines if len(line)]
+        
+        tabs = []
+        for line in lines:
+            id, title, content = line.split("\t")
+            tab = Tab(id, title, "", manager)
+            tabs.append(tab)
+        return tabs
+    except:
+        return []
 
 def active_tab():
-    url = get_url()
-    if url is None:
-        output = subprocess.check_output(['bt', 'active']).decode()
-    else:
-        output = subprocess.check_output(['bt', '--target', url, 'active']).decode()
-    
-    lines = output.strip().split('\n')
-    lines = [line for line in lines if len(line)]
-    if len(lines) == 0:
+    try:
+        url = get_url()
+        if url is None:
+            output = subprocess.check_output(['bt', 'active'], timeout=1).decode()
+        else:
+            output = subprocess.check_output(['bt', '--target', url, 'active'], timeout=1).decode()
+        
+        lines = output.strip().split('\n')
+        lines = [line for line in lines if len(line)]
+        if len(lines) == 0:
+            return None
+        data = lines[0].split('\t')
+        if (len(data) == 5):
+            return data[0]
         return None
-    data = lines[0].split('\t')
-    if (len(data) == 5):
-        return data[0]
-    return None
+    except:
+        return None
```

### Comparing `tabswitcher-0.0.8/src/tabswitcher/colors.py` & `tabswitcher-0.1.0/src/tabswitcher/colors.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.8/src/tabswitcher/fuzzySearch.py` & `tabswitcher-0.1.0/src/tabswitcher/fuzzySearch.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.0.8/src/tabswitcher/logTabs.py` & `tabswitcher-0.1.0/src/tabswitcher/logTabs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 tabHistory = deque(maxlen=settings.get_tab_logging_max())
 counter = 0
 
 def show_list():
     global counter
     counter += 1
     #Clear screen
-    print("\033[H\033[J")
+    os.system('cls' if os.name == 'nt' else 'clear')
     print(f"Run {counter}")
     for tab in tabHistory:
         print(tab)
     
 # Check the active tab every second and log it to the tabHistory
 def check_active_tab():
     tab_id = active_tab()
     if tab_id in tabHistory:
         tabHistory.remove(tab_id)
     tabHistory.appendleft(tab_id)
 
     with open(tab_history_path, 'wb') as f:
         pickle.dump(list(tabHistory), f)
-    show_list()
+    # show_list()
     
 # Start the scheculer just to make sure nothing is skipped
 def run_schedule():
     while 1:
         schedule.run_pending()
         time.sleep(1)
```

### Comparing `tabswitcher-0.0.8/tabswitcher.egg-info/SOURCES.txt` & `tabswitcher-0.1.0/tabswitcher.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 README.md
 setup.py
 src/tabswitcher/NetworkImage.py
 src/tabswitcher/SearchInput.py
 src/tabswitcher/Settings.py
 src/tabswitcher/Tab.py
 src/tabswitcher/TabList.py
+src/tabswitcher/VisibilityChecker.py
 src/tabswitcher/__main__.py
+src/tabswitcher/actions.py
 src/tabswitcher/brotab.py
 src/tabswitcher/colors.py
+src/tabswitcher/focusWindow.py
 src/tabswitcher/fuzzySearch.py
 src/tabswitcher/loadBookmarks.py
 src/tabswitcher/logTabs.py
+src/tabswitcher/shortcuts.py
 src/tabswitcher/assets/Icon.ico
-src/tabswitcher/assets/brotab_service.xml
 src/tabswitcher/assets/install.bat
 src/tabswitcher/assets/sans.ttf
 src/tabswitcher/assets/searchIcon.svg
 src/tabswitcher/assets/tabswitcher_service.xml
 tabswitcher.egg-info/PKG-INFO
 tabswitcher.egg-info/SOURCES.txt
 tabswitcher.egg-info/dependency_links.txt
```

