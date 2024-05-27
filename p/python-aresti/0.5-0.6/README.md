# Comparing `tmp/python-aresti-0.5.tar.gz` & `tmp/python_aresti-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-aresti-0.5.tar", last modified: Tue Jun 13 09:27:30 2023, max compression
+gzip compressed data, was "python_aresti-0.6.tar", last modified: Mon May 27 06:36:56 2024, max compression
```

## Comparing `python-aresti-0.5.tar` & `python_aresti-0.6.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-13 09:27:30.502029 python-aresti-0.5/
--rw-r--r--   0 aha        (501) staff       (20)      245 2023-06-13 09:27:30.501866 python-aresti-0.5/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)       71 2022-02-21 07:37:57.000000 python-aresti-0.5/README.md
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-13 09:27:30.498959 python-aresti-0.5/aresti/
--rw-r--r--   0 aha        (501) staff       (20)      141 2023-06-02 11:14:09.000000 python-aresti-0.5/aresti/__init__.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-13 09:27:30.500658 python-aresti-0.5/aresti/rajapinta/
--rw-r--r--   0 aha        (501) staff       (20)     3557 2023-01-08 12:22:04.000000 python-aresti-0.5/aresti/rajapinta/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      915 2022-12-27 18:18:56.000000 python-aresti-0.5/aresti/rajapinta/meta.py
--rw-r--r--   0 aha        (501) staff       (20)     6094 2023-01-08 12:22:55.000000 python-aresti-0.5/aresti/rajapinta/nakyma.py
--rw-r--r--   0 aha        (501) staff       (20)     1184 2023-01-02 14:19:10.000000 python-aresti-0.5/aresti/rajapinta/tyokalut.py
--rw-r--r--   0 aha        (501) staff       (20)     1715 2023-01-07 19:04:34.000000 python-aresti-0.5/aresti/rajapinta/vierasavain.py
--rw-r--r--   0 aha        (501) staff       (20)     3387 2023-06-08 10:10:22.000000 python-aresti-0.5/aresti/rest.py
--rw-r--r--   0 aha        (501) staff       (20)     1822 2022-09-14 10:13:57.000000 python-aresti-0.5/aresti/sanoma.py
--rw-r--r--   0 aha        (501) staff       (20)     1582 2022-08-29 18:09:52.000000 python-aresti-0.5/aresti/testi.py
--rw-r--r--   0 aha        (501) staff       (20)     2345 2023-06-05 08:50:11.000000 python-aresti-0.5/aresti/tyokalut.py
--rw-r--r--   0 aha        (501) staff       (20)     5253 2023-06-02 11:25:21.000000 python-aresti-0.5/aresti/yhteys.py
--rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-05 11:17:11.000000 python-aresti-0.5/pyproject.toml
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-06-13 09:27:30.501690 python-aresti-0.5/python_aresti.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      245 2023-06-13 09:27:30.000000 python-aresti-0.5/python_aresti.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      499 2023-06-13 09:27:30.000000 python-aresti-0.5/python_aresti.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2023-06-13 09:27:30.000000 python-aresti-0.5/python_aresti.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)     4020 2023-06-13 09:27:30.000000 python-aresti-0.5/python_aresti.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)        8 2023-06-13 09:27:30.000000 python-aresti-0.5/python_aresti.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)        7 2023-06-13 09:27:30.000000 python-aresti-0.5/python_aresti.egg-info/top_level.txt
--rw-r--r--   0 aha        (501) staff       (20)       38 2023-06-13 09:27:30.502082 python-aresti-0.5/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      461 2023-06-05 07:39:26.000000 python-aresti-0.5/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-05-27 06:36:56.974424 python_aresti-0.6/
+-rw-r--r--   0 aha        (501) staff       (20)      268 2024-05-27 06:36:56.974104 python_aresti-0.6/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)       71 2022-02-21 07:37:57.000000 python_aresti-0.6/README.md
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-05-27 06:36:56.971357 python_aresti-0.6/aresti/
+-rw-r--r--   0 aha        (501) staff       (20)      215 2024-05-26 09:26:09.000000 python_aresti-0.6/aresti/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)     1894 2024-05-26 09:26:09.000000 python_aresti-0.6/aresti/json.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-05-27 06:36:56.972746 python_aresti-0.6/aresti/rajapinta-vanha/
+-rw-r--r--   0 aha        (501) staff       (20)     3557 2023-01-08 12:22:04.000000 python_aresti-0.6/aresti/rajapinta-vanha/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      915 2022-12-27 18:18:56.000000 python_aresti-0.6/aresti/rajapinta-vanha/meta.py
+-rw-r--r--   0 aha        (501) staff       (20)     6094 2023-01-08 12:22:55.000000 python_aresti-0.6/aresti/rajapinta-vanha/nakyma.py
+-rw-r--r--   0 aha        (501) staff       (20)     1184 2023-01-02 14:19:10.000000 python_aresti-0.6/aresti/rajapinta-vanha/tyokalut.py
+-rw-r--r--   0 aha        (501) staff       (20)     1715 2023-01-07 19:04:34.000000 python_aresti-0.6/aresti/rajapinta-vanha/vierasavain.py
+-rw-r--r--   0 aha        (501) staff       (20)     4071 2024-05-26 09:26:09.000000 python_aresti-0.6/aresti/rajapinta.py
+-rw-r--r--   0 aha        (501) staff       (20)     2285 2024-05-27 05:46:26.000000 python_aresti-0.6/aresti/rest.py
+-rw-r--r--   0 aha        (501) staff       (20)     3882 2024-05-26 09:26:09.000000 python_aresti-0.6/aresti/sanoma.py
+-rw-r--r--   0 aha        (501) staff       (20)     1582 2022-08-29 18:09:52.000000 python_aresti-0.6/aresti/testi.py
+-rw-r--r--   0 aha        (501) staff       (20)     2345 2024-05-23 07:13:23.000000 python_aresti-0.6/aresti/tyokalut.py
+-rw-r--r--   0 aha        (501) staff       (20)     5253 2024-05-26 09:25:57.000000 python_aresti-0.6/aresti/yhteys.py
+-rw-r--r--   0 aha        (501) staff       (20)       80 2024-05-26 09:25:57.000000 python_aresti-0.6/pyproject.toml
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-05-27 06:36:56.973840 python_aresti-0.6/python_aresti.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      268 2024-05-27 06:36:56.000000 python_aresti-0.6/python_aresti.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      564 2024-05-27 06:36:56.000000 python_aresti-0.6/python_aresti.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2024-05-27 06:36:56.000000 python_aresti-0.6/python_aresti.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)     4523 2024-05-27 06:36:56.000000 python_aresti-0.6/python_aresti.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)        8 2024-05-27 06:36:56.000000 python_aresti-0.6/python_aresti.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)        7 2024-05-27 06:36:56.000000 python_aresti-0.6/python_aresti.egg-info/top_level.txt
+-rw-r--r--   0 aha        (501) staff       (20)       38 2024-05-27 06:36:56.974475 python_aresti-0.6/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      414 2024-05-26 09:25:57.000000 python_aresti-0.6/setup.py
```

### Comparing `python-aresti-0.5/aresti/rajapinta/__init__.py` & `python_aresti-0.6/aresti/rajapinta-vanha/__init__.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.5/aresti/rajapinta/meta.py` & `python_aresti-0.6/aresti/rajapinta-vanha/meta.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.5/aresti/rajapinta/nakyma.py` & `python_aresti-0.6/aresti/rajapinta-vanha/nakyma.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.5/aresti/rajapinta/tyokalut.py` & `python_aresti-0.6/aresti/rajapinta-vanha/tyokalut.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.5/aresti/rajapinta/vierasavain.py` & `python_aresti-0.6/aresti/rajapinta-vanha/vierasavain.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.5/aresti/testi.py` & `python_aresti-0.6/aresti/testi.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.5/aresti/tyokalut.py` & `python_aresti-0.6/aresti/tyokalut.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.5/aresti/yhteys.py` & `python_aresti-0.6/aresti/yhteys.py`

 * *Files identical despite different names*

### Comparing `python-aresti-0.5/python_aresti.egg-info/historia.json` & `python_aresti-0.6/python_aresti.egg-info/historia.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8846153846153846%*

 * *Differences: {'insert': "[(0, OrderedDict([('revisio', '7e51f3c5c590668e2c77a02cf10f6ef0464d2912'), ('versio', "*

 * *           "'0.6'), ('kuvaus', 'Lisätty `Rajapinta`-dataluokka')])), (1, OrderedDict([('revisio', "*

 * *           "'2b0ca3f43c4bd64187e53dc74bb5e6e3f6d7e4f7'), ('versio', '0.5.2'), ('kuvaus', "*

 * *           "'Tekijöistettu JSON-viestinvaihto erilliseen saateluokkaan')])), (2, "*

 * *           "OrderedDict([('revisio', 'f2ae585a2b86ef2fd6d8c3a28c3549f6d22c1fb3'), ('versio', "*

 * *           "'0.5.1'), ('kuvaus', 'Lisätty e […]*

```diff
@@ -1,9 +1,24 @@
 [
     {
+        "kuvaus": "Lis\u00e4tty `Rajapinta`-dataluokka",
+        "revisio": "7e51f3c5c590668e2c77a02cf10f6ef0464d2912",
+        "versio": "0.6"
+    },
+    {
+        "kuvaus": "Tekij\u00f6istettu JSON-viestinvaihto erilliseen saateluokkaan",
+        "revisio": "2b0ca3f43c4bd64187e53dc74bb5e6e3f6d7e4f7",
+        "versio": "0.5.2"
+    },
+    {
+        "kuvaus": "Lis\u00e4tty erillinen `RestKentta`-saateluokka: `lahteva`- ja `saapuva`-toteutukset",
+        "revisio": "f2ae585a2b86ef2fd6d8c3a28c3549f6d22c1fb3",
+        "versio": "0.5.1"
+    },
+    {
         "kuvaus": "Korjattu `nouda_sivutettu_data`",
         "revisio": "abb9fe3f792cf12027d91034c6a08245641f0eb2",
         "versio": "0.5"
     },
     {
         "kuvaus": "PEP 517 -yhteensopivuus",
         "revisio": "4b7cbfd6b7bfe7efe2ff036abe2569aea0f2d281",
```

