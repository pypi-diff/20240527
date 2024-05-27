# Comparing `tmp/wdbo_criterion-2.0.0-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/wdbo_criterion-2.1.0-cp310-cp310-musllinux_1_1_i686.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,13 @@
-Zip file size: 58364 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat   120320 b- defN 24-May-15 23:56 wdbo_criterion.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat      375 b- defN 24-May-15 23:56 wdbo_criterion-2.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 24-May-15 23:56 wdbo_criterion-2.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-May-15 23:56 wdbo_criterion-2.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      425 b- defN 24-May-15 23:56 wdbo_criterion-2.0.0.dist-info/RECORD
-5 files, 121242 bytes uncompressed, 57570 bytes compressed:  52.5%
+Zip file size: 912214 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 19:27 wdbo_criterion.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-27 19:27 wdbo_criterion-2.1.0.dist-info/
+-rwxr-xr-x  2.0 unx   337669 b- defN 24-May-27 19:27 libwdbo_bayesian.so
+-rwxr-xr-x  2.0 unx   194841 b- defN 24-May-27 19:27 wdbo_criterion.cpython-310-i386-linux-gnu.so
+-rw-r--r--  2.0 unx   101649 b- defN 24-May-27 19:27 wdbo_criterion.libs/libgcc_s-8b50eaaa.so.1
+-rwxr-xr-x  2.0 unx  2428961 b- defN 24-May-27 19:27 wdbo_criterion.libs/libstdc++-8baf04f9.so.6.0.28
+-rwxr-xr-x  2.0 unx   337413 b- defN 24-May-27 19:27 wdbo_criterion.libs/libwdbo_bayesian-170bea1d.so
+-rw-r--r--  2.0 unx      111 b- defN 24-May-27 19:27 wdbo_criterion-2.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-27 19:27 wdbo_criterion-2.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      832 b- defN 24-May-27 19:27 wdbo_criterion-2.1.0.dist-info/RECORD
+-rw-r--r--  2.0 unx      316 b- defN 24-May-27 19:27 wdbo_criterion-2.1.0.dist-info/METADATA
+11 files, 3401807 bytes uncompressed, 910540 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -1,16 +1,34 @@
-Filename: wdbo_criterion.pypy39-pp73-win_amd64.pyd
+Filename: wdbo_criterion.libs/
 Comment: 
 
-Filename: wdbo_criterion-2.0.0.dist-info/METADATA
+Filename: wdbo_criterion-2.1.0.dist-info/
 Comment: 
 
-Filename: wdbo_criterion-2.0.0.dist-info/WHEEL
+Filename: libwdbo_bayesian.so
 Comment: 
 
-Filename: wdbo_criterion-2.0.0.dist-info/top_level.txt
+Filename: wdbo_criterion.cpython-310-i386-linux-gnu.so
 Comment: 
 
-Filename: wdbo_criterion-2.0.0.dist-info/RECORD
+Filename: wdbo_criterion.libs/libgcc_s-8b50eaaa.so.1
+Comment: 
+
+Filename: wdbo_criterion.libs/libstdc++-8baf04f9.so.6.0.28
+Comment: 
+
+Filename: wdbo_criterion.libs/libwdbo_bayesian-170bea1d.so
+Comment: 
+
+Filename: wdbo_criterion-2.1.0.dist-info/WHEEL
+Comment: 
+
+Filename: wdbo_criterion-2.1.0.dist-info/top_level.txt
+Comment: 
+
+Filename: wdbo_criterion-2.1.0.dist-info/RECORD
+Comment: 
+
+Filename: wdbo_criterion-2.1.0.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

