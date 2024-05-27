# Comparing `tmp/sounddevice-0.4.5.tar.gz` & `tmp/sounddevice-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sounddevice-0.4.5.tar", last modified: Sun Aug 21 15:36:27 2022, max compression
+gzip compressed data, was "sounddevice-0.4.6.tar", last modified: Sun Feb 19 11:44:24 2023, max compression
```

## Comparing `sounddevice-0.4.5.tar` & `sounddevice-0.4.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-08-21 15:36:27.595208 sounddevice-0.4.5/
--rw-r--r--   0 mg        (1000) mg        (1000)     4143 2021-10-12 20:18:35.000000 sounddevice-0.4.5/CONTRIBUTING.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     1063 2022-08-21 15:22:18.000000 sounddevice-0.4.5/LICENSE
--rw-r--r--   0 mg        (1000) mg        (1000)      153 2020-07-15 15:23:35.000000 sounddevice-0.4.5/MANIFEST.in
--rw-r--r--   0 mg        (1000) mg        (1000)     3338 2022-08-21 15:24:03.000000 sounddevice-0.4.5/NEWS.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     1290 2022-08-21 15:36:27.595208 sounddevice-0.4.5/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)      622 2020-07-15 15:23:35.000000 sounddevice-0.4.5/README.rst
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-08-21 15:36:27.591208 sounddevice-0.4.5/doc/
--rw-r--r--   0 mg        (1000) mg        (1000)     4143 2021-10-12 20:18:35.000000 sounddevice-0.4.5/doc/CONTRIBUTING.rst
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-08-21 15:36:27.595208 sounddevice-0.4.5/doc/api/
--rw-r--r--   0 mg        (1000) mg        (1000)      443 2022-07-19 17:26:16.000000 sounddevice-0.4.5/doc/api/checking-hardware.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      454 2022-07-19 17:26:16.000000 sounddevice-0.4.5/doc/api/convenience-functions.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      304 2022-07-19 17:26:16.000000 sounddevice-0.4.5/doc/api/expert-mode.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      230 2021-06-01 16:39:31.000000 sounddevice-0.4.5/doc/api/index.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      458 2022-07-19 17:26:16.000000 sounddevice-0.4.5/doc/api/misc.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      127 2022-07-19 17:26:16.000000 sounddevice-0.4.5/doc/api/module-defaults.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      311 2022-07-19 17:26:16.000000 sounddevice-0.4.5/doc/api/platform-specific-settings.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      296 2022-07-19 17:26:16.000000 sounddevice-0.4.5/doc/api/raw-streams.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      339 2022-07-19 17:26:16.000000 sounddevice-0.4.5/doc/api/streams.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     2626 2021-07-18 10:17:30.000000 sounddevice-0.4.5/doc/conf.py
--rw-r--r--   0 mg        (1000) mg        (1000)     1643 2021-07-18 10:15:42.000000 sounddevice-0.4.5/doc/examples.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      926 2022-04-11 21:18:43.000000 sounddevice-0.4.5/doc/fake__sounddevice.py
--rw-r--r--   0 mg        (1000) mg        (1000)      169 2020-07-15 15:23:35.000000 sounddevice-0.4.5/doc/index.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     3350 2022-07-19 16:50:21.000000 sounddevice-0.4.5/doc/installation.rst
--rw-r--r--   0 mg        (1000) mg        (1000)       50 2022-08-21 15:06:06.000000 sounddevice-0.4.5/doc/requirements.txt
--rw-r--r--   0 mg        (1000) mg        (1000)     6084 2020-07-15 15:23:35.000000 sounddevice-0.4.5/doc/usage.rst
--rw-r--r--   0 mg        (1000) mg        (1000)       90 2021-06-01 16:39:31.000000 sounddevice-0.4.5/doc/version-history.rst
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-08-21 15:36:27.595208 sounddevice-0.4.5/examples/
--rwxr-xr-x   0 mg        (1000) mg        (1000)     2196 2022-07-15 18:49:18.000000 sounddevice-0.4.5/examples/asyncio_coroutines.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)     3390 2022-07-18 20:27:14.000000 sounddevice-0.4.5/examples/asyncio_generators.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)     2394 2022-03-21 21:19:39.000000 sounddevice-0.4.5/examples/play_file.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)     3476 2021-07-18 10:15:42.000000 sounddevice-0.4.5/examples/play_long_file.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)     3190 2021-07-18 10:15:42.000000 sounddevice-0.4.5/examples/play_long_file_raw.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)     1878 2020-07-15 15:23:35.000000 sounddevice-0.4.5/examples/play_sine.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)     3596 2021-06-01 16:39:31.000000 sounddevice-0.4.5/examples/play_stream.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)     3894 2022-04-11 21:18:43.000000 sounddevice-0.4.5/examples/plot_input.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)      793 2020-07-15 15:23:35.000000 sounddevice-0.4.5/examples/priming_output.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)     7648 2022-06-03 18:11:50.000000 sounddevice-0.4.5/examples/rec_gui.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)     2831 2022-07-19 17:26:16.000000 sounddevice-0.4.5/examples/rec_unlimited.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)     3718 2022-04-11 21:18:43.000000 sounddevice-0.4.5/examples/spectrogram.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)     2119 2022-07-19 17:26:16.000000 sounddevice-0.4.5/examples/wire.py
--rw-r--r--   0 mg        (1000) mg        (1000)       73 2022-08-21 15:36:27.595208 sounddevice-0.4.5/setup.cfg
--rw-r--r--   0 mg        (1000) mg        (1000)     2812 2022-04-11 21:18:43.000000 sounddevice-0.4.5/setup.py
-drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2022-08-21 15:36:27.595208 sounddevice-0.4.5/sounddevice.egg-info/
--rw-r--r--   0 mg        (1000) mg        (1000)     1290 2022-08-21 15:36:27.000000 sounddevice-0.4.5/sounddevice.egg-info/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)     1043 2022-08-21 15:36:27.000000 sounddevice-0.4.5/sounddevice.egg-info/SOURCES.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2022-08-21 15:36:27.000000 sounddevice-0.4.5/sounddevice.egg-info/dependency_links.txt
--rw-r--r--   0 mg        (1000) mg        (1000)       25 2022-08-21 15:36:27.000000 sounddevice-0.4.5/sounddevice.egg-info/requires.txt
--rw-r--r--   0 mg        (1000) mg        (1000)       25 2022-08-21 15:36:27.000000 sounddevice-0.4.5/sounddevice.egg-info/top_level.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2022-08-21 15:36:27.000000 sounddevice-0.4.5/sounddevice.egg-info/zip-safe
--rw-r--r--   0 mg        (1000) mg        (1000)   107959 2022-08-21 15:21:44.000000 sounddevice-0.4.5/sounddevice.py
--rw-r--r--   0 mg        (1000) mg        (1000)    10331 2022-03-03 19:40:29.000000 sounddevice-0.4.5/sounddevice_build.py
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-02-19 11:44:24.703644 sounddevice-0.4.6/
+-rw-r--r--   0 mg        (1000) mg        (1000)     4143 2021-10-12 20:18:35.000000 sounddevice-0.4.6/CONTRIBUTING.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     1063 2023-02-19 11:38:35.000000 sounddevice-0.4.6/LICENSE
+-rw-r--r--   0 mg        (1000) mg        (1000)      153 2020-07-15 15:23:35.000000 sounddevice-0.4.6/MANIFEST.in
+-rw-r--r--   0 mg        (1000) mg        (1000)     3415 2023-02-19 11:38:54.000000 sounddevice-0.4.6/NEWS.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     1290 2023-02-19 11:44:24.703644 sounddevice-0.4.6/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)      622 2020-07-15 15:23:35.000000 sounddevice-0.4.6/README.rst
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-02-19 11:44:24.699643 sounddevice-0.4.6/doc/
+-rw-r--r--   0 mg        (1000) mg        (1000)     4143 2021-10-12 20:18:35.000000 sounddevice-0.4.6/doc/CONTRIBUTING.rst
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-02-19 11:44:24.699643 sounddevice-0.4.6/doc/api/
+-rw-r--r--   0 mg        (1000) mg        (1000)      443 2022-07-19 17:26:16.000000 sounddevice-0.4.6/doc/api/checking-hardware.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      454 2022-07-19 17:26:16.000000 sounddevice-0.4.6/doc/api/convenience-functions.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      304 2022-07-19 17:26:16.000000 sounddevice-0.4.6/doc/api/expert-mode.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      230 2022-11-22 08:14:32.000000 sounddevice-0.4.6/doc/api/index.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      458 2022-07-19 17:26:16.000000 sounddevice-0.4.6/doc/api/misc.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      127 2022-07-19 17:26:16.000000 sounddevice-0.4.6/doc/api/module-defaults.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      311 2022-07-19 17:26:16.000000 sounddevice-0.4.6/doc/api/platform-specific-settings.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      296 2022-07-19 17:26:16.000000 sounddevice-0.4.6/doc/api/raw-streams.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      339 2022-07-19 17:26:16.000000 sounddevice-0.4.6/doc/api/streams.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     2626 2022-11-29 21:07:12.000000 sounddevice-0.4.6/doc/conf.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     1643 2021-07-18 10:15:42.000000 sounddevice-0.4.6/doc/examples.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)      926 2022-04-11 21:18:43.000000 sounddevice-0.4.6/doc/fake__sounddevice.py
+-rw-r--r--   0 mg        (1000) mg        (1000)      169 2022-11-29 21:07:12.000000 sounddevice-0.4.6/doc/index.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     3350 2022-07-19 16:50:21.000000 sounddevice-0.4.6/doc/installation.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)       50 2022-08-21 15:06:06.000000 sounddevice-0.4.6/doc/requirements.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)     6084 2020-07-15 15:23:35.000000 sounddevice-0.4.6/doc/usage.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)       90 2021-06-01 16:39:31.000000 sounddevice-0.4.6/doc/version-history.rst
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-02-19 11:44:24.703644 sounddevice-0.4.6/examples/
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     2196 2022-07-15 18:49:18.000000 sounddevice-0.4.6/examples/asyncio_coroutines.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     3390 2022-07-18 20:27:14.000000 sounddevice-0.4.6/examples/asyncio_generators.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     2394 2022-03-21 21:19:39.000000 sounddevice-0.4.6/examples/play_file.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     3476 2021-07-18 10:15:42.000000 sounddevice-0.4.6/examples/play_long_file.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     3190 2021-07-18 10:15:42.000000 sounddevice-0.4.6/examples/play_long_file_raw.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     1878 2020-07-15 15:23:35.000000 sounddevice-0.4.6/examples/play_sine.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     3596 2021-06-01 16:39:31.000000 sounddevice-0.4.6/examples/play_stream.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     3894 2022-04-11 21:18:43.000000 sounddevice-0.4.6/examples/plot_input.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)      793 2020-07-15 15:23:35.000000 sounddevice-0.4.6/examples/priming_output.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     7648 2022-06-03 18:11:50.000000 sounddevice-0.4.6/examples/rec_gui.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     2831 2022-07-19 17:26:16.000000 sounddevice-0.4.6/examples/rec_unlimited.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     3718 2022-04-11 21:18:43.000000 sounddevice-0.4.6/examples/spectrogram.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     2119 2022-07-19 17:26:16.000000 sounddevice-0.4.6/examples/wire.py
+-rw-r--r--   0 mg        (1000) mg        (1000)       73 2023-02-19 11:44:24.707644 sounddevice-0.4.6/setup.cfg
+-rw-r--r--   0 mg        (1000) mg        (1000)     2812 2022-04-11 21:18:43.000000 sounddevice-0.4.6/setup.py
+drwxr-xr-x   0 mg        (1000) mg        (1000)        0 2023-02-19 11:44:24.703644 sounddevice-0.4.6/sounddevice.egg-info/
+-rw-r--r--   0 mg        (1000) mg        (1000)     1290 2023-02-19 11:44:24.000000 sounddevice-0.4.6/sounddevice.egg-info/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)     1043 2023-02-19 11:44:24.000000 sounddevice-0.4.6/sounddevice.egg-info/SOURCES.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-02-19 11:44:24.000000 sounddevice-0.4.6/sounddevice.egg-info/dependency_links.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)       25 2023-02-19 11:44:24.000000 sounddevice-0.4.6/sounddevice.egg-info/requires.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)       25 2023-02-19 11:44:24.000000 sounddevice-0.4.6/sounddevice.egg-info/top_level.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2023-02-19 11:44:24.000000 sounddevice-0.4.6/sounddevice.egg-info/zip-safe
+-rw-r--r--   0 mg        (1000) mg        (1000)   107702 2023-02-19 11:38:38.000000 sounddevice-0.4.6/sounddevice.py
+-rw-r--r--   0 mg        (1000) mg        (1000)    10116 2023-01-25 10:29:46.000000 sounddevice-0.4.6/sounddevice_build.py
```

### Comparing `sounddevice-0.4.5/CONTRIBUTING.rst` & `sounddevice-0.4.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/LICENSE` & `sounddevice-0.4.6/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2015-2022 Matthias Geier
+Copyright (c) 2015-2023 Matthias Geier
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sounddevice-0.4.5/NEWS.rst` & `sounddevice-0.4.6/NEWS.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+0.4.6 (2023-02-19):
+ * Redirect stderr with os.dup2() instead of CFFI calls
+
 0.4.5 (2022-08-21):
  * Add ``index`` field to device dict
  * Require Python >= 3.7
  * Add PaWasapi_IsLoopback() to cdef (high-level interface not yet available)
 
 0.4.4 (2021-12-31):
  * Exact device string matches can now include the host API name
