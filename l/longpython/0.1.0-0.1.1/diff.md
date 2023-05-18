# Comparing `tmp/longpython-0.1.0.tar.gz` & `tmp/longpython-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longpython-0.1.0.tar", max compression
+gzip compressed data, was "longpython-0.1.1.tar", max compression
```

## Comparing `longpython-0.1.0.tar` & `longpython-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1063 2022-05-08 13:37:28.225914 longpython-0.1.0/LICENSE
--rw-r--r--   0        0        0     1364 2022-09-04 05:24:14.291733 longpython-0.1.0/README.md
--rw-r--r--   0        0        0        0 2022-05-16 10:03:21.870033 longpython-0.1.0/longpython/__init__.py
--rw-r--r--   0        0        0     1381 2022-05-17 02:46:58.273362 longpython-0.1.0/longpython/main.py
--rw-r--r--   0        0        0        0 2022-05-16 10:03:21.870033 longpython-0.1.0/longpython/py.typed
--rw-r--r--   0        0        0     1248 2022-09-05 07:19:59.559446 longpython-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2114 1970-01-01 00:00:00.000000 longpython-0.1.0/setup.py
--rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 longpython-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-16 07:33:12.991527 longpython-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1364 2023-05-16 07:33:12.991527 longpython-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 07:33:12.991527 longpython-0.1.1/longpython/__init__.py
+-rw-r--r--   0        0        0     1381 2023-05-16 07:33:12.995527 longpython-0.1.1/longpython/main.py
+-rw-r--r--   0        0        0        0 2023-05-16 07:33:12.995527 longpython-0.1.1/longpython/py.typed
+-rw-r--r--   0        0        0     1245 2023-05-18 09:05:50.161033 longpython-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2310 1970-01-01 00:00:00.000000 longpython-0.1.1/PKG-INFO
```

### Comparing `longpython-0.1.0/LICENSE` & `longpython-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `longpython-0.1.0/README.md` & `longpython-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `longpython-0.1.0/longpython/main.py` & `longpython-0.1.1/longpython/main.py`

 * *Files identical despite different names*

### Comparing `longpython-0.1.0/pyproject.toml` & `longpython-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "longpython"
-version = "0.1.0"
+version = "0.1.1"
 description = "CLI tool to print long python"
-authors = ["Hibiki(4513ECHO) <4513echo@gmail.com>"]
+authors = ["Hibiki(4513ECHO) <mail@4513echo.dev>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/4513ECHO/longpython"
 packages = [
   { include = "longpython" },
 ]
 classifiers = [
@@ -22,25 +22,25 @@
 
 [tool.poetry.scripts]
 longpython = "longpython.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
-[tool.poetry.dev-dependencies]
-black = "^22.8.0"
-isort = "^5.10.0"
-mypy = "^0.971"
-flake8 = "^5.0.0"
-flake8-pyproject = "^1.1.0"
-pre-commit = "^2.20.0"
-pytest = "^7.1.0"
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+isort = "^5.12.0"
+mypy = "^1.3.0"
+flake8 = "^6.0.0"
+flake8-pyproject = "^1.2.3"
+pre-commit = "^3.3.1"
+pytest = "^7.3.1"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
 py_version = 39
```

### Comparing `longpython-0.1.0/PKG-INFO` & `longpython-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: longpython
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI tool to print long python
 Home-page: https://github.com/4513ECHO/longpython
 License: MIT
 Author: Hibiki(4513ECHO)
-Author-email: 4513echo@gmail.com
+Author-email: mail@4513echo.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Project-URL: Repository, https://github.com/4513ECHO/longpython
```

