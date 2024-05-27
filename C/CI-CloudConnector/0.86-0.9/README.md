# Comparing `tmp/ci_cloudconnector-0.86.tar.gz` & `tmp/CI_CloudConnector-0.9.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-0.86.tar", last modified: Mon May 27 13:48:30 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
