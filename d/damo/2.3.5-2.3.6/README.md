# Comparing `tmp/damo-2.3.5.tar.gz` & `tmp/damo-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-2.3.5.tar", last modified: Mon May 20 18:59:59 2024, max compression
+gzip compressed data, was "damo-2.3.6.tar", last modified: Mon May 27 17:29:03 2024, max compression
```

## Comparing `damo-2.3.5.tar` & `damo-2.3.6.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-20 18:59:59.218819 damo-2.3.5/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7502 2024-05-20 18:59:59.218819 damo-2.3.5/PKG-INFO
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     6981 2024-05-20 18:59:55.000000 damo-2.3.5/README.md
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      104 2023-09-30 00:42:34.000000 damo-2.3.5/pyproject.toml
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       38 2024-05-20 18:59:59.218819 damo-2.3.5/setup.cfg
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1104 2024-05-11 18:53:35.000000 damo-2.3.5/setup.py
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-20 18:59:59.194819 damo-2.3.5/src/
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-20 18:59:59.214819 damo-2.3.5/src/damo/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        0 2024-05-20 18:59:55.000000 damo-2.3.5/src/damo/__init__.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1442 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_ascii_color.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7357 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_deprecated.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      963 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_deprecation_notice.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      620 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_dist.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10121 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_fmt_str.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2356 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_fs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5535 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_paddr_layout.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      522 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_print.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    44681 2024-05-19 19:03:17.000000 damo-2.3.5/src/damo/_damo_records.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      780 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damo_subcmds.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    47260 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damon.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    23912 2024-05-19 19:03:17.000000 damo-2.3.5/src/damo/_damon_args.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    17432 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damon_dbgfs.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    28814 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/_damon_sysfs.py
--rwxr-xr-x   0 sjpark    (1000) sjpark    (1000)     4278 2024-05-18 15:38:34.000000 damo-2.3.5/src/damo/damo.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1858 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_adjust.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1094 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_convert_record_format.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1309 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_features.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1144 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_fmt_json.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    12165 2024-05-19 17:56:08.000000 damo-2.3.5/src/damo/damo_heats.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4498 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_lru_sort.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2860 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_monitor.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2578 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_nr_regions.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4472 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_reclaim.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5645 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_record.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3866 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_record_info.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4278 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_replay.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1587 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_report.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4566 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_report_footprint.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1672 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_report_profile.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3886 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_report_raw.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1493 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_report_times.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1502 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_schemes.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)    26899 2024-05-19 19:34:35.000000 damo-2.3.5/src/damo/damo_show.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      520 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_start.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4201 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_status.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      567 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_stop.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)      685 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_tune.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3763 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_validate.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       22 2024-05-20 18:59:47.000000 damo-2.3.5/src/damo/damo_version.py
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     6186 2024-05-18 15:35:33.000000 damo-2.3.5/src/damo/damo_wss.py
-drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-20 18:59:59.218819 damo-2.3.5/src/damo.egg-info/
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7502 2024-05-20 18:59:59.000000 damo-2.3.5/src/damo.egg-info/PKG-INFO
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1277 2024-05-20 18:59:59.000000 damo-2.3.5/src/damo.egg-info/SOURCES.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        1 2024-05-20 18:59:59.000000 damo-2.3.5/src/damo.egg-info/dependency_links.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)       40 2024-05-20 18:59:59.000000 damo-2.3.5/src/damo.egg-info/entry_points.txt
--rw-r--r--   0 sjpark    (1000) sjpark    (1000)        5 2024-05-20 18:59:59.000000 damo-2.3.5/src/damo.egg-info/top_level.txt
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-27 17:29:03.291275 damo-2.3.6/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7502 2024-05-27 17:29:03.291275 damo-2.3.6/PKG-INFO
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     6981 2024-05-27 17:28:59.000000 damo-2.3.6/README.md
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      104 2023-09-30 00:42:34.000000 damo-2.3.6/pyproject.toml
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       38 2024-05-27 17:29:03.291275 damo-2.3.6/setup.cfg
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1104 2024-05-11 18:53:35.000000 damo-2.3.6/setup.py
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-27 17:29:03.275276 damo-2.3.6/src/
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-27 17:29:03.287275 damo-2.3.6/src/damo/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        0 2024-05-27 17:28:59.000000 damo-2.3.6/src/damo/__init__.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1442 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/_damo_ascii_color.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7357 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/_damo_deprecated.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      963 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/_damo_deprecation_notice.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      620 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/_damo_dist.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    10121 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/_damo_fmt_str.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2356 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/_damo_fs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5535 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/_damo_paddr_layout.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      522 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/_damo_print.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    47666 2024-05-25 16:33:33.000000 damo-2.3.6/src/damo/_damo_records.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      780 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/_damo_subcmds.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    47260 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/_damon.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    23912 2024-05-19 19:03:17.000000 damo-2.3.6/src/damo/_damon_args.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    17432 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/_damon_dbgfs.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    28814 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/_damon_sysfs.py
+-rwxr-xr-x   0 sjpark    (1000) sjpark    (1000)     4278 2024-05-18 15:38:34.000000 damo-2.3.6/src/damo/damo.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1858 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_adjust.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1094 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_convert_record_format.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1309 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_features.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1144 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_fmt_json.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    11558 2024-05-26 16:35:08.000000 damo-2.3.6/src/damo/damo_heatmap.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    12165 2024-05-19 17:56:08.000000 damo-2.3.6/src/damo/damo_heats.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4498 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_lru_sort.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2860 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_monitor.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     2578 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_nr_regions.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4472 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_reclaim.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     5814 2024-05-25 16:33:33.000000 damo-2.3.6/src/damo/damo_record.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3866 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_record_info.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4278 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_replay.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1724 2024-05-26 16:11:02.000000 damo-2.3.6/src/damo/damo_report.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4566 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_report_footprint.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1672 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_report_profile.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3886 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_report_raw.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1493 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_report_times.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1502 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_schemes.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)    27457 2024-05-26 16:54:44.000000 damo-2.3.6/src/damo/damo_show.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      520 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_start.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     4201 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_status.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      567 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_stop.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)      685 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_tune.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     3763 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_validate.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       22 2024-05-27 17:28:51.000000 damo-2.3.6/src/damo/damo_version.py
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     6186 2024-05-18 15:35:33.000000 damo-2.3.6/src/damo/damo_wss.py
+drwxr-xr-x   0 sjpark    (1000) sjpark    (1000)        0 2024-05-27 17:29:03.291275 damo-2.3.6/src/damo.egg-info/
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     7502 2024-05-27 17:29:03.000000 damo-2.3.6/src/damo.egg-info/PKG-INFO
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)     1302 2024-05-27 17:29:03.000000 damo-2.3.6/src/damo.egg-info/SOURCES.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        1 2024-05-27 17:29:03.000000 damo-2.3.6/src/damo.egg-info/dependency_links.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)       40 2024-05-27 17:29:03.000000 damo-2.3.6/src/damo.egg-info/entry_points.txt
+-rw-r--r--   0 sjpark    (1000) sjpark    (1000)        5 2024-05-27 17:29:03.000000 damo-2.3.6/src/damo.egg-info/top_level.txt
```

### Comparing `damo-2.3.5/PKG-INFO` & `damo-2.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 2.3.5
+Version: 2.3.6
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -48,15 +48,15 @@
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The second and last commands will show the access pattern of your workload,
 like below:
 
 ![masim_stairs_snapshot](images/masim_stairs_snapshot.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.5/images/masim_stairs_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.6/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -64,15 +64,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.6/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -92,15 +92,15 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some features are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file?
+Why some features are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.6/USAGE.md) file?
 ------------------------------------------------------------------
 
 Because those are not yet stabilized.  In other words, such features are in
 their experimental stages, and therefore could be deprecated and removed
 without notice and grace periods.  The documented features could also be
 deprecated, but those will provide some notifications and grace periods.  If
 there are some features you're relying on but not documented, please
