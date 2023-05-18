# Comparing `tmp/imageTable-0.1.2.tar.gz` & `tmp/imageTable-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imageTable-0.1.2.tar", last modified: Thu May 18 01:15:10 2023, max compression
+gzip compressed data, was "imageTable-0.1.3.tar", last modified: Thu May 18 01:20:34 2023, max compression
```

## Comparing `imageTable-0.1.2.tar` & `imageTable-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:15:10.748750 imageTable-0.1.2/
--rw-r--r--   0 kevin      (501) staff       (20)      210 2023-05-18 01:15:10.748181 imageTable-0.1.2/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)       38 2023-05-18 01:15:10.749111 imageTable-0.1.2/setup.cfg
--rw-r--r--   0 kevin      (501) staff       (20)      685 2023-05-18 01:14:51.000000 imageTable-0.1.2/setup.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:15:10.741109 imageTable-0.1.2/src/
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:15:10.744330 imageTable-0.1.2/src/imageTable/
--rw-rw-r--   0 kevin      (501) staff       (20)       70 2023-05-18 01:14:23.000000 imageTable-0.1.2/src/imageTable/__init__.py
--rwxr--r--   0 kevin      (501) staff       (20)     1201 2023-05-18 01:05:01.000000 imageTable-0.1.2/src/imageTable/image2csv.py
--rwxr-xr-x   0 kevin      (501) staff       (20)     4592 2023-05-17 23:08:13.000000 imageTable-0.1.2/src/imageTable/imageTable.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:15:10.747392 imageTable-0.1.2/src/imageTable.egg-info/
--rw-r--r--   0 kevin      (501) staff       (20)      210 2023-05-18 01:15:10.000000 imageTable-0.1.2/src/imageTable.egg-info/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)      281 2023-05-18 01:15:10.000000 imageTable-0.1.2/src/imageTable.egg-info/SOURCES.txt
--rw-r--r--   0 kevin      (501) staff       (20)        1 2023-05-18 01:15:10.000000 imageTable-0.1.2/src/imageTable.egg-info/dependency_links.txt
--rw-r--r--   0 kevin      (501) staff       (20)       44 2023-05-18 01:15:10.000000 imageTable-0.1.2/src/imageTable.egg-info/requires.txt
--rw-r--r--   0 kevin      (501) staff       (20)       11 2023-05-18 01:15:10.000000 imageTable-0.1.2/src/imageTable.egg-info/top_level.txt
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:20:34.066815 imageTable-0.1.3/
+-rw-r--r--   0 kevin      (501) staff       (20)      210 2023-05-18 01:20:34.066317 imageTable-0.1.3/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)       38 2023-05-18 01:20:34.066996 imageTable-0.1.3/setup.cfg
+-rw-r--r--   0 kevin      (501) staff       (20)      685 2023-05-18 01:19:57.000000 imageTable-0.1.3/setup.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:20:34.057964 imageTable-0.1.3/src/
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:20:34.059775 imageTable-0.1.3/src/imageTable/
+-rw-rw-r--   0 kevin      (501) staff       (20)       70 2023-05-18 01:14:23.000000 imageTable-0.1.3/src/imageTable/__init__.py
+-rwxr--r--   0 kevin      (501) staff       (20)     1212 2023-05-18 01:19:38.000000 imageTable-0.1.3/src/imageTable/image2csv.py
+-rwxr-xr-x   0 kevin      (501) staff       (20)     4592 2023-05-17 23:08:13.000000 imageTable-0.1.3/src/imageTable/imageTable.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-18 01:20:34.065146 imageTable-0.1.3/src/imageTable.egg-info/
+-rw-r--r--   0 kevin      (501) staff       (20)      210 2023-05-18 01:20:34.000000 imageTable-0.1.3/src/imageTable.egg-info/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)      281 2023-05-18 01:20:34.000000 imageTable-0.1.3/src/imageTable.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin      (501) staff       (20)        1 2023-05-18 01:20:34.000000 imageTable-0.1.3/src/imageTable.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       44 2023-05-18 01:20:34.000000 imageTable-0.1.3/src/imageTable.egg-info/requires.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       11 2023-05-18 01:20:34.000000 imageTable-0.1.3/src/imageTable.egg-info/top_level.txt
```

### Comparing `imageTable-0.1.2/setup.py` & `imageTable-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from warnings import warn
 
 if sys.version_info.major != 3:
     raise RuntimeError('imageTable requires Python 3')
 
 
 setup(name='imageTable',
-      version='0.1.2',
+      version='0.1.3',
       description='manipulation of czi and ims files',
       author='',
       author_email='',
       package_dir={'': 'src'},
       packages=['imageTable'],
       install_requires=[
           'numpy',
```

### Comparing `imageTable-0.1.2/src/imageTable/image2csv.py` & `imageTable-0.1.3/src/imageTable/image2csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,14 @@
 		raise
 
 
 def main(args: list = None):
 	args = parse_args(args)
 	print(args)
 	try:
-		imageTable.image2table(file_name=args.filename, outfile=args.output_file)
+		imageTable.imageTable.image2table(file_name=args.filename, outfile=args.output_file)
 
 	except:
 		raise
 
 if __name__ == '__main__':
 	main(sys.argv[1:])
```

### Comparing `imageTable-0.1.2/src/imageTable/imageTable.py` & `imageTable-0.1.3/src/imageTable/imageTable.py`

 * *Files identical despite different names*

