# Comparing `tmp/testlala-2.0.0.tar.gz` & `tmp/testlala-3.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testlala-2.0.0.tar", last modified: Mon May 27 10:44:11 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

