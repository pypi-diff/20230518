# Comparing `tmp/markdown-emdash-0.1.0.tar.gz` & `tmp/markdown-emdash-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/markdown-emdash-0.1.0.tar", last modified: Tue Feb 27 14:11:53 2018, max compression
+gzip compressed data, was "markdown-emdash-0.2.0.tar", last modified: Thu May 18 13:13:55 2023, max compression
```

## Comparing `markdown-emdash-0.1.0.tar` & `markdown-emdash-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 czue      (1000) czue      (1000)        0 2018-02-27 14:11:53.000000 markdown-emdash-0.1.0/
--rw-rw-r--   0 czue      (1000) czue      (1000)       38 2018-02-27 14:11:53.000000 markdown-emdash-0.1.0/setup.cfg
--rw-rw-r--   0 czue      (1000) czue      (1000)     1065 2018-02-27 13:40:35.000000 markdown-emdash-0.1.0/LICENSE
--rw-rw-r--   0 czue      (1000) czue      (1000)      716 2018-02-27 14:05:06.000000 markdown-emdash-0.1.0/mdx_emdash.py
--rw-rw-r--   0 czue      (1000) czue      (1000)     1510 2018-02-27 14:11:53.000000 markdown-emdash-0.1.0/PKG-INFO
--rw-rw-r--   0 czue      (1000) czue      (1000)       34 2018-02-27 13:44:57.000000 markdown-emdash-0.1.0/MANIFEST.in
-drwxrwxr-x   0 czue      (1000) czue      (1000)        0 2018-02-27 14:11:53.000000 markdown-emdash-0.1.0/markdown_emdash.egg-info/
--rw-rw-r--   0 czue      (1000) czue      (1000)      208 2018-02-27 14:11:53.000000 markdown-emdash-0.1.0/markdown_emdash.egg-info/SOURCES.txt
--rw-rw-r--   0 czue      (1000) czue      (1000)        1 2018-02-27 14:11:53.000000 markdown-emdash-0.1.0/markdown_emdash.egg-info/dependency_links.txt
--rw-rw-r--   0 czue      (1000) czue      (1000)       11 2018-02-27 14:11:53.000000 markdown-emdash-0.1.0/markdown_emdash.egg-info/top_level.txt
--rw-rw-r--   0 czue      (1000) czue      (1000)     1510 2018-02-27 14:11:53.000000 markdown-emdash-0.1.0/markdown_emdash.egg-info/PKG-INFO
--rw-rw-r--   0 czue      (1000) czue      (1000)      492 2018-02-27 14:07:01.000000 markdown-emdash-0.1.0/README.md
--rw-rw-r--   0 czue      (1000) czue      (1000)     1373 2018-02-27 14:11:41.000000 markdown-emdash-0.1.0/setup.py
+drwxrwxr-x   0 czue      (1000) czue      (1000)        0 2023-05-18 13:13:55.000108 markdown-emdash-0.2.0/
+-rw-rw-r--   0 czue      (1000) czue      (1000)     1065 2023-05-18 13:01:44.000000 markdown-emdash-0.2.0/LICENSE
+-rw-rw-r--   0 czue      (1000) czue      (1000)       34 2023-05-18 13:01:44.000000 markdown-emdash-0.2.0/MANIFEST.in
+-rw-rw-r--   0 czue      (1000) czue      (1000)     1313 2023-05-18 13:13:55.000108 markdown-emdash-0.2.0/PKG-INFO
+-rw-rw-r--   0 czue      (1000) czue      (1000)      496 2023-05-18 13:01:44.000000 markdown-emdash-0.2.0/README.md
+drwxrwxr-x   0 czue      (1000) czue      (1000)        0 2023-05-18 13:13:55.000108 markdown-emdash-0.2.0/markdown_emdash.egg-info/
+-rw-rw-r--   0 czue      (1000) czue      (1000)     1313 2023-05-18 13:13:54.000000 markdown-emdash-0.2.0/markdown_emdash.egg-info/PKG-INFO
+-rw-rw-r--   0 czue      (1000) czue      (1000)      208 2023-05-18 13:13:54.000000 markdown-emdash-0.2.0/markdown_emdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 czue      (1000) czue      (1000)        1 2023-05-18 13:13:54.000000 markdown-emdash-0.2.0/markdown_emdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 czue      (1000) czue      (1000)       11 2023-05-18 13:13:54.000000 markdown-emdash-0.2.0/markdown_emdash.egg-info/top_level.txt
+-rw-rw-r--   0 czue      (1000) czue      (1000)      699 2023-05-18 13:08:58.000000 markdown-emdash-0.2.0/mdx_emdash.py
+-rw-rw-r--   0 czue      (1000) czue      (1000)       38 2023-05-18 13:13:55.000108 markdown-emdash-0.2.0/setup.cfg
+-rw-rw-r--   0 czue      (1000) czue      (1000)     1468 2023-05-18 13:13:41.000000 markdown-emdash-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `markdown-emdash-0.1.0/LICENSE` & `markdown-emdash-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown-emdash-0.1.0/setup.py` & `markdown-emdash-0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 readme_name = os.path.join(os.path.dirname(__file__), 'README.md')
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='markdown-emdash',
-    version='0.1.0',
+    version='0.2.0',
     py_modules=['mdx_emdash'],
     include_package_data=True,
     license='MIT License',
-    description='Extension for python-markdown that replaces all triple dashes with em-dashes.',
+    description='Extension for python-markdown that replaces all triple dashes em-dashes.',
     long_description=read_md(readme_name),
     url='https://github.com/czue/markdown-emdash',
     author='Cory Zue',
     author_email='cory@coryzue.com',
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
 )
```

