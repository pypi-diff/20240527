# Comparing `tmp/damage_calculator-0.2.0.tar.gz` & `tmp/damage_calculator-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damage_calculator-0.2.0.tar", last modified: Mon May 27 04:32:54 2024, max compression
+gzip compressed data, was "damage_calculator-0.3.0.tar", last modified: Mon May 27 04:37:04 2024, max compression
```

## Comparing `damage_calculator-0.2.0.tar` & `damage_calculator-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 siro       (501) staff       (20)        0 2024-05-27 04:32:54.765582 damage_calculator-0.2.0/
--rw-r--r--   0 siro       (501) staff       (20)     1065 2024-05-24 03:59:28.000000 damage_calculator-0.2.0/LICENSE
--rw-r--r--   0 siro       (501) staff       (20)      896 2024-05-27 04:32:54.765207 damage_calculator-0.2.0/PKG-INFO
--rw-r--r--   0 siro       (501) staff       (20)      433 2024-05-27 04:29:01.000000 damage_calculator-0.2.0/README.md
-drwxr-xr-x   0 siro       (501) staff       (20)        0 2024-05-27 04:32:54.760798 damage_calculator-0.2.0/damage_calculator/
--rw-r--r--   0 siro       (501) staff       (20)       32 2024-05-24 03:59:28.000000 damage_calculator-0.2.0/damage_calculator/__init__.py
--rw-r--r--   0 siro       (501) staff       (20)     1579 2024-05-24 03:59:28.000000 damage_calculator-0.2.0/damage_calculator/calculator.py
-drwxr-xr-x   0 siro       (501) staff       (20)        0 2024-05-27 04:32:54.764836 damage_calculator-0.2.0/damage_calculator.egg-info/
--rw-r--r--   0 siro       (501) staff       (20)      896 2024-05-27 04:32:54.000000 damage_calculator-0.2.0/damage_calculator.egg-info/PKG-INFO
--rw-r--r--   0 siro       (501) staff       (20)      296 2024-05-27 04:32:54.000000 damage_calculator-0.2.0/damage_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 siro       (501) staff       (20)        1 2024-05-27 04:32:54.000000 damage_calculator-0.2.0/damage_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 siro       (501) staff       (20)       72 2024-05-27 04:32:54.000000 damage_calculator-0.2.0/damage_calculator.egg-info/entry_points.txt
--rw-r--r--   0 siro       (501) staff       (20)       18 2024-05-27 04:32:54.000000 damage_calculator-0.2.0/damage_calculator.egg-info/top_level.txt
--rw-r--r--   0 siro       (501) staff       (20)       38 2024-05-27 04:32:54.765648 damage_calculator-0.2.0/setup.cfg
--rw-r--r--   0 siro       (501) staff       (20)      794 2024-05-27 04:32:32.000000 damage_calculator-0.2.0/setup.py
+drwxr-xr-x   0 siro       (501) staff       (20)        0 2024-05-27 04:37:04.735277 damage_calculator-0.3.0/
+-rw-r--r--   0 siro       (501) staff       (20)     1065 2024-05-24 03:59:28.000000 damage_calculator-0.3.0/LICENSE
+-rw-r--r--   0 siro       (501) staff       (20)     1228 2024-05-27 04:37:04.734869 damage_calculator-0.3.0/PKG-INFO
+-rw-r--r--   0 siro       (501) staff       (20)      765 2024-05-27 04:36:56.000000 damage_calculator-0.3.0/README.md
+drwxr-xr-x   0 siro       (501) staff       (20)        0 2024-05-27 04:37:04.729376 damage_calculator-0.3.0/damage_calculator/
+-rw-r--r--   0 siro       (501) staff       (20)       32 2024-05-24 03:59:28.000000 damage_calculator-0.3.0/damage_calculator/__init__.py
+-rw-r--r--   0 siro       (501) staff       (20)     1579 2024-05-24 03:59:28.000000 damage_calculator-0.3.0/damage_calculator/calculator.py
+drwxr-xr-x   0 siro       (501) staff       (20)        0 2024-05-27 04:37:04.734550 damage_calculator-0.3.0/damage_calculator.egg-info/
+-rw-r--r--   0 siro       (501) staff       (20)     1228 2024-05-27 04:37:04.000000 damage_calculator-0.3.0/damage_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 siro       (501) staff       (20)      296 2024-05-27 04:37:04.000000 damage_calculator-0.3.0/damage_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 siro       (501) staff       (20)        1 2024-05-27 04:37:04.000000 damage_calculator-0.3.0/damage_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 siro       (501) staff       (20)       72 2024-05-27 04:37:04.000000 damage_calculator-0.3.0/damage_calculator.egg-info/entry_points.txt
+-rw-r--r--   0 siro       (501) staff       (20)       18 2024-05-27 04:37:04.000000 damage_calculator-0.3.0/damage_calculator.egg-info/top_level.txt
+-rw-r--r--   0 siro       (501) staff       (20)       38 2024-05-27 04:37:04.735316 damage_calculator-0.3.0/setup.cfg
+-rw-r--r--   0 siro       (501) staff       (20)      794 2024-05-27 04:36:56.000000 damage_calculator-0.3.0/setup.py
```

### Comparing `damage_calculator-0.2.0/LICENSE` & `damage_calculator-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `damage_calculator-0.2.0/PKG-INFO` & `damage_calculator-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damage_calculator
-Version: 0.2.0
+Version: 0.3.0
 Summary: A simple Pokemon damage calculator
 Home-page: https://github.com/siro-rai/pokemon_damade_ver.2.git
 Author: siro_rai
 Author-email: s2222013@stu.musashino-u.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,8 +21,23 @@
 attacker_attack = 150  # Attack stat of the attacking Pokémon
 defender_defense = 100  # Defense stat of the defending Pokémon
 stab = 1.5  # Same Type Attack Bonus (STAB)
 type_effectiveness = 2.0  # Type effectiveness (e.g., super effective)
 
 result=x
 
+# Pokémon Damage Calculator
+
+A simple Pokémon damage calculator.
+
+## Installation
+
+You can install the package using pip. First, ensure you have downloaded the package file (e.g., `pokemon_damage_calculator-0.2.0.tar.gz`).
+
+### Using pip
+
+If you have the package file:
+
+```bash
+pip install pokemon_damage_calculator-0.3.0.tar.gz
+
```

### Comparing `damage_calculator-0.2.0/damage_calculator/calculator.py` & `damage_calculator-0.3.0/damage_calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `damage_calculator-0.2.0/damage_calculator.egg-info/PKG-INFO` & `damage_calculator-0.3.0/damage_calculator.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damage_calculator
-Version: 0.2.0
+Version: 0.3.0
 Summary: A simple Pokemon damage calculator
 Home-page: https://github.com/siro-rai/pokemon_damade_ver.2.git
 Author: siro_rai
 Author-email: s2222013@stu.musashino-u.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,8 +21,23 @@
 attacker_attack = 150  # Attack stat of the attacking Pokémon
 defender_defense = 100  # Defense stat of the defending Pokémon
 stab = 1.5  # Same Type Attack Bonus (STAB)
 type_effectiveness = 2.0  # Type effectiveness (e.g., super effective)
 
 result=x
 
+# Pokémon Damage Calculator
+
+A simple Pokémon damage calculator.
+
+## Installation
+
+You can install the package using pip. First, ensure you have downloaded the package file (e.g., `pokemon_damage_calculator-0.2.0.tar.gz`).
+
+### Using pip
+
+If you have the package file:
+
+```bash
+pip install pokemon_damage_calculator-0.3.0.tar.gz
+
```

### Comparing `damage_calculator-0.2.0/setup.py` & `damage_calculator-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name="damage_calculator",
-    version="0.2.0",
+    version="0.3.0",
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'damage_calculator = damage_calculator.calculator:main',
         ],
     },
     install_requires=[],
```

