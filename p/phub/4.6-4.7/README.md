# Comparing `tmp/phub-4.6.tar.gz` & `tmp/phub-4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phub-4.6.tar", last modified: Thu Apr 11 17:33:43 2024, max compression
+gzip compressed data, was "phub-4.7.tar", last modified: Mon May 27 17:30:50 2024, max compression
```

## Comparing `phub-4.6.tar` & `phub-4.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:43.902743 phub-4.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 17:33:39.000000 phub-4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41938 2024-04-11 17:33:43.902743 phub-4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-11 17:33:39.000000 phub-4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-11 17:33:39.000000 phub-4.6/pypi.md
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-11 17:33:39.000000 phub-4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:33:43.902743 phub-4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 17:33:39.000000 phub-4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:43.894743 phub-4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:43.898743 phub-4.6/src/phub/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-11 17:33:39.000000 phub-4.6/src/phub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-11 17:33:39.000000 phub-4.6/src/phub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-04-11 17:33:39.000000 phub-4.6/src/phub/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16579 2024-04-11 17:33:39.000000 phub-4.6/src/phub/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-11 17:33:39.000000 phub-4.6/src/phub/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-04-11 17:33:39.000000 phub-4.6/src/phub/literals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:43.898743 phub-4.6/src/phub/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-11 17:33:39.000000 phub-4.6/src/phub/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-11 17:33:39.000000 phub-4.6/src/phub/modules/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-11 17:33:39.000000 phub-4.6/src/phub/modules/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-11 17:33:39.000000 phub-4.6/src/phub/modules/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-11 17:33:39.000000 phub-4.6/src/phub/modules/rss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:43.898743 phub-4.6/src/phub/objects/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/feed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    18719 2024-04-11 17:33:39.000000 phub-4.6/src/phub/objects/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:43.902743 phub-4.6/src/phub/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:39.000000 phub-4.6/src/phub/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-11 17:33:39.000000 phub-4.6/src/phub/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-11 17:33:39.000000 phub-4.6/src/phub/tests/test_playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-11 17:33:39.000000 phub-4.6/src/phub/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-11 17:33:39.000000 phub-4.6/src/phub/tests/test_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-11 17:33:39.000000 phub-4.6/src/phub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:33:43.902743 phub-4.6/src/phub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41938 2024-04-11 17:33:43.000000 phub-4.6/src/phub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-11 17:33:43.000000 phub-4.6/src/phub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:33:43.000000 phub-4.6/src/phub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 17:33:43.000000 phub-4.6/src/phub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 17:33:43.000000 phub-4.6/src/phub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:50.240161 phub-4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 17:30:42.000000 phub-4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    41663 2024-05-27 17:30:50.240161 phub-4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-27 17:30:42.000000 phub-4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-27 17:30:42.000000 phub-4.7/pypi.md
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-27 17:30:42.000000 phub-4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 17:30:50.240161 phub-4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 17:30:42.000000 phub-4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:50.232161 phub-4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:50.236161 phub-4.7/src/phub/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-27 17:30:42.000000 phub-4.7/src/phub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-27 17:30:42.000000 phub-4.7/src/phub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-05-27 17:30:42.000000 phub-4.7/src/phub/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16646 2024-05-27 17:30:42.000000 phub-4.7/src/phub/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-27 17:30:42.000000 phub-4.7/src/phub/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-05-27 17:30:42.000000 phub-4.7/src/phub/literals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:50.236161 phub-4.7/src/phub/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-27 17:30:42.000000 phub-4.7/src/phub/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-27 17:30:42.000000 phub-4.7/src/phub/modules/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-27 17:30:42.000000 phub-4.7/src/phub/modules/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-27 17:30:42.000000 phub-4.7/src/phub/modules/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-27 17:30:42.000000 phub-4.7/src/phub/modules/rss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:50.240161 phub-4.7/src/phub/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-27 17:30:42.000000 phub-4.7/src/phub/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-27 17:30:42.000000 phub-4.7/src/phub/objects/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-05-27 17:30:42.000000 phub-4.7/src/phub/objects/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-27 17:30:42.000000 phub-4.7/src/phub/objects/feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-27 17:30:42.000000 phub-4.7/src/phub/objects/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-27 17:30:42.000000 phub-4.7/src/phub/objects/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-27 17:30:42.000000 phub-4.7/src/phub/objects/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-27 17:30:42.000000 phub-4.7/src/phub/objects/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18672 2024-05-27 17:30:42.000000 phub-4.7/src/phub/objects/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:50.240161 phub-4.7/src/phub/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:42.000000 phub-4.7/src/phub/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-27 17:30:42.000000 phub-4.7/src/phub/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-27 17:30:42.000000 phub-4.7/src/phub/tests/test_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-27 17:30:42.000000 phub-4.7/src/phub/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-27 17:30:42.000000 phub-4.7/src/phub/tests/test_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-27 17:30:42.000000 phub-4.7/src/phub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:50.240161 phub-4.7/src/phub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41663 2024-05-27 17:30:50.000000 phub-4.7/src/phub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-27 17:30:50.000000 phub-4.7/src/phub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 17:30:50.000000 phub-4.7/src/phub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 17:30:50.000000 phub-4.7/src/phub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 17:30:50.000000 phub-4.7/src/phub.egg-info/top_level.txt
```

### Comparing `phub-4.6/LICENSE` & `phub-4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `phub-4.6/PKG-INFO` & `phub-4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 4.6
+Version: 4.7
 Summary: An API for Pornhub
-Author-email: Egsagon <egsagon12@gmail.com>, EchterAlsFake <EchterAlsFake@proton.me>
+Author-email: Egsagon <egsagon.git@gmail.com>, EchterAlsFake <EchterAlsFake@proton.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -679,45 +679,26 @@
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Documentation, https://phub.readthedocs.io
 Project-URL: Repository, https://github.com/EchterAlsFake/PHUB
 Keywords: pornhub,phub,porn,api,web scrapper,api wrapper
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: ffmpeg-progress-yield
 Provides-Extra: cli
 Requires-Dist: click; extra == "cli"
 
 <p align="center">
-  <img width="300" src="https://raw.githubusercontent.com/Egsagon/PHUB/master/assets/logo.svg">
+  <img width="200" src="https://raw.githubusercontent.com/Egsagon/PHUB/master/assets/logo.svg">
 </p>
 
 # PHUB - An API wrapper for PornHub.
 
-PHUB is a hybrid API for Pornhub. It is able to communicate with Pornhub
-using both web-scraping and Pornhub's HubTraffic API. It is
-able to access most used or useful PH features, such as video searching,
-accessing account features, video downloading, and a lot more.
+PHUB is an easy-to-use API wrapper for Pornhub. It can access most used or useful
+PH features, such as video searching, account features, video downloading, and more.
 
-Learn more on the project [documentation](https://phub.readthedocs.io) and
-[GitHub page](https://github.com/EchterAlsFake/PHUB).
-
-## Installation
-
-```sh
-pip install --upgrade phub
-```
-
-## Quickstart
-
-```python
-import phub
-
-client = phub.Client()
-
-video = client.get(url = '...')
-video.download('my-video.mp4', quality = 'best')
-```
+- Project documentation: [phub.readthedocs.io](https://phub.readthedocs.io)
+- Project repository: [EchterAlsFake/PHUB](https://github.com/EchterAlsFake/PHUB)
```

