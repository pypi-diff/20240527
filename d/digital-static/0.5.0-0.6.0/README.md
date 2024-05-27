# Comparing `tmp/digital_static-0.5.0.tar.gz` & `tmp/digital_static-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital_static-0.5.0.tar", last modified: Sun Jun 26 20:52:32 2022, max compression
+gzip compressed data, was "digital_static-0.6.0.tar", last modified: Mon May 27 21:13:18 2024, max compression
```

## Comparing `digital_static-0.5.0.tar` & `digital_static-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxr-x   0 chad      (1000) chad      (1000)        0 2022-06-26 20:52:32.963697 digital_static-0.5.0/
--rw-rw-r--   0 chad      (1000) chad      (1000)     1066 2022-06-22 13:46:12.000000 digital_static-0.5.0/LICENSE
--rw-rw-r--   0 chad      (1000) chad      (1000)     1638 2022-06-26 20:52:32.963697 digital_static-0.5.0/PKG-INFO
--rw-rw-r--   0 chad      (1000) chad      (1000)     1111 2022-06-26 02:53:25.000000 digital_static-0.5.0/README.md
-drwxrwxr-x   0 chad      (1000) chad      (1000)        0 2022-06-26 20:52:32.963697 digital_static-0.5.0/digital_static.egg-info/
--rw-rw-r--   0 chad      (1000) chad      (1000)     1638 2022-06-26 20:52:32.000000 digital_static-0.5.0/digital_static.egg-info/PKG-INFO
--rw-rw-r--   0 chad      (1000) chad      (1000)      305 2022-06-26 20:52:32.000000 digital_static-0.5.0/digital_static.egg-info/SOURCES.txt
--rw-rw-r--   0 chad      (1000) chad      (1000)        1 2022-06-26 20:52:32.000000 digital_static-0.5.0/digital_static.egg-info/dependency_links.txt
--rw-rw-r--   0 chad      (1000) chad      (1000)       49 2022-06-26 20:52:32.000000 digital_static-0.5.0/digital_static.egg-info/entry_points.txt
--rw-rw-r--   0 chad      (1000) chad      (1000)       94 2022-06-26 20:52:32.000000 digital_static-0.5.0/digital_static.egg-info/requires.txt
--rw-rw-r--   0 chad      (1000) chad      (1000)        8 2022-06-26 20:52:32.000000 digital_static-0.5.0/digital_static.egg-info/top_level.txt
-drwxrwxr-x   0 chad      (1000) chad      (1000)        0 2022-06-26 20:52:32.963697 digital_static-0.5.0/dstatic/
--rw-rw-r--   0 chad      (1000) chad      (1000)        0 2022-06-22 13:46:12.000000 digital_static-0.5.0/dstatic/__init__.py
--rw-rw-r--   0 chad      (1000) chad      (1000)    13351 2022-06-26 02:54:04.000000 digital_static-0.5.0/dstatic/dstatic.py
--rw-rw-r--   0 chad      (1000) chad      (1000)      832 2022-06-26 20:52:32.967697 digital_static-0.5.0/setup.cfg
--rw-rw-r--   0 chad      (1000) chad      (1000)       37 2022-06-22 13:46:12.000000 digital_static-0.5.0/setup.py
+drwxrwxr-x   0 chad      (1000) chad      (1000)        0 2024-05-27 21:13:18.333033 digital_static-0.6.0/
+-rw-rw-r--   0 chad      (1000) chad      (1000)     1066 2024-05-25 00:37:08.000000 digital_static-0.6.0/LICENSE
+-rw-r--r--   0 chad      (1000) chad      (1000)     2051 2024-05-27 21:13:18.333033 digital_static-0.6.0/PKG-INFO
+-rw-rw-r--   0 chad      (1000) chad      (1000)     1305 2024-05-27 21:02:49.000000 digital_static-0.6.0/README.md
+drwxrwxr-x   0 chad      (1000) chad      (1000)        0 2024-05-27 21:13:18.329033 digital_static-0.6.0/digital_static.egg-info/
+-rw-r--r--   0 chad      (1000) chad      (1000)     2051 2024-05-27 21:13:18.000000 digital_static-0.6.0/digital_static.egg-info/PKG-INFO
+-rw-rw-r--   0 chad      (1000) chad      (1000)      359 2024-05-27 21:13:18.000000 digital_static-0.6.0/digital_static.egg-info/SOURCES.txt
+-rw-rw-r--   0 chad      (1000) chad      (1000)        1 2024-05-27 21:13:18.000000 digital_static-0.6.0/digital_static.egg-info/dependency_links.txt
+-rw-rw-r--   0 chad      (1000) chad      (1000)       49 2024-05-27 21:13:18.000000 digital_static-0.6.0/digital_static.egg-info/entry_points.txt
+-rw-rw-r--   0 chad      (1000) chad      (1000)       94 2024-05-27 21:13:18.000000 digital_static-0.6.0/digital_static.egg-info/requires.txt
+-rw-rw-r--   0 chad      (1000) chad      (1000)        8 2024-05-27 21:13:18.000000 digital_static-0.6.0/digital_static.egg-info/top_level.txt
+drwxrwxr-x   0 chad      (1000) chad      (1000)        0 2024-05-27 21:13:18.329033 digital_static-0.6.0/dstatic/
+-rw-rw-r--   0 chad      (1000) chad      (1000)        0 2024-05-25 00:37:08.000000 digital_static-0.6.0/dstatic/__init__.py
+-rw-rw-r--   0 chad      (1000) chad      (1000)    20992 2024-05-27 21:02:49.000000 digital_static-0.6.0/dstatic/dstatic.py
+-rw-rw-r--   0 chad      (1000) chad      (1000)      911 2024-05-27 21:13:18.333033 digital_static-0.6.0/setup.cfg
+-rw-rw-r--   0 chad      (1000) chad      (1000)       37 2024-05-25 00:37:08.000000 digital_static-0.6.0/setup.py
+drwxrwxr-x   0 chad      (1000) chad      (1000)        0 2024-05-27 21:13:18.329033 digital_static-0.6.0/tests/
+-rw-rw-r--   0 chad      (1000) chad      (1000)    22340 2024-05-27 21:02:49.000000 digital_static-0.6.0/tests/test_dstatic.py
+-rw-rw-r--   0 chad      (1000) chad      (1000)     6503 2024-05-25 00:37:08.000000 digital_static-0.6.0/tests/test_dstatic_arguments.py
```

### Comparing `digital_static-0.5.0/LICENSE` & `digital_static-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `digital_static-0.5.0/PKG-INFO` & `digital_static-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: digital_static
-Version: 0.5.0
+Version: 0.6.0
 Summary: static/snow simulation using python 3 and curses
 Home-page: https://github.com/tech-chad/digitalstatic
 Author: Chad Larson
 Author-email: techchad2@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: importlib-metadata>=1.6; python_version < "3.8"
+Requires-Dist: windows-curses; sys_platform == "win32"
 
 # digital_static
 Digital Static / Snow with Python 3 and curses
 
+Python 3.7 +
+
 ### How to install
 ```pip install digital_static```
 
 ### To Run
 ```dstatic```
 
 ### Commands
@@ -29,15 +35,17 @@
 - <kbd>C</kbd> = Switch to color mode
 - <kbd>c</kbd> = Toggle cycle color mode
 - <kbd>a</kbd> = Toggle enable additive mode <kbd>r,t,y,u,i,o</kbd> to add and remove colors
 - <kbd>d</kbd> = Reset to default settings
 - <kbd>0 to 9</kbd> = Delay Speed
 - <kbd>shift 1 to 5</kbd> = Cycle color delay when inn cycle color mode
 - <kbd>l</kbd> = Clear the screen, wait 2 seconds and start again.
-- <kbd>f</kbd> = Freeze the screen until <kbd>f</kbd> is pressed again.  
+- <kbd>f</kbd> = Freeze the screen until <kbd>f</kbd> is pressed again.
+- <kbd>z</kbd> = Cycle through test patterns
+- <kbd>w</kbd> = Display a fake blue screen of death 
 
 #### Colors
 Change colors while running
 - <kbd>r</kbd> = Red
 - <kbd>t</kbd> = Green
 - <kbd>y</kbd> = Blue
 - <kbd>u</kbd> = Yellow
@@ -47,7 +55,10 @@
 ### Screen Shots
 ![screen1](https://i.fluffy.cc/PzDwTN3sZC6fbbnKL4SMSDQFwr1P1mTr.png)
 
 ![screen2](https://i.fluffy.cc/p38RJxwTn7rRCHKkFrxPKzM9CTK84MgP.png)
 
 ![screen3](https://i.fluffy.cc/sLz0sqC8pFdf27twrh6z4BJ27StlG7jc.png)
 
+Test Pattern
+![screen4](https://i.fluffy.cc/mGlGNWhG8CWFX2m266pxhpsm5GDj2Db7.png)
+
```