```

### Comparing `sounddevice-0.4.5/PKG-INFO` & `sounddevice-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sounddevice
-Version: 0.4.5
+Version: 0.4.6
 Summary: Play and Record Sound with Python
 Home-page: http://python-sounddevice.readthedocs.io/
 Author: Matthias Geier
 Author-email: Matthias.Geier@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/spatialaudio/python-sounddevice
 Keywords: sound,audio,PortAudio,play,record,playrec
```

### Comparing `sounddevice-0.4.5/README.rst` & `sounddevice-0.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/doc/CONTRIBUTING.rst` & `sounddevice-0.4.6/doc/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/doc/conf.py` & `sounddevice-0.4.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/doc/examples.rst` & `sounddevice-0.4.6/doc/examples.rst`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/doc/fake__sounddevice.py` & `sounddevice-0.4.6/doc/fake__sounddevice.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/doc/installation.rst` & `sounddevice-0.4.6/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/doc/usage.rst` & `sounddevice-0.4.6/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/examples/asyncio_coroutines.py` & `sounddevice-0.4.6/examples/asyncio_coroutines.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/examples/asyncio_generators.py` & `sounddevice-0.4.6/examples/asyncio_generators.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/examples/play_file.py` & `sounddevice-0.4.6/examples/play_file.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/examples/play_long_file.py` & `sounddevice-0.4.6/examples/play_long_file.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/examples/play_long_file_raw.py` & `sounddevice-0.4.6/examples/play_long_file_raw.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/examples/play_sine.py` & `sounddevice-0.4.6/examples/play_sine.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/examples/play_stream.py` & `sounddevice-0.4.6/examples/play_stream.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/examples/plot_input.py` & `sounddevice-0.4.6/examples/plot_input.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/examples/priming_output.py` & `sounddevice-0.4.6/examples/priming_output.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/examples/rec_gui.py` & `sounddevice-0.4.6/examples/rec_gui.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/examples/rec_unlimited.py` & `sounddevice-0.4.6/examples/rec_unlimited.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/examples/spectrogram.py` & `sounddevice-0.4.6/examples/spectrogram.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/examples/wire.py` & `sounddevice-0.4.6/examples/wire.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/setup.py` & `sounddevice-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/sounddevice.egg-info/PKG-INFO` & `sounddevice-0.4.6/sounddevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sounddevice
-Version: 0.4.5
+Version: 0.4.6
 Summary: Play and Record Sound with Python
 Home-page: http://python-sounddevice.readthedocs.io/
 Author: Matthias Geier
 Author-email: Matthias.Geier@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/spatialaudio/python-sounddevice
 Keywords: sound,audio,PortAudio,play,record,playrec
```

