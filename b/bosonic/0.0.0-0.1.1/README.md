# Comparing `tmp/bosonic-0.0.0.tar.gz` & `tmp/bosonic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosonic-0.0.0.tar", last modified: Tue Feb 20 21:15:12 2024, max compression
+gzip compressed data, was "bosonic-0.1.1.tar", last modified: Mon May 27 05:02:45 2024, max compression
```

## Comparing `bosonic-0.0.0.tar` & `bosonic-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,39 @@
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-02-20 21:15:12.158243 bosonic-0.0.0/
--rw-r--r--   0 phionx     (501) staff       (20)       45 2024-02-20 21:14:55.000000 bosonic-0.0.0/MANIFEST.in
--rw-r--r--   0 phionx     (501) staff       (20)      899 2024-02-20 21:15:12.158048 bosonic-0.0.0/PKG-INFO
--rw-r--r--   0 phionx     (501) staff       (20)       28 2024-02-20 21:14:51.000000 bosonic-0.0.0/README.md
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-02-20 21:15:12.157213 bosonic-0.0.0/bosonic/
--rw-r--r--   0 phionx     (501) staff       (20)        5 2024-02-20 21:14:04.000000 bosonic-0.0.0/bosonic/VERSION.txt
--rw-r--r--   0 phionx     (501) staff       (20)      253 2024-02-20 21:14:04.000000 bosonic-0.0.0/bosonic/__init__.py
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-02-20 21:15:12.157852 bosonic-0.0.0/bosonic.egg-info/
--rw-r--r--   0 phionx     (501) staff       (20)      899 2024-02-20 21:15:12.000000 bosonic-0.0.0/bosonic.egg-info/PKG-INFO
--rw-r--r--   0 phionx     (501) staff       (20)      194 2024-02-20 21:15:12.000000 bosonic-0.0.0/bosonic.egg-info/SOURCES.txt
--rw-r--r--   0 phionx     (501) staff       (20)        1 2024-02-20 21:15:12.000000 bosonic-0.0.0/bosonic.egg-info/dependency_links.txt
--rw-r--r--   0 phionx     (501) staff       (20)        8 2024-02-20 21:15:12.000000 bosonic-0.0.0/bosonic.egg-info/top_level.txt
--rw-r--r--   0 phionx     (501) staff       (20)       38 2024-02-20 21:15:12.158286 bosonic-0.0.0/setup.cfg
--rw-r--r--   0 phionx     (501) staff       (20)     1706 2024-02-20 21:14:46.000000 bosonic-0.0.0/setup.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:02:45.092842 bosonic-0.1.1/
+-rw-r--r--   0 phionx     (501) staff       (20)    11357 2024-03-04 08:27:52.000000 bosonic-0.1.1/LICENSE
+-rw-r--r--   0 phionx     (501) staff       (20)       77 2024-05-27 03:50:07.000000 bosonic-0.1.1/MANIFEST.in
+-rw-r--r--   0 phionx     (501) staff       (20)     5839 2024-05-27 05:02:45.092609 bosonic-0.1.1/PKG-INFO
+-rw-r--r--   0 phionx     (501) staff       (20)     3964 2024-05-27 04:58:15.000000 bosonic-0.1.1/README.md
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:02:45.087371 bosonic-0.1.1/bosonic/
+-rw-r--r--   0 phionx     (501) staff       (20)        5 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/VERSION.txt
+-rw-r--r--   0 phionx     (501) staff       (20)      323 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/__init__.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:02:45.088302 bosonic-0.1.1/bosonic/circuit/
+-rw-r--r--   0 phionx     (501) staff       (20)       84 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/circuit/__init__.py
+-rw-r--r--   0 phionx     (501) staff       (20)    10975 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/circuit/base.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:02:45.089220 bosonic-0.1.1/bosonic/circuit/gates/
+-rw-r--r--   0 phionx     (501) staff       (20)       86 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/circuit/gates/__init__.py
+-rw-r--r--   0 phionx     (501) staff       (20)     1360 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/circuit/gates/cavity.py
+-rw-r--r--   0 phionx     (501) staff       (20)     3095 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/circuit/gates/cavity_qubit.py
+-rw-r--r--   0 phionx     (501) staff       (20)      547 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/circuit/gates/qubit.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:02:45.090553 bosonic-0.1.1/bosonic/codes/
+-rw-r--r--   0 phionx     (501) staff       (20)      259 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/codes/__init__.py
+-rw-r--r--   0 phionx     (501) staff       (20)     7775 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/codes/base.py
+-rw-r--r--   0 phionx     (501) staff       (20)     1564 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/codes/binomial.py
+-rw-r--r--   0 phionx     (501) staff       (20)      963 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/codes/cat.py
+-rw-r--r--   0 phionx     (501) staff       (20)     5940 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/codes/gkp.py
+-rw-r--r--   0 phionx     (501) staff       (20)      624 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/codes/mode.py
+-rw-r--r--   0 phionx     (501) staff       (20)     1333 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/codes/qubit.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:02:45.090919 bosonic-0.1.1/bosonic/simulator/
+-rw-r--r--   0 phionx     (501) staff       (20)       45 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/simulator/__init__.py
+-rw-r--r--   0 phionx     (501) staff       (20)     7445 2024-05-27 03:50:07.000000 bosonic-0.1.1/bosonic/simulator/base.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:02:45.091653 bosonic-0.1.1/bosonic.egg-info/
+-rw-r--r--   0 phionx     (501) staff       (20)     5839 2024-05-27 05:02:45.000000 bosonic-0.1.1/bosonic.egg-info/PKG-INFO
+-rw-r--r--   0 phionx     (501) staff       (20)      682 2024-05-27 05:02:45.000000 bosonic-0.1.1/bosonic.egg-info/SOURCES.txt
+-rw-r--r--   0 phionx     (501) staff       (20)        1 2024-05-27 05:02:45.000000 bosonic-0.1.1/bosonic.egg-info/dependency_links.txt
+-rw-r--r--   0 phionx     (501) staff       (20)      211 2024-05-27 05:02:45.000000 bosonic-0.1.1/bosonic.egg-info/requires.txt
+-rw-r--r--   0 phionx     (501) staff       (20)       18 2024-05-27 05:02:45.000000 bosonic-0.1.1/bosonic.egg-info/top_level.txt
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:02:45.091108 bosonic-0.1.1/docs/
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 05:02:45.091261 bosonic-0.1.1/docs/assets/
+-rw-r--r--   0 phionx     (501) staff       (20)    16490 2024-03-04 07:56:20.000000 bosonic-0.1.1/docs/assets/logo_sq.png
+-rw-r--r--   0 phionx     (501) staff       (20)      940 2024-05-27 03:50:07.000000 bosonic-0.1.1/docs/gen_ref_pages.py
+-rw-r--r--   0 phionx     (501) staff       (20)       38 2024-05-27 05:02:45.092881 bosonic-0.1.1/setup.cfg
+-rw-r--r--   0 phionx     (501) staff       (20)     2387 2024-05-27 03:50:07.000000 bosonic-0.1.1/setup.py
```

### Comparing `bosonic-0.0.0/setup.py` & `bosonic-0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,83 @@
 """
-Setup
+Setup for bosonic
 """
 import os
 
 from setuptools import setup, find_namespace_packages
 
