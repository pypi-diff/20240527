# Comparing `tmp/special-octo-robot-0.0.7.tar.gz` & `tmp/special_octo_robot-0.0.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "special-octo-robot-0.0.7.tar", last modified: Fri Apr 12 07:41:09 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

