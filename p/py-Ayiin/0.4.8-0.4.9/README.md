# Comparing `tmp/py-Ayiin-0.4.8.tar.gz` & `tmp/py_Ayiin-0.4.9-cp39-cp39-manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.4.8.tar", last modified: Wed Aug  9 13:26:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

