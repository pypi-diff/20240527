# Comparing `tmp/cdt_path-2.1.1.tar.gz` & `tmp/cdt_path-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdt_path-2.1.1.tar", last modified: Thu May 23 14:57:38 2024, max compression
+gzip compressed data, was "cdt_path-2.1.4.tar", last modified: Mon May 27 13:40:55 2024, max compression
```

## Comparing `cdt_path-2.1.1.tar` & `cdt_path-2.1.4.tar`

### file list

```diff
@@ -1,56 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.953777 cdt_path-2.1.1/
--rw-rw-rw-   0        0        0      795 2024-05-23 14:57:38.953777 cdt_path-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      100 2024-05-23 07:09:32.000000 cdt_path-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.922524 cdt_path-2.1.1/cdt_path/
--rw-rw-rw-   0        0        0      546 2024-05-23 03:29:44.000000 cdt_path-2.1.1/cdt_path/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.922524 cdt_path-2.1.1/cdt_path/circumcircle/
--rw-rw-rw-   0        0        0        0 2024-05-14 14:48:14.000000 cdt_path-2.1.1/cdt_path/circumcircle/__init__.py
--rw-rw-rw-   0        0        0      648 2024-05-15 06:54:49.000000 cdt_path-2.1.1/cdt_path/circumcircle/calculate.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.922524 cdt_path-2.1.1/cdt_path/constrained_delaunay/
--rw-rw-rw-   0        0        0        0 2024-05-06 01:15:42.000000 cdt_path-2.1.1/cdt_path/constrained_delaunay/__init__.py
--rw-rw-rw-   0        0        0      117 2024-05-09 06:46:10.000000 cdt_path-2.1.1/cdt_path/constrained_delaunay/cdt_edge_additions.py
--rw-rw-rw-   0        0        0      352 2024-05-06 01:33:01.000000 cdt_path-2.1.1/cdt_path/constrained_delaunay/definition.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.938151 cdt_path-2.1.1/cdt_path/convex_hull/
--rw-rw-rw-   0        0        0      181 2024-04-13 02:40:26.000000 cdt_path-2.1.1/cdt_path/convex_hull/__init__.py
--rw-rw-rw-   0        0        0      202 2024-04-11 22:13:16.000000 cdt_path-2.1.1/cdt_path/convex_hull/display.py
--rw-rw-rw-   0        0        0     4543 2024-04-11 22:13:16.000000 cdt_path-2.1.1/cdt_path/convex_hull/divide_and_conquer.py
--rw-rw-rw-   0        0        0     1321 2024-04-11 22:13:16.000000 cdt_path-2.1.1/cdt_path/convex_hull/extreme_edge.py
--rw-rw-rw-   0        0        0     1225 2024-04-11 22:13:16.000000 cdt_path-2.1.1/cdt_path/convex_hull/gift_wrap.py
--rw-rw-rw-   0        0        0     4325 2024-05-06 15:05:43.000000 cdt_path-2.1.1/cdt_path/convex_hull/incremental.py
--rw-rw-rw-   0        0        0     1238 2024-04-11 22:13:16.000000 cdt_path-2.1.1/cdt_path/convex_hull/quick_hull.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.938151 cdt_path-2.1.1/cdt_path/delaunay/
--rw-rw-rw-   0        0        0       78 2024-04-18 11:20:20.000000 cdt_path-2.1.1/cdt_path/delaunay/__init__.py
--rw-rw-rw-   0        0        0     1219 2024-05-06 01:27:54.000000 cdt_path-2.1.1/cdt_path/delaunay/definition.py
--rw-rw-rw-   0        0        0     1080 2024-04-14 14:36:46.000000 cdt_path-2.1.1/cdt_path/delaunay/definition_Old_2.py
--rw-rw-rw-   0        0        0       75 2024-04-18 11:17:22.000000 cdt_path-2.1.1/cdt_path/delaunay/hhh.py
--rw-rw-rw-   0        0        0     3577 2024-04-15 03:58:05.000000 cdt_path-2.1.1/cdt_path/delaunay/incremental.py
--rw-rw-rw-   0        0        0     8444 2024-04-14 14:34:03.000000 cdt_path-2.1.1/cdt_path/delaunay/incremental_Old.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.938151 cdt_path-2.1.1/cdt_path/file/
--rw-rw-rw-   0        0        0       19 2024-05-22 13:26:45.000000 cdt_path-2.1.1/cdt_path/file/__init__.py
--rw-rw-rw-   0        0        0      116 2024-05-22 13:28:55.000000 cdt_path-2.1.1/cdt_path/file/load.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.938151 cdt_path-2.1.1/cdt_path/interact/
--rw-rw-rw-   0        0        0       66 2024-05-23 14:55:55.000000 cdt_path-2.1.1/cdt_path/interact/__init__.py
--rw-rw-rw-   0        0        0     3628 2024-05-23 12:04:51.000000 cdt_path-2.1.1/cdt_path/interact/base.py
--rw-rw-rw-   0        0        0      257 2024-05-23 03:30:04.000000 cdt_path-2.1.1/cdt_path/interact/border.py
--rw-rw-rw-   0        0        0     1285 2024-05-23 14:54:44.000000 cdt_path-2.1.1/cdt_path/interact/draw.py
--rw-rw-rw-   0        0        0     1523 2024-05-16 08:58:29.000000 cdt_path-2.1.1/cdt_path/interact/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.953777 cdt_path-2.1.1/cdt_path/manipulate/
--rw-rw-rw-   0        0        0       22 2024-05-21 13:38:19.000000 cdt_path-2.1.1/cdt_path/manipulate/__init__.py
--rw-rw-rw-   0        0        0     1000 2024-05-21 13:44:41.000000 cdt_path-2.1.1/cdt_path/manipulate/combine.py
--rw-rw-rw-   0        0        0       14 2024-05-12 06:05:36.000000 cdt_path-2.1.1/cdt_path/manipulate/save.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.953777 cdt_path-2.1.1/cdt_path/pathplan/
--rw-rw-rw-   0        0        0     3452 2024-05-23 11:51:41.000000 cdt_path-2.1.1/cdt_path/pathplan/A_star.py
--rw-rw-rw-   0        0        0     1373 2024-05-05 11:19:13.000000 cdt_path-2.1.1/cdt_path/pathplan/A_star_O.py
--rw-rw-rw-   0        0        0       68 2024-05-22 13:51:17.000000 cdt_path-2.1.1/cdt_path/pathplan/__init__.py
--rw-rw-rw-   0        0        0     1300 2024-05-22 13:01:38.000000 cdt_path-2.1.1/cdt_path/pathplan/funnel - 副本.py
--rw-rw-rw-   0        0        0     1300 2024-05-22 13:01:38.000000 cdt_path-2.1.1/cdt_path/pathplan/funnel.py
--rw-rw-rw-   0        0        0     1293 2024-05-22 13:51:02.000000 cdt_path-2.1.1/cdt_path/pathplan/utils.py
--rw-rw-rw-   0        0        0     2328 2024-04-11 22:13:16.000000 cdt_path-2.1.1/cdt_path/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:57:38.922524 cdt_path-2.1.1/cdt_path.egg-info/
--rw-rw-rw-   0        0        0      795 2024-05-23 14:57:38.000000 cdt_path-2.1.1/cdt_path.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1324 2024-05-23 14:57:38.000000 cdt_path-2.1.1/cdt_path.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 14:57:38.000000 cdt_path-2.1.1/cdt_path.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-23 14:57:38.000000 cdt_path-2.1.1/cdt_path.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 14:57:38.000000 cdt_path-2.1.1/cdt_path.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 14:57:38.953777 cdt_path-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1073 2024-05-23 14:56:45.000000 cdt_path-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:40:55.787019 cdt_path-2.1.4/
+-rw-rw-rw-   0        0        0      435 2024-05-27 13:40:55.787019 cdt_path-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      100 2024-05-23 07:09:32.000000 cdt_path-2.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 13:40:55.757634 cdt_path-2.1.4/cdt_path/
+-rw-rw-rw-   0        0        0      596 2024-05-27 06:18:44.000000 cdt_path-2.1.4/cdt_path/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:40:55.761636 cdt_path-2.1.4/cdt_path/circumcircle/
+-rw-rw-rw-   0        0        0        0 2024-05-14 14:48:14.000000 cdt_path-2.1.4/cdt_path/circumcircle/__init__.py
+-rw-rw-rw-   0        0        0      648 2024-05-15 06:54:49.000000 cdt_path-2.1.4/cdt_path/circumcircle/calculate.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:40:55.765636 cdt_path-2.1.4/cdt_path/constrained_delaunay/
+-rw-rw-rw-   0        0        0        0 2024-05-06 01:15:42.000000 cdt_path-2.1.4/cdt_path/constrained_delaunay/__init__.py
+-rw-rw-rw-   0        0        0      117 2024-05-09 06:46:10.000000 cdt_path-2.1.4/cdt_path/constrained_delaunay/cdt_edge_additions.py
+-rw-rw-rw-   0        0        0      352 2024-05-06 01:33:01.000000 cdt_path-2.1.4/cdt_path/constrained_delaunay/definition.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:40:55.765636 cdt_path-2.1.4/cdt_path/convex_hull/
+-rw-rw-rw-   0        0        0      181 2024-04-13 02:40:26.000000 cdt_path-2.1.4/cdt_path/convex_hull/__init__.py
+-rw-rw-rw-   0        0        0      202 2024-04-11 22:13:16.000000 cdt_path-2.1.4/cdt_path/convex_hull/display.py
+-rw-rw-rw-   0        0        0     4543 2024-04-11 22:13:16.000000 cdt_path-2.1.4/cdt_path/convex_hull/divide_and_conquer.py
+-rw-rw-rw-   0        0        0     1321 2024-04-11 22:13:16.000000 cdt_path-2.1.4/cdt_path/convex_hull/extreme_edge.py
+-rw-rw-rw-   0        0        0     1225 2024-04-11 22:13:16.000000 cdt_path-2.1.4/cdt_path/convex_hull/gift_wrap.py
+-rw-rw-rw-   0        0        0     3823 2024-05-27 13:38:41.000000 cdt_path-2.1.4/cdt_path/convex_hull/incremental.py
+-rw-rw-rw-   0        0        0     1238 2024-04-11 22:13:16.000000 cdt_path-2.1.4/cdt_path/convex_hull/quick_hull.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:40:55.773666 cdt_path-2.1.4/cdt_path/delaunay/
+-rw-rw-rw-   0        0        0       78 2024-04-18 11:20:20.000000 cdt_path-2.1.4/cdt_path/delaunay/__init__.py
+-rw-rw-rw-   0        0        0     1219 2024-05-06 01:27:54.000000 cdt_path-2.1.4/cdt_path/delaunay/definition.py
+-rw-rw-rw-   0        0        0     1080 2024-04-14 14:36:46.000000 cdt_path-2.1.4/cdt_path/delaunay/definition_Old_2.py
+-rw-rw-rw-   0        0        0       75 2024-04-18 11:17:22.000000 cdt_path-2.1.4/cdt_path/delaunay/hhh.py
+-rw-rw-rw-   0        0        0     3577 2024-04-15 03:58:05.000000 cdt_path-2.1.4/cdt_path/delaunay/incremental.py
+-rw-rw-rw-   0        0        0     8444 2024-04-14 14:34:03.000000 cdt_path-2.1.4/cdt_path/delaunay/incremental_Old.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:40:55.776808 cdt_path-2.1.4/cdt_path/demo/
+-rw-rw-rw-   0        0        0      348 2024-05-23 03:31:08.000000 cdt_path-2.1.4/cdt_path/demo/Interact_part.py
+-rw-rw-rw-   0        0        0       20 2024-05-27 13:39:44.000000 cdt_path-2.1.4/cdt_path/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:40:55.778671 cdt_path-2.1.4/cdt_path/file/
+-rw-rw-rw-   0        0        0       19 2024-05-22 13:26:45.000000 cdt_path-2.1.4/cdt_path/file/__init__.py
+-rw-rw-rw-   0        0        0      116 2024-05-22 13:28:55.000000 cdt_path-2.1.4/cdt_path/file/load.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:40:55.780897 cdt_path-2.1.4/cdt_path/interact/
+-rw-rw-rw-   0        0        0       66 2024-05-23 14:55:55.000000 cdt_path-2.1.4/cdt_path/interact/__init__.py
+-rw-rw-rw-   0        0        0     3628 2024-05-25 13:59:10.000000 cdt_path-2.1.4/cdt_path/interact/base.py
+-rw-rw-rw-   0        0        0      257 2024-05-23 03:30:04.000000 cdt_path-2.1.4/cdt_path/interact/border.py
+-rw-rw-rw-   0        0        0     1447 2024-05-24 08:52:59.000000 cdt_path-2.1.4/cdt_path/interact/draw.py
+-rw-rw-rw-   0        0        0     1523 2024-05-16 08:58:29.000000 cdt_path-2.1.4/cdt_path/interact/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:40:55.782909 cdt_path-2.1.4/cdt_path/manipulate/
+-rw-rw-rw-   0        0        0       22 2024-05-21 13:38:19.000000 cdt_path-2.1.4/cdt_path/manipulate/__init__.py
+-rw-rw-rw-   0        0        0     1000 2024-05-21 13:44:41.000000 cdt_path-2.1.4/cdt_path/manipulate/combine.py
+-rw-rw-rw-   0        0        0       14 2024-05-12 06:05:36.000000 cdt_path-2.1.4/cdt_path/manipulate/save.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:40:55.786553 cdt_path-2.1.4/cdt_path/pathplan/
+-rw-rw-rw-   0        0        0     3452 2024-05-23 11:51:41.000000 cdt_path-2.1.4/cdt_path/pathplan/A_star.py
+-rw-rw-rw-   0        0        0     1373 2024-05-05 11:19:13.000000 cdt_path-2.1.4/cdt_path/pathplan/A_star_O.py
+-rw-rw-rw-   0        0        0       68 2024-05-22 13:51:17.000000 cdt_path-2.1.4/cdt_path/pathplan/__init__.py
+-rw-rw-rw-   0        0        0     1300 2024-05-22 13:01:38.000000 cdt_path-2.1.4/cdt_path/pathplan/funnel - 副本.py
+-rw-rw-rw-   0        0        0     2707 2024-05-25 12:51:42.000000 cdt_path-2.1.4/cdt_path/pathplan/funnel.py
+-rw-rw-rw-   0        0        0     1512 2024-05-25 15:57:56.000000 cdt_path-2.1.4/cdt_path/pathplan/utils.py
+-rw-rw-rw-   0        0        0     2328 2024-04-11 22:13:16.000000 cdt_path-2.1.4/cdt_path/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:40:55.761636 cdt_path-2.1.4/cdt_path.egg-info/
+-rw-rw-rw-   0        0        0      435 2024-05-27 13:40:55.000000 cdt_path-2.1.4/cdt_path.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1381 2024-05-27 13:40:55.000000 cdt_path-2.1.4/cdt_path.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 13:40:55.000000 cdt_path-2.1.4/cdt_path.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-27 13:40:55.000000 cdt_path-2.1.4/cdt_path.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 13:40:55.000000 cdt_path-2.1.4/cdt_path.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 13:40:55.787019 cdt_path-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      727 2024-05-24 08:54:13.000000 cdt_path-2.1.4/setup.py
```

### Comparing `cdt_path-2.1.1/cdt_path/__init__.py` & `cdt_path-2.1.4/cdt_path/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from . import manipulate
 from . import convex_hull
 from .file import *
 from triangle import triangulate as _triangulate
 from .interact.base import Interact
 from .interact import border
 from matplotlib.tri import Triangulation as _Triangulation
