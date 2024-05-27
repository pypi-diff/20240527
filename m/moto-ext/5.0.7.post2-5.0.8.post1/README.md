# Comparing `tmp/moto_ext-5.0.7.post2.tar.gz` & `tmp/moto_ext-5.0.8.post1-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moto_ext-5.0.7.post2.tar", last modified: Wed May 22 12:16:37 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

