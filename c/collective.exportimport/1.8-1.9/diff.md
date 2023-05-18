# Comparing `tmp/collective.exportimport-1.8.tar.gz` & `tmp/collective.exportimport-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.exportimport-1.8.tar", last modified: Thu Apr 20 14:48:16 2023, max compression
+gzip compressed data, was "collective.exportimport-1.9.tar", last modified: Thu May 18 16:51:23 2023, max compression
```

## Comparing `collective.exportimport-1.8.tar` & `collective.exportimport-1.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.434996 collective.exportimport-1.8/
--rw-r--r--   0 pbauer     (501) staff       (20)     9514 2023-04-20 14:48:16.000000 collective.exportimport-1.8/CHANGES.rst
--rw-r--r--   0 pbauer     (501) staff       (20)      210 2023-04-20 14:48:16.000000 collective.exportimport-1.8/CONTRIBUTORS.rst
--rw-r--r--   0 pbauer     (501) staff       (20)      552 2023-04-20 14:48:16.000000 collective.exportimport-1.8/DEVELOP.rst
--rw-r--r--   0 pbauer     (501) staff       (20)    18092 2023-04-20 14:48:16.000000 collective.exportimport-1.8/LICENSE.GPL
--rw-r--r--   0 pbauer     (501) staff       (20)      666 2023-04-20 14:48:16.000000 collective.exportimport-1.8/LICENSE.rst
--rw-r--r--   0 pbauer     (501) staff       (20)      110 2023-04-20 14:48:16.000000 collective.exportimport-1.8/MANIFEST.in
--rw-r--r--   0 pbauer     (501) staff       (20)    93315 2023-04-20 14:48:16.435107 collective.exportimport-1.8/PKG-INFO
--rw-r--r--   0 pbauer     (501) staff       (20)    81888 2023-04-20 14:48:16.000000 collective.exportimport-1.8/README.rst
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.428356 collective.exportimport-1.8/docs/
--rw-r--r--   0 pbauer     (501) staff       (20)     7993 2023-04-20 14:48:16.000000 collective.exportimport-1.8/docs/conf.py
--rw-r--r--   0 pbauer     (501) staff       (20)   147262 2023-04-20 14:48:16.000000 collective.exportimport-1.8/docs/export.png
--rw-r--r--   0 pbauer     (501) staff       (20)   110637 2023-04-20 14:48:16.000000 collective.exportimport-1.8/docs/import.png
--rw-r--r--   0 pbauer     (501) staff       (20)       92 2023-04-20 14:48:16.000000 collective.exportimport-1.8/docs/index.rst
--rw-r--r--   0 pbauer     (501) staff       (20)     5663 2023-04-20 14:48:16.000000 collective.exportimport-1.8/docs/starzel.png
--rw-r--r--   0 pbauer     (501) staff       (20)      222 2023-04-20 14:48:16.000000 collective.exportimport-1.8/requirements.txt
--rw-r--r--   0 pbauer     (501) staff       (20)      547 2023-04-20 14:48:16.435459 collective.exportimport-1.8/setup.cfg
--rw-r--r--   0 pbauer     (501) staff       (20)     3297 2023-04-20 14:48:16.000000 collective.exportimport-1.8/setup.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.426006 collective.exportimport-1.8/src/
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.428462 collective.exportimport-1.8/src/collective/
--rw-r--r--   0 pbauer     (501) staff       (20)       80 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/__init__.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.431513 collective.exportimport-1.8/src/collective/exportimport/
--rw-r--r--   0 pbauer     (501) staff       (20)      140 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/__init__.py
--rw-r--r--   0 pbauer     (501) staff       (20)      666 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/config.py
--rw-r--r--   0 pbauer     (501) staff       (20)     7665 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/configure.zcml
--rw-r--r--   0 pbauer     (501) staff       (20)     1353 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/deserializer.py
--rw-r--r--   0 pbauer     (501) staff       (20)    20141 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/export_content.py
--rw-r--r--   0 pbauer     (501) staff       (20)    28015 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/export_other.py
--rw-r--r--   0 pbauer     (501) staff       (20)    19308 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/fix_html.py
--rw-r--r--   0 pbauer     (501) staff       (20)    39323 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/import_content.py
--rw-r--r--   0 pbauer     (501) staff       (20)    30663 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/import_other.py
--rw-r--r--   0 pbauer     (501) staff       (20)      653 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/interfaces.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.432092 collective.exportimport-1.8/src/collective/exportimport/locales/
--rw-r--r--   0 pbauer     (501) staff       (20)      639 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/locales/README.rst
--rw-r--r--   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/locales/__init__.py
--rw-r--r--   0 pbauer     (501) staff       (20)    12849 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/locales/collective.exportimport.pot
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.426236 collective.exportimport-1.8/src/collective/exportimport/locales/en/
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.432252 collective.exportimport-1.8/src/collective/exportimport/locales/en/LC_MESSAGES/
--rw-r--r--   0 pbauer     (501) staff       (20)    12723 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/locales/en/LC_MESSAGES/collective.exportimport.po
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.426337 collective.exportimport-1.8/src/collective/exportimport/locales/es/
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.432395 collective.exportimport-1.8/src/collective/exportimport/locales/es/LC_MESSAGES/
--rw-r--r--   0 pbauer     (501) staff       (20)    17399 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/locales/es/LC_MESSAGES/collective.exportimport.po
--rw-r--r--   0 pbauer     (501) staff       (20)     1762 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/locales/update.py
--rwxr-xr-x   0 pbauer     (501) staff       (20)      506 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/locales/update.sh
--rw-r--r--   0 pbauer     (501) staff       (20)      260 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/permissions.zcml
--rw-r--r--   0 pbauer     (501) staff       (20)    23410 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/serializer.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.434028 collective.exportimport-1.8/src/collective/exportimport/templates/
--rw-r--r--   0 pbauer     (501) staff       (20)     7850 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/export_content.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     2163 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/export_other.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     4745 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_content.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     2043 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_defaultpages.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     3490 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_discussion.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     2189 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_localroles.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     4059 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_members.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     1825 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_ordering.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     3300 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_portlets.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     1877 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_redirects.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     2052 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_relations.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     1884 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/import_translations.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     4035 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/templates/links.pt
--rw-r--r--   0 pbauer     (501) staff       (20)     1273 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/testing.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.434898 collective.exportimport-1.8/src/collective/exportimport/tests/
--rw-r--r--   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/tests/__init__.py
--rw-r--r--   0 pbauer     (501) staff       (20)     8561 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/tests/file.pdf
--rw-r--r--   0 pbauer     (501) staff       (20)     3397 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/tests/test_drop_and_include.py
--rw-r--r--   0 pbauer     (501) staff       (20)    29510 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/tests/test_export.py
--rw-r--r--   0 pbauer     (501) staff       (20)    11863 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/tests/test_fix_html.py
--rw-r--r--   0 pbauer     (501) staff       (20)    55401 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/tests/test_import.py
--rw-r--r--   0 pbauer     (501) staff       (20)      902 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective/exportimport/tests/test_setup.py
-drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-04-20 14:48:16.429450 collective.exportimport-1.8/src/collective.exportimport.egg-info/
--rw-r--r--   0 pbauer     (501) staff       (20)    93315 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/PKG-INFO
--rw-r--r--   0 pbauer     (501) staff       (20)     2697 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/SOURCES.txt
--rw-r--r--   0 pbauer     (501) staff       (20)        1 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/dependency_links.txt
--rw-r--r--   0 pbauer     (501) staff       (20)      128 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/entry_points.txt
--rw-r--r--   0 pbauer     (501) staff       (20)       11 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/namespace_packages.txt
--rw-r--r--   0 pbauer     (501) staff       (20)        1 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/not-zip-safe
--rw-r--r--   0 pbauer     (501) staff       (20)      156 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/requires.txt
--rw-r--r--   0 pbauer     (501) staff       (20)       11 2023-04-20 14:48:16.000000 collective.exportimport-1.8/src/collective.exportimport.egg-info/top_level.txt
--rw-r--r--   0 pbauer     (501) staff       (20)      987 2023-04-20 14:48:16.000000 collective.exportimport-1.8/tox.ini
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.707191 collective.exportimport-1.9/
+-rw-r--r--   0 pbauer     (501) staff       (20)    10317 2023-05-18 16:51:23.000000 collective.exportimport-1.9/CHANGES.rst
+-rw-r--r--   0 pbauer     (501) staff       (20)      210 2023-05-18 16:51:23.000000 collective.exportimport-1.9/CONTRIBUTORS.rst
+-rw-r--r--   0 pbauer     (501) staff       (20)      552 2023-05-18 16:51:23.000000 collective.exportimport-1.9/DEVELOP.rst
+-rw-r--r--   0 pbauer     (501) staff       (20)    18092 2023-05-18 16:51:23.000000 collective.exportimport-1.9/LICENSE.GPL
+-rw-r--r--   0 pbauer     (501) staff       (20)      666 2023-05-18 16:51:23.000000 collective.exportimport-1.9/LICENSE.rst
+-rw-r--r--   0 pbauer     (501) staff       (20)      110 2023-05-18 16:51:23.000000 collective.exportimport-1.9/MANIFEST.in
+-rw-r--r--   0 pbauer     (501) staff       (20)    94983 2023-05-18 16:51:23.707312 collective.exportimport-1.9/PKG-INFO
+-rw-r--r--   0 pbauer     (501) staff       (20)    82753 2023-05-18 16:51:23.000000 collective.exportimport-1.9/README.rst
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.701424 collective.exportimport-1.9/docs/
+-rw-r--r--   0 pbauer     (501) staff       (20)     7993 2023-05-18 16:51:23.000000 collective.exportimport-1.9/docs/conf.py
+-rw-r--r--   0 pbauer     (501) staff       (20)   147262 2023-05-18 16:51:23.000000 collective.exportimport-1.9/docs/export.png
+-rw-r--r--   0 pbauer     (501) staff       (20)   110637 2023-05-18 16:51:23.000000 collective.exportimport-1.9/docs/import.png
+-rw-r--r--   0 pbauer     (501) staff       (20)       92 2023-05-18 16:51:23.000000 collective.exportimport-1.9/docs/index.rst
+-rw-r--r--   0 pbauer     (501) staff       (20)     5663 2023-05-18 16:51:23.000000 collective.exportimport-1.9/docs/starzel.png
+-rw-r--r--   0 pbauer     (501) staff       (20)      222 2023-05-18 16:51:23.000000 collective.exportimport-1.9/requirements.txt
+-rw-r--r--   0 pbauer     (501) staff       (20)      547 2023-05-18 16:51:23.707681 collective.exportimport-1.9/setup.cfg
+-rw-r--r--   0 pbauer     (501) staff       (20)     3297 2023-05-18 16:51:23.000000 collective.exportimport-1.9/setup.py
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.698980 collective.exportimport-1.9/src/
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.701536 collective.exportimport-1.9/src/collective/
+-rw-r--r--   0 pbauer     (501) staff       (20)       80 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/__init__.py
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.703894 collective.exportimport-1.9/src/collective/exportimport/
+-rw-r--r--   0 pbauer     (501) staff       (20)      140 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/__init__.py
+-rw-r--r--   0 pbauer     (501) staff       (20)      666 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/config.py
+-rw-r--r--   0 pbauer     (501) staff       (20)     7736 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/configure.zcml
+-rw-r--r--   0 pbauer     (501) staff       (20)     1594 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/deserializer.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    20432 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/export_content.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    28201 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/export_other.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    19308 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/fix_html.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    39450 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/import_content.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    32610 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/import_other.py
+-rw-r--r--   0 pbauer     (501) staff       (20)      653 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/interfaces.py
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.704415 collective.exportimport-1.9/src/collective/exportimport/locales/
+-rw-r--r--   0 pbauer     (501) staff       (20)      639 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/locales/README.rst
+-rw-r--r--   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/locales/__init__.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    12849 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/locales/collective.exportimport.pot
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.699202 collective.exportimport-1.9/src/collective/exportimport/locales/en/
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.704531 collective.exportimport-1.9/src/collective/exportimport/locales/en/LC_MESSAGES/
+-rw-r--r--   0 pbauer     (501) staff       (20)    12723 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/locales/en/LC_MESSAGES/collective.exportimport.po
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.699310 collective.exportimport-1.9/src/collective/exportimport/locales/es/
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.704641 collective.exportimport-1.9/src/collective/exportimport/locales/es/LC_MESSAGES/
+-rw-r--r--   0 pbauer     (501) staff       (20)    17399 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/locales/es/LC_MESSAGES/collective.exportimport.po
+-rw-r--r--   0 pbauer     (501) staff       (20)     1762 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/locales/update.py
+-rwxr-xr-x   0 pbauer     (501) staff       (20)      506 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/locales/update.sh
+-rw-r--r--   0 pbauer     (501) staff       (20)      260 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/permissions.zcml
+-rw-r--r--   0 pbauer     (501) staff       (20)    23353 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/serializer.py
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.706007 collective.exportimport-1.9/src/collective/exportimport/templates/
+-rw-r--r--   0 pbauer     (501) staff       (20)     7850 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/templates/export_content.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     2163 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/templates/export_other.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     4745 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/templates/import_content.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     2043 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/templates/import_defaultpages.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     3490 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/templates/import_discussion.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     2189 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/templates/import_localroles.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     4059 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/templates/import_members.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     1825 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/templates/import_ordering.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     3300 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/templates/import_portlets.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     1877 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/templates/import_redirects.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     2052 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/templates/import_relations.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     1884 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/templates/import_translations.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     4035 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/templates/links.pt
+-rw-r--r--   0 pbauer     (501) staff       (20)     1273 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/testing.py
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.707074 collective.exportimport-1.9/src/collective/exportimport/tests/
+-rw-r--r--   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/tests/__init__.py
+-rw-r--r--   0 pbauer     (501) staff       (20)     8561 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/tests/file.pdf
+-rw-r--r--   0 pbauer     (501) staff       (20)     3397 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/tests/test_drop_and_include.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    29510 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/tests/test_export.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    11863 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/tests/test_fix_html.py
+-rw-r--r--   0 pbauer     (501) staff       (20)    55401 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/tests/test_import.py
+-rw-r--r--   0 pbauer     (501) staff       (20)      902 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective/exportimport/tests/test_setup.py
+drwxr-xr-x   0 pbauer     (501) staff       (20)        0 2023-05-18 16:51:23.702436 collective.exportimport-1.9/src/collective.exportimport.egg-info/
+-rw-r--r--   0 pbauer     (501) staff       (20)    94983 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective.exportimport.egg-info/PKG-INFO
+-rw-r--r--   0 pbauer     (501) staff       (20)     2697 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective.exportimport.egg-info/SOURCES.txt
+-rw-r--r--   0 pbauer     (501) staff       (20)        1 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective.exportimport.egg-info/dependency_links.txt
+-rw-r--r--   0 pbauer     (501) staff       (20)      128 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective.exportimport.egg-info/entry_points.txt
+-rw-r--r--   0 pbauer     (501) staff       (20)       11 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective.exportimport.egg-info/namespace_packages.txt
+-rw-r--r--   0 pbauer     (501) staff       (20)        1 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective.exportimport.egg-info/not-zip-safe
+-rw-r--r--   0 pbauer     (501) staff       (20)      156 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective.exportimport.egg-info/requires.txt
+-rw-r--r--   0 pbauer     (501) staff       (20)       11 2023-05-18 16:51:23.000000 collective.exportimport-1.9/src/collective.exportimport.egg-info/top_level.txt
+-rw-r--r--   0 pbauer     (501) staff       (20)      987 2023-05-18 16:51:23.000000 collective.exportimport-1.9/tox.ini
```

### Comparing `collective.exportimport-1.8/CHANGES.rst` & `collective.exportimport-1.9/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,46 @@
 Changelog
 =========
 
 