### Comparing `phub-4.6/README.md` & `phub-4.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,45 @@
 <p align="center">
-  <img width="300" src="https://github.com/Egsagon/PHUB/blob/master/assets/logo.svg">
+  <img width="200" src="https://github.com/Egsagon/PHUB/blob/master/assets/logo.svg">
 </p>
 
 <div align="center">
     <a href="https://pepy.tech/project/phub"><img src="https://static.pepy.tech/badge/phub" alt="Downloads"></a>
     <a href="https://badge.fury.io/py/phub"><img src="https://badge.fury.io/py/phub.svg" alt="PyPI version" height="18"></a>
     <a href="https://github.com/EchterAlsFake/PHUB/workflows/"><img src="https://github.com/EchterAlsFake/PHUB/actions/workflows/tests.yml/badge.svg" alt="API Tests"/></a>
 </div>
 
 <br>
-<br>
-PHUB is a hybrid API for Pornhub. It is able to communicate with Pornhub
-using both web-scraping and Pornhub's HubTraffic API. It is
-able to access most used or useful PH features, such as video searching,
-accessing account features, video downloading, and a lot more.
+PHUB is an easy-to-use API wrapper for Pornhub. It can access most used or useful
+PH features, such as video searching, account features, video downloading, and more.
 
 > [!WARNING]
 > This project is probably against Pornhub TOS. Use at your own risks.
 
-## Installation
+# Installation
 
-- Install using `pip` (python `3.11` or higher required, recommended version): 
+- Install using `pip` (python `3.9` or higher required): 
 ```shell
 pip install --upgrade phub
 ```
 
 - Or from this repo to get the latest fixes/features:
 ```shell
 pip install --upgrade git+https://github.com/EchterAlsFake/PHUB.git
 ```
 
-- Or, for python 3.10 and higher.
-```shell
-pip install --upgrade git+https://github.com/EchterAlsFake/PHUB.git@py-3.10
-```
-
-- Or, for even lower python versions, there is automatic branch with several features removed (might be unstable).
-```shell
-pip install --upgrade git+https://github.com/EchterAlsFake/PHUB.git@compat
-```
-
-## Usage from command line
+# Usage from command line
 ```shell
 # Download a single video
 py -m phub https://www.pornhub.com/view_video.php?viewkey=abcdef
 # Download multiple videos from a text file
 py -m phub path/to/file.txt --quality best --downloader threaded --output video.mp4
 ```
-###### Note: It does not matter how the URLs in the files are aranged, preferably one per line.
 
