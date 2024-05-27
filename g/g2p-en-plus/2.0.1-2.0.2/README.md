# Comparing `tmp/g2p_en_plus-2.0.1.tar.gz` & `tmp/g2p_en_plus-2.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2p_en_plus-2.0.1.tar", last modified: Thu Apr 18 03:47:20 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

## Comparing `g2p_en_plus-2.0.1.tar` & `g2p_en_plus/checkpoint20.npz`

 * *Files 21% similar despite different names*

### file list

```diff
@@ -1,19 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 03:47:20.433586 g2p_en_plus-2.0.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-18 03:02:21.000000 g2p_en_plus-2.0.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       71 2024-04-18 03:02:39.000000 g2p_en_plus-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4439 2024-04-18 03:47:20.433586 g2p_en_plus-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4003 2024-04-18 03:02:21.000000 g2p_en_plus-2.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 03:47:20.433586 g2p_en_plus-2.0.1/g2p_en_plus/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-18 03:02:21.000000 g2p_en_plus-2.0.1/g2p_en_plus/__init__.py
--rw-r--r--   0 root         (0) root         (0)  3342298 2024-04-18 03:02:21.000000 g2p_en_plus-2.0.1/g2p_en_plus/checkpoint20.npz
--rw-r--r--   0 root         (0) root         (0)     2492 2024-04-18 03:02:21.000000 g2p_en_plus-2.0.1/g2p_en_plus/expand.py
--rw-r--r--   0 root         (0) root         (0)     9308 2024-04-18 03:02:21.000000 g2p_en_plus-2.0.1/g2p_en_plus/g2p.py
--rw-r--r--   0 root         (0) root         (0)    18711 2024-04-18 03:02:21.000000 g2p_en_plus-2.0.1/g2p_en_plus/homographs.en
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 03:47:20.433586 g2p_en_plus-2.0.1/g2p_en_plus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4439 2024-04-18 03:47:20.000000 g2p_en_plus-2.0.1/g2p_en_plus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      347 2024-04-18 03:47:20.000000 g2p_en_plus-2.0.1/g2p_en_plus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 03:47:20.000000 g2p_en_plus-2.0.1/g2p_en_plus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-04-18 03:47:20.000000 g2p_en_plus-2.0.1/g2p_en_plus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-18 03:47:20.000000 g2p_en_plus-2.0.1/g2p_en_plus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-04-18 03:47:20.433586 g2p_en_plus-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      921 2024-04-18 03:47:14.000000 g2p_en_plus-2.0.1/setup.py
+-rw-------   0        0        0    29824 1980-01-01 00:00:00.000000 enc_emb.npy
+-rw-------   0        0        0   786560 1980-01-01 00:00:00.000000 enc_w_ih.npy
+-rw-------   0        0        0   786560 1980-01-01 00:00:00.000000 enc_w_hh.npy
+-rw-------   0        0        0     3200 1980-01-01 00:00:00.000000 enc_b_ih.npy
+-rw-------   0        0        0     3200 1980-01-01 00:00:00.000000 enc_b_hh.npy
+-rw-------   0        0        0    75904 1980-01-01 00:00:00.000000 dec_emb.npy
+-rw-------   0        0        0   786560 1980-01-01 00:00:00.000000 dec_w_ih.npy
+-rw-------   0        0        0   786560 1980-01-01 00:00:00.000000 dec_w_hh.npy
+-rw-------   0        0        0     3200 1980-01-01 00:00:00.000000 dec_b_ih.npy
+-rw-------   0        0        0     3200 1980-01-01 00:00:00.000000 dec_b_hh.npy
+-rw-------   0        0        0    75904 1980-01-01 00:00:00.000000 fc_w.npy
+-rw-------   0        0        0      424 1980-01-01 00:00:00.000000 fc_b.npy
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+Zip archive data, at least v2.0 to extract, compression method=store
```

### filetype from diffoscope

```diff
@@ -1 +1 @@
-TarFile
+ZipFile
```

