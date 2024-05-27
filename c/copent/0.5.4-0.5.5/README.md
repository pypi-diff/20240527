# Comparing `tmp/copent-0.5.4.tar.gz` & `tmp/copent-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copent-0.5.4.tar", last modified: Mon May 27 21:01:20 2024, max compression
+gzip compressed data, was "copent-0.5.5.tar", last modified: Mon May 27 21:45:03 2024, max compression
```

## Comparing `copent-0.5.4.tar` & `copent-0.5.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 21:01:20.225587 copent-0.5.4/
--rw-rw-r--   0 majian    (1000) majian    (1000)    35149 2022-09-11 06:39:52.000000 copent-0.5.4/LICENSE
--rw-rw-r--   0 majian    (1000) majian    (1000)     6220 2024-05-27 21:01:20.225587 copent-0.5.4/PKG-INFO
--rw-rw-r--   0 majian    (1000) majian    (1000)     5889 2024-03-14 23:57:08.000000 copent-0.5.4/README.md
-drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 21:01:20.225587 copent-0.5.4/copent/
--rw-rw-r--   0 majian    (1000) majian    (1000)       97 2024-02-12 06:43:57.000000 copent-0.5.4/copent/__init__.py
--rw-rw-r--   0 majian    (1000) majian    (1000)     5230 2024-05-27 20:58:51.000000 copent-0.5.4/copent/copent.py
-drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 21:01:20.225587 copent-0.5.4/copent.egg-info/
--rw-rw-r--   0 majian    (1000) majian    (1000)     6220 2024-05-27 21:01:20.000000 copent-0.5.4/copent.egg-info/PKG-INFO
--rw-rw-r--   0 majian    (1000) majian    (1000)      211 2024-05-27 21:01:20.000000 copent-0.5.4/copent.egg-info/SOURCES.txt
--rw-rw-r--   0 majian    (1000) majian    (1000)        1 2024-05-27 21:01:20.000000 copent-0.5.4/copent.egg-info/dependency_links.txt
--rw-rw-r--   0 majian    (1000) majian    (1000)       12 2024-05-27 21:01:20.000000 copent-0.5.4/copent.egg-info/requires.txt
--rw-rw-r--   0 majian    (1000) majian    (1000)        7 2024-05-27 21:01:20.000000 copent-0.5.4/copent.egg-info/top_level.txt
--rw-rw-r--   0 majian    (1000) majian    (1000)       38 2024-05-27 21:01:20.225587 copent-0.5.4/setup.cfg
--rw-rw-r--   0 majian    (1000) majian    (1000)      555 2024-05-27 21:01:04.000000 copent-0.5.4/setup.py
+drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 21:45:03.103928 copent-0.5.5/
+-rw-rw-r--   0 majian    (1000) majian    (1000)    35149 2022-09-11 06:39:52.000000 copent-0.5.5/LICENSE
+-rw-rw-r--   0 majian    (1000) majian    (1000)     6220 2024-05-27 21:45:03.103928 copent-0.5.5/PKG-INFO
+-rw-rw-r--   0 majian    (1000) majian    (1000)     5889 2024-03-14 23:57:08.000000 copent-0.5.5/README.md
+drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 21:45:03.103928 copent-0.5.5/copent/
+-rw-rw-r--   0 majian    (1000) majian    (1000)       97 2024-02-12 06:43:57.000000 copent-0.5.5/copent/__init__.py
+-rw-rw-r--   0 majian    (1000) majian    (1000)     5340 2024-05-27 21:44:55.000000 copent-0.5.5/copent/copent.py
+drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 21:45:03.103928 copent-0.5.5/copent.egg-info/
+-rw-rw-r--   0 majian    (1000) majian    (1000)     6220 2024-05-27 21:45:03.000000 copent-0.5.5/copent.egg-info/PKG-INFO
+-rw-rw-r--   0 majian    (1000) majian    (1000)      211 2024-05-27 21:45:03.000000 copent-0.5.5/copent.egg-info/SOURCES.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)        1 2024-05-27 21:45:03.000000 copent-0.5.5/copent.egg-info/dependency_links.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)       12 2024-05-27 21:45:03.000000 copent-0.5.5/copent.egg-info/requires.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)        7 2024-05-27 21:45:03.000000 copent-0.5.5/copent.egg-info/top_level.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)       38 2024-05-27 21:45:03.103928 copent-0.5.5/setup.cfg
+-rw-rw-r--   0 majian    (1000) majian    (1000)      555 2024-05-27 21:43:14.000000 copent-0.5.5/setup.py
```

### Comparing `copent-0.5.4/LICENSE` & `copent-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `copent-0.5.4/PKG-INFO` & `copent-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copent
-Version: 0.5.4
+Version: 0.5.5
 Summary: Estimating Copula Entropy and Transfer Entropy
 Home-page: https://github.com/majianthu/pycopent
 Author: MA Jian
 Author-email: majian03@gmail.com
 License: GPL License
 Platform: UNKNOWN
 Requires-Python: >=2.7
```