-## Quickstart
+# Quickstart
 
 > [!NOTE]
 > You can find the docs on this project [here](https://phub.readthedocs.io).
 
 ```python
 import phub
 from phub.locals import *
@@ -79,21 +65,19 @@
 
 # Access account history, liked and recommended stuff
 client.account.watched
 client.account.liked
 client.account.recommended
 ```
 
-# Note
-<strong>This repository was initiated and maintained by [Egsagon](https://github.com/Egsagon)
-He doesn't have any time to maintain this and transferred me the ownership.
-I'll do my best to maintain this repository functional.</strong>
-
-
-## License
+# License
 
 PHUB uses GPLv3. See the `LICENSE` file.
 
-## Contributing
+This repository was initiated and maintained by [Egsagon](https://github.com/Egsagon)
+He doesn't have any time to maintain this and transferred me the ownership.
+I'll do my best to maintain this repository functional.
+
+# Contributing
 
 Feel free to contribute to this project by submitting
 feature requests, issues, bugs, or whatever.
```

#### html2text {}

```diff
@@ -1,36 +1,27 @@
          [https://github.com/Egsagon/PHUB/blob/master/assets/logo.svg]
                      _[_D_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_A_P_I_ _T_e_s_t_s_]
 
-
-PHUB is a hybrid API for Pornhub. It is able to communicate with Pornhub using
-both web-scraping and Pornhub's HubTraffic API. It is able to access most used
-or useful PH features, such as video searching, accessing account features,
-video downloading, and a lot more. > [!WARNING] > This project is probably
-against Pornhub TOS. Use at your own risks. ## Installation - Install using
-`pip` (python `3.11` or higher required, recommended version): ```shell pip
-install --upgrade phub ``` - Or from this repo to get the latest fixes/
-features: ```shell pip install --upgrade git+https://github.com/EchterAlsFake/
-PHUB.git ``` - Or, for python 3.10 and higher. ```shell pip install --upgrade
-git+https://github.com/EchterAlsFake/PHUB.git@py-3.10 ``` - Or, for even lower
-python versions, there is automatic branch with several features removed (might
-be unstable). ```shell pip install --upgrade git+https://github.com/
-EchterAlsFake/PHUB.git@compat ``` ## Usage from command line ```shell #
-Download a single video py -m phub https://www.pornhub.com/
+PHUB is an easy-to-use API wrapper for Pornhub. It can access most used or
+useful PH features, such as video searching, account features, video
+downloading, and more. > [!WARNING] > This project is probably against Pornhub
+TOS. Use at your own risks. # Installation - Install using `pip` (python `3.9`
+or higher required): ```shell pip install --upgrade phub ``` - Or from this
+repo to get the latest fixes/features: ```shell pip install --upgrade
+git+https://github.com/EchterAlsFake/PHUB.git ``` # Usage from command line
+```shell # Download a single video py -m phub https://www.pornhub.com/
 view_video.php?viewkey=abcdef # Download multiple videos from a text file py -
 m phub path/to/file.txt --quality best --downloader threaded --output video.mp4
-``` ###### Note: It does not matter how the URLs in the files are aranged,
-preferably one per line. ## Quickstart > [!NOTE] > You can find the docs on
-this project [here](https://phub.readthedocs.io). ```python import phub from
-phub.locals import * # Initialise a client client = phub.Client() # Fetch and
-download a video video = client.get('https://...') video.download('my-
-video.mp4', Quality.BEST) # Fetch user videos user = client.get_user('this-
-user') for video in user.videos: print(video.title) # Perform a research for
-video in client.search('my-query'): print(video.title) # Connect to an account
-client = phub.Client('my-username', 'my-password') # Access account history,
-liked and recommended stuff client.account.watched client.account.liked
-client.account.recommended ``` # Note TThhiiss rreeppoossiittoorryy wwaass iinniittiiaatteedd aanndd
-mmaaiinnttaaiinneedd bbyy [[EEggssaaggoonn]]((hhttttppss::////ggiitthhuubb..ccoomm//EEggssaaggoonn)) HHee ddooeessnn''tt hhaavvee aannyy ttiimmee ttoo
-mmaaiinnttaaiinn tthhiiss aanndd ttrraannssffeerrrreedd mmee tthhee oowwnneerrsshhiipp.. II''llll ddoo mmyy bbeesstt ttoo mmaaiinnttaaiinn
-tthhiiss rreeppoossiittoorryy ffuunnccttiioonnaall.. ## License PHUB uses GPLv3. See the `LICENSE` file.
-## Contributing Feel free to contribute to this project by submitting feature
-requests, issues, bugs, or whatever.
+``` # Quickstart > [!NOTE] > You can find the docs on this project [here]
+(https://phub.readthedocs.io). ```python import phub from phub.locals import *
+# Initialise a client client = phub.Client() # Fetch and download a video video
+= client.get('https://...') video.download('my-video.mp4', Quality.BEST) #
+Fetch user videos user = client.get_user('this-user') for video in user.videos:
+print(video.title) # Perform a research for video in client.search('my-query'):
+print(video.title) # Connect to an account client = phub.Client('my-username',
+'my-password') # Access account history, liked and recommended stuff
+client.account.watched client.account.liked client.account.recommended ``` #
+License PHUB uses GPLv3. See the `LICENSE` file. This repository was initiated
+and maintained by [Egsagon](https://github.com/Egsagon) He doesn't have any
+time to maintain this and transferred me the ownership. I'll do my best to
+maintain this repository functional. # Contributing Feel free to contribute to
+this project by submitting feature requests, issues, bugs, or whatever.
```

### Comparing `phub-4.6/pyproject.toml` & `phub-4.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "phub"
-version = "4.6"
+version = "4.7"
 description = "An API for Pornhub"
 authors = [
-  {name = 'Egsagon', email = "egsagon12@gmail.com"},
+  {name = 'Egsagon', email = "egsagon.git@gmail.com"},
   {name = "EchterAlsFake", email = "EchterAlsFake@proton.me"}
 ]
 license = {file = "LICENSE"}
 readme = {file = "pypi.md", content-type = "text/markdown"}
 keywords = ["pornhub", "phub", "porn", "api", "web scrapper", "api wrapper"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
 dependencies = ["requests", "ffmpeg-progress-yield"]
-requires-python = ">=3.11"
+requires-python = ">=3.9"
 
 [project.optional-dependencies]
 cli = ["click"]
 
 [project.urls]
 Documentation = "https://phub.readthedocs.io"
 Repository = "https://github.com/EchterAlsFake/PHUB"
```

### Comparing `phub-4.6/src/phub/__init__.py` & `phub-4.7/src/phub/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 '''
-## PHUB v4.5.3
+## PHUB v4.7
 
 See https://phub.readthedocs.io/en/latest/ for docs.
 See https://github.com/EchterAlsFake/PHUB for code.
 '''
 
 # Package description
 __author__ = 'Egsagon, EchterAlsFake'
 __copyright__ = 'Copyright 2024, PHUB'
 __license__ = 'GPLv3'
-__version__  = '4.5.3'
+__version__  = '4.7'
 
 __all__ = ['Client', 'Quality', 'core', 'utils',
            'consts', 'errors', 'objects', 'modules']
 
 # Shortcuts
 from .core import Client
 from .utils import Quality
```

### Comparing `phub-4.6/src/phub/__main__.py` & `phub-4.7/src/phub/__main__.py`

 * *Files identical despite different names*

### Comparing `phub-4.6/src/phub/consts.py` & `phub-4.7/src/phub/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 PHUB constants.
 '''
 
 import logging
 import re as engine
 from re import Pattern as p
-from typing	import Callable
+from typing	import Callable, Union
 
 from . import errors
 
 logger = logging.getLogger(__name__)
 
 
 HOST = 'https://www.pornhub.com/'
@@ -59,15 +59,15 @@
     'stream_favourites_videos': 'Section.FAVORITE',
     'stream_grouped_comments_videos': 'Section.COMMENT',
     # TODO - More options
 }
 
 # Regex wrappers
 
-WrappedRegex = Callable[[str, bool | None], str | list[str]]
+WrappedRegex = Callable[[str, Union[bool, None]], Union[str, list[str]]]
 
 def _throw_re_error(pattern: str) -> None:
     '''
     Raises an error based on a pattern name.
     
     Args:
         pattern (str): The regex pattern.
```

### Comparing `phub-4.6/src/phub/core.py` & `phub-4.7/src/phub/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 PHUB core module.
 '''
 
 import time
 import logging
 
 import requests
-from typing import Iterable
+from typing import Iterable, Union
 from functools import cached_property
 
 from . import utils
 from . import consts
 from . import errors
 from . import literals
 
@@ -28,15 +28,15 @@
     '''
     
     def __init__(self,
                  email: str = None,
                  password: str = None,
                  *,
                  language: literals.language = 'en,en-US',
-                 delay: int | float = 0,
+                 delay: Union[int, float] = 0,
                  proxies: dict = None,
                  login: bool = True) -> None:
         '''
         Initialises a new client.
         
         Args:
             email (str): Account email address.
@@ -139,15 +139,16 @@
                 )
 
                 # Silent 429 errors
                 if b'429</title>' in response.content:
                     raise ConnectionError('Pornhub raised error 429: too many requests')
 
                 # Attempt to resolve the challenge if needed
-                if challenge := consts.re.get_challenge(response.text, False):
+                challenge = consts.re.get_challenge(response.text, False)
+                if challenge:
                     logger.info('Challenge found, attempting to resolve')
                     parser.challenge(self, *challenge)
                     
                     logger.info(f"Sleeping for {consts.CHALLENGE_TIMEOUT} seconds")
                     time.sleep(consts.CHALLENGE_TIMEOUT)
                     continue  # Reload page
 
@@ -210,15 +211,15 @@
         self._clear_granted_token()
         
         # Update account data
         self.account.connect(data)
         self.logged = bool(success)
         return self.logged
     
-    def get(self, video: str | Video) -> Video:
+    def get(self, video: Union[str, Video]) -> Video:
         '''
         Get a Pornhub video.
         
         Args:
             video (str | Video): Video URL or viewkey.
         
         Returns:
@@ -245,15 +246,15 @@
                 # Support key only
                 key = str(video)
             
             url = utils.concat(consts.HOST, 'view_video.php?viewkey=' + key)
         
         return Video(self, url)
 
-    def get_user(self, user: str | User) -> User:
+    def get_user(self, user: Union[str, User]) -> User:
         '''
         Get a Pornhub user.
         
         Args:
             user (str | User): user URL or name.
         
         Returns:
@@ -266,15 +267,15 @@
         logger.debug('Fetching user %s', user)
         return User.get(self, user)
 
     def search_hubtraffic(self,
                query: str,
                *,
                category: literals.category = None,
-               tags: str | list[str] = None,
+               tags: Union[str, list[str]] = None,
                sort: literals.ht_sort = None,
                period: literals.ht_period = None) -> Query:
         '''
         Perform searching on Pornhub using the HubTraffic API.
         It is condidered to be much faster but has less filters.
         
         Args:
@@ -308,15 +309,15 @@
         )
     
     def search(self,
                query: str,
                *,
                production: literals.production = None,
                category: literals.category = None,
-               exclude_category: literals.category | Iterable[literals.category] = None,
+               exclude_category: Union[literals.category, Iterable[literals.category]] = None,
                hd: bool = None,
                sort: literals.sort = None,
                period: literals.period = None) -> Query:
         '''
         Performs searching on Pornhub.
         
         Args:
@@ -357,29 +358,29 @@
                 'o': literals.map.sort.get(sort),
                 't': literals.map.period.get(period),
                 'hd': literals._craft_boolean(hd)
             },
             query_repr = query
         )
     
-    def get_playlist(self, playlist: str | int | Playlist) -> Playlist:
+    def get_playlist(self, playlist: Union[str, int, Playlist]) -> Playlist:
         '''
         Get a Pornhub playlist.
 
         Args:
             playlist (str | int | Playlist): The playlist url or id
 
         Returns:
             Playlist: The corresponding playlist object.
         
         Raises:
             TypeError: If the playlist argument is invalid.
         '''
         
-        if not isinstance(playlist, str | int | Playlist):
+        if not isinstance(playlist, (str, int, Playlist)):
             raise TypeError(f'Invalid type: {type(playlist)} should be str, int or Playlist.')
         
         if isinstance(playlist, Playlist):
             playlist = playlist.url
         
         if isinstance(playlist, str) and 'playlist' in playlist:
             playlist = playlist.split('/')[-1]
```

### Comparing `phub-4.6/src/phub/errors.py` & `phub-4.7/src/phub/errors.py`

 * *Files identical despite different names*

### Comparing `phub-4.6/src/phub/literals.py` & `phub-4.7/src/phub/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 PHUB Literals.
 '''
 
-from typing import Literal, Iterable, Type
+from typing import Literal, Iterable, Type, Union
 
 # Language locales
 language = Literal['en', 'cn', 'de', 'fr', 'it', 'pt', 'pl', 'rt', 'nl', 'cz', 'jp']
 
 # Production type
 production = Literal['homemade', 'professional']
 
@@ -195,29 +195,29 @@
     
     if isinstance(args, str):
         return args
     
     if args:
         return '-'.join(list(args))
 
-def _craft_boolean(b: bool | None) -> int | None:
+def _craft_boolean(b: Union[bool, None]) -> Union[int, None]:
     '''
     Craft a boolean into a url-valid int.
     
     Args:
         b (bool): Initial boolean value.
     
     Returns:
         int: URL-valid representation of b.
     '''
     
     if b is not None:
         return int(bool(b))
 
-def ass(name: str, item: str | list[str], literal: Type) -> None:
+def ass(name: str, item: Union[str, list[str]], literal: Type) -> None:
     '''
     Assert one or multiple items are part of a literal.
     
     Args:
         name (str): The literal name, used for error bodies.
         item (str | list[str]): The object(s) to assert.
         literal (Type): The literal that should match the item(s).
```

### Comparing `phub-4.6/src/phub/modules/display.py` & `phub-4.7/src/phub/modules/display.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 import time
-from typing import Callable
+from typing import Callable, Union
 
-def progress(color: dict  | None = dict(c1=30, c2=33, c3=34, c4=36), desc: str = 'Downloading') -> Callable:
+def progress(color: Union[dict, None] = dict(c1=30, c2=33, c3=34, c4=36), desc: str = 'Downloading') -> Callable:
     '''
     Simple progress display, with segment, percentage and speed display.
     
     Args:
         color (dict): ASCII progress colors.
         desc (str): Description to display.
```

### Comparing `phub-4.6/src/phub/modules/download.py` & `phub-4.7/src/phub/modules/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
 import time
 import logging
 import requests.adapters
 from pathlib import Path
-from typing import TYPE_CHECKING, Callable
-from concurrent.futures import ThreadPoolExecutor as Pool, as_completed
 from ffmpeg_progress_yield import FfmpegProgress
+from typing import TYPE_CHECKING, Callable, Union
+from concurrent.futures import ThreadPoolExecutor as Pool, as_completed
+
 from .. import consts
 
 if TYPE_CHECKING:
     from .. import Client
     from ..objects import Video
     from ..utils import Quality
 
 logger = logging.getLogger(__name__)
 
 CallbackType = Callable[[int, int], None]
 
 
-
 def default(video: Video,
             quality: Quality,
             callback: CallbackType,
             path: str,
             start: int = 0) -> None:
     '''
     Dummy downloader. Fetch a segment after the other.
@@ -68,15 +68,15 @@
     # Concatenate
     logger.info('Concatenating buffer to %s', path)
     with open(path, 'wb') as file:
         file.write(buffer)
     
     logger.info('Downloading successful.')
 
-def FFMPEG(video: Video, quality: Quality, callback: CallbackType, path: str | Path, start: int = 0) -> None:
+def FFMPEG(video: Video, quality: Quality, callback: CallbackType, path: Union[str, Path], start: int = 0) -> None:
     '''
     Download using FFMPEG with real-time progress reporting.
     FFMPEG must be installed on your system.
     You can override FFMPEG access with consts.FFMPEG_COMMAND.
 
     Args:
         video       (Video): The video object to download.
@@ -111,30 +111,28 @@
 
             if progress == 100:
                 logger.info("Download successful")
 
     except Exception as err:
         logger.error('Error while downloading: %s', err)
 
-
 def _thread(client: Client, url: str, timeout: int) -> bytes:
     '''
     Download a single segment using the client's call method.
     This function is intended to be used within a ThreadPoolExecutor.
     '''
     try:
         response = client.call(url, timeout=timeout, silent=True)
         response.raise_for_status()  # Assuming client.call returns an object with a similar interface to requests.Response
         return (url, response.content, True)
 
     except Exception as e:
         logging.warning(f"Failed to download segment {url}: {e}")
         return (url, b'', False)
 
-
 # Modify _base_threaded to use ThreadPoolExecutor
 def _base_threaded(client: Client, segments: list[str], callback: CallbackType, max_workers: int = 20,
                    timeout: int = 10) -> dict[str, bytes]:
     '''
     Base threaded downloader using ThreadPoolExecutor.
     '''
     logging.info('Threaded download initiated')
@@ -158,15 +156,14 @@
                 callback(len(buffer), length)
             except Exception as e:
                 logging.warning(f"Error processing segment {url}: {e}")
 
     client.session.mount('https://', old_adapter)
     return buffer
 
-
 def threaded(max_workers: int = 20,
              timeout: int = 10) -> Callable:
     '''
     Simple threaded downloader.
     
     Args:
         max_workers (int): How many downloads can take place simultaneously.
```

### Comparing `phub-4.6/src/phub/modules/parser.py` & `phub-4.7/src/phub/modules/parser.py`

 * *Files identical despite different names*

### Comparing `phub-4.6/src/phub/modules/rss.py` & `phub-4.7/src/phub/modules/rss.py`

 * *Files identical despite different names*

### Comparing `phub-4.6/src/phub/objects/account.py` & `phub-4.7/src/phub/objects/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 from functools import cached_property
-from typing import TYPE_CHECKING, Self, Literal, Iterator
+from typing import TYPE_CHECKING, Literal, Iterator, Union
 
 from .. import utils
 from .. import consts
 from . import User, Image
 
 if TYPE_CHECKING:
     from ..core import Client
@@ -18,15 +18,15 @@
 class Account:
     '''
     Represents a connected Ponhub account,
     capable of accessing account-only features.
     If the login fails, there will be None.
     '''
     
-    def __new__(cls, client: Client) -> Self | None:
+    def __new__(cls, client: Client) -> Union[object, None]:
         '''
         Check if the object creation is needed.
         
         Args:
             client (Client): The client that initialized this.
         
         Returns:
@@ -173,15 +173,15 @@
         '''
         
         from . import Feed
 
         return Feed(self.client)
     
     def dictify(self,
-                keys: Literal['all'] | list[str] = 'all',
+                keys: Union[Literal['all'], list[str]] = 'all',
                 recursive: bool = False) -> dict:
         '''
         Convert the object to a dictionary.
         
         Args:
             keys (str): The data keys to include.
             recursive (bool): Whether to allow other PHUB objects to dictify.
```

### Comparing `phub-4.6/src/phub/objects/data.py` & `phub-4.7/src/phub/objects/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from functools import cached_property
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Literal, Self
+from typing import TYPE_CHECKING, Literal, Union
 
 from .. import utils
 from .. import consts
 
 if TYPE_CHECKING:
     from .. import Client
     from . import User
@@ -24,15 +24,15 @@
     
     def __eq__(self, __value: object) -> bool:
         
         assert isinstance(__value, Tag)
         return self.name == __value.name
     
     def dictify(self,
-                keys: Literal['all'] | list[str] = 'all',
+                keys: Union[Literal['all'], list[str]] = 'all',
                 recursive: bool = False) -> dict:
         '''
         Convert the object to a dictionary.
         
         Args:
             keys (str): The data keys to include.
             recursive (bool): Whether to allow other PHUB objects to dictify.
@@ -50,15 +50,15 @@
     '''
     
     up: int
     down: int
     ratings: float = field(repr = False)
     
     def dictify(self,
-                keys: Literal['all'] | list[str] = 'all',
+                keys: Union[Literal['all'], list[str]] = 'all',
                 recursive: bool = False) -> dict:
         '''
         Convert the object to a dictionary.
         
         Args:
             keys (str): The data keys to include.
             recursive (bool): Whether to allow other PHUB objects to dictify.
@@ -79,15 +79,15 @@
     raw: str = None
     type: str = None
     
     def __repr__(self) -> str:
         return f'FeedItem(type={self.item_type})'
     
     def dictify(self,
-                keys: Literal['all'] | list[str] = 'all',
+                keys: Union[Literal['all'], list[str]] = 'all',
                 recursive: bool = False) -> dict:
         '''
         Convert the object to a dictionary.
         
         Args:
             keys (str): The data keys to include.
             recursive (bool): Whether to allow other PHUB objects to dictify.
@@ -156,15 +156,15 @@
 
 class _BaseQuality:
     '''
     Represents a constant quality object that can selects
     itself among a list of qualities.
     '''
     
-    def __init__(self, value: Literal['best', 'half', 'worst'] | int | Self) -> None:
+    def __init__(self, value: Union[Literal['best', 'half', 'worst'], int, object]) -> None:
         '''
         Initialize a new quality object.
         
         Args:
             value (Literal['best', 'half', 'worst'] | int | Self): String, number or quality object to initialize from.
         '''
         
@@ -207,14 +207,15 @@
             if self.value == 'best': return qualities[max(keys)]
             elif self.value == 'worst': return qualities[min(keys)]
             else: return qualities[ sorted(keys)[ len(keys) // 2 ] ]
         
         elif isinstance(self.value, int):
             # Get exact quality or nearest
             
-            if (s:= str(self.value)) in keys: return qualities[s]
+            raw = str(self.value)
+            if raw in keys: return qualities[raw]
             else: return qualities[utils.closest(keys, self.value)]
         
         # This should not happen
         raise TypeError('Internal error: quality type is', type(self.value))
 
 # EOF
```

### Comparing `phub-4.6/src/phub/objects/feed.py` & `phub-4.7/src/phub/objects/feed.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 from functools import cached_property
-from typing import TYPE_CHECKING, Callable, Iterator
+from typing import TYPE_CHECKING, Callable, Iterator, Union
 
 from .. import literals
 from . import User, FeedItem
 
 if TYPE_CHECKING:
     from . import queries
     from ..core import Client
@@ -33,15 +33,15 @@
     
     def __repr__(self) -> str:
         
         return f'phub.FeedCreator(for={self.client.account.name})'
     
     def filter(self,
                section: literals.section = None,
-               user: User | str = None) -> queries.FeedQuery:
+               user: Union[User, str] = None) -> queries.FeedQuery:
         '''
         Creates a Feed Query with specific filters.
         
         Args:
             section (str): Filter parameters.
             user (User | str): User to filter feed with.
         '''
```

### Comparing `phub-4.6/src/phub/objects/image.py` & `phub-4.7/src/phub/objects/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import os
 import logging
-from typing import TYPE_CHECKING, Literal
+from typing import TYPE_CHECKING, Literal, Union
 
 from .. import utils
 
 if TYPE_CHECKING:
     from ..core import Client
 
 
@@ -87,15 +87,15 @@
                 # Pop server and retry
                 server = self._servers.pop(0)
                 logger.info('Retrying download with server %s', server)
                 self.url = server['src']
                 self.download(path)
 
     def dictify(self,
-                keys: Literal['all'] | list[str] = 'all',
+                keys: Union[Literal['all'], list[str]] = 'all',
                 recursive: bool = False) -> dict:
         '''
         Convert the object to a dictionary.
         
         Args:
             keys (str): The data keys to include.
             recursive (bool): Whether to allow other PHUB objects to dictify.
```

### Comparing `phub-4.6/src/phub/objects/playlist.py` & `phub-4.7/src/phub/objects/playlist.py`

 * *Files identical despite different names*

### Comparing `phub-4.6/src/phub/objects/query.py` & `phub-4.7/src/phub/objects/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 import json
 import logging
 from functools import cache, cached_property
-from typing import TYPE_CHECKING, Iterator, Any, Callable
+from typing import TYPE_CHECKING, Iterator, Any, Callable, Union
 
 from . import Video, User, FeedItem
 
 from .. import utils
 from .. import consts
 from .. import errors
 
 if TYPE_CHECKING:
     from ..core import Client
 
 logger = logging.getLogger(__name__)
 
-QueryItem = Video | FeedItem | User
+QueryItem = Union[Video, FeedItem, User]
 
 class Pages:
     '''
     An iterator for query pages.
     '''
 
     def __init__(self, query: Query) -> None:
@@ -30,15 +30,15 @@
         
         self.query = query
     
     def __repr__(self) -> str:
         
         return f'phub.Pages(query={self.query})'
     
-    def __getitem__(self, index: int | slice) -> Iterator[QueryItem] | Iterator[Iterator[QueryItem]]:
+    def __getitem__(self, index: Union[int, slice]) -> Union[Iterator[QueryItem], Iterator[Iterator[QueryItem]]]:
         '''
         Get a single, or slice of pages.
         '''
         
         if isinstance(index, int):
             items = self.query._get_page(index)
             return self.query._iter_page(items)
@@ -70,15 +70,15 @@
     
     BASE: str = None
     
     def __init__(self,
                  client: Client,
                  func: str,
                  args: dict[str] = {},
-                 container_hint: consts.WrappedRegex | Callable = None,
+                 container_hint: Union[consts.WrappedRegex, Callable] = None,
                  query_repr: str = None) -> None:
         '''
         Initialise a new query.
         
         Args:
             client (Client): The parent client.
             func (str): The URL function.
@@ -133,16 +133,16 @@
         for page in self.pages:
             for item in page:
                 yield item
     
     def sample(self,
                max: int = 0,
                filter: Callable[[QueryItem], bool] = None,
-               watched: bool | None = None,
-               free_premium: bool | None = None) -> Iterator[QueryItem]:
+               watched: Union[bool, None] = None,
+               free_premium: Union[bool, None] = None) -> Iterator[QueryItem]:
         '''
         Get a sample of the query.
         
         Args:
             max (int): Maximum amount of items to fetch.
             filter (Callable): A filter function that decides whether to keep each QueryItems.
             watched (bool): Whether videos should have been watched by the account or not.
```

### Comparing `phub-4.6/src/phub/objects/user.py` & `phub-4.7/src/phub/objects/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
+from dataclasses import dataclass
 from functools import cached_property
-from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Self, Literal
+from typing import TYPE_CHECKING, Literal, Union
 
 from .. import utils
 from .. import consts
 from .. import errors
 
 if TYPE_CHECKING:
     from ..core import Client
@@ -70,15 +70,15 @@
         # Clear properties cache
         for key in list(self.__dict__.keys()):
             if not key in self.loaded_keys:
                 logger.debug('Deleting key %s', key)
                 delattr(self, key)
 
     def dictify(self,
-                keys: Literal['all'] | list[str] = 'all',
+                keys: Union[Literal['all'], list[str]] = 'all',
                 recursive: bool = False) -> dict:
             '''
             Convert the object to a dictionary.
             
             Args:
                 keys (str): The data keys to include.
                 recursive (bool): Whether to allow other PHUB objects to dictify.
@@ -123,26 +123,28 @@
         Args:
             client (Client): The parent client.
             user (str): Username or URL.
         '''
         
         if consts.re.is_url(user):
             url = user
-            user_type = (path := url.split('/'))[-2]
+            path = url.split('/')
+            user_type = path[-2]
             name = path[-1]
         
         else:
             name = '-'.join(user.split())
             
             # Guess the user type
             for type_ in ('model', 'pornstar', 'channels'):            
                 
                 guess = utils.concat(type_, name)
+                response = utils.head(client, guess)
                 
-                if response := utils.head(client, guess):
+                if response:
                     logger.info('Guessing type of %s is %s', user, type_)
                     url = response
                     user_type = type_
                     break
             
             else:
                 logger.error('Could not guess type of %s', user)
@@ -158,16 +160,17 @@
         
         index = _QuerySupportIndex()
         videos_url = utils.concat(self.url, 'videos')
 
         if utils.head(self.client, videos_url):
             index.videos = videos_url
         
-        if self.type == 'pornstar' and \
-           utils.head(self.client, upload_url := utils.concat(videos_url, 'upload')):
+        upload_url = utils.concat(videos_url, 'upload')
+        
+        if self.type == 'pornstar' and utils.head(self.client, upload_url):
             index.upload = upload_url
         
         return index
     
     @cached_property
     def videos(self) -> queries.VideoQuery:
         '''
@@ -210,15 +213,15 @@
         '''
         The user page.
         '''
         
         return self.client.call(self.url).text
 
     @cached_property
-    def bio(self) -> str | None:
+    def bio(self) -> Union[str, None]:
         '''
         The user bio.
         '''
         
         return consts.re.user_bio(self._page, throw = False)
 
     @cached_property
```

### Comparing `phub-4.6/src/phub/objects/video.py` & `phub-4.7/src/phub/objects/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 import html
 import os
 import random
 import logging
 from functools import cached_property
 from datetime import datetime, timedelta
-from typing import (TYPE_CHECKING, Iterator, Literal,
-                    LiteralString, Callable, Any)
+from typing import TYPE_CHECKING, Iterator, Literal, Callable, Any
 
 from . import Tag, Like, User, Image
 from .. import utils
 from .. import errors
 from .. import consts
 from .. import literals
 from ..modules import download, parser, display
@@ -541,15 +540,15 @@
         '''
         The categories of the video.
         '''
         
         return [item['category'] for item in self.fetch('data@categories')]
         
     @cached_property
-    def orientation(self) -> LiteralString:
+    def orientation(self) -> str:
         '''
         Video sexual orientation (e.g. straight).
         '''
         
         return self.fetch('data@segment')
     
     @cached_property
```

### Comparing `phub-4.6/src/phub/tests/test_model.py` & `phub-4.7/src/phub/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `phub-4.6/src/phub/tests/test_playlist.py` & `phub-4.7/src/phub/tests/test_playlist.py`

 * *Files identical despite different names*

### Comparing `phub-4.6/src/phub/tests/test_search.py` & `phub-4.7/src/phub/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `phub-4.6/src/phub/tests/test_video.py` & `phub-4.7/src/phub/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `phub-4.6/src/phub/utils.py` & `phub-4.7/src/phub/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 PHUB utilities.
 '''
 
 import math
 import logging
-from typing import Generator, Iterable, Iterator
+from typing import Generator, Iterable, Iterator, Union
 
 from . import errors
 
 logger = logging.getLogger(__name__)
 
 # Named constants for least_factors
 INCREMENT = 30
@@ -104,15 +104,15 @@
         recursive (bool): Whether to allow serializing PHUB objects inside the object.
     
     Returns:
         Any: A JSON serializable object.
     '''
     
     # if an object is a built-in
-    if isinstance(object_, str | int | float | bool):
+    if isinstance(object_, (str, int, float, bool)):
         ser = object_
     
     # If an object is a PHUB object
     elif hasattr(object_, 'dictify') and recursive:
         ser = object_.dictify(recursive = recursive)
     
     # If an object is a soup
@@ -120,24 +120,24 @@
         ser = object_.decode()
     
     # If an object is a dict
     elif isinstance(object_, dict):
         ser = {k: (serialize(v, True)) for k, v in object_.items()}
     
     # If an object is a list or a generator
-    elif isinstance(object_, list | tuple | Generator | Iterator | map):
+    elif isinstance(object_, (list, tuple, Generator, Iterator, map)):
         ser = [serialize(value, True) for value in object_]
     
     else:
         ser = str(object_)
     
     return ser
 
 def dictify(object_: object,
-            keys: str | list[str],
+            keys: Union[str, list[str]],
             all_: list[str],
             recursive: bool) -> dict:
     '''
     Dictify an object.
     
     Args:
         object_ (Any): The object to serialize.
@@ -151,15 +151,15 @@
     
     if isinstance(keys, str): keys = [keys]
     if 'all' in keys: keys = all_
     
     return {key: serialize(getattr(object_, key), recursive)
             for key in keys}
 
-def suppress(gen: Iterable, errs: Exception | tuple[Exception] = errors.VideoError) -> Iterator:
+def suppress(gen: Iterable, errs: Union[Exception, tuple[Exception]] = errors.VideoError) -> Iterator:
     '''
     Set up a generator to bypass items that throw errors.
     
     Args:
         gen (Iterable): The iterable to suppress.
         errs (Exception): The errors that fall under the suppression rule.
     
@@ -217,15 +217,15 @@
             if n % (i + offset) == 0:
                 return i + offset
 
         i += INCREMENT
 
     return n
 
-def head(client: object, url: str) -> str | bool:
+def head(client: object, url: str) -> Union[str, bool]:
     '''
     Performs a silent HEAD request to check if a page is available
     without fetching its content.
     
     Args:
         client (Client): A client containing an initialised session.
         url (str): The url of the request.
```

### Comparing `phub-4.6/src/phub.egg-info/PKG-INFO` & `phub-4.7/src/phub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 4.6
+Version: 4.7
 Summary: An API for Pornhub
-Author-email: Egsagon <egsagon12@gmail.com>, EchterAlsFake <EchterAlsFake@proton.me>
+Author-email: Egsagon <egsagon.git@gmail.com>, EchterAlsFake <EchterAlsFake@proton.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -679,45 +679,26 @@
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Documentation, https://phub.readthedocs.io
 Project-URL: Repository, https://github.com/EchterAlsFake/PHUB
 Keywords: pornhub,phub,porn,api,web scrapper,api wrapper
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: ffmpeg-progress-yield
 Provides-Extra: cli
 Requires-Dist: click; extra == "cli"
 
 <p align="center">
-  <img width="300" src="https://raw.githubusercontent.com/Egsagon/PHUB/master/assets/logo.svg">
+  <img width="200" src="https://raw.githubusercontent.com/Egsagon/PHUB/master/assets/logo.svg">
 </p>
 
 # PHUB - An API wrapper for PornHub.
 
-PHUB is a hybrid API for Pornhub. It is able to communicate with Pornhub
-using both web-scraping and Pornhub's HubTraffic API. It is
-able to access most used or useful PH features, such as video searching,
-accessing account features, video downloading, and a lot more.
+PHUB is an easy-to-use API wrapper for Pornhub. It can access most used or useful
+PH features, such as video searching, account features, video downloading, and more.
 
-Learn more on the project [documentation](https://phub.readthedocs.io) and
-[GitHub page](https://github.com/EchterAlsFake/PHUB).
-
-## Installation
-
-```sh
-pip install --upgrade phub
-```
-
-## Quickstart
-
-```python
-import phub
-
-client = phub.Client()
-
-video = client.get(url = '...')
-video.download('my-video.mp4', quality = 'best')
-```
+- Project documentation: [phub.readthedocs.io](https://phub.readthedocs.io)
+- Project repository: [EchterAlsFake/PHUB](https://github.com/EchterAlsFake/PHUB)
```

### Comparing `phub-4.6/src/phub.egg-info/SOURCES.txt` & `phub-4.7/src/phub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

