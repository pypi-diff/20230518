# Comparing `tmp/fasttreeshap-0.1.3.tar.gz` & `tmp/fasttreeshap-0.1.4-cp39-cp39-macosx_12_0_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttreeshap-0.1.3.tar", last modified: Tue Nov 29 01:40:47 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