@@ -115,15 +115,15 @@
 [FEATURES_DEPRECATION_SCHEDULE.md](FEATURES_DEPRECATION_SCHEDULE.md) file.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.6/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.3.5/README.md` & `damo-2.3.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The second and last commands will show the access pattern of your workload,
 like below:
 
 ![masim_stairs_snapshot](images/masim_stairs_snapshot.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.5/images/masim_stairs_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.6/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -49,15 +49,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.6/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -77,15 +77,15 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some features are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file?
+Why some features are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.6/USAGE.md) file?
 ------------------------------------------------------------------
 
 Because those are not yet stabilized.  In other words, such features are in
 their experimental stages, and therefore could be deprecated and removed
 without notice and grace periods.  The documented features could also be
 deprecated, but those will provide some notifications and grace periods.  If
 there are some features you're relying on but not documented, please
@@ -100,15 +100,15 @@
 [FEATURES_DEPRECATION_SCHEDULE.md](FEATURES_DEPRECATION_SCHEDULE.md) file.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.6/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.3.5/setup.py` & `damo-2.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/_damo_ascii_color.py` & `damo-2.3.6/src/damo/_damo_ascii_color.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/_damo_deprecated.py` & `damo-2.3.6/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/_damo_deprecation_notice.py` & `damo-2.3.6/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/_damo_dist.py` & `damo-2.3.6/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/_damo_fmt_str.py` & `damo-2.3.6/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/_damo_fs.py` & `damo-2.3.6/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/_damo_paddr_layout.py` & `damo-2.3.6/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/_damo_print.py` & `damo-2.3.6/src/damo/_damo_print.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/_damo_records.py` & `damo-2.3.6/src/damo/_damo_records.py`

 * *Files 3% similar despite different names*

```diff
@@ -651,14 +651,108 @@
     os.chmod(filepath, file_permission)
 
 def load_mem_footprint(filepath):
     with open(filepath, 'r') as f:
         kvpairs = json.load(f)
     return [MemFootprintsSnapshot.from_kvpairs(x) for x in kvpairs]
 
