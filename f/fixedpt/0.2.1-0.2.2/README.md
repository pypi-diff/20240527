# Comparing `tmp/fixedpt-0.2.1.tar.gz` & `tmp/fixedpt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixedpt-0.2.1.tar", last modified: Fri Nov 18 23:05:55 2022, max compression
+gzip compressed data, was "fixedpt-0.2.2.tar", last modified: Mon May 27 17:30:31 2024, max compression
```

## Comparing `fixedpt-0.2.1.tar` & `fixedpt-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 almund    (1000) almund    (1000)        0 2022-11-18 23:05:55.809850 fixedpt-0.2.1/
--rw-rw-r--   0 almund    (1000) almund    (1000)      121 2022-11-18 23:05:55.809850 fixedpt-0.2.1/PKG-INFO
--rw-rw-r--   0 almund    (1000) almund    (1000)        0 2022-10-27 01:45:13.000000 fixedpt-0.2.1/README.md
--rw-rw-r--   0 almund    (1000) almund    (1000)       38 2022-11-18 23:05:55.809850 fixedpt-0.2.1/setup.cfg
--rw-rw-r--   0 almund    (1000) almund    (1000)      252 2022-11-18 23:05:27.000000 fixedpt-0.2.1/setup.py
-drwxrwxr-x   0 almund    (1000) almund    (1000)        0 2022-11-18 23:05:55.805850 fixedpt-0.2.1/src/
-drwxrwxr-x   0 almund    (1000) almund    (1000)        0 2022-11-18 23:05:55.805850 fixedpt-0.2.1/src/fixedpt/
--rw-rw-r--   0 almund    (1000) almund    (1000)       51 2022-11-18 21:25:47.000000 fixedpt-0.2.1/src/fixedpt/__init__.py
--rw-rw-r--   0 almund    (1000) almund    (1000)     4357 2022-11-18 23:03:58.000000 fixedpt-0.2.1/src/fixedpt/cfixed.py
--rw-rw-r--   0 almund    (1000) almund    (1000)     5633 2022-11-18 21:43:42.000000 fixedpt-0.2.1/src/fixedpt/fixed.py
-drwxrwxr-x   0 almund    (1000) almund    (1000)        0 2022-11-18 23:05:55.809850 fixedpt-0.2.1/src/fixedpt.egg-info/
--rw-rw-r--   0 almund    (1000) almund    (1000)      121 2022-11-18 23:05:55.000000 fixedpt-0.2.1/src/fixedpt.egg-info/PKG-INFO
--rw-rw-r--   0 almund    (1000) almund    (1000)      225 2022-11-18 23:05:55.000000 fixedpt-0.2.1/src/fixedpt.egg-info/SOURCES.txt
--rw-rw-r--   0 almund    (1000) almund    (1000)        1 2022-11-18 23:05:55.000000 fixedpt-0.2.1/src/fixedpt.egg-info/dependency_links.txt
--rw-rw-r--   0 almund    (1000) almund    (1000)        8 2022-11-18 23:05:55.000000 fixedpt-0.2.1/src/fixedpt.egg-info/top_level.txt
+drwxr-xr-x   0 almund    (1000) almund    (1000)        0 2024-05-27 17:30:31.730877 fixedpt-0.2.2/
+-rw-r--r--   0 almund    (1000) almund    (1000)      121 2024-05-27 17:30:31.730877 fixedpt-0.2.2/PKG-INFO
+-rw-r--r--   0 almund    (1000) almund    (1000)        0 2024-05-27 17:04:12.000000 fixedpt-0.2.2/README.md
+-rw-r--r--   0 almund    (1000) almund    (1000)       38 2024-05-27 17:30:31.730877 fixedpt-0.2.2/setup.cfg
+-rw-r--r--   0 almund    (1000) almund    (1000)      252 2024-05-27 17:29:41.000000 fixedpt-0.2.2/setup.py
+drwxr-xr-x   0 almund    (1000) almund    (1000)        0 2024-05-27 17:30:31.720877 fixedpt-0.2.2/src/
+drwxr-xr-x   0 almund    (1000) almund    (1000)        0 2024-05-27 17:30:31.720877 fixedpt-0.2.2/src/fixedpt/
+-rw-r--r--   0 almund    (1000) almund    (1000)       51 2024-05-27 17:04:12.000000 fixedpt-0.2.2/src/fixedpt/__init__.py
+-rw-r--r--   0 almund    (1000) almund    (1000)     4357 2024-05-27 17:04:12.000000 fixedpt-0.2.2/src/fixedpt/cfixed.py
+-rw-r--r--   0 almund    (1000) almund    (1000)     5899 2024-05-27 17:19:08.000000 fixedpt-0.2.2/src/fixedpt/fixed.py
+drwxr-xr-x   0 almund    (1000) almund    (1000)        0 2024-05-27 17:30:31.730877 fixedpt-0.2.2/src/fixedpt.egg-info/
+-rw-r--r--   0 almund    (1000) almund    (1000)      121 2024-05-27 17:30:31.000000 fixedpt-0.2.2/src/fixedpt.egg-info/PKG-INFO
+-rw-r--r--   0 almund    (1000) almund    (1000)      266 2024-05-27 17:30:31.000000 fixedpt-0.2.2/src/fixedpt.egg-info/SOURCES.txt
+-rw-r--r--   0 almund    (1000) almund    (1000)        1 2024-05-27 17:30:31.000000 fixedpt-0.2.2/src/fixedpt.egg-info/dependency_links.txt
+-rw-r--r--   0 almund    (1000) almund    (1000)        8 2024-05-27 17:30:31.000000 fixedpt-0.2.2/src/fixedpt.egg-info/top_level.txt
+drwxr-xr-x   0 almund    (1000) almund    (1000)        0 2024-05-27 17:30:31.730877 fixedpt-0.2.2/tests/
+-rw-r--r--   0 almund    (1000) almund    (1000)     1914 2024-05-27 17:14:46.000000 fixedpt-0.2.2/tests/test_cfixed.py
+-rw-r--r--   0 almund    (1000) almund    (1000)     2505 2024-05-27 17:14:52.000000 fixedpt-0.2.2/tests/test_fixed.py
```

### Comparing `fixedpt-0.2.1/src/fixedpt/cfixed.py` & `fixedpt-0.2.2/src/fixedpt/cfixed.py`

 * *Files identical despite different names*

### Comparing `fixedpt-0.2.1/src/fixedpt/fixed.py` & `fixedpt-0.2.2/src/fixedpt/fixed.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from decimal import Decimal
+from __future__ import annotations
 
 # Fixed point number
 class Fixed():
 	# INVARIANT:
 	# n >= d
 	# d >= 0
 	# signed = 0 or 1
 
