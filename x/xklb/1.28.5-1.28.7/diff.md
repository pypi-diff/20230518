# Comparing `tmp/xklb-1.28.5.tar.gz` & `tmp/xklb-1.28.7.tar.gz`

## Comparing `xklb-1.28.5.tar` & `xklb-1.28.7.tar`

### file list

```diff
@@ -1,57 +1,56 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.28.5/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.28.5/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.28.5/Windows.md
--rw-r--r--   0        0        0   416122 2020-02-02 00:00:00.000000 xklb-1.28.5/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.28.5/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.28.5/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.28.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.28.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.28.5/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.28.5/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/__init__.py
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/av.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/books.py
--rw-r--r--   0        0        0     7732 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/consts.py
--rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/dl_config.py
--rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/dl_extract.py
--rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/fs_extract.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/hn_extract.py
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/lb.py
--rw-r--r--   0        0        0    37757 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/playback.py
--rw-r--r--   0        0        0    30250 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/praw_extract.py
--rw-r--r--   0        0        0    16161 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/stats.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21920 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/tube_backend.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/tube_extract.py
--rw-r--r--   0        0        0    28913 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/utils.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.28.5/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.28.5/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.28.5/LICENSE
--rw-r--r--   0        0        0    40704 2020-02-02 00:00:00.000000 xklb-1.28.5/README.md
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 xklb-1.28.5/pyproject.toml
--rw-r--r--   0        0        0    44218 2020-02-02 00:00:00.000000 xklb-1.28.5/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.28.7/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.28.7/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.28.7/Windows.md
+-rw-r--r--   0        0        0   416122 2020-02-02 00:00:00.000000 xklb-1.28.7/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.28.7/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.28.7/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.28.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.28.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.28.7/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.28.7/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/__init__.py
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/av.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/books.py
+-rw-r--r--   0        0        0     7732 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/consts.py
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/dl_config.py
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/lb.py
+-rw-r--r--   0        0        0    37927 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/playback.py
+-rw-r--r--   0        0        0    30606 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16161 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/stats.py
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21954 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28913 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/utils.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.28.7/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.28.7/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.28.7/LICENSE
+-rw-r--r--   0        0        0    40704 2020-02-02 00:00:00.000000 xklb-1.28.7/README.md
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 xklb-1.28.7/pyproject.toml
+-rw-r--r--   0        0        0    44218 2020-02-02 00:00:00.000000 xklb-1.28.7/PKG-INFO
```

### Comparing `xklb-1.28.5/Windows.md` & `xklb-1.28.7/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/pdm.lock` & `xklb-1.28.7/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -631,15 +631,15 @@
 summary = "Library for building powerful interactive command lines in Python"
 dependencies = [
     "wcwidth",
 ]
 
 [[package]]
 name = "protobuf"
-version = "4.23.0"
+version = "4.23.1"
 requires_python = ">=3.7"
 summary = ""
 
 [[package]]
 name = "psutil"
 version = "5.8.0"
 requires_python = ">=2.6, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
@@ -2249,28 +2249,28 @@
     {url = "https://files.pythonhosted.org/packages/d6/36/55cc2cab22aafbebd52ddac4ccb670b920b54eb6ddbdb8573c79ca870d8a/prawcore-2.3.0-py3-none-any.whl", hash = "sha256:48c17db447fa06a13ca3e722201f443031437708daa736c05a1df895fbcceff5"},
     {url = "https://files.pythonhosted.org/packages/ed/85/13e76be737f3159514cce609b29e95499ba6d2cfa0b88761bab318b5f63e/prawcore-2.3.0.tar.gz", hash = "sha256:daf1ccd4b7a80dc4e6567d48336d782e94a9a6dad83770fc2edf76dc9a84f56d"},
 ]
 "prompt-toolkit 3.0.38" = [
     {url = "https://files.pythonhosted.org/packages/4b/bb/75cdcd356f57d17b295aba121494c2333d26bfff1a837e6199b8b83c415a/prompt_toolkit-3.0.38.tar.gz", hash = "sha256:23ac5d50538a9a38c8bde05fecb47d0b403ecd0662857a86f886f798563d5b9b"},
     {url = "https://files.pythonhosted.org/packages/87/3f/1f5a0ff475ae6481f4b0d45d4d911824d3218b94ee2a97a8cb84e5569836/prompt_toolkit-3.0.38-py3-none-any.whl", hash = "sha256:45ea77a2f7c60418850331366c81cf6b5b9cf4c7fd34616f733c5427e6abbb1f"},
 ]
