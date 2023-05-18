# Comparing `tmp/lacss-0.3.0.tar.gz` & `tmp/lacss-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacss-0.3.0.tar", max compression
+gzip compressed data, was "lacss-0.3.1.tar", max compression
```

## Comparing `lacss-0.3.0.tar` & `lacss-0.3.1.tar`

### file list

```diff
@@ -1,50 +1,150 @@
--rw-r--r--   0        0        0     1062 2023-03-07 20:26:01.088077 lacss-0.3.0/LICENSE
--rw-r--r--   0        0        0     1140 2023-04-14 14:17:40.520445 lacss-0.3.0/README.md
--rw-r--r--   0        0        0       65 2023-04-20 16:47:25.199622 lacss-0.3.0/lacss/__init__.py
--rw-r--r--   0        0        0       47 2023-03-08 13:25:26.759293 lacss-0.3.0/lacss/data/__init__.py
--rw-r--r--   0        0        0     6063 2023-03-08 13:25:26.771841 lacss-0.3.0/lacss/data/generator.py
--rw-r--r--   0        0        0     9160 2023-04-09 15:45:08.107465 lacss-0.3.0/lacss/data/parser.py
--rw-r--r--   0        0        0     3107 2023-04-20 16:47:25.195421 lacss-0.3.0/lacss/deploy.py
--rw-r--r--   0        0        0       74 2023-03-08 13:25:26.788189 lacss-0.3.0/lacss/losses/__init__.py
--rw-r--r--   0        0        0     5524 2023-04-17 17:58:59.215796 lacss-0.3.0/lacss/losses/auxiliary.py
--rw-r--r--   0        0        0     3189 2023-04-09 15:45:08.834799 lacss-0.3.0/lacss/losses/detection.py
--rw-r--r--   0        0        0     8278 2023-04-19 18:55:57.265740 lacss-0.3.0/lacss/losses/instance.py
--rw-r--r--   0        0        0       56 2023-04-09 15:43:25.895964 lacss-0.3.0/lacss/metrics/__init__.py
--rw-r--r--   0        0        0     5547 2023-04-09 15:45:08.243066 lacss-0.3.0/lacss/metrics/ranked.py
--rw-r--r--   0        0        0      216 2023-04-09 15:45:09.203039 lacss-0.3.0/lacss/modules/__init__.py
--rw-r--r--   0        0        0     3171 2023-04-10 12:50:28.921730 lacss-0.3.0/lacss/modules/auxiliary.py
--rw-r--r--   0        0        0     2270 2023-04-09 15:43:26.027653 lacss-0.3.0/lacss/modules/common.py
--rw-r--r--   0        0        0     6557 2023-04-17 17:58:06.955449 lacss-0.3.0/lacss/modules/convnext.py
--rw-r--r--   0        0        0     6270 2023-04-09 15:43:26.072837 lacss-0.3.0/lacss/modules/detector.py
--rw-r--r--   0        0        0     3813 2023-04-09 15:45:08.267826 lacss-0.3.0/lacss/modules/lacss.py
--rw-r--r--   0        0        0     2934 2023-04-09 15:45:08.286815 lacss-0.3.0/lacss/modules/lpn.py
--rw-r--r--   0        0        0     3771 2023-04-09 15:45:07.023954 lacss-0.3.0/lacss/modules/resnet.py
--rw-r--r--   0        0        0     4595 2023-04-09 15:45:07.056520 lacss-0.3.0/lacss/modules/segmentor.py
--rw-r--r--   0        0        0     1979 2023-04-10 12:50:41.257622 lacss-0.3.0/lacss/modules/unet.py
--rw-r--r--   0        0        0      155 2023-03-08 13:25:26.937574 lacss-0.3.0/lacss/ops/__init__.py
--rw-r--r--   0        0        0     2175 2023-04-09 15:43:24.529427 lacss-0.3.0/lacss/ops/boxes.py
--rw-r--r--   0        0        0     2218 2023-04-09 15:45:07.073615 lacss-0.3.0/lacss/ops/image.py
--rw-r--r--   0        0        0     2739 2023-03-08 13:25:24.882290 lacss-0.3.0/lacss/ops/locations.py
--rw-r--r--   0        0        0     5967 2023-03-08 13:25:26.971031 lacss-0.3.0/lacss/ops/masks.py
--rw-r--r--   0        0        0     4704 2023-03-08 13:25:26.979821 lacss-0.3.0/lacss/ops/nms.py
--rw-r--r--   0        0        0     9245 2023-04-09 15:45:08.363814 lacss-0.3.0/lacss/ops/patches.py
--rw-r--r--   0        0        0       19 2023-03-07 23:30:16.150024 lacss-0.3.0/lacss/tracking/__init__.py
--rw-r--r--   0        0        0    13086 2023-04-09 15:41:06.218121 lacss-0.3.0/lacss/tracking/smc.py
--rw-r--r--   0        0        0       99 2023-04-09 15:43:27.268348 lacss-0.3.0/lacss/train/__init__.py
--rw-r--r--   0        0        0      718 2023-03-08 13:25:27.022221 lacss-0.3.0/lacss/train/data/__init__.py
--rw-r--r--   0        0        0     4076 2023-03-08 13:25:25.475969 lacss-0.3.0/lacss/train/data/array_adapter.py
--rw-r--r--   0        0        0     5529 2023-03-08 13:25:25.535533 lacss-0.3.0/lacss/train/data/data_adapter.py
--rw-r--r--   0        0        0     6287 2023-03-07 20:25:59.686559 lacss-0.3.0/lacss/train/data/data_handler.py
--rw-r--r--   0        0        0    10656 2023-03-07 23:30:16.170915 lacss-0.3.0/lacss/train/data/dataset.py
--rw-r--r--   0        0        0     2599 2023-03-07 20:26:00.050854 lacss-0.3.0/lacss/train/data/generator_adapter.py
--rw-r--r--   0        0        0     2105 2023-03-07 20:26:00.044184 lacss-0.3.0/lacss/train/data/list_adapter.py
--rw-r--r--   0        0        0     3440 2023-03-07 20:25:59.695064 lacss-0.3.0/lacss/train/data/tf_dataset_adapter.py
--rw-r--r--   0        0        0     2566 2023-03-07 20:25:59.999227 lacss-0.3.0/lacss/train/data/torch_dataloader_adapter.py
--rw-r--r--   0        0        0     6394 2023-03-08 13:25:25.861971 lacss-0.3.0/lacss/train/data/utils.py
--rw-r--r--   0        0        0     6826 2023-04-09 15:45:10.891402 lacss-0.3.0/lacss/train/loss.py
--rw-r--r--   0        0        0      222 2023-04-09 15:43:26.263916 lacss-0.3.0/lacss/train/metric.py
--rw-r--r--   0        0        0     4018 2023-04-09 15:45:10.909855 lacss-0.3.0/lacss/train/strategy.py
--rw-r--r--   0        0        0     7437 2023-04-14 17:55:24.096524 lacss-0.3.0/lacss/train/trainer.py
--rw-r--r--   0        0        0     4571 2023-04-20 16:47:25.237210 lacss-0.3.0/lacss/utils.py
--rw-r--r--   0        0        0      810 2023-04-21 18:21:08.516980 lacss-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 lacss-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-21 18:45:47.667328 lacss-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2188 2023-05-18 16:20:17.041288 lacss-0.3.1/README.md
+-rw-r--r--   0        0        0       58 2023-03-07 20:26:00.699876 lacss-0.3.1/lacss/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0       65 2023-04-21 18:45:47.772087 lacss-0.3.1/lacss/__init__.py
+-rw-r--r--   0        0        0      580 2023-05-18 16:12:05.535144 lacss-0.3.1/lacss/app/da.py
+-rw-r--r--   0        0        0       47 2023-04-21 18:45:47.795653 lacss-0.3.1/lacss/data/__init__.py
+-rw-r--r--   0        0        0      194 2023-03-07 20:26:00.289795 lacss-0.3.1/lacss/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      189 2023-04-26 16:05:13.976775 lacss-0.3.1/lacss/data/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4337 2023-03-07 20:26:00.277190 lacss-0.3.1/lacss/data/__pycache__/generator.cpython-310.pyc
+-rw-r--r--   0        0        0     4422 2023-04-26 16:05:14.005891 lacss-0.3.1/lacss/data/__pycache__/generator.cpython-38.pyc
+-rw-r--r--   0        0        0     3648 2023-03-07 20:26:00.257796 lacss-0.3.1/lacss/data/__pycache__/parser.cpython-310.pyc
+-rw-r--r--   0        0        0     5681 2023-04-26 16:05:14.758099 lacss-0.3.1/lacss/data/__pycache__/parser.cpython-38.pyc
+-rw-r--r--   0        0        0     6063 2023-04-21 18:45:47.824902 lacss-0.3.1/lacss/data/generator.py
+-rw-r--r--   0        0        0     9160 2023-04-21 18:45:47.837649 lacss-0.3.1/lacss/data/parser.py
+-rw-r--r--   0        0        0     3307 2023-05-17 12:27:49.433436 lacss-0.3.1/lacss/deploy.py
+-rw-r--r--   0        0        0       74 2023-05-18 16:15:17.877065 lacss-0.3.1/lacss/losses/__init__.py
+-rw-r--r--   0        0        0      216 2023-03-07 20:26:00.790038 lacss-0.3.1/lacss/losses/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      231 2023-05-17 13:50:37.368341 lacss-0.3.1/lacss/losses/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5330 2023-05-17 19:06:53.529626 lacss-0.3.1/lacss/losses/__pycache__/auxiliary.cpython-38.pyc
+-rw-r--r--   0        0        0     2049 2023-03-07 20:26:00.816719 lacss-0.3.1/lacss/losses/__pycache__/auxnet.cpython-310.pyc
+-rw-r--r--   0        0        0     2076 2023-03-07 20:26:00.777737 lacss-0.3.1/lacss/losses/__pycache__/auxnet.cpython-38.pyc
+-rw-r--r--   0        0        0     3271 2023-03-07 20:26:00.744429 lacss-0.3.1/lacss/losses/__pycache__/detection.cpython-310.pyc
+-rw-r--r--   0        0        0     3304 2023-05-17 13:50:37.737229 lacss-0.3.1/lacss/losses/__pycache__/detection.cpython-38.pyc
+-rw-r--r--   0        0        0     3243 2023-03-07 20:26:00.758307 lacss-0.3.1/lacss/losses/__pycache__/instance.cpython-310.pyc
+-rw-r--r--   0        0        0     4451 2023-05-17 13:50:40.487927 lacss-0.3.1/lacss/losses/__pycache__/instance.cpython-38.pyc
+-rw-r--r--   0        0        0     1986 2023-05-17 19:06:55.091616 lacss-0.3.1/lacss/losses/__pycache__/lacss.cpython-38.pyc
+-rw-r--r--   0        0        0     5087 2023-03-07 20:26:00.750432 lacss-0.3.1/lacss/losses/__pycache__/loss.cpython-38.pyc
+-rw-r--r--   0        0        0     5524 2023-05-18 16:15:17.883556 lacss-0.3.1/lacss/losses/auxiliary.py
+-rw-r--r--   0        0        0     3189 2023-05-18 16:15:17.890613 lacss-0.3.1/lacss/losses/detection.py
+-rw-r--r--   0        0        0     8278 2023-05-18 16:15:17.897817 lacss-0.3.1/lacss/losses/instance.py
+-rw-r--r--   0        0        0       56 2023-04-21 18:45:47.932120 lacss-0.3.1/lacss/metrics/__init__.py
+-rw-r--r--   0        0        0      176 2023-03-07 20:26:00.875358 lacss-0.3.1/lacss/metrics/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      219 2023-04-26 16:05:15.350411 lacss-0.3.1/lacss/metrics/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      650 2023-03-17 12:50:11.457103 lacss-0.3.1/lacss/metrics/__pycache__/metric.cpython-38.pyc
+-rw-r--r--   0        0        0     5469 2023-03-07 20:26:00.863743 lacss-0.3.1/lacss/metrics/__pycache__/ranked.cpython-310.pyc
+-rw-r--r--   0        0        0     5809 2023-04-26 16:05:15.382370 lacss-0.3.1/lacss/metrics/__pycache__/ranked.cpython-38.pyc
+-rw-r--r--   0        0        0     5547 2023-04-21 18:45:47.940716 lacss-0.3.1/lacss/metrics/ranked.py
+-rw-r--r--   0        0        0      216 2023-04-28 14:03:41.857622 lacss-0.3.1/lacss/modules/__init__.py
+-rw-r--r--   0        0        0      484 2023-03-07 20:26:00.615885 lacss-0.3.1/lacss/modules/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      435 2023-04-28 14:28:40.915459 lacss-0.3.1/lacss/modules/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3869 2023-05-17 15:11:16.098273 lacss-0.3.1/lacss/modules/__pycache__/auxiliary.cpython-38.pyc
+-rw-r--r--   0        0        0     1131 2023-03-07 20:26:00.643794 lacss-0.3.1/lacss/modules/__pycache__/auxnet.cpython-310.pyc
+-rw-r--r--   0        0        0     1066 2023-03-07 20:26:00.591783 lacss-0.3.1/lacss/modules/__pycache__/auxnet.cpython-38.pyc
+-rw-r--r--   0        0        0     4225 2023-05-17 15:22:00.187532 lacss-0.3.1/lacss/modules/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0        0        0     8008 2023-03-07 20:26:00.636668 lacss-0.3.1/lacss/modules/__pycache__/convnext.cpython-310.pyc
+-rw-r--r--   0        0        0     6398 2023-04-28 14:28:41.147671 lacss-0.3.1/lacss/modules/__pycache__/convnext.cpython-38.pyc
+-rw-r--r--   0        0        0     5064 2023-03-07 20:26:00.531471 lacss-0.3.1/lacss/modules/__pycache__/detector.cpython-310.pyc
+-rw-r--r--   0        0        0     4848 2023-05-15 14:38:02.594877 lacss-0.3.1/lacss/modules/__pycache__/detector.cpython-38.pyc
+-rw-r--r--   0        0        0     3995 2023-03-07 20:26:00.556378 lacss-0.3.1/lacss/modules/__pycache__/lacss.cpython-310.pyc
+-rw-r--r--   0        0        0     3430 2023-05-17 19:02:36.950020 lacss-0.3.1/lacss/modules/__pycache__/lacss.cpython-38.pyc
+-rw-r--r--   0        0        0     3129 2023-03-07 20:26:00.526426 lacss-0.3.1/lacss/modules/__pycache__/lpn.cpython-310.pyc
+-rw-r--r--   0        0        0     2985 2023-05-18 14:56:00.640109 lacss-0.3.1/lacss/modules/__pycache__/lpn.cpython-38.pyc
+-rw-r--r--   0        0        0     5339 2023-03-07 20:26:00.576473 lacss-0.3.1/lacss/modules/__pycache__/resnet.cpython-310.pyc
+-rw-r--r--   0        0        0     3578 2023-04-26 16:05:15.594809 lacss-0.3.1/lacss/modules/__pycache__/resnet.cpython-38.pyc
+-rw-r--r--   0        0        0     1680 2023-03-07 20:26:00.571302 lacss-0.3.1/lacss/modules/__pycache__/se_net.cpython-310.pyc
+-rw-r--r--   0        0        0      147 2023-03-07 20:26:00.489800 lacss-0.3.1/lacss/modules/__pycache__/se_net.cpython-38.pyc
+-rw-r--r--   0        0        0     4346 2023-03-07 20:26:00.597085 lacss-0.3.1/lacss/modules/__pycache__/segmentor.cpython-310.pyc
+-rw-r--r--   0        0        0     3951 2023-05-17 13:53:10.140274 lacss-0.3.1/lacss/modules/__pycache__/segmentor.cpython-38.pyc
+-rw-r--r--   0        0        0      969 2023-03-07 20:26:00.631053 lacss-0.3.1/lacss/modules/__pycache__/types.cpython-310.pyc
+-rw-r--r--   0        0        0     1424 2023-03-07 20:26:00.503425 lacss-0.3.1/lacss/modules/__pycache__/types.cpython-38.pyc
+-rw-r--r--   0        0        0     3097 2023-03-07 20:26:00.546308 lacss-0.3.1/lacss/modules/__pycache__/unet.cpython-310.pyc
+-rw-r--r--   0        0        0     2211 2023-04-28 14:28:41.128007 lacss-0.3.1/lacss/modules/__pycache__/unet.cpython-38.pyc
+-rw-r--r--   0        0        0     7267 2023-03-07 20:26:00.509827 lacss-0.3.1/lacss/modules/__pycache__/xcit.cpython-310.pyc
+-rw-r--r--   0        0        0     7215 2023-03-07 20:26:00.607719 lacss-0.3.1/lacss/modules/__pycache__/xcit.cpython-38.pyc
+-rw-r--r--   0        0        0     3171 2023-05-18 16:15:17.906763 lacss-0.3.1/lacss/modules/auxiliary.py
+-rw-r--r--   0        0        0     2270 2023-05-18 16:15:17.916458 lacss-0.3.1/lacss/modules/common.py
+-rw-r--r--   0        0        0     6557 2023-04-28 14:03:41.873034 lacss-0.3.1/lacss/modules/convnext.py
+-rw-r--r--   0        0        0     6579 2023-05-15 14:29:30.716593 lacss-0.3.1/lacss/modules/detector.py
+-rw-r--r--   0        0        0     3813 2023-05-18 16:15:17.927778 lacss-0.3.1/lacss/modules/lacss.py
+-rw-r--r--   0        0        0     2934 2023-05-18 16:15:17.938204 lacss-0.3.1/lacss/modules/lpn.py
+-rw-r--r--   0        0        0     3771 2023-04-21 18:45:48.045107 lacss-0.3.1/lacss/modules/resnet.py
+-rw-r--r--   0        0        0     4595 2023-05-18 16:15:17.967503 lacss-0.3.1/lacss/modules/segmentor.py
+-rw-r--r--   0        0        0     1979 2023-04-28 14:03:41.880651 lacss-0.3.1/lacss/modules/unet.py
+-rw-r--r--   0        0        0      155 2023-04-21 18:45:48.079314 lacss-0.3.1/lacss/ops/__init__.py
+-rw-r--r--   0        0        0      260 2023-03-07 20:26:00.414720 lacss-0.3.1/lacss/ops/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      255 2023-04-26 16:05:14.845951 lacss-0.3.1/lacss/ops/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1804 2023-03-07 20:26:00.409875 lacss-0.3.1/lacss/ops/__pycache__/boxes.cpython-310.pyc
+-rw-r--r--   0        0        0     1987 2023-04-26 16:05:14.869998 lacss-0.3.1/lacss/ops/__pycache__/boxes.cpython-38.pyc
+-rw-r--r--   0        0        0     1121 2023-03-07 20:26:00.435101 lacss-0.3.1/lacss/ops/__pycache__/image.cpython-310.pyc
+-rw-r--r--   0        0        0     2559 2023-04-26 16:05:14.898406 lacss-0.3.1/lacss/ops/__pycache__/image.cpython-38.pyc
+-rw-r--r--   0        0        0     2379 2023-03-07 20:26:00.429728 lacss-0.3.1/lacss/ops/__pycache__/locations.cpython-310.pyc
+-rw-r--r--   0        0        0     2347 2023-04-26 16:05:14.926967 lacss-0.3.1/lacss/ops/__pycache__/locations.cpython-38.pyc
+-rw-r--r--   0        0        0     5827 2023-03-07 20:26:00.371538 lacss-0.3.1/lacss/ops/__pycache__/masks.cpython-310.pyc
+-rw-r--r--   0        0        0     5806 2023-04-26 16:05:14.944134 lacss-0.3.1/lacss/ops/__pycache__/masks.cpython-38.pyc
+-rw-r--r--   0        0        0     3845 2023-03-07 20:26:00.404805 lacss-0.3.1/lacss/ops/__pycache__/nms.cpython-310.pyc
+-rw-r--r--   0        0        0     3857 2023-04-26 16:05:14.998332 lacss-0.3.1/lacss/ops/__pycache__/nms.cpython-38.pyc
+-rw-r--r--   0        0        0     5649 2023-03-07 20:26:00.394465 lacss-0.3.1/lacss/ops/__pycache__/patches.cpython-310.pyc
+-rw-r--r--   0        0        0     7853 2023-04-26 16:05:14.981060 lacss-0.3.1/lacss/ops/__pycache__/patches.cpython-38.pyc
+-rw-r--r--   0        0        0     2175 2023-04-21 18:45:48.091110 lacss-0.3.1/lacss/ops/boxes.py
+-rw-r--r--   0        0        0     2218 2023-04-21 18:45:48.100899 lacss-0.3.1/lacss/ops/image.py
+-rw-r--r--   0        0        0     2739 2023-04-21 18:45:48.114632 lacss-0.3.1/lacss/ops/locations.py
+-rw-r--r--   0        0        0     5967 2023-04-21 18:45:48.142871 lacss-0.3.1/lacss/ops/masks.py
+-rw-r--r--   0        0        0     4704 2023-04-21 18:45:48.169083 lacss-0.3.1/lacss/ops/nms.py
+-rw-r--r--   0        0        0     9245 2023-04-21 18:45:48.177726 lacss-0.3.1/lacss/ops/patches.py
+-rw-r--r--   0        0        0       63 2023-05-17 12:27:49.580967 lacss-0.3.1/lacss/tracking/__init__.py
+-rw-r--r--   0        0        0      205 2023-05-14 18:38:38.567521 lacss-0.3.1/lacss/tracking/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2689 2023-05-15 15:16:43.449032 lacss-0.3.1/lacss/tracking/__pycache__/predict.cpython-38.pyc
+-rw-r--r--   0        0        0     6517 2023-05-15 18:37:20.371555 lacss-0.3.1/lacss/tracking/__pycache__/smc.cpython-38.pyc
+-rw-r--r--   0        0        0     4358 2023-05-15 18:37:20.409926 lacss-0.3.1/lacss/tracking/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     3340 2023-05-17 12:27:49.587345 lacss-0.3.1/lacss/tracking/predict.py
+-rw-r--r--   0        0        0     6741 2023-05-17 12:27:49.597252 lacss-0.3.1/lacss/tracking/smc.py
+-rw-r--r--   0        0        0     5646 2023-05-17 12:27:49.616793 lacss-0.3.1/lacss/tracking/utils.py
+-rw-r--r--   0        0        0       99 2023-04-21 18:45:48.241245 lacss-0.3.1/lacss/train/__init__.py
+-rw-r--r--   0        0        0      191 2023-03-07 20:26:00.181652 lacss-0.3.1/lacss/train/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      257 2023-04-26 16:05:15.023476 lacss-0.3.1/lacss/train/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6686 2023-05-17 15:11:14.083243 lacss-0.3.1/lacss/train/__pycache__/loss.cpython-38.pyc
+-rw-r--r--   0        0        0      648 2023-04-28 14:28:40.891145 lacss-0.3.1/lacss/train/__pycache__/metric.cpython-38.pyc
+-rw-r--r--   0        0        0     4261 2023-03-16 23:08:03.154040 lacss-0.3.1/lacss/train/__pycache__/pytree.cpython-38.pyc
+-rw-r--r--   0        0        0     4680 2023-03-07 20:26:00.134879 lacss-0.3.1/lacss/train/__pycache__/strategy.cpython-310.pyc
+-rw-r--r--   0        0        0     4118 2023-04-28 14:28:40.802364 lacss-0.3.1/lacss/train/__pycache__/strategy.cpython-38.pyc
+-rw-r--r--   0        0        0     3496 2023-03-07 20:26:00.159397 lacss-0.3.1/lacss/train/__pycache__/trainer.cpython-310.pyc
+-rw-r--r--   0        0        0     6896 2023-05-17 17:49:39.333286 lacss-0.3.1/lacss/train/__pycache__/trainer.cpython-38.pyc
+-rw-r--r--   0        0        0     5272 2023-03-16 23:08:03.169159 lacss-0.3.1/lacss/train/__pycache__/wrapper.cpython-38.pyc
+-rw-r--r--   0        0        0      718 2023-04-21 18:45:48.299450 lacss-0.3.1/lacss/train/data/__init__.py
+-rw-r--r--   0        0        0      868 2023-03-07 20:25:59.860409 lacss-0.3.1/lacss/train/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      851 2023-04-26 16:05:15.050386 lacss-0.3.1/lacss/train/data/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4011 2023-03-07 20:25:59.910632 lacss-0.3.1/lacss/train/data/__pycache__/array_adapter.cpython-310.pyc
+-rw-r--r--   0        0        0     4005 2023-04-26 16:05:15.067195 lacss-0.3.1/lacss/train/data/__pycache__/array_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     6036 2023-03-07 20:25:59.794089 lacss-0.3.1/lacss/train/data/__pycache__/data_adapter.cpython-310.pyc
+-rw-r--r--   0        0        0     6093 2023-04-26 16:05:15.080415 lacss-0.3.1/lacss/train/data/__pycache__/data_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     5560 2023-03-07 20:25:59.837897 lacss-0.3.1/lacss/train/data/__pycache__/data_handler.cpython-310.pyc
+-rw-r--r--   0        0        0     5561 2023-04-26 16:05:15.114203 lacss-0.3.1/lacss/train/data/__pycache__/data_handler.cpython-38.pyc
+-rw-r--r--   0        0        0    11601 2023-03-07 20:25:59.891017 lacss-0.3.1/lacss/train/data/__pycache__/dataset.cpython-310.pyc
+-rw-r--r--   0        0        0    11577 2023-04-26 16:05:15.128310 lacss-0.3.1/lacss/train/data/__pycache__/dataset.cpython-38.pyc
+-rw-r--r--   0        0        0     3314 2023-03-07 20:25:59.948618 lacss-0.3.1/lacss/train/data/__pycache__/generator_adapter.cpython-310.pyc
+-rw-r--r--   0        0        0     3319 2023-04-26 16:05:15.141255 lacss-0.3.1/lacss/train/data/__pycache__/generator_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     2490 2023-03-07 20:25:59.735195 lacss-0.3.1/lacss/train/data/__pycache__/list_adapter.cpython-310.pyc
+-rw-r--r--   0        0        0     2515 2023-04-26 16:05:15.157133 lacss-0.3.1/lacss/train/data/__pycache__/list_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     3581 2023-03-07 20:25:59.741952 lacss-0.3.1/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-310.pyc
+-rw-r--r--   0        0        0     3562 2023-04-26 16:05:15.171168 lacss-0.3.1/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     3180 2023-03-07 20:25:59.763043 lacss-0.3.1/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-310.pyc
+-rw-r--r--   0        0        0     3167 2023-04-26 16:05:15.186154 lacss-0.3.1/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     6787 2023-03-07 20:25:59.810992 lacss-0.3.1/lacss/train/data/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     6796 2023-04-26 16:05:15.099537 lacss-0.3.1/lacss/train/data/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     4076 2023-04-21 18:45:48.325549 lacss-0.3.1/lacss/train/data/array_adapter.py
+-rw-r--r--   0        0        0     5529 2023-04-21 18:45:48.371676 lacss-0.3.1/lacss/train/data/data_adapter.py
+-rw-r--r--   0        0        0     6287 2023-04-21 18:45:48.396891 lacss-0.3.1/lacss/train/data/data_handler.py
+-rw-r--r--   0        0        0    10656 2023-04-21 18:45:48.433354 lacss-0.3.1/lacss/train/data/dataset.py
+-rw-r--r--   0        0        0     2599 2023-04-21 18:45:48.456058 lacss-0.3.1/lacss/train/data/generator_adapter.py
+-rw-r--r--   0        0        0     2105 2023-04-21 18:45:48.467534 lacss-0.3.1/lacss/train/data/list_adapter.py
+-rw-r--r--   0        0        0     3440 2023-04-21 18:45:48.479496 lacss-0.3.1/lacss/train/data/tf_dataset_adapter.py
+-rw-r--r--   0        0        0     2566 2023-04-21 18:45:48.526515 lacss-0.3.1/lacss/train/data/torch_dataloader_adapter.py
+-rw-r--r--   0        0        0     6394 2023-04-21 18:45:48.565291 lacss-0.3.1/lacss/train/data/utils.py
+-rw-r--r--   0        0        0     6826 2023-05-18 16:15:17.976482 lacss-0.3.1/lacss/train/loss.py
+-rw-r--r--   0        0        0      222 2023-04-28 13:52:59.277007 lacss-0.3.1/lacss/train/metric.py
+-rw-r--r--   0        0        0     4018 2023-04-28 14:03:41.907286 lacss-0.3.1/lacss/train/strategy.py
+-rw-r--r--   0        0        0     7437 2023-05-18 16:15:17.983603 lacss-0.3.1/lacss/train/trainer.py
+-rw-r--r--   0        0        0     4755 2023-05-17 12:27:49.626673 lacss-0.3.1/lacss/utils.py
+-rw-r--r--   0        0        0      810 2023-05-18 16:20:48.167902 lacss-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2875 1970-01-01 00:00:00.000000 lacss-0.3.1/PKG-INFO
```

### Comparing `lacss-0.3.0/LICENSE` & `lacss-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/data/generator.py` & `lacss-0.3.1/lacss/data/generator.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/data/parser.py` & `lacss-0.3.1/lacss/data/parser.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/deploy.py` & `lacss-0.3.1/lacss/deploy.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import optax
 from flax.core.frozen_dict import freeze, unfreeze
 from flax.training.train_state import TrainState
 
 import lacss.modules
 import lacss.train.strategy as strategy
 from lacss.ops import patches_to_label
