# Comparing `tmp/html2notion-0.1.9.tar.gz` & `tmp/html2notion-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2notion-0.1.9.tar", last modified: Sun May 14 05:53:25 2023, max compression
+gzip compressed data, was "html2notion-0.2.0.tar", last modified: Thu May 18 13:15:52 2023, max compression
```

## Comparing `html2notion-0.1.9.tar` & `html2notion-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-05-14 05:53:25.051017 html2notion-0.1.9/
--rw-r--r--   0 feizhao    (501) staff       (20)     1064 2023-03-22 13:58:21.000000 html2notion-0.1.9/LICENSE
--rw-r--r--   0 feizhao    (501) staff       (20)     4600 2023-05-14 05:53:25.052676 html2notion-0.1.9/PKG-INFO
--rw-r--r--   0 feizhao    (501) staff       (20)     4111 2023-04-22 07:11:47.000000 html2notion-0.1.9/README.md
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-05-14 05:53:25.001062 html2notion-0.1.9/html2notion/
--rw-r--r--   0 feizhao    (501) staff       (20)        0 2023-03-18 15:41:01.000000 html2notion-0.1.9/html2notion/__init__.py
--rw-r--r--   0 feizhao    (501) staff       (20)     6037 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/main.py
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-05-14 05:53:25.037976 html2notion-0.1.9/html2notion/translate/
--rw-r--r--   0 feizhao    (501) staff       (20)        0 2023-04-08 10:17:44.000000 html2notion-0.1.9/html2notion/translate/__init__.py
--rw-r--r--   0 feizhao    (501) staff       (20)     3610 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/translate/batch_import.py
--rw-r--r--   0 feizhao    (501) staff       (20)     2724 2023-04-19 14:40:39.000000 html2notion-0.1.9/html2notion/translate/cos_uploader.py
--rw-r--r--   0 feizhao    (501) staff       (20)     4546 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/translate/html2json.py
--rw-r--r--   0 feizhao    (501) staff       (20)    17995 2023-05-14 05:46:27.000000 html2notion-0.1.9/html2notion/translate/html2json_base.py
--rw-r--r--   0 feizhao    (501) staff       (20)     5810 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/translate/html2json_clipper.py
--rw-r--r--   0 feizhao    (501) staff       (20)      534 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/translate/html2json_default.py
--rw-r--r--   0 feizhao    (501) staff       (20)     8707 2023-05-14 05:22:26.000000 html2notion-0.1.9/html2notion/translate/html2json_markdown.py
--rw-r--r--   0 feizhao    (501) staff       (20)     7300 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/translate/html2json_yinxiang.py
--rw-r--r--   0 feizhao    (501) staff       (20)     2331 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/translate/import_stats.py
--rw-r--r--   0 feizhao    (501) staff       (20)     7168 2023-04-23 14:40:05.000000 html2notion-0.1.9/html2notion/translate/notion_export.py
--rw-r--r--   0 feizhao    (501) staff       (20)     3594 2023-05-13 08:31:32.000000 html2notion-0.1.9/html2notion/translate/notion_import.py
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-05-14 05:53:25.042565 html2notion-0.1.9/html2notion/utils/
--rw-r--r--   0 feizhao    (501) staff       (20)      453 2023-04-29 09:56:35.000000 html2notion-0.1.9/html2notion/utils/__init__.py
--rw-r--r--   0 feizhao    (501) staff       (20)      895 2023-04-29 09:55:54.000000 html2notion-0.1.9/html2notion/utils/load_config.py
--rw-r--r--   0 feizhao    (501) staff       (20)     1579 2023-04-20 14:39:58.000000 html2notion-0.1.9/html2notion/utils/log.py
--rw-r--r--   0 feizhao    (501) staff       (20)      437 2023-04-21 14:23:32.000000 html2notion-0.1.9/html2notion/utils/timeutil.py
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-05-14 05:53:25.008065 html2notion-0.1.9/html2notion.egg-info/
--rw-r--r--   0 feizhao    (501) staff       (20)     4600 2023-05-14 05:53:24.000000 html2notion-0.1.9/html2notion.egg-info/PKG-INFO
--rw-r--r--   0 feizhao    (501) staff       (20)     1023 2023-05-14 05:53:24.000000 html2notion-0.1.9/html2notion.egg-info/SOURCES.txt
--rw-r--r--   0 feizhao    (501) staff       (20)        1 2023-05-14 05:53:24.000000 html2notion-0.1.9/html2notion.egg-info/dependency_links.txt
--rw-r--r--   0 feizhao    (501) staff       (20)       54 2023-05-14 05:53:24.000000 html2notion-0.1.9/html2notion.egg-info/entry_points.txt
--rw-r--r--   0 feizhao    (501) staff       (20)      203 2023-05-14 05:53:24.000000 html2notion-0.1.9/html2notion.egg-info/requires.txt
--rw-r--r--   0 feizhao    (501) staff       (20)       12 2023-05-14 05:53:24.000000 html2notion-0.1.9/html2notion.egg-info/top_level.txt
--rw-r--r--   0 feizhao    (501) staff       (20)      103 2023-03-18 15:06:24.000000 html2notion-0.1.9/pyproject.toml
--rw-r--r--   0 feizhao    (501) staff       (20)      887 2023-05-14 05:53:25.057687 html2notion-0.1.9/setup.cfg
--rw-r--r--   0 feizhao    (501) staff       (20)       38 2023-03-18 07:34:12.000000 html2notion-0.1.9/setup.py
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-05-14 05:53:25.048173 html2notion-0.1.9/tests/
--rw-r--r--   0 feizhao    (501) staff       (20)     3940 2023-04-29 10:35:21.000000 html2notion-0.1.9/tests/test_batchimport.py
--rw-r--r--   0 feizhao    (501) staff       (20)     3038 2023-04-20 14:39:58.000000 html2notion-0.1.9/tests/test_cosupload.py
--rw-r--r--   0 feizhao    (501) staff       (20)     2698 2023-04-13 14:42:38.000000 html2notion-0.1.9/tests/test_notionexport.py
--rw-r--r--   0 feizhao    (501) staff       (20)     1801 2023-05-13 08:31:32.000000 html2notion-0.1.9/tests/test_reqlimit.py
--rw-r--r--   0 feizhao    (501) staff       (20)    32686 2023-05-13 08:31:32.000000 html2notion-0.1.9/tests/test_yinxiang.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-18 13:15:52.037252 html2notion-0.2.0/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1064 2023-03-22 08:52:55.000000 html2notion-0.2.0/LICENSE
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     5078 2023-05-18 13:15:52.037538 html2notion-0.2.0/PKG-INFO
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4590 2023-05-16 11:35:35.000000 html2notion-0.2.0/README.md
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-18 13:15:52.018984 html2notion-0.2.0/html2notion/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.2.0/html2notion/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     6303 2023-05-17 12:10:46.000000 html2notion-0.2.0/html2notion/main.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-18 13:15:52.027704 html2notion-0.2.0/html2notion/translate/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.2.0/html2notion/translate/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3610 2023-05-10 11:11:53.000000 html2notion-0.2.0/html2notion/translate/batch_import.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2724 2023-04-19 01:44:49.000000 html2notion-0.2.0/html2notion/translate/cos_uploader.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     5393 2023-05-17 02:24:15.000000 html2notion-0.2.0/html2notion/translate/html2json.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)    22089 2023-05-18 13:04:20.000000 html2notion-0.2.0/html2notion/translate/html2json_base.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     5782 2023-05-16 13:08:51.000000 html2notion-0.2.0/html2notion/translate/html2json_clipper.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      534 2023-05-10 11:11:53.000000 html2notion-0.2.0/html2notion/translate/html2json_default.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     8940 2023-05-18 13:09:34.000000 html2notion-0.2.0/html2notion/translate/html2json_markdown.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     7067 2023-05-18 13:00:56.000000 html2notion-0.2.0/html2notion/translate/html2json_yinxiang.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2649 2023-05-17 02:20:27.000000 html2notion-0.2.0/html2notion/translate/import_stats.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     7168 2023-04-23 11:21:17.000000 html2notion-0.2.0/html2notion/translate/notion_export.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3594 2023-05-12 05:20:31.000000 html2notion-0.2.0/html2notion/translate/notion_import.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-18 13:15:52.032871 html2notion-0.2.0/html2notion/utils/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      566 2023-05-16 12:58:24.000000 html2notion-0.2.0/html2notion/utils/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      792 2023-05-17 05:22:48.000000 html2notion-0.2.0/html2notion/utils/load_config.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1575 2023-05-17 09:53:40.000000 html2notion-0.2.0/html2notion/utils/log.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      576 2023-05-16 12:57:10.000000 html2notion-0.2.0/html2notion/utils/timeutil.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      525 2023-05-16 13:08:07.000000 html2notion-0.2.0/html2notion/utils/url_process.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-18 13:15:52.021400 html2notion-0.2.0/html2notion.egg-info/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     5078 2023-05-18 13:15:51.000000 html2notion-0.2.0/html2notion.egg-info/PKG-INFO
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1075 2023-05-18 13:15:51.000000 html2notion-0.2.0/html2notion.egg-info/SOURCES.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        1 2023-05-18 13:15:51.000000 html2notion-0.2.0/html2notion.egg-info/dependency_links.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       54 2023-05-18 13:15:51.000000 html2notion-0.2.0/html2notion.egg-info/entry_points.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      203 2023-05-18 13:15:51.000000 html2notion-0.2.0/html2notion.egg-info/requires.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       12 2023-05-18 13:15:51.000000 html2notion-0.2.0/html2notion.egg-info/top_level.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      103 2023-03-20 01:38:35.000000 html2notion-0.2.0/pyproject.toml
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      887 2023-05-18 13:15:52.038733 html2notion-0.2.0/setup.cfg
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       38 2023-03-17 05:39:04.000000 html2notion-0.2.0/setup.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-18 13:15:52.036530 html2notion-0.2.0/tests/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3684 2023-05-18 12:47:00.000000 html2notion-0.2.0/tests/test_batchimport.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2787 2023-05-18 12:46:37.000000 html2notion-0.2.0/tests/test_cosupload.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2643 2023-05-18 13:07:22.000000 html2notion-0.2.0/tests/test_notionexport.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1834 2023-05-18 13:01:57.000000 html2notion-0.2.0/tests/test_reqlimit.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1339 2023-05-16 13:22:19.000000 html2notion-0.2.0/tests/test_util.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)    32506 2023-05-18 12:47:19.000000 html2notion-0.2.0/tests/test_yinxiang.py
```

### Comparing `html2notion-0.1.9/LICENSE` & `html2notion-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.9/PKG-INFO` & `html2notion-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6874 6d6c  : 2.1.Name: html
 00000020: 326e 6f74 696f 6e0a 5665 7273 696f 6e3a  2notion.Version:
-00000030: 2030 2e31 2e39 0a53 756d 6d61 7279 3a20   0.1.9.Summary: 
+00000030: 2030 2e32 2e30 0a53 756d 6d61 7279 3a20   0.2.0.Summary: 
 00000040: 5468 6973 2074 6f6f 6c20 6361 6e20 6163  This tool can ac
 00000050: 6375 7261 7465 6c79 2063 6f6e 7665 7274  curately convert
 00000060: 2048 544d 4c20 746f 204e 6f74 696f 6e20   HTML to Notion 
 00000070: 6e6f 7465 7320 616e 6420 6973 2061 6c73  notes and is als
 00000080: 6f20 7573 6566 756c 2066 6f72 2065 7870  o useful for exp
 00000090: 6f72 7469 6e67 2045 7665 726e 6f74 6520  orting Evernote 
 000000a0: 6e6f 7465 7320 746f 204e 6f74 696f 6e2e  notes to Notion.
@@ -24,265 +24,295 @@
 00000170: 5420 4c69 6365 6e73 650a 436c 6173 7369  T License.Classi
 00000180: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
 00000190: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
 000001a0: 6570 656e 6465 6e74 0a44 6573 6372 6970  ependent.Descrip
 000001b0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
 000001c0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
 000001d0: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