-	def __init__(self, v=0, signed=0, n=32, d=16, raw=False):
+	def __init__(self, v: Fixed | int | float | Decimal, signed: bool, n: int, d: int, raw: bool = False) -> Fixed:
 		if (signed + d > n) or (signed >= n):
 			raise ValueError(f"Too many decimal places! ({signed} sign bits, {n} total bits, {d} decimal bits)")
 		self._signed = signed
 		self._n = n
 		self._d = d
 
 		self.set(v, raw)
 
 	@staticmethod
-	def cast(o, d=64): # casts a fixed value and copies it with default precision
+	def cast(o: Fixed | int | float | Decimal, d: int = 64) -> Fixed: # casts a fixed value and copies it with default precision
 		if (isinstance(o, Fixed)):
 			return o.clone()
 		
 		elif (isinstance(o, int)):
 			return Fixed(o, 1, max(1, o.bit_length()) + 1, 0)
 
 		elif (isinstance(o, float)):
@@ -31,43 +32,43 @@
 			i = int(o * (1 << d))
 			return Fixed(i, 1, max(1, int(i).bit_length()) + 1, d, raw=True)
 
 		else:
 			raise ValueError(f"Casting from invalid type {type(o)}")
 
 
-	def clone(self): # clone a Fixed
+	def clone(self) -> Fixed: # clone a Fixed
 		return Fixed(self.get(), self._signed, self._n, self._d, raw=True)
 
-	def set(self, k, raw=False):
+	def set(self, k: int | float | Decimal, raw: bool = False) -> None:
 		if not raw:
 			k = int(k * (1 << self._d))
 		else:
 			k = int(k)
 		self._data = k % (1 << len(self))
 
-	def get(self, raw=True): # get raw value
+	def get(self, raw: bool = True) -> int: # get raw value
 		if raw or (not self.is_neg()):
 			return self._data
 		else:
 			return self._data - (1 << len(self))
 
-	def is_neg(self):
+	def is_neg(self) -> bool:
 		return bool(self._signed and self[-1])
 
-	def fixed_left_shift(self, s): # left shift while fixing d
+	def fixed_left_shift(self, s: int) -> Fixed: # left shift while fixing d
 		self._data <<= s
 		self._n += s;
 		return self
 
-	def fixed_right_shift(self, s): # right shift while fixing d
+	def fixed_right_shift(self, s: int) -> Fixed: # right shift while fixing d
 		self._data >>= s
 		return self
 
-	def resize(self, signed=None, n=None, d=None):
+	def resize(self, signed: bool | None, n: int | None, d: int | None) -> Fixed:
 		n = n if n is not None else self._n
 		if signed and not self._signed:
 			n = n + 1
 		
 		if d is not None and d != self._d:
 			if d > self._d:
 				self.fixed_left_shift(d - self._d) # pad right
@@ -117,30 +118,30 @@
 
 	def __getitem__(self, key): # returns the nth bit of the number
 		return (self._data >> (key % len(self))) & 1
 
 ### OPERATORS
 
 	def __neg__(self):
-		t = self.clone();
+		t = self.clone()
 
 		# special case to add an extra bit when we are at MIN_INT
 		if self.is_neg() and self.get() == (1 << (len(self)-1)): 
 			t.resize(None, len(self)+1, None)
 
 		t.set(-t._data, raw=True)
 		return t
 
 	def __invert__(self):
 		t = self.clone()
 		t.set(-t._data - 1, raw=True)
 		return t
 
 	def __abs__(self):
-		return (-self) if self.is_neg else self.clone();
+		return (-self) if self.is_neg() else self.clone()
 
 	def __ilshift__(self, s):
 		if s > self._d:
 			self.fixed_left_shift(s-self._d) # do a real left shift here
 			self._d = 0
 		else:
 			self._d -= s
```

