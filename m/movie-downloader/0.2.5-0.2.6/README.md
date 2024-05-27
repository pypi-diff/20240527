# Comparing `tmp/movie-downloader-0.2.5.tar.gz` & `tmp/movie-downloader-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\projects\movie-downloader\dist\tmpgo646vgl\movie-downloader-0.2.5.tar", last modified: Wed May  8 02:17:24 2024, max compression
+gzip compressed data, was "C:\projects\movie-downloader\dist\tmppcllbyof\movie-downloader-0.2.6.tar", last modified: Mon May 27 03:34:36 2024, max compression
```

## Comparing `movie-downloader-0.2.5.tar` & `movie-downloader-0.2.6.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/
--rw-rw-rw-   0        0        0      177 2022-05-24 02:08:13.000000 movie-downloader-0.2.5/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/
--rw-rw-rw-   0        0        0     2137 2023-03-17 08:17:40.000000 movie-downloader-0.2.5/mdl/commons.py
-drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/conf/
--rw-rw-rw-   0        0        0     4229 2024-04-12 05:39:22.000000 movie-downloader-0.2.5/mdl/conf/dlops.conf
--rw-rw-rw-   0        0        0      253 2022-05-24 02:08:13.000000 movie-downloader-0.2.5/mdl/conf/misc.conf
--rw-rw-rw-   0        0        0    12875 2024-04-04 15:37:04.000000 movie-downloader-0.2.5/mdl/downloader.py
-drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/js/
--rw-rw-rw-   0        0        0    29485 2023-05-24 09:09:12.000000 movie-downloader-0.2.5/mdl/js/vqq_ckey-8.1.js
--rw-rw-rw-   0        0        0    31710 2023-09-26 16:39:11.000000 movie-downloader-0.2.5/mdl/js/vqq_ckey-8.5.js
--rw-rw-rw-   0        0        0    10669 2023-05-24 11:42:29.000000 movie-downloader-0.2.5/mdl/js/vqq_ckey-9.1.js
-drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/log/
--rw-rw-rw-   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/log/mdl.log
-drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/sites/
--rw-rw-rw-   0        0        0    14343 2024-03-08 16:14:06.000000 movie-downloader-0.2.5/mdl/sites/m1905.py
--rw-rw-rw-   0        0        0    45194 2024-04-12 05:39:22.000000 movie-downloader-0.2.5/mdl/sites/vqq.py
--rw-rw-rw-   0        0        0      360 2022-05-24 02:08:13.000000 movie-downloader-0.2.5/mdl/sites/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/third_parties/
-drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/third_parties/aria2/
--rw-rw-rw-   0        0        0      101 2022-06-12 03:41:05.000000 movie-downloader-0.2.5/mdl/third_parties/aria2/README
-drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/third_parties/ckey/
--rw-rw-rw-   0        0        0      161 2022-05-24 02:08:13.000000 movie-downloader-0.2.5/mdl/third_parties/ckey/README
-drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/third_parties/ffmpeg/
--rw-rw-rw-   0        0        0       76 2021-11-15 11:57:06.000000 movie-downloader-0.2.5/mdl/third_parties/ffmpeg/README
-drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/third_parties/mkvtoolnix/
--rw-rw-rw-   0        0        0      102 2022-06-12 03:41:05.000000 movie-downloader-0.2.5/mdl/third_parties/mkvtoolnix/README
-drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/third_parties/node/
--rw-rw-rw-   0        0        0       69 2022-05-24 02:08:13.000000 movie-downloader-0.2.5/mdl/third_parties/node/README
-drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/third_parties/setupext_janitor/
--rw-rw-rw-   0        0        0     7217 2022-03-03 03:10:20.000000 movie-downloader-0.2.5/mdl/third_parties/setupext_janitor/janitor.py
--rw-rw-rw-   0        0        0     5228 2021-11-15 11:57:06.000000 movie-downloader-0.2.5/mdl/third_parties/setupext_janitor/README.rst
--rw-rw-rw-   0        0        0    13647 2022-11-11 05:46:23.000000 movie-downloader-0.2.5/mdl/third_parties/__init__.py
--rw-rw-rw-   0        0        0      338 2021-11-15 11:57:06.000000 movie-downloader-0.2.5/mdl/third_parties/__main__.py
--rw-rw-rw-   0        0        0     5640 2022-06-01 04:53:01.000000 movie-downloader-0.2.5/mdl/utils.py
--rw-rw-rw-   0        0        0     3965 2024-04-05 10:09:24.000000 movie-downloader-0.2.5/mdl/videoconfig.py
--rw-rw-rw-   0        0        0     6893 2024-03-30 04:55:37.000000 movie-downloader-0.2.5/mdl/__init__.py
--rw-rw-rw-   0        0        0      392 2021-11-15 11:57:06.000000 movie-downloader-0.2.5/mdl/__main__.py
--rw-rw-rw-   0        0        0     7269 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     6107 2024-05-07 09:22:21.000000 movie-downloader-0.2.5/README.md
--rw-rw-rw-   0        0        0      213 2024-05-07 04:13:17.000000 movie-downloader-0.2.5/requirements.txt
--rw-rw-rw-   0        0        0       58 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2745 2024-05-07 04:13:17.000000 movie-downloader-0.2.5/setup.py
--rw-rw-rw-   0        0        0        5 2024-05-08 01:47:52.000000 movie-downloader-0.2.5/VERSION
+drwxrwxrwx   0        0        0        0 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/
+-rw-rw-rw-   0        0        0      177 2022-05-24 02:08:13.000000 movie-downloader-0.2.6/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/mdl/
+-rw-rw-rw-   0        0        0     2137 2023-03-17 08:17:40.000000 movie-downloader-0.2.6/mdl/commons.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/mdl/conf/
+-rw-rw-rw-   0        0        0     4229 2024-04-12 05:39:22.000000 movie-downloader-0.2.6/mdl/conf/dlops.conf
+-rw-rw-rw-   0        0        0      253 2022-05-24 02:08:13.000000 movie-downloader-0.2.6/mdl/conf/misc.conf
+-rw-rw-rw-   0        0        0    12875 2024-04-04 15:37:04.000000 movie-downloader-0.2.6/mdl/downloader.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/mdl/js/
+-rw-rw-rw-   0        0        0    29485 2023-05-24 09:09:12.000000 movie-downloader-0.2.6/mdl/js/vqq_ckey-8.1.js
+-rw-rw-rw-   0        0        0    31710 2023-09-26 16:39:11.000000 movie-downloader-0.2.6/mdl/js/vqq_ckey-8.5.js
+-rw-rw-rw-   0        0        0    10669 2023-05-24 11:42:29.000000 movie-downloader-0.2.6/mdl/js/vqq_ckey-9.1.js
+drwxrwxrwx   0        0        0        0 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/mdl/log/
+-rw-rw-rw-   0        0        0        0 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/mdl/log/mdl.log
+drwxrwxrwx   0        0        0        0 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/mdl/sites/
+-rw-rw-rw-   0        0        0    14343 2024-03-08 16:14:06.000000 movie-downloader-0.2.6/mdl/sites/m1905.py
+-rw-rw-rw-   0        0        0    45194 2024-04-12 05:39:22.000000 movie-downloader-0.2.6/mdl/sites/vqq.py
+-rw-rw-rw-   0        0        0      360 2022-05-24 02:08:13.000000 movie-downloader-0.2.6/mdl/sites/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/mdl/third_parties/
+drwxrwxrwx   0        0        0        0 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/mdl/third_parties/aria2/
+-rw-rw-rw-   0        0        0      101 2022-06-12 03:41:05.000000 movie-downloader-0.2.6/mdl/third_parties/aria2/README
+drwxrwxrwx   0        0        0        0 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/mdl/third_parties/ckey/
+-rw-rw-rw-   0        0        0      161 2022-05-24 02:08:13.000000 movie-downloader-0.2.6/mdl/third_parties/ckey/README
+drwxrwxrwx   0        0        0        0 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/mdl/third_parties/ffmpeg/
+-rw-rw-rw-   0        0        0       76 2021-11-15 11:57:06.000000 movie-downloader-0.2.6/mdl/third_parties/ffmpeg/README
+drwxrwxrwx   0        0        0        0 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/mdl/third_parties/mkvtoolnix/
+-rw-rw-rw-   0        0        0      102 2022-06-12 03:41:05.000000 movie-downloader-0.2.6/mdl/third_parties/mkvtoolnix/README
+drwxrwxrwx   0        0        0        0 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/mdl/third_parties/node/
+-rw-rw-rw-   0        0        0       69 2022-05-24 02:08:13.000000 movie-downloader-0.2.6/mdl/third_parties/node/README
+drwxrwxrwx   0        0        0        0 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/mdl/third_parties/setupext_janitor/
+-rw-rw-rw-   0        0        0     7217 2022-03-03 03:10:20.000000 movie-downloader-0.2.6/mdl/third_parties/setupext_janitor/janitor.py
+-rw-rw-rw-   0        0        0     5228 2021-11-15 11:57:06.000000 movie-downloader-0.2.6/mdl/third_parties/setupext_janitor/README.rst
+-rw-rw-rw-   0        0        0    18005 2024-05-20 07:37:00.000000 movie-downloader-0.2.6/mdl/third_parties/__init__.py
+-rw-rw-rw-   0        0        0      338 2021-11-15 11:57:06.000000 movie-downloader-0.2.6/mdl/third_parties/__main__.py
+-rw-rw-rw-   0        0        0     5640 2022-06-01 04:53:01.000000 movie-downloader-0.2.6/mdl/utils.py
+-rw-rw-rw-   0        0        0     3965 2024-04-05 10:09:24.000000 movie-downloader-0.2.6/mdl/videoconfig.py
+-rw-rw-rw-   0        0        0     6894 2024-05-09 12:04:45.000000 movie-downloader-0.2.6/mdl/__init__.py
+-rw-rw-rw-   0        0        0      392 2021-11-15 11:57:06.000000 movie-downloader-0.2.6/mdl/__main__.py
+-rw-rw-rw-   0        0        0     7425 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       80 2024-05-09 12:04:45.000000 movie-downloader-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0     6107 2024-05-07 09:22:21.000000 movie-downloader-0.2.6/README.md
+-rw-rw-rw-   0        0        0      213 2024-05-20 07:37:00.000000 movie-downloader-0.2.6/requirements.txt
+-rw-rw-rw-   0        0        0       58 2024-05-27 03:34:36.000000 movie-downloader-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     2895 2024-05-20 07:37:00.000000 movie-downloader-0.2.6/setup.py
+-rw-rw-rw-   0        0        0        5 2024-05-26 03:42:47.000000 movie-downloader-0.2.6/VERSION
```

### Comparing `movie-downloader-0.2.5/mdl/commons.py` & `movie-downloader-0.2.6/mdl/commons.py`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.2.5/mdl/conf/dlops.conf` & `movie-downloader-0.2.6/mdl/conf/dlops.conf`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.2.5/mdl/downloader.py` & `movie-downloader-0.2.6/mdl/downloader.py`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.2.5/mdl/js/vqq_ckey-8.1.js` & `movie-downloader-0.2.6/mdl/js/vqq_ckey-8.1.js`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.2.5/mdl/js/vqq_ckey-8.5.js` & `movie-downloader-0.2.6/mdl/js/vqq_ckey-8.5.js`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.2.5/mdl/js/vqq_ckey-9.1.js` & `movie-downloader-0.2.6/mdl/js/vqq_ckey-9.1.js`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.2.5/mdl/sites/m1905.py` & `movie-downloader-0.2.6/mdl/sites/m1905.py`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.2.5/mdl/sites/vqq.py` & `movie-downloader-0.2.6/mdl/sites/vqq.py`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.2.5/mdl/third_parties/setupext_janitor/janitor.py` & `movie-downloader-0.2.6/mdl/third_parties/setupext_janitor/janitor.py`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.2.5/mdl/third_parties/setupext_janitor/README.rst` & `movie-downloader-0.2.6/mdl/third_parties/setupext_janitor/README.rst`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.2.5/mdl/utils.py` & `movie-downloader-0.2.6/mdl/utils.py`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.2.5/mdl/videoconfig.py` & `movie-downloader-0.2.6/mdl/videoconfig.py`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.2.5/mdl/__init__.py` & `movie-downloader-0.2.6/mdl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
     confs['playlist_items'] = {url: items for url, items in url_plist}
 
 
 def check_deps():
     if not exists_3rd_parties():
         LOGGER.error('The third-parties such as Aria2, FFmpeg, MKVToolnix and Nodejs are required. Before moving on, '
                      'simply run "mdl_3rd_parties" from within the Shell to automatically download and install them. '
-                     'Note that "--proxy" option may be needed.'
+                     'Note that "--proxy" option may be needed. '
                      'For how to get and install them manually, please refer to README.md.')
         sys.exit(-1)
 
 
 def main():
     check_deps()  # make sure the prerequisites are satisfied
```

### Comparing `movie-downloader-0.2.5/PKG-INFO` & `movie-downloader-0.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movie-downloader
-Version: 0.2.5
+Version: 0.2.6
 Summary: A fast movie downloader using Aria2
 Home-page: https://github.com/Jesseatgao/movie-downloader
 Author: Jesse Gao
 Author-email: changxigao@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: End Users/Desktop
@@ -12,14 +12,17 @@
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `movie-downloader-0.2.5/README.md` & `movie-downloader-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.2.5/setup.py` & `movie-downloader-0.2.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 setup(
     name='movie-downloader',
     version=version,
     package_dir={'': '.'},
     packages=find_packages(where='.'),
     python_requires='>=3.6',
-    install_requires=['bdownload>=0.2.0'],
+    install_requires=['bdownload>=0.2.1'],
     include_package_data=True,
     package_data={
         'mdl': [
             'log/mdl.log',
             'conf/*.conf',
             'js/*',
             'third_parties/aria2/README',
@@ -73,13 +73,16 @@
         'Environment :: Console',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ]
 )
```