-000001e0: 4943 454e 5345 0a0a 5be7 ae80 e4bd 93e4  ICENSE..[.......
-000001f0: b8ad e696 875d 2868 7474 7073 3a2f 2f67  .....](https://g
-00000200: 6974 6875 622e 636f 6d2f 7365 6c66 626f  ithub.com/selfbo
-00000210: 6f74 2f68 746d 6c32 6e6f 7469 6f6e 2f62  ot/html2notion/b
-00000220: 6c6f 622f 6d61 7374 6572 2f52 4541 444d  lob/master/READM
-00000230: 455f 7a68 2e6d 6429 0a0a 6874 6d6c 326e  E_zh.md)..html2n
-00000240: 6f74 696f 6e20 6973 2061 6e20 696e 6372  otion is an incr
-00000250: 6564 6962 6c79 2075 7365 6675 6c20 746f  edibly useful to
-00000260: 6f6c 2077 7269 7474 656e 2069 6e20 5079  ol written in Py
-00000270: 7468 6f6e 2c20 7768 6963 6820 616c 6c6f  thon, which allo
-00000280: 7773 2079 6f75 2074 6f20 696d 706f 7274  ws you to import
-00000290: 2063 6f6e 7465 6e74 2066 726f 6d20 4854   content from HT
-000002a0: 4d4c 2064 6f63 756d 656e 7473 2069 6e74  ML documents int
-000002b0: 6f20 4e6f 7469 6f6e 206e 6f74 6573 2c20  o Notion notes, 
-000002c0: 6d61 6b69 6e67 2069 7420 6d6f 7265 2063  making it more c
-000002d0: 6f6e 7665 6e69 656e 7420 666f 7220 796f  onvenient for yo
-000002e0: 7520 746f 206f 7267 616e 697a 6520 696e  u to organize in
-000002f0: 666f 726d 6174 696f 6e20 6f6e 2074 6865  formation on the
-00000300: 204e 6f74 696f 6e20 706c 6174 666f 726d   Notion platform
-00000310: 2e20 496e 2061 6464 6974 696f 6e2c 2068  . In addition, h
-00000320: 746d 6c32 6e6f 7469 6f6e 2068 6173 2062  tml2notion has b
-00000330: 6565 6e20 7370 6563 6966 6963 616c 6c79  een specifically
-00000340: 206f 7074 696d 697a 6564 2066 6f72 2074   optimized for t
-00000350: 6865 2063 6f6e 7465 6e74 206f 6620 4576  he content of Ev
-00000360: 6572 6e6f 7465 2c20 616e 6420 796f 7520  ernote, and you 
-00000370: 6361 6e20 616c 736f 2075 7365 2069 7420  can also use it 
-00000380: 746f 2069 6d70 6f72 7420 6e6f 7465 7320  to import notes 
-00000390: 6672 6f6d 2045 7665 726e 6f74 6520 696e  from Evernote in
-000003a0: 746f 204e 6f74 696f 6e2e 0a0a 6874 6d6c  to Notion...html
-000003b0: 326e 6f74 696f 6e20 6861 7320 706f 7765  2notion has powe
-000003c0: 7266 756c 2066 6561 7475 7265 7320 616e  rful features an
-000003d0: 6420 7375 7070 6f72 7473 2063 6f6e 7665  d supports conve
-000003e0: 7274 696e 6720 7661 7269 6f75 7320 7461  rting various ta
-000003f0: 6773 2069 6e20 4854 4d4c 2066 696c 6573  gs in HTML files
-00000400: 2069 6e74 6f20 636f 7272 6573 706f 6e64   into correspond
-00000410: 696e 6720 426c 6f63 6b73 2069 6e20 4e6f  ing Blocks in No
-00000420: 7469 6f6e 2c20 7375 6368 2061 7320 7269  tion, such as ri
-00000430: 6368 2074 6578 7420 626c 6f63 6b73 2c20  ch text blocks, 
-00000440: 6865 6164 696e 6773 2c20 696d 6167 6573  headings, images
-00000450: 2c20 636f 6465 2062 6c6f 636b 732c 2071  , code blocks, q
-00000460: 756f 7465 732c 206c 696e 6b73 2c20 6574  uotes, links, et
-00000470: 632e 2042 656c 6f77 2061 7265 2065 7861  c. Below are exa
-00000480: 6d70 6c65 7320 6f66 2063 6f6e 7665 7274  mples of convert
-00000490: 696e 6720 6e6f 7465 7320 6672 6f6d 2045  ing notes from E
-000004a0: 7665 726e 6f74 6520 696e 746f 204e 6f74  vernote into Not
-000004b0: 696f 6e20 7061 6765 732e 0a0a 215b 7969  ion pages...![yi
-000004c0: 6e78 6961 6e67 206e 6f74 696f 6e28 7369  nxiang notion(si
-000004d0: 6d70 6c65 2064 656d 6f73 295d 2868 7474  mple demos)](htt
-000004e0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-000004f0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
-00000500: 656c 6662 6f6f 742f 6874 6d6c 326e 6f74  elfboot/html2not
-00000510: 696f 6e2f 6d61 7374 6572 2f64 656d 6f73  ion/master/demos
-00000520: 2f79 696e 7869 616e 675f 6e6f 7469 6f6e  /yinxiang_notion
-00000530: 2e70 6e67 290a 0a21 5b79 696e 7869 616e  .png)..![yinxian
-00000540: 6720 6e6f 7469 6f6e 3228 7269 6368 2074  g notion2(rich t
-00000550: 6578 7429 5d28 6874 7470 733a 2f2f 7261  ext)](https://ra
-00000560: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000570: 656e 742e 636f 6d2f 7365 6c66 626f 6f74  ent.com/selfboot
-00000580: 2f68 746d 6c32 6e6f 7469 6f6e 2f6d 6173  /html2notion/mas
-00000590: 7465 722f 6465 6d6f 732f 7969 6e78 6961  ter/demos/yinxia
-000005a0: 6e67 5f6e 6f74 696f 6e32 2e70 6e67 290a  ng_notion2.png).
-000005b0: 0a23 2050 7265 7061 7265 0a0a 596f 7520  .# Prepare..You 
-000005c0: 6f6e 6c79 206e 6565 6420 3320 7374 6570  only need 3 step
-000005d0: 7320 746f 2075 7365 2068 746d 6c6e 6f74  s to use htmlnot
-000005e0: 696f 6e20 746f 2069 6d70 6f72 7420 4854  ion to import HT
-000005f0: 4d4c 2069 6e74 6f20 4e6f 7469 6f6e 2e0a  ML into Notion..
-00000600: 0a23 2320 4475 706c 6963 6174 6520 6461  .## Duplicate da
-00000610: 7461 6261 7365 0a0a 436c 6963 6b20 7468  tabase..Click th
-00000620: 6520 6c69 6e6b 205b 6e6f 7469 6f6e 2074  e link [notion t
-00000630: 656d 706c 6174 655d 2868 7474 7073 3a2f  emplate](https:/
-00000640: 2f73 656c 6662 6f6f 742e 6e6f 7469 6f6e  /selfboot.notion
-00000650: 2e73 6974 652f 7365 6c66 626f 6f74 2f31  .site/selfboot/1
-00000660: 3330 6262 3438 6336 6362 6434 6162 6262  30bb48c6cbd4abbb
-00000670: 6237 3133 6434 6438 3437 3234 3831 613f  b713d4d8472481a?
-00000680: 763d 6464 6461 3230 6433 6634 3662 3462  v=ddda20d3f46b4b
-00000690: 3434 6130 3535 6430 3637 3932 6331 3432  44a055d06792c142
-000006a0: 6630 292e 2041 7320 7368 6f77 6e20 696e  f0). As shown in
-000006b0: 2074 6865 2069 6d61 6765 2062 656c 6f77   the image below
-000006c0: 2c20 7573 6520 7468 6520 2244 7570 6c69  , use the "Dupli
-000006d0: 6361 7465 2220 6275 7474 6f6e 2074 6f20  cate" button to 
-000006e0: 636f 7079 2061 206e 6577 2064 6174 6162  copy a new datab
-000006f0: 6173 6520 746f 2079 6f75 7220 6f77 6e20  ase to your own 
-00000700: 4e6f 7469 6f6e 2077 6f72 6b73 7061 6365  Notion workspace
-00000710: 2e0a 0a21 5b6e 6f74 696f 6e20 7465 6d70  ...![notion temp
-00000720: 6c61 7465 5d28 6874 7470 733a 2f2f 7261  late](https://ra
-00000730: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000740: 656e 742e 636f 6d2f 7365 6c66 626f 6f74  ent.com/selfboot
-00000750: 2f68 746d 6c32 6e6f 7469 6f6e 2f6d 6173  /html2notion/mas
-00000760: 7465 722f 6465 6d6f 732f 6e6f 7469 6f6e  ter/demos/notion
-00000770: 5f74 656d 706c 6167 652e 706e 6729 0a0a  _templage.png)..
-00000780: 2323 2049 6e73 7461 6c6c 2068 746d 6c32  ## Install html2
-00000790: 6e6f 7469 6f6e 0a0a 5265 7175 6972 6573  notion..Requires
-000007a0: 2070 7974 686f 6e3e 3d33 2e38 2c20 696e   python>=3.8, in
-000007b0: 7374 616c 6c20 7468 6520 6874 6d6c 326e  stall the html2n
-000007c0: 6f74 696f 6e20 6c69 6272 6172 792e 2059  otion library. Y
-000007d0: 6f75 2063 616e 2075 7365 2074 6865 2070  ou can use the p
-000007e0: 6970 2063 6f6d 6d61 6e64 2074 6f20 696e  ip command to in
-000007f0: 7374 616c 6c20 6974 3a0a 0a60 6060 0a70  stall it:..```.p
-00000800: 6970 2069 6e73 7461 6c6c 2068 746d 6c32  ip install html2
-00000810: 6e6f 7469 6f6e 0a60 6060 0a0a 2323 2050  notion.```..## P
-00000820: 7265 7061 7265 204e 6f74 696f 6e20 436f  repare Notion Co
-00000830: 6e66 6967 7572 6174 696f 6e0a 0a57 6520  nfiguration..We 
-00000840: 6e65 6564 2074 6f20 7573 6520 7468 6520  need to use the 
-00000850: 604e 6f74 696f 6e20 4150 4920 6b65 7960  `Notion API key`
-00000860: 2061 6e64 2060 4461 7461 6261 7365 2049   and `Database I
-00000870: 4460 2074 6f20 6175 7468 6f72 697a 6520  D` to authorize 
-00000880: 6874 6d6c 326e 6f74 696f 6e20 746f 2061  html2notion to a
-00000890: 6363 6573 7320 7468 6520 4e6f 7469 6f6e  ccess the Notion
-000008a0: 2064 6174 6162 6173 652e 2050 6c65 6173   database. Pleas
-000008b0: 6520 666f 6c6c 6f77 2074 6865 7365 2073  e follow these s
-000008c0: 7465 7073 3a0a 0a31 2e20 4372 6561 7465  teps:..1. Create
-000008d0: 2061 6e20 696e 7465 6772 6174 696f 6e3b   an integration;
-000008e0: 0a32 2e20 5368 6172 6520 6120 6461 7461  .2. Share a data
-000008f0: 6261 7365 2077 6974 6820 796f 7572 2069  base with your i
-00000900: 6e74 6567 7261 7469 6f6e 3b0a 332e 2045  ntegration;.3. E
-00000910: 7870 6f72 7420 7468 6520 6461 7461 6261  xport the databa
-00000920: 7365 2049 443b 0a0a 5768 656e 2073 6861  se ID;..When sha
-00000930: 7269 6e67 2074 6865 2064 6174 6162 6173  ring the databas
-00000940: 6520 6865 7265 2c20 796f 7520 6e65 6564  e here, you need
-00000950: 2074 6f20 6368 6f6f 7365 2074 6865 2070   to choose the p
-00000960: 7265 7669 6f75 736c 7920 6475 706c 6963  reviously duplic
-00000970: 6174 6564 2064 6174 6162 6173 6520 6265  ated database be
-00000980: 6361 7573 6520 7468 6520 696d 706f 7274  cause the import
-00000990: 206f 7065 7261 7469 6f6e 2072 6571 7569   operation requi
-000009a0: 7265 7320 736f 6d65 2070 7265 7365 7420  res some preset 
-000009b0: 5b70 726f 7065 7274 6965 735d 2868 7474  [properties](htt
-000009c0: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
-000009d0: 6e6f 7469 6f6e 2e63 6f6d 2f72 6566 6572  notion.com/refer
-000009e0: 656e 6365 2f70 726f 7065 7274 792d 6f62  ence/property-ob
-000009f0: 6a65 6374 2920 696e 666f 726d 6174 696f  ject) informatio
-00000a00: 6e20 696e 2074 6869 7320 6461 7461 6261  n in this databa
-00000a10: 7365 2e0a 0a46 6f72 2073 7065 6369 6669  se...For specifi
-00000a20: 6320 6d65 7468 6f64 732c 2070 6c65 6173  c methods, pleas
-00000a30: 6520 7265 6665 7220 746f 2074 6865 204e  e refer to the N
-00000a40: 6f74 696f 6e20 6f66 6669 6369 616c 2064  otion official d
-00000a50: 6f63 756d 656e 7461 7469 6f6e 205b 6372  ocumentation [cr
-00000a60: 6561 7465 2061 6e20 696e 7465 6772 6174  eate an integrat
-00000a70: 696f 6e5d 2868 7474 7073 3a2f 2f64 6576  ion](https://dev
-00000a80: 656c 6f70 6572 732e 6e6f 7469 6f6e 2e63  elopers.notion.c
-00000a90: 6f6d 2f64 6f63 732f 6372 6561 7465 2d61  om/docs/create-a
-00000aa0: 2d6e 6f74 696f 6e2d 696e 7465 6772 6174  -notion-integrat
-00000ab0: 696f 6e29 2e0a 0a41 6674 6572 2074 6865  ion)...After the
-00000ac0: 2073 6574 7570 2069 7320 636f 6d70 6c65   setup is comple
-00000ad0: 7465 2c20 7772 6974 6520 796f 7572 2041  te, write your A
-00000ae0: 5049 204b 6579 2061 6e64 2064 6174 6162  PI Key and datab
-00000af0: 6173 6520 4944 2069 6e74 6f20 6120 636f  ase ID into a co
-00000b00: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-00000b10: 2063 6f6e 6669 672e 6a73 6f6e 2e0a 0a60   config.json...`
-00000b20: 6060 7368 656c 6c0a 7b0a 2020 2020 226e  ``shell.{.    "n
-00000b30: 6f74 696f 6e22 3a20 7b0a 2020 2020 2020  otion": {.      
-00000b40: 2020 2264 6174 6162 6173 655f 6964 223a    "database_id":
-00000b50: 2022 3c2a 2a2a 6465 6d6f 2a2a 2a3e 222c   "<***demo***>",
-00000b60: 0a20 2020 2020 2020 2022 6170 695f 6b65  .        "api_ke
-00000b70: 7922 3a20 223c 2a2a 2a64 656d 6f2a 2a2a  y": "<***demo***
-00000b80: 3e22 0a20 2020 207d 0a7d 0a60 6060 0a0a  >".    }.}.```..
-00000b90: 2320 5573 6167 650a 0a59 6f75 2063 616e  # Usage..You can
-00000ba0: 2075 7365 2060 6874 6d6c 326e 6f74 696f   use `html2notio
-00000bb0: 6e20 2d68 6020 746f 2076 6965 7720 6465  n -h` to view de
-00000bc0: 7461 696c 6564 2068 656c 7020 646f 6375  tailed help docu
-00000bd0: 6d65 6e74 6174 696f 6e2e 0a0a 6060 6073  mentation...```s
-00000be0: 6865 6c6c 0a75 7361 6765 3a20 6874 6d6c  hell.usage: html
-00000bf0: 326e 6f74 696f 6e20 5b2d 685d 202d 2d63  2notion [-h] --c
-00000c00: 6f6e 6620 434f 4e46 205b 2d2d 6c6f 6720  onf CONF [--log 
-00000c10: 4c4f 475d 205b 2d2d 6261 7463 6820 4241  LOG] [--batch BA
-00000c20: 5443 485d 2028 2d2d 6669 6c65 2046 494c  TCH] (--file FIL
-00000c30: 4520 7c20 2d2d 6469 7220 4449 5229 0a0a  E | --dir DIR)..
-00000c40: 4874 6d6c 326e 6f74 696f 6e3a 2053 6176  Html2notion: Sav
-00000c50: 6520 4854 4d4c 2074 6f20 796f 7572 204e  e HTML to your N
-00000c60: 6f74 696f 6e20 6e6f 7465 7320 7175 6963  otion notes quic
-00000c70: 6b6c 7920 616e 6420 6561 7369 6c79 2c20  kly and easily, 
-00000c80: 7768 696c 6520 6b65 6570 696e 6720 7468  while keeping th
-00000c90: 6520 6f72 6967 696e 616c 2066 6f72 6d61  e original forma
-00000ca0: 7420 6173 206d 7563 6820 6173 2070 6f73  t as much as pos
-00000cb0: 7369 626c 650a 0a6f 7074 696f 6e73 3a0a  sible..options:.
-00000cc0: 2020 2d68 2c20 2d2d 6865 6c70 2020 2020    -h, --help    
-00000cd0: 2073 686f 7720 7468 6973 2068 656c 7020   show this help 
-00000ce0: 6d65 7373 6167 6520 616e 6420 6578 6974  message and exit
-00000cf0: 0a20 202d 2d63 6f6e 6620 434f 4e46 2020  .  --conf CONF  
-00000d00: 2020 636f 6e66 2066 696c 6520 7061 7468    conf file path
-00000d10: 0a20 202d 2d6c 6f67 204c 4f47 2020 2020  .  --log LOG    
-00000d20: 2020 6c6f 6720 6469 7265 6374 2070 6174    log direct pat
-00000d30: 680a 2020 2d2d 6261 7463 6820 4241 5443  h.  --batch BATC
-00000d40: 4820 2062 6174 6368 2073 6176 6520 636f  H  batch save co
-00000d50: 6e63 7572 7265 6e74 206c 696d 6974 0a20  ncurrent limit. 
-00000d60: 202d 2d66 696c 6520 4649 4c45 2020 2020   --file FILE    
-00000d70: 5361 7665 2073 696e 676c 6520 6874 6d6c  Save single html
-00000d80: 2066 696c 6520 746f 206e 6f74 696f 6e0a   file to notion.
-00000d90: 2020 2d2d 6469 7220 4449 5220 2020 2020    --dir DIR     
-00000da0: 2053 6176 6520 616c 6c20 6874 6d6c 2066   Save all html f
-00000db0: 696c 6573 2069 6e20 7468 6520 6469 7220  iles in the dir 
-00000dc0: 746f 206e 6f74 696f 6e0a 6060 600a 0a46  to notion.```..F
-00000dd0: 6f72 2065 7861 6d70 6c65 2c20 6966 2079  or example, if y
-00000de0: 6f75 2077 616e 7420 746f 2069 6d70 6f72  ou want to impor
-00000df0: 7420 616c 6c20 6874 6d6c 2066 696c 6573  t all html files
-00000e00: 2069 6e20 7468 6520 602e 2f64 656d 6f73   in the `./demos
-00000e10: 6020 6469 7265 6374 6f72 7920 696e 746f  ` directory into
-00000e20: 204e 6f74 696f 6e2c 2079 6f75 2063 616e   Notion, you can
-00000e30: 2075 7365 2074 6865 2066 6f6c 6c6f 7769   use the followi
-00000e40: 6e67 2063 6f6d 6d61 6e64 3a0a 0a60 6060  ng command:..```
-00000e50: 7368 656c 6c0a 6874 6d6c 326e 6f74 696f  shell.html2notio
-00000e60: 6e20 2d2d 636f 6e66 2063 6f6e 6669 672e  n --conf config.
-00000e70: 6a73 6f6e 202d 2d64 6972 202e 2f64 656d  json --dir ./dem
-00000e80: 6f73 202d 2d6c 6f67 207e 2f6c 6f67 7320  os --log ~/logs 
-00000e90: 2d2d 6261 7463 6820 3130 0a60 6060 0a0a  --batch 10.```..
-00000ea0: 5468 6520 6162 6f76 6520 636f 6d6d 616e  The above comman
-00000eb0: 6420 7769 6c6c 2069 6d70 6f72 7420 616c  d will import al
-00000ec0: 6c20 6874 6d6c 2066 696c 6573 2069 6e20  l html files in 
-00000ed0: 7468 6520 602e 2f64 656d 6f73 6020 6469  the `./demos` di
-00000ee0: 7265 6374 6f72 7920 696e 746f 204e 6f74  rectory into Not
-00000ef0: 696f 6e2c 2077 6869 6c65 206f 7574 7075  ion, while outpu
-00000f00: 7474 696e 6720 6c6f 6773 2074 6f20 7468  tting logs to th
-00000f10: 6520 607e 2f6c 6f67 7360 2064 6972 6563  e `~/logs` direc
-00000f20: 746f 7279 2c20 7769 7468 2075 7020 746f  tory, with up to
-00000f30: 2031 3020 636f 6e63 7572 7265 6e74 2074   10 concurrent t
-00000f40: 6173 6b73 2e0a 0a23 204d 6f72 6520 696e  asks...# More in
-00000f50: 666f 726d 6174 696f 6e0a 0a59 6f75 2063  formation..You c
-00000f60: 616e 2066 696e 6420 6d6f 7265 2069 6e66  an find more inf
-00000f70: 6f72 6d61 7469 6f6e 2061 6e64 2065 7861  ormation and exa
-00000f80: 6d70 6c65 7320 696e 2074 6865 2068 746d  mples in the htm
-00000f90: 6c32 6e6f 7469 6f6e 206c 6962 7261 7279  l2notion library
-00000fa0: 2773 2049 7373 7565 3a20 5b68 746d 6c32  's Issue: [html2
-00000fb0: 6e6f 7469 6f6e 5d28 6874 7470 733a 2f2f  notion](https://
-00000fc0: 6769 7468 7562 2e63 6f6d 2f73 656c 6662  github.com/selfb
-00000fd0: 6f6f 742f 6874 6d6c 326e 6f74 696f 6e2f  oot/html2notion/
-00000fe0: 6973 7375 6573 290a 0a23 2320 436f 6e74  issues)..## Cont
-00000ff0: 7269 6275 7469 6f6e 0a0a 4966 2079 6f75  ribution..If you
-00001000: 2066 696e 6420 616e 7920 6572 726f 7273   find any errors
-00001010: 206f 7220 6861 7665 2061 6e79 2073 7567   or have any sug
-00001020: 6765 7374 696f 6e73 2066 6f72 2069 6d70  gestions for imp
-00001030: 726f 7665 6d65 6e74 2c20 706c 6561 7365  rovement, please
-00001040: 2064 6f20 6e6f 7420 6865 7369 7461 7465   do not hesitate
-00001050: 2074 6f20 7375 626d 6974 2061 2070 756c   to submit a pul
-00001060: 6c20 7265 7175 6573 7420 6f72 2072 6169  l request or rai
-00001070: 7365 2061 6e20 6973 7375 652c 2049 2061  se an issue, I a
-00001080: 6d20 6d6f 7265 2074 6861 6e20 6861 7070  m more than happ
-00001090: 7920 746f 2061 6363 6570 7420 796f 7572  y to accept your
-000010a0: 2063 6f6e 7472 6962 7574 696f 6e73 2061   contributions a
-000010b0: 6e64 2066 6565 6462 6163 6b21 0a0a 4966  nd feedback!..If
-000010c0: 2079 6f75 2065 6e63 6f75 6e74 6572 2069   you encounter i
-000010d0: 6d70 6f72 7420 6661 696c 7572 6573 2c20  mport failures, 
-000010e0: 796f 7520 6361 6e20 7375 626d 6974 2074  you can submit t
-000010f0: 6865 2068 746d 6c20 6669 6c65 2061 6e64  he html file and
-00001100: 206c 6f67 2066 696c 6520 746f 6765 7468   log file togeth
-00001110: 6572 2069 6e20 7468 6520 6973 7375 6520  er in the issue 
-00001120: 666f 7220 6561 7369 6572 2070 726f 626c  for easier probl
-00001130: 656d 2069 6465 6e74 6966 6963 6174 696f  em identificatio
-00001140: 6e2e 0a0a 3e20 4966 2074 6865 7265 2061  n...> If there a
-00001150: 7265 2061 6e79 2070 7269 7661 7465 2069  re any private i
-00001160: 6e66 6f72 6d61 7469 6f6e 2069 6e20 7468  nformation in th
-00001170: 6520 6669 6c65 732c 2070 6c65 6173 6520  e files, please 
-00001180: 7265 6d6f 7665 2069 7420 6669 7273 742e  remove it first.
-00001190: 0a0a 0a23 2320 4c69 6365 6e73 650a 0a54  ...## License..T
-000011a0: 6869 7320 7072 6f6a 6563 7420 7573 6573  his project uses
-000011b0: 2074 6865 204d 4954 206c 6963 656e 7365   the MIT license
-000011c0: 2e20 506c 6561 7365 2072 6566 6572 2074  . Please refer t
-000011d0: 6f20 7468 6520 5b4c 4943 454e 5345 5d28  o the [LICENSE](
-000011e0: 2e2f 4c49 4345 4e53 4529 2066 6f72 2064  ./LICENSE) for d
-000011f0: 6574 6169 6c73 2e0a                      etails..
+000001e0: 4943 454e 5345 0a0a 3c68 3120 616c 6967  ICENSE..<h1 alig
+000001f0: 6e3d 2263 656e 7465 7222 3e48 746d 6c32  n="center">Html2
+00000200: 6e6f 7469 6f6e 203c 6120 6872 6566 3d27  notion <a href='
+00000210: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000220: 6f6d 2f73 656c 6662 6f6f 742f 6874 6d6c  om/selfboot/html
+00000230: 326e 6f74 696f 6e2f 626c 6f62 2f6d 6173  2notion/blob/mas
+00000240: 7465 722f 5245 4144 4d45 5f7a 682e 6d64  ter/README_zh.md
+00000250: 273e e7ae 80e4 bd93 e4b8 ade6 9687 3c2f  '>............</
+00000260: 613e 3c2f 6831 3e0a 3c70 2061 6c69 676e  a></h1>.<p align
+00000270: 3d22 6365 6e74 6572 223e 0a20 203c 6120  ="center">.  <a 
+00000280: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000290: 7468 7562 2e63 6f6d 2f73 656c 6662 6f6f  thub.com/selfboo
+000002a0: 742f 6874 6d6c 326e 6f74 696f 6e2f 6163  t/html2notion/ac
+000002b0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+000002c0: 7079 7468 6f6e 2d70 6163 6b61 6765 2e79  python-package.y
+000002d0: 6d6c 223e 0a20 2020 203c 696d 6720 7372  ml">.    <img sr
+000002e0: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+000002f0: 622e 636f 6d2f 7365 6c66 626f 6f74 2f68  b.com/selfboot/h
+00000300: 746d 6c32 6e6f 7469 6f6e 2f61 6374 696f  tml2notion/actio
+00000310: 6e73 2f77 6f72 6b66 6c6f 7773 2f70 7974  ns/workflows/pyt
+00000320: 686f 6e2d 7061 636b 6167 652e 796d 6c2f  hon-package.yml/
+00000330: 6261 6467 652e 7376 6722 2061 6c74 3d22  badge.svg" alt="
+00000340: 4349 2054 6573 7420 5374 6174 7573 223e  CI Test Status">
+00000350: 0a20 203c 2f61 3e0a 203c 6120 6872 6566  .  </a>. <a href
+00000360: 3d22 6874 7470 733a 2f2f 636f 6465 636f  ="https://codeco
+00000370: 762e 696f 2f67 682f 7365 6c66 626f 6f74  v.io/gh/selfboot
+00000380: 2f68 746d 6c32 6e6f 7469 6f6e 2220 3e0a  /html2notion" >.
+00000390: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+000003a0: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+000003b0: 2f73 656c 6662 6f6f 742f 6874 6d6c 326e  /selfboot/html2n
+000003c0: 6f74 696f 6e2f 6272 616e 6368 2f6d 6173  otion/branch/mas
+000003d0: 7465 722f 6772 6170 682f 6261 6467 652e  ter/graph/badge.
+000003e0: 7376 673f 746f 6b65 6e3d 5349 4d36 4937  svg?token=SIM6I7
+000003f0: 425a 5536 2220 616c 743d 2254 6573 7420  BZU6" alt="Test 
+00000400: 636f 7665 7261 6765 222f 3e0a 203c 2f61  coverage"/>. </a
+00000410: 3e0a 3c2f 703e 0a0a 6874 6d6c 326e 6f74  >.</p>..html2not
+00000420: 696f 6e20 6973 2061 6e20 696e 6372 6564  ion is an incred
+00000430: 6962 6c79 2075 7365 6675 6c20 746f 6f6c  ibly useful tool
+00000440: 2077 7269 7474 656e 2069 6e20 5079 7468   written in Pyth
+00000450: 6f6e 2c20 7768 6963 6820 616c 6c6f 7773  on, which allows
+00000460: 2079 6f75 2074 6f20 696d 706f 7274 2063   you to import c
+00000470: 6f6e 7465 6e74 2066 726f 6d20 4854 4d4c  ontent from HTML
+00000480: 2064 6f63 756d 656e 7473 2069 6e74 6f20   documents into 
+00000490: 4e6f 7469 6f6e 206e 6f74 6573 2c20 6d61  Notion notes, ma
+000004a0: 6b69 6e67 2069 7420 6d6f 7265 2063 6f6e  king it more con
+000004b0: 7665 6e69 656e 7420 666f 7220 796f 7520  venient for you 
+000004c0: 746f 206f 7267 616e 697a 6520 696e 666f  to organize info
+000004d0: 726d 6174 696f 6e20 6f6e 2074 6865 204e  rmation on the N
+000004e0: 6f74 696f 6e20 706c 6174 666f 726d 2e20  otion platform. 
+000004f0: 496e 2061 6464 6974 696f 6e2c 2068 746d  In addition, htm
+00000500: 6c32 6e6f 7469 6f6e 2068 6173 2062 6565  l2notion has bee
+00000510: 6e20 7370 6563 6966 6963 616c 6c79 206f  n specifically o
+00000520: 7074 696d 697a 6564 2066 6f72 2074 6865  ptimized for the
+00000530: 2063 6f6e 7465 6e74 206f 6620 4576 6572   content of Ever
+00000540: 6e6f 7465 2c20 616e 6420 796f 7520 6361  note, and you ca
+00000550: 6e20 616c 736f 2075 7365 2069 7420 746f  n also use it to
+00000560: 2069 6d70 6f72 7420 6e6f 7465 7320 6672   import notes fr
+00000570: 6f6d 2045 7665 726e 6f74 6520 696e 746f  om Evernote into
+00000580: 204e 6f74 696f 6e2e 0a0a 6874 6d6c 326e   Notion...html2n
+00000590: 6f74 696f 6e20 6861 7320 706f 7765 7266  otion has powerf
+000005a0: 756c 2066 6561 7475 7265 7320 616e 6420  ul features and 
+000005b0: 7375 7070 6f72 7473 2063 6f6e 7665 7274  supports convert
+000005c0: 696e 6720 7661 7269 6f75 7320 7461 6773  ing various tags
+000005d0: 2069 6e20 4854 4d4c 2066 696c 6573 2069   in HTML files i
+000005e0: 6e74 6f20 636f 7272 6573 706f 6e64 696e  nto correspondin
+000005f0: 6720 426c 6f63 6b73 2069 6e20 4e6f 7469  g Blocks in Noti
+00000600: 6f6e 2c20 7375 6368 2061 7320 7269 6368  on, such as rich
+00000610: 2074 6578 7420 626c 6f63 6b73 2c20 6865   text blocks, he
+00000620: 6164 696e 6773 2c20 696d 6167 6573 2c20  adings, images, 
+00000630: 636f 6465 2062 6c6f 636b 732c 2071 756f  code blocks, quo
+00000640: 7465 732c 206c 696e 6b73 2c20 6574 632e  tes, links, etc.
+00000650: 2042 656c 6f77 2061 7265 2065 7861 6d70   Below are examp
+00000660: 6c65 7320 6f66 2063 6f6e 7665 7274 696e  les of convertin
+00000670: 6720 6e6f 7465 7320 6672 6f6d 2045 7665  g notes from Eve
+00000680: 726e 6f74 6520 696e 746f 204e 6f74 696f  rnote into Notio
+00000690: 6e20 7061 6765 732e 0a0a 215b 7969 6e78  n pages...![yinx
+000006a0: 6961 6e67 206e 6f74 696f 6e28 7369 6d70  iang notion(simp
+000006b0: 6c65 2064 656d 6f73 295d 2868 7474 7073  le demos)](https
+000006c0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+000006d0: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 656c  rcontent.com/sel
+000006e0: 6662 6f6f 742f 6874 6d6c 326e 6f74 696f  fboot/html2notio
+000006f0: 6e2f 6d61 7374 6572 2f64 656d 6f73 2f79  n/master/demos/y
+00000700: 696e 7869 616e 675f 6e6f 7469 6f6e 2e70  inxiang_notion.p
+00000710: 6e67 290a 0a21 5b79 696e 7869 616e 6720  ng)..![yinxiang 
+00000720: 6e6f 7469 6f6e 3228 7269 6368 2074 6578  notion2(rich tex
+00000730: 7429 5d28 6874 7470 733a 2f2f 7261 772e  t)](https://raw.
+00000740: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000750: 742e 636f 6d2f 7365 6c66 626f 6f74 2f68  t.com/selfboot/h
+00000760: 746d 6c32 6e6f 7469 6f6e 2f6d 6173 7465  tml2notion/maste
+00000770: 722f 6465 6d6f 732f 7969 6e78 6961 6e67  r/demos/yinxiang
+00000780: 5f6e 6f74 696f 6e32 2e70 6e67 290a 0a23  _notion2.png)..#
+00000790: 2050 7265 7061 7265 0a0a 596f 7520 6f6e   Prepare..You on
+000007a0: 6c79 206e 6565 6420 3320 7374 6570 7320  ly need 3 steps 
+000007b0: 746f 2075 7365 2068 746d 6c6e 6f74 696f  to use htmlnotio
+000007c0: 6e20 746f 2069 6d70 6f72 7420 4854 4d4c  n to import HTML
+000007d0: 2069 6e74 6f20 4e6f 7469 6f6e 2e0a 0a23   into Notion...#
+000007e0: 2320 4475 706c 6963 6174 6520 6461 7461  # Duplicate data
+000007f0: 6261 7365 0a0a 436c 6963 6b20 7468 6520  base..Click the 
+00000800: 6c69 6e6b 205b 6e6f 7469 6f6e 2074 656d  link [notion tem
+00000810: 706c 6174 655d 2868 7474 7073 3a2f 2f73  plate](https://s
+00000820: 656c 6662 6f6f 742e 6e6f 7469 6f6e 2e73  elfboot.notion.s
+00000830: 6974 652f 7365 6c66 626f 6f74 2f31 3330  ite/selfboot/130
+00000840: 6262 3438 6336 6362 6434 6162 6262 6237  bb48c6cbd4abbbb7
+00000850: 3133 6434 6438 3437 3234 3831 613f 763d  13d4d8472481a?v=
+00000860: 6464 6461 3230 6433 6634 3662 3462 3434  ddda20d3f46b4b44
+00000870: 6130 3535 6430 3637 3932 6331 3432 6630  a055d06792c142f0
+00000880: 292e 2041 7320 7368 6f77 6e20 696e 2074  ). As shown in t
+00000890: 6865 2069 6d61 6765 2062 656c 6f77 2c20  he image below, 
+000008a0: 7573 6520 7468 6520 2244 7570 6c69 6361  use the "Duplica
+000008b0: 7465 2220 6275 7474 6f6e 2074 6f20 636f  te" button to co
+000008c0: 7079 2061 206e 6577 2064 6174 6162 6173  py a new databas
+000008d0: 6520 746f 2079 6f75 7220 6f77 6e20 4e6f  e to your own No
+000008e0: 7469 6f6e 2077 6f72 6b73 7061 6365 2e0a  tion workspace..
+000008f0: 0a21 5b6e 6f74 696f 6e20 7465 6d70 6c61  .![notion templa
+00000900: 7465 5d28 6874 7470 733a 2f2f 7261 772e  te](https://raw.
+00000910: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000920: 742e 636f 6d2f 7365 6c66 626f 6f74 2f68  t.com/selfboot/h
+00000930: 746d 6c32 6e6f 7469 6f6e 2f6d 6173 7465  tml2notion/maste
+00000940: 722f 6465 6d6f 732f 6e6f 7469 6f6e 5f74  r/demos/notion_t
+00000950: 656d 706c 6167 652e 706e 6729 0a0a 2323  emplage.png)..##
+00000960: 2049 6e73 7461 6c6c 2068 746d 6c32 6e6f   Install html2no
+00000970: 7469 6f6e 0a0a 5265 7175 6972 6573 2070  tion..Requires p
+00000980: 7974 686f 6e3e 3d33 2e38 2c20 696e 7374  ython>=3.8, inst
+00000990: 616c 6c20 7468 6520 6874 6d6c 326e 6f74  all the html2not
+000009a0: 696f 6e20 6c69 6272 6172 792e 2059 6f75  ion library. You
+000009b0: 2063 616e 2075 7365 2074 6865 2070 6970   can use the pip
+000009c0: 2063 6f6d 6d61 6e64 2074 6f20 696e 7374   command to inst
+000009d0: 616c 6c20 6974 3a0a 0a60 6060 0a70 6970  all it:..```.pip
+000009e0: 2069 6e73 7461 6c6c 2068 746d 6c32 6e6f   install html2no
+000009f0: 7469 6f6e 0a60 6060 0a0a 2323 2050 7265  tion.```..## Pre
+00000a00: 7061 7265 204e 6f74 696f 6e20 436f 6e66  pare Notion Conf
+00000a10: 6967 7572 6174 696f 6e0a 0a57 6520 6e65  iguration..We ne
+00000a20: 6564 2074 6f20 7573 6520 7468 6520 604e  ed to use the `N
+00000a30: 6f74 696f 6e20 4150 4920 6b65 7960 2061  otion API key` a
+00000a40: 6e64 2060 4461 7461 6261 7365 2049 4460  nd `Database ID`
+00000a50: 2074 6f20 6175 7468 6f72 697a 6520 6874   to authorize ht
+00000a60: 6d6c 326e 6f74 696f 6e20 746f 2061 6363  ml2notion to acc
+00000a70: 6573 7320 7468 6520 4e6f 7469 6f6e 2064  ess the Notion d
+00000a80: 6174 6162 6173 652e 2050 6c65 6173 6520  atabase. Please 
+00000a90: 666f 6c6c 6f77 2074 6865 7365 2073 7465  follow these ste
+00000aa0: 7073 3a0a 0a31 2e20 4372 6561 7465 2061  ps:..1. Create a
+00000ab0: 6e20 696e 7465 6772 6174 696f 6e3b 0a32  n integration;.2
+00000ac0: 2e20 5368 6172 6520 6120 6461 7461 6261  . Share a databa
+00000ad0: 7365 2077 6974 6820 796f 7572 2069 6e74  se with your int
+00000ae0: 6567 7261 7469 6f6e 3b0a 332e 2045 7870  egration;.3. Exp
+00000af0: 6f72 7420 7468 6520 6461 7461 6261 7365  ort the database
+00000b00: 2049 443b 0a0a 5768 656e 2073 6861 7269   ID;..When shari
+00000b10: 6e67 2074 6865 2064 6174 6162 6173 6520  ng the database 
+00000b20: 6865 7265 2c20 796f 7520 6e65 6564 2074  here, you need t
+00000b30: 6f20 6368 6f6f 7365 2074 6865 2070 7265  o choose the pre
+00000b40: 7669 6f75 736c 7920 6475 706c 6963 6174  viously duplicat
+00000b50: 6564 2064 6174 6162 6173 6520 6265 6361  ed database beca
+00000b60: 7573 6520 7468 6520 696d 706f 7274 206f  use the import o
+00000b70: 7065 7261 7469 6f6e 2072 6571 7569 7265  peration require
+00000b80: 7320 736f 6d65 2070 7265 7365 7420 5b70  s some preset [p
+00000b90: 726f 7065 7274 6965 735d 2868 7474 7073  roperties](https
+00000ba0: 3a2f 2f64 6576 656c 6f70 6572 732e 6e6f  ://developers.no
+00000bb0: 7469 6f6e 2e63 6f6d 2f72 6566 6572 656e  tion.com/referen
+00000bc0: 6365 2f70 726f 7065 7274 792d 6f62 6a65  ce/property-obje
+00000bd0: 6374 2920 696e 666f 726d 6174 696f 6e20  ct) information 
+00000be0: 696e 2074 6869 7320 6461 7461 6261 7365  in this database
+00000bf0: 2e0a 0a46 6f72 2073 7065 6369 6669 6320  ...For specific 
+00000c00: 6d65 7468 6f64 732c 2070 6c65 6173 6520  methods, please 
+00000c10: 7265 6665 7220 746f 2074 6865 204e 6f74  refer to the Not
+00000c20: 696f 6e20 6f66 6669 6369 616c 2064 6f63  ion official doc
+00000c30: 756d 656e 7461 7469 6f6e 205b 6372 6561  umentation [crea
+00000c40: 7465 2061 6e20 696e 7465 6772 6174 696f  te an integratio
+00000c50: 6e5d 2868 7474 7073 3a2f 2f64 6576 656c  n](https://devel
+00000c60: 6f70 6572 732e 6e6f 7469 6f6e 2e63 6f6d  opers.notion.com
+00000c70: 2f64 6f63 732f 6372 6561 7465 2d61 2d6e  /docs/create-a-n
+00000c80: 6f74 696f 6e2d 696e 7465 6772 6174 696f  otion-integratio
+00000c90: 6e29 2e0a 0a41 6674 6572 2074 6865 2073  n)...After the s
+00000ca0: 6574 7570 2069 7320 636f 6d70 6c65 7465  etup is complete
+00000cb0: 2c20 7772 6974 6520 796f 7572 2041 5049  , write your API
+00000cc0: 204b 6579 2061 6e64 2064 6174 6162 6173   Key and databas
+00000cd0: 6520 4944 2069 6e74 6f20 6120 636f 6e66  e ID into a conf
+00000ce0: 6967 7572 6174 696f 6e20 6669 6c65 2063  iguration file c
+00000cf0: 6f6e 6669 672e 6a73 6f6e 2e0a 0a60 6060  onfig.json...```
+00000d00: 7368 656c 6c0a 7b0a 2020 2020 226e 6f74  shell.{.    "not
+00000d10: 696f 6e22 3a20 7b0a 2020 2020 2020 2020  ion": {.        
+00000d20: 2264 6174 6162 6173 655f 6964 223a 2022  "database_id": "
+00000d30: 3c2a 2a2a 6465 6d6f 2a2a 2a3e 222c 0a20  <***demo***>",. 
+00000d40: 2020 2020 2020 2022 6170 695f 6b65 7922         "api_key"
+00000d50: 3a20 223c 2a2a 2a64 656d 6f2a 2a2a 3e22  : "<***demo***>"
+00000d60: 0a20 2020 207d 0a7d 0a60 6060 0a0a 2320  .    }.}.```..# 
+00000d70: 5573 6167 650a 0a59 6f75 2063 616e 2075  Usage..You can u
+00000d80: 7365 2060 6874 6d6c 326e 6f74 696f 6e20  se `html2notion 
+00000d90: 2d68 6020 746f 2076 6965 7720 6465 7461  -h` to view deta
+00000da0: 696c 6564 2068 656c 7020 646f 6375 6d65  iled help docume
+00000db0: 6e74 6174 696f 6e2e 0a0a 6060 6073 6865  ntation...```she
+00000dc0: 6c6c 0a75 7361 6765 3a20 6874 6d6c 326e  ll.usage: html2n
+00000dd0: 6f74 696f 6e20 5b2d 685d 202d 2d63 6f6e  otion [-h] --con
+00000de0: 6620 434f 4e46 205b 2d2d 6c6f 6720 4c4f  f CONF [--log LO
+00000df0: 475d 205b 2d2d 6261 7463 6820 4241 5443  G] [--batch BATC
+00000e00: 485d 2028 2d2d 6669 6c65 2046 494c 4520  H] (--file FILE 
+00000e10: 7c20 2d2d 6469 7220 4449 5229 0a0a 4874  | --dir DIR)..Ht
+00000e20: 6d6c 326e 6f74 696f 6e3a 2053 6176 6520  ml2notion: Save 
+00000e30: 4854 4d4c 2074 6f20 796f 7572 204e 6f74  HTML to your Not
+00000e40: 696f 6e20 6e6f 7465 7320 7175 6963 6b6c  ion notes quickl
+00000e50: 7920 616e 6420 6561 7369 6c79 2c20 7768  y and easily, wh
+00000e60: 696c 6520 6b65 6570 696e 6720 7468 6520  ile keeping the 
+00000e70: 6f72 6967 696e 616c 2066 6f72 6d61 7420  original format 
+00000e80: 6173 206d 7563 6820 6173 2070 6f73 7369  as much as possi
+00000e90: 626c 650a 0a6f 7074 696f 6e73 3a0a 2020  ble..options:.  
+00000ea0: 2d68 2c20 2d2d 6865 6c70 2020 2020 2073  -h, --help     s
+00000eb0: 686f 7720 7468 6973 2068 656c 7020 6d65  how this help me
+00000ec0: 7373 6167 6520 616e 6420 6578 6974 0a20  ssage and exit. 
+00000ed0: 202d 2d63 6f6e 6620 434f 4e46 2020 2020   --conf CONF    
+00000ee0: 636f 6e66 2066 696c 6520 7061 7468 0a20  conf file path. 
+00000ef0: 202d 2d6c 6f67 204c 4f47 2020 2020 2020   --log LOG      
+00000f00: 6c6f 6720 6469 7265 6374 2070 6174 680a  log direct path.
+00000f10: 2020 2d2d 6261 7463 6820 4241 5443 4820    --batch BATCH 
+00000f20: 2062 6174 6368 2073 6176 6520 636f 6e63   batch save conc
+00000f30: 7572 7265 6e74 206c 696d 6974 0a20 202d  urrent limit.  -
+00000f40: 2d66 696c 6520 4649 4c45 2020 2020 5361  -file FILE    Sa
+00000f50: 7665 2073 696e 676c 6520 6874 6d6c 2066  ve single html f
+00000f60: 696c 6520 746f 206e 6f74 696f 6e0a 2020  ile to notion.  
+00000f70: 2d2d 6469 7220 4449 5220 2020 2020 2053  --dir DIR      S
+00000f80: 6176 6520 616c 6c20 6874 6d6c 2066 696c  ave all html fil
+00000f90: 6573 2069 6e20 7468 6520 6469 7220 746f  es in the dir to
+00000fa0: 206e 6f74 696f 6e0a 6060 600a 0a46 6f72   notion.```..For
+00000fb0: 2065 7861 6d70 6c65 2c20 6966 2079 6f75   example, if you
+00000fc0: 2077 616e 7420 746f 2069 6d70 6f72 7420   want to import 
+00000fd0: 616c 6c20 6874 6d6c 2066 696c 6573 2069  all html files i
+00000fe0: 6e20 7468 6520 602e 2f64 656d 6f73 6020  n the `./demos` 
+00000ff0: 6469 7265 6374 6f72 7920 696e 746f 204e  directory into N
+00001000: 6f74 696f 6e2c 2079 6f75 2063 616e 2075  otion, you can u
+00001010: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
+00001020: 2063 6f6d 6d61 6e64 3a0a 0a60 6060 7368   command:..```sh
+00001030: 656c 6c0a 6874 6d6c 326e 6f74 696f 6e20  ell.html2notion 
+00001040: 2d2d 636f 6e66 2063 6f6e 6669 672e 6a73  --conf config.js
+00001050: 6f6e 202d 2d64 6972 202e 2f64 656d 6f73  on --dir ./demos
+00001060: 202d 2d6c 6f67 207e 2f6c 6f67 7320 2d2d   --log ~/logs --
+00001070: 6261 7463 6820 3130 0a60 6060 0a0a 5468  batch 10.```..Th
+00001080: 6520 6162 6f76 6520 636f 6d6d 616e 6420  e above command 
+00001090: 7769 6c6c 2069 6d70 6f72 7420 616c 6c20  will import all 
+000010a0: 6874 6d6c 2066 696c 6573 2069 6e20 7468  html files in th
+000010b0: 6520 602e 2f64 656d 6f73 6020 6469 7265  e `./demos` dire
+000010c0: 6374 6f72 7920 696e 746f 204e 6f74 696f  ctory into Notio
+000010d0: 6e2c 2077 6869 6c65 206f 7574 7075 7474  n, while outputt
+000010e0: 696e 6720 6c6f 6773 2074 6f20 7468 6520  ing logs to the 
+000010f0: 607e 2f6c 6f67 7360 2064 6972 6563 746f  `~/logs` directo
+00001100: 7279 2c20 7769 7468 2075 7020 746f 2031  ry, with up to 1
+00001110: 3020 636f 6e63 7572 7265 6e74 2074 6173  0 concurrent tas
+00001120: 6b73 2e0a 0a23 204d 6f72 6520 696e 666f  ks...# More info
+00001130: 726d 6174 696f 6e0a 0a59 6f75 2063 616e  rmation..You can
+00001140: 2066 696e 6420 6d6f 7265 2069 6e66 6f72   find more infor
+00001150: 6d61 7469 6f6e 2061 6e64 2065 7861 6d70  mation and examp
+00001160: 6c65 7320 696e 2074 6865 2068 746d 6c32  les in the html2
+00001170: 6e6f 7469 6f6e 206c 6962 7261 7279 2773  notion library's
+00001180: 2049 7373 7565 3a20 5b68 746d 6c32 6e6f   Issue: [html2no
+00001190: 7469 6f6e 5d28 6874 7470 733a 2f2f 6769  tion](https://gi
+000011a0: 7468 7562 2e63 6f6d 2f73 656c 6662 6f6f  thub.com/selfboo
+000011b0: 742f 6874 6d6c 326e 6f74 696f 6e2f 6973  t/html2notion/is
+000011c0: 7375 6573 290a 0a23 2320 436f 6e74 7269  sues)..## Contri
+000011d0: 6275 7469 6f6e 0a0a 4966 2079 6f75 2066  bution..If you f
+000011e0: 696e 6420 616e 7920 6572 726f 7273 206f  ind any errors o
+000011f0: 7220 6861 7665 2061 6e79 2073 7567 6765  r have any sugge
+00001200: 7374 696f 6e73 2066 6f72 2069 6d70 726f  stions for impro
+00001210: 7665 6d65 6e74 2c20 706c 6561 7365 2064  vement, please d
+00001220: 6f20 6e6f 7420 6865 7369 7461 7465 2074  o not hesitate t
+00001230: 6f20 7375 626d 6974 2061 2070 756c 6c20  o submit a pull 
+00001240: 7265 7175 6573 7420 6f72 2072 6169 7365  request or raise
+00001250: 2061 6e20 6973 7375 652c 2049 2061 6d20   an issue, I am 
+00001260: 6d6f 7265 2074 6861 6e20 6861 7070 7920  more than happy 
+00001270: 746f 2061 6363 6570 7420 796f 7572 2063  to accept your c
+00001280: 6f6e 7472 6962 7574 696f 6e73 2061 6e64  ontributions and
+00001290: 2066 6565 6462 6163 6b21 0a0a 4966 2079   feedback!..If y
+000012a0: 6f75 2065 6e63 6f75 6e74 6572 2069 6d70  ou encounter imp
+000012b0: 6f72 7420 6661 696c 7572 6573 2c20 796f  ort failures, yo
+000012c0: 7520 6361 6e20 7375 626d 6974 2074 6865  u can submit the
+000012d0: 2068 746d 6c20 6669 6c65 2061 6e64 206c   html file and l
+000012e0: 6f67 2066 696c 6520 746f 6765 7468 6572  og file together
+000012f0: 2069 6e20 7468 6520 6973 7375 6520 666f   in the issue fo
+00001300: 7220 6561 7369 6572 2070 726f 626c 656d  r easier problem
+00001310: 2069 6465 6e74 6966 6963 6174 696f 6e2e   identification.
+00001320: 0a0a 3e20 4966 2074 6865 7265 2061 7265  ..> If there are
+00001330: 2061 6e79 2070 7269 7661 7465 2069 6e66   any private inf
+00001340: 6f72 6d61 7469 6f6e 2069 6e20 7468 6520  ormation in the 
+00001350: 6669 6c65 732c 2070 6c65 6173 6520 7265  files, please re
+00001360: 6d6f 7665 2069 7420 6669 7273 742e 0a0a  move it first...
+00001370: 0a23 2320 4c69 6365 6e73 650a 0a54 6869  .## License..Thi
+00001380: 7320 7072 6f6a 6563 7420 7573 6573 2074  s project uses t
+00001390: 6865 204d 4954 206c 6963 656e 7365 2e20  he MIT license. 
+000013a0: 506c 6561 7365 2072 6566 6572 2074 6f20  Please refer to 
+000013b0: 7468 6520 5b4c 4943 454e 5345 5d28 2e2f  the [LICENSE](./
+000013c0: 4c49 4345 4e53 4529 2066 6f72 2064 6574  LICENSE) for det
+000013d0: 6169 6c73 2e0a                           ails..
```

### Comparing `html2notion-0.1.9/README.md` & `html2notion-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,257 +1,287 @@
-00000000: 5be7 ae80 e4bd 93e4 b8ad e696 875d 2868  [............](h
-00000010: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000020: 6d2f 7365 6c66 626f 6f74 2f68 746d 6c32  m/selfboot/html2
-00000030: 6e6f 7469 6f6e 2f62 6c6f 622f 6d61 7374  notion/blob/mast
-00000040: 6572 2f52 4541 444d 455f 7a68 2e6d 6429  er/README_zh.md)
-00000050: 0a0a 6874 6d6c 326e 6f74 696f 6e20 6973  ..html2notion is
-00000060: 2061 6e20 696e 6372 6564 6962 6c79 2075   an incredibly u
-00000070: 7365 6675 6c20 746f 6f6c 2077 7269 7474  seful tool writt
-00000080: 656e 2069 6e20 5079 7468 6f6e 2c20 7768  en in Python, wh
-00000090: 6963 6820 616c 6c6f 7773 2079 6f75 2074  ich allows you t
-000000a0: 6f20 696d 706f 7274 2063 6f6e 7465 6e74  o import content
-000000b0: 2066 726f 6d20 4854 4d4c 2064 6f63 756d   from HTML docum
-000000c0: 656e 7473 2069 6e74 6f20 4e6f 7469 6f6e  ents into Notion
-000000d0: 206e 6f74 6573 2c20 6d61 6b69 6e67 2069   notes, making i
-000000e0: 7420 6d6f 7265 2063 6f6e 7665 6e69 656e  t more convenien
-000000f0: 7420 666f 7220 796f 7520 746f 206f 7267  t for you to org
-00000100: 616e 697a 6520 696e 666f 726d 6174 696f  anize informatio
-00000110: 6e20 6f6e 2074 6865 204e 6f74 696f 6e20  n on the Notion 
-00000120: 706c 6174 666f 726d 2e20 496e 2061 6464  platform. In add
-00000130: 6974 696f 6e2c 2068 746d 6c32 6e6f 7469  ition, html2noti
-00000140: 6f6e 2068 6173 2062 6565 6e20 7370 6563  on has been spec
-00000150: 6966 6963 616c 6c79 206f 7074 696d 697a  ifically optimiz
-00000160: 6564 2066 6f72 2074 6865 2063 6f6e 7465  ed for the conte
-00000170: 6e74 206f 6620 4576 6572 6e6f 7465 2c20  nt of Evernote, 
-00000180: 616e 6420 796f 7520 6361 6e20 616c 736f  and you can also
-00000190: 2075 7365 2069 7420 746f 2069 6d70 6f72   use it to impor
-000001a0: 7420 6e6f 7465 7320 6672 6f6d 2045 7665  t notes from Eve
-000001b0: 726e 6f74 6520 696e 746f 204e 6f74 696f  rnote into Notio
-000001c0: 6e2e 0a0a 6874 6d6c 326e 6f74 696f 6e20  n...html2notion 
-000001d0: 6861 7320 706f 7765 7266 756c 2066 6561  has powerful fea
-000001e0: 7475 7265 7320 616e 6420 7375 7070 6f72  tures and suppor
-000001f0: 7473 2063 6f6e 7665 7274 696e 6720 7661  ts converting va
-00000200: 7269 6f75 7320 7461 6773 2069 6e20 4854  rious tags in HT
-00000210: 4d4c 2066 696c 6573 2069 6e74 6f20 636f  ML files into co
-00000220: 7272 6573 706f 6e64 696e 6720 426c 6f63  rresponding Bloc
-00000230: 6b73 2069 6e20 4e6f 7469 6f6e 2c20 7375  ks in Notion, su
-00000240: 6368 2061 7320 7269 6368 2074 6578 7420  ch as rich text 
-00000250: 626c 6f63 6b73 2c20 6865 6164 696e 6773  blocks, headings
-00000260: 2c20 696d 6167 6573 2c20 636f 6465 2062  , images, code b
-00000270: 6c6f 636b 732c 2071 756f 7465 732c 206c  locks, quotes, l
-00000280: 696e 6b73 2c20 6574 632e 2042 656c 6f77  inks, etc. Below
-00000290: 2061 7265 2065 7861 6d70 6c65 7320 6f66   are examples of
-000002a0: 2063 6f6e 7665 7274 696e 6720 6e6f 7465   converting note
-000002b0: 7320 6672 6f6d 2045 7665 726e 6f74 6520  s from Evernote 
-000002c0: 696e 746f 204e 6f74 696f 6e20 7061 6765  into Notion page
-000002d0: 732e 0a0a 215b 7969 6e78 6961 6e67 206e  s...![yinxiang n
-000002e0: 6f74 696f 6e28 7369 6d70 6c65 2064 656d  otion(simple dem
-000002f0: 6f73 295d 2868 7474 7073 3a2f 2f72 6177  os)](https://raw
-00000300: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000310: 6e74 2e63 6f6d 2f73 656c 6662 6f6f 742f  nt.com/selfboot/
-00000320: 6874 6d6c 326e 6f74 696f 6e2f 6d61 7374  html2notion/mast
-00000330: 6572 2f64 656d 6f73 2f79 696e 7869 616e  er/demos/yinxian
-00000340: 675f 6e6f 7469 6f6e 2e70 6e67 290a 0a21  g_notion.png)..!
-00000350: 5b79 696e 7869 616e 6720 6e6f 7469 6f6e  [yinxiang notion
-00000360: 3228 7269 6368 2074 6578 7429 5d28 6874  2(rich text)](ht
-00000370: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00000380: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000390: 7365 6c66 626f 6f74 2f68 746d 6c32 6e6f  selfboot/html2no
-000003a0: 7469 6f6e 2f6d 6173 7465 722f 6465 6d6f  tion/master/demo
-000003b0: 732f 7969 6e78 6961 6e67 5f6e 6f74 696f  s/yinxiang_notio
-000003c0: 6e32 2e70 6e67 290a 0a23 2050 7265 7061  n2.png)..# Prepa
-000003d0: 7265 0a0a 596f 7520 6f6e 6c79 206e 6565  re..You only nee
-000003e0: 6420 3320 7374 6570 7320 746f 2075 7365  d 3 steps to use
-000003f0: 2068 746d 6c6e 6f74 696f 6e20 746f 2069   htmlnotion to i
-00000400: 6d70 6f72 7420 4854 4d4c 2069 6e74 6f20  mport HTML into 
-00000410: 4e6f 7469 6f6e 2e0a 0a23 2320 4475 706c  Notion...## Dupl
-00000420: 6963 6174 6520 6461 7461 6261 7365 0a0a  icate database..
-00000430: 436c 6963 6b20 7468 6520 6c69 6e6b 205b  Click the link [
-00000440: 6e6f 7469 6f6e 2074 656d 706c 6174 655d  notion template]
-00000450: 2868 7474 7073 3a2f 2f73 656c 6662 6f6f  (https://selfboo
-00000460: 742e 6e6f 7469 6f6e 2e73 6974 652f 7365  t.notion.site/se
-00000470: 6c66 626f 6f74 2f31 3330 6262 3438 6336  lfboot/130bb48c6
-00000480: 6362 6434 6162 6262 6237 3133 6434 6438  cbd4abbbb713d4d8
-00000490: 3437 3234 3831 613f 763d 6464 6461 3230  472481a?v=ddda20
-000004a0: 6433 6634 3662 3462 3434 6130 3535 6430  d3f46b4b44a055d0
-000004b0: 3637 3932 6331 3432 6630 292e 2041 7320  6792c142f0). As 
-000004c0: 7368 6f77 6e20 696e 2074 6865 2069 6d61  shown in the ima
-000004d0: 6765 2062 656c 6f77 2c20 7573 6520 7468  ge below, use th
-000004e0: 6520 2244 7570 6c69 6361 7465 2220 6275  e "Duplicate" bu
-000004f0: 7474 6f6e 2074 6f20 636f 7079 2061 206e  tton to copy a n
-00000500: 6577 2064 6174 6162 6173 6520 746f 2079  ew database to y
-00000510: 6f75 7220 6f77 6e20 4e6f 7469 6f6e 2077  our own Notion w
-00000520: 6f72 6b73 7061 6365 2e0a 0a21 5b6e 6f74  orkspace...![not
-00000530: 696f 6e20 7465 6d70 6c61 7465 5d28 6874  ion template](ht
-00000540: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00000550: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000560: 7365 6c66 626f 6f74 2f68 746d 6c32 6e6f  selfboot/html2no
-00000570: 7469 6f6e 2f6d 6173 7465 722f 6465 6d6f  tion/master/demo
-00000580: 732f 6e6f 7469 6f6e 5f74 656d 706c 6167  s/notion_templag
-00000590: 652e 706e 6729 0a0a 2323 2049 6e73 7461  e.png)..## Insta
-000005a0: 6c6c 2068 746d 6c32 6e6f 7469 6f6e 0a0a  ll html2notion..
-000005b0: 5265 7175 6972 6573 2070 7974 686f 6e3e  Requires python>
-000005c0: 3d33 2e38 2c20 696e 7374 616c 6c20 7468  =3.8, install th
-000005d0: 6520 6874 6d6c 326e 6f74 696f 6e20 6c69  e html2notion li
-000005e0: 6272 6172 792e 2059 6f75 2063 616e 2075  brary. You can u
-000005f0: 7365 2074 6865 2070 6970 2063 6f6d 6d61  se the pip comma
-00000600: 6e64 2074 6f20 696e 7374 616c 6c20 6974  nd to install it
-00000610: 3a0a 0a60 6060 0a70 6970 2069 6e73 7461  :..```.pip insta
-00000620: 6c6c 2068 746d 6c32 6e6f 7469 6f6e 0a60  ll html2notion.`
-00000630: 6060 0a0a 2323 2050 7265 7061 7265 204e  ``..## Prepare N
-00000640: 6f74 696f 6e20 436f 6e66 6967 7572 6174  otion Configurat
-00000650: 696f 6e0a 0a57 6520 6e65 6564 2074 6f20  ion..We need to 
-00000660: 7573 6520 7468 6520 604e 6f74 696f 6e20  use the `Notion 
-00000670: 4150 4920 6b65 7960 2061 6e64 2060 4461  API key` and `Da
-00000680: 7461 6261 7365 2049 4460 2074 6f20 6175  tabase ID` to au
-00000690: 7468 6f72 697a 6520 6874 6d6c 326e 6f74  thorize html2not
-000006a0: 696f 6e20 746f 2061 6363 6573 7320 7468  ion to access th
-000006b0: 6520 4e6f 7469 6f6e 2064 6174 6162 6173  e Notion databas
-000006c0: 652e 2050 6c65 6173 6520 666f 6c6c 6f77  e. Please follow
-000006d0: 2074 6865 7365 2073 7465 7073 3a0a 0a31   these steps:..1
-000006e0: 2e20 4372 6561 7465 2061 6e20 696e 7465  . Create an inte
-000006f0: 6772 6174 696f 6e3b 0a32 2e20 5368 6172  gration;.2. Shar
-00000700: 6520 6120 6461 7461 6261 7365 2077 6974  e a database wit
-00000710: 6820 796f 7572 2069 6e74 6567 7261 7469  h your integrati
-00000720: 6f6e 3b0a 332e 2045 7870 6f72 7420 7468  on;.3. Export th
-00000730: 6520 6461 7461 6261 7365 2049 443b 0a0a  e database ID;..
-00000740: 5768 656e 2073 6861 7269 6e67 2074 6865  When sharing the
-00000750: 2064 6174 6162 6173 6520 6865 7265 2c20   database here, 
-00000760: 796f 7520 6e65 6564 2074 6f20 6368 6f6f  you need to choo
-00000770: 7365 2074 6865 2070 7265 7669 6f75 736c  se the previousl
-00000780: 7920 6475 706c 6963 6174 6564 2064 6174  y duplicated dat
-00000790: 6162 6173 6520 6265 6361 7573 6520 7468  abase because th
-000007a0: 6520 696d 706f 7274 206f 7065 7261 7469  e import operati
-000007b0: 6f6e 2072 6571 7569 7265 7320 736f 6d65  on requires some
-000007c0: 2070 7265 7365 7420 5b70 726f 7065 7274   preset [propert
-000007d0: 6965 735d 2868 7474 7073 3a2f 2f64 6576  ies](https://dev
-000007e0: 656c 6f70 6572 732e 6e6f 7469 6f6e 2e63  elopers.notion.c
-000007f0: 6f6d 2f72 6566 6572 656e 6365 2f70 726f  om/reference/pro
-00000800: 7065 7274 792d 6f62 6a65 6374 2920 696e  perty-object) in
-00000810: 666f 726d 6174 696f 6e20 696e 2074 6869  formation in thi
-00000820: 7320 6461 7461 6261 7365 2e0a 0a46 6f72  s database...For
-00000830: 2073 7065 6369 6669 6320 6d65 7468 6f64   specific method
-00000840: 732c 2070 6c65 6173 6520 7265 6665 7220  s, please refer 
-00000850: 746f 2074 6865 204e 6f74 696f 6e20 6f66  to the Notion of
-00000860: 6669 6369 616c 2064 6f63 756d 656e 7461  ficial documenta
-00000870: 7469 6f6e 205b 6372 6561 7465 2061 6e20  tion [create an 
-00000880: 696e 7465 6772 6174 696f 6e5d 2868 7474  integration](htt
-00000890: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
-000008a0: 6e6f 7469 6f6e 2e63 6f6d 2f64 6f63 732f  notion.com/docs/
-000008b0: 6372 6561 7465 2d61 2d6e 6f74 696f 6e2d  create-a-notion-
-000008c0: 696e 7465 6772 6174 696f 6e29 2e0a 0a41  integration)...A
-000008d0: 6674 6572 2074 6865 2073 6574 7570 2069  fter the setup i
-000008e0: 7320 636f 6d70 6c65 7465 2c20 7772 6974  s complete, writ
-000008f0: 6520 796f 7572 2041 5049 204b 6579 2061  e your API Key a
-00000900: 6e64 2064 6174 6162 6173 6520 4944 2069  nd database ID i
-00000910: 6e74 6f20 6120 636f 6e66 6967 7572 6174  nto a configurat
-00000920: 696f 6e20 6669 6c65 2063 6f6e 6669 672e  ion file config.
-00000930: 6a73 6f6e 2e0a 0a60 6060 7368 656c 6c0a  json...```shell.
-00000940: 7b0a 2020 2020 226e 6f74 696f 6e22 3a20  {.    "notion": 
-00000950: 7b0a 2020 2020 2020 2020 2264 6174 6162  {.        "datab
-00000960: 6173 655f 6964 223a 2022 3c2a 2a2a 6465  ase_id": "<***de
-00000970: 6d6f 2a2a 2a3e 222c 0a20 2020 2020 2020  mo***>",.       
-00000980: 2022 6170 695f 6b65 7922 3a20 223c 2a2a   "api_key": "<**
-00000990: 2a64 656d 6f2a 2a2a 3e22 0a20 2020 207d  *demo***>".    }
-000009a0: 0a7d 0a60 6060 0a0a 2320 5573 6167 650a  .}.```..# Usage.
-000009b0: 0a59 6f75 2063 616e 2075 7365 2060 6874  .You can use `ht
-000009c0: 6d6c 326e 6f74 696f 6e20 2d68 6020 746f  ml2notion -h` to
-000009d0: 2076 6965 7720 6465 7461 696c 6564 2068   view detailed h
-000009e0: 656c 7020 646f 6375 6d65 6e74 6174 696f  elp documentatio
-000009f0: 6e2e 0a0a 6060 6073 6865 6c6c 0a75 7361  n...```shell.usa
-00000a00: 6765 3a20 6874 6d6c 326e 6f74 696f 6e20  ge: html2notion 
-00000a10: 5b2d 685d 202d 2d63 6f6e 6620 434f 4e46  [-h] --conf CONF
-00000a20: 205b 2d2d 6c6f 6720 4c4f 475d 205b 2d2d   [--log LOG] [--
-00000a30: 6261 7463 6820 4241 5443 485d 2028 2d2d  batch BATCH] (--
-00000a40: 6669 6c65 2046 494c 4520 7c20 2d2d 6469  file FILE | --di
-00000a50: 7220 4449 5229 0a0a 4874 6d6c 326e 6f74  r DIR)..Html2not
-00000a60: 696f 6e3a 2053 6176 6520 4854 4d4c 2074  ion: Save HTML t
-00000a70: 6f20 796f 7572 204e 6f74 696f 6e20 6e6f  o your Notion no
-00000a80: 7465 7320 7175 6963 6b6c 7920 616e 6420  tes quickly and 
-00000a90: 6561 7369 6c79 2c20 7768 696c 6520 6b65  easily, while ke
-00000aa0: 6570 696e 6720 7468 6520 6f72 6967 696e  eping the origin
-00000ab0: 616c 2066 6f72 6d61 7420 6173 206d 7563  al format as muc
-00000ac0: 6820 6173 2070 6f73 7369 626c 650a 0a6f  h as possible..o
-00000ad0: 7074 696f 6e73 3a0a 2020 2d68 2c20 2d2d  ptions:.  -h, --
-00000ae0: 6865 6c70 2020 2020 2073 686f 7720 7468  help     show th
-00000af0: 6973 2068 656c 7020 6d65 7373 6167 6520  is help message 
-00000b00: 616e 6420 6578 6974 0a20 202d 2d63 6f6e  and exit.  --con
-00000b10: 6620 434f 4e46 2020 2020 636f 6e66 2066  f CONF    conf f
-00000b20: 696c 6520 7061 7468 0a20 202d 2d6c 6f67  ile path.  --log
-00000b30: 204c 4f47 2020 2020 2020 6c6f 6720 6469   LOG      log di
-00000b40: 7265 6374 2070 6174 680a 2020 2d2d 6261  rect path.  --ba
-00000b50: 7463 6820 4241 5443 4820 2062 6174 6368  tch BATCH  batch
-00000b60: 2073 6176 6520 636f 6e63 7572 7265 6e74   save concurrent
-00000b70: 206c 696d 6974 0a20 202d 2d66 696c 6520   limit.  --file 
-00000b80: 4649 4c45 2020 2020 5361 7665 2073 696e  FILE    Save sin
-00000b90: 676c 6520 6874 6d6c 2066 696c 6520 746f  gle html file to
-00000ba0: 206e 6f74 696f 6e0a 2020 2d2d 6469 7220   notion.  --dir 
-00000bb0: 4449 5220 2020 2020 2053 6176 6520 616c  DIR      Save al
-00000bc0: 6c20 6874 6d6c 2066 696c 6573 2069 6e20  l html files in 
-00000bd0: 7468 6520 6469 7220 746f 206e 6f74 696f  the dir to notio
-00000be0: 6e0a 6060 600a 0a46 6f72 2065 7861 6d70  n.```..For examp
-00000bf0: 6c65 2c20 6966 2079 6f75 2077 616e 7420  le, if you want 
-00000c00: 746f 2069 6d70 6f72 7420 616c 6c20 6874  to import all ht
-00000c10: 6d6c 2066 696c 6573 2069 6e20 7468 6520  ml files in the 
-00000c20: 602e 2f64 656d 6f73 6020 6469 7265 6374  `./demos` direct
-00000c30: 6f72 7920 696e 746f 204e 6f74 696f 6e2c  ory into Notion,
-00000c40: 2079 6f75 2063 616e 2075 7365 2074 6865   you can use the
-00000c50: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00000c60: 6e64 3a0a 0a60 6060 7368 656c 6c0a 6874  nd:..```shell.ht
-00000c70: 6d6c 326e 6f74 696f 6e20 2d2d 636f 6e66  ml2notion --conf
-00000c80: 2063 6f6e 6669 672e 6a73 6f6e 202d 2d64   config.json --d
-00000c90: 6972 202e 2f64 656d 6f73 202d 2d6c 6f67  ir ./demos --log
-00000ca0: 207e 2f6c 6f67 7320 2d2d 6261 7463 6820   ~/logs --batch 
-00000cb0: 3130 0a60 6060 0a0a 5468 6520 6162 6f76  10.```..The abov
-00000cc0: 6520 636f 6d6d 616e 6420 7769 6c6c 2069  e command will i
-00000cd0: 6d70 6f72 7420 616c 6c20 6874 6d6c 2066  mport all html f
-00000ce0: 696c 6573 2069 6e20 7468 6520 602e 2f64  iles in the `./d
-00000cf0: 656d 6f73 6020 6469 7265 6374 6f72 7920  emos` directory 
-00000d00: 696e 746f 204e 6f74 696f 6e2c 2077 6869  into Notion, whi
-00000d10: 6c65 206f 7574 7075 7474 696e 6720 6c6f  le outputting lo
-00000d20: 6773 2074 6f20 7468 6520 607e 2f6c 6f67  gs to the `~/log
-00000d30: 7360 2064 6972 6563 746f 7279 2c20 7769  s` directory, wi
-00000d40: 7468 2075 7020 746f 2031 3020 636f 6e63  th up to 10 conc
-00000d50: 7572 7265 6e74 2074 6173 6b73 2e0a 0a23  urrent tasks...#
-00000d60: 204d 6f72 6520 696e 666f 726d 6174 696f   More informatio
-00000d70: 6e0a 0a59 6f75 2063 616e 2066 696e 6420  n..You can find 
-00000d80: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-00000d90: 2061 6e64 2065 7861 6d70 6c65 7320 696e   and examples in
-00000da0: 2074 6865 2068 746d 6c32 6e6f 7469 6f6e   the html2notion
-00000db0: 206c 6962 7261 7279 2773 2049 7373 7565   library's Issue
-00000dc0: 3a20 5b68 746d 6c32 6e6f 7469 6f6e 5d28  : [html2notion](
-00000dd0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000de0: 6f6d 2f73 656c 6662 6f6f 742f 6874 6d6c  om/selfboot/html
-00000df0: 326e 6f74 696f 6e2f 6973 7375 6573 290a  2notion/issues).
-00000e00: 0a23 2320 436f 6e74 7269 6275 7469 6f6e  .## Contribution
-00000e10: 0a0a 4966 2079 6f75 2066 696e 6420 616e  ..If you find an
-00000e20: 7920 6572 726f 7273 206f 7220 6861 7665  y errors or have
-00000e30: 2061 6e79 2073 7567 6765 7374 696f 6e73   any suggestions
-00000e40: 2066 6f72 2069 6d70 726f 7665 6d65 6e74   for improvement
-00000e50: 2c20 706c 6561 7365 2064 6f20 6e6f 7420  , please do not 
-00000e60: 6865 7369 7461 7465 2074 6f20 7375 626d  hesitate to subm
-00000e70: 6974 2061 2070 756c 6c20 7265 7175 6573  it a pull reques
-00000e80: 7420 6f72 2072 6169 7365 2061 6e20 6973  t or raise an is
-00000e90: 7375 652c 2049 2061 6d20 6d6f 7265 2074  sue, I am more t
-00000ea0: 6861 6e20 6861 7070 7920 746f 2061 6363  han happy to acc
-00000eb0: 6570 7420 796f 7572 2063 6f6e 7472 6962  ept your contrib
-00000ec0: 7574 696f 6e73 2061 6e64 2066 6565 6462  utions and feedb
-00000ed0: 6163 6b21 0a0a 4966 2079 6f75 2065 6e63  ack!..If you enc
-00000ee0: 6f75 6e74 6572 2069 6d70 6f72 7420 6661  ounter import fa
-00000ef0: 696c 7572 6573 2c20 796f 7520 6361 6e20  ilures, you can 
-00000f00: 7375 626d 6974 2074 6865 2068 746d 6c20  submit the html 
-00000f10: 6669 6c65 2061 6e64 206c 6f67 2066 696c  file and log fil
-00000f20: 6520 746f 6765 7468 6572 2069 6e20 7468  e together in th
-00000f30: 6520 6973 7375 6520 666f 7220 6561 7369  e issue for easi
-00000f40: 6572 2070 726f 626c 656d 2069 6465 6e74  er problem ident
-00000f50: 6966 6963 6174 696f 6e2e 0a0a 3e20 4966  ification...> If
-00000f60: 2074 6865 7265 2061 7265 2061 6e79 2070   there are any p
-00000f70: 7269 7661 7465 2069 6e66 6f72 6d61 7469  rivate informati
-00000f80: 6f6e 2069 6e20 7468 6520 6669 6c65 732c  on in the files,
-00000f90: 2070 6c65 6173 6520 7265 6d6f 7665 2069   please remove i
-00000fa0: 7420 6669 7273 742e 0a0a 0a23 2320 4c69  t first....## Li
-00000fb0: 6365 6e73 650a 0a54 6869 7320 7072 6f6a  cense..This proj
-00000fc0: 6563 7420 7573 6573 2074 6865 204d 4954  ect uses the MIT
-00000fd0: 206c 6963 656e 7365 2e20 506c 6561 7365   license. Please
-00000fe0: 2072 6566 6572 2074 6f20 7468 6520 5b4c   refer to the [L
-00000ff0: 4943 454e 5345 5d28 2e2f 4c49 4345 4e53  ICENSE](./LICENS
-00001000: 4529 2066 6f72 2064 6574 6169 6c73 2e    E) for details.
+00000000: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+00000010: 7222 3e48 746d 6c32 6e6f 7469 6f6e 203c  r">Html2notion <
+00000020: 6120 6872 6566 3d27 6874 7470 733a 2f2f  a href='https://
+00000030: 6769 7468 7562 2e63 6f6d 2f73 656c 6662  github.com/selfb
+00000040: 6f6f 742f 6874 6d6c 326e 6f74 696f 6e2f  oot/html2notion/
+00000050: 626c 6f62 2f6d 6173 7465 722f 5245 4144  blob/master/READ
+00000060: 4d45 5f7a 682e 6d64 273e e7ae 80e4 bd93  ME_zh.md'>......
+00000070: e4b8 ade6 9687 3c2f 613e 3c2f 6831 3e0a  ......</a></h1>.
+00000080: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000090: 223e 0a20 203c 6120 6872 6566 3d22 6874  ">.  <a href="ht
+000000a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000000b0: 2f73 656c 6662 6f6f 742f 6874 6d6c 326e  /selfboot/html2n
+000000c0: 6f74 696f 6e2f 6163 7469 6f6e 732f 776f  otion/actions/wo
+000000d0: 726b 666c 6f77 732f 7079 7468 6f6e 2d70  rkflows/python-p
+000000e0: 6163 6b61 6765 2e79 6d6c 223e 0a20 2020  ackage.yml">.   
+000000f0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000100: 3a2f 2f67 6974 6875 622e 636f 6d2f 7365  ://github.com/se
+00000110: 6c66 626f 6f74 2f68 746d 6c32 6e6f 7469  lfboot/html2noti
+00000120: 6f6e 2f61 6374 696f 6e73 2f77 6f72 6b66  on/actions/workf
+00000130: 6c6f 7773 2f70 7974 686f 6e2d 7061 636b  lows/python-pack
+00000140: 6167 652e 796d 6c2f 6261 6467 652e 7376  age.yml/badge.sv
+00000150: 6722 2061 6c74 3d22 4349 2054 6573 7420  g" alt="CI Test 
+00000160: 5374 6174 7573 223e 0a20 203c 2f61 3e0a  Status">.  </a>.
+00000170: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000180: 2f2f 636f 6465 636f 762e 696f 2f67 682f  //codecov.io/gh/
+00000190: 7365 6c66 626f 6f74 2f68 746d 6c32 6e6f  selfboot/html2no
+000001a0: 7469 6f6e 2220 3e0a 203c 696d 6720 7372  tion" >. <img sr
+000001b0: 633d 2268 7474 7073 3a2f 2f63 6f64 6563  c="https://codec
+000001c0: 6f76 2e69 6f2f 6768 2f73 656c 6662 6f6f  ov.io/gh/selfboo
+000001d0: 742f 6874 6d6c 326e 6f74 696f 6e2f 6272  t/html2notion/br
+000001e0: 616e 6368 2f6d 6173 7465 722f 6772 6170  anch/master/grap
+000001f0: 682f 6261 6467 652e 7376 673f 746f 6b65  h/badge.svg?toke
+00000200: 6e3d 5349 4d36 4937 425a 5536 2220 616c  n=SIM6I7BZU6" al
+00000210: 743d 2254 6573 7420 636f 7665 7261 6765  t="Test coverage
+00000220: 222f 3e0a 203c 2f61 3e0a 3c2f 703e 0a0a  "/>. </a>.</p>..
+00000230: 6874 6d6c 326e 6f74 696f 6e20 6973 2061  html2notion is a
+00000240: 6e20 696e 6372 6564 6962 6c79 2075 7365  n incredibly use
+00000250: 6675 6c20 746f 6f6c 2077 7269 7474 656e  ful tool written
+00000260: 2069 6e20 5079 7468 6f6e 2c20 7768 6963   in Python, whic
+00000270: 6820 616c 6c6f 7773 2079 6f75 2074 6f20  h allows you to 
+00000280: 696d 706f 7274 2063 6f6e 7465 6e74 2066  import content f
+00000290: 726f 6d20 4854 4d4c 2064 6f63 756d 656e  rom HTML documen
+000002a0: 7473 2069 6e74 6f20 4e6f 7469 6f6e 206e  ts into Notion n
+000002b0: 6f74 6573 2c20 6d61 6b69 6e67 2069 7420  otes, making it 
+000002c0: 6d6f 7265 2063 6f6e 7665 6e69 656e 7420  more convenient 
+000002d0: 666f 7220 796f 7520 746f 206f 7267 616e  for you to organ
+000002e0: 697a 6520 696e 666f 726d 6174 696f 6e20  ize information 
+000002f0: 6f6e 2074 6865 204e 6f74 696f 6e20 706c  on the Notion pl
+00000300: 6174 666f 726d 2e20 496e 2061 6464 6974  atform. In addit
+00000310: 696f 6e2c 2068 746d 6c32 6e6f 7469 6f6e  ion, html2notion
+00000320: 2068 6173 2062 6565 6e20 7370 6563 6966   has been specif
+00000330: 6963 616c 6c79 206f 7074 696d 697a 6564  ically optimized
+00000340: 2066 6f72 2074 6865 2063 6f6e 7465 6e74   for the content
+00000350: 206f 6620 4576 6572 6e6f 7465 2c20 616e   of Evernote, an
+00000360: 6420 796f 7520 6361 6e20 616c 736f 2075  d you can also u
+00000370: 7365 2069 7420 746f 2069 6d70 6f72 7420  se it to import 
+00000380: 6e6f 7465 7320 6672 6f6d 2045 7665 726e  notes from Evern
+00000390: 6f74 6520 696e 746f 204e 6f74 696f 6e2e  ote into Notion.
+000003a0: 0a0a 6874 6d6c 326e 6f74 696f 6e20 6861  ..html2notion ha
+000003b0: 7320 706f 7765 7266 756c 2066 6561 7475  s powerful featu
+000003c0: 7265 7320 616e 6420 7375 7070 6f72 7473  res and supports
+000003d0: 2063 6f6e 7665 7274 696e 6720 7661 7269   converting vari
+000003e0: 6f75 7320 7461 6773 2069 6e20 4854 4d4c  ous tags in HTML
+000003f0: 2066 696c 6573 2069 6e74 6f20 636f 7272   files into corr
+00000400: 6573 706f 6e64 696e 6720 426c 6f63 6b73  esponding Blocks
+00000410: 2069 6e20 4e6f 7469 6f6e 2c20 7375 6368   in Notion, such
+00000420: 2061 7320 7269 6368 2074 6578 7420 626c   as rich text bl
+00000430: 6f63 6b73 2c20 6865 6164 696e 6773 2c20  ocks, headings, 
+00000440: 696d 6167 6573 2c20 636f 6465 2062 6c6f  images, code blo
+00000450: 636b 732c 2071 756f 7465 732c 206c 696e  cks, quotes, lin
+00000460: 6b73 2c20 6574 632e 2042 656c 6f77 2061  ks, etc. Below a
+00000470: 7265 2065 7861 6d70 6c65 7320 6f66 2063  re examples of c
+00000480: 6f6e 7665 7274 696e 6720 6e6f 7465 7320  onverting notes 
+00000490: 6672 6f6d 2045 7665 726e 6f74 6520 696e  from Evernote in
+000004a0: 746f 204e 6f74 696f 6e20 7061 6765 732e  to Notion pages.
+000004b0: 0a0a 215b 7969 6e78 6961 6e67 206e 6f74  ..![yinxiang not
+000004c0: 696f 6e28 7369 6d70 6c65 2064 656d 6f73  ion(simple demos
+000004d0: 295d 2868 7474 7073 3a2f 2f72 6177 2e67  )](https://raw.g
+000004e0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+000004f0: 2e63 6f6d 2f73 656c 6662 6f6f 742f 6874  .com/selfboot/ht
+00000500: 6d6c 326e 6f74 696f 6e2f 6d61 7374 6572  ml2notion/master
+00000510: 2f64 656d 6f73 2f79 696e 7869 616e 675f  /demos/yinxiang_
+00000520: 6e6f 7469 6f6e 2e70 6e67 290a 0a21 5b79  notion.png)..![y
+00000530: 696e 7869 616e 6720 6e6f 7469 6f6e 3228  inxiang notion2(
+00000540: 7269 6368 2074 6578 7429 5d28 6874 7470  rich text)](http
+00000550: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000560: 6572 636f 6e74 656e 742e 636f 6d2f 7365  ercontent.com/se
+00000570: 6c66 626f 6f74 2f68 746d 6c32 6e6f 7469  lfboot/html2noti
+00000580: 6f6e 2f6d 6173 7465 722f 6465 6d6f 732f  on/master/demos/
+00000590: 7969 6e78 6961 6e67 5f6e 6f74 696f 6e32  yinxiang_notion2
+000005a0: 2e70 6e67 290a 0a23 2050 7265 7061 7265  .png)..# Prepare
+000005b0: 0a0a 596f 7520 6f6e 6c79 206e 6565 6420  ..You only need 
+000005c0: 3320 7374 6570 7320 746f 2075 7365 2068  3 steps to use h
+000005d0: 746d 6c6e 6f74 696f 6e20 746f 2069 6d70  tmlnotion to imp
+000005e0: 6f72 7420 4854 4d4c 2069 6e74 6f20 4e6f  ort HTML into No
+000005f0: 7469 6f6e 2e0a 0a23 2320 4475 706c 6963  tion...## Duplic
+00000600: 6174 6520 6461 7461 6261 7365 0a0a 436c  ate database..Cl
+00000610: 6963 6b20 7468 6520 6c69 6e6b 205b 6e6f  ick the link [no
+00000620: 7469 6f6e 2074 656d 706c 6174 655d 2868  tion template](h
+00000630: 7474 7073 3a2f 2f73 656c 6662 6f6f 742e  ttps://selfboot.
+00000640: 6e6f 7469 6f6e 2e73 6974 652f 7365 6c66  notion.site/self
+00000650: 626f 6f74 2f31 3330 6262 3438 6336 6362  boot/130bb48c6cb
+00000660: 6434 6162 6262 6237 3133 6434 6438 3437  d4abbbb713d4d847
+00000670: 3234 3831 613f 763d 6464 6461 3230 6433  2481a?v=ddda20d3
+00000680: 6634 3662 3462 3434 6130 3535 6430 3637  f46b4b44a055d067
+00000690: 3932 6331 3432 6630 292e 2041 7320 7368  92c142f0). As sh
+000006a0: 6f77 6e20 696e 2074 6865 2069 6d61 6765  own in the image
+000006b0: 2062 656c 6f77 2c20 7573 6520 7468 6520   below, use the 
+000006c0: 2244 7570 6c69 6361 7465 2220 6275 7474  "Duplicate" butt
+000006d0: 6f6e 2074 6f20 636f 7079 2061 206e 6577  on to copy a new
+000006e0: 2064 6174 6162 6173 6520 746f 2079 6f75   database to you
+000006f0: 7220 6f77 6e20 4e6f 7469 6f6e 2077 6f72  r own Notion wor
+00000700: 6b73 7061 6365 2e0a 0a21 5b6e 6f74 696f  kspace...![notio
+00000710: 6e20 7465 6d70 6c61 7465 5d28 6874 7470  n template](http
+00000720: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000730: 6572 636f 6e74 656e 742e 636f 6d2f 7365  ercontent.com/se
+00000740: 6c66 626f 6f74 2f68 746d 6c32 6e6f 7469  lfboot/html2noti
+00000750: 6f6e 2f6d 6173 7465 722f 6465 6d6f 732f  on/master/demos/
+00000760: 6e6f 7469 6f6e 5f74 656d 706c 6167 652e  notion_templage.
+00000770: 706e 6729 0a0a 2323 2049 6e73 7461 6c6c  png)..## Install
+00000780: 2068 746d 6c32 6e6f 7469 6f6e 0a0a 5265   html2notion..Re
+00000790: 7175 6972 6573 2070 7974 686f 6e3e 3d33  quires python>=3
+000007a0: 2e38 2c20 696e 7374 616c 6c20 7468 6520  .8, install the 
+000007b0: 6874 6d6c 326e 6f74 696f 6e20 6c69 6272  html2notion libr
+000007c0: 6172 792e 2059 6f75 2063 616e 2075 7365  ary. You can use
+000007d0: 2074 6865 2070 6970 2063 6f6d 6d61 6e64   the pip command
+000007e0: 2074 6f20 696e 7374 616c 6c20 6974 3a0a   to install it:.
+000007f0: 0a60 6060 0a70 6970 2069 6e73 7461 6c6c  .```.pip install
+00000800: 2068 746d 6c32 6e6f 7469 6f6e 0a60 6060   html2notion.```
+00000810: 0a0a 2323 2050 7265 7061 7265 204e 6f74  ..## Prepare Not
+00000820: 696f 6e20 436f 6e66 6967 7572 6174 696f  ion Configuratio
+00000830: 6e0a 0a57 6520 6e65 6564 2074 6f20 7573  n..We need to us
+00000840: 6520 7468 6520 604e 6f74 696f 6e20 4150  e the `Notion AP
+00000850: 4920 6b65 7960 2061 6e64 2060 4461 7461  I key` and `Data
+00000860: 6261 7365 2049 4460 2074 6f20 6175 7468  base ID` to auth
+00000870: 6f72 697a 6520 6874 6d6c 326e 6f74 696f  orize html2notio
+00000880: 6e20 746f 2061 6363 6573 7320 7468 6520  n to access the 
+00000890: 4e6f 7469 6f6e 2064 6174 6162 6173 652e  Notion database.
+000008a0: 2050 6c65 6173 6520 666f 6c6c 6f77 2074   Please follow t
+000008b0: 6865 7365 2073 7465 7073 3a0a 0a31 2e20  hese steps:..1. 
+000008c0: 4372 6561 7465 2061 6e20 696e 7465 6772  Create an integr
+000008d0: 6174 696f 6e3b 0a32 2e20 5368 6172 6520  ation;.2. Share 
+000008e0: 6120 6461 7461 6261 7365 2077 6974 6820  a database with 
+000008f0: 796f 7572 2069 6e74 6567 7261 7469 6f6e  your integration
+00000900: 3b0a 332e 2045 7870 6f72 7420 7468 6520  ;.3. Export the 
+00000910: 6461 7461 6261 7365 2049 443b 0a0a 5768  database ID;..Wh
+00000920: 656e 2073 6861 7269 6e67 2074 6865 2064  en sharing the d
+00000930: 6174 6162 6173 6520 6865 7265 2c20 796f  atabase here, yo
+00000940: 7520 6e65 6564 2074 6f20 6368 6f6f 7365  u need to choose
+00000950: 2074 6865 2070 7265 7669 6f75 736c 7920   the previously 
+00000960: 6475 706c 6963 6174 6564 2064 6174 6162  duplicated datab
+00000970: 6173 6520 6265 6361 7573 6520 7468 6520  ase because the 
+00000980: 696d 706f 7274 206f 7065 7261 7469 6f6e  import operation
+00000990: 2072 6571 7569 7265 7320 736f 6d65 2070   requires some p
+000009a0: 7265 7365 7420 5b70 726f 7065 7274 6965  reset [propertie
+000009b0: 735d 2868 7474 7073 3a2f 2f64 6576 656c  s](https://devel
+000009c0: 6f70 6572 732e 6e6f 7469 6f6e 2e63 6f6d  opers.notion.com
+000009d0: 2f72 6566 6572 656e 6365 2f70 726f 7065  /reference/prope
+000009e0: 7274 792d 6f62 6a65 6374 2920 696e 666f  rty-object) info
+000009f0: 726d 6174 696f 6e20 696e 2074 6869 7320  rmation in this 
+00000a00: 6461 7461 6261 7365 2e0a 0a46 6f72 2073  database...For s
+00000a10: 7065 6369 6669 6320 6d65 7468 6f64 732c  pecific methods,
+00000a20: 2070 6c65 6173 6520 7265 6665 7220 746f   please refer to
+00000a30: 2074 6865 204e 6f74 696f 6e20 6f66 6669   the Notion offi
+00000a40: 6369 616c 2064 6f63 756d 656e 7461 7469  cial documentati
+00000a50: 6f6e 205b 6372 6561 7465 2061 6e20 696e  on [create an in
+00000a60: 7465 6772 6174 696f 6e5d 2868 7474 7073  tegration](https
+00000a70: 3a2f 2f64 6576 656c 6f70 6572 732e 6e6f  ://developers.no
+00000a80: 7469 6f6e 2e63 6f6d 2f64 6f63 732f 6372  tion.com/docs/cr
+00000a90: 6561 7465 2d61 2d6e 6f74 696f 6e2d 696e  eate-a-notion-in
+00000aa0: 7465 6772 6174 696f 6e29 2e0a 0a41 6674  tegration)...Aft
+00000ab0: 6572 2074 6865 2073 6574 7570 2069 7320  er the setup is 
+00000ac0: 636f 6d70 6c65 7465 2c20 7772 6974 6520  complete, write 
+00000ad0: 796f 7572 2041 5049 204b 6579 2061 6e64  your API Key and
+00000ae0: 2064 6174 6162 6173 6520 4944 2069 6e74   database ID int
+00000af0: 6f20 6120 636f 6e66 6967 7572 6174 696f  o a configuratio
+00000b00: 6e20 6669 6c65 2063 6f6e 6669 672e 6a73  n file config.js
+00000b10: 6f6e 2e0a 0a60 6060 7368 656c 6c0a 7b0a  on...```shell.{.
+00000b20: 2020 2020 226e 6f74 696f 6e22 3a20 7b0a      "notion": {.
+00000b30: 2020 2020 2020 2020 2264 6174 6162 6173          "databas
+00000b40: 655f 6964 223a 2022 3c2a 2a2a 6465 6d6f  e_id": "<***demo
+00000b50: 2a2a 2a3e 222c 0a20 2020 2020 2020 2022  ***>",.        "
+00000b60: 6170 695f 6b65 7922 3a20 223c 2a2a 2a64  api_key": "<***d
+00000b70: 656d 6f2a 2a2a 3e22 0a20 2020 207d 0a7d  emo***>".    }.}
+00000b80: 0a60 6060 0a0a 2320 5573 6167 650a 0a59  .```..# Usage..Y
+00000b90: 6f75 2063 616e 2075 7365 2060 6874 6d6c  ou can use `html
+00000ba0: 326e 6f74 696f 6e20 2d68 6020 746f 2076  2notion -h` to v
+00000bb0: 6965 7720 6465 7461 696c 6564 2068 656c  iew detailed hel
+00000bc0: 7020 646f 6375 6d65 6e74 6174 696f 6e2e  p documentation.
+00000bd0: 0a0a 6060 6073 6865 6c6c 0a75 7361 6765  ..```shell.usage
+00000be0: 3a20 6874 6d6c 326e 6f74 696f 6e20 5b2d  : html2notion [-
+00000bf0: 685d 202d 2d63 6f6e 6620 434f 4e46 205b  h] --conf CONF [
+00000c00: 2d2d 6c6f 6720 4c4f 475d 205b 2d2d 6261  --log LOG] [--ba
+00000c10: 7463 6820 4241 5443 485d 2028 2d2d 6669  tch BATCH] (--fi
+00000c20: 6c65 2046 494c 4520 7c20 2d2d 6469 7220  le FILE | --dir 
+00000c30: 4449 5229 0a0a 4874 6d6c 326e 6f74 696f  DIR)..Html2notio
+00000c40: 6e3a 2053 6176 6520 4854 4d4c 2074 6f20  n: Save HTML to 
+00000c50: 796f 7572 204e 6f74 696f 6e20 6e6f 7465  your Notion note
+00000c60: 7320 7175 6963 6b6c 7920 616e 6420 6561  s quickly and ea
+00000c70: 7369 6c79 2c20 7768 696c 6520 6b65 6570  sily, while keep
+00000c80: 696e 6720 7468 6520 6f72 6967 696e 616c  ing the original
+00000c90: 2066 6f72 6d61 7420 6173 206d 7563 6820   format as much 
+00000ca0: 6173 2070 6f73 7369 626c 650a 0a6f 7074  as possible..opt
+00000cb0: 696f 6e73 3a0a 2020 2d68 2c20 2d2d 6865  ions:.  -h, --he
+00000cc0: 6c70 2020 2020 2073 686f 7720 7468 6973  lp     show this
+00000cd0: 2068 656c 7020 6d65 7373 6167 6520 616e   help message an
+00000ce0: 6420 6578 6974 0a20 202d 2d63 6f6e 6620  d exit.  --conf 
+00000cf0: 434f 4e46 2020 2020 636f 6e66 2066 696c  CONF    conf fil
+00000d00: 6520 7061 7468 0a20 202d 2d6c 6f67 204c  e path.  --log L
+00000d10: 4f47 2020 2020 2020 6c6f 6720 6469 7265  OG      log dire
+00000d20: 6374 2070 6174 680a 2020 2d2d 6261 7463  ct path.  --batc
+00000d30: 6820 4241 5443 4820 2062 6174 6368 2073  h BATCH  batch s
+00000d40: 6176 6520 636f 6e63 7572 7265 6e74 206c  ave concurrent l
+00000d50: 696d 6974 0a20 202d 2d66 696c 6520 4649  imit.  --file FI
+00000d60: 4c45 2020 2020 5361 7665 2073 696e 676c  LE    Save singl
+00000d70: 6520 6874 6d6c 2066 696c 6520 746f 206e  e html file to n
+00000d80: 6f74 696f 6e0a 2020 2d2d 6469 7220 4449  otion.  --dir DI
+00000d90: 5220 2020 2020 2053 6176 6520 616c 6c20  R      Save all 
+00000da0: 6874 6d6c 2066 696c 6573 2069 6e20 7468  html files in th
+00000db0: 6520 6469 7220 746f 206e 6f74 696f 6e0a  e dir to notion.
+00000dc0: 6060 600a 0a46 6f72 2065 7861 6d70 6c65  ```..For example
+00000dd0: 2c20 6966 2079 6f75 2077 616e 7420 746f  , if you want to
+00000de0: 2069 6d70 6f72 7420 616c 6c20 6874 6d6c   import all html
+00000df0: 2066 696c 6573 2069 6e20 7468 6520 602e   files in the `.
+00000e00: 2f64 656d 6f73 6020 6469 7265 6374 6f72  /demos` director
+00000e10: 7920 696e 746f 204e 6f74 696f 6e2c 2079  y into Notion, y
+00000e20: 6f75 2063 616e 2075 7365 2074 6865 2066  ou can use the f
+00000e30: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00000e40: 3a0a 0a60 6060 7368 656c 6c0a 6874 6d6c  :..```shell.html
+00000e50: 326e 6f74 696f 6e20 2d2d 636f 6e66 2063  2notion --conf c
+00000e60: 6f6e 6669 672e 6a73 6f6e 202d 2d64 6972  onfig.json --dir
+00000e70: 202e 2f64 656d 6f73 202d 2d6c 6f67 207e   ./demos --log ~
+00000e80: 2f6c 6f67 7320 2d2d 6261 7463 6820 3130  /logs --batch 10
+00000e90: 0a60 6060 0a0a 5468 6520 6162 6f76 6520  .```..The above 
+00000ea0: 636f 6d6d 616e 6420 7769 6c6c 2069 6d70  command will imp
+00000eb0: 6f72 7420 616c 6c20 6874 6d6c 2066 696c  ort all html fil
+00000ec0: 6573 2069 6e20 7468 6520 602e 2f64 656d  es in the `./dem
+00000ed0: 6f73 6020 6469 7265 6374 6f72 7920 696e  os` directory in
+00000ee0: 746f 204e 6f74 696f 6e2c 2077 6869 6c65  to Notion, while
+00000ef0: 206f 7574 7075 7474 696e 6720 6c6f 6773   outputting logs
+00000f00: 2074 6f20 7468 6520 607e 2f6c 6f67 7360   to the `~/logs`
+00000f10: 2064 6972 6563 746f 7279 2c20 7769 7468   directory, with
+00000f20: 2075 7020 746f 2031 3020 636f 6e63 7572   up to 10 concur
+00000f30: 7265 6e74 2074 6173 6b73 2e0a 0a23 204d  rent tasks...# M
+00000f40: 6f72 6520 696e 666f 726d 6174 696f 6e0a  ore information.
+00000f50: 0a59 6f75 2063 616e 2066 696e 6420 6d6f  .You can find mo
+00000f60: 7265 2069 6e66 6f72 6d61 7469 6f6e 2061  re information a
+00000f70: 6e64 2065 7861 6d70 6c65 7320 696e 2074  nd examples in t
+00000f80: 6865 2068 746d 6c32 6e6f 7469 6f6e 206c  he html2notion l
+00000f90: 6962 7261 7279 2773 2049 7373 7565 3a20  ibrary's Issue: 
+00000fa0: 5b68 746d 6c32 6e6f 7469 6f6e 5d28 6874  [html2notion](ht
+00000fb0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000fc0: 2f73 656c 6662 6f6f 742f 6874 6d6c 326e  /selfboot/html2n
+00000fd0: 6f74 696f 6e2f 6973 7375 6573 290a 0a23  otion/issues)..#
+00000fe0: 2320 436f 6e74 7269 6275 7469 6f6e 0a0a  # Contribution..
+00000ff0: 4966 2079 6f75 2066 696e 6420 616e 7920  If you find any 
+00001000: 6572 726f 7273 206f 7220 6861 7665 2061  errors or have a
+00001010: 6e79 2073 7567 6765 7374 696f 6e73 2066  ny suggestions f
+00001020: 6f72 2069 6d70 726f 7665 6d65 6e74 2c20  or improvement, 
+00001030: 706c 6561 7365 2064 6f20 6e6f 7420 6865  please do not he
+00001040: 7369 7461 7465 2074 6f20 7375 626d 6974  sitate to submit
+00001050: 2061 2070 756c 6c20 7265 7175 6573 7420   a pull request 
+00001060: 6f72 2072 6169 7365 2061 6e20 6973 7375  or raise an issu
+00001070: 652c 2049 2061 6d20 6d6f 7265 2074 6861  e, I am more tha
+00001080: 6e20 6861 7070 7920 746f 2061 6363 6570  n happy to accep
+00001090: 7420 796f 7572 2063 6f6e 7472 6962 7574  t your contribut
+000010a0: 696f 6e73 2061 6e64 2066 6565 6462 6163  ions and feedbac
+000010b0: 6b21 0a0a 4966 2079 6f75 2065 6e63 6f75  k!..If you encou
+000010c0: 6e74 6572 2069 6d70 6f72 7420 6661 696c  nter import fail
+000010d0: 7572 6573 2c20 796f 7520 6361 6e20 7375  ures, you can su
+000010e0: 626d 6974 2074 6865 2068 746d 6c20 6669  bmit the html fi
+000010f0: 6c65 2061 6e64 206c 6f67 2066 696c 6520  le and log file 
+00001100: 746f 6765 7468 6572 2069 6e20 7468 6520  together in the 
+00001110: 6973 7375 6520 666f 7220 6561 7369 6572  issue for easier
+00001120: 2070 726f 626c 656d 2069 6465 6e74 6966   problem identif
+00001130: 6963 6174 696f 6e2e 0a0a 3e20 4966 2074  ication...> If t
+00001140: 6865 7265 2061 7265 2061 6e79 2070 7269  here are any pri
+00001150: 7661 7465 2069 6e66 6f72 6d61 7469 6f6e  vate information
+00001160: 2069 6e20 7468 6520 6669 6c65 732c 2070   in the files, p
+00001170: 6c65 6173 6520 7265 6d6f 7665 2069 7420  lease remove it 
+00001180: 6669 7273 742e 0a0a 0a23 2320 4c69 6365  first....## Lice
+00001190: 6e73 650a 0a54 6869 7320 7072 6f6a 6563  nse..This projec
+000011a0: 7420 7573 6573 2074 6865 204d 4954 206c  t uses the MIT l
+000011b0: 6963 656e 7365 2e20 506c 6561 7365 2072  icense. Please r
+000011c0: 6566 6572 2074 6f20 7468 6520 5b4c 4943  efer to the [LIC
+000011d0: 454e 5345 5d28 2e2f 4c49 4345 4e53 4529  ENSE](./LICENSE)
+000011e0: 2066 6f72 2064 6574 6169 6c73 2e0a        for details..
```

### Comparing `html2notion-0.1.9/html2notion/main.py` & `html2notion-0.2.0/html2notion/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import os
 import sys