+1.9 (2023-05-18)
+----------------
+
+- Allow passing custom filenames to exports
+  [pbauer]
+
+- Support export and import of Plone Site root (using update strategy).
+  [pbauer]
+
+- Fix blob export when Connection uses TmpStore
+  [gotcha, pbauer]
+
+- Fix portlet richtext field import
+  [mpeeters]
+
+- Add portlet location on exported data
+  [mpeeters]
+
+- Migrate root of portlets that used a path in plone4 to using a uid (navigation, search, events, collection).
+  [pbauer]
+
+- Make export of discussions and portlets contextual
+  [mpeeters]
+
+- Fix critical bug when importing groups: Do not import groups that a groups belongs to as members of the new group.
+  This could have caused groups to have more privileges than they should.
+  [pbauer]
+
+
 1.8 (2023-04-20)
 ----------------
 
 - Import: run set_uuid method before we call custom hooks, so the hooks have access to
   the item UUID. Fix #185.
+- Document COLLECTIVE_EXPORTIMPORT_CENTRAL_DIRECTORY in README.
   [fredvd]
 
 - Add Spanish translation.
   [macagua]
 
 - Add i18n support.
   [macagua]
@@ -37,15 +67,15 @@
 
 - Better serialization of Topics:
   - Use newer criteria added in Plone 5
   - Add fallback for some criteria
   - Export sort_on and sort_reversed
   - Export customView as tabular_view
   [pbauer]
