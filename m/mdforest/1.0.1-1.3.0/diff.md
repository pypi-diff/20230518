# Comparing `tmp/mdforest-1.0.1.tar.gz` & `tmp/mdforest-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdforest-1.0.1.tar", last modified: Sun May 14 23:03:48 2023, max compression
+gzip compressed data, was "mdforest-1.3.0.tar", last modified: Thu May 18 17:59:44 2023, max compression
```

## Comparing `mdforest-1.0.1.tar` & `mdforest-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 23:03:48.079975 mdforest-1.0.1/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 02:15:26.000000 mdforest-1.0.1/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2906 2023-05-14 23:03:48.079975 mdforest-1.0.1/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2457 2023-05-14 20:42:59.000000 mdforest-1.0.1/README.md
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 23:03:48.077974 mdforest-1.0.1/markdown_tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      430 2023-05-14 20:59:45.000000 mdforest-1.0.1/markdown_tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2444 2023-05-14 21:19:06.000000 mdforest-1.0.1/markdown_tree/markdown_tree.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-14 20:59:45.000000 mdforest-1.0.1/markdown_tree/treebuild.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 23:03:48.078975 mdforest-1.0.1/mdforest.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2906 2023-05-14 23:03:47.000000 mdforest-1.0.1/mdforest.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      305 2023-05-14 23:03:48.000000 mdforest-1.0.1/mdforest.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-14 23:03:47.000000 mdforest-1.0.1/mdforest.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       24 2023-05-14 23:03:47.000000 mdforest-1.0.1/mdforest.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       14 2023-05-14 23:03:47.000000 mdforest-1.0.1/mdforest.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 02:27:02.000000 mdforest-1.0.1/pyproject.toml
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-14 23:03:48.079975 mdforest-1.0.1/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1480 2023-05-14 23:03:45.000000 mdforest-1.0.1/setup.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 23:03:48.078975 mdforest-1.0.1/tests/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1201 2023-05-14 21:06:28.000000 mdforest-1.0.1/tests/test_mdtree.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 17:59:44.568893 mdforest-1.3.0/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 12:19:37.000000 mdforest-1.3.0/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3041 2023-05-18 17:59:44.568893 mdforest-1.3.0/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2457 2023-05-15 12:14:38.000000 mdforest-1.3.0/README.md
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 17:59:44.568893 mdforest-1.3.0/mdforest/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      425 2023-05-18 14:40:51.000000 mdforest-1.3.0/mdforest/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3789 2023-05-18 16:59:32.000000 mdforest-1.3.0/mdforest/mdforest.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 17:59:44.568893 mdforest-1.3.0/mdforest/tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 14:40:51.000000 mdforest-1.3.0/mdforest/tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3378 2023-05-18 14:57:37.000000 mdforest-1.3.0/mdforest/tree/types.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-18 14:40:51.000000 mdforest-1.3.0/mdforest/treebuild.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 17:59:44.568893 mdforest-1.3.0/mdforest.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3041 2023-05-18 17:59:44.000000 mdforest-1.3.0/mdforest.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      313 2023-05-18 17:59:44.000000 mdforest-1.3.0/mdforest.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-18 17:59:44.000000 mdforest-1.3.0/mdforest.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-05-18 17:59:44.000000 mdforest-1.3.0/mdforest.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        9 2023-05-18 17:59:44.000000 mdforest-1.3.0/mdforest.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 12:19:37.000000 mdforest-1.3.0/pyproject.toml
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-18 17:59:44.568893 mdforest-1.3.0/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1537 2023-05-18 17:59:38.000000 mdforest-1.3.0/setup.py
```

### Comparing `mdforest-1.0.1/LICENSE` & `mdforest-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdforest-1.0.1/PKG-INFO` & `mdforest-1.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,105 +1,115 @@
 Metadata-Version: 2.1
 Name: mdforest
