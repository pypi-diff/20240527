# Comparing `tmp/bpetokenizer-1.0.0.tar.gz` & `tmp/bpetokenizer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpetokenizer-1.0.0.tar", last modified: Mon May 27 09:25:30 2024, max compression
+gzip compressed data, was "bpetokenizer-1.0.1.tar", last modified: Mon May 27 18:18:56 2024, max compression
```

## Comparing `bpetokenizer-1.0.0.tar` & `bpetokenizer-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 09:25:30.442089 bpetokenizer-1.0.0/
--rw-rw-rw-   0        0        0      600 2024-05-27 09:25:30.438998 bpetokenizer-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       18 2024-05-27 09:01:58.000000 bpetokenizer-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 09:25:30.434365 bpetokenizer-1.0.0/bpetokenizer.egg-info/
--rw-rw-rw-   0        0        0      600 2024-05-27 09:25:29.000000 bpetokenizer-1.0.0/bpetokenizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-05-27 09:25:30.000000 bpetokenizer-1.0.0/bpetokenizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 09:25:29.000000 bpetokenizer-1.0.0/bpetokenizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-27 09:25:29.000000 bpetokenizer-1.0.0/bpetokenizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 09:25:29.000000 bpetokenizer-1.0.0/bpetokenizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 09:25:30.442089 bpetokenizer-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1162 2024-05-27 09:24:14.000000 bpetokenizer-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 09:25:30.430317 bpetokenizer-1.0.0/tests/
--rw-rw-rw-   0        0        0      945 2024-05-27 07:10:18.000000 bpetokenizer-1.0.0/tests/test_tokenizer.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:18:56.909775 bpetokenizer-1.0.1/
+-rw-rw-rw-   0        0        0     5787 2024-05-27 18:18:56.907666 bpetokenizer-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5181 2024-05-27 17:12:12.000000 bpetokenizer-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 18:18:56.905480 bpetokenizer-1.0.1/bpetokenizer.egg-info/
+-rw-rw-rw-   0        0        0     5787 2024-05-27 18:18:56.000000 bpetokenizer-1.0.1/bpetokenizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-05-27 18:18:56.000000 bpetokenizer-1.0.1/bpetokenizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 18:18:56.000000 bpetokenizer-1.0.1/bpetokenizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-27 18:18:56.000000 bpetokenizer-1.0.1/bpetokenizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 18:18:56.000000 bpetokenizer-1.0.1/bpetokenizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 18:18:56.909775 bpetokenizer-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1169 2024-05-27 17:19:44.000000 bpetokenizer-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:18:56.903436 bpetokenizer-1.0.1/tests/
+-rw-rw-rw-   0        0        0      945 2024-05-27 07:10:18.000000 bpetokenizer-1.0.1/tests/test_tokenizer.py
```

### Comparing `bpetokenizer-1.0.0/setup.py` & `bpetokenizer-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,13 +27,13 @@
     package_dir={"bpetokenizer": "bpetokenizer"},
     packages=find_packages(where="bpetokenizer"),
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-    install_requires=[],
+    install_requires=["regex"],
     extras_require={
         "dev": ["pytest", "twine"],
     },
     python_requires=">=3.9,<3.13",
 )
```

### Comparing `bpetokenizer-1.0.0/tests/test_tokenizer.py` & `bpetokenizer-1.0.1/tests/test_tokenizer.py`

 * *Files identical despite different names*