-  
+
 - Always import discussions independent if discussion support is enabled or not
   on a particular content object (#182)
   [ajung]
 
 
 1.7 (2023-01-20)
 ----------------
```

### Comparing `collective.exportimport-1.8/DEVELOP.rst` & `collective.exportimport-1.9/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/LICENSE.GPL` & `collective.exportimport-1.9/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/LICENSE.rst` & `collective.exportimport-1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/PKG-INFO` & `collective.exportimport-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.exportimport
-Version: 1.8
+Version: 1.9
 Summary: An add-on for Plone to Export and import content, members, relations, translations and localroles.
 Home-page: https://github.com/collective/collective.exportimport
 Author: Philip Bauer (for starzel.de)
 Author-email: info@starzel.de
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.exportimport
 Project-URL: Source, https://github.com/collective/collective.exportimport
@@ -118,14 +118,26 @@
 .. image:: ./docs/import.png
 
 
 The imports for members, relations, localroles and relations are linked to in this form but can also be called individually: ``/@@import_members``, ``/@@import_relations``, ``/@@import_localroles``, ``/@@import_translations``, ``/@@import_ordering``, ``/@@import_discussion``.
 
 As a last step in a migration there is another view ``@@reset_dates`` that resets the modified date on imported content to the date initially contained in the imported json-file. This is necessary since varous changes during a migration will likely result in a updated modified-date. During import the original is stored as ``obj.modification_date_migrated`` on each new object and this view sets this date.
 
+Export- and import locations
+----------------------------
+
+If you select 'Save to file on server', the Export view will save json files in the <var> directory of your Plone instanc in /var/instance.
+The import view will look for  files under /var/instance/import.
+These directories will normally be different, under different Plone instances and possibly on different servers. 
+
+You can set the environment variable 'COLLECTIVE_EXPORTIMPORT_CENTRAL_DIRECTORY' to add a 'shared' directory on one server or maybe network share.
+With this variable set, collective.exportimport will both save to and load .json files from the same server directory. 
+This saves time not having to move .json files around from the export- to the import location.
+You should be aware that the Export views will overwrite any existing previous .json file export that have the same name. 
+
 
 Use-cases
 =========
 
 Migrations
 ----------
 
@@ -2269,19 +2281,49 @@
 - Leonardo J. Caballero G., leonardocaballero@gmail.com
 
 
 Changelog
 =========
 
 
+1.9 (2023-05-18)
+----------------
+
+- Allow passing custom filenames to exports
+  [pbauer]
+
+- Support export and import of Plone Site root (using update strategy).
+  [pbauer]
+
+- Fix blob export when Connection uses TmpStore
+  [gotcha, pbauer]
+
+- Fix portlet richtext field import
+  [mpeeters]
+
+- Add portlet location on exported data
+  [mpeeters]
+
+- Migrate root of portlets that used a path in plone4 to using a uid (navigation, search, events, collection).
+  [pbauer]
+
+- Make export of discussions and portlets contextual
+  [mpeeters]
+
+- Fix critical bug when importing groups: Do not import groups that a groups belongs to as members of the new group.
+  This could have caused groups to have more privileges than they should.
+  [pbauer]
+
+
 1.8 (2023-04-20)
 ----------------
 
 - Import: run set_uuid method before we call custom hooks, so the hooks have access to
   the item UUID. Fix #185.
+- Document COLLECTIVE_EXPORTIMPORT_CENTRAL_DIRECTORY in README.
   [fredvd]
 
 - Add Spanish translation.
   [macagua]
 
 - Add i18n support.
   [macagua]
@@ -2308,15 +2350,15 @@
 
 - Better serialization of Topics:
   - Use newer criteria added in Plone 5
   - Add fallback for some criteria
   - Export sort_on and sort_reversed
   - Export customView as tabular_view
   [pbauer]
-  
+
 - Always import discussions independent if discussion support is enabled or not
   on a particular content object (#182)
   [ajung]
 
 
 1.7 (2023-01-20)
 ----------------
```

### Comparing `collective.exportimport-1.8/README.rst` & `collective.exportimport-1.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,26 @@
 .. image:: ./docs/import.png
 
 
 The imports for members, relations, localroles and relations are linked to in this form but can also be called individually: ``/@@import_members``, ``/@@import_relations``, ``/@@import_localroles``, ``/@@import_translations``, ``/@@import_ordering``, ``/@@import_discussion``.
 
 As a last step in a migration there is another view ``@@reset_dates`` that resets the modified date on imported content to the date initially contained in the imported json-file. This is necessary since varous changes during a migration will likely result in a updated modified-date. During import the original is stored as ``obj.modification_date_migrated`` on each new object and this view sets this date.
 
+Export- and import locations
+----------------------------
+
+If you select 'Save to file on server', the Export view will save json files in the <var> directory of your Plone instanc in /var/instance.
+The import view will look for  files under /var/instance/import.
+These directories will normally be different, under different Plone instances and possibly on different servers. 
+
+You can set the environment variable 'COLLECTIVE_EXPORTIMPORT_CENTRAL_DIRECTORY' to add a 'shared' directory on one server or maybe network share.
+With this variable set, collective.exportimport will both save to and load .json files from the same server directory. 
+This saves time not having to move .json files around from the export- to the import location.
+You should be aware that the Export views will overwrite any existing previous .json file export that have the same name. 
+
 
 Use-cases
 =========
 
 Migrations
 ----------
```

### Comparing `collective.exportimport-1.8/docs/conf.py` & `collective.exportimport-1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/docs/export.png` & `collective.exportimport-1.9/docs/export.png`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/docs/import.png` & `collective.exportimport-1.9/docs/import.png`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/docs/starzel.png` & `collective.exportimport-1.9/docs/starzel.png`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/setup.cfg` & `collective.exportimport-1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/setup.py` & `collective.exportimport-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 else:
     install_requires.append("plone.restapi")
     install_requires.append("beautifulsoup4")
 
 
 setup(
     name="collective.exportimport",
-    version="1.8",
+    version="1.9",
     description="An add-on for Plone to Export and import content, members, relations, translations and localroles.",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Web Environment",
```

### Comparing `collective.exportimport-1.8/src/collective/exportimport/config.py` & `collective.exportimport-1.9/src/collective/exportimport/config.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/configure.zcml` & `collective.exportimport-1.9/src/collective/exportimport/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,15 @@
   <adapter factory=".serializer.RichttextFieldSerializerWithRawText" />
   <adapter factory=".serializer.CollectionFieldSerializer" />
   <adapter factory=".serializer.ChoiceFieldSerializer" />
   <adapter factory=".serializer.long_converter" />
 
   <!-- Deserializers -->
   <adapter factory=".deserializer.RichTextFieldDeserializerWithoutUnescape" />
+  <adapter factory=".deserializer.PortletRichTextFieldDeserializer" />
 
   <browser:page
       name="exportimport_links"
       for="zope.interface.Interface"
       template="templates/links.pt"
       permission="cmf.ManagePortal"
       />
```

### Comparing `collective.exportimport-1.8/src/collective/exportimport/deserializer.py` & `collective.exportimport-1.9/src/collective/exportimport/deserializer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collective.exportimport.interfaces import IMigrationMarker
 from plone.app.textfield.interfaces import IRichText
 from plone.app.textfield.value import RichTextValue
 from plone.dexterity.interfaces import IDexterityContent
+from plone.portlets.interfaces import IPortletAssignment
 from plone.restapi.deserializer.dxfields import DefaultFieldDeserializer
 from plone.restapi.interfaces import IFieldDeserializer
 from zope.component import adapter
 from zope.interface import implementer
 
 
 @implementer(IFieldDeserializer)
@@ -27,7 +28,13 @@
             raw=data,
             mimeType=content_type,
             outputMimeType=self.field.output_mime_type,
             encoding=encoding,
         )
         self.field.validate(value)
         return value
+
+
+@implementer(IFieldDeserializer)
+@adapter(IRichText, IPortletAssignment, IMigrationMarker)
+class PortletRichTextFieldDeserializer(RichTextFieldDeserializerWithoutUnescape):
+    pass
```

### Comparing `collective.exportimport-1.8/src/collective/exportimport/export_content.py` & `collective.exportimport-1.9/src/collective/exportimport/export_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from operator import itemgetter
 from plone import api
 from plone.app.layout.viewlets.content import ContentHistoryViewlet
 from plone.i18n.normalizer.interfaces import IIDNormalizer
 from plone.restapi.interfaces import ISerializeToJson
 from plone.restapi.serializer.converters import json_compatible
 from plone.uuid.interfaces import IUUID
+from Products.CMFPlone.interfaces import IPloneSiteRoot
 from Products.CMFPlone.interfaces.constrains import ENABLED
 from Products.CMFPlone.interfaces.constrains import ISelectableConstrainTypes
 from Products.CMFPlone.utils import safe_unicode
 from Products.Five import BrowserView
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from zope.component import getMultiAdapter
 from zope.component import getUtility
@@ -162,19 +163,21 @@
             pass
 
         if self.migration:
             # Add marker-interface to request to use custom serializers
             alsoProvides(self.request, IMigrationMarker)
 
         # to get a useful filename...
-        if self.portal_type and len(self.portal_type) == 1:
-            filename = self.portal_type[0]
-        else:
-            filename = self.path.split("/")[-1]
-        filename = "{}.json".format(filename)
+        filename = self.request.form.get("filename")
+        if not filename:
+            if self.portal_type and len(self.portal_type) == 1:
+                filename = self.portal_type[0]
+            else:
+                filename = self.path.split("/")[-1]
+            filename = "{}.json".format(filename)
 
         content_generator = self.export_content()
 
         number = 0
         if download_to_server:
             directory = config.CENTRAL_DIRECTORY
             if directory:
@@ -296,15 +299,17 @@
                 continue
             obj = self.global_obj_hook(obj)
             if not obj:
                 continue
             try:
                 self.safe_portal_type = fix_portal_type(obj.portal_type)
                 serializer = getMultiAdapter((obj, self.request), ISerializeToJson)
-                if getattr(aq_base(obj), "isPrincipiaFolderish", False):
+                if IPloneSiteRoot.providedBy(obj):
+                    item = serializer()
+                elif getattr(aq_base(obj), "isPrincipiaFolderish", False):
                     item = serializer(include_items=False)
                 else:
                     item = serializer()
                 item = self.update_export_data(item, obj)
 
                 yield item
             except Exception:
@@ -461,16 +466,17 @@
         """Fix the id. Mostly relevant for collections, where the id is set to “@@export-content”
         because of the HypermediaBatch in plone.restapi
         """
         obj_url = obj.absolute_url()
         parent_url = obj.__parent__.absolute_url()
         if item["@id"] != obj_url:
             item["@id"] = obj_url
-        if item["parent"]["@id"] != parent_url:
-            item["parent"]["@id"] = parent_url
+        if "@id" in item["parent"]:
+            if item["parent"]["@id"] != parent_url:
+                item["parent"]["@id"] = parent_url
         return item
 
     def export_constraints(self, item, obj):
         constrains = ISelectableConstrainTypes(obj, None)
         if constrains is None:
             return item
         if constrains.getConstrainTypesMode() == ENABLED:
```

### Comparing `collective.exportimport-1.8/src/collective/exportimport/export_other.py` & `collective.exportimport-1.9/src/collective/exportimport/export_other.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,17 @@
 PORTAL_PLACEHOLDER = "<Portal>"
 
 
 class BaseExport(BrowserView):
     """Just DRY"""
 
     def download(self, data):
-        filename = u"{}.json".format(self.__name__)
+        filename = self.request.form.get("filename")
+        if not filename:
+            filename = u"{}.json".format(self.__name__)
         if not data:
             msg = _(u"No data to export for {}").format(self.__name__)
             logger.info(msg)
             api.portal.show_message(msg, self.request)
             return self.request.response.redirect(self.request["ACTUAL_URL"])
 
         if self.download_to_server:
@@ -591,15 +593,17 @@
         data = self.all_discussions()
         logger.info(u"Exported %s discussions", len(data))
         self.download(data)
 
     def all_discussions(self):
         results = []
         for brain in api.content.find(
-            object_provides=IContentish.__identifier__, sort_on="path"
+            object_provides=IContentish.__identifier__,
+            sort_on="path",
+            context=self.context,
         ):
             try:
                 obj = brain.getObject()
                 if obj is None:
                     logger.error(u"brain.getObject() is None %s", brain.getPath())
                     continue
                 conversation = IConversation(obj, None)
@@ -629,17 +633,16 @@
         logger.info(u"Exporting portlets...")
         data = self.all_portlets()
         logger.info(u"Exported info for %s items with portlets", len(data))
         self.download(data)
 
     def all_portlets(self):
         self.results = []
-
         portal = api.portal.get()
-        portal.ZopeFindAndApply(portal, search_sub=True, apply_func=self.get_portlets)
+        portal.ZopeFindAndApply(self.context, search_sub=True, apply_func=self.get_portlets)
         return self.results
 
     def get_portlets(self,obj, path):
         uid = IUUID(obj, None)
         if not uid:
             return
         portlets = export_local_portlets(obj)
@@ -648,14 +651,15 @@
         blacklist = self.portlets_blacklist_hook(blacklist)
         obj_results = {}
         if portlets:
             obj_results["portlets"] = portlets
         if blacklist:
             obj_results["blacklist_status"] = blacklist
         if obj_results:
+            obj_results["@id"] = obj.absolute_url()
             obj_results["uuid"] = uid
             self.results.append(obj_results)
         return
 
     def local_portlets_hook(self, portlets):
         return portlets
```

### Comparing `collective.exportimport-1.8/src/collective/exportimport/fix_html.py` & `collective.exportimport-1.9/src/collective/exportimport/fix_html.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/import_content.py` & `collective.exportimport-1.9/src/collective/exportimport/import_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,16 +423,17 @@
 
     def handle_new_object(self, item, index, new):
 
         new, item = self.global_obj_hook_before_deserializing(new, item)
 
         # import using plone.restapi deserializers
         deserializer = getMultiAdapter((new, self.request), IDeserializeFromJson)
+        self.request["BODY"] = json.dumps(item)
         try:
-            new = deserializer(validate_all=False, data=item)
+            new = deserializer(validate_all=False)
         except Exception:
             logger.warning("Cannot deserialize %s %s", item["@type"], item["@id"], exc_info=True)
             raise
 
         # Blobs can be exported as only a path in the blob storage.
         # It seems difficult to dynamically use a different deserializer,
         # based on whether or not there is a blob_path somewhere in the item.
@@ -876,14 +877,17 @@
         # The default is to use the UUID of the old parent to find it
         if item["parent"].get("UID"):
             # For some reason api.content.get(UID=xxx) does not work sometimes...
             brains = api.content.find(UID=item["parent"]["UID"])
             if brains:
                 return brains[0].getObject()
 
+        if item["@type"] == "Plone Site":
+            return api.portal.get().__parent__
+
         if item["parent"]["@type"] == "Plone Site":
             return api.portal.get()
 
         # If the item is missing look for a item with the path of the old parent
         parent_url = unquote(item["parent"]["@id"])
         parent_path = urlparse(parent_url).path
         # physical path is bytes in Zope 2 (not in Zope 4)
```

### Comparing `collective.exportimport-1.8/src/collective/exportimport/import_other.py` & `collective.exportimport-1.9/src/collective/exportimport/import_other.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from Acquisition import aq_base
 from BTrees.LLBTree import LLSet
 from collective.exportimport import _
 from collective.exportimport import config
+from collective.exportimport.interfaces import IMigrationMarker
 from datetime import datetime
 from OFS.interfaces import IOrderedContainer
 from operator import itemgetter
 from collective.exportimport.export_other import PORTAL_PLACEHOLDER
 from plone import api
 from plone.app.discussion.comment import Comment
 from plone.app.discussion.interfaces import IConversation
@@ -22,14 +23,15 @@
 from zope.annotation.interfaces import IAnnotations
 from zope.component import getUtility
 from zope.component import queryMultiAdapter
 from zope.component import queryUtility
 from zope.component.interfaces import IFactory
 from zope.container.interfaces import INameChooser
 from zope.globalrequest import getRequest
+from zope.interface import alsoProvides
 from ZPublisher.HTTPRequest import FileUpload
 
 import dateutil
 import json
 import logging
 import six
 import transaction
@@ -215,15 +217,14 @@
         for item in data:
             if item["groupid"] not in groupsIds:  # New group, 'have to create it
                 api.group.create(
                     groupname=item["groupid"],
                     title=item["title"],
                     description=item["description"],
                     roles=item["roles"],
-                    groups=item["groups"],
                 )
                 # add all principals
                 for principal in item.get("principals", []):
                     pg.addPrincipalToGroup(principal, item["groupid"])
                 groupsNumber += 1
         return groupsNumber
 
@@ -661,14 +662,15 @@
         return results
 
 
 class ImportPortlets(BrowserView):
     """Import portlets"""
 
     def __call__(self, jsonfile=None, return_json=False):
+        alsoProvides(self.request, IMigrationMarker)
         if jsonfile:
             self.portal = api.portal.get()
             status = "success"
             try:
                 if isinstance(jsonfile, str):
                     return_json = True
                     data = json.loads(jsonfile)
@@ -742,14 +744,58 @@
             if visible is not None:
                 settings = IPortletAssignmentSettings(assignment)
                 settings["visible"] = visible
 
             # 2. Apply portlet settings
             portlet_interface = getUtility(IPortletTypeInterface, name=portlet_type)
             for property_name, value in assignment_data.items():
+                # For core portlets a path changed to uuid between Plone 4 and 5
+                migration_mapping = [
+                    {
+                        "portlet_type": "portlets.Navigation",
+                        "old": "root",
+                        "new": "root_uid",
+                    },
+                    {
+                        "portlet_type": "portlets.Search",
+                        "old": "search_base",
+                        "new": "search_base_uid",
+                    },
+                    {
+                        "portlet_type": "portlets.Events",
+                        "old": "search_base",
+                        "new": "search_base_uid",
+                    },
+                    {
+                        "portlet_type": "plone.portlet.collection.Collection",
+                        "old": "target_collection",
+                        "new": "uid",
+                    },
+                ]
+                for mapping in migration_mapping:
+                    if (
+                        property_name == mapping["old"]
+                        and value
+                        and portlet_type == mapping["portlet_type"]
+                    ):
+                        property_name = mapping["new"]
+                        target = api.content.get(path=value)
+                        if target:
+                            value = target.UID()
+                            break
+                        else:
+                            logger.info(
+                                "Could not find path '%s'. Manually fix %s '%s' at %s",
+                                value,
+                                portlet_type,
+                                name,
+                                obj.absolute_url(),
+                            )
+                            continue
+
                 field = portlet_interface.get(property_name, None)
                 if field is None:
                     continue
                 field = field.bind(assignment)
                 # deserialize data (e.g. for RichText)
                 deserializer = queryMultiAdapter(
                     (field, assignment, request), IFieldDeserializer
```

### Comparing `collective.exportimport-1.8/src/collective/exportimport/interfaces.py` & `collective.exportimport-1.9/src/collective/exportimport/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/locales/README.rst` & `collective.exportimport-1.9/src/collective/exportimport/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/locales/collective.exportimport.pot` & `collective.exportimport-1.9/src/collective/exportimport/locales/collective.exportimport.pot`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/locales/en/LC_MESSAGES/collective.exportimport.po` & `collective.exportimport-1.9/src/collective/exportimport/locales/en/LC_MESSAGES/collective.exportimport.po`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/locales/es/LC_MESSAGES/collective.exportimport.po` & `collective.exportimport-1.9/src/collective/exportimport/locales/es/LC_MESSAGES/collective.exportimport.po`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/locales/update.py` & `collective.exportimport-1.9/src/collective/exportimport/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/serializer.py` & `collective.exportimport-1.9/src/collective/exportimport/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,26 +61,24 @@
 
 FILE_SIZE_WARNING = 10000000
 IMAGE_SIZE_WARNING = 5000000
 
 logger = logging.getLogger(__name__)
 
 
-# Custom Serializers for Dexterity
-
 def get_blob_path(blob):
     """Get the path of a ZODB.blob.Blob instance"""
     connection = blob._p_jar
     connection.setstate(blob)
-    db = blob._p_jar.db()
-    oid = blob._p_oid
-    tid = blob._p_serial
-    return connection._storage.fshelper.layout.getBlobFilePath(blob._p_oid, blob._p_serial)
+    db = connection.db()
+    return db.storage.fshelper.layout.getBlobFilePath(blob._p_oid, blob._p_serial)
 
 
+# Custom Serializers for Dexterity
+
 @adapter(INamedImageField, IDexterityContent, IBase64BlobsMarker)
 class ImageFieldSerializerWithBlobs(DefaultFieldSerializer):
     def __call__(self):
         try:
             image = self.field.get(self.context)
         except AttributeError:
             image = None
```

### Comparing `collective.exportimport-1.8/src/collective/exportimport/templates/export_content.pt` & `collective.exportimport-1.9/src/collective/exportimport/templates/export_content.pt`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/templates/export_other.pt` & `collective.exportimport-1.9/src/collective/exportimport/templates/export_other.pt`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/templates/import_content.pt` & `collective.exportimport-1.9/src/collective/exportimport/templates/import_content.pt`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/templates/import_defaultpages.pt` & `collective.exportimport-1.9/src/collective/exportimport/templates/import_defaultpages.pt`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/templates/import_discussion.pt` & `collective.exportimport-1.9/src/collective/exportimport/templates/import_discussion.pt`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/templates/import_localroles.pt` & `collective.exportimport-1.9/src/collective/exportimport/templates/import_localroles.pt`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/templates/import_members.pt` & `collective.exportimport-1.9/src/collective/exportimport/templates/import_members.pt`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/templates/import_ordering.pt` & `collective.exportimport-1.9/src/collective/exportimport/templates/import_ordering.pt`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/templates/import_portlets.pt` & `collective.exportimport-1.9/src/collective/exportimport/templates/import_portlets.pt`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/templates/import_redirects.pt` & `collective.exportimport-1.9/src/collective/exportimport/templates/import_redirects.pt`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/templates/import_relations.pt` & `collective.exportimport-1.9/src/collective/exportimport/templates/import_relations.pt`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/templates/import_translations.pt` & `collective.exportimport-1.9/src/collective/exportimport/templates/import_translations.pt`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/templates/links.pt` & `collective.exportimport-1.9/src/collective/exportimport/templates/links.pt`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/testing.py` & `collective.exportimport-1.9/src/collective/exportimport/testing.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/tests/file.pdf` & `collective.exportimport-1.9/src/collective/exportimport/tests/file.pdf`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/tests/test_drop_and_include.py` & `collective.exportimport-1.9/src/collective/exportimport/tests/test_drop_and_include.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/tests/test_export.py` & `collective.exportimport-1.9/src/collective/exportimport/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/tests/test_fix_html.py` & `collective.exportimport-1.9/src/collective/exportimport/tests/test_fix_html.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/tests/test_import.py` & `collective.exportimport-1.9/src/collective/exportimport/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective/exportimport/tests/test_setup.py` & `collective.exportimport-1.9/src/collective/exportimport/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/src/collective.exportimport.egg-info/PKG-INFO` & `collective.exportimport-1.9/src/collective.exportimport.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.exportimport
-Version: 1.8
+Version: 1.9
 Summary: An add-on for Plone to Export and import content, members, relations, translations and localroles.
 Home-page: https://github.com/collective/collective.exportimport
 Author: Philip Bauer (for starzel.de)
 Author-email: info@starzel.de
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.exportimport
 Project-URL: Source, https://github.com/collective/collective.exportimport
@@ -118,14 +118,26 @@
 .. image:: ./docs/import.png
 
 
 The imports for members, relations, localroles and relations are linked to in this form but can also be called individually: ``/@@import_members``, ``/@@import_relations``, ``/@@import_localroles``, ``/@@import_translations``, ``/@@import_ordering``, ``/@@import_discussion``.
 
 As a last step in a migration there is another view ``@@reset_dates`` that resets the modified date on imported content to the date initially contained in the imported json-file. This is necessary since varous changes during a migration will likely result in a updated modified-date. During import the original is stored as ``obj.modification_date_migrated`` on each new object and this view sets this date.
 
+Export- and import locations
+----------------------------
+
+If you select 'Save to file on server', the Export view will save json files in the <var> directory of your Plone instanc in /var/instance.
+The import view will look for  files under /var/instance/import.
+These directories will normally be different, under different Plone instances and possibly on different servers. 
+
+You can set the environment variable 'COLLECTIVE_EXPORTIMPORT_CENTRAL_DIRECTORY' to add a 'shared' directory on one server or maybe network share.
+With this variable set, collective.exportimport will both save to and load .json files from the same server directory. 
+This saves time not having to move .json files around from the export- to the import location.
+You should be aware that the Export views will overwrite any existing previous .json file export that have the same name. 
+
 
 Use-cases
 =========
 
 Migrations
 ----------
 
@@ -2269,19 +2281,49 @@
 - Leonardo J. Caballero G., leonardocaballero@gmail.com
 
 
 Changelog
 =========
 
 
+1.9 (2023-05-18)
+----------------
+
+- Allow passing custom filenames to exports
+  [pbauer]
+
+- Support export and import of Plone Site root (using update strategy).
+  [pbauer]
+
+- Fix blob export when Connection uses TmpStore
+  [gotcha, pbauer]
+
+- Fix portlet richtext field import
+  [mpeeters]
+
+- Add portlet location on exported data
+  [mpeeters]
+
+- Migrate root of portlets that used a path in plone4 to using a uid (navigation, search, events, collection).
+  [pbauer]
+
+- Make export of discussions and portlets contextual
+  [mpeeters]
+
+- Fix critical bug when importing groups: Do not import groups that a groups belongs to as members of the new group.
+  This could have caused groups to have more privileges than they should.
+  [pbauer]
+
+
 1.8 (2023-04-20)
 ----------------
 
 - Import: run set_uuid method before we call custom hooks, so the hooks have access to
   the item UUID. Fix #185.
+- Document COLLECTIVE_EXPORTIMPORT_CENTRAL_DIRECTORY in README.
   [fredvd]
 
 - Add Spanish translation.
   [macagua]
 
 - Add i18n support.
   [macagua]
@@ -2308,15 +2350,15 @@
 
 - Better serialization of Topics:
   - Use newer criteria added in Plone 5
   - Add fallback for some criteria
   - Export sort_on and sort_reversed
   - Export customView as tabular_view
   [pbauer]
-  
+
 - Always import discussions independent if discussion support is enabled or not
   on a particular content object (#182)
   [ajung]
 
 
 1.7 (2023-01-20)
 ----------------
```

### Comparing `collective.exportimport-1.8/src/collective.exportimport.egg-info/SOURCES.txt` & `collective.exportimport-1.9/src/collective.exportimport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.exportimport-1.8/tox.ini` & `collective.exportimport-1.9/tox.ini`

 * *Files identical despite different names*

