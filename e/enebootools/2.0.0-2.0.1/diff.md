# Comparing `tmp/enebootools-2.0.0.tar.gz` & `tmp/enebootools-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enebootools-2.0.0.tar", last modified: Tue May  9 13:18:26 2023, max compression
+gzip compressed data, was "enebootools-2.0.1.tar", last modified: Thu May 18 09:31:21 2023, max compression
```

## Comparing `enebootools-2.0.0.tar` & `enebootools-2.0.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.113034 enebootools-2.0.0/
--rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.0.0/AUTHORS
--rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.0.0/LICENSE.gplv3
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-09 13:18:26.113034 enebootools-2.0.0/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.0.0/README.rst
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-05-09 13:16:06.000000 enebootools-2.0.0/enebootools/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.0.0/enebootools/__init__.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools/assembler/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6000 2022-12-07 09:30:25.000000 enebootools-2.0.0/enebootools/assembler/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/assembler/config.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29507 2022-12-01 09:57:04.000000 enebootools-2.0.0/enebootools/assembler/database.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/assembler/databasemodels.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.0.0/enebootools/assembler/featureconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    23182 2023-05-09 13:12:22.000000 enebootools-2.0.0/enebootools/assembler/kobjects.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/assembler/mypeewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.0.0/enebootools/assembler/save_auto.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools/autoconfig/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.0/enebootools/autoconfig/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.0.0/enebootools/autoconfig/autoconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/autoconfig/parsers.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools/config/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.0/enebootools/config/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools/crypto/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/crypto/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools/crypto/certificates/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/crypto/certificates/CA_Test_Partners.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/crypto/certificates/Partner_Test.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/crypto/certificates/Partner_Test.pem
--rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/crypto/certificates/README.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/crypto/certificates/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.0.0/enebootools/crypto/main.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools/databaseadmin/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.0/enebootools/databaseadmin/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.109034 enebootools-2.0.0/enebootools/databaseadmin/dblayer/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/databaseadmin/dblayer/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/databaseadmin/dblayer/drivers.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.0.0/enebootools/entry_points.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.109034 enebootools-2.0.0/enebootools/extracttool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/extracttool/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/extracttool/extractfunctions.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.109034 enebootools-2.0.0/enebootools/lib/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.0/enebootools/lib/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.109034 enebootools-2.0.0/enebootools/lib/etree/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.0.0/enebootools/lib/etree/ElementInclude.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/lib/etree/ElementPath.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/lib/etree/ElementTree.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.0.0/enebootools/lib/etree/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.0.0/enebootools/lib/etree/cElementTree.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/lib/peewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/lib/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.109034 enebootools-2.0.0/enebootools/mergetool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    25980 2023-05-09 12:42:37.000000 enebootools-2.0.0/enebootools/mergetool/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.109034 enebootools-2.0.0/enebootools/mergetool/etc/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/mergetool/etc/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.113034 enebootools-2.0.0/enebootools/mergetool/etc/formats/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/mergetool/etc/formats/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/formats/aq23-kut.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.0.0/enebootools/mergetool/etc/formats/aq23-mtd.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/formats/aq23-xml.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/formats/qt3-ts.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/formats/qt3-ui.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/index.xml
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.113034 enebootools-2.0.0/enebootools/mergetool/etc/patch-styles/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/mergetool/etc/patch-styles/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
--rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/patch-styles/legacy1.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.0.0/enebootools/mergetool/etc/patch-styles/semantic1.xml
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76864 2023-05-09 12:45:28.000000 enebootools-2.0.0/enebootools/mergetool/flpatchapipy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    31272 2023-05-09 12:42:28.000000 enebootools-2.0.0/enebootools/mergetool/flpatchdir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    44114 2022-12-01 11:18:08.000000 enebootools-2.0.0/enebootools/mergetool/flpatchlxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77764 2022-09-28 07:55:55.000000 enebootools-2.0.0/enebootools/mergetool/flpatchmodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-09 12:25:44.000000 enebootools-2.0.0/enebootools/mergetool/flpatchpy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77369 2022-03-06 07:56:52.000000 enebootools-2.0.0/enebootools/mergetool/flpatchqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.0.0/enebootools/mergetool/flpatchtest.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/mergetool/flpatchxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3680 2022-12-01 13:23:45.000000 enebootools-2.0.0/enebootools/mergetool/projectbuilder.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.113034 enebootools-2.0.0/enebootools/mergetool/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.0.0/enebootools/mergetool/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.0.0/enebootools/mergetool/test/test_mergetool.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.113034 enebootools-2.0.0/enebootools/packager/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-2.0.0/enebootools/packager/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-2.0.0/enebootools/packager/pkgjoiner.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/packager/pkgsplitter.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.0.0/enebootools/parseargs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.0.0/enebootools/parseargs.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.113034 enebootools-2.0.0/enebootools/parser/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.0.0/enebootools/parser/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.113034 enebootools-2.0.0/enebootools/vcsworkflow/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.0.0/enebootools/vcsworkflow/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-09 13:18:26.105034 enebootools-2.0.0/enebootools.egg-info/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-09 13:18:25.000000 enebootools-2.0.0/enebootools.egg-info/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2874 2023-05-09 13:18:26.000000 enebootools-2.0.0/enebootools.egg-info/SOURCES.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-09 13:18:25.000000 enebootools-2.0.0/enebootools.egg-info/dependency_links.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-05-09 13:18:25.000000 enebootools-2.0.0/enebootools.egg-info/entry_points.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-09 13:18:25.000000 enebootools-2.0.0/enebootools.egg-info/requires.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-05-09 13:18:25.000000 enebootools-2.0.0/enebootools.egg-info/top_level.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-05-09 13:18:26.113034 enebootools-2.0.0/setup.cfg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.0.0/setup.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.633914 enebootools-2.0.1/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.0.1/AUTHORS
+-rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.0.1/LICENSE.gplv3
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-18 09:31:21.629913 enebootools-2.0.1/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.0.1/README.rst
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.613913 enebootools-2.0.1/enebootools/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-05-18 09:12:28.000000 enebootools-2.0.1/enebootools/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.0.1/enebootools/__init__.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.617913 enebootools-2.0.1/enebootools/assembler/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6326 2023-05-18 09:15:32.000000 enebootools-2.0.1/enebootools/assembler/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/assembler/config.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    29859 2023-05-18 09:20:33.000000 enebootools-2.0.1/enebootools/assembler/database.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/assembler/databasemodels.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.0.1/enebootools/assembler/featureconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    23182 2023-05-09 13:12:22.000000 enebootools-2.0.1/enebootools/assembler/kobjects.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/assembler/mypeewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.0.1/enebootools/assembler/save_auto.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.617913 enebootools-2.0.1/enebootools/autoconfig/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.1/enebootools/autoconfig/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.0.1/enebootools/autoconfig/autoconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/autoconfig/parsers.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.617913 enebootools-2.0.1/enebootools/config/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.1/enebootools/config/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.617913 enebootools-2.0.1/enebootools/crypto/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/crypto/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.621913 enebootools-2.0.1/enebootools/crypto/certificates/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/crypto/certificates/CA_Test_Partners.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/crypto/certificates/Partner_Test.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/crypto/certificates/Partner_Test.pem
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/crypto/certificates/README.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/crypto/certificates/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.0.1/enebootools/crypto/main.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.621913 enebootools-2.0.1/enebootools/databaseadmin/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.1/enebootools/databaseadmin/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.621913 enebootools-2.0.1/enebootools/databaseadmin/dblayer/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/databaseadmin/dblayer/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/databaseadmin/dblayer/drivers.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.0.1/enebootools/entry_points.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.621913 enebootools-2.0.1/enebootools/extracttool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/extracttool/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/extracttool/extractfunctions.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.621913 enebootools-2.0.1/enebootools/lib/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.1/enebootools/lib/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.625913 enebootools-2.0.1/enebootools/lib/etree/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.0.1/enebootools/lib/etree/ElementInclude.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/lib/etree/ElementPath.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/lib/etree/ElementTree.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.0.1/enebootools/lib/etree/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.0.1/enebootools/lib/etree/cElementTree.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/lib/peewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/lib/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.625913 enebootools-2.0.1/enebootools/mergetool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    25980 2023-05-09 12:42:37.000000 enebootools-2.0.1/enebootools/mergetool/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.629913 enebootools-2.0.1/enebootools/mergetool/etc/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/mergetool/etc/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.629913 enebootools-2.0.1/enebootools/mergetool/etc/formats/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/mergetool/etc/formats/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/formats/aq23-kut.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.0.1/enebootools/mergetool/etc/formats/aq23-mtd.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/formats/aq23-xml.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/formats/qt3-ts.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/formats/qt3-ui.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/index.xml
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.629913 enebootools-2.0.1/enebootools/mergetool/etc/patch-styles/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/mergetool/etc/patch-styles/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/patch-styles/legacy1.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/patch-styles/semantic1.xml
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76872 2023-05-17 19:00:59.000000 enebootools-2.0.1/enebootools/mergetool/flpatchapipy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    31272 2023-05-09 12:42:28.000000 enebootools-2.0.1/enebootools/mergetool/flpatchdir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    44114 2022-12-01 11:18:08.000000 enebootools-2.0.1/enebootools/mergetool/flpatchlxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77764 2022-09-28 07:55:55.000000 enebootools-2.0.1/enebootools/mergetool/flpatchmodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-09 12:25:44.000000 enebootools-2.0.1/enebootools/mergetool/flpatchpy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77369 2022-03-06 07:56:52.000000 enebootools-2.0.1/enebootools/mergetool/flpatchqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.0.1/enebootools/mergetool/flpatchtest.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/mergetool/flpatchxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3680 2022-12-01 13:23:45.000000 enebootools-2.0.1/enebootools/mergetool/projectbuilder.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.629913 enebootools-2.0.1/enebootools/mergetool/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.0.1/enebootools/mergetool/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.0.1/enebootools/mergetool/test/test_mergetool.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.629913 enebootools-2.0.1/enebootools/packager/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-2.0.1/enebootools/packager/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-2.0.1/enebootools/packager/pkgjoiner.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/packager/pkgsplitter.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.0.1/enebootools/parseargs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.0.1/enebootools/parseargs.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.629913 enebootools-2.0.1/enebootools/parser/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.0.1/enebootools/parser/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.629913 enebootools-2.0.1/enebootools/vcsworkflow/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/vcsworkflow/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.613913 enebootools-2.0.1/enebootools.egg-info/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-18 09:31:21.000000 enebootools-2.0.1/enebootools.egg-info/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2874 2023-05-18 09:31:21.000000 enebootools-2.0.1/enebootools.egg-info/SOURCES.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-18 09:31:21.000000 enebootools-2.0.1/enebootools.egg-info/dependency_links.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-05-18 09:31:21.000000 enebootools-2.0.1/enebootools.egg-info/entry_points.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-18 09:31:21.000000 enebootools-2.0.1/enebootools.egg-info/requires.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-05-18 09:31:21.000000 enebootools-2.0.1/enebootools.egg-info/top_level.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-05-18 09:31:21.633914 enebootools-2.0.1/setup.cfg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.0.1/setup.py
```

### Comparing `enebootools-2.0.0/LICENSE.gplv3` & `enebootools-2.0.1/LICENSE.gplv3`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/PKG-INFO` & `enebootools-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 2.0.0
+Version: 2.0.1
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-2.0.0/README.rst` & `enebootools-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/__init__.py` & `enebootools-2.0.1/enebootools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os.path
 import sys
 import traceback
 from pprint import pformat
 import enebootools.parseargs as pa
 
 
-__VERSION__ = "2.0.0"
+__VERSION__ = "2.0.1"
 QS_EXTEND_MODE = "legacy"
 
 
 def ustr(value):
     """Ustr."""
     if isinstance(value, str):
         return value
```