+from .circumcircle.calculate import circumcircle
 
 def triangulate(tri, opts = 'p'):
 	return _triangulate(tri, opts)
 	
 def Triangulation(tri, opts = 'p'):
 	cc = _triangulate(tri, opts)
 	return _Triangulation(cc['vertices'][:,0],cc['vertices'][:,1],cc['triangles'])
```

### Comparing `cdt_path-2.1.1/cdt_path/circumcircle/calculate.py` & `cdt_path-2.1.4/cdt_path/circumcircle/calculate.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path/convex_hull/divide_and_conquer.py` & `cdt_path-2.1.4/cdt_path/convex_hull/divide_and_conquer.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path/convex_hull/extreme_edge.py` & `cdt_path-2.1.4/cdt_path/convex_hull/extreme_edge.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path/convex_hull/gift_wrap.py` & `cdt_path-2.1.4/cdt_path/convex_hull/gift_wrap.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path/convex_hull/incremental.py` & `cdt_path-2.1.4/cdt_path/convex_hull/incremental.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from ..utils import ToLeft,Simplify_With_X_i
 
-def Incremental(P):
+def incremental(P):
 	l=len(P)
 	if l==0:
 		return []
 		
 	i1=1
 	while i1<l:
 		if np.array_equal(P[0],P[i1]):