+import json
 import asyncio
 from pathlib import Path
 from aiohttp import ClientSession
 from notion_client import AsyncClient
 from rich.console import Console
 from rich.table import Table
 from rich.text import Text
@@ -12,31 +13,33 @@
 from .utils import setup_logger, read_config, logger, config
 from .translate.notion_import import NotionImporter
 from .translate.batch_import import BatchImport
 from .translate.import_stats import StatLevel
 console = Console()
 
 
-def parse_args():
+def prepare_args():
     parser = argparse.ArgumentParser(
         description='Html2notion: Save HTML to your Notion notes quickly and easily, while keeping the original format as much as possible')
     parser.add_argument('--conf', type=str, help='conf file path', required=True)
-    parser.add_argument('--log', type=str, help='log direct path')
+    parser.add_argument('--log', type=str, help='log directory path')
     parser.add_argument('--batch', type=int, default=15, help='batch save concurrent limit')
 
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument('--file', type=str, help='Save single html file to notion')
     group.add_argument('--dir', type=str, help='Save all html files in the dir to notion')
-    return parser.parse_args()
+    return parser
 
 
 def print_single_stats(stat):
     if stat.get_level() == StatLevel.EXCEPTION.value:
         text = Text(f"Failed to import {stat.filename}", style="default")
         text.append(f"\nException: {stat.exception}", style="red")