### Comparing `enebootools-2.0.0/enebootools/__init__.pyc` & `enebootools-2.0.1/enebootools/__init__.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/assembler/__init__.py` & `enebootools-2.0.1/enebootools/assembler/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 class AssemblerInterface(EnebooToolsInterface):
     module_description = "Herramientas de gestión de proyectos de mezcla"
 
     def __init__(self, setup_parser=True):
         EnebooToolsInterface.__init__(self, False)
+        self.short_mode = False
         if setup_parser:
             self.setup_parser()
 
     def setup_parser(self):
         EnebooToolsInterface.setup_parser(self)
 
         self.new_action = self.parser.declare_action(
@@ -113,14 +114,22 @@
             call_function=self.do_howto_build,
         )
         self.howto_build_action.set_help_arg(
             target="Objetivo a construir",
             feat="Funcionalidad a construir",
         )
 
+        self.parser.declare_option(
+            name="short",
+            short="s",
+            description="Usa el modo de definiciones corto",
+            level="parser",
+            call_function=self.set_short_mode,
+        )
+
     # :::: ACTIONS ::::
 
     def do_dbupdate(self):
         try:
             return asmdb.update_database(self)
         except Exception as e:
             self.exception(type(e).__name__, str(e))
@@ -171,7 +180,10 @@
             self.exception(type(e).__name__, str(e))
 
     def do_new(self, subfoldername=None, description=None, patchurl=None):
         try:
             return asmdb.do_new(self, subfoldername, description, patchurl)
         except Exception as e:
             self.exception(type(e).__name__, str(e))
