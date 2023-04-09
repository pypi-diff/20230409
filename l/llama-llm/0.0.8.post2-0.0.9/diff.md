# Comparing `tmp/llama-llm-0.0.8.post2.tar.gz` & `tmp/llama_llm-0.0.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama-llm-0.0.8.post2.tar", last modified: Tue Feb 28 18:34:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

