# Comparing `tmp/ndradex-0.3.0.tar.gz` & `tmp/ndradex-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndradex-0.3.0.tar", max compression
+gzip compressed data, was "ndradex-0.3.1.tar", max compression
```

## Comparing `ndradex-0.3.0.tar` & `ndradex-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1076 2023-05-18 17:37:48.900780 ndradex-0.3.0/LICENSE
--rw-r--r--   0        0        0      416 2023-05-18 17:37:48.900780 ndradex-0.3.0/ndradex/__init__.py
--rw-r--r--   0        0        0      150 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/.devcontainer/Dockerfile
--rw-r--r--   0        0        0      377 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0       39 2023-05-18 17:37:49.548783 ndradex-0.3.0/ndradex/bin/.git
--rw-r--r--   0        0        0      958 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/.github/workflows/formula.yml
--rw-r--r--   0        0        0      412 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/.github/workflows/tests.yml
--rw-r--r--   0        0        0        7 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/.gitignore
--rw-r--r--   0        0        0      440 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/CITATION.cff
--rw-r--r--   0        0        0      902 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/Formula/radex.rb
--rw-r--r--   0        0        0     1076 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/LICENSE
--rw-r--r--   0        0        0     1304 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/Makefile
--rw-r--r--   0        0        0     2202 2023-05-18 17:37:50.632787 ndradex-0.3.0/ndradex/bin/README.md
--rw-r--r--   0        0        0     3569 2023-05-18 17:37:48.900780 ndradex-0.3.0/ndradex/consts.py
--rw-r--r--   0        0        0     6742 2023-05-18 17:37:48.900780 ndradex-0.3.0/ndradex/db.py
--rw-r--r--   0        0        0    12538 2023-05-18 17:37:48.900780 ndradex-0.3.0/ndradex/grid.py
--rw-r--r--   0        0        0      462 2023-05-18 17:37:48.900780 ndradex-0.3.0/ndradex/io.py
--rw-r--r--   0        0        0     3440 2023-05-18 17:37:48.900780 ndradex-0.3.0/ndradex/radex.py
--rw-r--r--   0        0        0      874 2023-05-18 17:37:48.900780 ndradex-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 ndradex-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-18 17:49:36.886191 ndradex-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7724 2023-05-18 17:49:36.886191 ndradex-0.3.1/README.md
+-rw-r--r--   0        0        0      416 2023-05-18 17:49:36.886191 ndradex-0.3.1/ndradex/__init__.py
+-rw-r--r--   0        0        0      150 2023-05-18 17:49:38.158186 ndradex-0.3.1/ndradex/bin/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0      377 2023-05-18 17:49:38.158186 ndradex-0.3.1/ndradex/bin/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       39 2023-05-18 17:49:37.386189 ndradex-0.3.1/ndradex/bin/.git
+-rw-r--r--   0        0        0      958 2023-05-18 17:49:38.158186 ndradex-0.3.1/ndradex/bin/.github/workflows/formula.yml
+-rw-r--r--   0        0        0      412 2023-05-18 17:49:38.158186 ndradex-0.3.1/ndradex/bin/.github/workflows/tests.yml
+-rw-r--r--   0        0        0        7 2023-05-18 17:49:38.158186 ndradex-0.3.1/ndradex/bin/.gitignore
+-rw-r--r--   0        0        0      440 2023-05-18 17:49:38.158186 ndradex-0.3.1/ndradex/bin/CITATION.cff
+-rw-r--r--   0        0        0      902 2023-05-18 17:49:38.158186 ndradex-0.3.1/ndradex/bin/Formula/radex.rb
+-rw-r--r--   0        0        0     1076 2023-05-18 17:49:38.158186 ndradex-0.3.1/ndradex/bin/LICENSE
+-rw-r--r--   0        0        0     1304 2023-05-18 17:49:38.158186 ndradex-0.3.1/ndradex/bin/Makefile
+-rw-r--r--   0        0        0     2202 2023-05-18 17:49:38.158186 ndradex-0.3.1/ndradex/bin/README.md
+-rw-r--r--   0        0        0     3569 2023-05-18 17:49:36.886191 ndradex-0.3.1/ndradex/consts.py
+-rw-r--r--   0        0        0     6742 2023-05-18 17:49:36.886191 ndradex-0.3.1/ndradex/db.py
+-rw-r--r--   0        0        0    12538 2023-05-18 17:49:36.886191 ndradex-0.3.1/ndradex/grid.py
+-rw-r--r--   0        0        0      462 2023-05-18 17:49:36.886191 ndradex-0.3.1/ndradex/io.py
+-rw-r--r--   0        0        0     3440 2023-05-18 17:49:36.886191 ndradex-0.3.1/ndradex/radex.py
+-rw-r--r--   0        0        0      896 2023-05-18 17:49:36.886191 ndradex-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8828 1970-01-01 00:00:00.000000 ndradex-0.3.1/PKG-INFO
```

### Comparing `ndradex-0.3.0/LICENSE` & `ndradex-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ndradex-0.3.0/ndradex/bin/.github/workflows/formula.yml` & `ndradex-0.3.1/ndradex/bin/.github/workflows/formula.yml`

 * *Files identical despite different names*

### Comparing `ndradex-0.3.0/ndradex/bin/Formula/radex.rb` & `ndradex-0.3.1/ndradex/bin/Formula/radex.rb`

 * *Files identical despite different names*

### Comparing `ndradex-0.3.0/ndradex/bin/LICENSE` & `ndradex-0.3.1/ndradex/bin/LICENSE`

 * *Files identical despite different names*

### Comparing `ndradex-0.3.0/ndradex/bin/Makefile` & `ndradex-0.3.1/ndradex/bin/Makefile`

 * *Files identical despite different names*

### Comparing `ndradex-0.3.0/ndradex/bin/README.md` & `ndradex-0.3.1/ndradex/bin/README.md`

 * *Files identical despite different names*

### Comparing `ndradex-0.3.0/ndradex/consts.py` & `ndradex-0.3.1/ndradex/consts.py`

 * *Files identical despite different names*

### Comparing `ndradex-0.3.0/ndradex/db.py` & `ndradex-0.3.1/ndradex/db.py`

 * *Files identical despite different names*

### Comparing `ndradex-0.3.0/ndradex/grid.py` & `ndradex-0.3.1/ndradex/grid.py`

 * *Files identical despite different names*

### Comparing `ndradex-0.3.0/ndradex/radex.py` & `ndradex-0.3.1/ndradex/radex.py`

 * *Files identical despite different names*

### Comparing `ndradex-0.3.0/pyproject.toml` & `ndradex-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "ndradex"
-version = "0.3.0"
+version = "0.3.1"
 description = " Multidimensional grid RADEX calculator"
 authors = ["Akio Taniguchi <taniguchi@a.phys.nagoya-u.ac.jp>"]
 keywords = ["astronomy", "radio-astronomy", "radex", "xarray"]
 license = "MIT"
+readme = "README.md"
 homepage = "https://github.com/astropenguin/ndradex/"
 documentation = "https://astropenguin.github.io/ndradex/"
 
 [tool.poetry.dependencies]
-python = ">3.8, <3.12"
+python = ">=3.8, <3.12"
 astropy = "^5.0"
 astroquery = "^0.4"
 netcdf4 = "^1.6"
 numpy = "^1.22"
 pandas = "^1.5"
 pandas-stubs = "^1.5"
 tomlkit = "^0.11"
```

