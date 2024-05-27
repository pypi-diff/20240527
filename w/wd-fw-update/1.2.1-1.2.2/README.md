# Comparing `tmp/wd_fw_update-1.2.1.tar.gz` & `tmp/wd_fw_update-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wd_fw_update-1.2.1.tar", last modified: Tue Apr 23 11:53:20 2024, max compression
+gzip compressed data, was "wd_fw_update-1.2.2.tar", last modified: Mon May 27 08:57:51 2024, max compression
```

## Comparing `wd_fw_update-1.2.1.tar` & `wd_fw_update-1.2.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:53:20.311230 wd_fw_update-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:53:20.303230 wd_fw_update-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:53:20.307230 wd_fw_update-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-23 11:53:20.311230 wd_fw_update-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:53:20.307230 wd_fw_update-1.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:53:20.307230 wd_fw_update-1.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     9999 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)   138313 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/gif.gif
--rw-r--r--   0 runner    (1001) docker     (127)   200575 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-23 11:53:20.311230 wd_fw_update-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:53:20.303230 wd_fw_update-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:53:20.307230 wd_fw_update-1.2.1/src/wd_fw_update/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/src/wd_fw_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16395 2024-04-23 11:53:15.000000 wd_fw_update-1.2.1/src/wd_fw_update/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:53:20.311230 wd_fw_update-1.2.1/src/wd_fw_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-23 11:53:20.000000 wd_fw_update-1.2.1/src/wd_fw_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-23 11:53:20.000000 wd_fw_update-1.2.1/src/wd_fw_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:53:20.000000 wd_fw_update-1.2.1/src/wd_fw_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 11:53:20.000000 wd_fw_update-1.2.1/src/wd_fw_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:53:20.000000 wd_fw_update-1.2.1/src/wd_fw_update.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 11:53:20.000000 wd_fw_update-1.2.1/src/wd_fw_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 11:53:20.000000 wd_fw_update-1.2.1/src/wd_fw_update.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:57:51.650578 wd_fw_update-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:57:51.642578 wd_fw_update-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:57:51.646578 wd_fw_update-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-27 08:57:51.650578 wd_fw_update-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:57:51.646578 wd_fw_update-1.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:57:51.646578 wd_fw_update-1.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9999 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   138313 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/gif.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   200575 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-27 08:57:51.650578 wd_fw_update-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:57:51.642578 wd_fw_update-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:57:51.646578 wd_fw_update-1.2.2/src/wd_fw_update/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/src/wd_fw_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-05-27 08:57:44.000000 wd_fw_update-1.2.2/src/wd_fw_update/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:57:51.650578 wd_fw_update-1.2.2/src/wd_fw_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-27 08:57:51.000000 wd_fw_update-1.2.2/src/wd_fw_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-27 08:57:51.000000 wd_fw_update-1.2.2/src/wd_fw_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:57:51.000000 wd_fw_update-1.2.2/src/wd_fw_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-27 08:57:51.000000 wd_fw_update-1.2.2/src/wd_fw_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:57:51.000000 wd_fw_update-1.2.2/src/wd_fw_update.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-27 08:57:51.000000 wd_fw_update-1.2.2/src/wd_fw_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 08:57:51.000000 wd_fw_update-1.2.2/src/wd_fw_update.egg-info/top_level.txt
```

### Comparing `wd_fw_update-1.2.1/.coveragerc` & `wd_fw_update-1.2.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/.github/workflows/python-publish.yml` & `wd_fw_update-1.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/.gitignore` & `wd_fw_update-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/.pre-commit-config.yaml` & `wd_fw_update-1.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/.readthedocs.yml` & `wd_fw_update-1.2.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/CHANGELOG.md` & `wd_fw_update-1.2.2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 # Changelog
+## Version 1.2.2
+- Fix download url.
+- Add http status code test.
+
+**Full Changelog**: [v1.2.1...v1.2.2](https://github.com/not-a-feature/wd_fw_update/compare/v1.2.1...v1.2.2)
+
 ## Version 1.2.1
 - Remove debug value
-**Full Changelog**: [v1.1.1...v1.2.0](https://github.com/not-a-feature/wd_fw_update/compare/v1.2.0...v1.2.1)
+
+**Full Changelog**: [v1.1.1...v1.2.1](https://github.com/not-a-feature/wd_fw_update/compare/v1.2.0...v1.2.1)
 
 ## Version 1.2.0
 - Perform version dependency check earlier s.t. it fails early.
 - Improved error messages.
 - Improved docstrings.
+
 **Full Changelog**: [v1.1.1...v1.2.0](https://github.com/not-a-feature/wd_fw_update/compare/v1.1.1...v1.2.0)
 
 ## Version 1.1.1
 - Improve nvme slot detection.
 - Improve Readme and Output.
 **Full Changelog**: [v1.1.0...v1.1.1](https://github.com/not-a-feature/wd_fw_update/compare/v1.1.0...v1.1.1)
 
 ## Version 1.1.0
 - Improve nvme slot detection.
 - Remove python 3.12 exclusive feature.
 - Fix whitespace issue in logo.
-- **Full Changelog**: [v1.0.1...v1.1.0](https://github.com/not-a-feature/wd_fw_update/compare/v1.0.1...v1.1.0)
+
+**Full Changelog**: [v1.0.1...v1.1.0](https://github.com/not-a-feature/wd_fw_update/compare/v1.0.1...v1.1.0)
 
 ## Version 1.0.1
 - Add message and improve docs.
-- **Full Changelog**: [v1.0.0...v1.0.1](https://github.com/not-a-feature/wd_fw_update/compare/v1.0.0...v1.0.1)
+
+**Full Changelog**: [v1.0.0...v1.0.1](https://github.com/not-a-feature/wd_fw_update/compare/v1.0.0...v1.0.1)
 
 ## Version 1.0.0 (initial release)
 
 - Initial release
```

### Comparing `wd_fw_update-1.2.1/CONTRIBUTING.md` & `wd_fw_update-1.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/LICENSE` & `wd_fw_update-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/PKG-INFO` & `wd_fw_update-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wd_fw_update
-Version: 1.2.1
+Version: 1.2.2
 Summary: Updates the firmware of Western Digital SSDs on Ubuntu / Linux Mint.
 Home-page: https://github.com/not-a-feature/wd_fw_update
 Author: Jules Kreuer
 Author-email: contact@juleskreuer.eu
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/not-a-feature/wd_fw_update
 Project-URL: Source, https://github.com/not-a-feature/wd_fw_update
@@ -34,15 +34,15 @@
 
 It provides a user-friendly interface to select the firmware version for the update process.
 
 It uses the Western Digital API and the NVME toolbox `nvme-cli` but is NOT associated in any case to them.
 
 It was originally developed for Frame.Work laptops, but should work with any Ubuntu / Mint device with Western Digital NVME SSD.
 
-See the discussion on: [community.frame.work](https://community.frame.work/t/western-digital-drive-update-guide-without-windows-wd-dashboard/20616)
+See the discussion on: [community.frame.work](https://community.frame.work/t/western-digital-drive-update-guide-without-windows-wd-dashboard/20616) and [juleskreuer.eu](https://juleskreuer.eu/western-digital-firmware-update/)
 
 <img alt="GIF" src=https://github.com/not-a-feature/wd_fw_update/raw/main/gif.gif height=250>
 
 ## Installation
 ### Prerequisites
 
 Make sure the following dependencies are installed on your system:
```

### Comparing `wd_fw_update-1.2.1/README.md` & `wd_fw_update-1.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 It provides a user-friendly interface to select the firmware version for the update process.
 
 It uses the Western Digital API and the NVME toolbox `nvme-cli` but is NOT associated in any case to them.
 
 It was originally developed for Frame.Work laptops, but should work with any Ubuntu / Mint device with Western Digital NVME SSD.
 
-See the discussion on: [community.frame.work](https://community.frame.work/t/western-digital-drive-update-guide-without-windows-wd-dashboard/20616)
+See the discussion on: [community.frame.work](https://community.frame.work/t/western-digital-drive-update-guide-without-windows-wd-dashboard/20616) and [juleskreuer.eu](https://juleskreuer.eu/western-digital-firmware-update/)
 
 <img alt="GIF" src=https://github.com/not-a-feature/wd_fw_update/raw/main/gif.gif height=250>
 
 ## Installation
 ### Prerequisites
 
 Make sure the following dependencies are installed on your system:
```

### Comparing `wd_fw_update-1.2.1/docs/Makefile` & `wd_fw_update-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/docs/conf.py` & `wd_fw_update-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/docs/index.md` & `wd_fw_update-1.2.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/gif.gif` & `wd_fw_update-1.2.2/gif.gif`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/logo.png` & `wd_fw_update-1.2.2/logo.png`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/setup.cfg` & `wd_fw_update-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/setup.py` & `wd_fw_update-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/src/wd_fw_update/__init__.py` & `wd_fw_update-1.2.2/src/wd_fw_update/__init__.py`

 * *Files identical despite different names*

### Comparing `wd_fw_update-1.2.1/src/wd_fw_update/main.py` & `wd_fw_update-1.2.2/src/wd_fw_update/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,16 @@
 
     slots = [s[3:] for s in sorted(result[2:10]) if s]
     _logger.debug(f"Firmware slots: {slots}")
 
     if len(slots) == 1:
         _logger.info("Only one slot to select, skipping user-promt.")
 
-        return int(slots[0].split(":")[0])  # Should always be 1
+        slot = int(slots[0].split(":")[0])  # Should always be 1
+        return current_slot, slot
 
     print("Select the slot to which the firmware should be installed.")
     questions = [
         inquirer.List(
             "slot",
             message="Slot ID: Current Firmware Version",
             choices=slots,
@@ -313,15 +314,16 @@
         current_fw_version (str): Current firmware version.
 
     Returns:
         firmware_url (srr): URL to new firmware file.
     """
 
     model = model.replace(" ", "_")
-    prop_url = f"{BASE_WD_DOMAIN}/firmware/{model}/{version}/device_properties.xml"
+    base_url = f"{BASE_WD_DOMAIN}/firmware/{model}/{version}"
+    prop_url = f"{base_url}/device_properties.xml"
 
     _logger.debug(f"Firmware properties url: {prop_url}")
 
     response = requests.get(prop_url)
     response.raise_for_status()
 
     root = ET.fromstring(response.content)
@@ -332,15 +334,15 @@
     # Check if current firmware is in dependencies
     if current_fw_version not in dependencies_list:
         print(f"The current firmware version {current_fw_version} is not in the dependency")
         print(f"list of the new firmware. In order to upgrade to {version}, please")
         print(f"upgrade to one of these versions first: {dependencies_list}")
         exit(1)
 
-    firmware_url = f"{prop_url}{root.findtext('fwfile')}"
+    firmware_url = f"{base_url}/{root.findtext('fwfile')}"
 
     _logger.debug(f"Firmware file url: {firmware_url}\n")
     return firmware_url
 
 
 def update_fw(
     current_fw_version: str,
@@ -383,14 +385,19 @@
         unit_scale=True,
         unit_divisor=1024,
     ) as pbar:
         for data in r.iter_content(1024):
             pbar.update(len(data))
             fw_file.write(data)
 
+        _logger.info(f"HTTP Status Code: {r.status_code}")
+        if not r.status_code == 200:
+            print("Error downloading the firmware file.")
+            exit(1)
+
         print()
         print("========== Summary ==========")
         print(f"NVME location:     {device}")
         print(f"Model:             {model}")
         print(f"Firmware Version:  {current_fw_version} --> {version}")
         print(f"Installation Slot: {slot}")
         print(f"Active Slot:       {current_slot} --> {slot}")
```

### Comparing `wd_fw_update-1.2.1/src/wd_fw_update.egg-info/PKG-INFO` & `wd_fw_update-1.2.2/src/wd_fw_update.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wd_fw_update
-Version: 1.2.1
+Version: 1.2.2
 Summary: Updates the firmware of Western Digital SSDs on Ubuntu / Linux Mint.
 Home-page: https://github.com/not-a-feature/wd_fw_update
 Author: Jules Kreuer
 Author-email: contact@juleskreuer.eu
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/not-a-feature/wd_fw_update
 Project-URL: Source, https://github.com/not-a-feature/wd_fw_update
@@ -34,15 +34,15 @@
 
 It provides a user-friendly interface to select the firmware version for the update process.
 
 It uses the Western Digital API and the NVME toolbox `nvme-cli` but is NOT associated in any case to them.
 
 It was originally developed for Frame.Work laptops, but should work with any Ubuntu / Mint device with Western Digital NVME SSD.
 
-See the discussion on: [community.frame.work](https://community.frame.work/t/western-digital-drive-update-guide-without-windows-wd-dashboard/20616)
+See the discussion on: [community.frame.work](https://community.frame.work/t/western-digital-drive-update-guide-without-windows-wd-dashboard/20616) and [juleskreuer.eu](https://juleskreuer.eu/western-digital-firmware-update/)
 
 <img alt="GIF" src=https://github.com/not-a-feature/wd_fw_update/raw/main/gif.gif height=250>
 
 ## Installation
 ### Prerequisites
 
 Make sure the following dependencies are installed on your system:
```

### Comparing `wd_fw_update-1.2.1/src/wd_fw_update.egg-info/SOURCES.txt` & `wd_fw_update-1.2.2/src/wd_fw_update.egg-info/SOURCES.txt`

 * *Files identical despite different names*