+from lacss.train import Inputs
 
 _cached_partial = lru_cache(partial)
 
 
 def load_from_pretrained(pretrained):
     if os.path.isdir(pretrained):
         import json
@@ -98,14 +99,20 @@
                 iter(precompile_shape[0])
             except:
                 precompile_shape = [precompile_shape]
             for shape in precompile_shape:
                 x = np.zeros(shape)
                 _ = self.predict(x)
 
+    def __call__(self, inputs, **kwargs):
+
+        inputs_obj = Inputs.from_value(inputs)
+
+        return self.predict(*inputs_obj.args, **inputs_obj.kwargs, **kwargs)
+
     def predict(self, image, **kwargs):
 
         module, params = self.model
 
         if len(kwargs) > 0:
             apply_fn = _cached_partial(module.apply, **kwargs)
         else:
```

### Comparing `lacss-0.3.0/lacss/losses/auxiliary.py` & `lacss-0.3.1/lacss/losses/auxiliary.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/losses/detection.py` & `lacss-0.3.1/lacss/losses/detection.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/losses/instance.py` & `lacss-0.3.1/lacss/losses/instance.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/metrics/ranked.py` & `lacss-0.3.1/lacss/metrics/ranked.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/modules/auxiliary.py` & `lacss-0.3.1/lacss/modules/auxiliary.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/modules/common.py` & `lacss-0.3.1/lacss/modules/common.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/modules/convnext.py` & `lacss-0.3.1/lacss/modules/convnext.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/modules/detector.py` & `lacss-0.3.1/lacss/modules/detector.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,31 +68,36 @@
 
         scores = jnp.concatenate(scores, axis=0)
         locations = jnp.concatenate(locations, axis=0)
 
         # select topk
         if topk <= 0 or topk > scores.size:
             topk = scores.size
