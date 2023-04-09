# Comparing `tmp/pyzw-0.0.5.tar.gz` & `tmp/pyzw-0.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzw-0.0.5.tar", last modified: Sun Apr  9 06:37:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