### Comparing `copent-0.5.4/README.md` & `copent-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `copent-0.5.4/copent/copent.py` & `copent-0.5.5/copent/copent.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,53 +123,55 @@
 	for i in range(0,n):
 		y1 = vstack((ones([N0,1]),ones([N1,1])*2)) + uniform(0, 0.0000001,[N0+N1,1])
 		y0 = ones([N0+N1,1]) + uniform(0,0.0000001,[N0+N1,1])
 		stat1 = stat1 + copent(hstack((x,y1)),k,dtype) - copent(hstack((x,y0)),k,dtype)
 	return stat1/n
 
 ##### single change point detection [6]
-def init_x_n(X,N):
-	global x,n
+def init(X,N,K,DTYPE):
+	global x,n,k,dtype
 	x = X
 	n = N
+	k = K
+	dtype = DTYPE
 
 def tsti(i):
 	s0 = x[0:(i+1),:]
 	s1 = x[(i+2):,:]
-	return tst(s0,s1,n)
+	return tst(s0,s1,n,k,dtype)
 	
-def cpd(x, thd = 0.13, n = 30):
+def cpd(x, thd = 0.13, n = 30, k = 3, dtype = 'chebychev'):
 	x = mat(x)
 	len1 = x.shape[0]
 	if len1 == 1:
 		len1 = x.shape[1]
 		x = x.T
 	pos = -1
 	maxstat = 0
-	pool = Pool(initializer = init_x_n, initargs=(x,n))
-	stat1 = [0] + pool.map(tsti,range(len1-1))
+	pool = Pool(initializer = init, initargs=(x,n,k,dtype))
+	stat1 = [0] + pool.map(tsti,range(len1-2))
 	if(max(stat1) > thd):
 		maxstat = max(stat1)
 		pos = where(stat1 == maxstat)[0][0]+1
 	return pos, maxstat, stat1
 
 ##### multiple change point detection [6]
-def mcpd(x, maxp = 5, thd = 0.13, minseglen = 10, n = 30):
+def mcpd(x, maxp = 5, thd = 0.13, minseglen = 10, n = 30, k = 3, dtype = 'chebychev'):
 	x = mat(x)
 	len1 = x.shape[0]
 	if len1 == 1:
 		len1 = x.shape[1]
 		x = x.T
 	maxstat = []
 	pos = []
 	bisegs = mat([0,len1-1])
 	for i in range(0,maxp):
 		if i >= bisegs.shape[0]:
 			break
-		rpos, rmaxstat, _ = cpd(x[bisegs[i,0]:bisegs[i,1],:],thd,n)
+		rpos, rmaxstat, _ = cpd(x[bisegs[i,0]:bisegs[i,1],:],thd,n,k,dtype)
 		if rpos > -1 :
 			rpos = rpos + bisegs[i,0]
 			maxstat.append(rmaxstat)
 			pos.append(rpos)
 			if (rpos - bisegs[i,0]) > minseglen :
 				bisegs = vstack((bisegs,[bisegs[i,0],rpos-1]))
 			if (bisegs[i,1] - rpos +1) > minseglen :
```

### Comparing `copent-0.5.4/copent.egg-info/PKG-INFO` & `copent-0.5.5/copent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copent
-Version: 0.5.4
+Version: 0.5.5
 Summary: Estimating Copula Entropy and Transfer Entropy
 Home-page: https://github.com/majianthu/pycopent
 Author: MA Jian
 Author-email: majian03@gmail.com
 License: GPL License
 Platform: UNKNOWN
 Requires-Python: >=2.7
```

### Comparing `copent-0.5.4/setup.py` & `copent-0.5.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="copent",
-    version="0.5.4",
+    version="0.5.5",
     author="MA Jian",
     author_email="majian03@gmail.com",
     description="Estimating Copula Entropy and Transfer Entropy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license = 'GPL License',
     url="https://github.com/majianthu/pycopent",
```