+class Vma:
+    start = None
+    end = None
+    name = None
+
+    def __init__(self, start, end, name):
+        self.start = start
+        self.end = end
+        self.name = name
+
+    def to_kvpairs(self):
+        return self.__dict__
+
+    @classmethod
+    def from_kvpairs(cls, kvpairs):
+        self = cls(None, None, None)
+        self.start = kvpairs['start']
+        self.end = kvpairs['end']
+        self.name = kvpairs['name']
+
+class ProcVmas:
+    pid = None
+    vmas = None
+
+    def __init__(self, pid):
+        self.pid = pid
+        self.vmas = []
+
+        if pid is None:
+            return
+
+        with open('/proc/%s/maps' % pid, 'r') as f:
+            for line in f:
+                fields = line.split()
+                start, end = [int(addr, 16) for addr in fields[0].split('-')]
+                name = fields[-1]
+                self.vmas.append(Vma(start, end, name))
+
+    def to_kvpairs(self):
+        kvpairs = {'pid': self.pid}
+        kvpairs['vmas'] = [v.to_kvpairs() for v in self.vmas]
+        return kvpairs
+
+    @classmethod
+    def from_kvpairs(cls, kvpairs):
+        self = cls(None)
+        self.pid = kvpairs['pid']
+        self.vmas = [Vma.from_kvpairs(kvp) for kvp in kvpairs['vmas']]
+
+class ProcVmasSnapshot:
+    time = None
+    procvmas = None
+
+    def __init__(self, pids):
+        if pids is None:
+            return
+
+        self.time = time.time()
+        self.procvmas = []
+        for pid in pids:
+            self.procvmas.append(ProcVmas(pid))
+
+    def to_kvpairs(self):
+        kvpairs = {'time': self.time}
+        kvpairs['procvmas'] = [p.to_kvpairs() for p in self.procvmas]
+        return kvpairs
+
+    @classmethod
+    def from_kvpairs(cls, kvpairs):
+        self = cls(None)
+        self.time = kvpairs['time']
+        self.procvmas = [ProcVmas.from_kvpairs(kvp)
+                         for kvp in kvapirs['procvmas']]
+
+def record_proc_vmas(kdamonds, snapshots):
+    pids = []
+    for kdamond in kdamonds:
+        for ctx in kdamond.contexts:
+            for target in ctx.targets:
+                if target.pid is None:
+                    continue
+                pids.append(target.pid)
+    snapshots.append(ProcVmasSnapshot(pids))
+
+def save_proc_vmas(snapshots, filepath, file_permission):
+    with open(filepath, 'w') as f:
+        json.dump([s.to_kvpairs() for s in snapshots], f, indent=4)
+    os.chmod(filepath, file_permission)
+
+def load_proc_vmas(filepath):
+    with open(filepath, 'r') as f:
+        kvpairs = json.load(f)
+    return [ProcVmasSnapshot.from_kvpairs(x) for x in kvpairs]
+
 def add_childs_target(kdamonds):
     current_targets = kdamonds[0].contexts[0].targets
 
     for target in current_targets:
         if target.pid == None:
             continue
         try:
@@ -732,30 +826,36 @@
     perf_profile_pipe = None
 
     # for adding child tasks and memory footprint recording
     kdamonds = None
     add_child_tasks = None
     mem_footprint_snapshots = None
 
+    # for vmas recording
+    vmas_snapshots = None
+
     def __init__(self, tracepoint, file_path, file_format, file_permission,
                  monitoring_intervals,
                  do_profile,
-                 kdamonds, add_child_tasks, record_mem_footprint):
+                 kdamonds, add_child_tasks, record_mem_footprint,
+                 record_vmas=False):
         self.tracepoint = tracepoint
         self.file_path = file_path
         self.file_format = file_format
         self.file_permission = file_permission
         self.monitoring_intervals = monitoring_intervals
 
         self.do_profile = do_profile
 
         self.kdamonds = kdamonds
         self.add_child_tasks = add_child_tasks
         if record_mem_footprint is True:
             self.mem_footprint_snapshots = []
+        if record_vmas is True:
+            self.vmas_snapshots = []
 
 def start_recording(handle):
     if handle.tracepoint is not None:
         handle.perf_pipe = subprocess.Popen(
                 [PERF, 'record', '-a', '-e', handle.tracepoint,
                  '-o', handle.file_path])
     if handle.do_profile:
@@ -765,14 +865,16 @@
            _damon.any_kdamond_running()):
         if handle.add_child_tasks is True:
             add_childs_target(handle.kdamonds)
 
         if handle.mem_footprint_snapshots is not None:
             record_mem_footprint(handle.kdamonds,
                                  handle.mem_footprint_snapshots)
+        if handle.vmas_snapshots is not None:
+            record_proc_vmas(handle.kdamonds, handle.vmas_snapshots)
         time.sleep(1)
 
 def finish_recording(handle):
     try:
         handle.perf_pipe.send_signal(signal.SIGINT)
         handle.perf_pipe.wait()
     except:
@@ -796,14 +898,17 @@
             pass
         os.chmod('%s.profile' % handle.file_path, handle.file_permission)
 
     if handle.mem_footprint_snapshots is not None:
         save_mem_footprint(
                 handle.mem_footprint_snapshots,
                 '%s.mem_footprint' % handle.file_path, handle.file_permission)
