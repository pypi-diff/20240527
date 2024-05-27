# Comparing `tmp/linkedit-1.0.5.tar.gz` & `tmp/linkedit-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedit-1.0.5.tar", last modified: Thu May 23 15:49:44 2024, max compression
+gzip compressed data, was "linkedit-1.0.7.tar", last modified: Mon May 27 17:46:32 2024, max compression
```

## Comparing `linkedit-1.0.5.tar` & `linkedit-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 15:49:44.963789 linkedit-1.0.5/
--rw-r--r--   0 khiat     (1000) khiat     (1000)    71475 2024-05-23 15:49:44.963789 linkedit-1.0.5/PKG-INFO
--rw-rw-r--   0 khiat     (1000) khiat     (1000)    71021 2024-05-20 21:58:54.000000 linkedit-1.0.5/README.md
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 15:49:44.963789 linkedit-1.0.5/linkedit/
--rw-rw-r--   0 khiat     (1000) khiat     (1000)   110724 2024-05-23 15:48:09.000000 linkedit-1.0.5/linkedit/__init__.py
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 15:49:44.963789 linkedit-1.0.5/linkedit.egg-info/
--rw-r--r--   0 khiat     (1000) khiat     (1000)    71475 2024-05-23 15:49:44.000000 linkedit-1.0.5/linkedit.egg-info/PKG-INFO
--rw-r--r--   0 khiat     (1000) khiat     (1000)      198 2024-05-23 15:49:44.000000 linkedit-1.0.5/linkedit.egg-info/SOURCES.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-23 15:49:44.000000 linkedit-1.0.5/linkedit.egg-info/dependency_links.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       16 2024-05-23 15:49:44.000000 linkedit-1.0.5/linkedit.egg-info/requires.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        9 2024-05-23 15:49:44.000000 linkedit-1.0.5/linkedit.egg-info/top_level.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-23 15:49:44.963789 linkedit-1.0.5/setup.cfg
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      721 2024-05-23 15:49:04.000000 linkedit-1.0.5/setup.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-27 17:46:32.396074 linkedit-1.0.7/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)    71475 2024-05-27 17:46:32.396074 linkedit-1.0.7/PKG-INFO
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)    71021 2024-05-27 17:43:50.000000 linkedit-1.0.7/README.md
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-27 17:46:32.396074 linkedit-1.0.7/linkedit/
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)   101573 2024-05-27 17:35:10.000000 linkedit-1.0.7/linkedit/__init__.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-27 17:46:32.396074 linkedit-1.0.7/linkedit.egg-info/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)    71475 2024-05-27 17:46:32.000000 linkedit-1.0.7/linkedit.egg-info/PKG-INFO
+-rw-r--r--   0 khiat     (1000) khiat     (1000)      198 2024-05-27 17:46:32.000000 linkedit-1.0.7/linkedit.egg-info/SOURCES.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-27 17:46:32.000000 linkedit-1.0.7/linkedit.egg-info/dependency_links.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       16 2024-05-27 17:46:32.000000 linkedit-1.0.7/linkedit.egg-info/requires.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        9 2024-05-27 17:46:32.000000 linkedit-1.0.7/linkedit.egg-info/top_level.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-27 17:46:32.396074 linkedit-1.0.7/setup.cfg
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      721 2024-05-27 17:46:19.000000 linkedit-1.0.7/setup.py
```

### Comparing `linkedit-1.0.5/PKG-INFO` & `linkedit-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedit
-Version: 1.0.5
+Version: 1.0.7
 Summary: Sophisticate Linked List
 Home-page: https://pypi.org/project/linkedit/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: linked list
 Classifier: Programming Language :: Python :: 3
@@ -70,15 +70,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│ current value   │ current value @ddress   │ next value   │ next value @ddress   │
+│ Current Value   │ Current Value @ddress   │ Next Value   │ Next Value @ddress   │
 ╞═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │ 6               │ 0x7febe8213950          │ 3            │ 0x7febe8213990       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 3               │ 0x7febe8213990          │ 8            │ 0x7febe82139d0       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 8               │ 0x7febe82139d0          │ 1            │ 0x7febe823c110       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -108,15 +108,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│ current value   │ current value @ddress   │ next value   │ next value @ddress   │
+│ Current Value   │ Current Value @ddress   │ Next Value   │ Next Value @ddress   │
 ╞═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │ 6               │ 140217964133136         │ 3            │ 140217964133264      │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 3               │ 140217964133264         │ 8            │ 140217964133200      │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 8               │ 140217964133200         │ 1            │ 140217964298704      │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -379,15 +379,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│   current value │ current value @ddress   │   next value │ next value @ddress   │
+│   Current Value │ Current Value @ddress   │   Next Value │ Next Value @ddress   │
 ╞═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │               6 │ 0x7fbe38bf3ad0          │            3 │ 0x7fbe38bf3b50       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │               3 │ 0x7fbe38bf3b50          │            8 │ 0x7fbe38bf3b10       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │               8 │ 0x7fbe38bf3b10          │            1 │ 0x7fbe38c07fd0       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -415,15 +415,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│   current value │   current value @ddress │   next value │   next value @ddress │
+│   Current Value │   Current Value @ddress │   Next Value │   Next Value @ddress │
 ╞═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │               6 │         140374800546256 │            3 │      140374800546448 │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │               3 │         140374800546448 │            8 │      140374800546192 │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │               8 │         140374800546192 │            1 │      140374800629712 │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -738,15 +738,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════════════════╤══════════════════════════╤═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│ previous value   │ previous value @ddress   │ current value   │ current value @ddress   │ next value   │ next value @ddress   │
+│ Previous Value   │ Previous Value @ddress   │ Current Value   │ Current Value @ddress   │ Next Value   │ Next Value @ddress   │
 ╞══════════════════╪══════════════════════════╪═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │                  │                          │ None (NULL)     │ 0x959cc0 (nil/0x0)      │              │                      │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ None (NULL)      │ 0x959cc0 (nil/0x0)       │ 6               │ 0x7effd8613950          │ 3            │ 0x7effd8613990       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 6                │ 0x7effd8613950           │ 3               │ 0x7effd8613990          │ 8            │ 0x7effd86139d0       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -778,15 +778,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════════════════╤══════════════════════════╤═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│ previous value   │ previous value @ddress   │ current value   │ current value @ddress   │ next value   │ next value @ddress   │
+│ Previous Value   │ Previous Value @ddress   │ Current Value   │ Current Value @ddress   │ Next Value   │ Next Value @ddress   │
 ╞══════════════════╪══════════════════════════╪═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │                  │                          │ None (NULL)     │ 9804992 (nil/0)         │              │                      │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ None (NULL)      │ 9804992 (nil/0)          │ 6               │ 140107643451856         │ 3            │ 140107643451984      │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 6                │ 140107643451856          │ 3               │ 140107643451984         │ 8            │ 140107643451920      │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -1054,15 +1054,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════════════════╤══════════════════════════╤═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│   previous value │ previous value @ddress   │   current value │ current value @ddress   │   next value │ next value @ddress   │
+│   Previous Value │ Previous Value @ddress   │   Current Value │ Current Value @ddress   │   Next Value │ Next Value @ddress   │
 ╞══════════════════╪══════════════════════════╪═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │                7 │ 0x7ff7a725be10           │               6 │ 0x7ff7a7413ad0          │            3 │ 0x7ff7a7413b50       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │                6 │ 0x7ff7a7413ad0           │               3 │ 0x7ff7a7413b50          │            8 │ 0x7ff7a7413b10       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │                3 │ 0x7ff7a7413b50           │               8 │ 0x7ff7a7413b10          │            1 │ 0x7ff7a7427fd0       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -1090,15 +1090,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════════════════╤══════════════════════════╤═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│   previous value │   previous value @ddress │   current value │   current value @ddress │   next value │   next value @ddress │
+│   Previous Value │   Previous Value @ddress │   Current Value │   Current Value @ddress │   Next Value │   Next Value @ddress │
 ╞══════════════════╪══════════════════════════╪═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │                7 │          140070320684368 │               6 │         140070322534992 │            3 │      140070322535184 │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │                6 │          140070322534992 │               3 │         140070322535184 │            8 │      140070322534928 │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │                3 │          140070322535184 │               8 │         140070322534928 │            1 │      140070322700432 │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -1441,15 +1441,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════╤════════════════╤════════════╤════════════════╤═══════════╤════════════════╤════════╤════════════════╤════════╤════════════════╕
-│ up   │ up @           │ previous   │ previous @     │   current │ current @      │ down   │ down @         │ next   │ next @         │
+│ Up   │ Up @           │ Previous   │ Previous @     │   Current │ Current @      │ Down   │ Down @         │ Next   │ Next @         │
 ╞══════╪════════════════╪════════════╪════════════════╪═══════════╪════════════════╪════════╪════════════════╪════════╪════════════════╡
 │ None │ 0x959cc0       │ None       │ 0x959cc0       │         6 │ 0x7f20d0213250 │ 1      │ 0x7f20d0213cd0 │ 3      │ 0x7f20d0213c50 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
 │ None │ 0x959cc0       │ 6          │ 0x7f20d0213250 │         3 │ 0x7f20d0213c50 │ 9      │ 0x7f20d023c090 │ 8      │ 0x7f20d0213c90 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
 │ None │ 0x959cc0       │ 3          │ 0x7f20d0213c50 │         8 │ 0x7f20d0213c90 │ 5      │ 0x7f20d005bcd0 │ None   │ 0x959cc0       │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
@@ -1507,15 +1507,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════╤════════════════╤════════════╤════════════════╤═══════════╤════════════════╤════════╤════════════════╤════════╤════════════════╕
-│   up │ up @           │   previous │ previous @     │   current │ current @      │   down │ down @         │   next │ next @         │
+│   Up │ Up @           │   Previous │ Previous @     │   Current │ Current @      │   Down │ Down @         │   Next │ Next @         │
 ╞══════╪════════════════╪════════════╪════════════════╪═══════════╪════════════════╪════════╪════════════════╪════════╪════════════════╡
 │    7 │ 0x7f01e6153ad0 │          8 │ 0x7f01e6317cd0 │         6 │ 0x7f01e6316250 │      1 │ 0x7f01e6317d10 │      3 │ 0x7f01e6317c90 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
 │    2 │ 0x7f01e6153dd0 │          6 │ 0x7f01e6316250 │         3 │ 0x7f01e6317c90 │      9 │ 0x7f01e632bfd0 │      8 │ 0x7f01e6317cd0 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
 │    4 │ 0x7f01e6153d10 │          3 │ 0x7f01e6317c90 │         8 │ 0x7f01e6317cd0 │      5 │ 0x7f01e6153c90 │      6 │ 0x7f01e6316250 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