@@ -133,18 +133,18 @@
 	if i_r<i_l:
 		L=[p]+L[i_r:i_l+1]
 	else:
 		L=L[0:i_l+1]+[p]+L[i_r:]
 	return L
 	
 	
-def Incremental_Sort(P):
-	return Incremental_Sorted_Simplified(Simplify_With_X_i(P[P[:,0].argsort()]))
+def incremental_sort(P):
+	return incremental_sorted_simplified(Simplify_With_X_i(P[P[:,0].argsort()]))
 	
-def Incremental_Sorted_Simplified(P):
+def incremental_sorted_simplified(P):
 	l=len(P)
 	if l<3:
 		return P
 		
 	i1=1
 	i=2
 	while i<l:
@@ -167,15 +167,15 @@
 	i+=1
 	while i<l:
 		L,i_xmax=Sorted_Increment_w(L,P[i],i_xmax)
 		i+=1
 		
 	return L
 	
-def Incremental_Sorted_Simplified_N(P):
+def incremental_sorted_simplified_N(P):
 	l=len(P)
 	if l<3:
 		return P
 		
 	i1=1
 	i=2
 	while i<l:
@@ -193,47 +193,20 @@
 			i_xmax=2
 			break
 	else:
 		return [P[0],P[i1]]
 		
 	i+=1
 	while i<l:
-		L,i_xmax=Sorted_Increment_w(L,P[i],i_xmax)
+		L,i_xmax=sorted_Increment_w(L,P[i],i_xmax)
 		i+=1
 		
 	return L
 	
-# def Sorted_Increment(A,p,a1=None):
-# 	if a1==None:
-# 		a1=max(enumerate(A), key=lambda x: x[1][0])[0]
-# 	a2=a1
-# 	la=len(A)
-# 	if a1+1==la: a1=-1
-	
-# 	if ToLeft(p,A[a1],A[a1+1])>0:
-# 		a2-=1
-# 	else:
-# 		if a1+2==la:
-# 			a1=-1
-# 		else:
-# 			a1+=1
-# 		while ToLeft(p,A[a1],A[a1+1])<=0:
-# 			if a1+2==la:
-# 				a1=-1
-# 			else:
-# 				a1+=1
-		
-# 	while ToLeft(p,A[a2-1],A[a2])<=0:
-# 		a2-=1
-			
-# 	if a1==0:
-# 		return A[:a2+1]+[p],a2+1
-# 	return A[:a2+1]+[p]+A[a1:],a2+1
-	
-def Sorted_Increment(A,p,a1=None):
+def sorted_increment(A,p,a1=None):
 	if a1==None:
 		a1=max(enumerate(A), key=lambda x: x[1][0])[0]
 	if ToLeft(p,A[a1-1],A[a1])>0:
 		a2=a1-len(A)+1
 	else:
 		a2=a1-len(A)
 		while ToLeft(p,A[a1-1],A[a1])<=0:
@@ -242,15 +215,15 @@
 	while ToLeft(p,A[a2],A[a2+1])<=0:
 		a2+=1
 			
 	if a2==0:
 		return A[:a1+1]+[p],a1+1
 	return A[:a1+1]+[p]+A[a2:],a1+1
 	
-def Sorted_Increment_w(A,p,a1):
+def sorted_increment_w(A,p,a1):
 	if ToLeft(p,A[a1-1],A[a1])>0:
 		a2=a1-len(A)+1
 	else:
 		a2=a1-len(A)
 		while ToLeft(p,A[a1-1],A[a1])<=0:
 			a1-=1
```

### Comparing `cdt_path-2.1.1/cdt_path/convex_hull/quick_hull.py` & `cdt_path-2.1.4/cdt_path/convex_hull/quick_hull.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path/delaunay/definition.py` & `cdt_path-2.1.4/cdt_path/delaunay/definition.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path/delaunay/definition_Old_2.py` & `cdt_path-2.1.4/cdt_path/delaunay/definition_Old_2.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path/delaunay/incremental.py` & `cdt_path-2.1.4/cdt_path/delaunay/incremental.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path/delaunay/incremental_Old.py` & `cdt_path-2.1.4/cdt_path/delaunay/incremental_Old.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path/interact/base.py` & `cdt_path-2.1.4/cdt_path/interact/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,18 +86,18 @@
 		Py = self.triang.y[Ll]
 		Pl = np.column_stack((Px, Py))
 		points = np.concatenate(([start_point], Pr, Pl))
 		self.polygon2 = Polygon(points, closed = True, facecolor='#80FF00',alpha = 0.6)
 		self.ax.add_patch(self.polygon2)
 		
 		Pl = np.concatenate((Pl[::-1], [end_point]))