### Comparing `sounddevice-0.4.5/sounddevice.egg-info/SOURCES.txt` & `sounddevice-0.4.6/sounddevice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sounddevice-0.4.5/sounddevice.py` & `sounddevice-0.4.6/sounddevice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2015-2021 Matthias Geier
+# Copyright (c) 2015-2023 Matthias Geier
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -44,15 +44,15 @@
     `sleep()`, `get_portaudio_version()`, `CallbackFlags`,
     `CallbackStop`, `CallbackAbort`
 
 Online documentation:
     https://python-sounddevice.readthedocs.io/
 
 """
-__version__ = '0.4.5'
+__version__ = '0.4.6'
 
 import atexit as _atexit
 import os as _os
 import platform as _platform
 import sys as _sys
 from ctypes.util import find_library as _find_library
 from _sounddevice import ffi as _ffi
@@ -2821,35 +2821,28 @@
 
     In most cases, this doesn't have to be called explicitly, because it
     is automatically called with the ``import sounddevice`` statement.
 
     """
     old_stderr = None
     try:
-        stdio = _ffi.dlopen(None)
+        old_stderr = _os.dup(2)
+        devnull = _os.open(_os.devnull, _os.O_WRONLY)
+        _os.dup2(devnull, 2)
+        _os.close(devnull)
     except OSError:
         pass