-        scores, selections = jax.lax.top_k(scores, topk)
-        locations = locations[selections]
 
         # refine
         if distance_threshold > 0:  # nms
+
+            scores, selections = jax.lax.top_k(scores, topk)
+            locations = locations[selections]
+
             threshold = 1 / distance_threshold / distance_threshold
             scores, locations = sorted_non_max_suppression(
                 scores,
                 locations,
                 output_size,
                 threshold,
                 score_threshold,
             )
+
         else:
-            is_valid = scores >= score_threshold
-            scores = jnp.where(is_valid, scores, -1.0)
-            locations = jnp.where(is_valid[:, None], locations, -1.0)
+
+            sel = jnp.where(scores >= score_threshold, size=output_size, fill_value=-1)
+            sel = sel[0]
+            scores = jnp.where(sel >= 0, scores[sel], -1.0)
+            locations = jnp.where((sel >= 0)[:, None], locations[sel], -1.0)
 
         return scores, locations
 
     def _gen_train_locations(self, gt_locations, pred_locations):
         """replacing gt_locations with pred_locations if the close enough
         gt_locations: [N, 2] tensor
         pred_locations: [M, 2] tensor, sorted with scores
@@ -153,28 +158,38 @@
                 pred_scores: [M] sorted, padded with -1
             }
         """
 
         scores = jax.lax.stop_gradient(scores)
         regressions = jax.lax.stop_gradient(regressions)
 