+
+    def set_short_mode(self):
+        self.short_mode = True
```

### Comparing `enebootools-2.0.0/enebootools/assembler/config.py` & `enebootools-2.0.1/enebootools/assembler/config.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/assembler/database.py` & `enebootools-2.0.1/enebootools/assembler/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -557,15 +557,18 @@
         except Exception as e:
             print(
                 "Hubo un problema al intentar comprobar el parche."
                 + " Probablemente la carpeta sea incorrecta."
             )
 
     while True:
-        fdstpath = os.path.join(fpath, "%s%s-%s" % (ftype, fcode, fname))
+        if iface.short_mode:
+            fdstpath = os.path.join(fpath, "%s" % (fname))
+        else:
+            fdstpath = os.path.join(fpath, "%s%s-%s" % (ftype, fcode, fname))
         print()
         print("**** Asistente de creación de nueva funcionalidad ****")
         print()
         print(" : Carpeta destino : %s" % fdstpath)
         print(" : Nombre          : %s - %s - %s " % (ftype_idx[ftype], fcode, fname))
         print(" : Descripción     : %s " % (fdesc))
         print()
@@ -675,15 +678,18 @@
                         callback=lambda a, o: fdep_modules.remove(o),
                     )
                 if a2 == "+f":
                     # Agregar dependencia funcionalidad
                     k1 = []
                     v1 = []
                     for feature in oi.features():