### Comparing `digital_static-0.5.0/README.md` & `digital_static-0.6.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # digital_static
 Digital Static / Snow with Python 3 and curses
 
+Python 3.7 +
+
 ### How to install
 ```pip install digital_static```
 
 ### To Run
 ```dstatic```
 
 ### Commands
@@ -13,15 +15,17 @@
 - <kbd>C</kbd> = Switch to color mode
 - <kbd>c</kbd> = Toggle cycle color mode
 - <kbd>a</kbd> = Toggle enable additive mode <kbd>r,t,y,u,i,o</kbd> to add and remove colors
 - <kbd>d</kbd> = Reset to default settings
 - <kbd>0 to 9</kbd> = Delay Speed
 - <kbd>shift 1 to 5</kbd> = Cycle color delay when inn cycle color mode
 - <kbd>l</kbd> = Clear the screen, wait 2 seconds and start again.
-- <kbd>f</kbd> = Freeze the screen until <kbd>f</kbd> is pressed again.  
+- <kbd>f</kbd> = Freeze the screen until <kbd>f</kbd> is pressed again.
+- <kbd>z</kbd> = Cycle through test patterns
+- <kbd>w</kbd> = Display a fake blue screen of death 
 
 #### Colors
 Change colors while running
 - <kbd>r</kbd> = Red
 - <kbd>t</kbd> = Green
 - <kbd>y</kbd> = Blue
 - <kbd>u</kbd> = Yellow