-		Ln = funnel_slow(start_point, Pl, Pr, Li)
+		Ln = funnel(start_point, Pl, Pr, Li)
 		Ln = [start_point] + Ln + [end_point]
 		Ln_np = np.array(Ln)
-		plt.plot(Ln_np[:,0],Ln_np[:,1])
+		plt.plot(Ln_np[:,0],Ln_np[:,1],lw=3)
 		
 	def on_click(self, event):
 		if event.inaxes is None or self.trifinder(event.xdata, event.ydata) == -1:
 			return
 		if event.button is MouseButton.LEFT:
 			if self._click_state==0:
 				self._start_point=(event.xdata, event.ydata)
```

### Comparing `cdt_path-2.1.1/cdt_path/interact/draw.py` & `cdt_path-2.1.4/cdt_path/interact/draw.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib.patches import Polygon
 from matplotlib.backend_bases import MouseButton
 import json
 class Draw:
-	def __init__(self, ax, save='data'):
+	def __init__(self, ax, save='data', r=1):
 		self.ax = ax
+		# self.r = r
 		self.points = []
 		self.segments = []
 		self.l=0
 		
 		plt.connect('button_press_event', self.on_click)
 		plt.connect('key_press_event', self.on_press)
 		ax.axes.set_aspect('equal')
-		ax.axis("off")
 		plt.show()
 		
-		data={"vertices":points, "segments":segments}
+		for i in range(self.l,len(self.points)-1):
+			self.segments.append((i,i+1))
+		self.segments.append((len(self.points)-1,self.l))
+		data={"vertices":self.points, "segments":self.segments}
 	
 		if save[-5:]!=".json":
 			save+='.json'
 			
 		with open(save,'w',encoding='utf-8') as f:
 			json.dump(data, f, ensure_ascii=False, indent=4)
 			
-		
-	
-	def onclick(event):  
+	def on_click(self, event):  
 		if event.inaxes:
-			rounded_x = round(event.xdata, 1)  
-			rounded_y = round(event.ydata, 1)  
+			rounded_x = round(event.xdata, r)  
+			rounded_y = round(event.ydata, r)  
 			  
 			self.points.append((rounded_x, rounded_y))  
 			print(f"Added point: ({rounded_x}, {rounded_y})")  
 			  
 			plt.scatter(rounded_x, rounded_y, color='red')  # 可视化新添加的点  
 			plt.draw()  # 更新图形
 	  
-	def on_press(event):
+	def on_press(self, event):
 		print('press', event.key)
 		if event.key == 'x':
 			for i in range(self.l,len(self.points)-1):
 				self.segments.append((i,i+1))
-			self.segments.append((len(self.points)-1,0))
-			self.l=len(points)
+			self.segments.append((len(self.points)-1,self.l))
+			self.l=len(self.points)
```

### Comparing `cdt_path-2.1.1/cdt_path/interact/utils.py` & `cdt_path-2.1.4/cdt_path/interact/utils.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path/manipulate/combine.py` & `cdt_path-2.1.4/cdt_path/manipulate/combine.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path/pathplan/A_star.py` & `cdt_path-2.1.4/cdt_path/pathplan/A_star.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path/pathplan/A_star_O.py` & `cdt_path-2.1.4/cdt_path/pathplan/A_star_O.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path/pathplan/funnel - 副本.py` & `cdt_path-2.1.4/cdt_path/pathplan/funnel - 副本.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path/utils.py` & `cdt_path-2.1.4/cdt_path/utils.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.1/cdt_path.egg-info/SOURCES.txt` & `cdt_path-2.1.4/cdt_path.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 cdt_path/convex_hull/quick_hull.py
 cdt_path/delaunay/__init__.py
 cdt_path/delaunay/definition.py
 cdt_path/delaunay/definition_Old_2.py
 cdt_path/delaunay/hhh.py
 cdt_path/delaunay/incremental.py
 cdt_path/delaunay/incremental_Old.py
+cdt_path/demo/Interact_part.py
+cdt_path/demo/__init__.py
 cdt_path/file/__init__.py
 cdt_path/file/load.py
 cdt_path/interact/__init__.py
 cdt_path/interact/base.py
 cdt_path/interact/border.py
 cdt_path/interact/draw.py
 cdt_path/interact/utils.py
```