```

### Comparing `linkedit-1.0.5/README.md` & `linkedit-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│ current value   │ current value @ddress   │ next value   │ next value @ddress   │
+│ Current Value   │ Current Value @ddress   │ Next Value   │ Next Value @ddress   │
 ╞═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │ 6               │ 0x7febe8213950          │ 3            │ 0x7febe8213990       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 3               │ 0x7febe8213990          │ 8            │ 0x7febe82139d0       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 8               │ 0x7febe82139d0          │ 1            │ 0x7febe823c110       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -93,15 +93,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│ current value   │ current value @ddress   │ next value   │ next value @ddress   │
+│ Current Value   │ Current Value @ddress   │ Next Value   │ Next Value @ddress   │
 ╞═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │ 6               │ 140217964133136         │ 3            │ 140217964133264      │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 3               │ 140217964133264         │ 8            │ 140217964133200      │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 8               │ 140217964133200         │ 1            │ 140217964298704      │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -364,15 +364,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│   current value │ current value @ddress   │   next value │ next value @ddress   │
+│   Current Value │ Current Value @ddress   │   Next Value │ Next Value @ddress   │
 ╞═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │               6 │ 0x7fbe38bf3ad0          │            3 │ 0x7fbe38bf3b50       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │               3 │ 0x7fbe38bf3b50          │            8 │ 0x7fbe38bf3b10       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │               8 │ 0x7fbe38bf3b10          │            1 │ 0x7fbe38c07fd0       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -400,15 +400,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│   current value │   current value @ddress │   next value │   next value @ddress │
+│   Current Value │   Current Value @ddress │   Next Value │   Next Value @ddress │
 ╞═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │               6 │         140374800546256 │            3 │      140374800546448 │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │               3 │         140374800546448 │            8 │      140374800546192 │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │               8 │         140374800546192 │            1 │      140374800629712 │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -723,15 +723,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════════════════╤══════════════════════════╤═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│ previous value   │ previous value @ddress   │ current value   │ current value @ddress   │ next value   │ next value @ddress   │
+│ Previous Value   │ Previous Value @ddress   │ Current Value   │ Current Value @ddress   │ Next Value   │ Next Value @ddress   │
 ╞══════════════════╪══════════════════════════╪═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │                  │                          │ None (NULL)     │ 0x959cc0 (nil/0x0)      │              │                      │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ None (NULL)      │ 0x959cc0 (nil/0x0)       │ 6               │ 0x7effd8613950          │ 3            │ 0x7effd8613990       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 6                │ 0x7effd8613950           │ 3               │ 0x7effd8613990          │ 8            │ 0x7effd86139d0       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -763,15 +763,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════════════════╤══════════════════════════╤═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│ previous value   │ previous value @ddress   │ current value   │ current value @ddress   │ next value   │ next value @ddress   │
+│ Previous Value   │ Previous Value @ddress   │ Current Value   │ Current Value @ddress   │ Next Value   │ Next Value @ddress   │
 ╞══════════════════╪══════════════════════════╪═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │                  │                          │ None (NULL)     │ 9804992 (nil/0)         │              │                      │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ None (NULL)      │ 9804992 (nil/0)          │ 6               │ 140107643451856         │ 3            │ 140107643451984      │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 6                │ 140107643451856          │ 3               │ 140107643451984         │ 8            │ 140107643451920      │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -1039,15 +1039,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════════════════╤══════════════════════════╤═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│   previous value │ previous value @ddress   │   current value │ current value @ddress   │   next value │ next value @ddress   │
+│   Previous Value │ Previous Value @ddress   │   Current Value │ Current Value @ddress   │   Next Value │ Next Value @ddress   │
 ╞══════════════════╪══════════════════════════╪═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │                7 │ 0x7ff7a725be10           │               6 │ 0x7ff7a7413ad0          │            3 │ 0x7ff7a7413b50       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │                6 │ 0x7ff7a7413ad0           │               3 │ 0x7ff7a7413b50          │            8 │ 0x7ff7a7413b10       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │                3 │ 0x7ff7a7413b50           │               8 │ 0x7ff7a7413b10          │            1 │ 0x7ff7a7427fd0       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -1075,15 +1075,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════════════════╤══════════════════════════╤═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│   previous value │   previous value @ddress │   current value │   current value @ddress │   next value │   next value @ddress │
+│   Previous Value │   Previous Value @ddress │   Current Value │   Current Value @ddress │   Next Value │   Next Value @ddress │
 ╞══════════════════╪══════════════════════════╪═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │                7 │          140070320684368 │               6 │         140070322534992 │            3 │      140070322535184 │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │                6 │          140070322534992 │               3 │         140070322535184 │            8 │      140070322534928 │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │                3 │          140070322535184 │               8 │         140070322534928 │            1 │      140070322700432 │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -1426,15 +1426,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════╤════════════════╤════════════╤════════════════╤═══════════╤════════════════╤════════╤════════════════╤════════╤════════════════╕
-│ up   │ up @           │ previous   │ previous @     │   current │ current @      │ down   │ down @         │ next   │ next @         │
+│ Up   │ Up @           │ Previous   │ Previous @     │   Current │ Current @      │ Down   │ Down @         │ Next   │ Next @         │
 ╞══════╪════════════════╪════════════╪════════════════╪═══════════╪════════════════╪════════╪════════════════╪════════╪════════════════╡
 │ None │ 0x959cc0       │ None       │ 0x959cc0       │         6 │ 0x7f20d0213250 │ 1      │ 0x7f20d0213cd0 │ 3      │ 0x7f20d0213c50 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
 │ None │ 0x959cc0       │ 6          │ 0x7f20d0213250 │         3 │ 0x7f20d0213c50 │ 9      │ 0x7f20d023c090 │ 8      │ 0x7f20d0213c90 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
 │ None │ 0x959cc0       │ 3          │ 0x7f20d0213c50 │         8 │ 0x7f20d0213c90 │ 5      │ 0x7f20d005bcd0 │ None   │ 0x959cc0       │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
@@ -1492,15 +1492,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════╤════════════════╤════════════╤════════════════╤═══════════╤════════════════╤════════╤════════════════╤════════╤════════════════╕
-│   up │ up @           │   previous │ previous @     │   current │ current @      │   down │ down @         │   next │ next @         │
+│   Up │ Up @           │   Previous │ Previous @     │   Current │ Current @      │   Down │ Down @         │   Next │ Next @         │
 ╞══════╪════════════════╪════════════╪════════════════╪═══════════╪════════════════╪════════╪════════════════╪════════╪════════════════╡
 │    7 │ 0x7f01e6153ad0 │          8 │ 0x7f01e6317cd0 │         6 │ 0x7f01e6316250 │      1 │ 0x7f01e6317d10 │      3 │ 0x7f01e6317c90 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
 │    2 │ 0x7f01e6153dd0 │          6 │ 0x7f01e6316250 │         3 │ 0x7f01e6317c90 │      9 │ 0x7f01e632bfd0 │      8 │ 0x7f01e6317cd0 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
 │    4 │ 0x7f01e6153d10 │          3 │ 0x7f01e6317c90 │         8 │ 0x7f01e6317cd0 │      5 │ 0x7f01e6153c90 │      6 │ 0x7f01e6316250 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
```

### Comparing `linkedit-1.0.5/linkedit/__init__.py` & `linkedit-1.0.7/linkedit/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,116 +68,56 @@
 
 
 # for the background coloring
 _BG_RED: str = "\033[41m"
 _RESET: str = "\033[0m"
 
 
-class singlyLinkedListNode:
+class _singlyLinkedListNode:
     def __init__(
-        self: "singlyLinkedListNode",
-        data: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        self: "_singlyLinkedListNode",
+        data: object,
     ) -> None:
-        self.data: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ) = data
-        self.next: singlyLinkedListNode | None = None
+        self.data: object = data
+        self.next: _singlyLinkedListNode | None = None
 
     def get_data(
-        self: "singlyLinkedListNode",
-    ) -> object | int | float | complex | str | list | tuple | set | dict | None | bool:
+        self: "_singlyLinkedListNode",
+    ) -> object:
         return self.data
 
-    def next_node(self: "singlyLinkedListNode") -> "singlyLinkedListNode":
+    def next_node(self: "_singlyLinkedListNode") -> "_singlyLinkedListNode":
         return self.next
 
 
-class doublyLinkedListNode:
+class _doublyLinkedListNode:
     def __init__(
-        self: "doublyLinkedListNode",
-        data: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        self: "_doublyLinkedListNode",
+        data: object,
     ) -> None:
-        self.data: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ) = data
-        self.prev: doublyLinkedListNode | None = None
-        self.next: doublyLinkedListNode | None = None
+        self.data: object = data
+        self.prev: _doublyLinkedListNode | None = None
+        self.next: _doublyLinkedListNode | None = None
 
     def get_data(
-        self: "doublyLinkedListNode",
-    ) -> object | int | float | complex | str | list | tuple | set | dict | None | bool:
+        self: "_doublyLinkedListNode",
+    ) -> object:
         return self.data
 
-    def prev_node(self: "doublyLinkedListNode") -> "doublyLinkedListNode":
+    def prev_node(self: "_doublyLinkedListNode") -> "_doublyLinkedListNode":
         return self.prev
 
-    def next_node(self: "doublyLinkedListNode") -> "doublyLinkedListNode":
+    def next_node(self: "_doublyLinkedListNode") -> "_doublyLinkedListNode":
         return self.next
 
 
 class _linkedList:
     def __init__(
         self: object,
-        data: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ) = None,
+        data: object = None,
         *,
         circular: bool = False,
         detail: bool = False,
         base: int = 16,
         reverse: bool = False,
     ) -> None:
         """constructor special method"""