@@ -31,7 +35,10 @@
 ### Screen Shots
 ![screen1](https://i.fluffy.cc/PzDwTN3sZC6fbbnKL4SMSDQFwr1P1mTr.png)
 
 ![screen2](https://i.fluffy.cc/p38RJxwTn7rRCHKkFrxPKzM9CTK84MgP.png)
 
 ![screen3](https://i.fluffy.cc/sLz0sqC8pFdf27twrh6z4BJ27StlG7jc.png)
 
+Test Pattern
+![screen4](https://i.fluffy.cc/mGlGNWhG8CWFX2m266pxhpsm5GDj2Db7.png)
+
```

### Comparing `digital_static-0.5.0/digital_static.egg-info/PKG-INFO` & `digital_static-0.6.0/digital_static.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
-Name: digital-static
-Version: 0.5.0
+Name: digital_static
+Version: 0.6.0
 Summary: static/snow simulation using python 3 and curses
 Home-page: https://github.com/tech-chad/digitalstatic
 Author: Chad Larson
 Author-email: techchad2@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: importlib-metadata>=1.6; python_version < "3.8"
+Requires-Dist: windows-curses; sys_platform == "win32"
 
 # digital_static
 Digital Static / Snow with Python 3 and curses
 
+Python 3.7 +
+
 ### How to install
 ```pip install digital_static```
 
 ### To Run
 ```dstatic```
 
 ### Commands
@@ -29,15 +35,17 @@
 - <kbd>C</kbd> = Switch to color mode
 - <kbd>c</kbd> = Toggle cycle color mode
 - <kbd>a</kbd> = Toggle enable additive mode <kbd>r,t,y,u,i,o</kbd> to add and remove colors
 - <kbd>d</kbd> = Reset to default settings
 - <kbd>0 to 9</kbd> = Delay Speed
 - <kbd>shift 1 to 5</kbd> = Cycle color delay when inn cycle color mode
 - <kbd>l</kbd> = Clear the screen, wait 2 seconds and start again.
-- <kbd>f</kbd> = Freeze the screen until <kbd>f</kbd> is pressed again.  
+- <kbd>f</kbd> = Freeze the screen until <kbd>f</kbd> is pressed again.
+- <kbd>z</kbd> = Cycle through test patterns
+- <kbd>w</kbd> = Display a fake blue screen of death 
 
 #### Colors
 Change colors while running
 - <kbd>r</kbd> = Red
 - <kbd>t</kbd> = Green
 - <kbd>y</kbd> = Blue
 - <kbd>u</kbd> = Yellow
@@ -47,7 +55,10 @@
 ### Screen Shots
 ![screen1](https://i.fluffy.cc/PzDwTN3sZC6fbbnKL4SMSDQFwr1P1mTr.png)
 
 ![screen2](https://i.fluffy.cc/p38RJxwTn7rRCHKkFrxPKzM9CTK84MgP.png)
 
 ![screen3](https://i.fluffy.cc/sLz0sqC8pFdf27twrh6z4BJ27StlG7jc.png)
 
+Test Pattern
+![screen4](https://i.fluffy.cc/mGlGNWhG8CWFX2m266pxhpsm5GDj2Db7.png)
+
```

