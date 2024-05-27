# Comparing `tmp/drf-tus-2.0.1.tar.gz` & `tmp/drf_tus-2.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-tus-2.0.1.tar", last modified: Fri Oct 13 09:32:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