-        if training and self.max_proposal_offset <= 0:
-            return dict(
-                training_locations=gt_locations,
-            )
-        proposed_scores, proposed_locations = self._proposal_locations(
-            scores, regressions, training
-        )
-        outputs = dict(
-            pred_locations=proposed_locations,
-            pred_scores=proposed_scores,
-        )
         if training:
-            outputs.update(
-                dict(
-                    training_locations=self._gen_train_locations(
-                        gt_locations,
-                        proposed_locations,
-                    )
+
+            if self.max_proposal_offset <= 0:
+                return dict(
+                    training_locations=gt_locations,
                 )
+
+            proposed_scores, proposed_locations = self._proposal_locations(
+                scores, regressions, True
             )
+
+            outputs = dict(
+                pred_locations=proposed_locations,
+                pred_scores=proposed_scores,
+                training_locations=self._gen_train_locations(
+                    gt_locations,
+                    proposed_locations,
+                ),
+            )
+
+        else:
+
+            proposed_scores, proposed_locations = self._proposal_locations(
+                scores, regressions, False
+            )
+            outputs = dict(
+                pred_locations=proposed_locations,
+                pred_scores=proposed_scores,
+            )
+
         return outputs
```

### Comparing `lacss-0.3.0/lacss/modules/lacss.py` & `lacss-0.3.1/lacss/modules/lacss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/modules/lpn.py` & `lacss-0.3.1/lacss/modules/lpn.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/modules/resnet.py` & `lacss-0.3.1/lacss/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/modules/segmentor.py` & `lacss-0.3.1/lacss/modules/segmentor.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/modules/unet.py` & `lacss-0.3.1/lacss/modules/unet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/ops/boxes.py` & `lacss-0.3.1/lacss/ops/boxes.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/ops/image.py` & `lacss-0.3.1/lacss/ops/image.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/ops/locations.py` & `lacss-0.3.1/lacss/ops/locations.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/ops/masks.py` & `lacss-0.3.1/lacss/ops/masks.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/ops/nms.py` & `lacss-0.3.1/lacss/ops/nms.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/ops/patches.py` & `lacss-0.3.1/lacss/ops/patches.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/train/data/__init__.py` & `lacss-0.3.1/lacss/train/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/train/data/array_adapter.py` & `lacss-0.3.1/lacss/train/data/array_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/train/data/data_adapter.py` & `lacss-0.3.1/lacss/train/data/data_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/train/data/data_handler.py` & `lacss-0.3.1/lacss/train/data/data_handler.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/train/data/dataset.py` & `lacss-0.3.1/lacss/train/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/train/data/generator_adapter.py` & `lacss-0.3.1/lacss/train/data/generator_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/train/data/list_adapter.py` & `lacss-0.3.1/lacss/train/data/list_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/train/data/tf_dataset_adapter.py` & `lacss-0.3.1/lacss/train/data/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/train/data/torch_dataloader_adapter.py` & `lacss-0.3.1/lacss/train/data/torch_dataloader_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/train/data/utils.py` & `lacss-0.3.1/lacss/train/data/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/train/loss.py` & `lacss-0.3.1/lacss/train/loss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/train/strategy.py` & `lacss-0.3.1/lacss/train/strategy.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/train/trainer.py` & `lacss-0.3.1/lacss/train/trainer.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.0/lacss/utils.py` & `lacss-0.3.1/lacss/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import dataclasses
 import re
 import typing as tp
 
+import jax.numpy as jnp
 import numpy as np
 from flax import struct
 
 from .ops import bboxes_of_patches
 
 InputLike = tp.Union[tp.Any, tp.Tuple[tp.Any, ...], tp.Dict[str, tp.Any], "Inputs"]
 
@@ -94,59 +95,67 @@
             return cls(args=(value,))
 
 
 def _to_str(p):
     return "".join(p.astype(int).reshape(-1).astype(str).tolist())
 
 
-def format_predictions(pred, mask=None, threshold=0.5):
-    """
+def format_predictions(pred, mask=None, encode_patch=True, threshold=0.5):
+    """Produce more readable data from model predictions
     Args:
         pred: model output without batch dim
-            instance_output: [n, patch_size, patch_size] float
-            instance_yx, instance_xc: [n, patch_size, patch_size]
-            pred_scores: [n]
-            instance_mask: [n, 1, 1]
         mask: optional mask selecting cells
-        threshold: float
-    Returns:
-        bboxes: [n, 4] int64
-        encodings: [n] string
+        threshold: float patch threshold
+    Returns: dict(locations, scores, centroids, bboxes, encodings)
     """
-    patches = np.asarray(pred["instance_output"]) > threshold
-    yc = np.asarray(pred["instance_yc"])
-    xc = np.asarray(pred["instance_xc"])
-    scores = np.asarray(pred["pred_scores"])
-    bboxes = np.asarray(bboxes_of_patches(pred))
 
-    is_valid = pred["instance_mask"].squeeze(axis=(-1, -2))
-    is_valid & patches.any(axis=(1, 2))  # no empty patches
-    if mask is not None:
-        is_valid &= mask
+    patches = pred["instance_output"] >= threshold
+    yc = pred["instance_yc"]
+    xc = pred["instance_xc"]
 
-    patches = patches[is_valid]
-    yc = yc[is_valid]
-    xc = xc[is_valid]
-    scores = scores[is_valid]
-
-    encodings = []
-    for (r0, c0, r1, c1), y0, x0, p in zip(bboxes, yc[:, 0, 0], xc[:, 0, 0], patches):
-        roi = p[r0 - y0 : r1 - y0, c0 - x0 : c1 - x0]
-        encodings.append(_to_str(roi))
+    bboxes = bboxes_of_patches(pred)
 
     n_pixels = np.count_nonzero(patches, axis=(1, 2))
-    yx = np.stack(
+    centroids = jnp.stack(
         [
             (patches * yc).sum(axis=(1, 2)) / n_pixels,
             (patches * xc).sum(axis=(1, 2)) / n_pixels,
         ],
         axis=-1,
     )  # centroid
 
-    return bboxes, encodings, scores, yx
+    outputs = dict(
+        locations=pred["pred_locations"],
+        scores=pred["pred_scores"],
+        centroids=centroids,
+        bboxes=bboxes,
+    )
+
+    is_valid = pred["instance_mask"].squeeze(axis=(-1, -2))
+    is_valid &= patches.any(axis=(1, 2))  # no empty patches
+    if mask is not None:
+        is_valid &= mask
+
+    outputs = {k: np.asarray(v)[is_valid] for k, v in outputs.items()}
+
+    if encode_patch:
+
+        encodings = []
+        patches = np.asarray(patches)[is_valid]
+        y0 = np.asarray(yc)[is_valid, 0, 0]
+        x0 = np.asarray(xc)[is_valid, 0, 0]
+        boxes = np.asarray(outputs["bboxes"]) - np.stack([y0, x0, y0, x0], axis=-1)
+
+        for box, patch in zip(boxes, patches):
+            roi = patch[box[0] : box[2], box[1] : box[3]]
+            encodings.append(_to_str(roi))
+
+        outputs["encodings"] = encodings
+
+    return outputs
 
 
 def show_images(imgs, locs=None, **kwargs):
 
     import matplotlib.patches
     import matplotlib.pyplot as plt
```

### Comparing `lacss-0.3.0/pyproject.toml` & `lacss-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacss"
-version = "0.3.0"
+version = "0.3.1"
 description = "Cell segmentation and tracking"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
```

