# Comparing `tmp/moat-gpio-0.6.4.tar.gz` & `tmp/moat-gpio-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moat-gpio-0.6.4.tar", last modified: Tue Jan  3 13:25:47 2023, max compression
+gzip compressed data, was "moat-gpio-0.6.5.tar", last modified: Thu May 18 12:46:31 2023, max compression
```

## Comparing `moat-gpio-0.6.4.tar` & `moat-gpio-0.6.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:25:47.389044 moat-gpio-0.6.4/
--rw-r--r--   0 smurf      (501) smurf      (501)      115 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/.coveragerc
--rw-r--r--   0 smurf      (501) smurf      (501)      436 2023-01-03 13:25:42.000000 moat-gpio-0.6.4/.gitignore
--rw-r--r--   0 smurf      (501) smurf      (501)      151 2022-09-06 07:14:20.000000 moat-gpio-0.6.4/.pylintrc
--rw-r--r--   0 smurf      (501) smurf      (501)      173 2022-09-06 07:14:20.000000 moat-gpio-0.6.4/.readthedocs.yml
--rw-r--r--   0 smurf      (501) smurf      (501)     5373 2022-09-06 07:14:20.000000 moat-gpio-0.6.4/.style.yapf
--rw-r--r--   0 smurf      (501) smurf      (501)      208 2022-09-06 07:14:20.000000 moat-gpio-0.6.4/.travis.yml
--rw-r--r--   0 smurf      (501) smurf      (501)      858 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/CHEATSHEET.rst
--rw-r--r--   0 smurf      (501) smurf      (501)    11358 2022-09-06 07:14:20.000000 moat-gpio-0.6.4/LICENSE.APACHE2
--rw-r--r--   0 smurf      (501) smurf      (501)     1046 2022-09-06 07:14:20.000000 moat-gpio-0.6.4/LICENSE.MIT
--rw-r--r--   0 smurf      (501) smurf      (501)      185 2023-01-03 13:20:56.000000 moat-gpio-0.6.4/LICENSE.txt
--rw-r--r--   0 smurf      (501) smurf      (501)      178 2022-09-06 07:14:20.000000 moat-gpio-0.6.4/MANIFEST.in
--rw-r--r--   0 smurf      (501) smurf      (501)      240 2023-01-03 13:20:56.000000 moat-gpio-0.6.4/Makefile
--rw-r--r--   0 smurf      (501) smurf      (501)     1690 2023-01-03 13:25:47.389044 moat-gpio-0.6.4/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)      797 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/README.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:25:47.385043 moat-gpio-0.6.4/ci/
--rw-r--r--   0 smurf      (501) smurf      (501)      123 2022-09-06 07:14:20.000000 moat-gpio-0.6.4/ci/rtd-requirements.txt
--rw-r--r--   0 smurf      (501) smurf      (501)       23 2022-09-06 07:14:20.000000 moat-gpio-0.6.4/ci/test-requirements.txt
--rwxr-xr-x   0 smurf      (501) smurf      (501)     1259 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/ci/travis.sh
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:25:47.385043 moat-gpio-0.6.4/docs/
--rw-r--r--   0 smurf      (501) smurf      (501)      611 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/docs/Makefile
--rw-r--r--   0 smurf      (501) smurf      (501)      781 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/docs/make.bat
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:25:47.385043 moat-gpio-0.6.4/docs/source/
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:25:47.385043 moat-gpio-0.6.4/docs/source/_static/
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-06 07:14:20.000000 moat-gpio-0.6.4/docs/source/_static/.gitkeep
--rw-r--r--   0 smurf      (501) smurf      (501)     6040 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/docs/source/conf.py
--rw-r--r--   0 smurf      (501) smurf      (501)       96 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/docs/source/history.rst
--rw-r--r--   0 smurf      (501) smurf      (501)      869 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/docs/source/index.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     4593 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/docs/source/usage.rst
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:25:47.385043 moat-gpio-0.6.4/examples/
--rw-r--r--   0 smurf      (501) smurf      (501)      807 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/examples/line_echo.py
--rw-r--r--   0 smurf      (501) smurf      (501)      759 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/examples/line_echo_polled.py
--rw-r--r--   0 smurf      (501) smurf      (501)      669 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/examples/line_value.py
--rw-r--r--   0 smurf      (501) smurf      (501)     2940 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/examples/push_button_event.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:25:47.385043 moat-gpio-0.6.4/moat/
--rw-r--r--   0 smurf      (501) smurf      (501)       65 2023-01-03 13:20:56.000000 moat-gpio-0.6.4/moat/__init__.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:25:47.385043 moat-gpio-0.6.4/moat/gpio/
--rw-r--r--   0 smurf      (501) smurf      (501)      539 2023-01-03 13:20:56.000000 moat-gpio-0.6.4/moat/gpio/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)     9527 2023-01-03 13:20:56.000000 moat-gpio-0.6.4/moat/gpio/gpio.py
--rw-r--r--   0 smurf      (501) smurf      (501)     9744 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/moat/gpio/libgpiod.py
--rw-r--r--   0 smurf      (501) smurf      (501)     5791 2023-01-03 13:20:56.000000 moat-gpio-0.6.4/moat/gpio/test.py
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:25:47.389044 moat-gpio-0.6.4/moat_gpio.egg-info/
--rw-r--r--   0 smurf      (501) smurf      (501)     1690 2023-01-03 13:25:47.000000 moat-gpio-0.6.4/moat_gpio.egg-info/PKG-INFO
--rw-r--r--   0 smurf      (501) smurf      (501)      860 2023-01-03 13:25:47.000000 moat-gpio-0.6.4/moat_gpio.egg-info/SOURCES.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        1 2023-01-03 13:25:47.000000 moat-gpio-0.6.4/moat_gpio.egg-info/dependency_links.txt
--rw-r--r--   0 smurf      (501) smurf      (501)       16 2023-01-03 13:25:47.000000 moat-gpio-0.6.4/moat_gpio.egg-info/requires.txt
--rw-r--r--   0 smurf      (501) smurf      (501)        5 2023-01-03 13:25:47.000000 moat-gpio-0.6.4/moat_gpio.egg-info/top_level.txt
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:25:47.389044 moat-gpio-0.6.4/newsfragments/
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-06 07:14:20.000000 moat-gpio-0.6.4/newsfragments/.gitkeep
--rw-r--r--   0 smurf      (501) smurf      (501)     1393 2022-09-06 07:14:20.000000 moat-gpio-0.6.4/newsfragments/README.rst
--rw-r--r--   0 smurf      (501) smurf      (501)     2140 2023-01-03 13:20:56.000000 moat-gpio-0.6.4/pyproject.toml
--rw-r--r--   0 smurf      (501) smurf      (501)       38 2023-01-03 13:25:47.389044 moat-gpio-0.6.4/setup.cfg
-drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-01-03 13:25:47.389044 moat-gpio-0.6.4/tests/
--rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-16 15:26:41.000000 moat-gpio-0.6.4/tests/__init__.py
--rw-r--r--   0 smurf      (501) smurf      (501)       27 2022-09-06 07:14:20.000000 moat-gpio-0.6.4/tests/run.py
--rwxr-xr-x   0 smurf      (501) smurf      (501)      521 2022-09-06 07:41:28.000000 moat-gpio-0.6.4/tests/test.sh
--rw-r--r--   0 smurf      (501) smurf      (501)      173 2023-01-03 13:20:56.000000 moat-gpio-0.6.4/tests/test_basic.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:31.126823 moat-gpio-0.6.5/
+-rw-r--r--   0 smurf      (501) smurf      (501)      115 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/.coveragerc
+-rw-r--r--   0 smurf      (501) smurf      (501)      436 2023-05-18 12:46:26.000000 moat-gpio-0.6.5/.gitignore
+-rw-r--r--   0 smurf      (501) smurf      (501)      151 2022-09-06 07:14:20.000000 moat-gpio-0.6.5/.pylintrc
+-rw-r--r--   0 smurf      (501) smurf      (501)      173 2022-09-06 07:14:20.000000 moat-gpio-0.6.5/.readthedocs.yml
+-rw-r--r--   0 smurf      (501) smurf      (501)     5373 2022-09-06 07:14:20.000000 moat-gpio-0.6.5/.style.yapf
+-rw-r--r--   0 smurf      (501) smurf      (501)      208 2022-09-06 07:14:20.000000 moat-gpio-0.6.5/.travis.yml
+-rw-r--r--   0 smurf      (501) smurf      (501)      858 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/CHEATSHEET.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)    11358 2022-09-06 07:14:20.000000 moat-gpio-0.6.5/LICENSE.APACHE2
+-rw-r--r--   0 smurf      (501) smurf      (501)     1046 2022-09-06 07:14:20.000000 moat-gpio-0.6.5/LICENSE.MIT
+-rw-r--r--   0 smurf      (501) smurf      (501)      185 2023-01-03 13:20:56.000000 moat-gpio-0.6.5/LICENSE.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)      178 2022-09-06 07:14:20.000000 moat-gpio-0.6.5/MANIFEST.in
+-rw-r--r--   0 smurf      (501) smurf      (501)      270 2023-05-18 12:46:09.000000 moat-gpio-0.6.5/Makefile
+-rw-r--r--   0 smurf      (501) smurf      (501)     1690 2023-05-18 12:46:31.126823 moat-gpio-0.6.5/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)      797 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/README.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:31.118822 moat-gpio-0.6.5/ci/
+-rw-r--r--   0 smurf      (501) smurf      (501)      123 2022-09-06 07:14:20.000000 moat-gpio-0.6.5/ci/rtd-requirements.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       23 2022-09-06 07:14:20.000000 moat-gpio-0.6.5/ci/test-requirements.txt
+-rwxr-xr-x   0 smurf      (501) smurf      (501)     1259 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/ci/travis.sh
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:31.122823 moat-gpio-0.6.5/docs/
+-rw-r--r--   0 smurf      (501) smurf      (501)      611 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/docs/Makefile
+-rw-r--r--   0 smurf      (501) smurf      (501)      781 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/docs/make.bat
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:31.122823 moat-gpio-0.6.5/docs/source/
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:31.122823 moat-gpio-0.6.5/docs/source/_static/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-06 07:14:20.000000 moat-gpio-0.6.5/docs/source/_static/.gitkeep
+-rw-r--r--   0 smurf      (501) smurf      (501)     6040 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/docs/source/conf.py
+-rw-r--r--   0 smurf      (501) smurf      (501)       96 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/docs/source/history.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)      869 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/docs/source/index.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     4593 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/docs/source/usage.rst
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:31.126823 moat-gpio-0.6.5/examples/
+-rw-r--r--   0 smurf      (501) smurf      (501)      807 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/examples/line_echo.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      759 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/examples/line_echo_polled.py
+-rw-r--r--   0 smurf      (501) smurf      (501)      669 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/examples/line_value.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     2940 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/examples/push_button_event.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:31.126823 moat-gpio-0.6.5/moat/
+-rw-r--r--   0 smurf      (501) smurf      (501)      105 2023-05-18 12:46:09.000000 moat-gpio-0.6.5/moat/__init__.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:31.126823 moat-gpio-0.6.5/moat/gpio/
+-rw-r--r--   0 smurf      (501) smurf      (501)      539 2023-01-03 13:20:56.000000 moat-gpio-0.6.5/moat/gpio/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     9527 2023-01-03 13:20:56.000000 moat-gpio-0.6.5/moat/gpio/gpio.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     9744 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/moat/gpio/libgpiod.py
+-rw-r--r--   0 smurf      (501) smurf      (501)     5791 2023-01-03 13:20:56.000000 moat-gpio-0.6.5/moat/gpio/test.py
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:31.126823 moat-gpio-0.6.5/moat_gpio.egg-info/
+-rw-r--r--   0 smurf      (501) smurf      (501)     1690 2023-05-18 12:46:30.000000 moat-gpio-0.6.5/moat_gpio.egg-info/PKG-INFO
+-rw-r--r--   0 smurf      (501) smurf      (501)      860 2023-05-18 12:46:31.000000 moat-gpio-0.6.5/moat_gpio.egg-info/SOURCES.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        1 2023-05-18 12:46:30.000000 moat-gpio-0.6.5/moat_gpio.egg-info/dependency_links.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)       16 2023-05-18 12:46:30.000000 moat-gpio-0.6.5/moat_gpio.egg-info/requires.txt
+-rw-r--r--   0 smurf      (501) smurf      (501)        5 2023-05-18 12:46:30.000000 moat-gpio-0.6.5/moat_gpio.egg-info/top_level.txt
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:31.126823 moat-gpio-0.6.5/newsfragments/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-06 07:14:20.000000 moat-gpio-0.6.5/newsfragments/.gitkeep
+-rw-r--r--   0 smurf      (501) smurf      (501)     1393 2022-09-06 07:14:20.000000 moat-gpio-0.6.5/newsfragments/README.rst
+-rw-r--r--   0 smurf      (501) smurf      (501)     2140 2023-04-18 13:36:52.000000 moat-gpio-0.6.5/pyproject.toml
+-rw-r--r--   0 smurf      (501) smurf      (501)       38 2023-05-18 12:46:31.126823 moat-gpio-0.6.5/setup.cfg
+drwxr-xr-x   0 smurf      (501) smurf      (501)        0 2023-05-18 12:46:31.126823 moat-gpio-0.6.5/tests/
+-rw-r--r--   0 smurf      (501) smurf      (501)        0 2022-09-16 15:26:41.000000 moat-gpio-0.6.5/tests/__init__.py
+-rw-r--r--   0 smurf      (501) smurf      (501)       27 2022-09-06 07:14:20.000000 moat-gpio-0.6.5/tests/run.py
+-rwxr-xr-x   0 smurf      (501) smurf      (501)      521 2022-09-06 07:41:28.000000 moat-gpio-0.6.5/tests/test.sh
+-rw-r--r--   0 smurf      (501) smurf      (501)      173 2023-01-03 13:20:56.000000 moat-gpio-0.6.5/tests/test_basic.py
```

### Comparing `moat-gpio-0.6.4/.style.yapf` & `moat-gpio-0.6.5/.style.yapf`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/CHEATSHEET.rst` & `moat-gpio-0.6.5/CHEATSHEET.rst`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/LICENSE.APACHE2` & `moat-gpio-0.6.5/LICENSE.APACHE2`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/LICENSE.MIT` & `moat-gpio-0.6.5/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/PKG-INFO` & `moat-gpio-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moat-gpio
-Version: 0.6.4
+Version: 0.6.5
 Summary: Easy async access to GPIO pins
 Author-email: Matthias Urlichs <matthias@urlichs.de>
 License: This software is made available under the terms of *either* of the
         licenses found in LICENSE.APACHE2 or LICENSE.MIT. Contributions to are
         made under the terms of *both* these licenses.
         
 Project-URL: homepage, https://m-o-a-t.org
```

