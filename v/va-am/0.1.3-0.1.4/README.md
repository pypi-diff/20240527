# Comparing `tmp/va_am-0.1.3.tar.gz` & `tmp/va_am-0.1.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "va_am-0.1.3.tar", last modified: Fri May 10 08:18:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

