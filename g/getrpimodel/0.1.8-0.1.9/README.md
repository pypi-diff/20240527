# Comparing `tmp/getrpimodel-0.1.8.tar.gz` & `tmp/getrpimodel-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/getrpimodel-0.1.8.tar", last modified: Thu Feb 16 12:37:53 2017, max compression
+gzip compressed data, was "dist/getrpimodel-0.1.9.tar", last modified: Tue Feb 21 11:58:07 2017, max compression
```

## Comparing `getrpimodel-0.1.8.tar` & `getrpimodel-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2017-02-16 12:37:53.000000 getrpimodel-0.1.8/
--rw-r--r--   0 pi        (1000) pi        (1000)      422 2017-02-16 12:37:53.000000 getrpimodel-0.1.8/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2017-02-16 12:37:53.000000 getrpimodel-0.1.8/getrpimodel/
--rw-r--r--   0 pi        (1000) pi        (1000)     2401 2017-02-16 12:26:19.000000 getrpimodel-0.1.8/getrpimodel/getrpimodel.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2222 2017-02-16 02:36:45.000000 getrpimodel-0.1.8/getrpimodel/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)      270 2017-02-16 02:36:45.000000 getrpimodel-0.1.8/getrpimodel/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)      609 2017-02-16 12:37:21.000000 getrpimodel-0.1.8/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)       40 2017-02-16 02:36:45.000000 getrpimodel-0.1.8/setup.cfg
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2017-02-21 11:58:07.000000 getrpimodel-0.1.9/
+-rw-r--r--   0 pi        (1000) pi        (1000)      422 2017-02-21 11:58:07.000000 getrpimodel-0.1.9/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2017-02-21 11:58:07.000000 getrpimodel-0.1.9/getrpimodel/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2401 2017-02-21 11:54:59.000000 getrpimodel-0.1.9/getrpimodel/getrpimodel.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2401 2017-02-21 11:55:57.000000 getrpimodel-0.1.9/getrpimodel/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      270 2017-02-21 11:54:59.000000 getrpimodel-0.1.9/getrpimodel/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      609 2017-02-21 11:57:18.000000 getrpimodel-0.1.9/setup.py
+-rw-r--r--   0 pi        (1000) pi        (1000)       40 2017-02-21 11:54:59.000000 getrpimodel-0.1.9/setup.cfg
```

### Comparing `getrpimodel-0.1.8/getrpimodel/getrpimodel.py` & `getrpimodel-0.1.9/getrpimodel/getrpimodel.py`

 * *Files identical despite different names*

### Comparing `getrpimodel-0.1.8/getrpimodel/__init__.py` & `getrpimodel-0.1.9/getrpimodel/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 # © Takeyuki UEDA 2016 -.
 
 #import getpirevision
 import re
 import sys
 
 
-usage = 'Usage: python {} [--s]'.format(__file__)
+usage = 'Usage: python -m getrpimodel [--s]'
 
 # model definition table from revision info.
 # refer http://elinux.org/RPi_HardwareHistory
 model_a          = ["0007","0008","0009",]
-model_b          = ["0002","0004","0005","0006",]
+model_b          = ["0002","0004","0005","0006","000d","000e","000e",]
 model_b_beta     = ["Beta",]
 model_b_ECN0001  = ["0003",]
-model_cm         = ["0011","0011",]
-model_a_plus     = ["0012","0015",]
+model_cm         = ["0011","0014",]
+model_cm3        = ["a020a0",]
+model_a_plus     = ["0012","0015","900021",]
 model_b_plus     = ["0010","0013",]
 model_2b         = ["a01040","a01041","a21041",]
 model_2b_2837    = ["a22042",]
-model_3b         = ["a02082", "a22082",]
+model_3b         = ["a02082", "a22082","a32082",]
 model_zero       = ["900092","900093","920093",]
 
 def revision():
   revision = "unknown"
   with open('/proc/cpuinfo', 'r') as f:
     for line in f:
       m = re.search('Revision.*: ([0123456789abcdef]*)', line)
@@ -41,54 +42,58 @@
     return "B"
   elif rev in model_b_beta:
     return "B (Beta)"
   elif rev in model_b_ECN0001:
     return "B (ECN0001)"
   elif rev in model_cm:
     return "Compute Module"
+  elif rev in model_cm3:
+    return "Compute Module 3(and CM3 Lite)"
   elif rev in model_a_plus:
     return "A+"
   elif rev in model_b_plus:
     return "B+"
   elif rev in model_2b:
     return "2 Model B"
   elif rev in model_2b_2837:
     return "2 Model B (with BCM2837)"
   elif rev in model_3b:
     return "3 Model B"
   elif rev in model_zero:
     return "Zero"
   else:
-    return None
+    return rev
+#    return None
 
 def model():
 #  rev = getpirevision.revision()
   rev = revision()
   if rev in model_a:
     return "A"
   elif rev in model_b + model_b_beta + model_b_ECN0001:
     return "B"
-  elif rev in model_cm:
+  elif rev in model_cm + model_cm3:
     return "Compute Module"
   elif rev in model_a_plus:
     return "A+"
   elif rev in model_b_plus:
     return "B+"
   elif rev in model_2b + model_2b_2837:
     return "2 Model B"
   elif rev in model_3b:
     return "3 Model B"
   elif rev in model_zero:
     return "Zero"
   else:
-    return None
+    return rev
+#    return None
 
 if __name__ == '__main__':
   if len(sys.argv) == 1:
     print (model())
   elif len(sys.argv) == 2:
     if sys.argv[1] == '--s':
       print (model_strict())
     else:
       print usage
   else:
-    print usage
+    print usage
```

### Comparing `getrpimodel-0.1.8/setup.py` & `getrpimodel-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'getrpimodel',
   packages = ['getrpimodel'], # this must be the same as the name above
-  version = '0.1.8',
+  version = '0.1.9',
   description = 'Get Raspberry Pi model Name(eg: A, B, B+...)',
   author = 'Takeyuki UEDA',
   author_email = 'gde00107@nifty.com',
   license='MIT',
   url = 'https://github.com/UedaTakeyuki/getrpimodel', # use the URL to the github repo
   keywords = ['testing', 'logging', 'example'], # arbitrary keywords
   classifiers = ['Development Status :: 4 - Beta',
```