### Comparing `moat-gpio-0.6.4/README.rst` & `moat-gpio-0.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/ci/travis.sh` & `moat-gpio-0.6.5/ci/travis.sh`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/docs/Makefile` & `moat-gpio-0.6.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/docs/make.bat` & `moat-gpio-0.6.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/docs/source/conf.py` & `moat-gpio-0.6.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/docs/source/index.rst` & `moat-gpio-0.6.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/docs/source/usage.rst` & `moat-gpio-0.6.5/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/examples/line_echo.py` & `moat-gpio-0.6.5/examples/line_echo.py`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/examples/line_echo_polled.py` & `moat-gpio-0.6.5/examples/line_echo_polled.py`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/examples/line_value.py` & `moat-gpio-0.6.5/examples/line_value.py`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/examples/push_button_event.py` & `moat-gpio-0.6.5/examples/push_button_event.py`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/moat/gpio/__init__.py` & `moat-gpio-0.6.5/moat/gpio/__init__.py`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/moat/gpio/gpio.py` & `moat-gpio-0.6.5/moat/gpio/gpio.py`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/moat/gpio/libgpiod.py` & `moat-gpio-0.6.5/moat/gpio/libgpiod.py`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/moat/gpio/test.py` & `moat-gpio-0.6.5/moat/gpio/test.py`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/moat_gpio.egg-info/PKG-INFO` & `moat-gpio-0.6.5/moat_gpio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moat-gpio
-Version: 0.6.4
+Version: 0.6.5
 Summary: Easy async access to GPIO pins
 Author-email: Matthias Urlichs <matthias@urlichs.de>
 License: This software is made available under the terms of *either* of the
         licenses found in LICENSE.APACHE2 or LICENSE.MIT. Contributions to are
         made under the terms of *both* these licenses.
         
 Project-URL: homepage, https://m-o-a-t.org
```

### Comparing `moat-gpio-0.6.4/moat_gpio.egg-info/SOURCES.txt` & `moat-gpio-0.6.5/moat_gpio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/newsfragments/README.rst` & `moat-gpio-0.6.5/newsfragments/README.rst`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/pyproject.toml` & `moat-gpio-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moat-gpio-0.6.4/tests/test.sh` & `moat-gpio-0.6.5/tests/test.sh`

 * *Files identical despite different names*

