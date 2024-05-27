# Comparing `tmp/gqylpy_dict-1.2.5.tar.gz` & `tmp/gqylpy_dict-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqylpy_dict-1.2.5.tar", last modified: Sun Sep  3 02:36:14 2023, max compression
+gzip compressed data, was "gqylpy_dict-1.2.6.tar", last modified: Mon May 27 07:17:52 2024, max compression
```

## Comparing `gqylpy_dict-1.2.5.tar` & `gqylpy_dict-1.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 02:36:14.158754 gqylpy_dict-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (999)    12343 2023-09-03 02:36:03.000000 gqylpy_dict-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     2039 2023-09-03 02:36:03.000000 gqylpy_dict-1.2.5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (999)     4005 2023-09-03 02:36:14.158754 gqylpy_dict-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2870 2023-09-03 02:36:03.000000 gqylpy_dict-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 02:36:14.154754 gqylpy_dict-1.2.5/gqylpy_dict/
--rw-r--r--   0 runner    (1001) docker     (999)    10919 2023-09-03 02:36:03.000000 gqylpy_dict-1.2.5/gqylpy_dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    10090 2023-09-03 02:36:03.000000 gqylpy_dict-1.2.5/gqylpy_dict/g dict.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 02:36:14.158754 gqylpy_dict-1.2.5/gqylpy_dict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     4005 2023-09-03 02:36:14.000000 gqylpy_dict-1.2.5/gqylpy_dict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      219 2023-09-03 02:36:14.000000 gqylpy_dict-1.2.5/gqylpy_dict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-03 02:36:14.000000 gqylpy_dict-1.2.5/gqylpy_dict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       12 2023-09-03 02:36:14.000000 gqylpy_dict-1.2.5/gqylpy_dict.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-03 02:36:14.158754 gqylpy_dict-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1511 2023-09-03 02:36:03.000000 gqylpy_dict-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:17:52.331693 gqylpy_dict-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    12342 2024-05-27 07:17:48.000000 gqylpy_dict-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-27 07:17:48.000000 gqylpy_dict-1.2.6/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-27 07:17:52.331693 gqylpy_dict-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-27 07:17:48.000000 gqylpy_dict-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:17:52.327693 gqylpy_dict-1.2.6/gqylpy_dict/
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-27 07:17:48.000000 gqylpy_dict-1.2.6/gqylpy_dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-05-27 07:17:48.000000 gqylpy_dict-1.2.6/gqylpy_dict/g dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:17:52.327693 gqylpy_dict-1.2.6/gqylpy_dict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-27 07:17:52.000000 gqylpy_dict-1.2.6/gqylpy_dict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-27 07:17:52.000000 gqylpy_dict-1.2.6/gqylpy_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:17:52.000000 gqylpy_dict-1.2.6/gqylpy_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 07:17:52.000000 gqylpy_dict-1.2.6/gqylpy_dict.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:17:52.331693 gqylpy_dict-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-27 07:17:48.000000 gqylpy_dict-1.2.6/setup.py
```

### Comparing `gqylpy_dict-1.2.5/LICENSE` & `gqylpy_dict-1.2.6/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
+   Copyright (c) 2022-2024 GQYLPY <http://gqylpy.com>. All rights reserved.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `gqylpy_dict-1.2.5/NOTICE` & `gqylpy_dict-1.2.6/NOTICE`

 * *Files identical despite different names*

### Comparing `gqylpy_dict-1.2.5/gqylpy_dict/__init__.py` & `gqylpy_dict-1.2.6/gqylpy_dict/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
-The `gqylpy_dict` based on the built-in `dict`, it is an enhancement of the
-built-in `dict`. It can do anything `dict` can do, and can do more what `dict`
-cannot do.
+`gqylpy-dict` is based on the built-in `dict` and serves as an enhancement
+to it. It can do everything the built-in `dict` can do, and even more.
 
     >>> from gqylpy_dict import gdict
 
     >>> gdict == dict
     True
 
     >>> gdict is dict
@@ -15,20 +14,20 @@
     >>> x = gdict(x)
     >>> x.a[0].b
     'B'
 
     >>> x.deepget('a[0].b')
     'B'
 
-    @version: 1.2.5
+    @version: 1.2.6
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/gqylpy-dict
 
 ────────────────────────────────────────────────────────────────────────────────
-Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
+Copyright (c) 2022-2024 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 This file is licensed under the WTFPL:
 
             DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                     Version 2, December 2004
 
  Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>
```

### Comparing `gqylpy_dict-1.2.5/gqylpy_dict/g dict.py` & `gqylpy_dict-1.2.6/gqylpy_dict/g dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
+Copyright (c) 2022-2024 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 ────────────────────────────────────────────────────────────────────────────────
 
 Lines 51 through 99 is licensed under the Apache-2.0:
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
```

