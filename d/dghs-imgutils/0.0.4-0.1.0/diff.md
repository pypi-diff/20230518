# Comparing `tmp/dghs-imgutils-0.0.4.tar.gz` & `tmp/dghs-imgutils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dghs-imgutils-0.0.4.tar", last modified: Tue May 16 11:00:05 2023, max compression
+gzip compressed data, was "dghs-imgutils-0.1.0.tar", last modified: Thu May 18 08:52:53 2023, max compression
```

## Comparing `dghs-imgutils-0.0.4.tar` & `dghs-imgutils-0.1.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.634635 dghs-imgutils-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-16 11:00:05.634635 dghs-imgutils-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/dghs_imgutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-16 11:00:05.000000 dghs-imgutils-0.0.4/dghs_imgutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-16 11:00:05.000000 dghs-imgutils-0.0.4/dghs_imgutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:00:05.000000 dghs-imgutils-0.0.4/dghs_imgutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-16 11:00:05.000000 dghs-imgutils-0.0.4/dghs_imgutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 11:00:05.000000 dghs-imgutils-0.0.4/dghs_imgutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/data/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/data/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/data/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/data/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/data/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/detect/_yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/detect/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/detect/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/detect/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/edge/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/edge/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/edge/canny.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/edge/lineart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/edge/lineart_anime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/metrics/aesthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/metrics/lpips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/metrics/psnr_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/segment/isnetis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/tagging/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/tagging/deepdanbooru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/tagging/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/tagging/mldanbooru.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/tagging/wd14.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/utils/onnxruntime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.634635 dghs-imgutils-0.0.4/imgutils/validate/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/validate/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/validate/monochrome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/validate/truncate.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/requirements-zoo.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 11:00:05.634635 dghs-imgutils-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.610600 dghs-imgutils-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-18 08:51:55.000000 dghs-imgutils-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-18 08:51:55.000000 dghs-imgutils-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-18 08:51:55.000000 dghs-imgutils-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/dghs_imgutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-05-18 08:52:53.000000 dghs-imgutils-0.1.0/dghs_imgutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-18 08:52:53.000000 dghs-imgutils-0.1.0/dghs_imgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:52:53.000000 dghs-imgutils-0.1.0/dghs_imgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-18 08:52:53.000000 dghs-imgutils-0.1.0/dghs_imgutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 08:52:53.000000 dghs-imgutils-0.1.0/dghs_imgutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/data/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/data/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/data/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/data/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/detect/_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/detect/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/detect/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/detect/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/detect/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/edge/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/edge/canny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/edge/lineart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/edge/lineart_anime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/metrics/aesthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/metrics/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/metrics/psnr_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/segment/isnetis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/tagging/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/tagging/deepdanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/tagging/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/tagging/mldanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/tagging/wd14.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/utils/onnxruntime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:52:53.606600 dghs-imgutils-0.1.0/imgutils/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/validate/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/validate/monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/imgutils/validate/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/requirements-zoo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 08:52:53.610600 dghs-imgutils-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-18 08:51:56.000000 dghs-imgutils-0.1.0/setup.py
```

### Comparing `dghs-imgutils-0.0.4/LICENSE` & `dghs-imgutils-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.4/PKG-INFO` & `dghs-imgutils-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.0.4
+Version: 0.1.0
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -74,15 +74,15 @@
 * [Image Tagging](https://github.com/deepghs/imgutils#image-tagging)
 * [Character Extraction](https://github.com/deepghs/imgutils#character-extraction)
 
 ### Tachie(差分) Detection and Clustering
 
 For the dataset, we need to filter the differences between the tachie(差分). As shown in the following picture
 
-![tachie](https://deepghs.github.io/imgutils/main/_images/lpips_full.dat.svg)
+![tachie](https://deepghs.github.io/imgutils/main/_images/lpips_full.plot.py.svg)
 
 We can use `lpips_clustering` to cluster such situations as shown below
 
 ```python
 from imgutils.metrics import lpips_clustering
 
 images = [f'lpips/{i}.jpg' for i in range(1, 10)]
@@ -90,45 +90,45 @@
 # ['lpips/1.jpg', 'lpips/2.jpg', 'lpips/3.jpg', 'lpips/4.jpg', 'lpips/5.jpg', 'lpips/6.jpg', 'lpips/7.jpg', 'lpips/8.jpg', 'lpips/9.jpg']
 print(lpips_clustering(images))  # -1 means noises, the same as that in sklearn
 # [0, 0, 0, 1, 1, -1, -1, -1, -1]
 ```
 
 ### Object Detection
 
-Currently, object detection is supported for anime faces and person, as shown below
+Currently, object detection is supported for anime heads and person, as shown below
 
-* Face Detection
+* Head Detection
 
-![face detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/face_detect.dat.svg)
+![head detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/head_detect.plot.py.svg)
 
 * Person Detection
 
-![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect.dat.svg)
+![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect.plot.py.svg)
 
-Based on practical tests, face detection currently has a very stable performance and can be used for automation tasks.
+Based on practical tests, head detection currently has a very stable performance and can be used for automation tasks.
 However, person detection is still being further iterated and will focus on enhancing detection capabilities for
 artistic illustrations in the future.
 
 ### Edge Detection / Lineart Generation
 
 Anime images can be converted to line drawings using the model provided
 by [patrickvonplaten/controlnet_aux](https://github.com/patrickvonplaten/controlnet_aux), as shown below.
 
-![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge.dat.svg)
+![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge.plot.py.svg)
 
 It is worth noting that the `lineart` model may consume more computational resources, while `canny` is the fastest but
 has average effect. Therefore, `lineart_anime` may be the most balanced choice in most cases.
 
 ### Monochrome Image Detection
 
 When filtering the crawled images, we need to remove monochrome images. However, monochrome images are often not simply
 composed of grayscale colors and may still contain colors, as shown by the first two rows of six images in the figure
 below
 
-![monochrome example](https://deepghs.github.io/imgutils/main/_images/monochrome.dat.svg)
+![monochrome example](https://deepghs.github.io/imgutils/main/_images/monochrome.plot.py.svg)
 
 We can use `is_monochrome` to determine whether an image is monochrome, as shown below:
 
 ```python
 from imgutils.validate import is_monochrome
 
 print(is_monochrome('mono/1.jpg'))  # monochrome images
@@ -180,15 +180,15 @@
 ```
 
 ### Image Tagging
 
 The `imgutils` library integrates various anime-style image tagging models, allowing for results similar to the
 following:
 
-![tagging demo images](https://deepghs.github.io/imgutils/main/_images/tagging_demo.dat.svg)
+![tagging demo images](https://deepghs.github.io/imgutils/main/_images/tagging_demo.plot.py.svg)
 
 The ratings, features, and characters in the image can be detected, like this:
 
 ```python
 import os
 from imgutils.tagging import get_wd14_tags
 
@@ -267,15 +267,15 @@
 ### Character Extraction
 
 When we need to extract the character parts from anime images, we can use
 the [`segment-rgba-with-isnetis`](https://deepghs.github.io/imgutils/main/api_doc/segment/isnetis.html#segment-rgba-with-isnetis)
 function for extraction and obtain an RGBA format image (with the background part being transparent), just like the
 example shown below.
 
-![isnetis](https://deepghs.github.io/imgutils/main/_images/isnetis_trans.dat.svg)
+![isnetis](https://deepghs.github.io/imgutils/main/_images/isnetis_trans.plot.py.svg)
 
 ```python
 from imgutils.segment import segment_rgba_with_isnetis
 
 mask_, image_ = segment_rgba_with_isnetis('hutao.png')
 image_.save('hutao_seg.png')
```

### Comparing `dghs-imgutils-0.0.4/README.md` & `dghs-imgutils-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 * [Image Tagging](https://github.com/deepghs/imgutils#image-tagging)
 * [Character Extraction](https://github.com/deepghs/imgutils#character-extraction)
 
 ### Tachie(差分) Detection and Clustering
 
 For the dataset, we need to filter the differences between the tachie(差分). As shown in the following picture
 
-![tachie](https://deepghs.github.io/imgutils/main/_images/lpips_full.dat.svg)
+![tachie](https://deepghs.github.io/imgutils/main/_images/lpips_full.plot.py.svg)
 
 We can use `lpips_clustering` to cluster such situations as shown below
 
 ```python
 from imgutils.metrics import lpips_clustering
 
 images = [f'lpips/{i}.jpg' for i in range(1, 10)]
@@ -65,45 +65,45 @@
 # ['lpips/1.jpg', 'lpips/2.jpg', 'lpips/3.jpg', 'lpips/4.jpg', 'lpips/5.jpg', 'lpips/6.jpg', 'lpips/7.jpg', 'lpips/8.jpg', 'lpips/9.jpg']
 print(lpips_clustering(images))  # -1 means noises, the same as that in sklearn
 # [0, 0, 0, 1, 1, -1, -1, -1, -1]
 ```
 
 ### Object Detection
 
-Currently, object detection is supported for anime faces and person, as shown below
+Currently, object detection is supported for anime heads and person, as shown below
 
-* Face Detection
+* Head Detection
 
-![face detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/face_detect.dat.svg)
+![head detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/head_detect.plot.py.svg)
 
 * Person Detection
 
-![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect.dat.svg)
+![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect.plot.py.svg)
 
-Based on practical tests, face detection currently has a very stable performance and can be used for automation tasks.
+Based on practical tests, head detection currently has a very stable performance and can be used for automation tasks.
 However, person detection is still being further iterated and will focus on enhancing detection capabilities for
 artistic illustrations in the future.
 
 ### Edge Detection / Lineart Generation
 
 Anime images can be converted to line drawings using the model provided
 by [patrickvonplaten/controlnet_aux](https://github.com/patrickvonplaten/controlnet_aux), as shown below.
 
-![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge.dat.svg)
+![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge.plot.py.svg)
 
 It is worth noting that the `lineart` model may consume more computational resources, while `canny` is the fastest but
 has average effect. Therefore, `lineart_anime` may be the most balanced choice in most cases.
 
 ### Monochrome Image Detection
 
 When filtering the crawled images, we need to remove monochrome images. However, monochrome images are often not simply
 composed of grayscale colors and may still contain colors, as shown by the first two rows of six images in the figure
 below
 
-![monochrome example](https://deepghs.github.io/imgutils/main/_images/monochrome.dat.svg)
+![monochrome example](https://deepghs.github.io/imgutils/main/_images/monochrome.plot.py.svg)
 
 We can use `is_monochrome` to determine whether an image is monochrome, as shown below:
 
 ```python
 from imgutils.validate import is_monochrome
 
 print(is_monochrome('mono/1.jpg'))  # monochrome images
@@ -155,15 +155,15 @@
 ```
 
 ### Image Tagging
 
 The `imgutils` library integrates various anime-style image tagging models, allowing for results similar to the
 following:
 
-![tagging demo images](https://deepghs.github.io/imgutils/main/_images/tagging_demo.dat.svg)
+![tagging demo images](https://deepghs.github.io/imgutils/main/_images/tagging_demo.plot.py.svg)
 
 The ratings, features, and characters in the image can be detected, like this:
 
 ```python
 import os
 from imgutils.tagging import get_wd14_tags
 
@@ -242,15 +242,15 @@
 ### Character Extraction
 
 When we need to extract the character parts from anime images, we can use
 the [`segment-rgba-with-isnetis`](https://deepghs.github.io/imgutils/main/api_doc/segment/isnetis.html#segment-rgba-with-isnetis)
 function for extraction and obtain an RGBA format image (with the background part being transparent), just like the
 example shown below.
 
-![isnetis](https://deepghs.github.io/imgutils/main/_images/isnetis_trans.dat.svg)
+![isnetis](https://deepghs.github.io/imgutils/main/_images/isnetis_trans.plot.py.svg)
 
 ```python
 from imgutils.segment import segment_rgba_with_isnetis
 
 mask_, image_ = segment_rgba_with_isnetis('hutao.png')
 image_.save('hutao_seg.png')
```

### Comparing `dghs-imgutils-0.0.4/dghs_imgutils.egg-info/PKG-INFO` & `dghs-imgutils-0.1.0/dghs_imgutils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.0.4
+Version: 0.1.0
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
@@ -74,15 +74,15 @@
 * [Image Tagging](https://github.com/deepghs/imgutils#image-tagging)
 * [Character Extraction](https://github.com/deepghs/imgutils#character-extraction)
 
 ### Tachie(差分) Detection and Clustering
 
 For the dataset, we need to filter the differences between the tachie(差分). As shown in the following picture
 
-![tachie](https://deepghs.github.io/imgutils/main/_images/lpips_full.dat.svg)
+![tachie](https://deepghs.github.io/imgutils/main/_images/lpips_full.plot.py.svg)
 
 We can use `lpips_clustering` to cluster such situations as shown below
 
 ```python
 from imgutils.metrics import lpips_clustering
 
 images = [f'lpips/{i}.jpg' for i in range(1, 10)]
@@ -90,45 +90,45 @@
 # ['lpips/1.jpg', 'lpips/2.jpg', 'lpips/3.jpg', 'lpips/4.jpg', 'lpips/5.jpg', 'lpips/6.jpg', 'lpips/7.jpg', 'lpips/8.jpg', 'lpips/9.jpg']
 print(lpips_clustering(images))  # -1 means noises, the same as that in sklearn
 # [0, 0, 0, 1, 1, -1, -1, -1, -1]
 ```
 
 ### Object Detection
 
-Currently, object detection is supported for anime faces and person, as shown below
+Currently, object detection is supported for anime heads and person, as shown below
 
-* Face Detection
+* Head Detection
 
-![face detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/face_detect.dat.svg)
+![head detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/head_detect.plot.py.svg)
 
 * Person Detection
 
-![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect.dat.svg)
+![person detection](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/person_detect.plot.py.svg)
 
-Based on practical tests, face detection currently has a very stable performance and can be used for automation tasks.
+Based on practical tests, head detection currently has a very stable performance and can be used for automation tasks.
 However, person detection is still being further iterated and will focus on enhancing detection capabilities for
 artistic illustrations in the future.
 
 ### Edge Detection / Lineart Generation
 
 Anime images can be converted to line drawings using the model provided
 by [patrickvonplaten/controlnet_aux](https://github.com/patrickvonplaten/controlnet_aux), as shown below.
 
-![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge.dat.svg)
+![edge example](https://github.com/deepghs/imgutils/blob/gh-pages/main/_images/edge.plot.py.svg)
 
 It is worth noting that the `lineart` model may consume more computational resources, while `canny` is the fastest but
 has average effect. Therefore, `lineart_anime` may be the most balanced choice in most cases.
 
 ### Monochrome Image Detection
 
 When filtering the crawled images, we need to remove monochrome images. However, monochrome images are often not simply
 composed of grayscale colors and may still contain colors, as shown by the first two rows of six images in the figure
 below
 
-![monochrome example](https://deepghs.github.io/imgutils/main/_images/monochrome.dat.svg)
+![monochrome example](https://deepghs.github.io/imgutils/main/_images/monochrome.plot.py.svg)
 
 We can use `is_monochrome` to determine whether an image is monochrome, as shown below:
 
 ```python
 from imgutils.validate import is_monochrome
 
 print(is_monochrome('mono/1.jpg'))  # monochrome images
@@ -180,15 +180,15 @@
 ```
 
 ### Image Tagging
 
 The `imgutils` library integrates various anime-style image tagging models, allowing for results similar to the
 following:
 
-![tagging demo images](https://deepghs.github.io/imgutils/main/_images/tagging_demo.dat.svg)
+![tagging demo images](https://deepghs.github.io/imgutils/main/_images/tagging_demo.plot.py.svg)
 
 The ratings, features, and characters in the image can be detected, like this:
 
 ```python
 import os
 from imgutils.tagging import get_wd14_tags
 
@@ -267,15 +267,15 @@
 ### Character Extraction
 
 When we need to extract the character parts from anime images, we can use
 the [`segment-rgba-with-isnetis`](https://deepghs.github.io/imgutils/main/api_doc/segment/isnetis.html#segment-rgba-with-isnetis)
 function for extraction and obtain an RGBA format image (with the background part being transparent), just like the
 example shown below.
 
-![isnetis](https://deepghs.github.io/imgutils/main/_images/isnetis_trans.dat.svg)
+![isnetis](https://deepghs.github.io/imgutils/main/_images/isnetis_trans.plot.py.svg)
 
 ```python
 from imgutils.segment import segment_rgba_with_isnetis
 
 mask_, image_ = segment_rgba_with_isnetis('hutao.png')
 image_.save('hutao_seg.png')
```

### Comparing `dghs-imgutils-0.0.4/dghs_imgutils.egg-info/SOURCES.txt` & `dghs-imgutils-0.1.0/dghs_imgutils.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 imgutils/data/decode.py
 imgutils/data/encode.py
 imgutils/data/image.py
 imgutils/data/layer.py
 imgutils/detect/__init__.py
 imgutils/detect/_yolo.py
 imgutils/detect/face.py
+imgutils/detect/head.py
 imgutils/detect/person.py
 imgutils/detect/visual.py
 imgutils/edge/__init__.py
 imgutils/edge/_base.py
 imgutils/edge/canny.py
 imgutils/edge/lineart.py
 imgutils/edge/lineart_anime.py
```

### Comparing `dghs-imgutils-0.0.4/dghs_imgutils.egg-info/requires.txt` & `dghs-imgutils-0.1.0/dghs_imgutils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.4/imgutils/config/meta.py` & `dghs-imgutils-0.1.0/imgutils/config/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Meta information for imgutils package.
 """
 
 #: Title of this project (should be `imgutils`).
 __TITLE__ = 'imgutils'
 
 #: Version of this project.
-__VERSION__ = '0.0.4'
+__VERSION__ = '0.1.0'
 
 #: Short description of the project, will be included in ``setup.py``.
 __DESCRIPTION__ = 'A convenient and user-friendly anime-style image data processing library that integrates ' \
                   'various advanced anime-style image processing models.'
 
 #: Author of this project.
 __AUTHOR__ = 'narugo1992, 7eu7d'
```

### Comparing `dghs-imgutils-0.0.4/imgutils/data/background.py` & `dghs-imgutils-0.1.0/imgutils/data/background.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,13 +54,13 @@
     :param backcolor: Color of the back grids.
     :return: A RGB image which contains the grids and the original image.
 
     .. note::
         In this document, :func:`grid_transparent` is the default option used to
         accurately present the state of the generated image, as shown in the following figure
 
-        .. image:: grid_transparent.dat.svg
+        .. image:: grid_transparent.plot.py.svg
            :align: center
 
     """
     retval = grid_background(image.height, image.width, step, forecolor, backcolor)
     return istack(retval, image).convert('RGB')
```

### Comparing `dghs-imgutils-0.0.4/imgutils/data/decode.py` & `dghs-imgutils-0.1.0/imgutils/data/decode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.4/imgutils/data/encode.py` & `dghs-imgutils-0.1.0/imgutils/data/encode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.4/imgutils/data/image.py` & `dghs-imgutils-0.1.0/imgutils/data/image.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.4/imgutils/data/layer.py` & `dghs-imgutils-0.1.0/imgutils/data/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         >>> hs1 = (1 - np.abs(np.linspace(-1 / 3, 1, height))) ** 0.5
         >>> ws1 = (1 - np.abs(np.linspace(-1, 1, width))) ** 0.5
         >>> nian_mask = hs1[..., None] * ws1  # HxW
         >>> istack(('nian.png', nian_mask)).save('nian_mask.png')
 
         The result should be
 
-        .. image:: grid_istack.dat.svg
+        .. image:: grid_istack.plot.py.svg
            :align: center
     """
     if size is None:
         height, width = None, None
         items = list(map(_process, items))
         for item, alpha in items:
             if isinstance(item, Image.Image):
```

### Comparing `dghs-imgutils-0.0.4/imgutils/detect/_yolo.py` & `dghs-imgutils-0.1.0/imgutils/detect/_yolo.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.4/imgutils/detect/face.py` & `dghs-imgutils-0.1.0/imgutils/detect/head.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 """
 Overview:
-    Detect human faces (including the entire head) in anime images.
+    Detect human heads (including the entire head) in anime images.
 
     Trained on dataset `ani_face_detection <https://universe.roboflow.com/linog/ani_face_detection>`_ with YOLOv8.
 
-    .. image:: face_detect.dat.svg
+    .. image:: head_detect_demo.plot.py.svg
         :align: center
 
-    This is an overall benchmark of all the face detect models:
+    This is an overall benchmark of all the head detect models:
 
-    .. image:: face_detect.benchmark.py.svg
+    .. image:: head_detect_benchmark.plot.py.svg
         :align: center
 
 """
 from functools import lru_cache
 from typing import List, Tuple
 
 from huggingface_hub import hf_hub_download
 
 from ._yolo import _image_preprocess, _data_postprocess
 from ..data import ImageTyping, load_image, rgb_encode
 from ..utils import open_onnx_model
 
 
 @lru_cache()
-def _open_face_detect_model(level: str = 's'):
+def _open_head_detect_model(level: str = 's'):
     return open_onnx_model(hf_hub_download(
         'deepghs/imgutils-models',
-        f'face_detect/face_detect_best_{level}.onnx'
+        f'head_detect/head_detect_best_{level}.onnx'
     ))
 
 
-def detect_faces(image: ImageTyping, level: str = 's', max_infer_size=640,
-                 conf_threshold: float = 0.25, iou_threshold: float = 0.7) \
+def detect_heads(image: ImageTyping, level: str = 's', max_infer_size=640,
+                 conf_threshold: float = 0.3, iou_threshold: float = 0.7) \
         -> List[Tuple[Tuple[int, int, int, int], str, float]]:
     """
     Overview:
-        Detect human faces (including the entire head) in anime images.
+        Detect human heads in anime images.
 
     :param image: Image to detect.
     :param level: The model level being used can be either `s` or `n`.
         The `n` model runs faster with smaller system overhead, while the `s` model achieves higher accuracy.
         The default value is `s`.
     :param max_infer_size: The maximum image size used for model inference, if the image size exceeds this limit,
         the image will be resized and used for inference. The default value is `640` pixels.
     :param conf_threshold: The confidence threshold, only detection results with confidence scores above
-        this threshold will be returned. The default value is `0.25`.
+        this threshold will be returned. The default value is `0.3`.
     :param iou_threshold: The detection area coverage overlap threshold, areas with overlaps above this threshold
         will be discarded. The default value is `0.7`.
     :return: The detection results list, each item includes the detected area `(x0, y0, x1, y1)`,
         the target type (always `head`) and the target confidence score.
 
     Examples::
-        >>> from imgutils.detect import detect_faces, detection_visualize
+        >>> from imgutils.detect import detect_heads, detection_visualize
         >>>
         >>> image = 'mostima_post.jpg'
-        >>> result = detect_faces(image)  # detect it
+        >>> result = detect_heads(image)  # detect it
         >>> result
         [
             ((29, 441, 204, 584), 'head', 0.7874319553375244),
             ((346, 59, 529, 275), 'head', 0.7510495185852051),
             ((606, 51, 895, 336), 'head', 0.6986488103866577)
         ]
         >>>
@@ -68,9 +68,9 @@
         >>> plt.imshow(detection_visualize(image, result))
         >>> plt.show()
     """
     image = load_image(image, mode='RGB')
     new_image, old_size, new_size = _image_preprocess(image, max_infer_size)
 
     data = rgb_encode(new_image)[None, ...]
-    output, = _open_face_detect_model(level).run(['output0'], {'images': data})
+    output, = _open_head_detect_model(level).run(['output0'], {'images': data})
     return _data_postprocess(output[0], conf_threshold, iou_threshold, old_size, new_size, ['head'])
```

### Comparing `dghs-imgutils-0.0.4/imgutils/detect/person.py` & `dghs-imgutils-0.1.0/imgutils/detect/person.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Overview:
     Detect human bodies (including the entire body) in anime images.
 
     Trained on dataset `AniDet3 <https://universe.roboflow.com/university-of-michigan-ann-arbor/anidet3-ai42v>`_ \
         with YOLOv8.
 
-    .. image:: person_detect.dat.svg
+    .. image:: person_detect_demo.plot.py.svg
         :align: center
 
     This is an overall benchmark of all the person detect models:
 
-    .. image:: person_detect.benchmark.py.svg
+    .. image:: person_detect_benchmark.plot.py.svg
         :align: center
 
 """
 from functools import lru_cache
 
 from huggingface_hub import hf_hub_download
```

### Comparing `dghs-imgutils-0.0.4/imgutils/detect/visual.py` & `dghs-imgutils-0.1.0/imgutils/detect/visual.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Overview:
     Visualize the detection results.
 
-    See :func:`imgutils.detect.face.detect_faces` and :func:`imgutils.detect.person.detect_person` for examples.
+    See :func:`imgutils.detect.head.detect_heads` and :func:`imgutils.detect.person.detect_person` for examples.
 """
 from typing import List, Tuple, Optional
 
 from PIL import ImageFont, ImageDraw
 from hbutils.color import rnd_colors, Color
 
 from imgutils.data import ImageTyping, load_image
@@ -42,15 +42,15 @@
         for rendering from `matplotlib`. Therefore, if `matplotlib` is not installed, only the default pixel font
         provided with `Pillow` can be used, and the font size cannot be changed.
     :param no_label: Do not show labels. Default is ``False``.
     :return: A `PIL` image with the same size as the provided image `image`, which contains the original image
         content as well as the visualized bounding boxes.
 
     Examples::
-        See :func:`imgutils.detect.face.detect_faces` and :func:`imgutils.detect.person.detect_person` for examples.
+        See :func:`imgutils.detect.head.detect_heads` and :func:`imgutils.detect.person.detect_person` for examples.
     """
     image = load_image(image, force_background=None, mode='RGBA')
     visual_image = image.copy()
     draw = ImageDraw.Draw(visual_image, mode='RGBA')
     font = _try_get_font_from_matplotlib(fontsize) or ImageFont.load_default()
 
     labels = sorted(labels or {label for _, label, _ in detection})
```

### Comparing `dghs-imgutils-0.0.4/imgutils/edge/__init__.py` & `dghs-imgutils-0.1.0/imgutils/edge/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Overview:
     Obtaining the outline (or you can call that line drawing) of an anime image.
 
     Here is the example and comparison:
 
-    .. image:: edge.dat.svg
+    .. image:: edge_demo.plot.py.svg
         :align: center
 
     This is an overall benchmark of all the outline models:
 
-    .. image:: edge.benchmark.py.svg
+    .. image:: edge_benchmark.plot.py.svg
         :align: center
 
 """
 from .canny import get_edge_by_canny, edge_image_with_canny
 from .lineart import get_edge_by_lineart, edge_image_with_lineart
 from .lineart_anime import get_edge_by_lineart_anime, edge_image_with_lineart_anime
```

### Comparing `dghs-imgutils-0.0.4/imgutils/edge/_base.py` & `dghs-imgutils-0.1.0/imgutils/edge/_base.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.4/imgutils/edge/canny.py` & `dghs-imgutils-0.1.0/imgutils/edge/canny.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     :param backcolor: Background color the target image. Default is ``white``. When ``transparent`` is given, \
         the background will be transparent.
     :param forecolor: Fore color of the target image. Default is ``None`` which means use the color \
         from the given ``image``.
     :return: An image with the extracted edge from ``image``.
 
     Examples::
-        .. image:: canny.dat.svg
+        .. image:: canny.plot.py.svg
             :align: center
     """
     return _get_image_edge(
         image,
         partial(get_edge_by_canny, low_threshold=low_threshold, high_threshold=high_threshold),
         backcolor, forecolor
     )
```

### Comparing `dghs-imgutils-0.0.4/imgutils/edge/lineart.py` & `dghs-imgutils-0.1.0/imgutils/edge/lineart.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,20 +61,20 @@
     :param backcolor: Background color the target image. Default is ``white``. When ``transparent`` is given, \
         the background will be transparent.
     :param forecolor: Fore color of the target image. Default is ``None`` which means use the color \
         from the given ``image``.
     :return: An image with the extracted edge from ``image``.
 
     Examples::
-        .. image:: lineart.dat.svg
+        .. image:: lineart.plot.py.svg
             :align: center
 
         When ``coarse`` is used:
 
-        .. image:: lineart_coarse.dat.svg
+        .. image:: lineart_coarse.plot.py.svg
             :align: center
     """
     return _get_image_edge(
         image,
         partial(get_edge_by_lineart, coarse=coarse, detect_resolution=detect_resolution),
         backcolor, forecolor
     )
```

### Comparing `dghs-imgutils-0.0.4/imgutils/edge/lineart_anime.py` & `dghs-imgutils-0.1.0/imgutils/edge/lineart_anime.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     :param backcolor: Background color the target image. Default is ``white``. When ``transparent`` is given, \
         the background will be transparent.
     :param forecolor: Fore color of the target image. Default is ``None`` which means use the color \
         from the given ``image``.
     :return: An image with the extracted edge from ``image``.
 
     Examples::
-        .. image:: lineart_anime.dat.svg
+        .. image:: lineart_anime.plot.py.svg
             :align: center
     """
     return _get_image_edge(
         image,
         partial(get_edge_by_lineart_anime, detect_resolution=detect_resolution),
         backcolor, forecolor
     )
```

### Comparing `dghs-imgutils-0.0.4/imgutils/metrics/aesthetic.py` & `dghs-imgutils-0.1.0/imgutils/metrics/aesthetic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Overview:
     A tool for measuring the aesthetic level of anime images, with the model
     obtained from `skytnt/anime-aesthetic <https://huggingface.co/skytnt/anime-aesthetic>`_.
 
-    .. image:: aesthetic_full.dat.svg
+    .. image:: aesthetic_full.plot.py.svg
         :align: center
 
     This is an overall benchmark of all the operations in aesthetic models:
 
-    .. image:: aesthetic.benchmark.py.svg
+    .. image:: aesthetic_benchmark.plot.py.svg
         :align: center
 """
 from functools import lru_cache
 
 import cv2
 import numpy as np
 from PIL import Image
```

### Comparing `dghs-imgutils-0.0.4/imgutils/metrics/lpips.py` & `dghs-imgutils-0.1.0/imgutils/metrics/lpips.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Useful utilities based on `richzhang/PerceptualSimilarity <https://github.com/richzhang/PerceptualSimilarity>`_, \
     tested with dataset `deepghs/chafen_arknights(private) <https://huggingface.co/datasets/deepghs/chafen_arknights>`_.
 
     When threshold is `0.45`, the `adjusted rand score <https://scikit-learn.org/stable/modules/generated/sklearn.metrics.adjusted_rand_score.html>`_ can reach `0.995`.
 
     This is an overall benchmark of all the operations in LPIPS models:
 
-    .. image:: lpips.benchmark.py.svg
+    .. image:: lpips_benchmark.plot.py.svg
         :align: center
 
 """
 from functools import lru_cache
 from typing import Tuple, Union, List
 
 import numpy as np
@@ -115,15 +115,15 @@
     :param img1: Image file, PIL object or extracted feature of image.
     :param img2: Image file, PIL object or extracted feature of another image.
     :return: LPIPS difference. Value lower than ``0.45`` usually represents similar.
 
     Example:
         Here are some images for example
 
-        .. image:: lpips_small.dat.svg
+        .. image:: lpips_small.plot.py.svg
            :align: center
 
         >>> from imgutils.metrics import lpips_difference
         >>>
         >>> lpips_difference('lpips/1.jpg', 'lpips/2.jpg')
         0.16922694444656372
         >>> lpips_difference('lpips/1.jpg', 'lpips/3.jpg')
@@ -150,15 +150,15 @@
     :param images: List of multiple images.
     :param threshold: Threshold of clustering. Default value ``0.45`` is recommended.
     :return: Clustering result with LPIPS, each integer represent one group, ``-1`` means this is a noise sample.
 
     Example:
         Here are some images for example
 
-        .. image:: lpips_full.dat.svg
+        .. image:: lpips_full.plot.py.svg
            :align: center
 
         >>> from imgutils.metrics import lpips_clustering
         >>>
         >>> images = [f'lpips/{i}.jpg' for i in range(1, 10)]
         >>> images
         ['lpips/1.jpg', 'lpips/2.jpg', 'lpips/3.jpg', 'lpips/4.jpg', 'lpips/5.jpg', 'lpips/6.jpg', 'lpips/7.jpg', 'lpips/8.jpg', 'lpips/9.jpg']
```

### Comparing `dghs-imgutils-0.0.4/imgutils/metrics/psnr_.py` & `dghs-imgutils-0.1.0/imgutils/metrics/psnr_.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     :param img1: First image.
     :param img2: Second image.
     :return: Psnr difference of these two images.
 
     Example:
         Here are some images for example
 
-        .. image:: psnr.dat.svg
+        .. image:: psnr.plot.py.svg
            :align: center
 
         >>> from imgutils.metrics import psnr
         >>>
         >>> psnr('psnr/origin.jpg', 'psnr/origin.jpg')  # same image
         inf
         >>> psnr('psnr/origin.jpg', 'psnr/gaussian_20.dat.jpg')
```

### Comparing `dghs-imgutils-0.0.4/imgutils/segment/isnetis.py` & `dghs-imgutils-0.1.0/imgutils/segment/isnetis.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         >>> image_.save('hutao_seg.png')
         >>>
         >>> mask_, image_ = segment_with_isnetis('skadi.jpg', background='white')  # white background
         >>> image_.save('skadi_seg.jpg')
 
         The result should be
 
-        .. image:: isnetis_color.dat.svg
+        .. image:: isnetis_color.plot.py.svg
            :align: center
 
     """
     image = load_image(image, mode='RGB')
     mask = get_isnetis_mask(image, scale)
     return mask, istack((background, 1.0), (image, mask)).convert('RGB')
 
@@ -91,14 +91,14 @@
         >>> image_.save('hutao_seg.png')
         >>>
         >>> mask_, image_ = segment_rgba_with_isnetis('skadi.jpg')
         >>> image_.save('skadi_seg.png')
 
         The result should be
 
-        .. image:: isnetis_trans.dat.svg
+        .. image:: isnetis_trans.plot.py.svg
            :align: center
 
     """
     image = load_image(image, mode='RGB')
     mask = get_isnetis_mask(image, scale)
     return mask, istack((image, mask))
```

### Comparing `dghs-imgutils-0.0.4/imgutils/tagging/deepdanbooru.py` & `dghs-imgutils-0.1.0/imgutils/tagging/deepdanbooru.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     :param general_threshold: Threshold for default tags, default is ``0.35``.
     :param character_threshold: Threshold for character tags, default is ``0.85``.
     :return: Tagging results for levels, features and characters.
 
     Example:
         Here are some images for example
 
-        .. image:: tagging_demo.dat.svg
+        .. image:: tagging_demo.plot.py.svg
            :align: center
 
         >>> from imgutils.tagging import get_deepdanbooru_tags
         >>>
         >>> rating, features, chars = get_deepdanbooru_tags('skadi.jpg')
         >>> rating
         {'rating:safe': 0.9897817373275757, 'rating:questionable': 0.010265946388244629, 'rating:explicit': 5.2809715270996094e-05}
```

### Comparing `dghs-imgutils-0.0.4/imgutils/tagging/format.py` & `dghs-imgutils-0.1.0/imgutils/tagging/format.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.4/imgutils/tagging/mldanbooru.py` & `dghs-imgutils-0.1.0/imgutils/tagging/mldanbooru.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     :param size: Size when passing the resized image into model, default is ``448``.
     :param keep_ratio: Keep the original ratio between height and width when passing the image into
         model, default is ``False``.
 
     Example:
         Here are some images for example
 
-        .. image:: tagging_demo.dat.svg
+        .. image:: tagging_demo.plot.py.svg
            :align: center
 
         >>> import os
         >>> from imgutils.tagging import get_mldanbooru_tags
         >>>
         >>> get_mldanbooru_tags('skadi.jpg')
         {'1girl': 0.9999984502792358, 'long_hair': 0.9999946355819702, 'red_eyes': 0.9994951486587524, 'navel': 0.998144268989563, 'breasts': 0.9978417158126831, 'solo': 0.9941409230232239, 'shorts': 0.9799384474754333, 'gloves': 0.979142427444458, 'very_long_hair': 0.961823582649231, 'looking_at_viewer': 0.961323618888855, 'silver_hair': 0.9490893483161926, 'large_breasts': 0.9450850486755371, 'midriff': 0.9425153136253357, 'sweat': 0.9409335255622864, 'thighs': 0.9319437146186829, 'crop_top': 0.9265308976173401, 'baseball_bat': 0.9259042143821716, 'sky': 0.922250509262085, 'holding': 0.9199565052986145, 'outdoors': 0.9175475835800171, 'day': 0.9102761745452881, 'black_gloves': 0.9076938629150391, 'stomach': 0.9052775502204895, 'shirt': 0.8938589692115784, 'cowboy_shot': 0.8894285559654236, 'bangs': 0.8891903162002563, 'blue_sky': 0.8845980763435364, 'parted_lips': 0.8842408061027527, 'hair_between_eyes': 0.8659475445747375, 'sportswear': 0.862621009349823, 'no_headwear': 0.8616052865982056, 'cloud': 0.8562789559364319, 'short_shorts': 0.8555729389190674, 'no_hat': 0.8533340096473694, 'black_shorts': 0.8477485775947571, 'short_sleeves': 0.8430152535438538, 'low-tied_long_hair': 0.8340626955032349, 'crop_top_overhang': 0.8266023397445679, 'holding_baseball_bat': 0.8222048282623291, 'standing': 0.8202669620513916, 'black_shirt': 0.8061150312423706, 'ass_visible_through_thighs': 0.7803354859352112, 'thigh_gap': 0.7789446711540222, 'arms_up': 0.7052110433578491}
```

### Comparing `dghs-imgutils-0.0.4/imgutils/tagging/wd14.py` & `dghs-imgutils-0.1.0/imgutils/tagging/wd14.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     :param general_threshold: Threshold for default tags, default is ``0.35``.
     :param character_threshold: Threshold for character tags, default is ``0.85``.
     :return: Tagging results for levels, features and characters.
 
     Example:
         Here are some images for example
 
-        .. image:: tagging_demo.dat.svg
+        .. image:: tagging_demo.plot.py.svg
            :align: center
 
         >>> import os
         >>> from imgutils.tagging import get_wd14_tags
         >>>
         >>> rating, features, chars = get_wd14_tags('skadi.jpg')
         >>> rating
```

### Comparing `dghs-imgutils-0.0.4/imgutils/utils/onnxruntime.py` & `dghs-imgutils-0.1.0/imgutils/utils/onnxruntime.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.4/imgutils/validate/color.py` & `dghs-imgutils-0.1.0/imgutils/validate/color.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     :param image: Path or PIL object of image.
     :return: Is greyscale or not.
 
     Examples:
         Here are some images for example
 
-        .. image:: greyscale.dat.svg
+        .. image:: greyscale.plot.py.svg
            :align: center
 
         >>> from imgutils.validate import is_greyscale
         >>>
         >>> is_greyscale('jpeg_full.jpeg')
         False
         >>> is_greyscale('6125901.jpg')
```

### Comparing `dghs-imgutils-0.0.4/imgutils/validate/monochrome.py` & `dghs-imgutils-0.1.0/imgutils/validate/monochrome.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Overview:
     A model for screening monochrome images, with the definition of monochrome images referring to Danbooru.
 
     The following are testing images. The top two rows are monochrome images, and the bottom two rows are color images.
     Please note that **monochrome images are not only those with all pixels in grayscale**.
 
-    .. image:: monochrome.dat.svg
+    .. image:: monochrome.plot.py.svg
         :align: center
 
     This is an overall benchmark of all the monochrome validation models:
 
-    .. image:: monochrome.benchmark.py.svg
+    .. image:: monochrome_benchmark.plot.py.svg
         :align: center
 """
 from functools import lru_cache
 from typing import Optional, Tuple, Mapping
 
 import numpy as np
 from PIL import Image
```

### Comparing `dghs-imgutils-0.0.4/imgutils/validate/truncate.py` & `dghs-imgutils-0.1.0/imgutils/validate/truncate.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     :param path: Path of file (must be a string which represents the path of image).
     :return: Is truncated or not.
 
     Examples:
         Here are some images for example
 
-        .. image:: truncated.dat.svg
+        .. image:: truncated.plot.py.svg
            :align: center
 
         >>> from imgutils.validate import is_truncated_file
         >>>
         >>> is_truncated_file('jpeg_full.jpeg')
         False
         >>> is_truncated_file('jpeg_truncated.jpeg')
```

### Comparing `dghs-imgutils-0.0.4/setup.py` & `dghs-imgutils-0.1.0/setup.py`

 * *Files identical despite different names*

