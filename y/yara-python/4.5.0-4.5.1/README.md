# Comparing `tmp/yara-python-4.5.0.tar.gz` & `tmp/yara_python-4.5.1-cp310-cp310-macosx_10_9_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yara-python-4.5.0.tar", last modified: Tue Mar 26 17:40:34 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