@@ -186,39 +126,27 @@
         if self.detail:
             self.base: int = base
         else:
             # if detail is not true we assign directely the default base 16 hexa
             self._base: int = 16
         # O(1) len (track the object)
         self.len: int = 0
-        self._tail: singlyLinkedListNode | doublyLinkedListNode | None = None
-        self.head: singlyLinkedListNode | doublyLinkedListNode | None = data
+        self._tail: _singlyLinkedListNode | _doublyLinkedListNode | None = None
+        self.head: _singlyLinkedListNode | _doublyLinkedListNode | None = data
         self.rev: bool = reverse
 
     def __len__(self: object) -> int:
         """length special method"""
         return self.len
 
     def __contains__(
         self: object,
-        item: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        item: object,
     ) -> bool:
-        head: singlyLinkedListNode | doublyLinkedListNode = self._head
+        head: _singlyLinkedListNode | _doublyLinkedListNode = self._head
         for _ in range(self.len):
             if head.data == item:
                 return True
             head: object | None = head.next
         return False
 
     def __mul__(self: object, other: int) -> object:
@@ -226,36 +154,24 @@
             raise ValueError("Unsupported operand type for *")
         if self.isEmpty():
             for _ in range(other):
                 self.append(None)
         else:
             length = self.len
             for _ in range(other - 1):
-                head: singlyLinkedListNode | doublyLinkedListNode = self._head
+                head: _singlyLinkedListNode | _doublyLinkedListNode = self._head
                 for _ in range(length):
                     self.append(head.data)
                     head = head.next
         return self
 
     def __setitem__(
         self: object,
         index: int,
-        value: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        value: object,
     ) -> None:
         self.node(index).data = value
 
     def __eq__(
         self: object,
         other: object,
     ) -> bool:
@@ -263,25 +179,25 @@
             if id(self) == id(other):
                 return True
             elif len(self) != len(other):
                 return False
             elif len(self) == 0 and len(other) == 0:
                 return True
             else:
-                head1: singlyLinkedListNode | doublyLinkedListNode = self._head
-                head2: singlyLinkedListNode | doublyLinkedListNode = other._head
+                head1: _singlyLinkedListNode | _doublyLinkedListNode = self._head
+                head2: _singlyLinkedListNode | _doublyLinkedListNode = other._head
                 for _ in range(len(self)):
                     if head1.data == head2.data:
                         pass
                     else:
                         return False
