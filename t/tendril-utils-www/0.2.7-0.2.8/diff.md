# Comparing `tmp/tendril-utils-www-0.2.7.tar.gz` & `tmp/tendril-utils-www-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-utils-www-0.2.7.tar", last modified: Fri Apr 21 08:32:49 2023, max compression
+gzip compressed data, was "tendril-utils-www-0.2.8.tar", last modified: Thu May 18 11:35:40 2023, max compression
```

## Comparing `tendril-utils-www-0.2.7.tar` & `tendril-utils-www-0.2.8.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:32:49.790429 tendril-utils-www-0.2.7/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2121 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3518 2023-04-21 08:32:49.790429 tendril-utils-www-0.2.7/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2223 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:32:49.786430 tendril-utils-www-0.2.7/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:32:49.786430 tendril-utils-www-0.2.7/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:32:49.786430 tendril-utils-www-0.2.7/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:32:49.786430 tendril-utils-www-0.2.7/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      577 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       93 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/api/tendril.config.www.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       97 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/api/tendril.utils.www.bare.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      100 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/api/tendril.utils.www.caching.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      100 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/api/tendril.utils.www.helpers.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      106 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/api/tendril.utils.www.redirectcache.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       96 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/api/tendril.utils.www.req.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       97 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/api/tendril.utils.www.soap.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       99 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/api/tendril.utils.www.status.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1088 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1723 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:32:49.786430 tendril-utils-www-0.2.7/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-21 08:32:49.790429 tendril-utils-www-0.2.7/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3431 2023-04-20 11:35:41.000000 tendril-utils-www-0.2.7/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:32:49.782430 tendril-utils-www-0.2.7/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:32:49.786430 tendril-utils-www-0.2.7/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:50:25.000000 tendril-utils-www-0.2.7/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:32:49.786430 tendril-utils-www-0.2.7/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2031 2023-04-20 18:47:00.000000 tendril-utils-www-0.2.7/src/tendril/config/www.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:32:49.786430 tendril-utils-www-0.2.7/src/tendril/utils/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:50:32.000000 tendril-utils-www-0.2.7/src/tendril/utils/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:32:49.786430 tendril-utils-www-0.2.7/src/tendril/utils/www/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3123 2023-04-21 07:13:06.000000 tendril-utils-www-0.2.7/src/tendril/utils/www/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7607 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/src/tendril/utils/www/bare.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7694 2023-04-20 11:45:06.000000 tendril-utils-www-0.2.7/src/tendril/utils/www/caching.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3401 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/src/tendril/utils/www/helpers.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4844 2023-04-21 08:32:04.000000 tendril-utils-www-0.2.7/src/tendril/utils/www/hx.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3868 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/src/tendril/utils/www/redirectcache.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5089 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/src/tendril/utils/www/req.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9328 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/src/tendril/utils/www/soap.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      303 2023-04-20 16:44:31.000000 tendril-utils-www-0.2.7/src/tendril/utils/www/ssl.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1490 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/src/tendril/utils/www/status.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:32:49.790429 tendril-utils-www-0.2.7/src/tendril_utils_www.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3518 2023-04-21 08:32:49.000000 tendril-utils-www-0.2.7/src/tendril_utils_www.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1428 2023-04-21 08:32:49.000000 tendril-utils-www-0.2.7/src/tendril_utils_www.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-21 08:32:49.000000 tendril-utils-www-0.2.7/src/tendril_utils_www.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      639 2023-04-21 08:32:49.000000 tendril-utils-www-0.2.7/src/tendril_utils_www.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-21 08:32:49.000000 tendril-utils-www-0.2.7/src/tendril_utils_www.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-21 08:32:49.790429 tendril-utils-www-0.2.7/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1721 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/tests/test_bare.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1106 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/tests/test_helpers.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2245 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/tests/test_redirectcache.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      829 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.7/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-05-18 11:35:40.159511 tendril-utils-www-0.2.8/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2121 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3518 2023-05-18 11:35:40.159511 tendril-utils-www-0.2.8/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2223 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-05-18 11:35:40.151512 tendril-utils-www-0.2.8/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-05-18 11:35:40.151512 tendril-utils-www-0.2.8/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-05-18 11:35:40.151512 tendril-utils-www-0.2.8/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-05-18 11:35:40.155511 tendril-utils-www-0.2.8/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      577 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       93 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/api/tendril.config.www.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       97 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/api/tendril.utils.www.bare.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      100 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/api/tendril.utils.www.caching.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      100 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/api/tendril.utils.www.helpers.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      106 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/api/tendril.utils.www.redirectcache.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       96 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/api/tendril.utils.www.req.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       97 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/api/tendril.utils.www.soap.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       99 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/api/tendril.utils.www.status.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1088 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1723 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-05-18 11:35:40.155511 tendril-utils-www-0.2.8/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-05-18 11:35:40.159511 tendril-utils-www-0.2.8/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3431 2023-04-20 11:35:41.000000 tendril-utils-www-0.2.8/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-05-18 11:35:40.147512 tendril-utils-www-0.2.8/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-05-18 11:35:40.155511 tendril-utils-www-0.2.8/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:50:25.000000 tendril-utils-www-0.2.8/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-05-18 11:35:40.155511 tendril-utils-www-0.2.8/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2031 2023-04-20 18:47:00.000000 tendril-utils-www-0.2.8/src/tendril/config/www.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-05-18 11:35:40.155511 tendril-utils-www-0.2.8/src/tendril/utils/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:50:32.000000 tendril-utils-www-0.2.8/src/tendril/utils/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-05-18 11:35:40.155511 tendril-utils-www-0.2.8/src/tendril/utils/www/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3123 2023-04-21 07:13:06.000000 tendril-utils-www-0.2.8/src/tendril/utils/www/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7607 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/src/tendril/utils/www/bare.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7694 2023-04-20 11:45:06.000000 tendril-utils-www-0.2.8/src/tendril/utils/www/caching.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3401 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/src/tendril/utils/www/helpers.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4957 2023-04-21 09:12:08.000000 tendril-utils-www-0.2.8/src/tendril/utils/www/hx.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3889 2023-05-18 11:34:03.000000 tendril-utils-www-0.2.8/src/tendril/utils/www/redirectcache.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5089 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/src/tendril/utils/www/req.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9328 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/src/tendril/utils/www/soap.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      303 2023-04-20 16:44:31.000000 tendril-utils-www-0.2.8/src/tendril/utils/www/ssl.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1490 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/src/tendril/utils/www/status.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-05-18 11:35:40.159511 tendril-utils-www-0.2.8/src/tendril_utils_www.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3518 2023-05-18 11:35:40.000000 tendril-utils-www-0.2.8/src/tendril_utils_www.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1428 2023-05-18 11:35:40.000000 tendril-utils-www-0.2.8/src/tendril_utils_www.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-05-18 11:35:40.000000 tendril-utils-www-0.2.8/src/tendril_utils_www.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      639 2023-05-18 11:35:40.000000 tendril-utils-www-0.2.8/src/tendril_utils_www.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-05-18 11:35:40.000000 tendril-utils-www-0.2.8/src/tendril_utils_www.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-05-18 11:35:40.159511 tendril-utils-www-0.2.8/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1721 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/tests/test_bare.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1106 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/tests/test_helpers.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2245 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/tests/test_redirectcache.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      829 2020-08-18 06:57:10.000000 tendril-utils-www-0.2.8/tox.ini
```

### Comparing `tendril-utils-www-0.2.7/.gitignore` & `tendril-utils-www-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/.readthedocs.yml` & `tendril-utils-www-0.2.8/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/.travis.yml` & `tendril-utils-www-0.2.8/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/LICENSE` & `tendril-utils-www-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/PKG-INFO` & `tendril-utils-www-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-utils-www
-Version: 0.2.7
+Version: 0.2.8
 Summary: Internet utilities for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-www
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-utils-www.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-www/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-www
```

### Comparing `tendril-utils-www-0.2.7/README.rst` & `tendril-utils-www-0.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/docs/Makefile` & `tendril-utils-www-0.2.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/docs/_static/custom.css` & `tendril-utils-www-0.2.8/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/docs/_static/favicon.ico` & `tendril-utils-www-0.2.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/docs/_static/logo.png` & `tendril-utils-www-0.2.8/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/docs/_static/logo_packed.png` & `tendril-utils-www-0.2.8/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/docs/_templates/about.html` & `tendril-utils-www-0.2.8/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/docs/api/index.rst` & `tendril-utils-www-0.2.8/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/docs/conf.py` & `tendril-utils-www-0.2.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/docs/index.rst` & `tendril-utils-www-0.2.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/docs/installation.rst` & `tendril-utils-www-0.2.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/setup.py` & `tendril-utils-www-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/src/tendril/config/__init__.py` & `tendril-utils-www-0.2.8/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/src/tendril/config/www.py` & `tendril-utils-www-0.2.8/src/tendril/config/www.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/src/tendril/utils/www/__init__.py` & `tendril-utils-www-0.2.8/src/tendril/utils/www/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/src/tendril/utils/www/bare.py` & `tendril-utils-www-0.2.8/src/tendril/utils/www/bare.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/src/tendril/utils/www/caching.py` & `tendril-utils-www-0.2.8/src/tendril/utils/www/caching.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/src/tendril/utils/www/helpers.py` & `tendril-utils-www-0.2.8/src/tendril/utils/www/helpers.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/src/tendril/utils/www/hx.py` & `tendril-utils-www-0.2.8/src/tendril/utils/www/hx.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,16 @@
         async def inject_client(self, *args, **kwargs):
             client = kwargs.get('client', None)
             if client is None:
                 ckw = {}
                 if hasattr(self, '_async_http_client_args'):
                     ckw.update(self._async_http_client_args())
                 ckw.update(client_kwargs)