+        if 'body.parent.page_id should be defined' in str(stat.exception):
+            text.append(f"\nHeadmeta : \n{json.dumps(stat.head_meta, indent=4)}", style="yellow")
         console.print(text)
         return
     
     title = f"{stat.filename}" if stat.filename else "Import Result (Loss filename)"
     style = "default"
     if stat.get_level() == StatLevel.LOSS.value:
         title += " (Loss some content)"
@@ -90,16 +93,16 @@
 def prepare_env(args: argparse.Namespace):
     log_path = Path(args.log) if args.log else Path.cwd() / 'logs/'
     if not log_path.is_dir():
         log_path.mkdir(parents=True)
 
     conf_path = Path(args.conf)
     if not conf_path.is_file():
-        console.print(f"Read conf file({conf_path}) failed.", style="red")
-        logger.fatal(f"Read conf file({conf_path}) failed.")
+        text = Text(f"Read conf {conf_path} failed.", style="red")
+        console.print(text)
         sys.exit(1)
 
     setup_logger(log_path)
     read_config(conf_path)
     logger.info(f"Read log {log_path}, conf {conf_path}")
 
 
@@ -113,33 +116,36 @@
         async with AsyncClient(auth=notion_api_key) as notion_client:
             notion_importer = NotionImporter(session, notion_client)
             await notion_importer.process_file(file)
             return notion_importer.import_stats
 
 
 def main():
