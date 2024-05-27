# Comparing `tmp/turboconf-0.2.1.tar.gz` & `tmp/turboconf-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turboconf-0.2.1.tar", last modified: Sun May 26 14:02:22 2024, max compression
+gzip compressed data, was "turboconf-0.3.1.tar", last modified: Mon May 27 16:46:47 2024, max compression
```

## Comparing `turboconf-0.2.1.tar` & `turboconf-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-26 14:02:22.492735 turboconf-0.2.1/
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-05-25 21:39:05.000000 turboconf-0.2.1/LICENSE
--rw-r--r--   0 robertdegen   (501) staff       (20)      477 2024-05-26 14:02:22.492552 turboconf-0.2.1/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-05-25 21:39:05.000000 turboconf-0.2.1/README.md
--rw-r--r--   0 robertdegen   (501) staff       (20)      562 2024-05-26 14:02:20.000000 turboconf-0.2.1/pyproject.toml
--rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-05-26 14:02:22.492773 turboconf-0.2.1/setup.cfg
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-26 14:02:22.490798 turboconf-0.2.1/src/
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-26 14:02:22.491774 turboconf-0.2.1/src/turboconf/
--rw-r--r--   0 robertdegen   (501) staff       (20)      376 2024-05-25 21:41:47.000000 turboconf-0.2.1/src/turboconf/__init__.py
--rw-r--r--   0 robertdegen   (501) staff       (20)        0 2024-05-25 21:41:47.000000 turboconf-0.2.1/src/turboconf/__main__.py
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-26 14:02:22.492381 turboconf-0.2.1/src/turboconf.egg-info/
--rw-r--r--   0 robertdegen   (501) staff       (20)      477 2024-05-26 14:02:22.000000 turboconf-0.2.1/src/turboconf.egg-info/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      232 2024-05-26 14:02:22.000000 turboconf-0.2.1/src/turboconf.egg-info/SOURCES.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-05-26 14:02:22.000000 turboconf-0.2.1/src/turboconf.egg-info/dependency_links.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)       10 2024-05-26 14:02:22.000000 turboconf-0.2.1/src/turboconf.egg-info/top_level.txt
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-27 16:46:47.887395 turboconf-0.3.1/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-05-25 21:39:05.000000 turboconf-0.3.1/LICENSE
+-rw-r--r--   0 robertdegen   (501) staff       (20)      477 2024-05-27 16:46:47.887215 turboconf-0.3.1/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-05-25 21:39:05.000000 turboconf-0.3.1/README.md
+-rw-r--r--   0 robertdegen   (501) staff       (20)      562 2024-05-27 16:46:45.000000 turboconf-0.3.1/pyproject.toml
+-rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-05-27 16:46:47.887434 turboconf-0.3.1/setup.cfg
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-27 16:46:47.884319 turboconf-0.3.1/src/
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-27 16:46:47.886287 turboconf-0.3.1/src/turboconf/
+-rw-r--r--   0 robertdegen   (501) staff       (20)      560 2024-05-27 16:45:04.000000 turboconf-0.3.1/src/turboconf/__init__.py
+-rw-r--r--   0 robertdegen   (501) staff       (20)       45 2024-05-27 16:45:13.000000 turboconf-0.3.1/src/turboconf/__main__.py
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-05-27 16:46:47.887047 turboconf-0.3.1/src/turboconf.egg-info/
+-rw-r--r--   0 robertdegen   (501) staff       (20)      477 2024-05-27 16:46:47.000000 turboconf-0.3.1/src/turboconf.egg-info/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      232 2024-05-27 16:46:47.000000 turboconf-0.3.1/src/turboconf.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-05-27 16:46:47.000000 turboconf-0.3.1/src/turboconf.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       10 2024-05-27 16:46:47.000000 turboconf-0.3.1/src/turboconf.egg-info/top_level.txt
```

### Comparing `turboconf-0.2.1/pyproject.toml` & `turboconf-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "turboconf"
-version = "0.2.1"
+version = "0.3.1"
 authors = [
   { name="Robert Degen", email="turbodev@mailbox.org" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