-    else:
-        for stderr_name in 'stderr', '__stderrp':
-            try:
-                old_stderr = getattr(stdio, stderr_name)
-            except _ffi.error:
-                continue
-            else:
-                devnull = stdio.fopen(_os.devnull.encode(), b'w')
-                setattr(stdio, stderr_name, devnull)
-                break
     try:
         _check(_lib.Pa_Initialize(), 'Error initializing PortAudio')
         global _initialized
         _initialized += 1
     finally:
         if old_stderr is not None:
-            setattr(stdio, stderr_name, old_stderr)
-            stdio.fclose(devnull)
+            _os.dup2(old_stderr, 2)
+            _os.close(old_stderr)
 
 
 def _terminate():
     """Terminate PortAudio.
 
     In most cases, this doesn't have to be called explicitly.
```

### Comparing `sounddevice-0.4.5/sounddevice_build.py` & `sounddevice-0.4.6/sounddevice_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,17 +307,9 @@
     PaWasapiStreamCategory streamCategory;
     PaWasapiStreamOption streamOption;
 } PaWasapiStreamInfo;
 
 int PaWasapi_IsLoopback( PaDeviceIndex device );
 """)
 
-ffibuilder.cdef("""
-    /* from stdio.h */
-    FILE* fopen(const char* path, const char* mode);
-    int fclose(FILE* fp);
-    extern FILE* stderr;  /* GNU C library */
-    extern FILE* __stderrp;  /* macOS */
-""")
-
 if __name__ == '__main__':
     ffibuilder.compile(verbose=True)
```