-    args = parse_args()
+    arg_parse = prepare_args()
+    args = arg_parse.parse_args()
     prepare_env(args)
 
+    text = Text("")
     file_path = Path(args.file) if args.file else None
     dir_path = Path(args.dir) if args.dir else None
     max_concurrency = args.batch
     if file_path and file_path.is_file():
         stats = asyncio.run(import_single_file(file_path))
         print_single_stats(stats)
     elif dir_path and dir_path.is_dir():
         logger.info(f"Begin save all html files in the dir: {dir_path}.")
         batch_import = BatchImport(dir_path, max_concurrency)
         result = asyncio.run(batch_import.process_directory())
         logger.info(f"Finish save all html files in the dir: {dir_path}.\n{result}")
         print_batch_stats(batch_import)
     else:
-        text = Text("The parameters provided are incorrect, please check.", style="red")
+        text.append("The parameters provided are incorrect, please check.", style="red")
+        text.append(f"\n{arg_parse.format_help()}", style="default")
 
-    text = Text("\nIf you need help, please submit an ", style="default")
+    text.append("\nIf you need help, please submit an ", style="default")
     link = Text("issue", style="cyan underline link https://github.com/selfboot/html2notion/issues")
     text.append(link)
     text.append(" on gitHub.", style="default")
     console.print(text)
     return
```

### Comparing `html2notion-0.1.9/html2notion/translate/batch_import.py` & `html2notion-0.2.0/html2notion/translate/batch_import.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.9/html2notion/translate/cos_uploader.py` & `html2notion-0.2.0/html2notion/translate/cos_uploader.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.9/html2notion/translate/html2json.py` & `html2notion-0.2.0/html2notion/translate/html2json.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,70 +13,82 @@
 
 
 """
 <meta name="source" content="yinxiang.superNote"/>
 <meta name="source" content="desktop.mac"/>
 <meta name="source" content="mobile.android"/>
 """
-def _is_yinxiang_export_html(html_soup):
+def _is_yinxiang_export_html(html_soup, import_stat):
     meta_source = html_soup.select_one('html > head > meta[name="source"]')
     meta_source_content = meta_source.get('content', "") if isinstance(meta_source, Tag) else ""
+    if not meta_source_content:
+        return False
     yinxiang_source_content = ["yinxiang", "desktop", "mobile"]
+    import_stat.head_meta["source"] = meta_source_content
     for prefix in yinxiang_source_content:
         if isinstance(meta_source_content, str) and meta_source_content.startswith(prefix):
             return True
     return False
 
 
 """
 <meta name="source-application" content="webclipper.evernote" />
 <meta name="source-application" content="微信" />
 """
-def _is_yinxiang_clipper_html(html_soup):
+def _is_yinxiang_clipper_html(html_soup, import_stat):
     meta_source_application = html_soup.select_one('html > head > meta[name="source-application"]')
     source_application = meta_source_application.get('content', "") if isinstance(meta_source_application, Tag) else ""
+    if not source_application:
+        return False
+    import_stat.head_meta["source-application"] = source_application
     if isinstance(source_application, str) and source_application.endswith("evernote"):
         return True
     if isinstance(source_application, str) and source_application in ["微信",]:
         return True
     return False
 
 
 """
 <meta name="content-class" content="yinxiang.markdown" />
 """
-def _is_yinxiang_markdown_html(html_soup):
+def _is_yinxiang_markdown_html(html_soup, import_stat):
     meta_content_class = html_soup.select_one('html > head > meta[name="content-class"]')
     content_class = meta_content_class.get('content', "") if isinstance(meta_content_class, Tag) else ""
+    if not content_class:
+        return False
+    import_stat.head_meta["content_class"] = content_class
     if isinstance(content_class, str) and content_class.endswith("markdown"):
         return True
     return False
 
 
-def _infer_input_type(html_content):
+# <meta name="exporter-version" content="YXBJ Windows/607246 (zh-CN, DDL); Windows/10.0.0 (Win64); EDAMVersion=V2;"/>
+# <meta name="exporter-version" content="Evernote Mac 9.6.8 (470886)"/>
+def _infer_input_type(html_content, import_stat):
     soup = BeautifulSoup(html_content, 'html.parser')
     exporter_version_meta = soup.select_one('html > head > meta[name="exporter-version"]')
-    exporter_version_content = exporter_version_meta.get(
-        'content', "") if isinstance(
-        exporter_version_meta, Tag) else ""
-
-    # yinxiang export
-    if isinstance(exporter_version_content, str) and exporter_version_content.startswith("Evernote"):
-        if _is_yinxiang_markdown_html(soup):
+    exporter_version_content = exporter_version_meta.get('content', "") if isinstance( exporter_version_meta, Tag) else ""
+    import_stat.head_meta["exporter-version"] = exporter_version_content
+    exporter_version = exporter_version_content if isinstance(exporter_version_content, str) else ""
+    if exporter_version.startswith("Evernote") or exporter_version.startswith("YXBJ"):
+        if _is_yinxiang_markdown_html(soup, import_stat):
             return YinXiangMarkdown_Type
-        if _is_yinxiang_clipper_html(soup):
+        if _is_yinxiang_clipper_html(soup, import_stat):
             return YinXiangClipper_Type
-        elif _is_yinxiang_export_html(soup):
+        elif _is_yinxiang_export_html(soup, import_stat):
             return YinXiang_Type
 
+        return YinXiang_Type # default
+    
     return Default_Type
 
 
 def _get_converter(html_content, import_stat):
-    html_type = _infer_input_type(html_content)
+    html_type = _infer_input_type(html_content, import_stat)
+    import_stat.head_meta["parse_type"] = html_type
     logger.info(f"Input type: {html_type}")
     converter = Html2JsonBase.create(html_type, html_content, import_stat)
     return converter
 
 
 @singledispatch
 def html2json_process(html_content, import_stat):
```

### Comparing `html2notion-0.1.9/html2notion/translate/html2json_base.py` & `html2notion-0.2.0/html2notion/translate/html2json_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 import re
 import os
+import copy
 from collections import namedtuple
 from bs4 import NavigableString, Tag, PageElement
 from enum import Enum
-from ..utils import logger, config
+from ..utils import logger, config, is_valid_url
 
 class Block(Enum):
     FAIL = "fail"
     PARAGRAPH = "paragraph"
     QUOTE = "quote"
     NUMBERED_LIST = "numbered_list_item"
     BULLETED_LIST = "bulleted_list_item"
     HEADING = "heading"
     CODE = "code"
     DIVIDER = "divider"
     TABLE = "table"
     TO_DO = "to_do"
     EQUATION = "equation"
 
+
 class Html2JsonBase:
+    # https://developers.notion.com/reference/request-limits
+    URL_MAX_LENGTH = 2000
+    TEXT_MAX_LENGTH = 2000
+    EXPRESSION_MAX_LENGTH = 1000
+    RICHTEXT_ARRAY_LENGTH = 100
+
     _registry = {}
     _text_annotations = {
         "bold": bool,
         "italic": bool,
         "strikethrough": bool,
         "underline": bool,
         "code": bool,
@@ -80,29 +88,34 @@
             }.items()
             if value
         }
 
     @staticmethod
     def extract_text_and_parents(tag: PageElement, parents=[]):
         results = []
-        # Filter empty content
-        if isinstance(tag, NavigableString) and tag.text:
-            results.append((tag.text, parents))
+        # Filter empty content when tag is not img
+        if isinstance(tag, NavigableString) and tag.strip():
+            results.append((tag, parents))
             return results
         elif isinstance(tag, Tag):
-            for child in tag.children:
-                if isinstance(child, NavigableString):
-                    if child.strip():
-                        text = child.text
-                        parent_tags = [p for p in parents + [tag]]
-                        results.append((text, parent_tags))
-                elif isinstance(child, Tag) and child.name == 'br':  
-                    results.append(('<br>', []))
-                else:
-                    results.extend(Html2JsonBase.extract_text_and_parents(child, parents + [tag]))
+            if tag.name == 'img':
+                img_src = tag.get('src', '')
+                parent_tags = [p for p in parents + [tag]]
+                results.append((img_src, parent_tags))
+            else:
+                for child in tag.children:
+                    if isinstance(child, NavigableString):
+                        if tag.name != 'img' and child.strip():
+                            text = child.text
+                            parent_tags = [p for p in parents + [tag]]
+                            results.append((text, parent_tags))
+                    elif isinstance(child, Tag) and child.name == 'br':  
+                        results.append(('<br>', []))
+                    else:
+                        results.extend(Html2JsonBase.extract_text_and_parents(child, parents + [tag]))
         return results
 
     @staticmethod
     def parse_one_style(tag_soup: Tag, text_params: dict):
         tag_name = tag_soup.name.lower()
         styles = Html2JsonBase.get_tag_style(tag_soup)
         if Html2JsonBase.is_bold(tag_name, styles):
@@ -121,65 +134,98 @@
             text_params["color"] = color
 
         if tag_name == 'a':
             href = tag_soup.get('href', "")
             if not href:
                 logger.warning("Link href is empty")
             text_params["url"] = href
+        elif tag_name == 'img':
+            src = tag_soup.get('src', "")
+            # only support external image here.
+            if not src:
+                logger.warning("Image src is empty")
+            text_params["src"] = src
         return
 
     # https://developers.notion.com/reference/request-limits
     # Process one tag and return a list of objects
     # <b><u>unlineline and bold</u></b>
     # <div><font color="#ff2600">Red color4</font></div>
     # <div> Code in super note</div>
     def generate_inline_obj(self, tag: PageElement):
         res_obj = []
         text_with_parents = Html2JsonBase.extract_text_and_parents(tag)
         for (text, parent_tags) in text_with_parents:
-            # Split the text into chunks of 2000 characters
-            text_chunks = [text[i:i+2000] for i in range(0, len(text), 2000)]
-            for chunk in text_chunks:
-                text_params = {"plain_text": chunk}
-                for parent in parent_tags:
-                    Html2JsonBase.parse_one_style(parent, text_params)
-                # process inline line break
-                if chunk == "<br>":
-                    try:
-                        res_obj[-1]["text"]["content"] += "\n"
-                        res_obj[-1]["plain_text"] += "\n"
-                    except Exception as e:
-                        logger.error(f'{res_obj}, {str(e)}')
-                    continue
-
-                if text_params.get("url", ""):
-                    text_obj = self.generate_link(**text_params)
-                else:
+            text_params = {"plain_text": text}
+            for parent in parent_tags:
+                Html2JsonBase.parse_one_style(parent, text_params)
+            if text == "<br>":
+                try:
+                    res_obj[-1]["text"]["content"] += "\n"
+                    res_obj[-1]["plain_text"] += "\n"
+                except Exception as e:
+                    pass
+                continue
+
+            link_url = text_params.get("url", "")
+            text_obj = {}
+            if text_params.get("url", "") and is_valid_url(link_url):
+                text_obj = self.generate_link(**text_params)
+            # Here image is a independent block, split out in the outer layer
+            elif text_params.get("src", ""):
+                text_obj = self.generate_image(**text_params)
+            else:
+                if len(text) <= self.TEXT_MAX_LENGTH:
                     text_obj = self.generate_text(**text_params)
-                if text_obj:
-                    res_obj.append(text_obj)
+                else:
+                    for chunk in [text[i:i+self.TEXT_MAX_LENGTH] for i in range(0, len(text), self.TEXT_MAX_LENGTH)]:
+                        text_params["plain_text"] = chunk
+                        text_obj = self.generate_text(**text_params)
+                        if text_obj:
+                            res_obj.append(text_obj)
+                    text_obj = None
+            if text_obj:
+                res_obj.append(text_obj)
         return res_obj
 
