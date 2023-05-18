# Comparing `tmp/JBPhD-2.1.7.tar.gz` & `tmp/JBPhD-2.1.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBPhD-2.1.7.tar", last modified: Mon May 15 21:30:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

