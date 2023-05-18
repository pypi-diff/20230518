# Comparing `tmp/cpi_tools-0.0.2.tar.gz` & `tmp/cpi_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpi_tools-0.0.2.tar", last modified: Thu Jan 26 18:20:41 2023, max compression
+gzip compressed data, was "cpi_tools-0.0.3.tar", last modified: Fri Jan 27 17:00:13 2023, max compression
```

## Comparing `cpi_tools-0.0.2.tar` & `cpi_tools-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-01-26 18:20:41.226553 cpi_tools-0.0.2/
--rw-rw-rw-   0        0        0     1074 2023-01-26 16:53:27.000000 cpi_tools-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       89 2023-01-26 16:53:27.000000 cpi_tools-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      902 2023-01-26 18:20:41.226553 cpi_tools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-01-26 18:05:14.000000 cpi_tools-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-01-26 18:20:41.210549 cpi_tools-0.0.2/cpi_tools/
--rw-rw-rw-   0        0        0        0 2023-01-26 16:53:26.000000 cpi_tools-0.0.2/cpi_tools/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-01-26 18:02:41.000000 cpi_tools-0.0.2/cpi_tools/aws_tools.py
-drwxrwxrwx   0        0        0        0 2023-01-26 18:20:41.226553 cpi_tools-0.0.2/cpi_tools.egg-info/
--rw-rw-rw-   0        0        0      902 2023-01-26 18:20:41.000000 cpi_tools-0.0.2/cpi_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-01-26 18:20:41.000000 cpi_tools-0.0.2/cpi_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-26 18:20:41.000000 cpi_tools-0.0.2/cpi_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-01-26 18:20:41.000000 cpi_tools-0.0.2/cpi_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-01-26 16:53:27.000000 cpi_tools-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      566 2023-01-26 18:20:41.234553 cpi_tools-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-01-27 17:00:13.920125 cpi_tools-0.0.3/
+-rw-rw-rw-   0        0        0     1074 2023-01-26 16:53:27.000000 cpi_tools-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-01-27 16:40:16.000000 cpi_tools-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      941 2023-01-27 17:00:13.920125 cpi_tools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-01-27 16:58:15.000000 cpi_tools-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-01-27 17:00:13.896388 cpi_tools-0.0.3/cpi_tools/
+-rw-rw-rw-   0        0        0        0 2023-01-26 16:53:26.000000 cpi_tools-0.0.3/cpi_tools/__init__.py
+-rw-rw-rw-   0        0        0     2375 2023-01-27 16:56:14.000000 cpi_tools-0.0.3/cpi_tools/aws_tools.py
+drwxrwxrwx   0        0        0        0 2023-01-27 17:00:13.912127 cpi_tools-0.0.3/cpi_tools.egg-info/
+-rw-rw-rw-   0        0        0      941 2023-01-27 17:00:13.000000 cpi_tools-0.0.3/cpi_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-01-27 17:00:13.000000 cpi_tools-0.0.3/cpi_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-27 17:00:13.000000 cpi_tools-0.0.3/cpi_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-01-27 17:00:13.000000 cpi_tools-0.0.3/cpi_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-01-27 16:46:45.000000 cpi_tools-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      566 2023-01-27 17:00:13.928126 cpi_tools-0.0.3/setup.cfg
```

### Comparing `cpi_tools-0.0.2/LICENSE` & `cpi_tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.0.2/PKG-INFO` & `cpi_tools-0.0.3/cpi_tools.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cpi_tools
-Version: 0.0.2
+Name: cpi-tools
+Version: 0.0.3
 Summary: Repository of functions used across CPI
 Home-page: https://github.com/climatepolicydata/cpi_tools
 Author: Jake Connolly
 Author-email: datascience@cpiglobal.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,17 +26,20 @@
 
 AWS Tools
 
 ```python
 from cpi_tools import aws_tools
 
 #S3 Bucket
-afolu_bucket = 'cpi-afolu-landscape'
+bucket = 'YOUR_BUCKET'
 #Path within S3
-path = 'entity_name_data'
+path = 'PATH_IN_BUCKET'
 #S3 File name 
-file_name = 'afolu_entity_list.csv'
+file_name = 'FILE_NAME'
 
 #Read file from S3
-df = aws_tools.read_from_s3(afolu_bucket, path, file_name)
+df = aws_tools.read_from_s3(bucket, path, file_name)
+
+#Write file to S3
+aws_tools.write_to_s3(df, bucket, path, file_name)
 ```
```

### Comparing `cpi_tools-0.0.2/cpi_tools.egg-info/PKG-INFO` & `cpi_tools-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cpi-tools
-Version: 0.0.2
+Name: cpi_tools
+Version: 0.0.3
 Summary: Repository of functions used across CPI
 Home-page: https://github.com/climatepolicydata/cpi_tools
 Author: Jake Connolly
 Author-email: datascience@cpiglobal.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,17 +26,20 @@
 
 AWS Tools
 
 ```python
 from cpi_tools import aws_tools
 
 #S3 Bucket
-afolu_bucket = 'cpi-afolu-landscape'
+bucket = 'YOUR_BUCKET'
 #Path within S3
-path = 'entity_name_data'
+path = 'PATH_IN_BUCKET'
 #S3 File name 
-file_name = 'afolu_entity_list.csv'
+file_name = 'FILE_NAME'
 
 #Read file from S3
-df = aws_tools.read_from_s3(afolu_bucket, path, file_name)
+df = aws_tools.read_from_s3(bucket, path, file_name)
+
+#Write file to S3
+aws_tools.write_to_s3(df, bucket, path, file_name)
 ```
```

### Comparing `cpi_tools-0.0.2/setup.cfg` & `cpi_tools-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 7069 5f74 6f6f 6c73 0d0a 7665   = cpi_tools..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 320d 0a61  rsion = 0.0.2..a
+00000020: 7273 696f 6e20 3d20 302e 302e 330d 0a61  rsion = 0.0.3..a
 00000030: 7574 686f 7220 3d20 4a61 6b65 2043 6f6e  uthor = Jake Con
 00000040: 6e6f 6c6c 790d 0a61 7574 686f 725f 656d  nolly..author_em
 00000050: 6169 6c20 3d20 6461 7461 7363 6965 6e63  ail = datascienc
 00000060: 6540 6370 6967 6c6f 6261 6c2e 6f72 670d  e@cpiglobal.org.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2052  .description = R
 00000080: 6570 6f73 6974 6f72 7920 6f66 2066 756e  epository of fun
 00000090: 6374 696f 6e73 2075 7365 6420 6163 726f  ctions used acro
```