-
     def generate_link(self, **kwargs):
+        link_url = kwargs.get("url", "")
         plain_text = kwargs.get("plain_text", "")
-        if not plain_text:
+        if not plain_text or not is_valid_url(link_url):
             return
-        
+
+        link_url = link_url[:self.URL_MAX_LENGTH]
         self.import_stat.add_notion_text(plain_text)
         return {
-            "href": kwargs.get("url", ""),
+            "href": link_url,
             "plain_text": plain_text,
             "text": {
-                "link": {"url": kwargs.get("url", "")},
+                "link": {"url": link_url},
                 "content": plain_text
             },
             "type": "text"
         }
 
+    def generate_image(self, **kwargs):
+        source = kwargs.get("src", "")
+        if not source or not is_valid_url(source):
+            return
+        self.import_stat.add_notion_image(source)
+        image_block = {
+            "object": "block",
+            "type": "image",
+            "image": {
+                "type": "external",
+                "external": {
+                    "url": source
+                }
+            }
+        }
+        return image_block
+
     def generate_text(self, **kwargs):
         plain_text = kwargs.get("plain_text", "")
         if not plain_text:
             return
         annotations = {
             key: value
             for key, value in kwargs.items()
@@ -217,14 +263,20 @@
         return properties_obj
 
     @staticmethod
     def is_same_annotations_text(text_one: dict, text_another: dict):
         if text_one["type"] != "text" or text_another["type"] != "text":
             return False
         attributes = ["annotations", "href"]
+
+        # When merging, be careful not to let the text length exceed the limit
+        total_size = len(text_one["text"]["content"]) + len(text_another["text"]["content"])
+        if total_size > Html2JsonBase.TEXT_MAX_LENGTH:
+            return False
+
         return all(text_one.get(attr) == text_another.get(attr) for attr in attributes)
 
     @staticmethod
     def merge_rich_text(rich_text: list):
         if not rich_text:
             return []
         merged_text = []
@@ -345,15 +397,18 @@
                 "rich_text": []
             }
         }
         rich_text = json_obj["paragraph"]["rich_text"]
         text_obj = self.generate_inline_obj(soup)
         if text_obj:
             rich_text.extend(text_obj)
-        return json_obj
+
+        # Split out image into a independent blocks
+        split_objs = Html2JsonBase.split_image_src(json_obj)
+        return Html2JsonBase.ensure_array_len(split_objs)
 
     def convert_divider(self, soup):
         return {
             "object": "block",
             "type": "divider",
             "divider": {}
         }
@@ -461,14 +516,41 @@
                 "has_column_header": has_header,
                 "table_width": table_width,
                 "children": table_rows,
             }
         }
         return table_obj
 
+    @staticmethod
+    def split_image_src(text_obj):
+        rich_text = text_obj["paragraph"]["rich_text"]
+        need_split = any(text.get("object") == "block" for text in rich_text)
+        if not need_split:
+            return [text_obj]
+        
+        split_obj = []
+        cur_obj = {
+            "object": "block",
+            "type": "paragraph",
+            "paragraph": {
+                "rich_text": []
+            }
+        }
+        for text in rich_text:
+            if text.get("object") == "block":
+                if len(cur_obj["paragraph"]["rich_text"]) > 0:
+                    split_obj.append(copy.deepcopy(cur_obj))
+                    cur_obj["paragraph"]["rich_text"].clear()
+                split_obj.append(text)
+                continue
+            cur_obj["paragraph"]["rich_text"].append(text)
+        if len(cur_obj["paragraph"]["rich_text"]) > 0:
+            split_obj.append(cur_obj)
+        return split_obj
+
     # Only if there is no ";" in the value of the attribute, you can use this method to get all attributes.
     # Can't use this way like: background-image: url('data:image/png;base64...') 
     @staticmethod
     def get_tag_style(tag_soup):
         styles = {}
         if not isinstance(tag_soup, Tag):
             return styles
@@ -484,14 +566,38 @@
 
     @staticmethod
     def get_valid_language(language):
         if language in Html2JsonBase._language:
             return language
         return "plain text"
     
+    @staticmethod
+    def ensure_array_len(blocks):
+        final_objs = []
+        for obj in blocks:
+            if "paragraph" not in obj or "rich_text" not in obj["paragraph"] or len(
+                    obj["paragraph"]["rich_text"]) <= Html2JsonBase.RICHTEXT_ARRAY_LENGTH:
+                final_objs.append(obj)
+                continue
+
+            # If the length of rich_text is greater than RICHTEXT_ARRAY_LENGTH, we split it
+            rich_text_arr = obj["paragraph"]["rich_text"]
+            rich_texts = [rich_text_arr[i:i+Html2JsonBase.RICHTEXT_ARRAY_LENGTH]
+                          for i in range(0, len(rich_text_arr), Html2JsonBase.RICHTEXT_ARRAY_LENGTH)]
+            for rich_text in rich_texts:
+                new_json_obj = {
+                    "object": "block",
+                    "type": "paragraph",
+                    "paragraph": {
+                        "rich_text": rich_text
+                    }
+                }
+                final_objs.append(new_json_obj)
+        return final_objs
+
     @classmethod
     def register(cls, input_type, subclass):
         cls._registry[input_type] = subclass
 
     @classmethod
     def create(cls, input_type, html_content, import_stat):
         subclass = cls._registry.get(input_type)
```

### Comparing `html2notion-0.1.9/html2notion/translate/html2json_clipper.py` & `html2notion-0.2.0/html2notion/translate/html2json_clipper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from bs4 import BeautifulSoup, NavigableString, Tag
-from ..utils import logger
+from ..utils import logger, DateStrToISO8601
 from ..translate.html2json_base import Html2JsonBase, Block
-from ..utils.timeutil import DateStrToISO8601
 
 YinXiangClipper_Type = "clipper.yinxiang"
 
 
 class Html2JsonClipper(Html2JsonBase):
     input_type = YinXiangClipper_Type
```

### Comparing `html2notion-0.1.9/html2notion/translate/html2json_default.py` & `html2notion-0.2.0/html2notion/translate/html2json_default.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.9/html2notion/translate/html2json_markdown.py` & `html2notion-0.2.0/html2notion/translate/html2json_markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 from bs4 import BeautifulSoup, Tag
 from urllib.parse import unquote
-from ..utils import logger
+from ..utils import logger, is_valid_url, DateStrToISO8601
 from ..translate.html2json_base import Html2JsonBase, Block
-from ..utils.timeutil import DateStrToISO8601
 
 YinXiangMarkdown_Type = "markdown.yinxiang"
 
 # Yinxiang markdown
 # https://list.yinxiang.com/markdown/eef42447-db3f-48ee-827b-1bb34c03eb83.php
 
 
@@ -36,14 +35,20 @@
         if isinstance(center_to_delete, Tag):
             center_to_delete.decompose()
 
         # Special handling contains blocks of code, 
         # because some chart blocks are converted into images and cannot be processed directly
         self._replace_pre_code(soup)
         self.import_stat.add_text(content_tags.get_text())
+        img_tags = content_tags.find_all('img')
+        for img in img_tags:
+            img_src = img.get('src', '')
+            if is_valid_url(img_src):
+                self.import_stat.add_image(img_src)
+
         self.convert_children(content_tags)  # Assesume only one body tag
 
         return YinXiangMarkdown_Type
 
     def convert_properties(self, soup):
         properties = {"title": "Unknown"}
         title_tag = soup.select_one('head > title')
@@ -152,15 +157,15 @@
         json_obj = {
             "object": "block",
             "type": "paragraph",
             "paragraph": {
                 "rich_text": []
             }
         }
-        expression = soup.get_text()
+        expression = soup.get_text()[:Html2JsonBase.EXPRESSION_MAX_LENGTH]
         equation = json_obj["paragraph"]["rich_text"]
         equation.append({
             "type": "equation",
             "equation": {
                 "expression": expression
             }
         })
```

### Comparing `html2notion-0.1.9/html2notion/translate/html2json_yinxiang.py` & `html2notion-0.2.0/html2notion/translate/html2json_yinxiang.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from bs4 import BeautifulSoup, Tag
-from ..utils import logger
-from ..translate.html2json_base import Html2JsonBase, Block
-from ..utils.timeutil import DateStrToISO8601
+from ..utils import logger, DateStrToISO8601
+from ..translate.html2json_base import Html2JsonBase, Block 
 
 YinXiang_Type = "yinxiang"
 
 
 class Html2JsonYinXiang(Html2JsonBase):
     input_type = YinXiang_Type
 
@@ -78,15 +77,14 @@
                 rich_text.extend(text_obj)
             if not is_last_child:
                 rich_text.append(self.generate_text(plain_text='\n', stats_count=False))
         json_obj["code"]["rich_text"] = self.merge_rich_text(rich_text)
         css_dict = Html2JsonBase.get_tag_style(soup)
         language = css_dict.get('--en-codeblockLanguage', 'plain text')
         json_obj["code"]["language"] = language