+                logger.debug("Creating httpx client with args : "
+                             "{}".format(ckw))
                 async with async_client(**ckw) as c:
                     kwargs['client'] = c
                     result = await func(self, *args, **kwargs)
                     return result
             else:
                 result = await func(self, *args, **kwargs)
                 return result
```

### Comparing `tendril-utils-www-0.2.7/src/tendril/utils/www/redirectcache.py` & `tendril-utils-www-0.2.8/src/tendril/utils/www/redirectcache.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     with open(REDIR_CACHE_FILE, "rb") as rdcf:
         redirect_cache = pickle.load(rdcf)
     logger.info('Loaded Redirect Cache from file')
 except EOFError:
     os.remove(REDIR_CACHE_FILE)
     redirect_cache = {}
     logger.warning('Discarded Corrupt Redirect Cache')
-except IOError:
+except (IOError, FileNotFoundError):
     redirect_cache = {}
     logger.info('Created new Redirect Cache')
 
 
 def dump_redirect_cache():
     """
     Called during python interpreter shutdown, this function dumps the
```

### Comparing `tendril-utils-www-0.2.7/src/tendril/utils/www/req.py` & `tendril-utils-www-0.2.8/src/tendril/utils/www/req.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/src/tendril/utils/www/soap.py` & `tendril-utils-www-0.2.8/src/tendril/utils/www/soap.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/src/tendril/utils/www/status.py` & `tendril-utils-www-0.2.8/src/tendril/utils/www/status.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/src/tendril_utils_www.egg-info/PKG-INFO` & `tendril-utils-www-0.2.8/src/tendril_utils_www.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-utils-www
-Version: 0.2.7
+Version: 0.2.8
 Summary: Internet utilities for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-www
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-utils-www.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-www/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-www
```

### Comparing `tendril-utils-www-0.2.7/src/tendril_utils_www.egg-info/SOURCES.txt` & `tendril-utils-www-0.2.8/src/tendril_utils_www.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/src/tendril_utils_www.egg-info/requires.txt` & `tendril-utils-www-0.2.8/src/tendril_utils_www.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/tests/coveralls.py` & `tendril-utils-www-0.2.8/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/tests/test_bare.py` & `tendril-utils-www-0.2.8/tests/test_bare.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/tests/test_helpers.py` & `tendril-utils-www-0.2.8/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/tests/test_redirectcache.py` & `tendril-utils-www-0.2.8/tests/test_redirectcache.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-www-0.2.7/tox.ini` & `tendril-utils-www-0.2.8/tox.ini`

 * *Files identical despite different names*