-"protobuf 4.23.0" = [
-    {url = "https://files.pythonhosted.org/packages/06/38/e72c556c25aaaaafca75018d2d0ebc50c5ab80983dd4def086624fba43f2/protobuf-4.23.0-cp37-abi3-manylinux2014_x86_64.whl", hash = "sha256:ebde3a023b8e11bfa6c890ef34cd6a8b47d586f26135e86c21344fe433daf2e2"},
-    {url = "https://files.pythonhosted.org/packages/15/a9/287edf57651a60336a92f2d959a244ac3184bd3e0d0616b21e1731fc3e5e/protobuf-4.23.0-cp37-abi3-macosx_10_9_universal2.whl", hash = "sha256:2b94bd6df92d71bd1234a2ffe7ce96ddf6d10cf637a18d6b55ad0a89fbb7fc21"},
-    {url = "https://files.pythonhosted.org/packages/17/ba/29ff6b6ff827178ac7f66ee7fd383342a188ffa6a96084bad1513d942da1/protobuf-4.23.0-cp39-cp39-win32.whl", hash = "sha256:03eee35b60317112a72d19c54d0bff7bc58ff12fea4cd7b018232bd99758ffdf"},
-    {url = "https://files.pythonhosted.org/packages/31/d1/bc0780924e53c7dd0aca42be0c2d933998dbb744c30bdda48bd9e63808a5/protobuf-4.23.0-cp38-cp38-win32.whl", hash = "sha256:d5a35ff54e3f62e8fc7be02bb0d2fbc212bba1a5a9cc2748090690093996f07b"},
-    {url = "https://files.pythonhosted.org/packages/60/1a/79f077c5baf5a9262ed41cc0909c1230ecac5cb4f4960cd97942c88d1726/protobuf-4.23.0.tar.gz", hash = "sha256:5f1eba1da2a2f3f7df469fccddef3cc060b8a16cfe3cc65961ad36b4dbcf59c5"},
-    {url = "https://files.pythonhosted.org/packages/60/db/9579f388a3627b867519f476ab5b3cf8391fbf79e5827f370a86ba911483/protobuf-4.23.0-cp37-abi3-manylinux2014_aarch64.whl", hash = "sha256:9f5a0fbfcdcc364f3986f9ed9f8bb1328fb84114fd790423ff3d7fdb0f85c2d1"},
-    {url = "https://files.pythonhosted.org/packages/6a/a2/c0b1c36c146212815a8307469054bb972b0d82fcecf21c83600d7882574f/protobuf-4.23.0-cp38-cp38-win_amd64.whl", hash = "sha256:e62fb869762b4ba18666370e2f8a18f17f8ab92dd4467295c6d38be6f8fef60b"},
-    {url = "https://files.pythonhosted.org/packages/6f/2e/49169f6fc6b39f77e0fa94bc8a2e300a75d57ca7953cc1dbe15c1ead9efa/protobuf-4.23.0-cp37-cp37m-win_amd64.whl", hash = "sha256:6fe180b56e1169d72ecc4acbd39186339aed20af5384531b8e8979b02bbee159"},
-    {url = "https://files.pythonhosted.org/packages/89/e1/c03399e5bf8b2fb97f0f41e9039583fc78040503559bed5a09ac3ea15421/protobuf-4.23.0-cp310-abi3-win_amd64.whl", hash = "sha256:baca40d067dddd62141a129f244703160d278648b569e90bb0e3753067644711"},
-    {url = "https://files.pythonhosted.org/packages/aa/f1/b17e29296a85eeeebac34a9a631ba4c46e23b632e64ceea86633de1e69e1/protobuf-4.23.0-cp37-cp37m-win32.whl", hash = "sha256:7cb5b9a05ce52c6a782bb97de52679bd3438ff2b7460eff5da348db65650f227"},
-    {url = "https://files.pythonhosted.org/packages/ba/59/bea9d68041fa6899eb47a60c0f3821e88f73ee6f69ad95a557158da40a60/protobuf-4.23.0-cp310-abi3-win32.whl", hash = "sha256:6c16657d6717a0c62d5d740cb354fbad1b0d8cb811669e06fc1caa0ff4799ddd"},
-    {url = "https://files.pythonhosted.org/packages/bf/65/f0ee96df56178e36705b3c97e69f9f7f08f64907632ecbbc08df0d3545da/protobuf-4.23.0-py3-none-any.whl", hash = "sha256:9744e934ea5855d12191040ea198eaf704ac78665d365a89d9572e3b627c2688"},
-    {url = "https://files.pythonhosted.org/packages/d3/3c/6bbbe3a5ccb68f117dc572d8b612efb77dc5824b87687ee52eb61abf965f/protobuf-4.23.0-cp39-cp39-win_amd64.whl", hash = "sha256:36f5370a930cb77c8ad2f4135590c672d0d2c72d4a707c7d0058dce4b4b4a598"},
+"protobuf 4.23.1" = [
+    {url = "https://files.pythonhosted.org/packages/12/40/d5333cf8adbd6bf77bf33aecd96d69545424aa0fd63b9ae30cf6c61efa47/protobuf-4.23.1-cp310-abi3-win_amd64.whl", hash = "sha256:32e78beda26d7a101fecf15d7a4a792278a0d26a31bc327ff05564a9d68ab8ee"},
+    {url = "https://files.pythonhosted.org/packages/24/e7/f193d7480b5f777c64515f81c3b8c074c1d7b283695397d4f965441c6bc8/protobuf-4.23.1-cp310-abi3-win32.whl", hash = "sha256:410bcc0a5b279f634d3e16082ce221dfef7c3392fac723500e2e64d1806dd2be"},
+    {url = "https://files.pythonhosted.org/packages/2f/b4/966ccfcac26d8f56cacf56e4c0878d367ea9f5597be0144774fbc464271e/protobuf-4.23.1-cp39-cp39-win_amd64.whl", hash = "sha256:ac50be82491369a9ec3710565777e4da87c6d2e20404e0abb1f3a8f10ffd20f0"},
+    {url = "https://files.pythonhosted.org/packages/40/b7/700f2a5fc5aa009903d816a040ababcc7e5874df2deacb168f3a718b0d73/protobuf-4.23.1-cp37-abi3-manylinux2014_aarch64.whl", hash = "sha256:346990f634272caac1f09efbcfbbacb23098b1f606d172534c6fa2d9758bb436"},
+    {url = "https://files.pythonhosted.org/packages/49/be/78eb56a8c035bb582dbd89ec48b0be4f67288ae872d55d7698b3cb8b5562/protobuf-4.23.1-cp37-abi3-macosx_10_9_universal2.whl", hash = "sha256:f9510cac91e764e86acd74e2b7f7bc5e6127a7f3fb646d7c8033cfb84fd1176a"},
+    {url = "https://files.pythonhosted.org/packages/56/65/d1e5919fe13d46e8dabefe32526745c3ef1f47d88b0e1d5593fdbc1e1dd3/protobuf-4.23.1-cp37-cp37m-win_amd64.whl", hash = "sha256:3b8905eafe4439076e1f58e9d1fa327025fd2777cf90f14083092ae47f77b0aa"},
+    {url = "https://files.pythonhosted.org/packages/59/81/cdf57f5e952f7ff0512b9b04ba46424bf4fde1553feb710e1f1d9330be34/protobuf-4.23.1-cp38-cp38-win32.whl", hash = "sha256:5b9cd6097e6acae48a68cb29b56bc79339be84eca65b486910bb1e7a30e2b7c1"},
+    {url = "https://files.pythonhosted.org/packages/61/33/876ca85424503ae048ec3b765d228494eb27f240600835b5be6c23d1d209/protobuf-4.23.1-cp38-cp38-win_amd64.whl", hash = "sha256:decf119d54e820f298ee6d89c72d6b289ea240c32c521f00433f9dc420595f38"},
+    {url = "https://files.pythonhosted.org/packages/73/8b/926449627e192b022f71d2c48b51dbdc1271271e0fa4b809cff2dffab339/protobuf-4.23.1-cp37-abi3-manylinux2014_x86_64.whl", hash = "sha256:3ce113b3f3362493bddc9069c2163a38f240a9ed685ff83e7bcb756b05e1deb0"},
+    {url = "https://files.pythonhosted.org/packages/c7/fc/4775e99b4bc52309ac30e1751f260b8b637482b0e6647b397a52c4adff77/protobuf-4.23.1-cp39-cp39-win32.whl", hash = "sha256:91fac0753c3c4951fbb98a93271c43cc7cf3b93cf67747b3e600bb1e5cc14d61"},
+    {url = "https://files.pythonhosted.org/packages/d1/2a/bf4c68e2ef7552bbd9f6a17937fd46ab4eaee6b7b5e4723a6e00b4270144/protobuf-4.23.1-py3-none-any.whl", hash = "sha256:65f0ac96ef67d7dd09b19a46aad81a851b6f85f89725577f16de38f2d68ad477"},
+    {url = "https://files.pythonhosted.org/packages/d8/6c/a2a6fe10cdc9bc81e03be56139d5bc70427054eb0b3864b31ff9a2a4849d/protobuf-4.23.1.tar.gz", hash = "sha256:95789b569418a3e32a53f43d7763be3d490a831e9c08042539462b6d972c2d7e"},
+    {url = "https://files.pythonhosted.org/packages/e4/78/665cb3b2165c29037cea06e9d4774713a6bf1844dec118af98a8c427c24c/protobuf-4.23.1-cp37-cp37m-win32.whl", hash = "sha256:2036a3a1e7fc27f973fa0a7888dce712393af644f4695385f117886abc792e39"},
 ]
 "psutil 5.8.0" = [
     {url = "https://files.pythonhosted.org/packages/10/d6/c5c19e40bb05e2cb5f053f480dfe47e9543a8322f1a5985d7352bf689611/psutil-5.8.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:6223d07a1ae93f86451d0198a0c361032c4c93ebd4bf6d25e2fb3edfad9571ef"},
     {url = "https://files.pythonhosted.org/packages/12/80/8d09c345f19af2b29a309f8f9284e3ba1ae1ebd9438419080c14630f743a/psutil-5.8.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6323d5d845c2785efb20aded4726636546b26d3b577aded22492908f7c1bdda7"},
     {url = "https://files.pythonhosted.org/packages/15/28/47c28171fd7eeb83df74f78ccac090211f4a49408f376eb8e78a7bb47dc0/psutil-5.8.0-cp27-cp27mu-manylinux2010_i686.whl", hash = "sha256:02b8292609b1f7fcb34173b25e48d0da8667bc85f81d7476584d889c6e0f2131"},
     {url = "https://files.pythonhosted.org/packages/18/c9/1db6aa0d28831f60408a6aab9d108c2edbd5a9ed11e5957a91d9d8023898/psutil-5.8.0-cp37-cp37m-win32.whl", hash = "sha256:1bff0d07e76114ec24ee32e7f7f8d0c4b0514b3fae93e3d2aaafd65d22502394"},
     {url = "https://files.pythonhosted.org/packages/19/29/f7a38ee30083f2caa14cc77a6d34c4d5cfd1a69641e87bf1b3d6ba90d0ba/psutil-5.8.0-cp36-cp36m-win32.whl", hash = "sha256:36b3b6c9e2a34b7d7fbae330a85bf72c30b1c827a4366a07443fc4b6270449e2"},
```

### Comparing `xklb-1.28.5/readme.py` & `xklb-1.28.7/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.28.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.28.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/.github/workflows/push.yaml` & `xklb-1.28.7/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/sql/transfer.sql` & `xklb-1.28.7/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/av.py` & `xklb-1.28.7/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/books.py` & `xklb-1.28.7/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/consts.py` & `xklb-1.28.7/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/db.py` & `xklb-1.28.7/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/dl_config.py` & `xklb-1.28.7/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/dl_extract.py` & `xklb-1.28.7/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/fs_extract.py` & `xklb-1.28.7/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/gui.py` & `xklb-1.28.7/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/hn_extract.py` & `xklb-1.28.7/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/lb.py` & `xklb-1.28.7/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/play_actions.py` & `xklb-1.28.7/xklb/play_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -711,37 +711,37 @@
     Path(path).unlink()
     shutil.move(temp_video, transcode_dest)
     with args.db.conn:
         args.db.conn.execute("UPDATE media SET path = ? where path = ?", [transcode_dest, path])
     return transcode_dest
 
 
-def prep_media(args, m: Dict):
+def prep_media(args, m: Dict, ignore_paths):
     t = utils.Timer()
     args.db = db.connect(args)
     log.debug("db.connect: %s", t.elapsed())
 
     if is_play_in_order_lvl2(args, m["path"]):
-        m = player.get_ordinal_media(args, m)
+        m = player.get_ordinal_media(args, m, ignore_paths)
         log.debug("player.get_ordinal_media: %s", t.elapsed())
 
     m["original_path"] = m["path"]
-    if args.action in (SC.watch, SC.listen) and not m["path"].startswith("http"):
+    if not m["path"].startswith("http"):
         media_path = Path(args.prefix + m["path"]).resolve() if args.prefix else Path(m["path"])
         m["path"] = str(media_path)
 
         if not media_path.exists():
             log.debug("media_path exists: %s", t.elapsed())
             log.warning("[%s]: Does not exist. Skipping...", m["path"])
             mark_media_deleted(args, m["original_path"])
             log.debug("mark_media_deleted: %s", t.elapsed())
             return None
 
         if args.transcode or args.transcode_audio:
-            m["path"] = transcode(args, m["path"])
+            m["path"] = m["original_path"] = transcode(args, m["path"])
             log.debug("transcode: %s", t.elapsed())
 
     m["now_playing"] = now_playing(m["path"])
 
     return m
 
 
@@ -854,26 +854,28 @@
     else:
         if args.related >= consts.RELATED:
             media = player.get_related_media(args, media[0])
             log.debug("player.get_related_media: %s", t.elapsed())
         try:
             mp_args = argparse.Namespace(**{k: v for k, v in args.__dict__.items() if k not in {"db"}})
             media.reverse()  # because media.pop()
+            ignore_paths = []
             futures = deque()
             with ThreadPoolExecutor(max_workers=1) as executor:
                 while media or futures:
                     while media and len(futures) < 3:
                         m = media.pop()
-                        future = executor.submit(prep_media, mp_args, m)
+                        future = executor.submit(prep_media, mp_args, m, ignore_paths)
+                        ignore_paths.append(m["path"])
                         futures.append(future)
 
                     if futures:
                         future = futures.popleft()
                         m = future.result()
-                        if m is not None:
+                        if m is not None and (m["path"].startswith("http") or Path(m["path"]).exists()):
                             play(args, m)
         finally:
             if args.interdimensional_cable:
                 args.sock.send(b"raw quit \n")
             Path(args.mpv_socket).unlink(missing_ok=True)
             if args.chromecast:
                 Path(consts.CAST_NOW_PLAYING).unlink(missing_ok=True)
```

### Comparing `xklb-1.28.5/xklb/playback.py` & `xklb-1.28.7/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/player.py` & `xklb-1.28.7/xklb/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,16 +381,18 @@
     while len(remove_chars) < 1:
         remove_chars += remove_groups[-number_of_groups]
         number_of_groups += 1
 
     return remove_chars
 
 
-def get_ordinal_media(args, m: Dict) -> Dict:
+def get_ordinal_media(args, m: Dict, ignore_paths=None) -> Dict:
     # TODO: maybe try https://dba.stackexchange.com/questions/43415/algorithm-for-finding-the-longest-prefix
+    if ignore_paths is None:
+        ignore_paths = []
 
     columns = args.db["media"].columns_dict
 
     total_media = args.db.execute("select count(*) val from media").fetchone()[0]
     candidate = deepcopy(m["path"])
     similar_videos = []
     while len(similar_videos) <= 1:
@@ -410,18 +412,20 @@
             SELECT
                 {args.select_sql}
             FROM {'media' if args.play_in_order >= consts.SIMILAR_NO_FILTER_NO_FTS else args.table}
             WHERE 1=1
                 and path like :candidate
                 {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in columns else ''}
                 {'' if args.play_in_order >= consts.SIMILAR_NO_FILTER else (" ".join(args.filter_sql) or '')}
+                {"and path not in ({})".format(",".join([":ignore_path{}".format(i) for i in range(len(ignore_paths))])) if len(ignore_paths) > 0 else ''}
             ORDER BY play_count, path
             LIMIT 1000
             """
-        bindings = {"candidate": candidate + "%"}
+        ignore_path_params = {":ignore_path{}".format(i): value for i, value in enumerate(ignore_paths)}
+        bindings = {"candidate": candidate + "%", **ignore_path_params}
         if args.play_in_order >= consts.SIMILAR_NO_FILTER:
             if args.include or args.exclude:
                 bindings = {**bindings, "query": args.filter_bindings["query"]}
         else:
             bindings = {**bindings, **args.filter_bindings}
 
         similar_videos = list(args.db.query(query, bindings))
```

### Comparing `xklb-1.28.5/xklb/praw_extract.py` & `xklb-1.28.7/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/stats.py` & `xklb-1.28.7/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/subtitle.py` & `xklb-1.28.7/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/tabs_actions.py` & `xklb-1.28.7/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/tabs_extract.py` & `xklb-1.28.7/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/tube_backend.py` & `xklb-1.28.7/xklb/tube_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,18 +460,19 @@
         return
 
     assert info["local_path"] != ""
     if Path(info["local_path"]).exists():
         fs_args = argparse.Namespace(
             profile=args.profile,
             scan_subtitles=args.profile == DBType.video,
-            delete_unplayable=False,
             ocr=False,
             speech_recognition=False,
+            delete_unplayable=False,
             check_corrupt=False,
+            delete_corrupt=False,
         )
         fs_tags = utils.dict_filter_bool(fs_extract.extract_metadata(fs_args, info["local_path"]), keep_0=False) or {}
         fs_extract.clean_up_temp_dirs()
     else:
         fs_tags = {}
 
     tube_entry = consolidate(info) or {}
```

### Comparing `xklb-1.28.5/xklb/tube_extract.py` & `xklb-1.28.7/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/utils.py` & `xklb-1.28.7/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/__init__.py` & `xklb-1.28.7/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/bigdirs.py` & `xklb-1.28.7/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/christen.py` & `xklb-1.28.7/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/copy_play_counts.py` & `xklb-1.28.7/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/dedupe.py` & `xklb-1.28.7/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/merge_dbs.py` & `xklb-1.28.7/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/merge_online_local.py` & `xklb-1.28.7/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/move_list.py` & `xklb-1.28.7/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/optimize_db.py` & `xklb-1.28.7/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/redownload.py` & `xklb-1.28.7/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/relmv.py` & `xklb-1.28.7/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/scatter.py` & `xklb-1.28.7/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/streaming_tab_loader.py` & `xklb-1.28.7/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/mining/data.py` & `xklb-1.28.7/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/mining/extract_links.py` & `xklb-1.28.7/xklb/scripts/mining/extract_links.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,103 @@
-import argparse
+import argparse, time
+from shutil import which
 
-from xklb import consts
 from xklb.utils import log, pipe_print
 
 
-def get_page_links(url, include=None, exclude=None) -> None:
+def get_links(url, markup, include=None, exclude=None) -> None:
     from urllib.parse import urlparse
 
-    import requests
     from bs4 import BeautifulSoup
 
-    soup = BeautifulSoup(requests.get(url, timeout=120).content, "html.parser")
+    soup = BeautifulSoup(markup, "html.parser")
     film_list = set()
 
     for a in soup.findAll("a", attrs={"href": True}):
         log.debug(a)
 
         href = a["href"].strip()
         if (len(href) > 1) and href[0] != "#":
             if any(s in href for s in (exclude or [])):
                 log.debug("excluded: %s", href)
                 continue
 
-            up = urlparse(url)
-            full_path = up.scheme + "://" + up.netloc + href
+            up = urlparse(href)
+            if not up.netloc:
+                up = urlparse(url)
+                href = up.scheme + "://" + up.netloc + href
+
             if include is None or len(include) == 0:
-                film_list.add(full_path)
+                film_list.add(href)
             elif all(s in href for s in include):
                 log.debug("included: %s", href)
-                film_list.add(full_path)
+                film_list.add(href)
             else:
                 log.debug("else: %s", href)
 
         # breakpoint()
 
     pipe_print("\n".join(film_list))
 
 
+def get_page_infinite_scroll(driver, url):
+    driver.get(url)
+    time.sleep(1)
+
+    last_height = driver.execute_script("return document.body.scrollHeight")
+    while True:
+        driver.execute_script("window.scrollTo(0, document.body.scrollHeight);")
+        time.sleep(2)
+        new_height = driver.execute_script("return document.body.scrollHeight")
+        if new_height == last_height:
+            break
+        last_height = new_height
+
+    return driver.page_source
+
+
 def extract_links() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument("--include", "-s", nargs="*", help="substrings for inclusion (all must match to include)")
     parser.add_argument(
         "--exclude",
         "-E",
         nargs="*",
         default=["javascript:", "mailto:", "tel:"],
         help="substrings for exclusion (any must match to exclude)",
     )
+    parser.add_argument("--scroll", action="store_true", help="Scroll down the page; infinite scroll")
+    parser.add_argument("--verbose", "-v", action="count", default=0)
+
     parser.add_argument("filename", help="File with one URL per line")
     args = parser.parse_args()
 
+    import requests
+
+    if args.scroll:
+        from selenium import webdriver
+
+        if which("firefox"):
+            driver = webdriver.Firefox()
+        else:
+            driver = webdriver.Chrome()
+
     with open(args.filename, "r") as f:
         for line in f:
-            line = line.rstrip("\n")
-            if line in ["", '""', "\n"]:
+            url = line.rstrip("\n")
+            if url in ["", '""', "\n"]:
                 continue
 
-            get_page_links(line, include=args.include, exclude=args.exclude)
+            if args.scroll:
+                markup = get_page_infinite_scroll(driver, url)
+            else:
+                markup = requests.get(url, timeout=120).content
+
+            get_links(url, markup, include=args.include, exclude=args.exclude)
+
+    if args.scroll:
+        driver.quit()
 
 
 if __name__ == "__main__":
     # echo $directors | python scripts/mining/nfb.ca.py | tee -a ~/.jobs/75
     extract_links()
```

### Comparing `xklb-1.28.5/xklb/scripts/mining/nouns.py` & `xklb-1.28.7/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/mining/pushshift.py` & `xklb-1.28.7/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.28.7/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/.gitignore` & `xklb-1.28.7/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/LICENSE` & `xklb-1.28.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.28.5/README.md` & `xklb-1.28.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.28.005)
+    xk media library subcommands (v1.28.007)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.28.5/pyproject.toml` & `xklb-1.28.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 [tool.hatch.build]
 exclude = [
   "tests/",
   "examples/",
 ]
 
 [tool.hatch.build.force-include]
-"assets/" = "xklb/assets/"
+"xklb/assets/" = "xklb/assets/"
 
 [tool.black]
 line-length = 120
 target-version = ['py38', 'py39', 'py310']
 
 [tool.isort]
 atomic = true
```

### Comparing `xklb-1.28.5/PKG-INFO` & `xklb-1.28.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.28.5
+Version: 1.28.7
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -99,15 +99,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.28.005)
+    xk media library subcommands (v1.28.007)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