-        
         return json_obj
 
     def convert_quote(self, soup):
         json_obj = {
             "object": "block",
             "type": "quote",
             "quote": {
@@ -163,22 +161,20 @@
             return Block.CODE.value
 
         # Issue 5: <div style="orphans: 2; widows: 2">
         if tag_name == 'div':
             return Block.PARAGRAPH.value
         return Block.FAIL.value
 
+    # <div> <table> </table> </div>
     def _check_is_table(self, tag):
         if tag.name == "div":
             children = list(filter(lambda x: x != '\n', tag.contents))
             table_count = sum(1 for child in children if child.name == "table")
-            div_br_count = sum(1 for child in children if child.name == "div" and len(
-                child.contents) == 1 and child.contents[0].name == "br")
-
-            return table_count == 1 and div_br_count >= 2 and (table_count + div_br_count) == len(children)
+            return table_count >= 1
         return False
 
     def _check_is_todo(self, tag):
         if not isinstance(tag, Tag):
             return False
         input_tag = tag.find('input')
         if input_tag and isinstance(input_tag, Tag) and input_tag.get('type') == 'checkbox':
```

### Comparing `html2notion-0.1.9/html2notion/translate/import_stats.py` & `html2notion-0.2.0/html2notion/translate/import_stats.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,28 +15,33 @@
         self.notion_text_count = 0
         self.notion_image_count = 0
         self.skip_tag = []
         self.exception = None
         self.filename = "None"
         self.html_content = ""
         self.notion_content = ""
+        self.html_image_src = []
+        self.notion_image_src = []
+        self.head_meta = {}
 
     def add_text(self, text: str):
         self.text_count += len(text)
         self.html_content += text
 
     def add_notion_text(self, text: str):
         self.notion_content += text
         self.notion_text_count += len(text)
 
-    def add_image(self, count: int):
-        self.image_count += count
-
-    def add_notion_image(self, count: int):
-        self.notion_image_count += count
+    def add_image(self, src: str):
+        self.html_image_src.append(src)
+        self.image_count += 1
+
+    def add_notion_image(self, src: str):
+        self.notion_image_src.append(src)
+        self.notion_image_count += 1
 
     def add_skip_tag(self, tag):
         self.skip_tag.append(tag)
 
     def set_filename(self, filename: Path):
         self.filename = filename
 
@@ -47,17 +52,20 @@
         if self.exception:
             return StatLevel.EXCEPTION.value
         if self.notion_text_count < self.text_count:
             return StatLevel.LOSS.value
         return StatLevel.SUCC.value
 
     def __str__(self):
-        if self.get_level() == StatLevel.EXCEPTION.value:
-            return f"[red]{str(self.exception)}[/red]"
         msg = ""
+        if self.get_level() == StatLevel.EXCEPTION.value:
+            msg += f"[red]{str(self.exception)}[/red]"
+            if 'body.parent.page_id should be defined' in str(self.exception):
+                msg += f"\nHeadmeta: [yellow]{self.head_meta}[/yellow]"
+
         if self.get_level() == StatLevel.LOSS.value:
             if self.text_count != self.notion_text_count:
                 msg += f"Text Len {self.text_count} -> {self.notion_text_count}, Loss [yellow]{self.text_count-self.notion_text_count}[/yellow]"
 
             msg += '\nDetail: [yellow]' + ";".join([repr(s) for s in self.skip_tag])[:500] + "[/yellow]"
         return msg
```

### Comparing `html2notion-0.1.9/html2notion/translate/notion_export.py` & `html2notion-0.2.0/html2notion/translate/notion_export.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.9/html2notion/translate/notion_import.py` & `html2notion-0.2.0/html2notion/translate/notion_import.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.9/html2notion/utils/load_config.py` & `html2notion-0.2.0/html2notion/utils/load_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import sys
-from pathlib import Path
 from aiolimiter import AsyncLimiter
 rate_limit = AsyncLimiter(3, 1)
 config = {}
 
 
 def read_config(file_path):
     """
@@ -27,11 +26,8 @@
         raise Exception("notion is not set in config.json")
 
     notion_conf = config["notion"]
     if "database_id" not in notion_conf:
         raise Exception("database_id is not set in config.json")
     if "api_key" not in notion_conf:
         raise Exception("api_key is not set in config.json")
-
-    if "log_path" not in config:
-        config["log_path"] = Path('~/logs')
     return
```

### Comparing `html2notion-0.1.9/html2notion/utils/log.py` & `html2notion-0.2.0/html2notion/utils/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 class CustomFormatter(logging.Formatter):
     green = "\033[92m"
     normal = "\x1b[38;21m"
     yellow = "\x1b[33;21m"
     red = "\x1b[31;21m"
     bold_red = "\x1b[31;1m"
     reset = "\x1b[0m"
-    # type: ignore
-    format = "%(asctime)s - %(levelname)s - %(filename)s:%(lineno)d - %(message)s"
+    format = "%(asctime)s - %(levelname)s - %(filename)s:%(lineno)d - %(message)s" # type: ignore
 
     FORMATS = {
         logging.DEBUG: green + format + reset,  # type: ignore
         logging.INFO: normal + format + reset,  # type: ignore
         logging.WARNING: yellow + format + reset,  # type: ignore
         logging.ERROR: red + format + reset,  # type: ignore
         logging.CRITICAL: bold_red + format + reset  # type: ignore
```

### Comparing `html2notion-0.1.9/html2notion.egg-info/PKG-INFO` & `html2notion-0.2.0/html2notion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6874 6d6c  : 2.1.Name: html
 00000020: 326e 6f74 696f 6e0a 5665 7273 696f 6e3a  2notion.Version:
-00000030: 2030 2e31 2e39 0a53 756d 6d61 7279 3a20   0.1.9.Summary: 
+00000030: 2030 2e32 2e30 0a53 756d 6d61 7279 3a20   0.2.0.Summary: 
 00000040: 5468 6973 2074 6f6f 6c20 6361 6e20 6163  This tool can ac
 00000050: 6375 7261 7465 6c79 2063 6f6e 7665 7274  curately convert
 00000060: 2048 544d 4c20 746f 204e 6f74 696f 6e20   HTML to Notion 
 00000070: 6e6f 7465 7320 616e 6420 6973 2061 6c73  notes and is als
 00000080: 6f20 7573 6566 756c 2066 6f72 2065 7870  o useful for exp
 00000090: 6f72 7469 6e67 2045 7665 726e 6f74 6520  orting Evernote 
 000000a0: 6e6f 7465 7320 746f 204e 6f74 696f 6e2e  notes to Notion.
@@ -24,265 +24,295 @@
 00000170: 5420 4c69 6365 6e73 650a 436c 6173 7369  T License.Classi
 00000180: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
 00000190: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
 000001a0: 6570 656e 6465 6e74 0a44 6573 6372 6970  ependent.Descrip
 000001b0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
 000001c0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
 000001d0: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
-000001e0: 4943 454e 5345 0a0a 5be7 ae80 e4bd 93e4  ICENSE..[.......
-000001f0: b8ad e696 875d 2868 7474 7073 3a2f 2f67  .....](https://g
-00000200: 6974 6875 622e 636f 6d2f 7365 6c66 626f  ithub.com/selfbo
-00000210: 6f74 2f68 746d 6c32 6e6f 7469 6f6e 2f62  ot/html2notion/b
-00000220: 6c6f 622f 6d61 7374 6572 2f52 4541 444d  lob/master/READM
-00000230: 455f 7a68 2e6d 6429 0a0a 6874 6d6c 326e  E_zh.md)..html2n
-00000240: 6f74 696f 6e20 6973 2061 6e20 696e 6372  otion is an incr
-00000250: 6564 6962 6c79 2075 7365 6675 6c20 746f  edibly useful to
-00000260: 6f6c 2077 7269 7474 656e 2069 6e20 5079  ol written in Py
-00000270: 7468 6f6e 2c20 7768 6963 6820 616c 6c6f  thon, which allo
-00000280: 7773 2079 6f75 2074 6f20 696d 706f 7274  ws you to import
-00000290: 2063 6f6e 7465 6e74 2066 726f 6d20 4854   content from HT
-000002a0: 4d4c 2064 6f63 756d 656e 7473 2069 6e74  ML documents int
-000002b0: 6f20 4e6f 7469 6f6e 206e 6f74 6573 2c20  o Notion notes, 
-000002c0: 6d61 6b69 6e67 2069 7420 6d6f 7265 2063  making it more c
-000002d0: 6f6e 7665 6e69 656e 7420 666f 7220 796f  onvenient for yo
-000002e0: 7520 746f 206f 7267 616e 697a 6520 696e  u to organize in
-000002f0: 666f 726d 6174 696f 6e20 6f6e 2074 6865  formation on the
-00000300: 204e 6f74 696f 6e20 706c 6174 666f 726d   Notion platform
-00000310: 2e20 496e 2061 6464 6974 696f 6e2c 2068  . In addition, h
-00000320: 746d 6c32 6e6f 7469 6f6e 2068 6173 2062  tml2notion has b
-00000330: 6565 6e20 7370 6563 6966 6963 616c 6c79  een specifically
-00000340: 206f 7074 696d 697a 6564 2066 6f72 2074   optimized for t
-00000350: 6865 2063 6f6e 7465 6e74 206f 6620 4576  he content of Ev
-00000360: 6572 6e6f 7465 2c20 616e 6420 796f 7520  ernote, and you 
-00000370: 6361 6e20 616c 736f 2075 7365 2069 7420  can also use it 
-00000380: 746f 2069 6d70 6f72 7420 6e6f 7465 7320  to import notes 
-00000390: 6672 6f6d 2045 7665 726e 6f74 6520 696e  from Evernote in
-000003a0: 746f 204e 6f74 696f 6e2e 0a0a 6874 6d6c  to Notion...html
-000003b0: 326e 6f74 696f 6e20 6861 7320 706f 7765  2notion has powe
-000003c0: 7266 756c 2066 6561 7475 7265 7320 616e  rful features an
-000003d0: 6420 7375 7070 6f72 7473 2063 6f6e 7665  d supports conve
-000003e0: 7274 696e 6720 7661 7269 6f75 7320 7461  rting various ta
-000003f0: 6773 2069 6e20 4854 4d4c 2066 696c 6573  gs in HTML files
-00000400: 2069 6e74 6f20 636f 7272 6573 706f 6e64   into correspond
-00000410: 696e 6720 426c 6f63 6b73 2069 6e20 4e6f  ing Blocks in No
-00000420: 7469 6f6e 2c20 7375 6368 2061 7320 7269  tion, such as ri
-00000430: 6368 2074 6578 7420 626c 6f63 6b73 2c20  ch text blocks, 
-00000440: 6865 6164 696e 6773 2c20 696d 6167 6573  headings, images
-00000450: 2c20 636f 6465 2062 6c6f 636b 732c 2071  , code blocks, q
-00000460: 756f 7465 732c 206c 696e 6b73 2c20 6574  uotes, links, et
-00000470: 632e 2042 656c 6f77 2061 7265 2065 7861  c. Below are exa
-00000480: 6d70 6c65 7320 6f66 2063 6f6e 7665 7274  mples of convert
-00000490: 696e 6720 6e6f 7465 7320 6672 6f6d 2045  ing notes from E
-000004a0: 7665 726e 6f74 6520 696e 746f 204e 6f74  vernote into Not
-000004b0: 696f 6e20 7061 6765 732e 0a0a 215b 7969  ion pages...![yi
-000004c0: 6e78 6961 6e67 206e 6f74 696f 6e28 7369  nxiang notion(si
-000004d0: 6d70 6c65 2064 656d 6f73 295d 2868 7474  mple demos)](htt
-000004e0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-000004f0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
-00000500: 656c 6662 6f6f 742f 6874 6d6c 326e 6f74  elfboot/html2not
-00000510: 696f 6e2f 6d61 7374 6572 2f64 656d 6f73  ion/master/demos
-00000520: 2f79 696e 7869 616e 675f 6e6f 7469 6f6e  /yinxiang_notion
-00000530: 2e70 6e67 290a 0a21 5b79 696e 7869 616e  .png)..![yinxian
-00000540: 6720 6e6f 7469 6f6e 3228 7269 6368 2074  g notion2(rich t
-00000550: 6578 7429 5d28 6874 7470 733a 2f2f 7261  ext)](https://ra
-00000560: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000570: 656e 742e 636f 6d2f 7365 6c66 626f 6f74  ent.com/selfboot
-00000580: 2f68 746d 6c32 6e6f 7469 6f6e 2f6d 6173  /html2notion/mas
-00000590: 7465 722f 6465 6d6f 732f 7969 6e78 6961  ter/demos/yinxia
-000005a0: 6e67 5f6e 6f74 696f 6e32 2e70 6e67 290a  ng_notion2.png).
-000005b0: 0a23 2050 7265 7061 7265 0a0a 596f 7520  .# Prepare..You 
-000005c0: 6f6e 6c79 206e 6565 6420 3320 7374 6570  only need 3 step
-000005d0: 7320 746f 2075 7365 2068 746d 6c6e 6f74  s to use htmlnot
-000005e0: 696f 6e20 746f 2069 6d70 6f72 7420 4854  ion to import HT
-000005f0: 4d4c 2069 6e74 6f20 4e6f 7469 6f6e 2e0a  ML into Notion..
-00000600: 0a23 2320 4475 706c 6963 6174 6520 6461  .## Duplicate da
-00000610: 7461 6261 7365 0a0a 436c 6963 6b20 7468  tabase..Click th
-00000620: 6520 6c69 6e6b 205b 6e6f 7469 6f6e 2074  e link [notion t
-00000630: 656d 706c 6174 655d 2868 7474 7073 3a2f  emplate](https:/
-00000640: 2f73 656c 6662 6f6f 742e 6e6f 7469 6f6e  /selfboot.notion
-00000650: 2e73 6974 652f 7365 6c66 626f 6f74 2f31  .site/selfboot/1
-00000660: 3330 6262 3438 6336 6362 6434 6162 6262  30bb48c6cbd4abbb
-00000670: 6237 3133 6434 6438 3437 3234 3831 613f  b713d4d8472481a?
-00000680: 763d 6464 6461 3230 6433 6634 3662 3462  v=ddda20d3f46b4b
-00000690: 3434 6130 3535 6430 3637 3932 6331 3432  44a055d06792c142
-000006a0: 6630 292e 2041 7320 7368 6f77 6e20 696e  f0). As shown in
-000006b0: 2074 6865 2069 6d61 6765 2062 656c 6f77   the image below
-000006c0: 2c20 7573 6520 7468 6520 2244 7570 6c69  , use the "Dupli
-000006d0: 6361 7465 2220 6275 7474 6f6e 2074 6f20  cate" button to 
-000006e0: 636f 7079 2061 206e 6577 2064 6174 6162  copy a new datab
-000006f0: 6173 6520 746f 2079 6f75 7220 6f77 6e20  ase to your own 
-00000700: 4e6f 7469 6f6e 2077 6f72 6b73 7061 6365  Notion workspace
-00000710: 2e0a 0a21 5b6e 6f74 696f 6e20 7465 6d70  ...![notion temp
-00000720: 6c61 7465 5d28 6874 7470 733a 2f2f 7261  late](https://ra
-00000730: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000740: 656e 742e 636f 6d2f 7365 6c66 626f 6f74  ent.com/selfboot
-00000750: 2f68 746d 6c32 6e6f 7469 6f6e 2f6d 6173  /html2notion/mas
-00000760: 7465 722f 6465 6d6f 732f 6e6f 7469 6f6e  ter/demos/notion
-00000770: 5f74 656d 706c 6167 652e 706e 6729 0a0a  _templage.png)..
-00000780: 2323 2049 6e73 7461 6c6c 2068 746d 6c32  ## Install html2
-00000790: 6e6f 7469 6f6e 0a0a 5265 7175 6972 6573  notion..Requires
-000007a0: 2070 7974 686f 6e3e 3d33 2e38 2c20 696e   python>=3.8, in
-000007b0: 7374 616c 6c20 7468 6520 6874 6d6c 326e  stall the html2n
-000007c0: 6f74 696f 6e20 6c69 6272 6172 792e 2059  otion library. Y
-000007d0: 6f75 2063 616e 2075 7365 2074 6865 2070  ou can use the p
-000007e0: 6970 2063 6f6d 6d61 6e64 2074 6f20 696e  ip command to in
-000007f0: 7374 616c 6c20 6974 3a0a 0a60 6060 0a70  stall it:..```.p
-00000800: 6970 2069 6e73 7461 6c6c 2068 746d 6c32  ip install html2
-00000810: 6e6f 7469 6f6e 0a60 6060 0a0a 2323 2050  notion.```..## P
-00000820: 7265 7061 7265 204e 6f74 696f 6e20 436f  repare Notion Co
-00000830: 6e66 6967 7572 6174 696f 6e0a 0a57 6520  nfiguration..We 
-00000840: 6e65 6564 2074 6f20 7573 6520 7468 6520  need to use the 
-00000850: 604e 6f74 696f 6e20 4150 4920 6b65 7960  `Notion API key`
-00000860: 2061 6e64 2060 4461 7461 6261 7365 2049   and `Database I
-00000870: 4460 2074 6f20 6175 7468 6f72 697a 6520  D` to authorize 
-00000880: 6874 6d6c 326e 6f74 696f 6e20 746f 2061  html2notion to a
-00000890: 6363 6573 7320 7468 6520 4e6f 7469 6f6e  ccess the Notion
-000008a0: 2064 6174 6162 6173 652e 2050 6c65 6173   database. Pleas
-000008b0: 6520 666f 6c6c 6f77 2074 6865 7365 2073  e follow these s
-000008c0: 7465 7073 3a0a 0a31 2e20 4372 6561 7465  teps:..1. Create
-000008d0: 2061 6e20 696e 7465 6772 6174 696f 6e3b   an integration;
-000008e0: 0a32 2e20 5368 6172 6520 6120 6461 7461  .2. Share a data
-000008f0: 6261 7365 2077 6974 6820 796f 7572 2069  base with your i
-00000900: 6e74 6567 7261 7469 6f6e 3b0a 332e 2045  ntegration;.3. E
-00000910: 7870 6f72 7420 7468 6520 6461 7461 6261  xport the databa
-00000920: 7365 2049 443b 0a0a 5768 656e 2073 6861  se ID;..When sha
-00000930: 7269 6e67 2074 6865 2064 6174 6162 6173  ring the databas
-00000940: 6520 6865 7265 2c20 796f 7520 6e65 6564  e here, you need
-00000950: 2074 6f20 6368 6f6f 7365 2074 6865 2070   to choose the p
-00000960: 7265 7669 6f75 736c 7920 6475 706c 6963  reviously duplic
-00000970: 6174 6564 2064 6174 6162 6173 6520 6265  ated database be
-00000980: 6361 7573 6520 7468 6520 696d 706f 7274  cause the import
-00000990: 206f 7065 7261 7469 6f6e 2072 6571 7569   operation requi
-000009a0: 7265 7320 736f 6d65 2070 7265 7365 7420  res some preset 
-000009b0: 5b70 726f 7065 7274 6965 735d 2868 7474  [properties](htt
-000009c0: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
-000009d0: 6e6f 7469 6f6e 2e63 6f6d 2f72 6566 6572  notion.com/refer
-000009e0: 656e 6365 2f70 726f 7065 7274 792d 6f62  ence/property-ob
-000009f0: 6a65 6374 2920 696e 666f 726d 6174 696f  ject) informatio
-00000a00: 6e20 696e 2074 6869 7320 6461 7461 6261  n in this databa
-00000a10: 7365 2e0a 0a46 6f72 2073 7065 6369 6669  se...For specifi
-00000a20: 6320 6d65 7468 6f64 732c 2070 6c65 6173  c methods, pleas
-00000a30: 6520 7265 6665 7220 746f 2074 6865 204e  e refer to the N
-00000a40: 6f74 696f 6e20 6f66 6669 6369 616c 2064  otion official d
-00000a50: 6f63 756d 656e 7461 7469 6f6e 205b 6372  ocumentation [cr
-00000a60: 6561 7465 2061 6e20 696e 7465 6772 6174  eate an integrat
-00000a70: 696f 6e5d 2868 7474 7073 3a2f 2f64 6576  ion](https://dev
-00000a80: 656c 6f70 6572 732e 6e6f 7469 6f6e 2e63  elopers.notion.c
-00000a90: 6f6d 2f64 6f63 732f 6372 6561 7465 2d61  om/docs/create-a
-00000aa0: 2d6e 6f74 696f 6e2d 696e 7465 6772 6174  -notion-integrat
-00000ab0: 696f 6e29 2e0a 0a41 6674 6572 2074 6865  ion)...After the
-00000ac0: 2073 6574 7570 2069 7320 636f 6d70 6c65   setup is comple
-00000ad0: 7465 2c20 7772 6974 6520 796f 7572 2041  te, write your A
-00000ae0: 5049 204b 6579 2061 6e64 2064 6174 6162  PI Key and datab
-00000af0: 6173 6520 4944 2069 6e74 6f20 6120 636f  ase ID into a co
-00000b00: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-00000b10: 2063 6f6e 6669 672e 6a73 6f6e 2e0a 0a60   config.json...`
-00000b20: 6060 7368 656c 6c0a 7b0a 2020 2020 226e  ``shell.{.    "n
-00000b30: 6f74 696f 6e22 3a20 7b0a 2020 2020 2020  otion": {.      
-00000b40: 2020 2264 6174 6162 6173 655f 6964 223a    "database_id":
-00000b50: 2022 3c2a 2a2a 6465 6d6f 2a2a 2a3e 222c   "<***demo***>",
-00000b60: 0a20 2020 2020 2020 2022 6170 695f 6b65  .        "api_ke
-00000b70: 7922 3a20 223c 2a2a 2a64 656d 6f2a 2a2a  y": "<***demo***
-00000b80: 3e22 0a20 2020 207d 0a7d 0a60 6060 0a0a  >".    }.}.```..
-00000b90: 2320 5573 6167 650a 0a59 6f75 2063 616e  # Usage..You can
-00000ba0: 2075 7365 2060 6874 6d6c 326e 6f74 696f   use `html2notio
-00000bb0: 6e20 2d68 6020 746f 2076 6965 7720 6465  n -h` to view de
-00000bc0: 7461 696c 6564 2068 656c 7020 646f 6375  tailed help docu
-00000bd0: 6d65 6e74 6174 696f 6e2e 0a0a 6060 6073  mentation...```s
-00000be0: 6865 6c6c 0a75 7361 6765 3a20 6874 6d6c  hell.usage: html
-00000bf0: 326e 6f74 696f 6e20 5b2d 685d 202d 2d63  2notion [-h] --c
-00000c00: 6f6e 6620 434f 4e46 205b 2d2d 6c6f 6720  onf CONF [--log 
-00000c10: 4c4f 475d 205b 2d2d 6261 7463 6820 4241  LOG] [--batch BA
-00000c20: 5443 485d 2028 2d2d 6669 6c65 2046 494c  TCH] (--file FIL
-00000c30: 4520 7c20 2d2d 6469 7220 4449 5229 0a0a  E | --dir DIR)..
-00000c40: 4874 6d6c 326e 6f74 696f 6e3a 2053 6176  Html2notion: Sav
-00000c50: 6520 4854 4d4c 2074 6f20 796f 7572 204e  e HTML to your N
-00000c60: 6f74 696f 6e20 6e6f 7465 7320 7175 6963  otion notes quic
-00000c70: 6b6c 7920 616e 6420 6561 7369 6c79 2c20  kly and easily, 
-00000c80: 7768 696c 6520 6b65 6570 696e 6720 7468  while keeping th
-00000c90: 6520 6f72 6967 696e 616c 2066 6f72 6d61  e original forma
-00000ca0: 7420 6173 206d 7563 6820 6173 2070 6f73  t as much as pos
-00000cb0: 7369 626c 650a 0a6f 7074 696f 6e73 3a0a  sible..options:.
-00000cc0: 2020 2d68 2c20 2d2d 6865 6c70 2020 2020    -h, --help    
-00000cd0: 2073 686f 7720 7468 6973 2068 656c 7020   show this help 
-00000ce0: 6d65 7373 6167 6520 616e 6420 6578 6974  message and exit
-00000cf0: 0a20 202d 2d63 6f6e 6620 434f 4e46 2020  .  --conf CONF  
-00000d00: 2020 636f 6e66 2066 696c 6520 7061 7468    conf file path
-00000d10: 0a20 202d 2d6c 6f67 204c 4f47 2020 2020  .  --log LOG    
-00000d20: 2020 6c6f 6720 6469 7265 6374 2070 6174    log direct pat
-00000d30: 680a 2020 2d2d 6261 7463 6820 4241 5443  h.  --batch BATC
-00000d40: 4820 2062 6174 6368 2073 6176 6520 636f  H  batch save co
-00000d50: 6e63 7572 7265 6e74 206c 696d 6974 0a20  ncurrent limit. 
-00000d60: 202d 2d66 696c 6520 4649 4c45 2020 2020   --file FILE    
-00000d70: 5361 7665 2073 696e 676c 6520 6874 6d6c  Save single html
-00000d80: 2066 696c 6520 746f 206e 6f74 696f 6e0a   file to notion.
-00000d90: 2020 2d2d 6469 7220 4449 5220 2020 2020    --dir DIR     
-00000da0: 2053 6176 6520 616c 6c20 6874 6d6c 2066   Save all html f
-00000db0: 696c 6573 2069 6e20 7468 6520 6469 7220  iles in the dir 
-00000dc0: 746f 206e 6f74 696f 6e0a 6060 600a 0a46  to notion.```..F
-00000dd0: 6f72 2065 7861 6d70 6c65 2c20 6966 2079  or example, if y
-00000de0: 6f75 2077 616e 7420 746f 2069 6d70 6f72  ou want to impor
-00000df0: 7420 616c 6c20 6874 6d6c 2066 696c 6573  t all html files
-00000e00: 2069 6e20 7468 6520 602e 2f64 656d 6f73   in the `./demos
-00000e10: 6020 6469 7265 6374 6f72 7920 696e 746f  ` directory into
-00000e20: 204e 6f74 696f 6e2c 2079 6f75 2063 616e   Notion, you can
-00000e30: 2075 7365 2074 6865 2066 6f6c 6c6f 7769   use the followi
-00000e40: 6e67 2063 6f6d 6d61 6e64 3a0a 0a60 6060  ng command:..```
-00000e50: 7368 656c 6c0a 6874 6d6c 326e 6f74 696f  shell.html2notio
-00000e60: 6e20 2d2d 636f 6e66 2063 6f6e 6669 672e  n --conf config.
-00000e70: 6a73 6f6e 202d 2d64 6972 202e 2f64 656d  json --dir ./dem
-00000e80: 6f73 202d 2d6c 6f67 207e 2f6c 6f67 7320  os --log ~/logs 
-00000e90: 2d2d 6261 7463 6820 3130 0a60 6060 0a0a  --batch 10.```..
-00000ea0: 5468 6520 6162 6f76 6520 636f 6d6d 616e  The above comman
-00000eb0: 6420 7769 6c6c 2069 6d70 6f72 7420 616c  d will import al
-00000ec0: 6c20 6874 6d6c 2066 696c 6573 2069 6e20  l html files in 
-00000ed0: 7468 6520 602e 2f64 656d 6f73 6020 6469  the `./demos` di
-00000ee0: 7265 6374 6f72 7920 696e 746f 204e 6f74  rectory into Not
-00000ef0: 696f 6e2c 2077 6869 6c65 206f 7574 7075  ion, while outpu
-00000f00: 7474 696e 6720 6c6f 6773 2074 6f20 7468  tting logs to th
-00000f10: 6520 607e 2f6c 6f67 7360 2064 6972 6563  e `~/logs` direc
-00000f20: 746f 7279 2c20 7769 7468 2075 7020 746f  tory, with up to
-00000f30: 2031 3020 636f 6e63 7572 7265 6e74 2074   10 concurrent t
-00000f40: 6173 6b73 2e0a 0a23 204d 6f72 6520 696e  asks...# More in
-00000f50: 666f 726d 6174 696f 6e0a 0a59 6f75 2063  formation..You c
-00000f60: 616e 2066 696e 6420 6d6f 7265 2069 6e66  an find more inf
-00000f70: 6f72 6d61 7469 6f6e 2061 6e64 2065 7861  ormation and exa
-00000f80: 6d70 6c65 7320 696e 2074 6865 2068 746d  mples in the htm
-00000f90: 6c32 6e6f 7469 6f6e 206c 6962 7261 7279  l2notion library
-00000fa0: 2773 2049 7373 7565 3a20 5b68 746d 6c32  's Issue: [html2
-00000fb0: 6e6f 7469 6f6e 5d28 6874 7470 733a 2f2f  notion](https://
-00000fc0: 6769 7468 7562 2e63 6f6d 2f73 656c 6662  github.com/selfb
-00000fd0: 6f6f 742f 6874 6d6c 326e 6f74 696f 6e2f  oot/html2notion/
-00000fe0: 6973 7375 6573 290a 0a23 2320 436f 6e74  issues)..## Cont
-00000ff0: 7269 6275 7469 6f6e 0a0a 4966 2079 6f75  ribution..If you
-00001000: 2066 696e 6420 616e 7920 6572 726f 7273   find any errors
-00001010: 206f 7220 6861 7665 2061 6e79 2073 7567   or have any sug
-00001020: 6765 7374 696f 6e73 2066 6f72 2069 6d70  gestions for imp
-00001030: 726f 7665 6d65 6e74 2c20 706c 6561 7365  rovement, please
-00001040: 2064 6f20 6e6f 7420 6865 7369 7461 7465   do not hesitate
-00001050: 2074 6f20 7375 626d 6974 2061 2070 756c   to submit a pul
-00001060: 6c20 7265 7175 6573 7420 6f72 2072 6169  l request or rai
-00001070: 7365 2061 6e20 6973 7375 652c 2049 2061  se an issue, I a
-00001080: 6d20 6d6f 7265 2074 6861 6e20 6861 7070  m more than happ
-00001090: 7920 746f 2061 6363 6570 7420 796f 7572  y to accept your
-000010a0: 2063 6f6e 7472 6962 7574 696f 6e73 2061   contributions a
-000010b0: 6e64 2066 6565 6462 6163 6b21 0a0a 4966  nd feedback!..If
-000010c0: 2079 6f75 2065 6e63 6f75 6e74 6572 2069   you encounter i
-000010d0: 6d70 6f72 7420 6661 696c 7572 6573 2c20  mport failures, 
-000010e0: 796f 7520 6361 6e20 7375 626d 6974 2074  you can submit t
-000010f0: 6865 2068 746d 6c20 6669 6c65 2061 6e64  he html file and
-00001100: 206c 6f67 2066 696c 6520 746f 6765 7468   log file togeth
-00001110: 6572 2069 6e20 7468 6520 6973 7375 6520  er in the issue 
-00001120: 666f 7220 6561 7369 6572 2070 726f 626c  for easier probl
-00001130: 656d 2069 6465 6e74 6966 6963 6174 696f  em identificatio
-00001140: 6e2e 0a0a 3e20 4966 2074 6865 7265 2061  n...> If there a
-00001150: 7265 2061 6e79 2070 7269 7661 7465 2069  re any private i
-00001160: 6e66 6f72 6d61 7469 6f6e 2069 6e20 7468  nformation in th
-00001170: 6520 6669 6c65 732c 2070 6c65 6173 6520  e files, please 
-00001180: 7265 6d6f 7665 2069 7420 6669 7273 742e  remove it first.
-00001190: 0a0a 0a23 2320 4c69 6365 6e73 650a 0a54  ...## License..T
-000011a0: 6869 7320 7072 6f6a 6563 7420 7573 6573  his project uses
-000011b0: 2074 6865 204d 4954 206c 6963 656e 7365   the MIT license
-000011c0: 2e20 506c 6561 7365 2072 6566 6572 2074  . Please refer t
-000011d0: 6f20 7468 6520 5b4c 4943 454e 5345 5d28  o the [LICENSE](
-000011e0: 2e2f 4c49 4345 4e53 4529 2066 6f72 2064  ./LICENSE) for d
-000011f0: 6574 6169 6c73 2e0a                      etails..
+000001e0: 4943 454e 5345 0a0a 3c68 3120 616c 6967  ICENSE..<h1 alig
+000001f0: 6e3d 2263 656e 7465 7222 3e48 746d 6c32  n="center">Html2
+00000200: 6e6f 7469 6f6e 203c 6120 6872 6566 3d27  notion <a href='
+00000210: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000220: 6f6d 2f73 656c 6662 6f6f 742f 6874 6d6c  om/selfboot/html
+00000230: 326e 6f74 696f 6e2f 626c 6f62 2f6d 6173  2notion/blob/mas
+00000240: 7465 722f 5245 4144 4d45 5f7a 682e 6d64  ter/README_zh.md
+00000250: 273e e7ae 80e4 bd93 e4b8 ade6 9687 3c2f  '>............</
+00000260: 613e 3c2f 6831 3e0a 3c70 2061 6c69 676e  a></h1>.<p align
+00000270: 3d22 6365 6e74 6572 223e 0a20 203c 6120  ="center">.  <a 
+00000280: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000290: 7468 7562 2e63 6f6d 2f73 656c 6662 6f6f  thub.com/selfboo
+000002a0: 742f 6874 6d6c 326e 6f74 696f 6e2f 6163  t/html2notion/ac
+000002b0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+000002c0: 7079 7468 6f6e 2d70 6163 6b61 6765 2e79  python-package.y
+000002d0: 6d6c 223e 0a20 2020 203c 696d 6720 7372  ml">.    <img sr
+000002e0: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+000002f0: 622e 636f 6d2f 7365 6c66 626f 6f74 2f68  b.com/selfboot/h
+00000300: 746d 6c32 6e6f 7469 6f6e 2f61 6374 696f  tml2notion/actio
+00000310: 6e73 2f77 6f72 6b66 6c6f 7773 2f70 7974  ns/workflows/pyt
+00000320: 686f 6e2d 7061 636b 6167 652e 796d 6c2f  hon-package.yml/
+00000330: 6261 6467 652e 7376 6722 2061 6c74 3d22  badge.svg" alt="
+00000340: 4349 2054 6573 7420 5374 6174 7573 223e  CI Test Status">
+00000350: 0a20 203c 2f61 3e0a 203c 6120 6872 6566  .  </a>. <a href
+00000360: 3d22 6874 7470 733a 2f2f 636f 6465 636f  ="https://codeco
+00000370: 762e 696f 2f67 682f 7365 6c66 626f 6f74  v.io/gh/selfboot
+00000380: 2f68 746d 6c32 6e6f 7469 6f6e 2220 3e0a  /html2notion" >.
+00000390: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+000003a0: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+000003b0: 2f73 656c 6662 6f6f 742f 6874 6d6c 326e  /selfboot/html2n
+000003c0: 6f74 696f 6e2f 6272 616e 6368 2f6d 6173  otion/branch/mas
+000003d0: 7465 722f 6772 6170 682f 6261 6467 652e  ter/graph/badge.
+000003e0: 7376 673f 746f 6b65 6e3d 5349 4d36 4937  svg?token=SIM6I7
+000003f0: 425a 5536 2220 616c 743d 2254 6573 7420  BZU6" alt="Test 
+00000400: 636f 7665 7261 6765 222f 3e0a 203c 2f61  coverage"/>. </a
+00000410: 3e0a 3c2f 703e 0a0a 6874 6d6c 326e 6f74  >.</p>..html2not
+00000420: 696f 6e20 6973 2061 6e20 696e 6372 6564  ion is an incred
+00000430: 6962 6c79 2075 7365 6675 6c20 746f 6f6c  ibly useful tool
+00000440: 2077 7269 7474 656e 2069 6e20 5079 7468   written in Pyth
+00000450: 6f6e 2c20 7768 6963 6820 616c 6c6f 7773  on, which allows
+00000460: 2079 6f75 2074 6f20 696d 706f 7274 2063   you to import c
+00000470: 6f6e 7465 6e74 2066 726f 6d20 4854 4d4c  ontent from HTML
+00000480: 2064 6f63 756d 656e 7473 2069 6e74 6f20   documents into 
+00000490: 4e6f 7469 6f6e 206e 6f74 6573 2c20 6d61  Notion notes, ma
+000004a0: 6b69 6e67 2069 7420 6d6f 7265 2063 6f6e  king it more con
+000004b0: 7665 6e69 656e 7420 666f 7220 796f 7520  venient for you 
+000004c0: 746f 206f 7267 616e 697a 6520 696e 666f  to organize info
+000004d0: 726d 6174 696f 6e20 6f6e 2074 6865 204e  rmation on the N
+000004e0: 6f74 696f 6e20 706c 6174 666f 726d 2e20  otion platform. 
+000004f0: 496e 2061 6464 6974 696f 6e2c 2068 746d  In addition, htm
+00000500: 6c32 6e6f 7469 6f6e 2068 6173 2062 6565  l2notion has bee
+00000510: 6e20 7370 6563 6966 6963 616c 6c79 206f  n specifically o
+00000520: 7074 696d 697a 6564 2066 6f72 2074 6865  ptimized for the
+00000530: 2063 6f6e 7465 6e74 206f 6620 4576 6572   content of Ever
+00000540: 6e6f 7465 2c20 616e 6420 796f 7520 6361  note, and you ca
+00000550: 6e20 616c 736f 2075 7365 2069 7420 746f  n also use it to
+00000560: 2069 6d70 6f72 7420 6e6f 7465 7320 6672   import notes fr
+00000570: 6f6d 2045 7665 726e 6f74 6520 696e 746f  om Evernote into
+00000580: 204e 6f74 696f 6e2e 0a0a 6874 6d6c 326e   Notion...html2n
+00000590: 6f74 696f 6e20 6861 7320 706f 7765 7266  otion has powerf
+000005a0: 756c 2066 6561 7475 7265 7320 616e 6420  ul features and 
+000005b0: 7375 7070 6f72 7473 2063 6f6e 7665 7274  supports convert
+000005c0: 696e 6720 7661 7269 6f75 7320 7461 6773  ing various tags
+000005d0: 2069 6e20 4854 4d4c 2066 696c 6573 2069   in HTML files i
+000005e0: 6e74 6f20 636f 7272 6573 706f 6e64 696e  nto correspondin
+000005f0: 6720 426c 6f63 6b73 2069 6e20 4e6f 7469  g Blocks in Noti
+00000600: 6f6e 2c20 7375 6368 2061 7320 7269 6368  on, such as rich
+00000610: 2074 6578 7420 626c 6f63 6b73 2c20 6865   text blocks, he
+00000620: 6164 696e 6773 2c20 696d 6167 6573 2c20  adings, images, 
+00000630: 636f 6465 2062 6c6f 636b 732c 2071 756f  code blocks, quo
+00000640: 7465 732c 206c 696e 6b73 2c20 6574 632e  tes, links, etc.
+00000650: 2042 656c 6f77 2061 7265 2065 7861 6d70   Below are examp
+00000660: 6c65 7320 6f66 2063 6f6e 7665 7274 696e  les of convertin
+00000670: 6720 6e6f 7465 7320 6672 6f6d 2045 7665  g notes from Eve
+00000680: 726e 6f74 6520 696e 746f 204e 6f74 696f  rnote into Notio
+00000690: 6e20 7061 6765 732e 0a0a 215b 7969 6e78  n pages...![yinx
+000006a0: 6961 6e67 206e 6f74 696f 6e28 7369 6d70  iang notion(simp
+000006b0: 6c65 2064 656d 6f73 295d 2868 7474 7073  le demos)](https
+000006c0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+000006d0: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 656c  rcontent.com/sel
+000006e0: 6662 6f6f 742f 6874 6d6c 326e 6f74 696f  fboot/html2notio
+000006f0: 6e2f 6d61 7374 6572 2f64 656d 6f73 2f79  n/master/demos/y
+00000700: 696e 7869 616e 675f 6e6f 7469 6f6e 2e70  inxiang_notion.p
+00000710: 6e67 290a 0a21 5b79 696e 7869 616e 6720  ng)..![yinxiang 
+00000720: 6e6f 7469 6f6e 3228 7269 6368 2074 6578  notion2(rich tex
+00000730: 7429 5d28 6874 7470 733a 2f2f 7261 772e  t)](https://raw.
+00000740: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000750: 742e 636f 6d2f 7365 6c66 626f 6f74 2f68  t.com/selfboot/h
+00000760: 746d 6c32 6e6f 7469 6f6e 2f6d 6173 7465  tml2notion/maste
+00000770: 722f 6465 6d6f 732f 7969 6e78 6961 6e67  r/demos/yinxiang
+00000780: 5f6e 6f74 696f 6e32 2e70 6e67 290a 0a23  _notion2.png)..#
+00000790: 2050 7265 7061 7265 0a0a 596f 7520 6f6e   Prepare..You on
+000007a0: 6c79 206e 6565 6420 3320 7374 6570 7320  ly need 3 steps 
+000007b0: 746f 2075 7365 2068 746d 6c6e 6f74 696f  to use htmlnotio
+000007c0: 6e20 746f 2069 6d70 6f72 7420 4854 4d4c  n to import HTML
+000007d0: 2069 6e74 6f20 4e6f 7469 6f6e 2e0a 0a23   into Notion...#
+000007e0: 2320 4475 706c 6963 6174 6520 6461 7461  # Duplicate data
+000007f0: 6261 7365 0a0a 436c 6963 6b20 7468 6520  base..Click the 
+00000800: 6c69 6e6b 205b 6e6f 7469 6f6e 2074 656d  link [notion tem
+00000810: 706c 6174 655d 2868 7474 7073 3a2f 2f73  plate](https://s
+00000820: 656c 6662 6f6f 742e 6e6f 7469 6f6e 2e73  elfboot.notion.s
+00000830: 6974 652f 7365 6c66 626f 6f74 2f31 3330  ite/selfboot/130
+00000840: 6262 3438 6336 6362 6434 6162 6262 6237  bb48c6cbd4abbbb7
+00000850: 3133 6434 6438 3437 3234 3831 613f 763d  13d4d8472481a?v=
+00000860: 6464 6461 3230 6433 6634 3662 3462 3434  ddda20d3f46b4b44
+00000870: 6130 3535 6430 3637 3932 6331 3432 6630  a055d06792c142f0
+00000880: 292e 2041 7320 7368 6f77 6e20 696e 2074  ). As shown in t
+00000890: 6865 2069 6d61 6765 2062 656c 6f77 2c20  he image below, 
+000008a0: 7573 6520 7468 6520 2244 7570 6c69 6361  use the "Duplica
+000008b0: 7465 2220 6275 7474 6f6e 2074 6f20 636f  te" button to co
+000008c0: 7079 2061 206e 6577 2064 6174 6162 6173  py a new databas
+000008d0: 6520 746f 2079 6f75 7220 6f77 6e20 4e6f  e to your own No
+000008e0: 7469 6f6e 2077 6f72 6b73 7061 6365 2e0a  tion workspace..
+000008f0: 0a21 5b6e 6f74 696f 6e20 7465 6d70 6c61  .![notion templa
+00000900: 7465 5d28 6874 7470 733a 2f2f 7261 772e  te](https://raw.
+00000910: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000920: 742e 636f 6d2f 7365 6c66 626f 6f74 2f68  t.com/selfboot/h
+00000930: 746d 6c32 6e6f 7469 6f6e 2f6d 6173 7465  tml2notion/maste
+00000940: 722f 6465 6d6f 732f 6e6f 7469 6f6e 5f74  r/demos/notion_t
+00000950: 656d 706c 6167 652e 706e 6729 0a0a 2323  emplage.png)..##
+00000960: 2049 6e73 7461 6c6c 2068 746d 6c32 6e6f   Install html2no
+00000970: 7469 6f6e 0a0a 5265 7175 6972 6573 2070  tion..Requires p
+00000980: 7974 686f 6e3e 3d33 2e38 2c20 696e 7374  ython>=3.8, inst
+00000990: 616c 6c20 7468 6520 6874 6d6c 326e 6f74  all the html2not
+000009a0: 696f 6e20 6c69 6272 6172 792e 2059 6f75  ion library. You
+000009b0: 2063 616e 2075 7365 2074 6865 2070 6970   can use the pip
+000009c0: 2063 6f6d 6d61 6e64 2074 6f20 696e 7374   command to inst
+000009d0: 616c 6c20 6974 3a0a 0a60 6060 0a70 6970  all it:..```.pip
+000009e0: 2069 6e73 7461 6c6c 2068 746d 6c32 6e6f   install html2no
+000009f0: 7469 6f6e 0a60 6060 0a0a 2323 2050 7265  tion.```..## Pre
+00000a00: 7061 7265 204e 6f74 696f 6e20 436f 6e66  pare Notion Conf
+00000a10: 6967 7572 6174 696f 6e0a 0a57 6520 6e65  iguration..We ne
+00000a20: 6564 2074 6f20 7573 6520 7468 6520 604e  ed to use the `N
+00000a30: 6f74 696f 6e20 4150 4920 6b65 7960 2061  otion API key` a
+00000a40: 6e64 2060 4461 7461 6261 7365 2049 4460  nd `Database ID`
+00000a50: 2074 6f20 6175 7468 6f72 697a 6520 6874   to authorize ht
+00000a60: 6d6c 326e 6f74 696f 6e20 746f 2061 6363  ml2notion to acc
+00000a70: 6573 7320 7468 6520 4e6f 7469 6f6e 2064  ess the Notion d
+00000a80: 6174 6162 6173 652e 2050 6c65 6173 6520  atabase. Please 
+00000a90: 666f 6c6c 6f77 2074 6865 7365 2073 7465  follow these ste
+00000aa0: 7073 3a0a 0a31 2e20 4372 6561 7465 2061  ps:..1. Create a
+00000ab0: 6e20 696e 7465 6772 6174 696f 6e3b 0a32  n integration;.2
+00000ac0: 2e20 5368 6172 6520 6120 6461 7461 6261  . Share a databa
+00000ad0: 7365 2077 6974 6820 796f 7572 2069 6e74  se with your int
+00000ae0: 6567 7261 7469 6f6e 3b0a 332e 2045 7870  egration;.3. Exp
+00000af0: 6f72 7420 7468 6520 6461 7461 6261 7365  ort the database
+00000b00: 2049 443b 0a0a 5768 656e 2073 6861 7269   ID;..When shari
+00000b10: 6e67 2074 6865 2064 6174 6162 6173 6520  ng the database 
+00000b20: 6865 7265 2c20 796f 7520 6e65 6564 2074  here, you need t
+00000b30: 6f20 6368 6f6f 7365 2074 6865 2070 7265  o choose the pre
+00000b40: 7669 6f75 736c 7920 6475 706c 6963 6174  viously duplicat
+00000b50: 6564 2064 6174 6162 6173 6520 6265 6361  ed database beca
+00000b60: 7573 6520 7468 6520 696d 706f 7274 206f  use the import o
+00000b70: 7065 7261 7469 6f6e 2072 6571 7569 7265  peration require
+00000b80: 7320 736f 6d65 2070 7265 7365 7420 5b70  s some preset [p
+00000b90: 726f 7065 7274 6965 735d 2868 7474 7073  roperties](https
+00000ba0: 3a2f 2f64 6576 656c 6f70 6572 732e 6e6f  ://developers.no
+00000bb0: 7469 6f6e 2e63 6f6d 2f72 6566 6572 656e  tion.com/referen
+00000bc0: 6365 2f70 726f 7065 7274 792d 6f62 6a65  ce/property-obje
+00000bd0: 6374 2920 696e 666f 726d 6174 696f 6e20  ct) information 
+00000be0: 696e 2074 6869 7320 6461 7461 6261 7365  in this database
+00000bf0: 2e0a 0a46 6f72 2073 7065 6369 6669 6320  ...For specific 
+00000c00: 6d65 7468 6f64 732c 2070 6c65 6173 6520  methods, please 
+00000c10: 7265 6665 7220 746f 2074 6865 204e 6f74  refer to the Not
+00000c20: 696f 6e20 6f66 6669 6369 616c 2064 6f63  ion official doc
+00000c30: 756d 656e 7461 7469 6f6e 205b 6372 6561  umentation [crea
+00000c40: 7465 2061 6e20 696e 7465 6772 6174 696f  te an integratio
+00000c50: 6e5d 2868 7474 7073 3a2f 2f64 6576 656c  n](https://devel
+00000c60: 6f70 6572 732e 6e6f 7469 6f6e 2e63 6f6d  opers.notion.com
+00000c70: 2f64 6f63 732f 6372 6561 7465 2d61 2d6e  /docs/create-a-n
+00000c80: 6f74 696f 6e2d 696e 7465 6772 6174 696f  otion-integratio
+00000c90: 6e29 2e0a 0a41 6674 6572 2074 6865 2073  n)...After the s
+00000ca0: 6574 7570 2069 7320 636f 6d70 6c65 7465  etup is complete
+00000cb0: 2c20 7772 6974 6520 796f 7572 2041 5049  , write your API
+00000cc0: 204b 6579 2061 6e64 2064 6174 6162 6173   Key and databas
+00000cd0: 6520 4944 2069 6e74 6f20 6120 636f 6e66  e ID into a conf
+00000ce0: 6967 7572 6174 696f 6e20 6669 6c65 2063  iguration file c
+00000cf0: 6f6e 6669 672e 6a73 6f6e 2e0a 0a60 6060  onfig.json...```
+00000d00: 7368 656c 6c0a 7b0a 2020 2020 226e 6f74  shell.{.    "not
+00000d10: 696f 6e22 3a20 7b0a 2020 2020 2020 2020  ion": {.        
+00000d20: 2264 6174 6162 6173 655f 6964 223a 2022  "database_id": "
+00000d30: 3c2a 2a2a 6465 6d6f 2a2a 2a3e 222c 0a20  <***demo***>",. 
+00000d40: 2020 2020 2020 2022 6170 695f 6b65 7922         "api_key"
+00000d50: 3a20 223c 2a2a 2a64 656d 6f2a 2a2a 3e22  : "<***demo***>"
+00000d60: 0a20 2020 207d 0a7d 0a60 6060 0a0a 2320  .    }.}.```..# 
+00000d70: 5573 6167 650a 0a59 6f75 2063 616e 2075  Usage..You can u
+00000d80: 7365 2060 6874 6d6c 326e 6f74 696f 6e20  se `html2notion 
+00000d90: 2d68 6020 746f 2076 6965 7720 6465 7461  -h` to view deta
+00000da0: 696c 6564 2068 656c 7020 646f 6375 6d65  iled help docume
+00000db0: 6e74 6174 696f 6e2e 0a0a 6060 6073 6865  ntation...```she
+00000dc0: 6c6c 0a75 7361 6765 3a20 6874 6d6c 326e  ll.usage: html2n
+00000dd0: 6f74 696f 6e20 5b2d 685d 202d 2d63 6f6e  otion [-h] --con
+00000de0: 6620 434f 4e46 205b 2d2d 6c6f 6720 4c4f  f CONF [--log LO
+00000df0: 475d 205b 2d2d 6261 7463 6820 4241 5443  G] [--batch BATC
+00000e00: 485d 2028 2d2d 6669 6c65 2046 494c 4520  H] (--file FILE 
+00000e10: 7c20 2d2d 6469 7220 4449 5229 0a0a 4874  | --dir DIR)..Ht
+00000e20: 6d6c 326e 6f74 696f 6e3a 2053 6176 6520  ml2notion: Save 
+00000e30: 4854 4d4c 2074 6f20 796f 7572 204e 6f74  HTML to your Not
+00000e40: 696f 6e20 6e6f 7465 7320 7175 6963 6b6c  ion notes quickl
+00000e50: 7920 616e 6420 6561 7369 6c79 2c20 7768  y and easily, wh
+00000e60: 696c 6520 6b65 6570 696e 6720 7468 6520  ile keeping the 
+00000e70: 6f72 6967 696e 616c 2066 6f72 6d61 7420  original format 
+00000e80: 6173 206d 7563 6820 6173 2070 6f73 7369  as much as possi
+00000e90: 626c 650a 0a6f 7074 696f 6e73 3a0a 2020  ble..options:.  
+00000ea0: 2d68 2c20 2d2d 6865 6c70 2020 2020 2073  -h, --help     s
+00000eb0: 686f 7720 7468 6973 2068 656c 7020 6d65  how this help me
+00000ec0: 7373 6167 6520 616e 6420 6578 6974 0a20  ssage and exit. 
+00000ed0: 202d 2d63 6f6e 6620 434f 4e46 2020 2020   --conf CONF    
+00000ee0: 636f 6e66 2066 696c 6520 7061 7468 0a20  conf file path. 
+00000ef0: 202d 2d6c 6f67 204c 4f47 2020 2020 2020   --log LOG      
+00000f00: 6c6f 6720 6469 7265 6374 2070 6174 680a  log direct path.
+00000f10: 2020 2d2d 6261 7463 6820 4241 5443 4820    --batch BATCH 
+00000f20: 2062 6174 6368 2073 6176 6520 636f 6e63   batch save conc
+00000f30: 7572 7265 6e74 206c 696d 6974 0a20 202d  urrent limit.  -
+00000f40: 2d66 696c 6520 4649 4c45 2020 2020 5361  -file FILE    Sa
+00000f50: 7665 2073 696e 676c 6520 6874 6d6c 2066  ve single html f
+00000f60: 696c 6520 746f 206e 6f74 696f 6e0a 2020  ile to notion.  
+00000f70: 2d2d 6469 7220 4449 5220 2020 2020 2053  --dir DIR      S
+00000f80: 6176 6520 616c 6c20 6874 6d6c 2066 696c  ave all html fil
+00000f90: 6573 2069 6e20 7468 6520 6469 7220 746f  es in the dir to
+00000fa0: 206e 6f74 696f 6e0a 6060 600a 0a46 6f72   notion.```..For
+00000fb0: 2065 7861 6d70 6c65 2c20 6966 2079 6f75   example, if you
+00000fc0: 2077 616e 7420 746f 2069 6d70 6f72 7420   want to import 
+00000fd0: 616c 6c20 6874 6d6c 2066 696c 6573 2069  all html files i
+00000fe0: 6e20 7468 6520 602e 2f64 656d 6f73 6020  n the `./demos` 
+00000ff0: 6469 7265 6374 6f72 7920 696e 746f 204e  directory into N
+00001000: 6f74 696f 6e2c 2079 6f75 2063 616e 2075  otion, you can u
+00001010: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
+00001020: 2063 6f6d 6d61 6e64 3a0a 0a60 6060 7368   command:..```sh
+00001030: 656c 6c0a 6874 6d6c 326e 6f74 696f 6e20  ell.html2notion 
+00001040: 2d2d 636f 6e66 2063 6f6e 6669 672e 6a73  --conf config.js
+00001050: 6f6e 202d 2d64 6972 202e 2f64 656d 6f73  on --dir ./demos
+00001060: 202d 2d6c 6f67 207e 2f6c 6f67 7320 2d2d   --log ~/logs --
+00001070: 6261 7463 6820 3130 0a60 6060 0a0a 5468  batch 10.```..Th
+00001080: 6520 6162 6f76 6520 636f 6d6d 616e 6420  e above command 
+00001090: 7769 6c6c 2069 6d70 6f72 7420 616c 6c20  will import all 
+000010a0: 6874 6d6c 2066 696c 6573 2069 6e20 7468  html files in th
+000010b0: 6520 602e 2f64 656d 6f73 6020 6469 7265  e `./demos` dire
+000010c0: 6374 6f72 7920 696e 746f 204e 6f74 696f  ctory into Notio
+000010d0: 6e2c 2077 6869 6c65 206f 7574 7075 7474  n, while outputt
+000010e0: 696e 6720 6c6f 6773 2074 6f20 7468 6520  ing logs to the 
+000010f0: 607e 2f6c 6f67 7360 2064 6972 6563 746f  `~/logs` directo
+00001100: 7279 2c20 7769 7468 2075 7020 746f 2031  ry, with up to 1
+00001110: 3020 636f 6e63 7572 7265 6e74 2074 6173  0 concurrent tas
+00001120: 6b73 2e0a 0a23 204d 6f72 6520 696e 666f  ks...# More info
+00001130: 726d 6174 696f 6e0a 0a59 6f75 2063 616e  rmation..You can
+00001140: 2066 696e 6420 6d6f 7265 2069 6e66 6f72   find more infor
+00001150: 6d61 7469 6f6e 2061 6e64 2065 7861 6d70  mation and examp
+00001160: 6c65 7320 696e 2074 6865 2068 746d 6c32  les in the html2
+00001170: 6e6f 7469 6f6e 206c 6962 7261 7279 2773  notion library's
+00001180: 2049 7373 7565 3a20 5b68 746d 6c32 6e6f   Issue: [html2no
+00001190: 7469 6f6e 5d28 6874 7470 733a 2f2f 6769  tion](https://gi
+000011a0: 7468 7562 2e63 6f6d 2f73 656c 6662 6f6f  thub.com/selfboo
+000011b0: 742f 6874 6d6c 326e 6f74 696f 6e2f 6973  t/html2notion/is
+000011c0: 7375 6573 290a 0a23 2320 436f 6e74 7269  sues)..## Contri
+000011d0: 6275 7469 6f6e 0a0a 4966 2079 6f75 2066  bution..If you f
+000011e0: 696e 6420 616e 7920 6572 726f 7273 206f  ind any errors o
+000011f0: 7220 6861 7665 2061 6e79 2073 7567 6765  r have any sugge
+00001200: 7374 696f 6e73 2066 6f72 2069 6d70 726f  stions for impro
+00001210: 7665 6d65 6e74 2c20 706c 6561 7365 2064  vement, please d
+00001220: 6f20 6e6f 7420 6865 7369 7461 7465 2074  o not hesitate t
+00001230: 6f20 7375 626d 6974 2061 2070 756c 6c20  o submit a pull 
+00001240: 7265 7175 6573 7420 6f72 2072 6169 7365  request or raise
+00001250: 2061 6e20 6973 7375 652c 2049 2061 6d20   an issue, I am 
+00001260: 6d6f 7265 2074 6861 6e20 6861 7070 7920  more than happy 
+00001270: 746f 2061 6363 6570 7420 796f 7572 2063  to accept your c
+00001280: 6f6e 7472 6962 7574 696f 6e73 2061 6e64  ontributions and
+00001290: 2066 6565 6462 6163 6b21 0a0a 4966 2079   feedback!..If y
+000012a0: 6f75 2065 6e63 6f75 6e74 6572 2069 6d70  ou encounter imp
+000012b0: 6f72 7420 6661 696c 7572 6573 2c20 796f  ort failures, yo
+000012c0: 7520 6361 6e20 7375 626d 6974 2074 6865  u can submit the
+000012d0: 2068 746d 6c20 6669 6c65 2061 6e64 206c   html file and l
+000012e0: 6f67 2066 696c 6520 746f 6765 7468 6572  og file together
+000012f0: 2069 6e20 7468 6520 6973 7375 6520 666f   in the issue fo
+00001300: 7220 6561 7369 6572 2070 726f 626c 656d  r easier problem
+00001310: 2069 6465 6e74 6966 6963 6174 696f 6e2e   identification.
+00001320: 0a0a 3e20 4966 2074 6865 7265 2061 7265  ..> If there are
+00001330: 2061 6e79 2070 7269 7661 7465 2069 6e66   any private inf
+00001340: 6f72 6d61 7469 6f6e 2069 6e20 7468 6520  ormation in the 
+00001350: 6669 6c65 732c 2070 6c65 6173 6520 7265  files, please re
+00001360: 6d6f 7665 2069 7420 6669 7273 742e 0a0a  move it first...
+00001370: 0a23 2320 4c69 6365 6e73 650a 0a54 6869  .## License..Thi
+00001380: 7320 7072 6f6a 6563 7420 7573 6573 2074  s project uses t
+00001390: 6865 204d 4954 206c 6963 656e 7365 2e20  he MIT license. 
+000013a0: 506c 6561 7365 2072 6566 6572 2074 6f20  Please refer to 
+000013b0: 7468 6520 5b4c 4943 454e 5345 5d28 2e2f  the [LICENSE](./
+000013c0: 4c49 4345 4e53 4529 2066 6f72 2064 6574  LICENSE) for det
+000013d0: 6169 6c73 2e0a                           ails..
```

### Comparing `html2notion-0.1.9/html2notion.egg-info/SOURCES.txt` & `html2notion-0.2.0/html2notion.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,12 +23,14 @@
 html2notion/translate/import_stats.py
 html2notion/translate/notion_export.py
 html2notion/translate/notion_import.py
 html2notion/utils/__init__.py
 html2notion/utils/load_config.py
 html2notion/utils/log.py
 html2notion/utils/timeutil.py
+html2notion/utils/url_process.py
 tests/test_batchimport.py
 tests/test_cosupload.py
 tests/test_notionexport.py
 tests/test_reqlimit.py
+tests/test_util.py
 tests/test_yinxiang.py
```

### Comparing `html2notion-0.1.9/setup.cfg` & `html2notion-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = html2notion
-version = 0.1.9
+version = 0.2.0
 author = selfboot
 author_email = xuezaigds@gmail.com
 description = This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/selfboot/html2notion
 license_files = LICENSE
```

### Comparing `html2notion-0.1.9/tests/test_batchimport.py` & `html2notion-0.2.0/tests/test_batchimport.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,14 @@
 from html2notion.translate.batch_import import BatchImport
 from html2notion.utils import rate_limit
 from html2notion.utils.log import log_only_local
 
 process_once_time = 0.5
 
 
-@pytest.fixture(scope="session", autouse=True)
-def prepare_conf_fixture():
-    if 'GITHUB_ACTIONS' not in os.environ:
-        from html2notion.utils import test_prepare_conf, logger
-        test_prepare_conf()
-        logger.info("prepare_conf_fixture")
-
-
 async def mock_notion_api_request(file_path, *args, **kwargs):
     class MockResponse:
         def __init__(self, status_code, file_content, elapsed_time):
             self.status_code = status_code
             self.file_content = file_content
             self.elapsed_time = elapsed_time
```

### Comparing `html2notion-0.1.9/tests/test_cosupload.py` & `html2notion-0.2.0/tests/test_cosupload.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,22 +8,14 @@
 from unittest.mock import patch
 from tempfile import TemporaryDirectory
 from html2notion.translate.batch_import import BatchImport
 from html2notion.translate.cos_uploader import TencentCosUploaderAsync
 from html2notion.utils.log import log_only_local
 
 
-@pytest.fixture(scope="session", autouse=True)
-def prepare_conf_fixture():
-    if 'GITHUB_ACTIONS' not in os.environ:
-        from html2notion.utils import test_prepare_conf
-        test_prepare_conf()
-        log_only_local("prepare_conf_fixture")
-
-
 async def mock_cos_upload_request(file_path, *args, **kwargs):
     if 'GITHUB_ACTIONS' not in os.environ:
         from html2notion.utils import config
         secret_id = config["cos"]["secret_id"]
         secret_key = config["cos"]["secret_key"]
         region = config["cos"]["region"]
         bucket = config["cos"]["bucket"]
```

### Comparing `html2notion-0.1.9/tests/test_notionexport.py` & `html2notion-0.2.0/tests/test_notionexport.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from html2notion.translate.notion_export import NotionExporter
 import os
 import json
+from html2notion.translate.notion_export import NotionExporter
+from html2notion.utils import config
 
 
 def test_check_is_delete():
     del_keyvalue = [
         (["id"], "95948188-43cb-451f-b538-e0375368ca96"),
         (["parent", "type"], "page_id"),
         (["created_by", "object"], "user"),
@@ -36,16 +37,14 @@
 
 
 def test_export_blocks():
     if 'GITHUB_ACTIONS' in os.environ:
         api_key = os.environ['notion_api_key']
         page_id = os.environ['notion_page_id_1']
     else:
-        from html2notion.utils import config, test_prepare_conf
-        test_prepare_conf()
         api_key = config['notion']['api_key']
         page_id = config['notion']['page_id']
 
     names = locals()
     page_sizes = [1, 5, 10, 100]
     for i in page_sizes:
         names['exporter_' + str(i)] = NotionExporter(
```

### Comparing `html2notion-0.1.9/tests/test_reqlimit.py` & `html2notion-0.2.0/tests/test_reqlimit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,70 @@
 import json
-import os
 from html2notion.translate.html2json_yinxiang import Html2JsonYinXiang
 from html2notion.translate.import_stats import ImportStats
 
 
-paragram_rich_content = f'<div>{"Some words" * 400} more words</div>'
 block_max_conent = "Some words" * 200
-paragram_rich_block = [
-    {
-        "object": "block",
-        "type": "paragraph",
-        "paragraph": {
-            "rich_text": [
-                {
-                    "plain_text": block_max_conent,
-                    "text": {
-                        "content": block_max_conent
-                    },
-                    "type": "text"
-                },
-                {
-                    "plain_text": block_max_conent,
-                    "text": {
-                        "content": block_max_conent
-                    },
-                    "type": "text"
-                },
-                {
-                    "plain_text": " more words",
-                    "text": {
-                        "content": " more words"
-                    },
-                    "type": "text"
-                }
-            ]
-        }
-    }
-]
+one_text_obj = {
+    "plain_text": block_max_conent,
+    "text": {
+        "content": block_max_conent
+    },
+    "type": "text"
+}
+remain_text_obj = {
+    "plain_text": " more words",
+    "text": {
+        "content": " more words"
+    },
+    "type": "text"
+}
 
 
 def test_reqlimit():
-    if 'GITHUB_ACTIONS' not in os.environ:
-        from html2notion.utils import test_prepare_conf, logger
-        test_prepare_conf()
-        logger.info("prepare_conf_fixture")
-
-    html_jsons = {
-        paragram_rich_content: paragram_rich_block,
-    }
-
-    for html_content in html_jsons:
-        body_content = '<body>' + html_content + '</body>'
-        import_stats = ImportStats()
-        yinxiang = Html2JsonYinXiang(body_content, import_stats)
-        yinxiang.process()
-        json_obj = yinxiang.children
-        # print(json.dumps(json_obj, indent=4))
-        assert json_obj == html_jsons[html_content]
+    paragram_rich_block = [
+        {
+            "object": "block",
+            "type": "paragraph",
+            "paragraph": {
+                "rich_text": [
+                    one_text_obj, one_text_obj, remain_text_obj
+                ]
+            }
+        }
+    ]
+
+    paragram_rich_content = f'<body><div>{block_max_conent * 2} more words</div></body>'
+    import_stats = ImportStats()
+    yinxiang = Html2JsonYinXiang(paragram_rich_content, import_stats)
+    yinxiang.process()
+    json_obj = yinxiang.children
+    # print(json.dumps(json_obj, indent=4))
+    assert json_obj == paragram_rich_block
+
+
+def test_code_reqlimit():
+    code_rich_content = f'<body><div style="-en-codeblock: true">{block_max_conent * 2} more words</div></body>'
+    import_stats = ImportStats()
+    yinxiang = Html2JsonYinXiang(code_rich_content, import_stats)
+    yinxiang.process()
+    json_obj = yinxiang.children
+    # print(json.dumps(json_obj, indent=4))
+
+    split_block_result = [
+        {
+            "object": "block",
+            "type": "code",
+            "code": {
+                "rich_text": [
+                    one_text_obj, one_text_obj, remain_text_obj
+                ],
+                "language": "plain text"
+            }
+        }
+    ]
+    assert json_obj == split_block_result
 
 
 if __name__ == '__main__':
-    test_reqlimit()
+    # test_reqlimit()
+    test_code_reqlimit()
```

### Comparing `html2notion-0.1.9/tests/test_yinxiang.py` & `html2notion-0.2.0/tests/test_yinxiang.py`

 * *Files 1% similar despite different names*

```diff
@@ -834,19 +834,14 @@
                 }
             ]
         }
     }
 ]
 
 def test_convert():
-    if 'GITHUB_ACTIONS' not in os.environ:
-        from html2notion.utils import test_prepare_conf, logger
-        test_prepare_conf()
-        logger.info("prepare_conf_fixture")
-
     html_jsons = {
         paragram_br_content: paragram_br_block,
         link_content: link_block,
         order_list_content: ordered_list_block,
         nested_bold_content: nested_bold_block,
         paragram_rich_content: paragram_rich_block,
         heading_content: heading_block,
```

#### html2text {}

```diff
@@ -217,24 +217,21 @@
 ".\n\nFirst, you\u2019ll need a prompt that makes it clear what you want.
 Let\u2019s start with an instruction.\u00a0", "text": { "content": ".\n\nFirst,
 you\u2019ll need a prompt that makes it clear what you want. Let\u2019s start
 with an instruction.\u00a0" }, "type": "text" }, { "plain_text": "Submit this
 prompt", "text": { "content": "Submit this prompt" }, "type": "text",
 "annotations": { "bold": True } }, { "plain_text": "\u00a0to generate your
 first completion.", "text": { "content": "\u00a0to generate your first
-completion." }, "type": "text" } ] } } ] def test_convert(): if
-'GITHUB_ACTIONS' not in os.environ: from html2notion.utils import
-test_prepare_conf, logger test_prepare_conf() logger.info
-("prepare_conf_fixture") html_jsons = { paragram_br_content: paragram_br_block,
-link_content: link_block, order_list_content: ordered_list_block,
-nested_bold_content: nested_bold_block, paragram_rich_content:
-paragram_rich_block, heading_content: heading_block, code_content: code_block,
-code_paragraph_content: code_paragraph_block, language_code_content:
-language_code_block, table_content: table_block, super_note_table_content:
-table_block, to_do_content: to_do_block, to_do_normal_content: to_do_block,
-divider_content: divider_block, quote_content: quote_block, } for html_content
-in html_jsons: body_content = '
+completion." }, "type": "text" } ] } } ] def test_convert(): html_jsons =
+{ paragram_br_content: paragram_br_block, link_content: link_block,
+order_list_content: ordered_list_block, nested_bold_content: nested_bold_block,
+paragram_rich_content: paragram_rich_block, heading_content: heading_block,
+code_content: code_block, code_paragraph_content: code_paragraph_block,
+language_code_content: language_code_block, table_content: table_block,
+super_note_table_content: table_block, to_do_content: to_do_block,
+to_do_normal_content: to_do_block, divider_content: divider_block,
+quote_content: quote_block, } for html_content in html_jsons: body_content = '
 ' + html_content + '
 ' import_stats = ImportStats() yinxiang = Html2JsonYinXiang(body_content,
 import_stats) yinxiang.process() json_obj = yinxiang.children # print
 (json.dumps(json_obj, indent=4)) assert json_obj == html_jsons[html_content] if
 __name__ == '__main__': test_convert()
```

