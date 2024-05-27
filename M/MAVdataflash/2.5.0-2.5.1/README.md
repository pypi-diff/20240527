# Comparing `tmp/MAVdataflash-2.5.0.tar.gz` & `tmp/MAVdataflash-2.5.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MAVdataflash-2.5.0.tar", last modified: Tue Sep 26 06:38:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