-                        k, v = feature.code or feature.name, feature.formal_name()
+                        k, v = (
+                            feature.code or feature.name,
+                            feature.name if iface.short_mode else feature.formal_name(),
+                        )
                         if v in fdep_features:
                             continue
                         k1.append(k)
                         v1.append(v)
 
                     select_option(
                         title="--  Agregar dependencia de funcionalidad --",
@@ -694,15 +700,18 @@
                         callback=lambda a, o: fdep_features.append(o),
                     )
                 if a2 == "-f":
                     # Eliminar dependencia funcionalidad
                     k1 = []
                     v1 = []
                     for feature in oi.features():
-                        k, v = feature.code or feature.name, feature.formal_name()
+                        k, v = (
+                            feature.code or feature.name,
+                            feature.name if iface.short_mode else feature.formal_name(),
+                        )
                         if v not in fdep_features:
                             continue
                         k1.append(k)
                         v1.append(v)
 
                     select_option(
                         title="--  Eliminar dependencia de funcionalidad --",
```

### Comparing `enebootools-2.0.0/enebootools/assembler/databasemodels.py` & `enebootools-2.0.1/enebootools/assembler/databasemodels.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/assembler/featureconfig.py` & `enebootools-2.0.1/enebootools/assembler/featureconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/assembler/kobjects.py` & `enebootools-2.0.1/enebootools/assembler/kobjects.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/assembler/mypeewee.py` & `enebootools-2.0.1/enebootools/assembler/mypeewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/assembler/save_auto.py` & `enebootools-2.0.1/enebootools/assembler/save_auto.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/autoconfig/autoconfig.py` & `enebootools-2.0.1/enebootools/autoconfig/autoconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/autoconfig/parsers.py` & `enebootools-2.0.1/enebootools/autoconfig/parsers.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/crypto/__init__.py` & `enebootools-2.0.1/enebootools/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt` & `enebootools-2.0.1/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/crypto/certificates/CA_Test_Partners.crt` & `enebootools-2.0.1/enebootools/crypto/certificates/CA_Test_Partners.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt` & `enebootools-2.0.1/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/crypto/certificates/Partner_Test.crt` & `enebootools-2.0.1/enebootools/crypto/certificates/Partner_Test.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/crypto/certificates/Partner_Test.pem` & `enebootools-2.0.1/enebootools/crypto/certificates/Partner_Test.pem`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/crypto/certificates/README.txt` & `enebootools-2.0.1/enebootools/crypto/certificates/README.txt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/crypto/main.py` & `enebootools-2.0.1/enebootools/crypto/main.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/databaseadmin/dblayer/drivers.py` & `enebootools-2.0.1/enebootools/databaseadmin/dblayer/drivers.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/entry_points.py` & `enebootools-2.0.1/enebootools/entry_points.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/extracttool/__init__.py` & `enebootools-2.0.1/enebootools/extracttool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/extracttool/extractfunctions.py` & `enebootools-2.0.1/enebootools/extracttool/extractfunctions.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/lib/etree/ElementInclude.py` & `enebootools-2.0.1/enebootools/lib/etree/ElementInclude.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/lib/etree/ElementPath.py` & `enebootools-2.0.1/enebootools/lib/etree/ElementPath.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/lib/etree/ElementTree.py` & `enebootools-2.0.1/enebootools/lib/etree/ElementTree.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/lib/etree/__init__.py` & `enebootools-2.0.1/enebootools/lib/etree/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/lib/peewee.py` & `enebootools-2.0.1/enebootools/lib/peewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/lib/utils.py` & `enebootools-2.0.1/enebootools/lib/utils.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/__init__.py` & `enebootools-2.0.1/enebootools/mergetool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/etc/formats/aq23-kut.xml` & `enebootools-2.0.1/enebootools/mergetool/etc/formats/aq23-kut.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/etc/formats/aq23-mtd.xml` & `enebootools-2.0.1/enebootools/mergetool/etc/formats/aq23-mtd.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/etc/formats/aq23-xml.xml` & `enebootools-2.0.1/enebootools/mergetool/etc/formats/aq23-xml.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/etc/formats/qt3-ts.xml` & `enebootools-2.0.1/enebootools/mergetool/etc/formats/qt3-ts.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/etc/formats/qt3-ui.xml` & `enebootools-2.0.1/enebootools/mergetool/etc/formats/qt3-ui.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/etc/index.xml` & `enebootools-2.0.1/enebootools/mergetool/etc/index.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl` & `enebootools-2.0.1/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/etc/patch-styles/legacy1.xml` & `enebootools-2.0.1/enebootools/mergetool/etc/patch-styles/legacy1.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/flpatchapipy.py` & `enebootools-2.0.1/enebootools/mergetool/flpatchapipy.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 
                     if cname in heu_cnames:
                         heu_cname = cname
 
                 if heu_cname:
                     heu_dtype = "class_definition"
 
-            if heu_dtype and dtype != "delete_class":
+            """ if heu_dtype and dtype != "delete_class":
                 heu_line = "# @%s %s #" % (heu_dtype, heu_cname)
                 myline = "# @%s %s #" % (dtype, cname)
                 if "_" in cname:
                     iface.info(
                         "La autodetección de contenido de bloques no funciona con clases que contengan el carácter de guión bajo como %r"
                         % cname
                     )
@@ -218,15 +218,15 @@
                     iface.error(
                         "La definición de bloque %r no corresponde con el contenido (file: %s:%d) ... asumiendo '%s'"
                         % (line2.strip(), file_name, n, heu_line)
                     )
                     dtype, cname = heu_dtype, heu_cname
                     classpatch += ["@@ -%d,1 +%d,1 @@" % (n + 1, n + 1)]
                     classpatch += ["-%s" % line2.rstrip()]
-                    classpatch += ["+%s" % heu_line]
+                    classpatch += ["+%s" % heu_line] """
 
             npos = len(linelist)
             if dtype == "class_declaration":
                 if cname in classes:
                     iface.error(
                         "Hay dos bloques 'class_declaration' para la clase %s (file: %s) ... asumiendo 'class_definiton'"
                         % (cname, file_name)
```

### Comparing `enebootools-2.0.0/enebootools/mergetool/flpatchdir.py` & `enebootools-2.0.1/enebootools/mergetool/flpatchdir.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/flpatchlxml.py` & `enebootools-2.0.1/enebootools/mergetool/flpatchlxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/flpatchmodel.py` & `enebootools-2.0.1/enebootools/mergetool/flpatchmodel.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/flpatchpy.py` & `enebootools-2.0.1/enebootools/mergetool/flpatchpy.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/flpatchqs.py` & `enebootools-2.0.1/enebootools/mergetool/flpatchqs.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/flpatchtest.py` & `enebootools-2.0.1/enebootools/mergetool/flpatchtest.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/flpatchxml.py` & `enebootools-2.0.1/enebootools/mergetool/flpatchxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/projectbuilder.py` & `enebootools-2.0.1/enebootools/mergetool/projectbuilder.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/test/__init__.py` & `enebootools-2.0.1/enebootools/mergetool/test/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/mergetool/test/test_mergetool.py` & `enebootools-2.0.1/enebootools/mergetool/test/test_mergetool.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/packager/__init__.py` & `enebootools-2.0.1/enebootools/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/packager/pkgjoiner.py` & `enebootools-2.0.1/enebootools/packager/pkgjoiner.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/packager/pkgsplitter.py` & `enebootools-2.0.1/enebootools/packager/pkgsplitter.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/parseargs.py` & `enebootools-2.0.1/enebootools/parseargs.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools/parseargs.pyc` & `enebootools-2.0.1/enebootools/parseargs.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/enebootools.egg-info/PKG-INFO` & `enebootools-2.0.1/enebootools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 2.0.0
+Version: 2.0.1
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-2.0.0/enebootools.egg-info/SOURCES.txt` & `enebootools-2.0.1/enebootools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.0/setup.py` & `enebootools-2.0.1/setup.py`

 * *Files identical despite different names*