+    if handle.vmas_snapshots is not None:
+        save_proc_vmas(handle.vmas_snapshots, '%s.vmas' % handle.file_path,
+                       handle.file_permission)
 
 # for snapshot
 
 def find_install_scheme(scheme_to_find):
     '''Install given scheme to all contexts if effectively same scheme is not
     installed.
     Returns whether it found a context doesn't having the scheme, indices list
```

### Comparing `damo-2.3.5/src/damo/_damo_subcmds.py` & `damo-2.3.6/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/_damon.py` & `damo-2.3.6/src/damo/_damon.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/_damon_args.py` & `damo-2.3.6/src/damo/_damon_args.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/_damon_dbgfs.py` & `damo-2.3.6/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/_damon_sysfs.py` & `damo-2.3.6/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo.py` & `damo-2.3.6/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_adjust.py` & `damo-2.3.6/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_convert_record_format.py` & `damo-2.3.6/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_features.py` & `damo-2.3.6/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_fmt_json.py` & `damo-2.3.6/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_heats.py` & `damo-2.3.6/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_lru_sort.py` & `damo-2.3.6/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_monitor.py` & `damo-2.3.6/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_nr_regions.py` & `damo-2.3.6/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_reclaim.py` & `damo-2.3.6/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_record.py` & `damo-2.3.6/src/damo/damo_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,16 @@
             file_format=args.output_type,
             file_permission=args.output_permission,
             monitoring_intervals=monitoring_intervals,
             # for perf profile
             do_profile=args.profile is True,
             # for childs recording and memory footprint
             kdamonds=kdamonds, add_child_tasks=args.include_child_tasks,
-            record_mem_footprint=args.footprint)
+            record_mem_footprint=args.footprint,
+            record_vmas=args.vmas)
     data_for_cleanup.record_handle = record_handle
 
     print('Press Ctrl+C to stop')
     _damo_records.start_recording(record_handle)
     cleanup_exit(0)
 
 def set_argparser(parser):
@@ -148,9 +149,11 @@
     parser.add_argument('--profile', action='store_true',
                         help='record profiling information together')
     parser.add_argument('--no_footprint', action='store_false',
                         dest='footprint',
                         help='do not record memory footprint')
     parser.add_argument('--footprint', action='store_true',
                         help='record memory footprint')
+    parser.add_argument('--vmas', action='store_true',
+                        help='record virtual memory areas (/proc/<pid>/maps)')
     parser.description = 'Record monitoring results'
     return parser
```

### Comparing `damo-2.3.5/src/damo/damo_record_info.py` & `damo-2.3.6/src/damo/damo_record_info.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_replay.py` & `damo-2.3.6/src/damo/damo_replay.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_report.py` & `damo-2.3.6/src/damo/damo_report.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
 import _damo_subcmds
+import damo_heatmap
 import damo_heats
 import damo_nr_regions
 import damo_report_footprint
 import damo_report_profile
 import damo_report_raw
 import damo_report_times
 import damo_wss
 
 subcmds = [
         _damo_subcmds.DamoSubCmd(name='raw', module=damo_report_raw,
             msg='human readable raw data'),
+        _damo_subcmds.DamoSubCmd(name='heatmap', module=damo_heatmap,
+            msg='heatmap of access patterns'),
         _damo_subcmds.DamoSubCmd(name='heats', module=damo_heats,
             msg='heats of regions'),
         _damo_subcmds.DamoSubCmd(name='wss', module=damo_wss,
             msg='working set size'),
         _damo_subcmds.DamoSubCmd(name='nr_regions', module=damo_nr_regions,
             msg='number of regions'),
         _damo_subcmds.DamoSubCmd(name='profile', module=damo_report_profile,
```

### Comparing `damo-2.3.5/src/damo/damo_report_footprint.py` & `damo-2.3.6/src/damo/damo_report_footprint.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_report_profile.py` & `damo-2.3.6/src/damo/damo_report_profile.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_report_raw.py` & `damo-2.3.6/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_report_times.py` & `damo-2.3.6/src/damo/damo_report_times.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_schemes.py` & `damo-2.3.6/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_show.py` & `damo-2.3.6/src/damo/damo_show.py`

 * *Files 5% similar despite different names*

```diff
@@ -417,36 +417,43 @@
             args.format_region = '<box>%s' % default_region_format
         else:
             args.format_region = '<box>\n%s' % default_region_format
         if args.format_snapshot_tail.find('<region box description>') == -1:
             args.format_snapshot_tail = ('%s\n<region box description>' %
                     args.format_record_tail)
 
-def temperature_of(region):
+def temperature_of(region, weights):
+    sz_weight, access_rate_weight, age_weight = weights
+    sz_score = region.size() * sz_weight
+    ar_score = region.nr_accesses.percent * access_rate_weight
+    age_score = region.age.usec * age_weight
+    score = sz_score + ar_score + age_score
+
     if region.nr_accesses.percent > 0:
-        return region.nr_accesses.percent * region.age.usec
+        return score
     else:
-        return -1 * region.age.usec
+        return -1 * score
 
-def sorted_regions(regions, sort_fields, sort_dsc_keys):
+def sorted_regions(regions, sort_fields, sort_dsc_keys, temperature_weights):
     for field in sort_fields:
         dsc = sort_dsc_keys != None and ('all' in sort_dsc_keys or
                                          field in sort_dsc_keys)
         if field == 'address':
             regions = sorted(regions, key=lambda r: r.start, reverse=dsc)
         elif field == 'access_rate':
             regions = sorted(regions, key=lambda r: r.nr_accesses.percent,
                     reverse=dsc)
         elif field == 'age':
             regions = sorted(regions, key=lambda r: r.age.usec, reverse=dsc)
         elif field == 'size':
             regions = sorted(regions, key=lambda r: r.size(), reverse=dsc)
         elif field == 'temperature':
-            regions = sorted(regions, key=lambda r: temperature_of(r),
-                             reverse=dsc)
+            regions = sorted(
+                    regions, reverse=dsc,
+                    key=lambda r: temperature_of(r, temperature_weights))
     return regions
 
 def pr_records(args, records):
     if args.json:
         _damo_print.pr_with_pager_if_needed(
                 json.dumps([r.to_kvpairs(args.raw_number) for r in records],
                            indent=4))
@@ -481,15 +488,15 @@
                         args.min_chars_for, args.raw_number, region_box_args,
                         record, snapshot))
             for r in snapshot.regions:
                 r.nr_accesses.add_unset_unit(record.intervals)
                 r.age.add_unset_unit(record.intervals)
             for idx, r in enumerate(
                     sorted_regions(snapshot.regions, args.sort_regions_by,
-                        args.sort_regions_dsc)):
+                        args.sort_regions_dsc, args.temperature_weights)):
                 outputs.append(
                         format_output(
                             args.format_region, region_formatters,
                             args.min_chars_for, args.raw_number,
                             region_box_args, record, snapshot, r, idx))
             outputs.append(
                     format_output(
@@ -587,14 +594,20 @@
             default=['address'],
             help='fields to sort regions by')
     parser.add_argument('--sort_regions_dsc',
             choices=['address', 'access_rate', 'age', 'size', 'temperature',
                      'all'],
             nargs='+',
             help='sort regions in descending order for the given keys')
+    parser.add_argument(
+            '--temperature_weights', type=int, metavar='<int>', nargs=3,
+            default=[0, 100, 100],
+            help=' '.join(
+                ['temperature weights for size, access rate, and age',
+                 'of each region']))
     parser.add_argument('--dont_merge_regions', action='store_true',
             help='don\'t merge contiguous regions of same access pattern')
 
     # don't set default for record head and snapshot head because it depends on
     # given number of record and snapshots.  Decide those in set_formats().
     parser.add_argument('--format_record_head', metavar='<template>',
             help='output format to show at the beginning of each record')
```

### Comparing `damo-2.3.5/src/damo/damo_start.py` & `damo-2.3.6/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_status.py` & `damo-2.3.6/src/damo/damo_status.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_stop.py` & `damo-2.3.6/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_tune.py` & `damo-2.3.6/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_validate.py` & `damo-2.3.6/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo/damo_wss.py` & `damo-2.3.6/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-2.3.5/src/damo.egg-info/PKG-INFO` & `damo-2.3.6/src/damo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 2.3.5
+Version: 2.3.6
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -48,15 +48,15 @@
     $ sudo damo record $(pidof <your workload>)
     $ sudo damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The second and last commands will show the access pattern of your workload,
 like below:
 
 ![masim_stairs_snapshot](images/masim_stairs_snapshot.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.5/images/masim_stairs_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v2.3.6/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I ensure DAMON is enabled on my kernel?
 -----------------------------------------------
@@ -64,15 +64,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.6/USAGE.md) file.
 
 
 What does the version numbers mean?
 -----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -92,15 +92,15 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some features are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file?
+Why some features are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.6/USAGE.md) file?
 ------------------------------------------------------------------
 
 Because those are not yet stabilized.  In other words, such features are in
 their experimental stages, and therefore could be deprecated and removed
 without notice and grace periods.  The documented features could also be
 deprecated, but those will provide some notifications and grace periods.  If
 there are some features you're relying on but not documented, please
@@ -115,15 +115,15 @@
 [FEATURES_DEPRECATION_SCHEDULE.md](FEATURES_DEPRECATION_SCHEDULE.md) file.
 
 
 Quick Intro for Major Features
 ==============================
 
 Below are quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.5/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v2.3.6/USAGE.md) file.
 
 
 Snapshot Data Access Pattern
 ----------------------------
 
 Below commands repeatedly get a snapshot of the access pattern of a program for
 every second.
```

### Comparing `damo-2.3.5/src/damo.egg-info/SOURCES.txt` & `damo-2.3.6/src/damo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/damo/_damon_dbgfs.py
 src/damo/_damon_sysfs.py
 src/damo/damo.py
 src/damo/damo_adjust.py
 src/damo/damo_convert_record_format.py
 src/damo/damo_features.py
 src/damo/damo_fmt_json.py
+src/damo/damo_heatmap.py
 src/damo/damo_heats.py
 src/damo/damo_lru_sort.py
 src/damo/damo_monitor.py
 src/damo/damo_nr_regions.py
 src/damo/damo_reclaim.py
 src/damo/damo_record.py
 src/damo/damo_record_info.py
```

