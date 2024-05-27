# Comparing `tmp/beam-ds-2.5.0b0.tar.gz` & `tmp/beam_ds-2.5.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beam-ds-2.5.0b0.tar", last modified: Sun Mar 31 08:51:27 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

