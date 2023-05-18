# Comparing `tmp/crowsetta-5.0.0rc1.tar.gz` & `tmp/crowsetta-5.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowsetta-5.0.0rc1.tar", last modified: Wed Mar  1 17:11:01 2023, max compression
+gzip compressed data, was "crowsetta-5.0.0rc2.tar", last modified: Mon Mar  6 16:54:23 2023, max compression
```

## Comparing `crowsetta-5.0.0rc1.tar` & `crowsetta-5.0.0rc2.tar`

### file list

```diff
@@ -1,170 +1,170 @@
--rw-r--r--   0        0        0      815 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/.all-contributorsrc
--rw-r--r--   0        0        0     1311 2023-02-28 02:25:58.381961 crowsetta-5.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      248 2022-05-29 23:39:40.790272 crowsetta-5.0.0rc1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      615 2022-05-29 23:39:40.790272 crowsetta-5.0.0rc1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      749 2022-07-09 15:59:11.933074 crowsetta-5.0.0rc1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      823 2023-02-28 03:20:43.051389 crowsetta-5.0.0rc1/.github/workflows/lint.yml
--rw-r--r--   0        0        0      356 2022-06-17 12:22:33.160303 crowsetta-5.0.0rc1/.gitignore
--rw-r--r--   0        0        0     1089 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      366 2022-05-14 19:55:14.983897 crowsetta-5.0.0rc1/.readthedocs.yaml
--rw-r--r--   0        0        0      746 2022-03-26 14:16:03.816914 crowsetta-5.0.0rc1/CITATION.cff
--rw-r--r--   0        0        0     5556 2023-02-28 02:25:58.381961 crowsetta-5.0.0rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1879 2023-01-28 00:47:08.677330 crowsetta-5.0.0rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1515 2020-11-08 19:17:24.773706 crowsetta-5.0.0rc1/LICENSE
--rw-r--r--   0        0        0     8972 2023-03-01 17:08:05.259918 crowsetta-5.0.0rc1/README.md
--rw-r--r--   0        0        0    21569 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/doc/CHANGELOG.md
--rw-r--r--   0        0        0      580 2023-02-28 02:25:58.381961 crowsetta-5.0.0rc1/doc/Makefile
--rw-r--r--   0        0        0    26325 2022-06-24 16:51:56.243598 crowsetta-5.0.0rc1/doc/_static/crowsetta-logomark.png
--rw-r--r--   0        0        0   250992 2022-06-24 16:51:56.243598 crowsetta-5.0.0rc1/doc/_static/crowsetta-primary-logo.png
--rw-r--r--   0        0        0    83463 2022-06-24 16:51:56.247598 crowsetta-5.0.0rc1/doc/_static/crowsetta-secondary-logo.png
--rw-r--r--   0        0        0  1638145 2022-06-17 12:22:33.180303 crowsetta-5.0.0rc1/doc/_static/example-raven-for-index.png
--rw-r--r--   0        0        0   640083 2022-06-17 12:22:33.184303 crowsetta-5.0.0rc1/doc/_static/example-textgrid-for-index.png
--rw-r--r--   0        0        0      612 2023-02-28 02:25:58.381961 crowsetta-5.0.0rc1/doc/_templates/class.rst
--rw-r--r--   0        0        0     1177 2023-02-28 02:25:58.381961 crowsetta-5.0.0rc1/doc/_templates/module.rst
--rw-r--r--   0        0        0     1857 2023-02-28 02:25:58.381961 crowsetta-5.0.0rc1/doc/api/core.md
--rw-r--r--   0        0        0      409 2023-02-28 02:25:58.381961 crowsetta-5.0.0rc1/doc/api/formats.md
--rw-r--r--   0        0        0      581 2023-02-28 02:25:58.381961 crowsetta-5.0.0rc1/doc/api/index.md
--rw-r--r--   0        0        0      565 2022-06-17 12:22:33.184303 crowsetta-5.0.0rc1/doc/api/interface.md
--rw-r--r--   0        0        0     6936 2023-01-29 04:28:20.964269 crowsetta-5.0.0rc1/doc/conf.py
--rw-r--r--   0        0        0        0 2022-06-17 12:22:33.184303 crowsetta-5.0.0rc1/doc/data/.gitkeep
--rw-r--r--   0        0        0        0 2023-01-29 04:28:20.964269 crowsetta-5.0.0rc1/doc/data/giraudon-et-al-2021/.gitkeep
--rw-r--r--   0        0        0      446 2022-12-26 02:24:00.910465 crowsetta-5.0.0rc1/doc/development/commit-abbreviations.rst
--rw-r--r--   0        0        0     8631 2023-02-28 02:25:58.385961 crowsetta-5.0.0rc1/doc/development/contributors.md
--rw-r--r--   0        0        0     1024 2023-02-28 02:25:58.385961 crowsetta-5.0.0rc1/doc/development/index.md
--rw-r--r--   0        0        0      741 2023-02-28 02:25:58.385961 crowsetta-5.0.0rc1/doc/formats/bbox/raven.md
--rw-r--r--   0        0        0     1556 2023-02-28 02:25:58.385961 crowsetta-5.0.0rc1/doc/formats/index.md
--rw-r--r--   0        0        0     1092 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/doc/formats/seq/aud-seq.md
--rw-r--r--   0        0        0     1179 2023-02-28 02:25:58.385961 crowsetta-5.0.0rc1/doc/formats/seq/birdsongrec.md
--rw-r--r--   0        0        0     1268 2023-02-28 02:25:58.385961 crowsetta-5.0.0rc1/doc/formats/seq/generic-seq.md
--rw-r--r--   0        0        0      783 2023-02-28 02:25:58.385961 crowsetta-5.0.0rc1/doc/formats/seq/notmat.md
--rw-r--r--   0        0        0     1294 2023-02-28 02:25:58.385961 crowsetta-5.0.0rc1/doc/formats/seq/simple-seq.md
--rw-r--r--   0        0        0      717 2023-02-28 02:25:58.385961 crowsetta-5.0.0rc1/doc/formats/seq/textgrid.md
--rw-r--r--   0        0        0      739 2023-02-28 02:25:58.385961 crowsetta-5.0.0rc1/doc/formats/seq/timit.md
--rw-r--r--   0        0        0      231 2023-01-29 04:28:20.964269 crowsetta-5.0.0rc1/doc/howto.md
--rw-r--r--   0        0        0     7488 2022-06-17 12:22:33.188303 crowsetta-5.0.0rc1/doc/howto/bat1_annotation.mat
--rw-r--r--   0        0        0     4503 2023-02-27 03:31:23.217511 crowsetta-5.0.0rc1/doc/howto/batlab.py
--rw-r--r--   0        0        0     7256 2023-03-01 15:59:42.478523 crowsetta-5.0.0rc1/doc/howto/convert-generic-seq.md
--rw-r--r--   0        0        0     9563 2023-02-28 02:25:58.385961 crowsetta-5.0.0rc1/doc/howto/convert-simple-seq.md
--rw-r--r--   0        0        0    26382 2023-03-01 14:42:53.673937 crowsetta-5.0.0rc1/doc/howto/howto-user-format.md
--rw-r--r--   0        0        0     2265 2022-06-17 12:22:33.188303 crowsetta-5.0.0rc1/doc/howto/parsebat.py
--rw-r--r--   0        0        0    29107 2023-03-01 15:59:42.478523 crowsetta-5.0.0rc1/doc/howto/remove-silent-labels-textgrid.md
--rw-r--r--   0        0        0    12885 2023-02-28 02:25:58.385961 crowsetta-5.0.0rc1/doc/index.md
--rw-r--r--   0        0        0      752 2020-11-08 19:17:24.773706 crowsetta-5.0.0rc1/doc/make.bat
--rw-r--r--   0        0        0      881 2023-02-28 02:25:58.385961 crowsetta-5.0.0rc1/doc/nitpick-ignore.txt
--rw-r--r--   0        0        0    19417 2022-06-17 12:22:33.188303 crowsetta-5.0.0rc1/doc/scripts/annot/Recording_1_Segment_07.Table.1.selections.txt
--rw-r--r--   0        0        0  2942427 2023-02-28 02:25:58.393961 crowsetta-5.0.0rc1/doc/scripts/annot/b06_concat_dtw.TextGrid
--rw-r--r--   0        0        0   640046 2022-06-17 12:22:33.200304 crowsetta-5.0.0rc1/doc/scripts/audio/Recording_1_Segment_07-snippet.wav
--rw-r--r--   0        0        0   150046 2022-06-17 12:22:33.200304 crowsetta-5.0.0rc1/doc/scripts/audio/b06_concat-snippet.wav
--rw-r--r--   0        0        0     3885 2023-02-28 02:25:58.393961 crowsetta-5.0.0rc1/doc/scripts/raven-chronister-et-al-2021.md
--rw-r--r--   0        0        0     5966 2023-02-28 02:25:58.393961 crowsetta-5.0.0rc1/doc/scripts/textgrid-BF-dataset.md
--rw-r--r--   0        0        0    10627 2023-03-01 15:59:42.478523 crowsetta-5.0.0rc1/doc/tutorial.md
--rw-r--r--   0        0        0     2927 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/noxfile.py
--rw-r--r--   0        0        0     1969 2023-03-01 17:10:23.499388 crowsetta-5.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0      846 2023-03-01 17:09:20.879628 crowsetta-5.0.0rc1/src/crowsetta/__about__.py
--rw-r--r--   0        0        0      882 2023-03-01 16:38:02.701773 crowsetta-5.0.0rc1/src/crowsetta/__init__.py
--rw-r--r--   0        0        0        0 2022-01-02 15:09:55.128327 crowsetta-5.0.0rc1/src/crowsetta/_vendor/__init__.py
--rw-r--r--   0        0        0      379 2023-02-28 02:25:58.393961 crowsetta-5.0.0rc1/src/crowsetta/_vendor/textgrid/AUTHORS
--rw-r--r--   0        0        0     1090 2022-01-02 15:09:55.128327 crowsetta-5.0.0rc1/src/crowsetta/_vendor/textgrid/LICENSE
--rw-r--r--   0        0        0      723 2022-01-02 15:09:55.128327 crowsetta-5.0.0rc1/src/crowsetta/_vendor/textgrid/README.md
--rw-r--r--   0        0        0       78 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/_vendor/textgrid/__init__.py
--rw-r--r--   0        0        0       41 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/_vendor/textgrid/exceptions.py
--rw-r--r--   0        0        0    32141 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/_vendor/textgrid/textgrid.py
--rw-r--r--   0        0        0     3206 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/annotation.py
--rw-r--r--   0        0        0     1627 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/bbox.py
--rw-r--r--   0        0        0      469 2023-03-01 16:38:02.701773 crowsetta-5.0.0rc1/src/crowsetta/data/__init__.py
--rw-r--r--   0        0        0        0 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/src/crowsetta/data/audbbox/__init__.py
--rw-r--r--   0        0        0      153 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/src/crowsetta/data/audbbox/citation.txt
--rw-r--r--   0        0        0      887 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/src/crowsetta/data/audbbox/spinetail.txt
--rw-r--r--   0        0        0     1828 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/src/crowsetta/data/audseq/405_marron1_June_14_2016_69640887.audacity.txt
--rw-r--r--   0        0        0        0 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/src/crowsetta/data/audseq/__init__.py
--rw-r--r--   0        0        0      238 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/src/crowsetta/data/audseq/citation.txt
--rw-r--r--   0        0        0   651901 2022-05-22 18:53:26.010027 crowsetta-5.0.0rc1/src/crowsetta/data/birdsongrec/Annotation.xml
--rw-r--r--   0        0        0        0 2022-05-22 18:53:26.010027 crowsetta-5.0.0rc1/src/crowsetta/data/birdsongrec/__init__.py
--rw-r--r--   0        0        0      172 2023-02-28 02:25:58.397961 crowsetta-5.0.0rc1/src/crowsetta/data/birdsongrec/citation.txt
--rw-r--r--   0        0        0    10424 2023-03-01 17:08:05.263918 crowsetta-5.0.0rc1/src/crowsetta/data/data.py
--rw-r--r--   0        0        0        0 2022-05-22 18:53:26.010027 crowsetta-5.0.0rc1/src/crowsetta/data/generic/__init__.py
--rw-r--r--   0        0        0        5 2022-05-22 18:53:26.010027 crowsetta-5.0.0rc1/src/crowsetta/data/generic/citation.txt
--rw-r--r--   0        0        0    19451 2022-05-22 18:53:26.010027 crowsetta-5.0.0rc1/src/crowsetta/data/generic/example_custom_format.csv
--rw-r--r--   0        0        0        0 2022-05-22 18:53:26.010027 crowsetta-5.0.0rc1/src/crowsetta/data/notmat/__init__.py
--rw-r--r--   0        0        0      161 2023-02-28 02:25:58.397961 crowsetta-5.0.0rc1/src/crowsetta/data/notmat/citation.txt
--rw-r--r--   0        0        0     2154 2022-05-22 18:53:26.010027 crowsetta-5.0.0rc1/src/crowsetta/data/notmat/gy6or6_baseline_230312_0808.138.cbin.not.mat
--rw-r--r--   0        0        0      482 2022-05-22 18:53:26.010027 crowsetta-5.0.0rc1/src/crowsetta/data/raven/Recording_1_Segment_02.Table.1.selections.txt
--rw-r--r--   0        0        0        0 2022-05-22 18:53:26.010027 crowsetta-5.0.0rc1/src/crowsetta/data/raven/__init__.py
--rw-r--r--   0        0        0      257 2023-02-28 02:25:58.397961 crowsetta-5.0.0rc1/src/crowsetta/data/raven/citation.txt
--rw-r--r--   0        0        0        0 2022-05-22 18:53:26.010027 crowsetta-5.0.0rc1/src/crowsetta/data/simple/__init__.py
--rw-r--r--   0        0        0     2341 2022-05-22 18:53:26.010027 crowsetta-5.0.0rc1/src/crowsetta/data/simple/bl26lb16_190412_0721.20144_annotations.csv
--rw-r--r--   0        0        0      194 2023-02-28 02:25:58.397961 crowsetta-5.0.0rc1/src/crowsetta/data/simple/citation.txt
--rw-r--r--   0        0        0    18463 2023-02-28 02:25:58.397961 crowsetta-5.0.0rc1/src/crowsetta/data/textgrid/1179.TextGrid
--rw-r--r--   0        0        0        0 2022-05-22 18:53:26.010027 crowsetta-5.0.0rc1/src/crowsetta/data/textgrid/__init__.py
--rw-r--r--   0        0        0      233 2023-02-28 02:25:58.397961 crowsetta-5.0.0rc1/src/crowsetta/data/textgrid/citation.txt
--rw-r--r--   0        0        0        0 2022-05-22 18:53:26.010027 crowsetta-5.0.0rc1/src/crowsetta/data/timit/__init__.py
--rw-r--r--   0        0        0      173 2023-02-28 02:25:58.397961 crowsetta-5.0.0rc1/src/crowsetta/data/timit/citation.txt
--rwxr-xr-x   0        0        0      542 2022-05-22 18:53:26.010027 crowsetta-5.0.0rc1/src/crowsetta/data/timit/sa1.phn
--rw-r--r--   0        0        0     2631 2023-03-01 17:08:05.263918 crowsetta-5.0.0rc1/src/crowsetta/formats/__init__.py
--rw-r--r--   0        0        0       97 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/src/crowsetta/formats/bbox/__init__.py
--rw-r--r--   0        0        0     8045 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/src/crowsetta/formats/bbox/audbbox.py
--rw-r--r--   0        0        0     5935 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/src/crowsetta/formats/bbox/raven.py
--rw-r--r--   0        0        0      398 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/src/crowsetta/formats/seq/__init__.py
--rw-r--r--   0        0        0     7753 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/src/crowsetta/formats/seq/audseq.py
--rw-r--r--   0        0        0    12711 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/formats/seq/birdsongrec.py
--rw-r--r--   0        0        0    14505 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/formats/seq/generic.py
--rw-r--r--   0        0        0     9478 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/formats/seq/notmat.py
--rw-r--r--   0        0        0    11167 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/formats/seq/simple.py
--rw-r--r--   0        0        0     7262 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/formats/seq/textgrid.py
--rw-r--r--   0        0        0     9960 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/formats/seq/timit.py
--rw-r--r--   0        0        0     7749 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/formats/seq/yarden.py
--rw-r--r--   0        0        0      286 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/interface/__init__.py
--rw-r--r--   0        0        0      935 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/interface/base.py
--rw-r--r--   0        0        0       58 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/src/crowsetta/interface/bbox/__init__.py
--rw-r--r--   0        0        0     1636 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/interface/bbox/base.py
--rw-r--r--   0        0        0       56 2023-03-01 15:27:43.610627 crowsetta-5.0.0rc1/src/crowsetta/interface/seq/__init__.py
--rw-r--r--   0        0        0     1826 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/interface/seq/base.py
--rw-r--r--   0        0        0     3193 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/segment.py
--rw-r--r--   0        0        0    18494 2023-03-01 17:08:05.263918 crowsetta-5.0.0rc1/src/crowsetta/sequence.py
--rw-r--r--   0        0        0     3540 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/transcriber.py
--rw-r--r--   0        0        0      167 2022-06-17 12:22:33.200304 crowsetta-5.0.0rc1/src/crowsetta/typing.py
--rw-r--r--   0        0        0     3508 2023-02-28 03:20:43.055389 crowsetta-5.0.0rc1/src/crowsetta/validation.py
--rw-r--r--   0        0        0       24 2021-12-01 22:40:47.771260 crowsetta-5.0.0rc1/tests/__init__.py
--rw-r--r--   0        0        0      174 2022-05-22 18:53:26.014026 crowsetta-5.0.0rc1/tests/conftest.py
--rw-r--r--   0        0        0      345 2023-03-01 15:27:43.622627 crowsetta-5.0.0rc1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      270 2023-03-01 15:27:43.622627 crowsetta-5.0.0rc1/tests/fixtures/audbbox.py
--rw-r--r--   0        0        0      314 2023-03-01 15:27:43.622627 crowsetta-5.0.0rc1/tests/fixtures/audseq.py
--rw-r--r--   0        0        0      556 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/fixtures/bbox.py
--rw-r--r--   0        0        0      579 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/fixtures/birdsongrec.py
--rw-r--r--   0        0        0     1953 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/fixtures/csv.py
--rw-r--r--   0        0        0      254 2022-05-14 19:55:15.447898 crowsetta-5.0.0rc1/tests/fixtures/data.py
--rw-r--r--   0        0        0      406 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/fixtures/example_user_format.py
--rw-r--r--   0        0        0      490 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/fixtures/notmat.py
--rw-r--r--   0        0        0      884 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/fixtures/raven.py
--rw-r--r--   0        0        0      938 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/fixtures/segment.py
--rw-r--r--   0        0        0     1324 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/fixtures/sequence.py
--rw-r--r--   0        0        0      530 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/fixtures/simple.py
--rw-r--r--   0        0        0      283 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/fixtures/textgrid.py
--rw-r--r--   0        0        0     1491 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/fixtures/timit.py
--rw-r--r--   0        0        0      167 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/fixtures/yarden.py
--rw-r--r--   0        0        0       23 2021-12-01 22:40:49.867233 crowsetta-5.0.0rc1/tests/helpers/__init__.py
--rw-r--r--   0        0        0      603 2022-05-22 18:53:26.050027 crowsetta-5.0.0rc1/tests/helpers/keywords.py
--rw-r--r--   0        0        0     4806 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/scripts/remake_test_csv.py
--rw-r--r--   0        0        0     2194 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/test_annotation.py
--rw-r--r--   0        0        0     1798 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/test_bbox.py
--rw-r--r--   0        0        0     9566 2023-03-01 15:27:43.622627 crowsetta-5.0.0rc1/tests/test_data.py
--rw-r--r--   0        0        0        0 2022-05-14 19:55:15.447898 crowsetta-5.0.0rc1/tests/test_formats/__init__.py
--rw-r--r--   0        0        0        0 2022-05-14 19:55:15.447898 crowsetta-5.0.0rc1/tests/test_formats/test_bbox/__init__.py
--rw-r--r--   0        0        0     4160 2023-03-01 15:27:43.622627 crowsetta-5.0.0rc1/tests/test_formats/test_bbox/test_audbbox.py
--rw-r--r--   0        0        0     2744 2023-03-01 15:27:43.622627 crowsetta-5.0.0rc1/tests/test_formats/test_bbox/test_raven.py
--rw-r--r--   0        0        0     1793 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/test_formats/test_formats.py
--rw-r--r--   0        0        0        0 2022-05-14 19:55:15.447898 crowsetta-5.0.0rc1/tests/test_formats/test_seq/__init__.py
--rw-r--r--   0        0        0      200 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/test_formats/test_seq/asserts.py
--rw-r--r--   0        0        0     3579 2023-03-01 15:27:43.622627 crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_audseq.py
--rw-r--r--   0        0        0     7271 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_birdsongrec.py
--rw-r--r--   0        0        0    24465 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_generic.py
--rw-r--r--   0        0        0     3897 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_notmat.py
--rw-r--r--   0        0        0     3940 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_simple.py
--rw-r--r--   0        0        0     3065 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_textgrid.py
--rw-r--r--   0        0        0     1937 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_timit.py
--rw-r--r--   0        0        0     3485 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_yarden.py
--rw-r--r--   0        0        0     2388 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/test_segment.py
--rw-r--r--   0        0        0     7325 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/test_sequence.py
--rw-r--r--   0        0        0     3180 2023-03-01 15:27:43.622627 crowsetta-5.0.0rc1/tests/test_transcriber.py
--rw-r--r--   0        0        0      931 2023-02-28 03:20:43.059389 crowsetta-5.0.0rc1/tests/test_validation.py
--rw-r--r--   0        0        0    11470 1970-01-01 00:00:00.000000 crowsetta-5.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      815 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.all-contributorsrc
+-rw-r--r--   0        0        0     1311 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      248 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      615 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      749 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      823 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      356 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.gitignore
+-rw-r--r--   0        0        0     1089 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      366 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/.readthedocs.yaml
+-rw-r--r--   0        0        0      746 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/CITATION.cff
+-rw-r--r--   0        0        0     5556 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1879 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1515 2020-11-08 19:17:24.773706 crowsetta-5.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     8972 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/README.md
+-rw-r--r--   0        0        0    21762 2023-03-06 15:41:14.149711 crowsetta-5.0.0rc2/doc/CHANGELOG.md
+-rw-r--r--   0        0        0      580 2023-02-28 02:25:58.381961 crowsetta-5.0.0rc2/doc/Makefile
+-rw-r--r--   0        0        0    26325 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/doc/_static/crowsetta-logomark.png
+-rw-r--r--   0        0        0   250992 2023-03-06 13:01:07.250070 crowsetta-5.0.0rc2/doc/_static/crowsetta-primary-logo.png
+-rw-r--r--   0        0        0    83463 2023-03-06 13:01:07.254070 crowsetta-5.0.0rc2/doc/_static/crowsetta-secondary-logo.png
+-rw-r--r--   0        0        0  1638145 2023-03-06 13:01:07.258070 crowsetta-5.0.0rc2/doc/_static/example-raven-for-index.png
+-rw-r--r--   0        0        0   640083 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/_static/example-textgrid-for-index.png
+-rw-r--r--   0        0        0      612 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/_templates/class.rst
+-rw-r--r--   0        0        0     1177 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/_templates/module.rst
+-rw-r--r--   0        0        0     1857 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/api/core.md
+-rw-r--r--   0        0        0      409 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/api/formats.md
+-rw-r--r--   0        0        0      581 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/api/index.md
+-rw-r--r--   0        0        0      565 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/api/interface.md
+-rw-r--r--   0        0        0     6936 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/conf.py
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/data/.gitkeep
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/data/giraudon-et-al-2021/.gitkeep
+-rw-r--r--   0        0        0      446 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/development/commit-abbreviations.rst
+-rw-r--r--   0        0        0     8631 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/development/contributors.md
+-rw-r--r--   0        0        0     1024 2023-03-06 13:01:07.262070 crowsetta-5.0.0rc2/doc/development/index.md
+-rw-r--r--   0        0        0      741 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/bbox/raven.md
+-rw-r--r--   0        0        0     1556 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/index.md
+-rw-r--r--   0        0        0     1092 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/seq/aud-seq.md
+-rw-r--r--   0        0        0     1179 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/seq/birdsongrec.md
+-rw-r--r--   0        0        0     1268 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/seq/generic-seq.md
+-rw-r--r--   0        0        0      783 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/seq/notmat.md
+-rw-r--r--   0        0        0     1294 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/seq/simple-seq.md
+-rw-r--r--   0        0        0      717 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/seq/textgrid.md
+-rw-r--r--   0        0        0      739 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/formats/seq/timit.md
+-rw-r--r--   0        0        0      231 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto.md
+-rw-r--r--   0        0        0     7488 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto/bat1_annotation.mat
+-rw-r--r--   0        0        0     4503 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto/batlab.py
+-rw-r--r--   0        0        0     7256 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto/convert-generic-seq.md
+-rw-r--r--   0        0        0     9563 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto/convert-simple-seq.md
+-rw-r--r--   0        0        0    26382 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto/howto-user-format.md
+-rw-r--r--   0        0        0     2265 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto/parsebat.py
+-rw-r--r--   0        0        0    29107 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/howto/remove-silent-labels-textgrid.md
+-rw-r--r--   0        0        0    12885 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/index.md
+-rw-r--r--   0        0        0      752 2020-11-08 19:17:24.773706 crowsetta-5.0.0rc2/doc/make.bat
+-rw-r--r--   0        0        0      881 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/nitpick-ignore.txt
+-rw-r--r--   0        0        0    19417 2023-03-06 13:01:07.266070 crowsetta-5.0.0rc2/doc/scripts/annot/Recording_1_Segment_07.Table.1.selections.txt
+-rw-r--r--   0        0        0  2942427 2023-03-06 13:01:07.270070 crowsetta-5.0.0rc2/doc/scripts/annot/b06_concat_dtw.TextGrid
+-rw-r--r--   0        0        0   640046 2023-03-06 13:01:07.274070 crowsetta-5.0.0rc2/doc/scripts/audio/Recording_1_Segment_07-snippet.wav
+-rw-r--r--   0        0        0   150046 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/doc/scripts/audio/b06_concat-snippet.wav
+-rw-r--r--   0        0        0     3885 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/doc/scripts/raven-chronister-et-al-2021.md
+-rw-r--r--   0        0        0     5966 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/doc/scripts/textgrid-BF-dataset.md
+-rw-r--r--   0        0        0    10627 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/doc/tutorial.md
+-rw-r--r--   0        0        0     2927 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/noxfile.py
+-rw-r--r--   0        0        0     1969 2023-03-06 16:53:57.406967 crowsetta-5.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      846 2023-03-06 16:53:57.394967 crowsetta-5.0.0rc2/src/crowsetta/__about__.py
+-rw-r--r--   0        0        0      882 2023-03-06 16:27:50.541769 crowsetta-5.0.0rc2/src/crowsetta/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/_vendor/__init__.py
+-rw-r--r--   0        0        0      379 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/AUTHORS
+-rw-r--r--   0        0        0     1090 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/LICENSE
+-rw-r--r--   0        0        0      723 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/README.md
+-rw-r--r--   0        0        0       78 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/__init__.py
+-rw-r--r--   0        0        0       41 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/exceptions.py
+-rw-r--r--   0        0        0    32141 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/textgrid.py
+-rw-r--r--   0        0        0     4559 2023-03-06 16:45:20.193235 crowsetta-5.0.0rc2/src/crowsetta/annotation.py
+-rw-r--r--   0        0        0     2406 2023-03-06 16:50:53.755772 crowsetta-5.0.0rc2/src/crowsetta/bbox.py
+-rw-r--r--   0        0        0      469 2023-03-06 16:27:50.537769 crowsetta-5.0.0rc2/src/crowsetta/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/data/audbbox/__init__.py
+-rw-r--r--   0        0        0      153 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/data/audbbox/citation.txt
+-rw-r--r--   0        0        0      887 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/data/audbbox/spinetail.txt
+-rw-r--r--   0        0        0     1828 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/data/audseq/405_marron1_June_14_2016_69640887.audacity.txt
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/data/audseq/__init__.py
+-rw-r--r--   0        0        0      238 2023-03-06 13:01:07.278070 crowsetta-5.0.0rc2/src/crowsetta/data/audseq/citation.txt
+-rw-r--r--   0        0        0   651901 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/birdsongrec/Annotation.xml
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/birdsongrec/__init__.py
+-rw-r--r--   0        0        0      172 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/birdsongrec/citation.txt
+-rw-r--r--   0        0        0    10424 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/data.py
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/generic/__init__.py
+-rw-r--r--   0        0        0        5 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/generic/citation.txt
+-rw-r--r--   0        0        0    19451 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/generic/example_custom_format.csv
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/notmat/__init__.py
+-rw-r--r--   0        0        0      161 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/notmat/citation.txt
+-rw-r--r--   0        0        0     2154 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/notmat/gy6or6_baseline_230312_0808.138.cbin.not.mat
+-rw-r--r--   0        0        0      482 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/raven/Recording_1_Segment_02.Table.1.selections.txt
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/raven/__init__.py
+-rw-r--r--   0        0        0      257 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/raven/citation.txt
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/simple/__init__.py
+-rw-r--r--   0        0        0     2341 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/simple/bl26lb16_190412_0721.20144_annotations.csv
+-rw-r--r--   0        0        0      194 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/simple/citation.txt
+-rw-r--r--   0        0        0    18463 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/textgrid/1179.TextGrid
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/textgrid/__init__.py
+-rw-r--r--   0        0        0      233 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/textgrid/citation.txt
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/timit/__init__.py
+-rw-r--r--   0        0        0      173 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/timit/citation.txt
+-rwxr-xr-x   0        0        0      542 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/data/timit/sa1.phn
+-rw-r--r--   0        0        0     2631 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/__init__.py
+-rw-r--r--   0        0        0       97 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/bbox/__init__.py
+-rw-r--r--   0        0        0     8045 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/bbox/audbbox.py
+-rw-r--r--   0        0        0     5935 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/bbox/raven.py
+-rw-r--r--   0        0        0      398 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/__init__.py
+-rw-r--r--   0        0        0     7753 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/audseq.py
+-rw-r--r--   0        0        0    12711 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/birdsongrec.py
+-rw-r--r--   0        0        0    14505 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/generic.py
+-rw-r--r--   0        0        0     9478 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/notmat.py
+-rw-r--r--   0        0        0    11167 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/simple.py
+-rw-r--r--   0        0        0     7262 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/textgrid.py
+-rw-r--r--   0        0        0     9960 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/timit.py
+-rw-r--r--   0        0        0     7749 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/formats/seq/yarden.py
+-rw-r--r--   0        0        0      286 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/interface/__init__.py
+-rw-r--r--   0        0        0      935 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/interface/base.py
+-rw-r--r--   0        0        0       58 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/interface/bbox/__init__.py
+-rw-r--r--   0        0        0     1636 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/interface/bbox/base.py
+-rw-r--r--   0        0        0       56 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/interface/seq/__init__.py
+-rw-r--r--   0        0        0     1800 2023-03-06 16:45:20.193235 crowsetta-5.0.0rc2/src/crowsetta/interface/seq/base.py
+-rw-r--r--   0        0        0     4123 2023-03-06 16:45:20.193235 crowsetta-5.0.0rc2/src/crowsetta/segment.py
+-rw-r--r--   0        0        0    18671 2023-03-06 16:45:20.193235 crowsetta-5.0.0rc2/src/crowsetta/sequence.py
+-rw-r--r--   0        0        0     7288 2023-03-06 16:45:20.193235 crowsetta-5.0.0rc2/src/crowsetta/transcriber.py
+-rw-r--r--   0        0        0      167 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/typing.py
+-rw-r--r--   0        0        0     3508 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/src/crowsetta/validation.py
+-rw-r--r--   0        0        0       24 2021-12-01 22:40:47.771260 crowsetta-5.0.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0      174 2023-03-06 13:01:07.282070 crowsetta-5.0.0rc2/tests/conftest.py
+-rw-r--r--   0        0        0      345 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      270 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/audbbox.py
+-rw-r--r--   0        0        0      314 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/audseq.py
+-rw-r--r--   0        0        0      556 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/bbox.py
+-rw-r--r--   0        0        0      579 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/birdsongrec.py
+-rw-r--r--   0        0        0     1953 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/csv.py
+-rw-r--r--   0        0        0      254 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/data.py
+-rw-r--r--   0        0        0      406 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/example_user_format.py
+-rw-r--r--   0        0        0      490 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/notmat.py
+-rw-r--r--   0        0        0      884 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/raven.py
+-rw-r--r--   0        0        0      912 2023-03-06 16:45:20.193235 crowsetta-5.0.0rc2/tests/fixtures/segment.py
+-rw-r--r--   0        0        0     1324 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/sequence.py
+-rw-r--r--   0        0        0      530 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/simple.py
+-rw-r--r--   0        0        0      283 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/textgrid.py
+-rw-r--r--   0        0        0     1491 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/timit.py
+-rw-r--r--   0        0        0      167 2023-03-06 13:01:07.782067 crowsetta-5.0.0rc2/tests/fixtures/yarden.py
+-rw-r--r--   0        0        0       23 2021-12-01 22:40:49.867233 crowsetta-5.0.0rc2/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      603 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/helpers/keywords.py
+-rw-r--r--   0        0        0     4806 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/scripts/remake_test_csv.py
+-rw-r--r--   0        0        0     2194 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_annotation.py
+-rw-r--r--   0        0        0     1798 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_bbox.py
+-rw-r--r--   0        0        0     9566 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_data.py
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_bbox/__init__.py
+-rw-r--r--   0        0        0     4160 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_bbox/test_audbbox.py
+-rw-r--r--   0        0        0     2744 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_bbox/test_raven.py
+-rw-r--r--   0        0        0     1793 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_formats.py
+-rw-r--r--   0        0        0        0 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/__init__.py
+-rw-r--r--   0        0        0      200 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/asserts.py
+-rw-r--r--   0        0        0     3579 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_audseq.py
+-rw-r--r--   0        0        0     7271 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_birdsongrec.py
+-rw-r--r--   0        0        0    24465 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_generic.py
+-rw-r--r--   0        0        0     3897 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_notmat.py
+-rw-r--r--   0        0        0     3940 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_simple.py
+-rw-r--r--   0        0        0     3065 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_textgrid.py
+-rw-r--r--   0        0        0     1937 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_timit.py
+-rw-r--r--   0        0        0     3485 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_yarden.py
+-rw-r--r--   0        0        0     1250 2023-03-06 16:45:20.193235 crowsetta-5.0.0rc2/tests/test_segment.py
+-rw-r--r--   0        0        0     7325 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_sequence.py
+-rw-r--r--   0        0        0     3180 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_transcriber.py
+-rw-r--r--   0        0        0      931 2023-03-06 13:01:07.786067 crowsetta-5.0.0rc2/tests/test_validation.py
+-rw-r--r--   0        0        0    11470 1970-01-01 00:00:00.000000 crowsetta-5.0.0rc2/PKG-INFO
```

### Comparing `crowsetta-5.0.0rc1/.all-contributorsrc` & `crowsetta-5.0.0rc2/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.md` & `crowsetta-5.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/.github/ISSUE_TEMPLATE/feature_request.md` & `crowsetta-5.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/.github/workflows/ci.yml` & `crowsetta-5.0.0rc2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/.github/workflows/lint.yml` & `crowsetta-5.0.0rc2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/.pre-commit-config.yaml` & `crowsetta-5.0.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/CITATION.cff` & `crowsetta-5.0.0rc2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/CODE_OF_CONDUCT.md` & `crowsetta-5.0.0rc2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/CONTRIBUTING.md` & `crowsetta-5.0.0rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/LICENSE` & `crowsetta-5.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/README.md` & `crowsetta-5.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/CHANGELOG.md` & `crowsetta-5.0.0rc2/doc/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
-## Added
+### Added
 - Add information on contributing and setting up a development environment
   [#212](https://github.com/NickleDave/crowsetta/pull/212).
   Fixes [#30](https://github.com/NickleDave/crowsetta/issues/30).
 - Add method to convert generic sequence format to a pandas DataFrame
   [#216](https://github.com/NickleDave/crowsetta/pull/216).
 - Add additional vignettes to docs:
   on removing "silent" labels from TextGrid annotations,
@@ -18,15 +18,20 @@
   Fixes [#152](https://github.com/NickleDave/crowsetta/issues/152)
   and [#197](https://github.com/NickleDave/crowsetta/issues/197).
 - Add format class for Audacity extended label track format
   [#226](https://github.com/NickleDave/crowsetta/pull/226).
   Fixes [#222](https://github.com/NickleDave/crowsetta/issues/222)
   and [#213](https://github.com/NickleDave/crowsetta/issues/213).
 
-## Fixed
+### Removed
+- Remove `Segment.from_row` method, no longer used
+  [#232](https://github.com/NickleDave/crowsetta/pull/232).
+  Fixes [#231](https://github.com/NickleDave/crowsetta/issues/231)
+
+### Fixed
 - Revise landing page of docs, and some vignettes. 
   Make other changes to clean up the docs build process 
   [#216](https://github.com/NickleDave/crowsetta/pull/216).
 
 ## 4.0.0.post2 -- 2022-06-25
 ### Changed
 - [c6ba100](https://github.com/vocalpy/crowsetta/commit/c6ba100d7335a880f2e1dbf66f5673ef562f3cc5)
```

### Comparing `crowsetta-5.0.0rc1/doc/Makefile` & `crowsetta-5.0.0rc2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/_static/crowsetta-logomark.png` & `crowsetta-5.0.0rc2/doc/_static/crowsetta-logomark.png`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/_static/crowsetta-primary-logo.png` & `crowsetta-5.0.0rc2/doc/_static/crowsetta-primary-logo.png`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/_static/crowsetta-secondary-logo.png` & `crowsetta-5.0.0rc2/doc/_static/crowsetta-secondary-logo.png`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/_static/example-raven-for-index.png` & `crowsetta-5.0.0rc2/doc/_static/example-raven-for-index.png`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/_static/example-textgrid-for-index.png` & `crowsetta-5.0.0rc2/doc/_static/example-textgrid-for-index.png`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/_templates/class.rst` & `crowsetta-5.0.0rc2/doc/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/_templates/module.rst` & `crowsetta-5.0.0rc2/doc/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/api/core.md` & `crowsetta-5.0.0rc2/doc/api/core.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/api/index.md` & `crowsetta-5.0.0rc2/doc/api/index.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/api/interface.md` & `crowsetta-5.0.0rc2/doc/api/interface.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/conf.py` & `crowsetta-5.0.0rc2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/development/contributors.md` & `crowsetta-5.0.0rc2/doc/development/contributors.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/development/index.md` & `crowsetta-5.0.0rc2/doc/development/index.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/formats/bbox/raven.md` & `crowsetta-5.0.0rc2/doc/formats/bbox/raven.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/formats/index.md` & `crowsetta-5.0.0rc2/doc/formats/index.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/formats/seq/aud-seq.md` & `crowsetta-5.0.0rc2/doc/formats/seq/aud-seq.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/formats/seq/birdsongrec.md` & `crowsetta-5.0.0rc2/doc/formats/seq/birdsongrec.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/formats/seq/generic-seq.md` & `crowsetta-5.0.0rc2/doc/formats/seq/generic-seq.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/formats/seq/notmat.md` & `crowsetta-5.0.0rc2/doc/formats/seq/notmat.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/formats/seq/simple-seq.md` & `crowsetta-5.0.0rc2/doc/formats/seq/simple-seq.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/formats/seq/textgrid.md` & `crowsetta-5.0.0rc2/doc/formats/seq/textgrid.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/formats/seq/timit.md` & `crowsetta-5.0.0rc2/doc/formats/seq/timit.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/howto/bat1_annotation.mat` & `crowsetta-5.0.0rc2/doc/howto/bat1_annotation.mat`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/howto/batlab.py` & `crowsetta-5.0.0rc2/doc/howto/batlab.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/howto/convert-generic-seq.md` & `crowsetta-5.0.0rc2/doc/howto/convert-generic-seq.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/howto/convert-simple-seq.md` & `crowsetta-5.0.0rc2/doc/howto/convert-simple-seq.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/howto/howto-user-format.md` & `crowsetta-5.0.0rc2/doc/howto/howto-user-format.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/howto/parsebat.py` & `crowsetta-5.0.0rc2/doc/howto/parsebat.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/howto/remove-silent-labels-textgrid.md` & `crowsetta-5.0.0rc2/doc/howto/remove-silent-labels-textgrid.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/index.md` & `crowsetta-5.0.0rc2/doc/index.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/make.bat` & `crowsetta-5.0.0rc2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/nitpick-ignore.txt` & `crowsetta-5.0.0rc2/doc/nitpick-ignore.txt`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/scripts/annot/Recording_1_Segment_07.Table.1.selections.txt` & `crowsetta-5.0.0rc2/doc/scripts/annot/Recording_1_Segment_07.Table.1.selections.txt`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/scripts/annot/b06_concat_dtw.TextGrid` & `crowsetta-5.0.0rc2/doc/scripts/annot/b06_concat_dtw.TextGrid`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/scripts/audio/Recording_1_Segment_07-snippet.wav` & `crowsetta-5.0.0rc2/doc/scripts/audio/Recording_1_Segment_07-snippet.wav`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/scripts/audio/b06_concat-snippet.wav` & `crowsetta-5.0.0rc2/doc/scripts/audio/b06_concat-snippet.wav`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/scripts/raven-chronister-et-al-2021.md` & `crowsetta-5.0.0rc2/doc/scripts/raven-chronister-et-al-2021.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/scripts/textgrid-BF-dataset.md` & `crowsetta-5.0.0rc2/doc/scripts/textgrid-BF-dataset.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/doc/tutorial.md` & `crowsetta-5.0.0rc2/doc/tutorial.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/noxfile.py` & `crowsetta-5.0.0rc2/noxfile.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/pyproject.toml` & `crowsetta-5.0.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "importlib-resources >=5.7.1",
     "numpy >=1.18.1",
     "pandas >= 1.3.5",
     "pandera >= 0.9.0",
     "scipy >=1.4.1",
     "SoundFile >=0.10.3",
 ]
-version = "5.0.0rc1"
+version = "5.0.0rc2"
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     'License :: OSI Approved :: BSD License',
     'Development Status :: 5 - Production/Stable',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
```

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/__about__.py` & `crowsetta-5.0.0rc2/src/crowsetta/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     base_dir = None
 
 
 __title__ = "crowsetta"
 __summary__ = "A Python tool to work with any format for annotating animal vocalizations and bioacoustics data"
 __uri__ = "https://github.com/vocalpy/crowsetta"
 
-__version__ = "5.0.0rc1"
+__version__ = "5.0.0rc2"
 
 if base_dir is not None and os.path.exists(os.path.join(base_dir, ".commit")):
     with open(os.path.join(base_dir, ".commit")) as fp:
         __commit__ = fp.read().strip()
 else:
     __commit__ = None
```

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/__init__.py` & `crowsetta-5.0.0rc2/src/crowsetta/__init__.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/_vendor/textgrid/LICENSE` & `crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/LICENSE`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/_vendor/textgrid/README.md` & `crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/README.md`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/_vendor/textgrid/textgrid.py` & `crowsetta-5.0.0rc2/src/crowsetta/_vendor/textgrid/textgrid.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/bbox.py` & `crowsetta-5.0.0rc2/src/crowsetta/bbox.py`

 * *Files 25% similar despite different names*

```diff
@@ -25,14 +25,26 @@
         Time of sound offset, typically in seconds.
     low_freq : float
         Lowest frequency bounding sound, typically in Hz.
     high_freq : float
         Highest frequency bounding sound, typically in Hz.
     label : str
         string label that annotates bounding box
+
+    Examples
+    --------
+
+    A toy example of a bounding box-like annotation.
+
+    >>> bbox1 = crowsetta.BBox(label='Pinacosaurus grangeri', onset=1.0, offset=2.0, low_freq=3e3, high_freq=1e4)
+    >>> bbox2 = crowsetta.BBox(label='Pinacosaurus grangeri', onset=3.0, offset=4.0, low_freq=3.25e3, high_freq=1.25e4)
+    >>> bboxes = [bbox1, bbox2]
+    >>> annot = crowsetta.Annotation(notated_path='prebird1.wav', annot_path='prebird1.csv', bboxes=bboxes)
+    >>> print(annot)
+    Annotation(annot_path=PosixPath('prebird1.csv'), notated_path=PosixPath('prebird1.wav'), bboxes=[BBox(onset=1.0, offset=2.0, low_freq=3000.0, high_freq=10000.0, label='Pinacosaurus grangeri'), BBox(onset=3.0, offset=4.0, low_freq=3250.0, high_freq=12500.0, label='Pinacosaurus grangeri')])  # noqa
     """
 
     onset: float = field(validator=is_positive)
 
     @onset.validator
     def lt_offset(self, attribute, value):
         if not value < self.offset:
```

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/data/audbbox/spinetail.txt` & `crowsetta-5.0.0rc2/src/crowsetta/data/audbbox/spinetail.txt`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/data/audseq/405_marron1_June_14_2016_69640887.audacity.txt` & `crowsetta-5.0.0rc2/src/crowsetta/data/audseq/405_marron1_June_14_2016_69640887.audacity.txt`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/data/birdsongrec/Annotation.xml` & `crowsetta-5.0.0rc2/src/crowsetta/data/birdsongrec/Annotation.xml`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/data/data.py` & `crowsetta-5.0.0rc2/src/crowsetta/data/data.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/data/generic/example_custom_format.csv` & `crowsetta-5.0.0rc2/src/crowsetta/data/generic/example_custom_format.csv`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/data/notmat/gy6or6_baseline_230312_0808.138.cbin.not.mat` & `crowsetta-5.0.0rc2/src/crowsetta/data/notmat/gy6or6_baseline_230312_0808.138.cbin.not.mat`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/data/simple/bl26lb16_190412_0721.20144_annotations.csv` & `crowsetta-5.0.0rc2/src/crowsetta/data/simple/bl26lb16_190412_0721.20144_annotations.csv`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/data/textgrid/1179.TextGrid` & `crowsetta-5.0.0rc2/src/crowsetta/data/textgrid/1179.TextGrid`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/data/timit/sa1.phn` & `crowsetta-5.0.0rc2/src/crowsetta/data/timit/sa1.phn`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/formats/__init__.py` & `crowsetta-5.0.0rc2/src/crowsetta/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/formats/bbox/audbbox.py` & `crowsetta-5.0.0rc2/src/crowsetta/formats/bbox/audbbox.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/formats/bbox/raven.py` & `crowsetta-5.0.0rc2/src/crowsetta/formats/bbox/raven.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/formats/seq/audseq.py` & `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/audseq.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/formats/seq/birdsongrec.py` & `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/birdsongrec.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/formats/seq/generic.py` & `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/generic.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/formats/seq/notmat.py` & `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/notmat.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/formats/seq/simple.py` & `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/simple.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/formats/seq/textgrid.py` & `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/textgrid.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/formats/seq/timit.py` & `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/timit.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/formats/seq/yarden.py` & `crowsetta-5.0.0rc2/src/crowsetta/formats/seq/yarden.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/interface/base.py` & `crowsetta-5.0.0rc2/src/crowsetta/interface/base.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/interface/bbox/base.py` & `crowsetta-5.0.0rc2/src/crowsetta/interface/bbox/base.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/interface/seq/base.py` & `crowsetta-5.0.0rc2/src/crowsetta/interface/seq/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,20 @@
     that can be represented as a
     ``crowsetta.Sequence`` made up of ``crowsetta.Segment``s.
     The code block below shows some of the features of these data types.
 
     .. code-block:: python
 
        >>> from crowsetta import Segment, Sequence
-       >>> a_segment = Segment.from_keyword(
+       >>> a_segment = Segment(
        ...     label='a',
        ...     onset_sample=16000,
        ...     offset_sample=32000,
        ...     )
-       >>> another_segment = Segment.from_keyword(
+       >>> another_segment = Segment(
        ...     label='b',
        ...     onset_sample=36000,
        ...     offset_sample=48000,
        ...     )
        >>> list_of_segments = [a_segment, another_segment]
        >>> seq = Sequence.from_segments(segments=list_of_segments)
        >>> print(seq)
```

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/sequence.py` & `crowsetta-5.0.0rc2/src/crowsetta/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,21 +36,27 @@
     from_keyword : make a Sequence by passing keywords (all arguments except segments)
     from_dict : like from_keyword, but pass a Python dictionary where keys are keywords
         and values are arguments for those keywords
     to_dict : convert to a dict. The inverse of from_dict.
 
     Examples
     --------
+
+    A sequence with onsets and offsets given in seconds.
+
     >>> import numpy as np
     >>> import crowsetta
     >>> onsets_s = np.array([1.0, 3.0, 5.0])
     >>> offsets_s = np.array(2.0, 4.0, 6.0])
     >>> labels = np.array(['a', 'a', 'b'])
     >>> seq = crowsetta.Sequence.from_keyword(labels=labels, onsets_s=onsets_s, offsets_s=offsets_s)
 
+    The same sequence could also be made with ``crowsetta.Segment`` instances,
+    by calling the ``from_segments`` class method.
+
     >>> segments = []
     >>> for onset, offset, label in zip(onsets_s, offsets_s, labels):
     ...     segments.append(crowsetta.Segment(onset_s=onset, offset_s=offset, label=label))
     >>> seq2 = crowsetta.Sequence.from_segments(segments)
     """
 
     def __init__(self, segments, labels, onsets_s=None, offsets_s=None, onset_samples=None, offset_samples=None):
@@ -373,15 +379,15 @@
             onsets_s, offsets_s, onset_samples, offset_samples, labels
         )
 
         segments = []
         zipped = zip(labels, onset_samples, offset_samples, onsets_s, offsets_s)
         for label, onset_sample, offset_sample, onset_s, offset_s in zipped:
             segments.append(
-                Segment.from_keyword(
+                Segment(
                     label=label,
                     onset_sample=onset_sample,
                     offset_sample=offset_sample,
                     onset_s=onset_s,
                     offset_s=offset_s,
                 )
             )
```

### Comparing `crowsetta-5.0.0rc1/src/crowsetta/validation.py` & `crowsetta-5.0.0rc2/src/crowsetta/validation.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/fixtures/bbox.py` & `crowsetta-5.0.0rc2/tests/fixtures/bbox.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/fixtures/birdsongrec.py` & `crowsetta-5.0.0rc2/tests/fixtures/birdsongrec.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/fixtures/csv.py` & `crowsetta-5.0.0rc2/tests/fixtures/csv.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/fixtures/raven.py` & `crowsetta-5.0.0rc2/tests/fixtures/raven.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/fixtures/segment.py` & `crowsetta-5.0.0rc2/tests/fixtures/segment.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @pytest.fixture
 def list_of_segments():
     list_of_segments = []
 
     for label, onset_sample, offset_sample in zip(("a", "b", "c"), (16000, 32000, 64000), (17000, 33000, 65000)):
         list_of_segments.append(
-            Segment.from_keyword(
+            Segment(
                 label=label,
                 onset_sample=onset_sample,
                 offset_sample=offset_sample,
             )
         )
 
     return list_of_segments
@@ -23,15 +23,15 @@
 def different_list_of_segments():
     list_of_segments = []
 
     for label, onset_sample, offset_sample in zip(
         ("a", "b", "c", "d"), (16000, 32000, 64000, 128000), (17100, 33100, 65100, 129100)
     ):
         list_of_segments.append(
-            Segment.from_keyword(
+            Segment(
                 label=label,
                 onset_sample=onset_sample,
                 offset_sample=offset_sample,
             )
         )
 
     return list_of_segments
```

### Comparing `crowsetta-5.0.0rc1/tests/fixtures/sequence.py` & `crowsetta-5.0.0rc2/tests/fixtures/sequence.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/fixtures/simple.py` & `crowsetta-5.0.0rc2/tests/fixtures/simple.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/fixtures/timit.py` & `crowsetta-5.0.0rc2/tests/fixtures/timit.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/helpers/keywords.py` & `crowsetta-5.0.0rc2/tests/helpers/keywords.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/scripts/remake_test_csv.py` & `crowsetta-5.0.0rc2/tests/scripts/remake_test_csv.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_annotation.py` & `crowsetta-5.0.0rc2/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_bbox.py` & `crowsetta-5.0.0rc2/tests/test_bbox.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_data.py` & `crowsetta-5.0.0rc2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_formats/test_bbox/test_audbbox.py` & `crowsetta-5.0.0rc2/tests/test_formats/test_bbox/test_audbbox.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_formats/test_bbox/test_raven.py` & `crowsetta-5.0.0rc2/tests/test_formats/test_bbox/test_raven.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_formats/test_formats.py` & `crowsetta-5.0.0rc2/tests/test_formats/test_formats.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_audseq.py` & `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_audseq.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_birdsongrec.py` & `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_birdsongrec.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_generic.py` & `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_generic.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_notmat.py` & `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_notmat.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_simple.py` & `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_simple.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_textgrid.py` & `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_textgrid.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_timit.py` & `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_timit.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_formats/test_seq/test_yarden.py` & `crowsetta-5.0.0rc2/tests/test_formats/test_seq/test_yarden.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_sequence.py` & `crowsetta-5.0.0rc2/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_transcriber.py` & `crowsetta-5.0.0rc2/tests/test_transcriber.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/tests/test_validation.py` & `crowsetta-5.0.0rc2/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `crowsetta-5.0.0rc1/PKG-INFO` & `crowsetta-5.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowsetta
-Version: 5.0.0rc1
+Version: 5.0.0rc2
 Summary: A Python tool to work with any format for annotating animal vocalizations and bioacoustics data
 Author-email: David Nicholson <nickledave@users.noreply.github.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