-
-DIST_NAME = "bosonic"
-PACKAGE_NAME = "bosonic"
-
-REQUIREMENTS = []
+REQUIREMENTS = [
+    "numpy",
+    "scipy",
+    "matplotlib",
+    "qutip",
+    "tqdm",
+    "cython>=0.29.20",
+    "jax[cpu]",
+]
 
 EXTRA_REQUIREMENTS = {
+   "dev": [
+        "jupyterlab>=3.1.0",
+        "mypy",
+        "pylint",
+        "black"
+    ],
+    "docs": [
+        "mkdocs",
+        "mkdocs-material",
+        "mkdocs-literate-nav",
+        "mkdocs-section-index",
+        "mkdocs-gen-files",
+        "mkdocstrings-python",
+    ]
 }
 
 # Read long description from README.
 README_PATH = os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")
 with open(README_PATH) as readme_file:
     README = readme_file.read()
 
 version_path = os.path.abspath(
-    os.path.join(os.path.dirname(__file__), PACKAGE_NAME, "VERSION.txt")
+    os.path.join(os.path.dirname(__file__), "bosonic", "VERSION.txt")
 )
 
 with open(version_path, "r") as fd:
     version_str = fd.read().rstrip()
 
-
 setup(
-    name=DIST_NAME,
+    name="bosonic",
     version=version_str,
-    description=DIST_NAME,
+    description="Bosonic JAX",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/EQuS/bosonic",
-    author="Shantanu Jha, Shoumik Chowdhury",
+    author="Shantanu Jha, Shoumik Chowdhury, Max Hays",
     author_email="shantanu.rajesh.jha@gmail.com",
+    license="Apache 2.0",
     packages=find_namespace_packages(exclude=["tutorials*"]),
     install_requires=REQUIREMENTS,
     extras_require=EXTRA_REQUIREMENTS,
     classifiers=[
         "Environment :: Console",
+        "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: Microsoft :: Windows",
-        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: MacOS",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Topic :: Scientific/Engineering",
     ],
-    keywords="quantum computing circuits",
+    keywords="bosonic jax qubits cQED QEC GKP quantum error correction",
     python_requires=">=3.7",
     project_urls={
-        "Documentation": "https://github.com/EQuS/bosonic",
+        "Bug Tracker": "https://github.com/EQuS/bosonic/issues",
+        "Documentation": "https://equs.github.io/bosonic",
         "Source Code": "https://github.com/EQuS/bosonic",
-        "Tutorials": "https://github.com/EQuS/bosonic/tree/master/tutorials",
+        "Tutorials": "https://github.com/EQuS/bosonic/tutorials",
+        "Tests": "https://github.com/EQuS/bosonic/test",
     },
     include_package_data=True,
 )
```

