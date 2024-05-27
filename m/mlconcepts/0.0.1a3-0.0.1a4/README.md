# Comparing `tmp/mlconcepts-0.0.1a3.tar.gz` & `tmp/mlconcepts-0.0.1a4-cp311-cp311-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlconcepts-0.0.1a3.tar", last modified: Fri May 24 15:55:13 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