-Version: 1.0.1
-Summary: A package to convert between Markdown and a forest data structure for effecient processing.
+Version: 1.3.0
+Summary: A package to convert between Markdown and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/markdown-tree
-Download-URL: https://github.com/kj3moraes/markdown-tree/archive/1.0.1.zip
+Download-URL: https://github.com/kj3moraes/markdown-tree/archive/1.3.0.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
 Classifier: Topic :: Utilities
 Description-Content-Type: Markdown
 License-File: LICENSE
 
-![icon](media/forest-icon-display.png)
+mdforest - Markdown Forest
+==========================
 
-# mdforest - Markdown Forest
+A library to convert Markdown documents into tree data structures and
+vice versa. There is greater functionality available to modify, prune,
+add and delete parts of documents when there are in the MarkdownTree
+structure.
+
+markdown-tree is a fork of `md2py <https://github.com/alvinwan/md2py>`__
+which is no longer maintained. This library adds far more functionality
+and broadens the scope of the older libary. The full list of features
+can be found under `Features <##%20Features>`__
 
-A library to convert Markdown documents into tree data structures and vice versa. There is greater functionality available to modify, prune, add and delete parts of documents when there are in the MarkdownTree structure.
-
-markdown-tree is a fork of [md2py](https://github.com/alvinwan/md2py) which is no longer maintained. This library adds far more functionality and broadens the scope of the older libary. The full list of features can be found under [Features](## Features)
-
-## Install
+Install
+-------
 
 Install via pip
 
-```bash
-pip install markdown-tree
-```
+.. code:: bash
 
-You can find the library page here [here](nil)
+   pip install markdown-tree
 
-## Quick Usage Guide
+You can find the library page here `here <nil>`__
 
-Markdown2Python offers only one function `md2py`, which generates a Python
-object from markdown text. This object is a navigable, "Tree of Contents"
-abstraction for the markdown file.
+Quick Usage Guide
+-----------------
+
+Markdown2Python offers only one function ``md2py``, which generates a
+Python object from markdown text. This object is a navigable, “Tree of
+Contents” abstraction for the markdown file.
 
 Take, for example, the following markdown file.
 
 [[ chikin.md ]]
 
-```markdown
-# Chikin Tales
-
-Once there was a chikin.
+.. code:: markdown
 
-## Chapter 1 : Chikin Fly
+   # Chikin Tales
 
-Chickens don't fly. They do only the following:
+   Once there was a chikin.
 
-- waddle
-- plop 
+   ## Chapter 1 : Chikin Fly
 
+   Chickens don't fly. They do only the following:
 
-### Waddling
+   - waddle
+   - plop 
 
-A waddle is what these birds do.
 
-## Chapter 2 : Chikin Scream
+   ### Waddling
 
-### Plopping
+   A waddle is what these birds do.
 
-Plopping involves three steps:
+   ## Chapter 2 : Chikin Scream
 
-1. squawk
-2. plop
-3. repeat, unless ordered to squat
+   ### Plopping
 
-```
+   Plopping involves three steps:
 
-Akin to a navigation bar, the `TreeOfContents` object allows you to expand a
-markdown file one level at a time. Running `md2py` on the above markdown file
-will generate a tree, abstracting the below structure.
+   1. squawk
+   2. plop
+   3. repeat, unless ordered to squat
 
-```text
-               Chikin Tales
-              /     \       \
-             /       \       \ 
-       (Once th..)    |       \
-                      |        \
-                  Chapter 1     \
-                  /     |     Chapter 2   
-                 /      |         |
-       (Chickens do..)  |       Plopping
-                        |         |
-                     Waddling   (Plopping...)
-                        |
-                    (A waddle...)
+Akin to a navigation bar, the ``TreeOfContents`` object allows you to
+expand a markdown file one level at a time. Running ``md2py`` on the
+above markdown file will generate a tree, abstracting the below
+structure.
 
+.. code:: text
 
-```
+                  Chikin Tales
+                 /     \       \
+                /       \       \ 
+          (Once th..)    |       \
+                         |        \
+                     Chapter 1     \
+                     /     |     Chapter 2   
+                    /      |         |
+          (Chickens do..)  |       Plopping
+                           |         |
+                        Waddling   (Plopping...)
+                           |
+                       (A waddle...)
 
 For the full usage guide, access the SAMPLES.md file.
 
-## Features
+Features
+--------
 
 Some of the features of this library are:
 
-1. Converts a markdown file to a manipulatable, light Python data structure.
+1. Converts a markdown file to a manipulatable, light Python data
+   structure.
 2. Converts the Python data structure back into a Markdown file.
 3. Traverse and edit the Python data structure.
 
-## License 
+License
+-------
 
-The [original project](https://github.com/alvinwan/md2py) was licensed under the Apache 2.0 License and a copy is provided in this repo as well. All the files changed are listed in the CHANGELOG.
+The `original project <https://github.com/alvinwan/md2py>`__ was
+licensed under the Apache 2.0 License and a copy is provided in this
+repo as well. All the files changed are listed in the CHANGELOG.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mdforest-1.0.1/README.md` & `mdforest-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mdforest-1.0.1/markdown_tree/treebuild.py` & `mdforest-1.3.0/mdforest/treebuild.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.0.1/mdforest.egg-info/PKG-INFO` & `mdforest-1.3.0/mdforest.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,105 +1,115 @@
 Metadata-Version: 2.1
 Name: mdforest
-Version: 1.0.1
-Summary: A package to convert between Markdown and a forest data structure for effecient processing.
+Version: 1.3.0
+Summary: A package to convert between Markdown and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/markdown-tree
-Download-URL: https://github.com/kj3moraes/markdown-tree/archive/1.0.1.zip
+Download-URL: https://github.com/kj3moraes/markdown-tree/archive/1.3.0.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
 Classifier: Topic :: Utilities
 Description-Content-Type: Markdown
 License-File: LICENSE
 
-![icon](media/forest-icon-display.png)
+mdforest - Markdown Forest
+==========================
 
-# mdforest - Markdown Forest
+A library to convert Markdown documents into tree data structures and
+vice versa. There is greater functionality available to modify, prune,
+add and delete parts of documents when there are in the MarkdownTree
+structure.
+
+markdown-tree is a fork of `md2py <https://github.com/alvinwan/md2py>`__
+which is no longer maintained. This library adds far more functionality
+and broadens the scope of the older libary. The full list of features
+can be found under `Features <##%20Features>`__
 
-A library to convert Markdown documents into tree data structures and vice versa. There is greater functionality available to modify, prune, add and delete parts of documents when there are in the MarkdownTree structure.
-
-markdown-tree is a fork of [md2py](https://github.com/alvinwan/md2py) which is no longer maintained. This library adds far more functionality and broadens the scope of the older libary. The full list of features can be found under [Features](## Features)
-
-## Install
+Install
+-------
 
 Install via pip
 
-```bash
-pip install markdown-tree
-```
+.. code:: bash
 
-You can find the library page here [here](nil)
+   pip install markdown-tree
 
-## Quick Usage Guide
+You can find the library page here `here <nil>`__
 
-Markdown2Python offers only one function `md2py`, which generates a Python
-object from markdown text. This object is a navigable, "Tree of Contents"
-abstraction for the markdown file.
+Quick Usage Guide
+-----------------
+
+Markdown2Python offers only one function ``md2py``, which generates a
+Python object from markdown text. This object is a navigable, “Tree of
+Contents” abstraction for the markdown file.
 
 Take, for example, the following markdown file.
 
 [[ chikin.md ]]
 
-```markdown
-# Chikin Tales
-
-Once there was a chikin.
+.. code:: markdown
 
-## Chapter 1 : Chikin Fly
+   # Chikin Tales
 
-Chickens don't fly. They do only the following:
+   Once there was a chikin.
 
-- waddle
-- plop 
+   ## Chapter 1 : Chikin Fly
 
+   Chickens don't fly. They do only the following:
 
-### Waddling
+   - waddle
+   - plop 
 
-A waddle is what these birds do.
 
-## Chapter 2 : Chikin Scream
+   ### Waddling
 
-### Plopping
+   A waddle is what these birds do.
 
-Plopping involves three steps:
+   ## Chapter 2 : Chikin Scream
 
-1. squawk
-2. plop
-3. repeat, unless ordered to squat
+   ### Plopping
 
-```
+   Plopping involves three steps:
 
-Akin to a navigation bar, the `TreeOfContents` object allows you to expand a
-markdown file one level at a time. Running `md2py` on the above markdown file
-will generate a tree, abstracting the below structure.
+   1. squawk
+   2. plop
+   3. repeat, unless ordered to squat
 
-```text
-               Chikin Tales
-              /     \       \
-             /       \       \ 
-       (Once th..)    |       \
-                      |        \
-                  Chapter 1     \
-                  /     |     Chapter 2   
-                 /      |         |
-       (Chickens do..)  |       Plopping
-                        |         |
-                     Waddling   (Plopping...)
-                        |
-                    (A waddle...)
+Akin to a navigation bar, the ``TreeOfContents`` object allows you to
+expand a markdown file one level at a time. Running ``md2py`` on the
+above markdown file will generate a tree, abstracting the below
+structure.
 
+.. code:: text
 
-```
+                  Chikin Tales
+                 /     \       \
+                /       \       \ 
+          (Once th..)    |       \
+                         |        \
+                     Chapter 1     \
+                     /     |     Chapter 2   
+                    /      |         |
+          (Chickens do..)  |       Plopping
+                           |         |
+                        Waddling   (Plopping...)
+                           |
+                       (A waddle...)
 
 For the full usage guide, access the SAMPLES.md file.
 
-## Features
+Features
+--------
 
 Some of the features of this library are:
 
-1. Converts a markdown file to a manipulatable, light Python data structure.
+1. Converts a markdown file to a manipulatable, light Python data
+   structure.
 2. Converts the Python data structure back into a Markdown file.
 3. Traverse and edit the Python data structure.
 
-## License 
+License
+-------
 
-The [original project](https://github.com/alvinwan/md2py) was licensed under the Apache 2.0 License and a copy is provided in this repo as well. All the files changed are listed in the CHANGELOG.
+The `original project <https://github.com/alvinwan/md2py>`__ was
+licensed under the Apache 2.0 License and a copy is provided in this
+repo as well. All the files changed are listed in the CHANGELOG.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mdforest-1.0.1/setup.py` & `mdforest-1.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 
     def run_tests(self):
         # import here, cause outside the eggs aren't loaded
         import pytest
         errno = pytest.main(self.pytest_args)
         sys.exit(errno)
 
-this_directory = Path(__file__).parent
-LONG_DESCRIPTION = (this_directory / "README.md").read_text()
+this_directory = Path(__file__)
+LONG_DESCRIPTION = (this_directory.parent / "media" / "README.rst").read_text()
 
-VERSION = '1.0.1'
-DESCRIPTION = 'A package to convert between Markdown and a forest data structure for effecient processing.'
+VERSION = '1.3.0'
+DESCRIPTION = 'A package to convert between Markdown and a forest data structure for efficient processing.'
 
 setup(
     name = "mdforest",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
     description = DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="Markdown",
     readme="README.md",
     license = "Apache 2.0",
     url = "http://github.com/kj3moraes/markdown-tree",
-    packages = ['markdown_tree'],
+    packages = ['mdforest', 'mdforest.tree'],
     cmdclass = {'test': PyTest},
-    tests_require = ['pytest'],
-    install_requires = ['markdown', 'beautifulsoup4'],
+    tests_require = ['unittest', 'pytest'],
+    install_requires = ['markdown', 'beautifulsoup4', 'python-frontmatter'],
     download_url = 'https://github.com/kj3moraes/markdown-tree/archive/%s.zip' % VERSION,
     classifiers = [
         "Topic :: Utilities",
     ],
 )
```

