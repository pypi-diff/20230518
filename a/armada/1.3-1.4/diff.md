# Comparing `tmp/armada-1.3.tar.gz` & `tmp/armada-1.4-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/armada-1.3.tar", last modified: Mon Oct 29 13:33:40 2018, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