-                    head1: singlyLinkedListNode | doublyLinkedListNode | None = (
+                    head1: _singlyLinkedListNode | _doublyLinkedListNode | None = (
                         head1.next
                     )
-                    head2: singlyLinkedListNode | doublyLinkedListNode | None = (
+                    head2: _singlyLinkedListNode | _doublyLinkedListNode | None = (
                         head2.next
                     )
                 return True
         else:
             return False
 
     def __gt__(
@@ -343,15 +259,15 @@
                     + _white(", ")
                     + _red(f"{base} ")
                     + _white("not a valid base")
                 )
             else:
                 self._base: int = base
 
-    def node(self: object, index: int) -> singlyLinkedListNode | doublyLinkedListNode:
+    def node(self: object, index: int) -> _singlyLinkedListNode | _doublyLinkedListNode:
         """node(s) searching method"""
         if not isinstance(index, int):
             if not self.circular:
                 raise TypeError(
                     "non circular singly linked list indices must be integers"
                 )
             else:
@@ -373,104 +289,70 @@
                             raise IndexError(
                                 "non circular singly linked list index out of range"
                             )
                         else:
                             raise IndexError(
                                 "circular singly linked list index out of range"
                             )
-                head: singlyLinkedListNode | doublyLinkedListNode = self._head
+                head: _singlyLinkedListNode | _doublyLinkedListNode = self._head
                 if index == self.len - 1:
                     return self._tail
                 for _ in range(index):
-                    head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
+                    head: _singlyLinkedListNode | _doublyLinkedListNode | None = (
+                        head.next
+                    )
                 return head
 
     @property
     def tail(
         self: object,
-    ) -> singlyLinkedListNode | doublyLinkedListNode:
+    ) -> _singlyLinkedListNode | _doublyLinkedListNode:
         return self._tail
 
     @tail.deleter
     def tail(self: object) -> None:
         self._tail = None
 
     def isEmpty(self: object) -> bool:
         return not self._head
 
     def index(
         self: object,
-        value: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        value: object,
     ) -> int:
         """Return first index of value.
 
         Raises ValueError if the value is not present."""
-        head: singlyLinkedListNode | doublyLinkedListNode | None = self._head
+        head: _singlyLinkedListNode | _doublyLinkedListNode | None = self._head
         for i in range(self.len):
             if head.data == value:
                 return i
-            head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
+            head: _singlyLinkedListNode | _doublyLinkedListNode | None = head.next
         if not self.circular:
             error_msg: str = f"{value} is not in the non circular linked list"
             raise ValueError(error_msg)
         else:
             error_msg: str = f"{value} is not in the circular linked list"
             raise ValueError(error_msg)
 
     def clear(self: object) -> None:
         self._head: None = None
         self._tail: None = None
         self.len: int = 0
 
     def append(
         self: object,
-        data: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        data: object,
     ) -> None:
         """Append object to the end of the linked list."""
         self.insert(self.len, data)
 
     def remove(
         self: object,
-        value: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        value: object,
     ) -> None:
         """Remove first occurrence of value.
 
         Raises ValueError if the value is not present."""
         node_index: int = self.index(value)
         try:
             self.pop(node_index)
@@ -490,176 +372,142 @@
 
         The sort is in-place (i.e. the linked list itself is modified) and stable (i.e. the order of two equal elements is maintained).
 
         If a key function is given, apply it once to each linked list item and sort them, ascending or descending, according to their function values.
 
         The reverse flag can be set to sort in descending order."""
         non_sorted_list: list = []
-        head: singlyLinkedListNode | doublyLinkedListNode | None = self._head
+        head: _singlyLinkedListNode | _doublyLinkedListNode | None = self._head
         if self.len >= 1:
             for _ in range(self.len - 1):
                 if type(head.data) == type(head.next.data):
                     non_sorted_list.append(head.data)
-                    head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
+                    head: _singlyLinkedListNode | _doublyLinkedListNode | None = (
+                        head.next
+                    )
                 else:
                     raise TypeError(
                         f"'<' not supported between instances of '{type(head.data).__name__}' and '{type(head.next.data).__name__}'"
                     )
             non_sorted_list.append(head.data)
             non_sorted_list.sort(reverse=reverse)
-            head: singlyLinkedListNode | doublyLinkedListNode = self._head
+            head: _singlyLinkedListNode | _doublyLinkedListNode = self._head
             for i in range(self.len):
                 head.data = non_sorted_list[i]
-                head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
+                head: _singlyLinkedListNode | _doublyLinkedListNode | None = head.next
 
     def count(
         self: object,
-        value: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        value: object,
     ) -> int:
         """Return number of occurrences of value."""
-        head: singlyLinkedListNode | doublyLinkedListNode | None = self._head
+        head: _singlyLinkedListNode | _doublyLinkedListNode | None = self._head
         counter: int = 0
         if self.len >= 1:
             for _ in range(self.len):
                 if head.data == value:
                     counter += 1
-                head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
+                head: _singlyLinkedListNode | _doublyLinkedListNode | None = head.next
             return counter
 
     def right_shift(self: object, rotate: int) -> None:
         if not isinstance(rotate, int):
             raise TypeError("rotate must be an integer")
         helper1: list = []
         helper2: list = []
-        head: singlyLinkedListNode | doublyLinkedListNode | None = self._head
+        head: _singlyLinkedListNode | _doublyLinkedListNode | None = self._head
         try:
             rotate: int = rotate % self.len
         except ZeroDivisionError as e1:
             return
         for _ in range(self.len - rotate):
             helper1.append(head.data)
-            head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
+            head: _singlyLinkedListNode | _doublyLinkedListNode | None = head.next
         for _ in range(self.len - rotate, self.len):
             helper2.append(head.data)
-            head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
-        head: singlyLinkedListNode | doublyLinkedListNode | None = self._head
+            head: _singlyLinkedListNode | _doublyLinkedListNode | None = head.next
+        head: _singlyLinkedListNode | _doublyLinkedListNode | None = self._head
         helper2.extend(helper1)
         for i in range(self.len):
             head.data = helper2[i]
-            head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
+            head: _singlyLinkedListNode | _doublyLinkedListNode | None = head.next
 
     def left_shift(self: object, rotate: int) -> None:
         if not isinstance(rotate, int):
             raise TypeError("rotate must be an integer")
         helper1: list = []
         helper2: list = []
-        head: singlyLinkedListNode | doublyLinkedListNode | None = self._head
+        head: _singlyLinkedListNode | _doublyLinkedListNode | None = self._head
         try:
             rotate: int = rotate % self.len
         except ZeroDivisionError as e2:
             return
         for _ in range(rotate):
             helper1.append(head.data)
-            head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
+            head: _singlyLinkedListNode | _doublyLinkedListNode | None = head.next
         for _ in range(rotate, self.len):
             helper2.append(head.data)
-            head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
+            head: _singlyLinkedListNode | _doublyLinkedListNode | None = head.next
         head: object | None = self._head
         helper2.extend(helper1)
         for i in range(self.len):
             head.data = helper2[i]
-            head: singlyLinkedListNode | doublyLinkedListNode | None = head.next
+            head: _singlyLinkedListNode | _doublyLinkedListNode | None = head.next
 
     def prepend(
         self: object,
-        data: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        data: object,
     ) -> None:
         self.insert(0, data)
 
 
 class singlyLinkedList(_linkedList):
     @property
     def head(
         self: "singlyLinkedList",
-    ) -> singlyLinkedListNode:
+    ) -> _singlyLinkedListNode:
         return self._head
 
     @head.setter
     def head(
         self: "singlyLinkedList",
-        data: (
-            object
-            | int
-            | float
-            | str
-            | complex
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        data: object,
     ) -> None:
         self._head: None = None
         if isinstance(data, singlyLinkedList):
-            self._head: singlyLinkedListNode | None = data._head
-        elif isinstance(data, singlyLinkedListNode):
-            old_head: singlyLinkedListNode = data
-            old_self_head: singlyLinkedListNode = data
-            new_head: singlyLinkedListNode = singlyLinkedListNode(data.data)
-            self._head: singlyLinkedListNode = new_head
+            self._head: _singlyLinkedListNode | None = data._head
+        elif isinstance(data, _singlyLinkedListNode):
+            old_head: _singlyLinkedListNode = data
+            old_self_head: _singlyLinkedListNode = data
+            new_head: _singlyLinkedListNode = _singlyLinkedListNode(data.data)
+            self._head: _singlyLinkedListNode = new_head
             self.len += 1
-            old_head: singlyLinkedListNode | None = old_head.next
+            old_head: _singlyLinkedListNode | None = old_head.next
             while old_head and old_head != old_self_head:
-                new_node: singlyLinkedListNode = singlyLinkedListNode(old_head.data)
+                new_node: _singlyLinkedListNode = _singlyLinkedListNode(old_head.data)
                 self.len += 1
                 new_head.next = new_node
-                new_head: singlyLinkedListNode | None = new_head.next
-                old_head: singlyLinkedListNode | None = old_head.next
+                new_head: _singlyLinkedListNode | None = new_head.next
+                old_head: _singlyLinkedListNode | None = old_head.next
             if self.circular:
                 new_node.next = self._head
-            self._tail: singlyLinkedListNode = new_node
+            self._tail: _singlyLinkedListNode = new_node
         else:
             try:
                 if len(data) > 0:
                     for i in data:
                         self.append(i)
             except TypeError as e3:
                 if data is not None:
-                    new_node: singlyLinkedListNode = singlyLinkedListNode(data)
+                    new_node: _singlyLinkedListNode = _singlyLinkedListNode(data)
                     self.len += 1
-                    self._head: singlyLinkedListNode = new_node
+                    self._head: _singlyLinkedListNode = new_node
                     if self.circular:
                         new_node.next = new_node
-                    self._tail: singlyLinkedListNode = new_node
+                    self._tail: _singlyLinkedListNode = new_node
 
     @head.deleter
     def head(self: "singlyLinkedList") -> None:
         self._head: None = None
 
     def copy(self: "singlyLinkedList") -> "singlyLinkedList":
         """Return a shallow copy of the non circular/circular singly linked list."""
@@ -676,66 +524,54 @@
 
     def set_non_circular(self: "singlyLinkedList") -> None:
         self._tail.next = None
         self.circular: bool = False
 
     def __add__(
         self: "singlyLinkedList",
-        other: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        other: object,
     ) -> None:
         helper: list = []
-        head1: singlyLinkedListNode | None = self._head
+        head1: _singlyLinkedListNode | None = self._head
         if isinstance(other, singlyLinkedList) or isinstance(other, doublyLinkedList):
-            head2: singlyLinkedListNode | None = other._head
+            head2: _singlyLinkedListNode | None = other._head
         else:
             other: singlyLinkedList = singlyLinkedList(other)
-            head2: singlyLinkedListNode = other._head
+            head2: _singlyLinkedListNode = other._head
         for _ in range(self.len):
             helper.append(head1.data)
-            head1: singlyLinkedListNode | None = head1.next
+            head1: _singlyLinkedListNode | None = head1.next
         for _ in range(other.len):
             helper.append(head2.data)
-            head2: singlyLinkedListNode | None = head2.next
+            head2: _singlyLinkedListNode | None = head2.next
         return singlyLinkedList(helper, circular=other.circular)
 
     def __str__(self: "singlyLinkedList") -> str:
         """Return str(self)."""
         if not self._head:
             if not self.circular:
                 raise TypeError("Empty non circular singly linked list")
             else:
                 raise TypeError("Empty circular singly linked list")
         else:
-            head: singlyLinkedListNode = self._head
+            head: _singlyLinkedListNode = self._head
             linked_list: list = []
             counter: int = 0
             if not self.detail:
                 while head and head.next != self._head:
                     if isinstance(head.data, str):
                         if len(head.data) == 0:
                             linked_list.append(f"[{head.data}] -> ")
                         elif len(head.data) == 1:
                             linked_list.append(f"['{head.data}'] -> ")
                         else:
                             linked_list.append(f'["{head.data}"] -> ')
                     else:
                         linked_list.append(f"[{head.data}] -> ")
-                    head: singlyLinkedListNode | None = head.next
+                    head: _singlyLinkedListNode | None = head.next
                 if not self.circular:
                     linked_list.append("None (NULL)")
                 else:
                     linked_list.insert(0, "> ")
                     if isinstance(head.data, str):
                         if len(head.data) == 0:
                             linked_list.append(f"[{head.data}]")
@@ -746,18 +582,18 @@
                     else:
                         linked_list.append(f"[{head.data}]")
                     linked_list.append(" -")
                 return "".join(linked_list)
             else:
                 linked_list.append(
                     [
-                        _white("current value"),
-                        _white("current value ") + _green("@") + _white("ddress"),
-                        _white("next value"),
-                        _white("next value ") + _green("@") + _white("ddress"),
+                        _white("Current Value"),
+                        _white("Current Value ") + _green("@") + _white("ddress"),
+                        _white("Next Value"),
+                        _white("Next Value ") + _green("@") + _white("ddress"),
                     ]
                 )
                 if head.next == self._head:
                     linked_list.append(
                         [
                             (
                                 _blue(f"{head.data}")
@@ -829,15 +665,15 @@
                                         _red("0") if self._base == 10 else _red("0x0")
                                     )
                                 )
                             )
                             + _white(")"),
                         ]
                     )
-                    head: singlyLinkedListNode | None = head.next
+                    head: _singlyLinkedListNode | None = head.next
                 else:
                     linked_list.append(
                         [
                             (
                                 _blue(f"{head.data}")
                                 if not isinstance(head.data, str)
                                 else (
@@ -863,15 +699,15 @@
                                         else f"{head.next.data}"
                                     )
                                 )
                             ),
                             f"{_yellow(bin(id(head.next)) if self._base == 2 else oct(id(head.next)) if self._base == 8 else id(head.next) if self._base == 10 else hex(id(head.next)))}",
                         ]
                     )
-                    head: singlyLinkedListNode | None = head.next
+                    head: _singlyLinkedListNode | None = head.next
                     while head and head.next != self._head:
                         first: str = (
                             f"{(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))}"
                         )
                         second: str = (
                             f"{bin(id(head.next)) if self._base == 2 else oct(id(head.next)) if self._base == 8 else id(head.next) if self._base == 10 else hex(id(head.next))}"
                             + (" " if head.next is None else "")
@@ -957,15 +793,15 @@
                                         if second.endswith(" ")
                                         else _yellow(second)
                                     )
                                 ),
                             ]
                         )
                         counter += 1
-                        head: singlyLinkedListNode | None = head.next
+                        head: _singlyLinkedListNode | None = head.next
                     if self.circular:
                         first: str = (
                             f"{(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))}"
                         )
                         second: str = (
                             f"{bin(id(head.next)) if self._base == 2 else oct(id(head.next)) if self._base == 8 else id(head.next) if self._base == 10 else hex(id(head.next))}"
                         )
@@ -1053,217 +889,139 @@
                         ]
                     )
                 return tabulate(linked_list, headers="firstrow", tablefmt="fancy_grid")
 
     def insert(
         self: "singlyLinkedList",
         index: int,
-        data: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        data: object,
     ) -> None:
         """Insert object before index."""
         if not isinstance(index, int):
             raise TypeError("index must be an integer")
         if not self._head:
-            new_node: singlyLinkedListNode = singlyLinkedListNode(data)
-            self._head: singlyLinkedListNode = new_node
+            new_node: _singlyLinkedListNode = _singlyLinkedListNode(data)
+            self._head: _singlyLinkedListNode = new_node
             self.len += 1
-            self._tail: singlyLinkedListNode = new_node
+            self._tail: _singlyLinkedListNode = new_node
             if self.circular:
                 self._head.next = self._head
         else:
             if index == 0:
-                new_node: singlyLinkedListNode = singlyLinkedListNode(data)
+                new_node: _singlyLinkedListNode = _singlyLinkedListNode(data)
                 self.len += 1
                 new_node.next = self._head
                 if self.circular:
                     self._tail.next = new_node
                 self._head: object = new_node
             elif index >= self.len:
-                new_node: singlyLinkedListNode = singlyLinkedListNode(data)
+                new_node: _singlyLinkedListNode = _singlyLinkedListNode(data)
                 self._tail.next = new_node
                 if self.circular:
                     new_node.next = self._head
                 self.len += 1
-                self._tail: singlyLinkedListNode = new_node
+                self._tail: _singlyLinkedListNode = new_node
             else:
                 if index < 0:
                     if index > -self.len:
                         index = self.len + index
                     else:
                         self.insert(0, data)
                         return
-                new_node: singlyLinkedListNode = singlyLinkedListNode(data)
-                prev_head: singlyLinkedListNode = self.node(index - 1)
+                new_node: _singlyLinkedListNode = _singlyLinkedListNode(data)
+                prev_head: _singlyLinkedListNode = self.node(index - 1)
                 new_node.next = prev_head.next
                 prev_head.next = new_node
                 self.len += 1
 
-    def pop(
-        self: "singlyLinkedList", index: int = -1
-    ) -> object | int | float | complex | str | list | tuple | set | dict | None | bool:
+    def pop(self: "singlyLinkedList", index: int = -1) -> object:
         """Remove and return item at index (default last).
 
         Raises IndexError if list is empty or index is out of range."""
         if not isinstance(index, int):
             raise TypeError("index must be an integer")
         if not self._head:
             if not self.circular:
                 raise IndexError("pop from empty non circular singly linked list")
             else:
                 raise IndexError("pop from empty circular singly linked list")
         else:
-            head: singlyLinkedListNode = self._head
+            head: _singlyLinkedListNode = self._head
             if index == 0 or index == -self.len:
-                old_head_value: (
-                    object
-                    | int
-                    | float
-                    | complex
-                    | str
-                    | list
-                    | tuple
-                    | set
-                    | dict
-                    | None
-                    | bool
-                ) = self._head.data
-                old_head: singlyLinkedListNode = self._head
+                old_head_value: object = self._head.data
+                old_head: _singlyLinkedListNode = self._head
                 if not self.circular:
-                    self._head: singlyLinkedListNode = head.next
+                    self._head: _singlyLinkedListNode = head.next
                     if self.len == 1:
                         self._tail: None = None
                     self.len -= 1
                 else:
                     if self._head != head.next:
                         self._tail.next = head.next
-                        self._head: singlyLinkedListNode = head.next
+                        self._head: _singlyLinkedListNode = head.next
                     else:
                         self._head: None = None
                         self._tail: None = None
                     self.len -= 1
                 del old_head
                 return old_head_value
             elif index == -1 or index == self.len - 1:
-                prev_current: singlyLinkedListNode = self.node(index - 1)
-                removed_node_value: (
-                    object
-                    | int
-                    | float
-                    | complex
-                    | str
-                    | list
-                    | tuple
-                    | set
-                    | dict
-                    | None
-                    | bool
-                ) = prev_current.next.data
-                removed_node: singlyLinkedListNode = prev_current.next
+                prev_current: _singlyLinkedListNode = self.node(index - 1)
+                removed_node_value: object = prev_current.next.data
+                removed_node: _singlyLinkedListNode = prev_current.next
                 if self.circular:
                     prev_current.next = self._head
                 else:
                     prev_current.next = None
                 self.len -= 1
-                self._tail: singlyLinkedListNode = prev_current
+                self._tail: _singlyLinkedListNode = prev_current
                 del removed_node
                 return removed_node_value
             elif index > self.len - 1 or index < -self.len:
                 raise IndexError("pop index out of range")
             else:
-                prev_node: singlyLinkedListNode = self.node(index - 1)
-                removed_node_value: (
-                    object
-                    | int
-                    | float
-                    | complex
-                    | str
-                    | list
-                    | tuple
-                    | set
-                    | dict
-                    | None
-                    | bool
-                ) = prev_node.next.data
-                removed_node: singlyLinkedListNode = prev_node.next
+                prev_node: _singlyLinkedListNode = self.node(index - 1)
+                removed_node_value: object = prev_node.next.data
+                removed_node: _singlyLinkedListNode = prev_node.next
                 prev_node.next = prev_node.next.next
                 self.len -= 1
                 del removed_node
                 return removed_node_value
 
     def extend(
         self: "singlyLinkedList",
-        extended_object: (
-            singlyLinkedListNode
-            | object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        extended_object: object,
     ) -> None:
         """Extend non circular/circular singly linked list by appending elements from the iterable."""
         if isinstance(extended_object, singlyLinkedList):
-            first_last_node: singlyLinkedListNode | None = self._tail
-            second_first_node: singlyLinkedListNode | None = extended_object._head
+            first_last_node: _singlyLinkedListNode | None = self._tail
+            second_first_node: _singlyLinkedListNode | None = extended_object._head
             for _ in range(extended_object.len):
-                new_node: singlyLinkedListNode = singlyLinkedListNode(
+                new_node: _singlyLinkedListNode = _singlyLinkedListNode(
                     second_first_node.data
                 )
                 first_last_node.next = new_node
-                first_last_node: singlyLinkedListNode = first_last_node.next
-                second_first_node: singlyLinkedListNode | None = second_first_node.next
+                first_last_node: _singlyLinkedListNode = first_last_node.next
+                second_first_node: _singlyLinkedListNode | None = second_first_node.next
             self.len += extended_object.len
             if self.circular:
                 first_last_node.next = self._head
         else:
             extended_linked_list: singlyLinkedList = singlyLinkedList(extended_object)
             self.extend(extended_linked_list)
 
-    def __getitem__(
-        self: "singlyLinkedList", index: int
-    ) -> (
-        object
-        | str
-        | int
-        | complex
-        | float
-        | list
-        | tuple
-        | set
-        | dict
-        | None
-        | bool
-        | object
-    ):
+    def __getitem__(self: "singlyLinkedList", index: int) -> object:
         if not isinstance(index, slice):
             return self.node(index).data
         else:
-            head: singlyLinkedListNode | None = self._head
+            head: _singlyLinkedListNode | None = self._head
             new_list: list = []
             for _ in range(self.len):
                 new_list.append(head.data)
-                head: singlyLinkedListNode | None = head.next
+                head: _singlyLinkedListNode | None = head.next
             try:
                 new_list: list = new_list[index.start : index.stop : index.step]
                 return singlyLinkedList(
                     new_list,
                     detail=self.detail,
                     circular=self.circular,
                     base=self._base,
@@ -1275,96 +1033,73 @@
             )
 
     def to_doubly(self: "singlyLinkedList") -> "doublyLinkedList":
         return doublyLinkedList() + self
 
     def add(
         self: "singlyLinkedList",
-        data: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        data: object,
     ) -> None:
         """To add in an organized manner"""
         if not self._head:
-            self._head: singlyLinkedListNode = singlyLinkedListNode(data)
+            self._head: _singlyLinkedListNode = _singlyLinkedListNode(data)
             self.len += 1
-            self._tail: singlyLinkedListNode = self._head
+            self._tail: _singlyLinkedListNode = self._head
             if self.circular:
                 self._head.next = self._head
         else:
-            head: singlyLinkedListNode = self._head
-            prev_head: singlyLinkedListNode | None = None
+            head: _singlyLinkedListNode = self._head
+            prev_head: _singlyLinkedListNode | None = None
             for i in range(self.len):
                 if type(head.data) != type(data):
                     raise TypeError(
                         f"'<' not supported between instances of '{type(head.data).__name__}' and '{type(data).__name__}'"
                     )
                 else:
                     if not self.rev:
                         if data < head.data:
                             if i == 0 or i == self.len - 1:
                                 self.insert(i, data)
                                 break
                             else:
-                                new_node: singlyLinkedListNode = singlyLinkedListNode(
+                                new_node: _singlyLinkedListNode = _singlyLinkedListNode(
                                     data
                                 )
                                 new_node.next = head
                                 prev_head.next = new_node
                                 self.len += 1
                                 break
                         else:
-                            prev_head: singlyLinkedListNode = head
+                            prev_head: _singlyLinkedListNode = head
                             head = head.next
                     else:
                         if data > head.data:
                             if i == 0 or i == self.len - 1:
                                 self.insert(i, data)
                                 break
                             else:
-                                new_node: singlyLinkedListNode = singlyLinkedListNode(
+                                new_node: _singlyLinkedListNode = _singlyLinkedListNode(
                                     data
                                 )
                                 new_node.next = head
                                 prev_head.next = new_node
                                 self.len += 1
                                 break
                         else:
-                            prev_head: singlyLinkedListNode = head
-                            head: singlyLinkedListNode = head.next
+                            prev_head: _singlyLinkedListNode = head
+                            head: _singlyLinkedListNode = head.next
             else:
                 self.insert(self.len, data)
 
     def to_dict(self: "singlyLinkedList", node: bool = False) -> dict:
-        head: singlyLinkedListNode | None = self._head
+        head: _singlyLinkedListNode | None = self._head
         new_dict: dict = {}
         for _ in range(self.len):
             try:
-                next_value: (
-                    int
-                    | float
-                    | complex
-                    | str
-                    | list
-                    | tuple
-                    | set
-                    | dict
-                    | None
-                    | bool
-                ) = head.next.data
+                next_value: object = head.next.data
             except AttributeError as e6:
                 next_value: None = None
             new_dict[head.data] = {
                 "current value @ddress" if not node else "current node": (
                     (
                         (
                             bin(id(head))
@@ -1394,93 +1129,81 @@
                             )
                         )
                     )
                     if not node
                     else head.next
                 ),
             }
-            head: singlyLinkedListNode | None = head.next
+            head: _singlyLinkedListNode | None = head.next
         return new_dict
 
     def reverse(self: "singlyLinkedList") -> None:
-        head: singlyLinkedListNode | None = self._head
+        head: _singlyLinkedListNode | None = self._head
         elements: list = []
         for _ in range(self.len):
             elements.append(head.data)
-            head: singlyLinkedListNode | None = head.next
-        head: singlyLinkedListNode | None = self._head
+            head: _singlyLinkedListNode | None = head.next
+        head: _singlyLinkedListNode | None = self._head
         for i in range(1, self.len + 1):
             head.data = elements[-i]
-            head: singlyLinkedListNode | None = head.next
+            head: _singlyLinkedListNode | None = head.next
 
 
 class sll(singlyLinkedList):
     pass
 
 
 class doublyLinkedList(_linkedList):
     @property
     def head(
         self: "doublyLinkedList",
-    ) -> doublyLinkedListNode:
+    ) -> _doublyLinkedListNode:
         return self._head
 
     @head.setter
     def head(
         self: "doublyLinkedList",
-        data: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        data: object,
     ) -> None:
         self._head: None = None
         if isinstance(data, doublyLinkedList):
-            self._head: doublyLinkedListNode | None = data._head
-        elif isinstance(data, doublyLinkedListNode):
-            old_head: doublyLinkedListNode = data
-            old_self_head: doublyLinkedListNode = data
-            new_head: doublyLinkedListNode = doublyLinkedListNode(data.data)
+            self._head: _doublyLinkedListNode | None = data._head
+        elif isinstance(data, _doublyLinkedListNode):
+            old_head: _doublyLinkedListNode = data
+            old_self_head: _doublyLinkedListNode = data
+            new_head: _doublyLinkedListNode = _doublyLinkedListNode(data.data)
             if self.circular:
                 new_head.prev = data.prev
-            self._head: doublyLinkedListNode = new_head
+            self._head: _doublyLinkedListNode = new_head
             self.len += 1
-            old_head: doublyLinkedListNode | None = old_head.next
+            old_head: _doublyLinkedListNode | None = old_head.next
             while old_head and old_head != old_self_head:
-                new_node: doublyLinkedListNode = doublyLinkedListNode(old_head.data)
+                new_node: _doublyLinkedListNode = _doublyLinkedListNode(old_head.data)
                 self.len += 1
                 new_head.next = new_node
                 new_node.prev = new_head
-                new_head: doublyLinkedListNode | None = new_head.next
-                old_head: doublyLinkedListNode | None = old_head.next
+                new_head: _doublyLinkedListNode | None = new_head.next
+                old_head: _doublyLinkedListNode | None = old_head.next
             if self.circular:
                 new_node.next = self._head
-            self._tail: doublyLinkedListNode = new_node
+            self._tail: _doublyLinkedListNode = new_node
         else:
             try:
                 if len(data) > 0:
                     for i in data:
                         self.append(i)
             except TypeError as e7:
                 if data is not None:
-                    new_node: doublyLinkedListNode = doublyLinkedListNode(data)
+                    new_node: _doublyLinkedListNode = _doublyLinkedListNode(data)
                     self.len += 1
-                    self._head: doublyLinkedListNode = new_node
+                    self._head: _doublyLinkedListNode = new_node
                     if self.circular:
                         new_node.next = new_node
                         new_node.prev = new_node
-                    self._tail: doublyLinkedListNode = new_node
+                    self._tail: _doublyLinkedListNode = new_node
 
     @head.deleter
     def head(self: "doublyLinkedList") -> None:
         self._head: None = None
 
     def set_circular(self: "doublyLinkedList") -> None:
         self._tail.next = self._head
@@ -1490,52 +1213,40 @@
     def set_non_circular(self: "doublyLinkedList") -> None:
         self._tail.next = None
         self._head.prev = None
         self.circular: bool = False
 
     def __add__(
         self: "doublyLinkedList",
-        other: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        other: object,
     ) -> None:
         helper: list = []
-        head1: doublyLinkedListNode | None = self._head
+        head1: _doublyLinkedListNode | None = self._head
         if isinstance(other, doublyLinkedList) or isinstance(other, singlyLinkedList):
-            head2: doublyLinkedListNode | None = other._head
+            head2: _doublyLinkedListNode | None = other._head
         else:
-            other: doublyLinkedListNode = doublyLinkedList(other)
-            head2: doublyLinkedListNode = other._head
+            other: _doublyLinkedListNode = doublyLinkedList(other)
+            head2: _doublyLinkedListNode = other._head
         for _ in range(self.len):
             helper.append(head1.data)
-            head1: doublyLinkedListNode | None = head1.next
+            head1: _doublyLinkedListNode | None = head1.next
         for _ in range(other.len):
             helper.append(head2.data)
-            head2: doublyLinkedListNode | None = head2.next
+            head2: _doublyLinkedListNode | None = head2.next
         return doublyLinkedList(helper, circular=other.circular)
 
     def __str__(self: "doublyLinkedList") -> str:
         """Return str(self)."""
         if not self._head:
             if not self.circular:
                 raise TypeError("Empty non circular doubly linked list")
             else:
                 raise TypeError("Empty circular doubly linked list")
         else:
-            head: doublyLinkedListNode = self._head
+            head: _doublyLinkedListNode = self._head
             linked_list: list = []
             counter: int = 0
             if not self.detail:
                 if not self.circular:
                     linked_list.append("None (NULL) <- ")
                 else:
                     linked_list.append("=> ")
@@ -1553,15 +1264,15 @@
                             linked_list.append(
                                 f"['{head.data}'] " + ("<=> " if head.next else "-> ")
                             )
                         else:
                             linked_list.append(
                                 f'["{head.data}"] ' + ("<=> " if head.next else "-> ")
                             )
-                    head: doublyLinkedListNode | None = head.next
+                    head: _doublyLinkedListNode | None = head.next
                 if not self.circular:
                     if self.len > 1:
                         linked_list.append("None (NULL)")
                     else:
                         try:
                             if not isinstance(head.data, str):
                                 linked_list.append(f"[{head.data}] -> None (NULL)")
@@ -1588,20 +1299,20 @@
                             linked_list.append(f"['{head.data}'] <=")
                         else:
                             linked_list.append(f'["{head.data}"] <=')
                 return "".join(linked_list)
             else:
                 linked_list.append(
                     [
-                        _white("previous value"),
-                        _white("previous value ") + _green("@") + _white("ddress"),
-                        _white("current value"),
-                        _white("current value ") + _green("@") + _white("ddress"),
-                        _white("next value"),
-                        _white("next value ") + _green("@") + _white("ddress"),
+                        _white("Previous Value"),
+                        _white("Previous Value ") + _green("@") + _white("ddress"),
+                        _white("Current Value"),
+                        _white("Current Value ") + _green("@") + _white("ddress"),
+                        _white("Next Value"),
+                        _white("Next Value ") + _green("@") + _white("ddress"),
                     ]
                 )
                 if not self.circular:
                     linked_list.append(
                         [
                             _BG_RED + " " * len("previous value") + _RESET,
                             _BG_RED + " " * len("previous value @ddress") + _RESET,
@@ -1623,27 +1334,15 @@
                             )
                             + _white(")"),
                             _BG_RED + " " * len("next value") + _RESET,
                             _BG_RED + " " * len("next value @ddress") + _RESET,
                         ]
                     )
                 try:
-                    helper: (
-                        object
-                        | int
-                        | float
-                        | complex
-                        | str
-                        | list
-                        | tuple
-                        | set
-                        | dict
-                        | None
-                        | bool
-                    ) = head.next.data
+                    helper: object = head.next.data
                 except AttributeError as e9:
                     helper: None = None
                 linked_list.append(
                     [
                         (
                             f"{_blue('None')} {_green('(')}{_red('NULL')}{_green(')')}"
                             if not head.prev
@@ -1733,15 +1432,15 @@
                                 + _white(")")
                                 if head.next is None
                                 else ""
                             )
                         ),
                     ]
                 )
-                head: doublyLinkedListNode | None = head.next
+                head: _doublyLinkedListNode | None = head.next
                 while head and head.next != self._head:
                     first: str = (
                         f"{bin(id(head.prev)) if self._base == 2 else oct(id(head.prev)) if self._base == 8 else id(head.prev) if self._base == 10 else hex(id(head.prev))}"
                     )
                     second: str = (
                         f"{(bin(id(head)) if self._base == 2 else oct(id(head)) if self._base == 8 else id(head) if self._base == 10 else hex(id(head)))}"
                     )
@@ -1844,15 +1543,15 @@
                                     if last.endswith(" ")
                                     else _yellow(last)
                                 )
                             ),
                         ]
                     )
                     counter += 1
-                    head: doublyLinkedListNode | None = head.next
+                    head: _doublyLinkedListNode | None = head.next
                 if not self.circular:
                     linked_list.append(
                         [
                             _BG_RED + " " * len("previous value") + _RESET,
                             _BG_RED + " " * len("previous value @ddress") + _RESET,
                             f"{_blue('None')} {_green('(')}{_red('NULL')}{_green(')')}",
                             (
@@ -1963,25 +1662,23 @@
         return doublyLinkedList(
             self._head,
             detail=self.detail,
             circular=self.circular,
             base=self._base,
         )
 
-    def __getitem__(
-        self: "doublyLinkedList", index: int
-    ) -> object | str | int | complex | float | list | tuple | set | dict | None | bool:
+    def __getitem__(self: "doublyLinkedList", index: int) -> object:
         if not isinstance(index, slice):
             return self.node(index).data
         else:
-            head: doublyLinkedListNode | None = self._head
+            head: _doublyLinkedListNode | None = self._head
             new_list: list = []
             for _ in range(self.len):
                 new_list.append(head.data)
-                head: doublyLinkedListNode | None = head.next
+                head: _doublyLinkedListNode | None = head.next
             try:
                 new_list: list = new_list[index.start : index.stop : index.step]
                 return doublyLinkedList(
                     new_list,
                     detail=self.detail,
                     circular=self.circular,
                     base=self._base,
@@ -1991,303 +1688,204 @@
             raise TypeError(
                 "slice indices must be integers or None or have an __index__ method"
             )
 
     def insert(
         self: "doublyLinkedList",
         index: int,
-        data: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        data: object,
     ) -> None:
         """Insert object before index."""
         if not isinstance(index, int):
             raise TypeError("index must be an integer")
         if not self._head:
-            new_node: doublyLinkedListNode = doublyLinkedListNode(data)
-            self._head: doublyLinkedListNode = new_node
-            self._tail: doublyLinkedListNode = new_node
+            new_node: _doublyLinkedListNode = _doublyLinkedListNode(data)
+            self._head: _doublyLinkedListNode = new_node
+            self._tail: _doublyLinkedListNode = new_node
             self.len: int = 1
             if self.circular:
                 new_node.next = new_node
                 new_node.prev = new_node
         else:
             if index >= self.len:
-                new_node: doublyLinkedListNode = doublyLinkedListNode(data)
+                new_node: _doublyLinkedListNode = _doublyLinkedListNode(data)
                 self._tail.next = new_node
                 new_node.prev = self._tail
-                self._tail: doublyLinkedListNode = new_node
+                self._tail: _doublyLinkedListNode = new_node
                 if self.circular:
                     self._tail.next = self._head
                     self._head.prev = self._tail
                 self.len += 1
             elif index <= -self.len or index == 0:
-                new_node: doublyLinkedListNode = doublyLinkedListNode(data)
+                new_node: _doublyLinkedListNode = _doublyLinkedListNode(data)
                 new_node.next = self._head
                 self._head.prev = new_node
-                self._head: doublyLinkedListNode = new_node
+                self._head: _doublyLinkedListNode = new_node
                 if self.circular:
                     self._head.prev = self._tail
                     self._tail.next = self._head
                 self.len += 1
             else:
-                current: doublyLinkedListNode = self.node(index)
-                new_node: doublyLinkedListNode = doublyLinkedListNode(data)
+                current: _doublyLinkedListNode = self.node(index)
+                new_node: _doublyLinkedListNode = _doublyLinkedListNode(data)
                 new_node.prev = current.prev
                 new_node.next = current
                 current.prev.next = new_node
                 current.prev = new_node
                 self.len += 1
 
-    def pop(
-        self: "doublyLinkedList", index: int = -1
-    ) -> object | int | float | complex | str | list | tuple | set | dict | None | bool:
+    def pop(self: "doublyLinkedList", index: int = -1) -> object:
         """Remove and return item at index (default last).
 
         Raises IndexError if list is empty or index is out of range."""
         if not isinstance(index, int):
             raise TypeError("index must be an integer")
         if not self._head:
             if not self.circular:
                 raise IndexError("pop from empty non circular doubly linked list")
             else:
                 raise IndexError("pop from empty circular doubly linked list")
         else:
             if self.len > 1:
                 if index == -1 or index == self.len - 1:
-                    returned_value: (
-                        object
-                        | int
-                        | float
-                        | complex
-                        | str
-                        | list
-                        | tuple
-                        | set
-                        | dict
-                        | None
-                        | bool
-                    ) = self._tail.data
-                    removed_node: doublyLinkedListNode = self._tail
-                    self._tail: doublyLinkedListNode = self._tail.prev
+                    returned_value: object = self._tail.data
+                    removed_node: _doublyLinkedListNode = self._tail
+                    self._tail: _doublyLinkedListNode = self._tail.prev
                     if self.circular:
                         self._tail.next = self._head
                         self._head.prev = self._tail
                     else:
                         self._tail.next = None
                     self.len -= 1
                     del removed_node
                     return returned_value
                 elif index == 0 or index == -self.len:
-                    returned_value: (
-                        object
-                        | int
-                        | float
-                        | complex
-                        | str
-                        | list
-                        | tuple
-                        | set
-                        | dict
-                        | None
-                        | bool
-                    ) = self._head.data
-                    removed_node: doublyLinkedListNode = self._head
-                    self._head: doublyLinkedListNode = self._head.next
+                    returned_value: object = self._head.data
+                    removed_node: _doublyLinkedListNode = self._head
+                    self._head: _doublyLinkedListNode = self._head.next
                     if self.circular:
                         self._head.prev = self._tail
                         self._tail.next = self._head
                     else:
                         self._head.prev = None
                     self.len -= 1
                     del removed_node
                     return returned_value
                 elif index >= self.len or index < -self.len:
                     raise IndexError("pop index out of range")
                 else:
-                    current: doublyLinkedListNode = self.node(index)
-                    returned_value: (
-                        object
-                        | int
-                        | float
-                        | complex
-                        | str
-                        | list
-                        | tuple
-                        | set
-                        | dict
-                        | None
-                        | bool
-                    ) = current.data
+                    current: _doublyLinkedListNode = self.node(index)
+                    returned_value: object = current.data
                     current.prev.next = current.next
                     current.next.prev = current.prev
                     self.len -= 1
                     del current
                     return returned_value
             else:
                 if index == 0 or index == -1:
-                    returned_value: (
-                        object
-                        | int
-                        | float
-                        | complex
-                        | str
-                        | list
-                        | tuple
-                        | set
-                        | dict
-                        | None
-                        | bool
-                    ) = self._head.data
-                    removed_node: doublyLinkedListNode = self._head
+                    returned_value: object = self._head.data
+                    removed_node: _doublyLinkedListNode = self._head
                     self._head: None = None
                     self._tail: None = None
                     self.len: int = 0
                     del removed_node
                     return returned_value
                 else:
                     raise IndexError("pop index out of range")
 
     def extend(
         self: "doublyLinkedList",
-        extended_object: (
-            doublyLinkedListNode
-            | object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        extended_object: object,
     ) -> None:
         """Extend non circular/circular doubly linked list by appending elements from the iterable."""
         if isinstance(extended_object, doublyLinkedList):
-            first_last_node: doublyLinkedListNode | None = self._tail
-            second_first_node: doublyLinkedListNode | None = extended_object._head
+            first_last_node: _doublyLinkedListNode | None = self._tail
+            second_first_node: _doublyLinkedListNode | None = extended_object._head
             for _ in range(extended_object.len):
-                new_node: doublyLinkedListNode = doublyLinkedListNode(
+                new_node: _doublyLinkedListNode = _doublyLinkedListNode(
                     second_first_node.data
                 )
                 first_last_node.next = new_node
                 new_node.prev = first_last_node
-                first_last_node: doublyLinkedListNode = first_last_node.next
-                second_first_node: doublyLinkedListNode | None = second_first_node.next
+                first_last_node: _doublyLinkedListNode = first_last_node.next
+                second_first_node: _doublyLinkedListNode | None = second_first_node.next
             self.len += extended_object.len
             if self.circular:
                 first_last_node.next = self._head
                 self._head.prev = first_last_node
         else:
             extended_linked_list: doublyLinkedList = doublyLinkedList(extended_object)
             self.extend(extended_linked_list)
 
     def to_singly(self: "doublyLinkedList") -> singlyLinkedList:
         return singlyLinkedList() + self
 
     def add(
         self: "doublyLinkedList",
-        data: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        data: object,
     ) -> None:
         """To add in an organized manner"""
         if not self._head:
-            self._head: doublyLinkedListNode = doublyLinkedListNode(data)
+            self._head: _doublyLinkedListNode = _doublyLinkedListNode(data)
             self.len += 1
-            self._tail: doublyLinkedListNode = self._head
+            self._tail: _doublyLinkedListNode = self._head
             if self.circular:
                 self._head.next = self._head
                 self._head.prev = self._head
         else:
-            head: doublyLinkedListNode = self._head
+            head: _doublyLinkedListNode = self._head
             for i in range(self.len):
                 if type(head.data) != type(data):
                     raise TypeError(
                         f"'<' not supported between instances of '{type(head.data).__name__}' and '{type(data).__name__}'"
                     )
                 else:
                     if not self.rev:
                         if data < head.data:
                             if i == 0 or i == self.len - 1:
                                 self.insert(i, data)
                                 break
                             else:
-                                new_node: doublyLinkedListNode = doublyLinkedListNode(
+                                new_node: _doublyLinkedListNode = _doublyLinkedListNode(
                                     data
                                 )
                                 new_node.next = head
                                 new_node.prev = head.prev
                                 head.prev.next = new_node
                                 head.prev = new_node
                                 self.len += 1
                                 break
                         else:
-                            head: doublyLinkedListNode | None = head.next
+                            head: _doublyLinkedListNode | None = head.next
                     else:
                         if data > head.data:
                             if i == 0 or i == self.len - 1:
                                 self.insert(i, data)
                                 break
                             else:
-                                new_node: doublyLinkedListNode = doublyLinkedListNode(
+                                new_node: _doublyLinkedListNode = _doublyLinkedListNode(
                                     data
                                 )
                                 new_node.next = head
                                 new_node.prev = head.prev
                                 head.prev.next = new_node
                                 head.prev = new_node
                                 self.len += 1
                                 break
                         else:
-                            head: doublyLinkedListNode | None = head.next
+                            head: _doublyLinkedListNode | None = head.next
             else:
                 self.insert(self.len, data)
 
     def to_dict(self: "doublyLinkedList", node: bool = False) -> dict:
-        head: doublyLinkedListNode | None = self._head
+        head: _doublyLinkedListNode | None = self._head
         new_dict: dict = {}
         for _ in range(self.len):
             try:
-                next_value: (
-                    object
-                    | int
-                    | float
-                    | complex
-                    | str
-                    | list
-                    | tuple
-                    | set
-                    | dict
-                    | None
-                    | bool
-                ) = head.next.data
+                next_value: object = head.next.data
             except AttributeError as e12:
                 next_value: None = None
             new_dict[head.data] = {
                 "prev value" if not node else "prev node value": (
                     (head.prev.data if head.prev is not None else None)
                     if not node
                     else head.prev.data if head.prev is not None else None
@@ -2339,64 +1937,40 @@
                             )
                         )
                     )
                     if not node
                     else head.next
                 ),
             }
-            head: doublyLinkedListNode | None = head.next
+            head: _doublyLinkedListNode | None = head.next
         return new_dict
 
     def reverse(self: "doublyLinkedList") -> None:
-        head: doublyLinkedListNode = self._head
-        tail: doublyLinkedListNode = self._tail
+        head: _doublyLinkedListNode = self._head
+        tail: _doublyLinkedListNode = self._tail
         for _ in range(self.len // 2):
             head.data, tail.data = tail.data, head.data
-            head: doublyLinkedListNode | None = head.next
-            tail: doublyLinkedListNode | None = tail.prev
+            head: _doublyLinkedListNode | None = head.next
+            tail: _doublyLinkedListNode | None = tail.prev
 
 
 class dll(doublyLinkedList):
     pass
 
 
 class orthogonalLinkedListNode:
     def __init__(
         self: "orthogonalLinkedListNode",
-        data: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        data: object,
     ) -> None:
         self.prev: None = None
         self.next: None = None
         self.up: None = None
         self.down: None = None
-        self.data: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ) = data
+        self.data: object = data
 
     def prev_node(self: "orthogonalLinkedListNode") -> "orthogonalLinkedListNode":
         return self.prev
 
     def next_node(self: "orthogonalLinkedListNode") -> "orthogonalLinkedListNode":
         return self.next
 
@@ -2404,15 +1978,15 @@
         return self.up
 
     def down_node(self: "orthogonalLinkedListNode") -> "orthogonalLinkedListNode":
         return self.down
 
     def get_data(
         self: "orthogonalLinkedListNode",
-    ) -> object | int | float | complex | str | list | tuple | set | dict | None | bool:
+    ) -> object:
         return self.data
 
 
 class orthogonalLinkedList:
     def __init__(
         self: "orthogonalLinkedList",
         data: list,
@@ -2442,27 +2016,15 @@
         for i in range(len(self._head[index])):
             values.append(self._head[index][i].data)
         return values
 
     def __setitem__(
         self: "orthogonalLinkedList",
         index: int,
-        value: (
-            object
-            | int
-            | float
-            | complex
-            | str
-            | list
-            | tuple
-            | set
-            | dict
-            | None
-            | bool
-        ),
+        value: object,
     ) -> None:
         if len(value) == len(self._head[index]):
             for i in range(len(self._head[index])):
                 self._head[index][i].data = value[i]
         else:
             raise TypeError("columns len not the same")
 
@@ -2580,24 +2142,24 @@
                 linked_list.append(["None"] * (len(self._head[0]) + 2))
                 linked_list[-1][0], linked_list[-1][-1] = "", ""
             return tabulate(linked_list, tablefmt="fancy_grid")
         else:
             counter: int = 0
             linked_list.append(
                 [
-                    _white("up"),
-                    _white("up ") + _green("@"),
-                    _white("previous"),
-                    _white("previous ") + _green("@"),
-                    _white("current"),
-                    _white("current ") + _green("@"),
-                    _white("down"),
-                    _white("down ") + _green("@"),
-                    _white("next"),
-                    _white("next ") + _green("@"),
+                    _white("Up"),
+                    _white("Up ") + _green("@"),
+                    _white("Previous"),
+                    _white("Previous ") + _green("@"),
+                    _white("Current"),
+                    _white("Current ") + _green("@"),
+                    _white("Down"),
+                    _white("Down ") + _green("@"),
+                    _white("Next"),
+                    _white("Next ") + _green("@"),
                 ]
             )
             for i in range(len(self._head)):
                 for j in range(len(self._head[i])):
                     try:
                         if not isinstance(self._head[i][j].prev.data, str):
                             prev_data: str = _blue(f"{self._head[i][j].prev.data}")
@@ -2742,13 +2304,13 @@
         return self._head
 
 
 class oll(orthogonalLinkedList):
     pass
 
 
-def _main() -> None:
-    print("linkedit")
+# def _main() -> None:
+#     print("linkedit")
 
 
-if __name__ == "__main__":
-    _main()
+# if __name__ == "__main__":
+#     _main()
```

### Comparing `linkedit-1.0.5/linkedit.egg-info/PKG-INFO` & `linkedit-1.0.7/linkedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedit
-Version: 1.0.5
+Version: 1.0.7
 Summary: Sophisticate Linked List
 Home-page: https://pypi.org/project/linkedit/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: linked list
 Classifier: Programming Language :: Python :: 3
@@ -70,15 +70,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│ current value   │ current value @ddress   │ next value   │ next value @ddress   │
+│ Current Value   │ Current Value @ddress   │ Next Value   │ Next Value @ddress   │
 ╞═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │ 6               │ 0x7febe8213950          │ 3            │ 0x7febe8213990       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 3               │ 0x7febe8213990          │ 8            │ 0x7febe82139d0       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 8               │ 0x7febe82139d0          │ 1            │ 0x7febe823c110       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -108,15 +108,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│ current value   │ current value @ddress   │ next value   │ next value @ddress   │
+│ Current Value   │ Current Value @ddress   │ Next Value   │ Next Value @ddress   │
 ╞═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │ 6               │ 140217964133136         │ 3            │ 140217964133264      │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 3               │ 140217964133264         │ 8            │ 140217964133200      │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 8               │ 140217964133200         │ 1            │ 140217964298704      │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -379,15 +379,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│   current value │ current value @ddress   │   next value │ next value @ddress   │
+│   Current Value │ Current Value @ddress   │   Next Value │ Next Value @ddress   │
 ╞═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │               6 │ 0x7fbe38bf3ad0          │            3 │ 0x7fbe38bf3b50       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │               3 │ 0x7fbe38bf3b50          │            8 │ 0x7fbe38bf3b10       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │               8 │ 0x7fbe38bf3b10          │            1 │ 0x7fbe38c07fd0       │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -415,15 +415,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│   current value │   current value @ddress │   next value │   next value @ddress │
+│   Current Value │   Current Value @ddress │   Next Value │   Next Value @ddress │
 ╞═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │               6 │         140374800546256 │            3 │      140374800546448 │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │               3 │         140374800546448 │            8 │      140374800546192 │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │               8 │         140374800546192 │            1 │      140374800629712 │
 ├─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -738,15 +738,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════════════════╤══════════════════════════╤═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│ previous value   │ previous value @ddress   │ current value   │ current value @ddress   │ next value   │ next value @ddress   │
+│ Previous Value   │ Previous Value @ddress   │ Current Value   │ Current Value @ddress   │ Next Value   │ Next Value @ddress   │
 ╞══════════════════╪══════════════════════════╪═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │                  │                          │ None (NULL)     │ 0x959cc0 (nil/0x0)      │              │                      │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ None (NULL)      │ 0x959cc0 (nil/0x0)       │ 6               │ 0x7effd8613950          │ 3            │ 0x7effd8613990       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 6                │ 0x7effd8613950           │ 3               │ 0x7effd8613990          │ 8            │ 0x7effd86139d0       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -778,15 +778,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════════════════╤══════════════════════════╤═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│ previous value   │ previous value @ddress   │ current value   │ current value @ddress   │ next value   │ next value @ddress   │
+│ Previous Value   │ Previous Value @ddress   │ Current Value   │ Current Value @ddress   │ Next Value   │ Next Value @ddress   │
 ╞══════════════════╪══════════════════════════╪═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │                  │                          │ None (NULL)     │ 9804992 (nil/0)         │              │                      │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ None (NULL)      │ 9804992 (nil/0)          │ 6               │ 140107643451856         │ 3            │ 140107643451984      │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │ 6                │ 140107643451856          │ 3               │ 140107643451984         │ 8            │ 140107643451920      │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -1054,15 +1054,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════════════════╤══════════════════════════╤═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│   previous value │ previous value @ddress   │   current value │ current value @ddress   │   next value │ next value @ddress   │
+│   Previous Value │ Previous Value @ddress   │   Current Value │ Current Value @ddress   │   Next Value │ Next Value @ddress   │
 ╞══════════════════╪══════════════════════════╪═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │                7 │ 0x7ff7a725be10           │               6 │ 0x7ff7a7413ad0          │            3 │ 0x7ff7a7413b50       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │                6 │ 0x7ff7a7413ad0           │               3 │ 0x7ff7a7413b50          │            8 │ 0x7ff7a7413b10       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │                3 │ 0x7ff7a7413b50           │               8 │ 0x7ff7a7413b10          │            1 │ 0x7ff7a7427fd0       │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -1090,15 +1090,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════════════════╤══════════════════════════╤═════════════════╤═════════════════════════╤══════════════╤══════════════════════╕
-│   previous value │   previous value @ddress │   current value │   current value @ddress │   next value │   next value @ddress │
+│   Previous Value │   Previous Value @ddress │   Current Value │   Current Value @ddress │   Next Value │   Next Value @ddress │
 ╞══════════════════╪══════════════════════════╪═════════════════╪═════════════════════════╪══════════════╪══════════════════════╡
 │                7 │          140070320684368 │               6 │         140070322534992 │            3 │      140070322535184 │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │                6 │          140070322534992 │               3 │         140070322535184 │            8 │      140070322534928 │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
 │                3 │          140070322535184 │               8 │         140070322534928 │            1 │      140070322700432 │
 ├──────────────────┼──────────────────────────┼─────────────────┼─────────────────────────┼──────────────┼──────────────────────┤
@@ -1441,15 +1441,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════╤════════════════╤════════════╤════════════════╤═══════════╤════════════════╤════════╤════════════════╤════════╤════════════════╕
-│ up   │ up @           │ previous   │ previous @     │   current │ current @      │ down   │ down @         │ next   │ next @         │
+│ Up   │ Up @           │ Previous   │ Previous @     │   Current │ Current @      │ Down   │ Down @         │ Next   │ Next @         │
 ╞══════╪════════════════╪════════════╪════════════════╪═══════════╪════════════════╪════════╪════════════════╪════════╪════════════════╡
 │ None │ 0x959cc0       │ None       │ 0x959cc0       │         6 │ 0x7f20d0213250 │ 1      │ 0x7f20d0213cd0 │ 3      │ 0x7f20d0213c50 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
 │ None │ 0x959cc0       │ 6          │ 0x7f20d0213250 │         3 │ 0x7f20d0213c50 │ 9      │ 0x7f20d023c090 │ 8      │ 0x7f20d0213c90 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
 │ None │ 0x959cc0       │ 3          │ 0x7f20d0213c50 │         8 │ 0x7f20d0213c90 │ 5      │ 0x7f20d005bcd0 │ None   │ 0x959cc0       │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
@@ -1507,15 +1507,15 @@
 
 
 ### Output
 
 
 ```bash
 ╒══════╤════════════════╤════════════╤════════════════╤═══════════╤════════════════╤════════╤════════════════╤════════╤════════════════╕
-│   up │ up @           │   previous │ previous @     │   current │ current @      │   down │ down @         │   next │ next @         │
+│   Up │ Up @           │   Previous │ Previous @     │   Current │ Current @      │   Down │ Down @         │   Next │ Next @         │
 ╞══════╪════════════════╪════════════╪════════════════╪═══════════╪════════════════╪════════╪════════════════╪════════╪════════════════╡
 │    7 │ 0x7f01e6153ad0 │          8 │ 0x7f01e6317cd0 │         6 │ 0x7f01e6316250 │      1 │ 0x7f01e6317d10 │      3 │ 0x7f01e6317c90 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
 │    2 │ 0x7f01e6153dd0 │          6 │ 0x7f01e6316250 │         3 │ 0x7f01e6317c90 │      9 │ 0x7f01e632bfd0 │      8 │ 0x7f01e6317cd0 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
 │    4 │ 0x7f01e6153d10 │          3 │ 0x7f01e6317c90 │         8 │ 0x7f01e6317cd0 │      5 │ 0x7f01e6153c90 │      6 │ 0x7f01e6316250 │
 ├──────┼────────────────┼────────────┼────────────────┼───────────┼────────────────┼────────┼────────────────┼────────┼────────────────┤
```

### Comparing `linkedit-1.0.5/setup.py` & `linkedit-1.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="linkedit",
-    version="1.0.5",
+    version="1.0.7",
     author="khiat Mohammed Abderrezzak",
     author_email="khiat.abderrezzak@gmail.com",
     license="MIT",
     description="Sophisticate Linked List",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/linkedit/",
```

