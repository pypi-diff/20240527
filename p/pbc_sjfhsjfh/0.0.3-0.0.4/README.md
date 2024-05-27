# Comparing `tmp/pbc_sjfhsjfh-0.0.3.tar.gz` & `tmp/pbc_sjfhsjfh-0.0.4.tar.gz`

## Comparing `pbc_sjfhsjfh-0.0.3.tar` & `pbc_sjfhsjfh-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.3/requirements.txt
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.3/src/pbc/__init__.py
--rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.3/src/pbc/bin.py
--rw-r--r--   0        0        0     7331 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.3/src/pbc/phira_chart.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.3/src/pbc/utils/__init__.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.3/src/pbc/utils/fraction.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.3/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.3/LICENSE
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.3/README.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/src/pbc/__init__.py
+-rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/src/pbc/bin.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/src/pbc/phira_chart.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/src/pbc/utils/__init__.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/src/pbc/utils/fraction.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/LICENSE
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/README.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/PKG-INFO
```

### Comparing `pbc_sjfhsjfh-0.0.3/src/pbc/bin.py` & `pbc_sjfhsjfh-0.0.4/src/pbc/bin.py`

 * *Files identical despite different names*

### Comparing `pbc_sjfhsjfh-0.0.3/src/pbc/phira_chart.py` & `pbc_sjfhsjfh-0.0.4/src/pbc/phira_chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         Args:
             time (float): time
             value (T): value
             tween (int): tween function id, see [here](https://github.com/TeamFlos/phira/blob/98fcaccda75db867232fe65bbacbae56a2b5d928/prpr/src/core/tween.rs#L100)
         """
         self.time = time
         self.value = value
+        self.tween = tween
 
 
 class PhiraAnim(Generic[T]):
     def __init__(
         self,
         time: float = 0.,
         keyframes: List[PhiraKeyFrame[T]] = [],
```

### Comparing `pbc_sjfhsjfh-0.0.3/src/pbc/utils/fraction.py` & `pbc_sjfhsjfh-0.0.4/src/pbc/utils/fraction.py`

 * *Files identical despite different names*

### Comparing `pbc_sjfhsjfh-0.0.3/LICENSE` & `pbc_sjfhsjfh-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pbc_sjfhsjfh-0.0.3/pyproject.toml` & `pbc_sjfhsjfh-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pbc_sjfhsjfh"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "sjfhsjfh", email = "sjfhsjfh@qq.com" }]
 description = "Phira chart structure package"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

