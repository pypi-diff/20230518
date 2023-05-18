# Comparing `tmp/lacss-0.3.1.tar.gz` & `tmp/lacss-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacss-0.3.1.tar", max compression
+gzip compressed data, was "lacss-0.3.2.tar", max compression
```

## Comparing `lacss-0.3.1.tar` & `lacss-0.3.2.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0     1062 2023-04-21 18:45:47.667328 lacss-0.3.1/LICENSE
--rw-r--r--   0        0        0     2188 2023-05-18 16:20:17.041288 lacss-0.3.1/README.md
--rw-r--r--   0        0        0       58 2023-03-07 20:26:00.699876 lacss-0.3.1/lacss/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0       65 2023-04-21 18:45:47.772087 lacss-0.3.1/lacss/__init__.py
--rw-r--r--   0        0        0      580 2023-05-18 16:12:05.535144 lacss-0.3.1/lacss/app/da.py
--rw-r--r--   0        0        0       47 2023-04-21 18:45:47.795653 lacss-0.3.1/lacss/data/__init__.py
--rw-r--r--   0        0        0      194 2023-03-07 20:26:00.289795 lacss-0.3.1/lacss/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      189 2023-04-26 16:05:13.976775 lacss-0.3.1/lacss/data/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4337 2023-03-07 20:26:00.277190 lacss-0.3.1/lacss/data/__pycache__/generator.cpython-310.pyc
--rw-r--r--   0        0        0     4422 2023-04-26 16:05:14.005891 lacss-0.3.1/lacss/data/__pycache__/generator.cpython-38.pyc
--rw-r--r--   0        0        0     3648 2023-03-07 20:26:00.257796 lacss-0.3.1/lacss/data/__pycache__/parser.cpython-310.pyc
--rw-r--r--   0        0        0     5681 2023-04-26 16:05:14.758099 lacss-0.3.1/lacss/data/__pycache__/parser.cpython-38.pyc
--rw-r--r--   0        0        0     6063 2023-04-21 18:45:47.824902 lacss-0.3.1/lacss/data/generator.py
--rw-r--r--   0        0        0     9160 2023-04-21 18:45:47.837649 lacss-0.3.1/lacss/data/parser.py
--rw-r--r--   0        0        0     3307 2023-05-17 12:27:49.433436 lacss-0.3.1/lacss/deploy.py
--rw-r--r--   0        0        0       74 2023-05-18 16:15:17.877065 lacss-0.3.1/lacss/losses/__init__.py
--rw-r--r--   0        0        0      216 2023-03-07 20:26:00.790038 lacss-0.3.1/lacss/losses/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      231 2023-05-17 13:50:37.368341 lacss-0.3.1/lacss/losses/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5330 2023-05-17 19:06:53.529626 lacss-0.3.1/lacss/losses/__pycache__/auxiliary.cpython-38.pyc
--rw-r--r--   0        0        0     2049 2023-03-07 20:26:00.816719 lacss-0.3.1/lacss/losses/__pycache__/auxnet.cpython-310.pyc
--rw-r--r--   0        0        0     2076 2023-03-07 20:26:00.777737 lacss-0.3.1/lacss/losses/__pycache__/auxnet.cpython-38.pyc
--rw-r--r--   0        0        0     3271 2023-03-07 20:26:00.744429 lacss-0.3.1/lacss/losses/__pycache__/detection.cpython-310.pyc
--rw-r--r--   0        0        0     3304 2023-05-17 13:50:37.737229 lacss-0.3.1/lacss/losses/__pycache__/detection.cpython-38.pyc
--rw-r--r--   0        0        0     3243 2023-03-07 20:26:00.758307 lacss-0.3.1/lacss/losses/__pycache__/instance.cpython-310.pyc
--rw-r--r--   0        0        0     4451 2023-05-17 13:50:40.487927 lacss-0.3.1/lacss/losses/__pycache__/instance.cpython-38.pyc
--rw-r--r--   0        0        0     1986 2023-05-17 19:06:55.091616 lacss-0.3.1/lacss/losses/__pycache__/lacss.cpython-38.pyc
--rw-r--r--   0        0        0     5087 2023-03-07 20:26:00.750432 lacss-0.3.1/lacss/losses/__pycache__/loss.cpython-38.pyc
--rw-r--r--   0        0        0     5524 2023-05-18 16:15:17.883556 lacss-0.3.1/lacss/losses/auxiliary.py
--rw-r--r--   0        0        0     3189 2023-05-18 16:15:17.890613 lacss-0.3.1/lacss/losses/detection.py
--rw-r--r--   0        0        0     8278 2023-05-18 16:15:17.897817 lacss-0.3.1/lacss/losses/instance.py
--rw-r--r--   0        0        0       56 2023-04-21 18:45:47.932120 lacss-0.3.1/lacss/metrics/__init__.py
--rw-r--r--   0        0        0      176 2023-03-07 20:26:00.875358 lacss-0.3.1/lacss/metrics/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      219 2023-04-26 16:05:15.350411 lacss-0.3.1/lacss/metrics/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      650 2023-03-17 12:50:11.457103 lacss-0.3.1/lacss/metrics/__pycache__/metric.cpython-38.pyc
--rw-r--r--   0        0        0     5469 2023-03-07 20:26:00.863743 lacss-0.3.1/lacss/metrics/__pycache__/ranked.cpython-310.pyc
--rw-r--r--   0        0        0     5809 2023-04-26 16:05:15.382370 lacss-0.3.1/lacss/metrics/__pycache__/ranked.cpython-38.pyc
--rw-r--r--   0        0        0     5547 2023-04-21 18:45:47.940716 lacss-0.3.1/lacss/metrics/ranked.py
--rw-r--r--   0        0        0      216 2023-04-28 14:03:41.857622 lacss-0.3.1/lacss/modules/__init__.py
--rw-r--r--   0        0        0      484 2023-03-07 20:26:00.615885 lacss-0.3.1/lacss/modules/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      435 2023-04-28 14:28:40.915459 lacss-0.3.1/lacss/modules/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3869 2023-05-17 15:11:16.098273 lacss-0.3.1/lacss/modules/__pycache__/auxiliary.cpython-38.pyc
--rw-r--r--   0        0        0     1131 2023-03-07 20:26:00.643794 lacss-0.3.1/lacss/modules/__pycache__/auxnet.cpython-310.pyc
--rw-r--r--   0        0        0     1066 2023-03-07 20:26:00.591783 lacss-0.3.1/lacss/modules/__pycache__/auxnet.cpython-38.pyc
--rw-r--r--   0        0        0     4225 2023-05-17 15:22:00.187532 lacss-0.3.1/lacss/modules/__pycache__/common.cpython-38.pyc
--rw-r--r--   0        0        0     8008 2023-03-07 20:26:00.636668 lacss-0.3.1/lacss/modules/__pycache__/convnext.cpython-310.pyc
--rw-r--r--   0        0        0     6398 2023-04-28 14:28:41.147671 lacss-0.3.1/lacss/modules/__pycache__/convnext.cpython-38.pyc
--rw-r--r--   0        0        0     5064 2023-03-07 20:26:00.531471 lacss-0.3.1/lacss/modules/__pycache__/detector.cpython-310.pyc
--rw-r--r--   0        0        0     4848 2023-05-15 14:38:02.594877 lacss-0.3.1/lacss/modules/__pycache__/detector.cpython-38.pyc
--rw-r--r--   0        0        0     3995 2023-03-07 20:26:00.556378 lacss-0.3.1/lacss/modules/__pycache__/lacss.cpython-310.pyc
--rw-r--r--   0        0        0     3430 2023-05-17 19:02:36.950020 lacss-0.3.1/lacss/modules/__pycache__/lacss.cpython-38.pyc
--rw-r--r--   0        0        0     3129 2023-03-07 20:26:00.526426 lacss-0.3.1/lacss/modules/__pycache__/lpn.cpython-310.pyc
--rw-r--r--   0        0        0     2985 2023-05-18 14:56:00.640109 lacss-0.3.1/lacss/modules/__pycache__/lpn.cpython-38.pyc
--rw-r--r--   0        0        0     5339 2023-03-07 20:26:00.576473 lacss-0.3.1/lacss/modules/__pycache__/resnet.cpython-310.pyc
--rw-r--r--   0        0        0     3578 2023-04-26 16:05:15.594809 lacss-0.3.1/lacss/modules/__pycache__/resnet.cpython-38.pyc
--rw-r--r--   0        0        0     1680 2023-03-07 20:26:00.571302 lacss-0.3.1/lacss/modules/__pycache__/se_net.cpython-310.pyc
--rw-r--r--   0        0        0      147 2023-03-07 20:26:00.489800 lacss-0.3.1/lacss/modules/__pycache__/se_net.cpython-38.pyc
--rw-r--r--   0        0        0     4346 2023-03-07 20:26:00.597085 lacss-0.3.1/lacss/modules/__pycache__/segmentor.cpython-310.pyc
--rw-r--r--   0        0        0     3951 2023-05-17 13:53:10.140274 lacss-0.3.1/lacss/modules/__pycache__/segmentor.cpython-38.pyc
--rw-r--r--   0        0        0      969 2023-03-07 20:26:00.631053 lacss-0.3.1/lacss/modules/__pycache__/types.cpython-310.pyc
--rw-r--r--   0        0        0     1424 2023-03-07 20:26:00.503425 lacss-0.3.1/lacss/modules/__pycache__/types.cpython-38.pyc
--rw-r--r--   0        0        0     3097 2023-03-07 20:26:00.546308 lacss-0.3.1/lacss/modules/__pycache__/unet.cpython-310.pyc
--rw-r--r--   0        0        0     2211 2023-04-28 14:28:41.128007 lacss-0.3.1/lacss/modules/__pycache__/unet.cpython-38.pyc
--rw-r--r--   0        0        0     7267 2023-03-07 20:26:00.509827 lacss-0.3.1/lacss/modules/__pycache__/xcit.cpython-310.pyc
--rw-r--r--   0        0        0     7215 2023-03-07 20:26:00.607719 lacss-0.3.1/lacss/modules/__pycache__/xcit.cpython-38.pyc
--rw-r--r--   0        0        0     3171 2023-05-18 16:15:17.906763 lacss-0.3.1/lacss/modules/auxiliary.py
--rw-r--r--   0        0        0     2270 2023-05-18 16:15:17.916458 lacss-0.3.1/lacss/modules/common.py
--rw-r--r--   0        0        0     6557 2023-04-28 14:03:41.873034 lacss-0.3.1/lacss/modules/convnext.py
--rw-r--r--   0        0        0     6579 2023-05-15 14:29:30.716593 lacss-0.3.1/lacss/modules/detector.py
--rw-r--r--   0        0        0     3813 2023-05-18 16:15:17.927778 lacss-0.3.1/lacss/modules/lacss.py
--rw-r--r--   0        0        0     2934 2023-05-18 16:15:17.938204 lacss-0.3.1/lacss/modules/lpn.py
--rw-r--r--   0        0        0     3771 2023-04-21 18:45:48.045107 lacss-0.3.1/lacss/modules/resnet.py
--rw-r--r--   0        0        0     4595 2023-05-18 16:15:17.967503 lacss-0.3.1/lacss/modules/segmentor.py
--rw-r--r--   0        0        0     1979 2023-04-28 14:03:41.880651 lacss-0.3.1/lacss/modules/unet.py
--rw-r--r--   0        0        0      155 2023-04-21 18:45:48.079314 lacss-0.3.1/lacss/ops/__init__.py
--rw-r--r--   0        0        0      260 2023-03-07 20:26:00.414720 lacss-0.3.1/lacss/ops/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      255 2023-04-26 16:05:14.845951 lacss-0.3.1/lacss/ops/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1804 2023-03-07 20:26:00.409875 lacss-0.3.1/lacss/ops/__pycache__/boxes.cpython-310.pyc
--rw-r--r--   0        0        0     1987 2023-04-26 16:05:14.869998 lacss-0.3.1/lacss/ops/__pycache__/boxes.cpython-38.pyc
--rw-r--r--   0        0        0     1121 2023-03-07 20:26:00.435101 lacss-0.3.1/lacss/ops/__pycache__/image.cpython-310.pyc
--rw-r--r--   0        0        0     2559 2023-04-26 16:05:14.898406 lacss-0.3.1/lacss/ops/__pycache__/image.cpython-38.pyc
--rw-r--r--   0        0        0     2379 2023-03-07 20:26:00.429728 lacss-0.3.1/lacss/ops/__pycache__/locations.cpython-310.pyc
--rw-r--r--   0        0        0     2347 2023-04-26 16:05:14.926967 lacss-0.3.1/lacss/ops/__pycache__/locations.cpython-38.pyc
--rw-r--r--   0        0        0     5827 2023-03-07 20:26:00.371538 lacss-0.3.1/lacss/ops/__pycache__/masks.cpython-310.pyc
--rw-r--r--   0        0        0     5806 2023-04-26 16:05:14.944134 lacss-0.3.1/lacss/ops/__pycache__/masks.cpython-38.pyc
--rw-r--r--   0        0        0     3845 2023-03-07 20:26:00.404805 lacss-0.3.1/lacss/ops/__pycache__/nms.cpython-310.pyc
--rw-r--r--   0        0        0     3857 2023-04-26 16:05:14.998332 lacss-0.3.1/lacss/ops/__pycache__/nms.cpython-38.pyc
--rw-r--r--   0        0        0     5649 2023-03-07 20:26:00.394465 lacss-0.3.1/lacss/ops/__pycache__/patches.cpython-310.pyc
--rw-r--r--   0        0        0     7853 2023-04-26 16:05:14.981060 lacss-0.3.1/lacss/ops/__pycache__/patches.cpython-38.pyc
--rw-r--r--   0        0        0     2175 2023-04-21 18:45:48.091110 lacss-0.3.1/lacss/ops/boxes.py
--rw-r--r--   0        0        0     2218 2023-04-21 18:45:48.100899 lacss-0.3.1/lacss/ops/image.py
--rw-r--r--   0        0        0     2739 2023-04-21 18:45:48.114632 lacss-0.3.1/lacss/ops/locations.py
--rw-r--r--   0        0        0     5967 2023-04-21 18:45:48.142871 lacss-0.3.1/lacss/ops/masks.py
--rw-r--r--   0        0        0     4704 2023-04-21 18:45:48.169083 lacss-0.3.1/lacss/ops/nms.py
--rw-r--r--   0        0        0     9245 2023-04-21 18:45:48.177726 lacss-0.3.1/lacss/ops/patches.py
--rw-r--r--   0        0        0       63 2023-05-17 12:27:49.580967 lacss-0.3.1/lacss/tracking/__init__.py
--rw-r--r--   0        0        0      205 2023-05-14 18:38:38.567521 lacss-0.3.1/lacss/tracking/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2689 2023-05-15 15:16:43.449032 lacss-0.3.1/lacss/tracking/__pycache__/predict.cpython-38.pyc
--rw-r--r--   0        0        0     6517 2023-05-15 18:37:20.371555 lacss-0.3.1/lacss/tracking/__pycache__/smc.cpython-38.pyc
--rw-r--r--   0        0        0     4358 2023-05-15 18:37:20.409926 lacss-0.3.1/lacss/tracking/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     3340 2023-05-17 12:27:49.587345 lacss-0.3.1/lacss/tracking/predict.py
--rw-r--r--   0        0        0     6741 2023-05-17 12:27:49.597252 lacss-0.3.1/lacss/tracking/smc.py
--rw-r--r--   0        0        0     5646 2023-05-17 12:27:49.616793 lacss-0.3.1/lacss/tracking/utils.py
--rw-r--r--   0        0        0       99 2023-04-21 18:45:48.241245 lacss-0.3.1/lacss/train/__init__.py
--rw-r--r--   0        0        0      191 2023-03-07 20:26:00.181652 lacss-0.3.1/lacss/train/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      257 2023-04-26 16:05:15.023476 lacss-0.3.1/lacss/train/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     6686 2023-05-17 15:11:14.083243 lacss-0.3.1/lacss/train/__pycache__/loss.cpython-38.pyc
--rw-r--r--   0        0        0      648 2023-04-28 14:28:40.891145 lacss-0.3.1/lacss/train/__pycache__/metric.cpython-38.pyc
--rw-r--r--   0        0        0     4261 2023-03-16 23:08:03.154040 lacss-0.3.1/lacss/train/__pycache__/pytree.cpython-38.pyc
--rw-r--r--   0        0        0     4680 2023-03-07 20:26:00.134879 lacss-0.3.1/lacss/train/__pycache__/strategy.cpython-310.pyc
--rw-r--r--   0        0        0     4118 2023-04-28 14:28:40.802364 lacss-0.3.1/lacss/train/__pycache__/strategy.cpython-38.pyc
--rw-r--r--   0        0        0     3496 2023-03-07 20:26:00.159397 lacss-0.3.1/lacss/train/__pycache__/trainer.cpython-310.pyc
--rw-r--r--   0        0        0     6896 2023-05-17 17:49:39.333286 lacss-0.3.1/lacss/train/__pycache__/trainer.cpython-38.pyc
--rw-r--r--   0        0        0     5272 2023-03-16 23:08:03.169159 lacss-0.3.1/lacss/train/__pycache__/wrapper.cpython-38.pyc
--rw-r--r--   0        0        0      718 2023-04-21 18:45:48.299450 lacss-0.3.1/lacss/train/data/__init__.py
--rw-r--r--   0        0        0      868 2023-03-07 20:25:59.860409 lacss-0.3.1/lacss/train/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      851 2023-04-26 16:05:15.050386 lacss-0.3.1/lacss/train/data/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4011 2023-03-07 20:25:59.910632 lacss-0.3.1/lacss/train/data/__pycache__/array_adapter.cpython-310.pyc
--rw-r--r--   0        0        0     4005 2023-04-26 16:05:15.067195 lacss-0.3.1/lacss/train/data/__pycache__/array_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     6036 2023-03-07 20:25:59.794089 lacss-0.3.1/lacss/train/data/__pycache__/data_adapter.cpython-310.pyc
--rw-r--r--   0        0        0     6093 2023-04-26 16:05:15.080415 lacss-0.3.1/lacss/train/data/__pycache__/data_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     5560 2023-03-07 20:25:59.837897 lacss-0.3.1/lacss/train/data/__pycache__/data_handler.cpython-310.pyc
--rw-r--r--   0        0        0     5561 2023-04-26 16:05:15.114203 lacss-0.3.1/lacss/train/data/__pycache__/data_handler.cpython-38.pyc
--rw-r--r--   0        0        0    11601 2023-03-07 20:25:59.891017 lacss-0.3.1/lacss/train/data/__pycache__/dataset.cpython-310.pyc
--rw-r--r--   0        0        0    11577 2023-04-26 16:05:15.128310 lacss-0.3.1/lacss/train/data/__pycache__/dataset.cpython-38.pyc
--rw-r--r--   0        0        0     3314 2023-03-07 20:25:59.948618 lacss-0.3.1/lacss/train/data/__pycache__/generator_adapter.cpython-310.pyc
--rw-r--r--   0        0        0     3319 2023-04-26 16:05:15.141255 lacss-0.3.1/lacss/train/data/__pycache__/generator_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     2490 2023-03-07 20:25:59.735195 lacss-0.3.1/lacss/train/data/__pycache__/list_adapter.cpython-310.pyc
--rw-r--r--   0        0        0     2515 2023-04-26 16:05:15.157133 lacss-0.3.1/lacss/train/data/__pycache__/list_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     3581 2023-03-07 20:25:59.741952 lacss-0.3.1/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-310.pyc
--rw-r--r--   0        0        0     3562 2023-04-26 16:05:15.171168 lacss-0.3.1/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     3180 2023-03-07 20:25:59.763043 lacss-0.3.1/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-310.pyc
--rw-r--r--   0        0        0     3167 2023-04-26 16:05:15.186154 lacss-0.3.1/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     6787 2023-03-07 20:25:59.810992 lacss-0.3.1/lacss/train/data/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     6796 2023-04-26 16:05:15.099537 lacss-0.3.1/lacss/train/data/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     4076 2023-04-21 18:45:48.325549 lacss-0.3.1/lacss/train/data/array_adapter.py
--rw-r--r--   0        0        0     5529 2023-04-21 18:45:48.371676 lacss-0.3.1/lacss/train/data/data_adapter.py
--rw-r--r--   0        0        0     6287 2023-04-21 18:45:48.396891 lacss-0.3.1/lacss/train/data/data_handler.py
--rw-r--r--   0        0        0    10656 2023-04-21 18:45:48.433354 lacss-0.3.1/lacss/train/data/dataset.py
--rw-r--r--   0        0        0     2599 2023-04-21 18:45:48.456058 lacss-0.3.1/lacss/train/data/generator_adapter.py
--rw-r--r--   0        0        0     2105 2023-04-21 18:45:48.467534 lacss-0.3.1/lacss/train/data/list_adapter.py
--rw-r--r--   0        0        0     3440 2023-04-21 18:45:48.479496 lacss-0.3.1/lacss/train/data/tf_dataset_adapter.py
--rw-r--r--   0        0        0     2566 2023-04-21 18:45:48.526515 lacss-0.3.1/lacss/train/data/torch_dataloader_adapter.py
--rw-r--r--   0        0        0     6394 2023-04-21 18:45:48.565291 lacss-0.3.1/lacss/train/data/utils.py
--rw-r--r--   0        0        0     6826 2023-05-18 16:15:17.976482 lacss-0.3.1/lacss/train/loss.py
--rw-r--r--   0        0        0      222 2023-04-28 13:52:59.277007 lacss-0.3.1/lacss/train/metric.py
--rw-r--r--   0        0        0     4018 2023-04-28 14:03:41.907286 lacss-0.3.1/lacss/train/strategy.py
--rw-r--r--   0        0        0     7437 2023-05-18 16:15:17.983603 lacss-0.3.1/lacss/train/trainer.py
--rw-r--r--   0        0        0     4755 2023-05-17 12:27:49.626673 lacss-0.3.1/lacss/utils.py
--rw-r--r--   0        0        0      810 2023-05-18 16:20:48.167902 lacss-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2875 1970-01-01 00:00:00.000000 lacss-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-21 18:45:47.667328 lacss-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2184 2023-05-18 16:28:06.120257 lacss-0.3.2/README.md
+-rw-r--r--   0        0        0       58 2023-03-07 20:26:00.699876 lacss-0.3.2/lacss/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0       65 2023-04-21 18:45:47.772087 lacss-0.3.2/lacss/__init__.py
+-rw-r--r--   0        0        0      580 2023-05-18 16:12:05.535144 lacss-0.3.2/lacss/app/da.py
+-rw-r--r--   0        0        0       47 2023-04-21 18:45:47.795653 lacss-0.3.2/lacss/data/__init__.py
+-rw-r--r--   0        0        0      194 2023-03-07 20:26:00.289795 lacss-0.3.2/lacss/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      189 2023-04-26 16:05:13.976775 lacss-0.3.2/lacss/data/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4337 2023-03-07 20:26:00.277190 lacss-0.3.2/lacss/data/__pycache__/generator.cpython-310.pyc
+-rw-r--r--   0        0        0     4422 2023-04-26 16:05:14.005891 lacss-0.3.2/lacss/data/__pycache__/generator.cpython-38.pyc
+-rw-r--r--   0        0        0     3648 2023-03-07 20:26:00.257796 lacss-0.3.2/lacss/data/__pycache__/parser.cpython-310.pyc
+-rw-r--r--   0        0        0     5681 2023-04-26 16:05:14.758099 lacss-0.3.2/lacss/data/__pycache__/parser.cpython-38.pyc
+-rw-r--r--   0        0        0     6063 2023-04-21 18:45:47.824902 lacss-0.3.2/lacss/data/generator.py
+-rw-r--r--   0        0        0     9160 2023-04-21 18:45:47.837649 lacss-0.3.2/lacss/data/parser.py
+-rw-r--r--   0        0        0     3307 2023-05-17 12:27:49.433436 lacss-0.3.2/lacss/deploy.py
+-rw-r--r--   0        0        0       74 2023-05-18 16:15:17.877065 lacss-0.3.2/lacss/losses/__init__.py
+-rw-r--r--   0        0        0      216 2023-03-07 20:26:00.790038 lacss-0.3.2/lacss/losses/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      231 2023-05-17 13:50:37.368341 lacss-0.3.2/lacss/losses/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5330 2023-05-17 19:06:53.529626 lacss-0.3.2/lacss/losses/__pycache__/auxiliary.cpython-38.pyc
+-rw-r--r--   0        0        0     2049 2023-03-07 20:26:00.816719 lacss-0.3.2/lacss/losses/__pycache__/auxnet.cpython-310.pyc
+-rw-r--r--   0        0        0     2076 2023-03-07 20:26:00.777737 lacss-0.3.2/lacss/losses/__pycache__/auxnet.cpython-38.pyc
+-rw-r--r--   0        0        0     3271 2023-03-07 20:26:00.744429 lacss-0.3.2/lacss/losses/__pycache__/detection.cpython-310.pyc
+-rw-r--r--   0        0        0     3304 2023-05-17 13:50:37.737229 lacss-0.3.2/lacss/losses/__pycache__/detection.cpython-38.pyc
+-rw-r--r--   0        0        0     3243 2023-03-07 20:26:00.758307 lacss-0.3.2/lacss/losses/__pycache__/instance.cpython-310.pyc
+-rw-r--r--   0        0        0     4451 2023-05-17 13:50:40.487927 lacss-0.3.2/lacss/losses/__pycache__/instance.cpython-38.pyc
+-rw-r--r--   0        0        0     1986 2023-05-17 19:06:55.091616 lacss-0.3.2/lacss/losses/__pycache__/lacss.cpython-38.pyc
+-rw-r--r--   0        0        0     5087 2023-03-07 20:26:00.750432 lacss-0.3.2/lacss/losses/__pycache__/loss.cpython-38.pyc
+-rw-r--r--   0        0        0     5524 2023-05-18 16:15:17.883556 lacss-0.3.2/lacss/losses/auxiliary.py
+-rw-r--r--   0        0        0     3189 2023-05-18 16:15:17.890613 lacss-0.3.2/lacss/losses/detection.py
+-rw-r--r--   0        0        0     8278 2023-05-18 16:15:17.897817 lacss-0.3.2/lacss/losses/instance.py
+-rw-r--r--   0        0        0       56 2023-04-21 18:45:47.932120 lacss-0.3.2/lacss/metrics/__init__.py
+-rw-r--r--   0        0        0      176 2023-03-07 20:26:00.875358 lacss-0.3.2/lacss/metrics/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      219 2023-04-26 16:05:15.350411 lacss-0.3.2/lacss/metrics/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      650 2023-03-17 12:50:11.457103 lacss-0.3.2/lacss/metrics/__pycache__/metric.cpython-38.pyc
+-rw-r--r--   0        0        0     5469 2023-03-07 20:26:00.863743 lacss-0.3.2/lacss/metrics/__pycache__/ranked.cpython-310.pyc
+-rw-r--r--   0        0        0     5809 2023-04-26 16:05:15.382370 lacss-0.3.2/lacss/metrics/__pycache__/ranked.cpython-38.pyc
+-rw-r--r--   0        0        0     5547 2023-04-21 18:45:47.940716 lacss-0.3.2/lacss/metrics/ranked.py
+-rw-r--r--   0        0        0      216 2023-04-28 14:03:41.857622 lacss-0.3.2/lacss/modules/__init__.py
+-rw-r--r--   0        0        0      484 2023-03-07 20:26:00.615885 lacss-0.3.2/lacss/modules/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      435 2023-04-28 14:28:40.915459 lacss-0.3.2/lacss/modules/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3869 2023-05-17 15:11:16.098273 lacss-0.3.2/lacss/modules/__pycache__/auxiliary.cpython-38.pyc
+-rw-r--r--   0        0        0     1131 2023-03-07 20:26:00.643794 lacss-0.3.2/lacss/modules/__pycache__/auxnet.cpython-310.pyc
+-rw-r--r--   0        0        0     1066 2023-03-07 20:26:00.591783 lacss-0.3.2/lacss/modules/__pycache__/auxnet.cpython-38.pyc
+-rw-r--r--   0        0        0     4225 2023-05-17 15:22:00.187532 lacss-0.3.2/lacss/modules/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0        0        0     8008 2023-03-07 20:26:00.636668 lacss-0.3.2/lacss/modules/__pycache__/convnext.cpython-310.pyc
+-rw-r--r--   0        0        0     6398 2023-04-28 14:28:41.147671 lacss-0.3.2/lacss/modules/__pycache__/convnext.cpython-38.pyc
+-rw-r--r--   0        0        0     5064 2023-03-07 20:26:00.531471 lacss-0.3.2/lacss/modules/__pycache__/detector.cpython-310.pyc
+-rw-r--r--   0        0        0     4848 2023-05-15 14:38:02.594877 lacss-0.3.2/lacss/modules/__pycache__/detector.cpython-38.pyc
+-rw-r--r--   0        0        0     3995 2023-03-07 20:26:00.556378 lacss-0.3.2/lacss/modules/__pycache__/lacss.cpython-310.pyc
+-rw-r--r--   0        0        0     3430 2023-05-17 19:02:36.950020 lacss-0.3.2/lacss/modules/__pycache__/lacss.cpython-38.pyc
+-rw-r--r--   0        0        0     3129 2023-03-07 20:26:00.526426 lacss-0.3.2/lacss/modules/__pycache__/lpn.cpython-310.pyc
+-rw-r--r--   0        0        0     2985 2023-05-18 14:56:00.640109 lacss-0.3.2/lacss/modules/__pycache__/lpn.cpython-38.pyc
+-rw-r--r--   0        0        0     5339 2023-03-07 20:26:00.576473 lacss-0.3.2/lacss/modules/__pycache__/resnet.cpython-310.pyc
+-rw-r--r--   0        0        0     3578 2023-04-26 16:05:15.594809 lacss-0.3.2/lacss/modules/__pycache__/resnet.cpython-38.pyc
+-rw-r--r--   0        0        0     1680 2023-03-07 20:26:00.571302 lacss-0.3.2/lacss/modules/__pycache__/se_net.cpython-310.pyc
+-rw-r--r--   0        0        0      147 2023-03-07 20:26:00.489800 lacss-0.3.2/lacss/modules/__pycache__/se_net.cpython-38.pyc
+-rw-r--r--   0        0        0     4346 2023-03-07 20:26:00.597085 lacss-0.3.2/lacss/modules/__pycache__/segmentor.cpython-310.pyc
+-rw-r--r--   0        0        0     3951 2023-05-17 13:53:10.140274 lacss-0.3.2/lacss/modules/__pycache__/segmentor.cpython-38.pyc
+-rw-r--r--   0        0        0      969 2023-03-07 20:26:00.631053 lacss-0.3.2/lacss/modules/__pycache__/types.cpython-310.pyc
+-rw-r--r--   0        0        0     1424 2023-03-07 20:26:00.503425 lacss-0.3.2/lacss/modules/__pycache__/types.cpython-38.pyc
+-rw-r--r--   0        0        0     3097 2023-03-07 20:26:00.546308 lacss-0.3.2/lacss/modules/__pycache__/unet.cpython-310.pyc
+-rw-r--r--   0        0        0     2211 2023-04-28 14:28:41.128007 lacss-0.3.2/lacss/modules/__pycache__/unet.cpython-38.pyc
+-rw-r--r--   0        0        0     7267 2023-03-07 20:26:00.509827 lacss-0.3.2/lacss/modules/__pycache__/xcit.cpython-310.pyc
+-rw-r--r--   0        0        0     7215 2023-03-07 20:26:00.607719 lacss-0.3.2/lacss/modules/__pycache__/xcit.cpython-38.pyc
+-rw-r--r--   0        0        0     3171 2023-05-18 16:15:17.906763 lacss-0.3.2/lacss/modules/auxiliary.py
+-rw-r--r--   0        0        0     2270 2023-05-18 16:15:17.916458 lacss-0.3.2/lacss/modules/common.py
+-rw-r--r--   0        0        0     6557 2023-04-28 14:03:41.873034 lacss-0.3.2/lacss/modules/convnext.py
+-rw-r--r--   0        0        0     6579 2023-05-15 14:29:30.716593 lacss-0.3.2/lacss/modules/detector.py
+-rw-r--r--   0        0        0     3813 2023-05-18 16:15:17.927778 lacss-0.3.2/lacss/modules/lacss.py
+-rw-r--r--   0        0        0     2934 2023-05-18 16:15:17.938204 lacss-0.3.2/lacss/modules/lpn.py
+-rw-r--r--   0        0        0     3771 2023-04-21 18:45:48.045107 lacss-0.3.2/lacss/modules/resnet.py
+-rw-r--r--   0        0        0     4595 2023-05-18 16:15:17.967503 lacss-0.3.2/lacss/modules/segmentor.py
+-rw-r--r--   0        0        0     1979 2023-04-28 14:03:41.880651 lacss-0.3.2/lacss/modules/unet.py
+-rw-r--r--   0        0        0      155 2023-04-21 18:45:48.079314 lacss-0.3.2/lacss/ops/__init__.py
+-rw-r--r--   0        0        0      260 2023-03-07 20:26:00.414720 lacss-0.3.2/lacss/ops/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      255 2023-04-26 16:05:14.845951 lacss-0.3.2/lacss/ops/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1804 2023-03-07 20:26:00.409875 lacss-0.3.2/lacss/ops/__pycache__/boxes.cpython-310.pyc
+-rw-r--r--   0        0        0     1987 2023-04-26 16:05:14.869998 lacss-0.3.2/lacss/ops/__pycache__/boxes.cpython-38.pyc
+-rw-r--r--   0        0        0     1121 2023-03-07 20:26:00.435101 lacss-0.3.2/lacss/ops/__pycache__/image.cpython-310.pyc
+-rw-r--r--   0        0        0     2559 2023-04-26 16:05:14.898406 lacss-0.3.2/lacss/ops/__pycache__/image.cpython-38.pyc
+-rw-r--r--   0        0        0     2379 2023-03-07 20:26:00.429728 lacss-0.3.2/lacss/ops/__pycache__/locations.cpython-310.pyc
+-rw-r--r--   0        0        0     2347 2023-04-26 16:05:14.926967 lacss-0.3.2/lacss/ops/__pycache__/locations.cpython-38.pyc
+-rw-r--r--   0        0        0     5827 2023-03-07 20:26:00.371538 lacss-0.3.2/lacss/ops/__pycache__/masks.cpython-310.pyc
+-rw-r--r--   0        0        0     5806 2023-04-26 16:05:14.944134 lacss-0.3.2/lacss/ops/__pycache__/masks.cpython-38.pyc
+-rw-r--r--   0        0        0     3845 2023-03-07 20:26:00.404805 lacss-0.3.2/lacss/ops/__pycache__/nms.cpython-310.pyc
+-rw-r--r--   0        0        0     3857 2023-04-26 16:05:14.998332 lacss-0.3.2/lacss/ops/__pycache__/nms.cpython-38.pyc
+-rw-r--r--   0        0        0     5649 2023-03-07 20:26:00.394465 lacss-0.3.2/lacss/ops/__pycache__/patches.cpython-310.pyc
+-rw-r--r--   0        0        0     7853 2023-04-26 16:05:14.981060 lacss-0.3.2/lacss/ops/__pycache__/patches.cpython-38.pyc
+-rw-r--r--   0        0        0     2175 2023-04-21 18:45:48.091110 lacss-0.3.2/lacss/ops/boxes.py
+-rw-r--r--   0        0        0     2218 2023-04-21 18:45:48.100899 lacss-0.3.2/lacss/ops/image.py
+-rw-r--r--   0        0        0     2739 2023-04-21 18:45:48.114632 lacss-0.3.2/lacss/ops/locations.py
+-rw-r--r--   0        0        0     5967 2023-04-21 18:45:48.142871 lacss-0.3.2/lacss/ops/masks.py
+-rw-r--r--   0        0        0     4704 2023-04-21 18:45:48.169083 lacss-0.3.2/lacss/ops/nms.py
+-rw-r--r--   0        0        0     9245 2023-04-21 18:45:48.177726 lacss-0.3.2/lacss/ops/patches.py
+-rw-r--r--   0        0        0       63 2023-05-17 12:27:49.580967 lacss-0.3.2/lacss/tracking/__init__.py
+-rw-r--r--   0        0        0      205 2023-05-14 18:38:38.567521 lacss-0.3.2/lacss/tracking/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2689 2023-05-15 15:16:43.449032 lacss-0.3.2/lacss/tracking/__pycache__/predict.cpython-38.pyc
+-rw-r--r--   0        0        0     6517 2023-05-15 18:37:20.371555 lacss-0.3.2/lacss/tracking/__pycache__/smc.cpython-38.pyc
+-rw-r--r--   0        0        0     4358 2023-05-15 18:37:20.409926 lacss-0.3.2/lacss/tracking/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     3340 2023-05-17 12:27:49.587345 lacss-0.3.2/lacss/tracking/predict.py
+-rw-r--r--   0        0        0     6741 2023-05-17 12:27:49.597252 lacss-0.3.2/lacss/tracking/smc.py
+-rw-r--r--   0        0        0     5646 2023-05-17 12:27:49.616793 lacss-0.3.2/lacss/tracking/utils.py
+-rw-r--r--   0        0        0       99 2023-04-21 18:45:48.241245 lacss-0.3.2/lacss/train/__init__.py
+-rw-r--r--   0        0        0      191 2023-03-07 20:26:00.181652 lacss-0.3.2/lacss/train/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      257 2023-04-26 16:05:15.023476 lacss-0.3.2/lacss/train/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6686 2023-05-17 15:11:14.083243 lacss-0.3.2/lacss/train/__pycache__/loss.cpython-38.pyc
+-rw-r--r--   0        0        0      648 2023-04-28 14:28:40.891145 lacss-0.3.2/lacss/train/__pycache__/metric.cpython-38.pyc
+-rw-r--r--   0        0        0     4261 2023-03-16 23:08:03.154040 lacss-0.3.2/lacss/train/__pycache__/pytree.cpython-38.pyc
+-rw-r--r--   0        0        0     4680 2023-03-07 20:26:00.134879 lacss-0.3.2/lacss/train/__pycache__/strategy.cpython-310.pyc
+-rw-r--r--   0        0        0     4118 2023-04-28 14:28:40.802364 lacss-0.3.2/lacss/train/__pycache__/strategy.cpython-38.pyc
+-rw-r--r--   0        0        0     3496 2023-03-07 20:26:00.159397 lacss-0.3.2/lacss/train/__pycache__/trainer.cpython-310.pyc
+-rw-r--r--   0        0        0     6896 2023-05-17 17:49:39.333286 lacss-0.3.2/lacss/train/__pycache__/trainer.cpython-38.pyc
+-rw-r--r--   0        0        0     5272 2023-03-16 23:08:03.169159 lacss-0.3.2/lacss/train/__pycache__/wrapper.cpython-38.pyc
+-rw-r--r--   0        0        0      718 2023-04-21 18:45:48.299450 lacss-0.3.2/lacss/train/data/__init__.py
+-rw-r--r--   0        0        0      868 2023-03-07 20:25:59.860409 lacss-0.3.2/lacss/train/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      851 2023-04-26 16:05:15.050386 lacss-0.3.2/lacss/train/data/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4011 2023-03-07 20:25:59.910632 lacss-0.3.2/lacss/train/data/__pycache__/array_adapter.cpython-310.pyc
+-rw-r--r--   0        0        0     4005 2023-04-26 16:05:15.067195 lacss-0.3.2/lacss/train/data/__pycache__/array_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     6036 2023-03-07 20:25:59.794089 lacss-0.3.2/lacss/train/data/__pycache__/data_adapter.cpython-310.pyc
+-rw-r--r--   0        0        0     6093 2023-04-26 16:05:15.080415 lacss-0.3.2/lacss/train/data/__pycache__/data_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     5560 2023-03-07 20:25:59.837897 lacss-0.3.2/lacss/train/data/__pycache__/data_handler.cpython-310.pyc
+-rw-r--r--   0        0        0     5561 2023-04-26 16:05:15.114203 lacss-0.3.2/lacss/train/data/__pycache__/data_handler.cpython-38.pyc
+-rw-r--r--   0        0        0    11601 2023-03-07 20:25:59.891017 lacss-0.3.2/lacss/train/data/__pycache__/dataset.cpython-310.pyc
+-rw-r--r--   0        0        0    11577 2023-04-26 16:05:15.128310 lacss-0.3.2/lacss/train/data/__pycache__/dataset.cpython-38.pyc
+-rw-r--r--   0        0        0     3314 2023-03-07 20:25:59.948618 lacss-0.3.2/lacss/train/data/__pycache__/generator_adapter.cpython-310.pyc
+-rw-r--r--   0        0        0     3319 2023-04-26 16:05:15.141255 lacss-0.3.2/lacss/train/data/__pycache__/generator_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     2490 2023-03-07 20:25:59.735195 lacss-0.3.2/lacss/train/data/__pycache__/list_adapter.cpython-310.pyc
+-rw-r--r--   0        0        0     2515 2023-04-26 16:05:15.157133 lacss-0.3.2/lacss/train/data/__pycache__/list_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     3581 2023-03-07 20:25:59.741952 lacss-0.3.2/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-310.pyc
+-rw-r--r--   0        0        0     3562 2023-04-26 16:05:15.171168 lacss-0.3.2/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     3180 2023-03-07 20:25:59.763043 lacss-0.3.2/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-310.pyc
+-rw-r--r--   0        0        0     3167 2023-04-26 16:05:15.186154 lacss-0.3.2/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     6787 2023-03-07 20:25:59.810992 lacss-0.3.2/lacss/train/data/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     6796 2023-04-26 16:05:15.099537 lacss-0.3.2/lacss/train/data/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     4076 2023-04-21 18:45:48.325549 lacss-0.3.2/lacss/train/data/array_adapter.py
+-rw-r--r--   0        0        0     5529 2023-04-21 18:45:48.371676 lacss-0.3.2/lacss/train/data/data_adapter.py
+-rw-r--r--   0        0        0     6287 2023-04-21 18:45:48.396891 lacss-0.3.2/lacss/train/data/data_handler.py
+-rw-r--r--   0        0        0    10656 2023-04-21 18:45:48.433354 lacss-0.3.2/lacss/train/data/dataset.py
+-rw-r--r--   0        0        0     2599 2023-04-21 18:45:48.456058 lacss-0.3.2/lacss/train/data/generator_adapter.py
+-rw-r--r--   0        0        0     2105 2023-04-21 18:45:48.467534 lacss-0.3.2/lacss/train/data/list_adapter.py
+-rw-r--r--   0        0        0     3440 2023-04-21 18:45:48.479496 lacss-0.3.2/lacss/train/data/tf_dataset_adapter.py
+-rw-r--r--   0        0        0     2566 2023-04-21 18:45:48.526515 lacss-0.3.2/lacss/train/data/torch_dataloader_adapter.py
+-rw-r--r--   0        0        0     6394 2023-04-21 18:45:48.565291 lacss-0.3.2/lacss/train/data/utils.py
+-rw-r--r--   0        0        0     6826 2023-05-18 16:15:17.976482 lacss-0.3.2/lacss/train/loss.py
+-rw-r--r--   0        0        0      222 2023-04-28 13:52:59.277007 lacss-0.3.2/lacss/train/metric.py
+-rw-r--r--   0        0        0     4018 2023-04-28 14:03:41.907286 lacss-0.3.2/lacss/train/strategy.py
+-rw-r--r--   0        0        0     7437 2023-05-18 16:15:17.983603 lacss-0.3.2/lacss/train/trainer.py
+-rw-r--r--   0        0        0     4755 2023-05-17 12:27:49.626673 lacss-0.3.2/lacss/utils.py
+-rw-r--r--   0        0        0      810 2023-05-18 16:30:30.838014 lacss-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2871 1970-01-01 00:00:00.000000 lacss-0.3.2/PKG-INFO
```

### Comparing `lacss-0.3.1/LICENSE` & `lacss-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/README.md` & `lacss-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 Ref: https://arxiv.org/abs/2304.10671
 
 ### Why LACSS?
 LACSS is designed to utilize point labels for model training. You have three options:
 
 | Method | Data(left) / Label(right)|
 | --- | --- |
-| Point | <img src="https://github.com/jiyuuchc/lacss_jax/blob/main/.github/images/label_scheme_1.png" width="300"> |
-| Point + Mask | <img src="https://github.com/jiyuuchc/lacss_jax/blob/main/.github/images/label_scheme_2.png" width="300"> |
-| Segmentation | <img src="https://github.com/jiyuuchc/lacss_jax/blob/main/.github/images/label_scheme_3.png" width="300"> |
+| Point | <img src="https://github.com/jiyuuchc/lacss_jax/raw/main/.github/images/label_scheme_1.png" width="300"> |
+| Point + Mask | <img src="https://github.com/jiyuuchc/lacss_jax/raw/main/.github/images/label_scheme_2.png" width="300"> |
+| Segmentation | <img src="https://github.com/jiyuuchc/lacss_jax/raw/main/.github/images/label_scheme_3.png" width="300"> |
 
 You can of course also combined these labels in any way you want.
 
 ### What is included?
 
 - A library for training LACSS model and performing inference
 - A few pretrained models as transfer learning starting point
 - SMC-based cell tracking utility for people interested in cell tracking
 
 ### How to generate point label?
 
 If your data include nuclei counter-stain, the easist way to generate point label for your image is to use a [blob detection](https://scikit-image.org/docs/stable/auto_examples/features_detection/plot_blob.html) algorithm on the nuclei images:
 
-![](https://github.com/jiyuuchc/lacss_jax/blob/main/.github/images/blob_detection.png)
+![](https://github.com/jiyuuchc/lacss_jax/raw/main/.github/images/blob_detection.png)
 
 ### Give it a try:
 * Model training
   * [Supervised Training ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jiyuuchc/lacss_jax/blob/main/notebooks/train_with_segmentation_label.ipynb)
   * [With point label + mask ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jiyuuchc/lacss_jax/blob/main/notebooks/train_with_point_and_mask.ipynb)
   * [With point label only ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jiyuuchc/lacss_jax/blob/main/notebooks/train_with_point_label.ipynb)
```

### Comparing `lacss-0.3.1/lacss/app/da.py` & `lacss-0.3.2/lacss/app/da.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/data/__pycache__/generator.cpython-310.pyc` & `lacss-0.3.2/lacss/data/__pycache__/generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/data/__pycache__/generator.cpython-38.pyc` & `lacss-0.3.2/lacss/data/__pycache__/generator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/data/__pycache__/parser.cpython-310.pyc` & `lacss-0.3.2/lacss/data/__pycache__/parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/data/__pycache__/parser.cpython-38.pyc` & `lacss-0.3.2/lacss/data/__pycache__/parser.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/data/generator.py` & `lacss-0.3.2/lacss/data/generator.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/data/parser.py` & `lacss-0.3.2/lacss/data/parser.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/deploy.py` & `lacss-0.3.2/lacss/deploy.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/losses/__pycache__/auxiliary.cpython-38.pyc` & `lacss-0.3.2/lacss/losses/__pycache__/auxiliary.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/losses/__pycache__/auxnet.cpython-310.pyc` & `lacss-0.3.2/lacss/losses/__pycache__/auxnet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/losses/__pycache__/auxnet.cpython-38.pyc` & `lacss-0.3.2/lacss/losses/__pycache__/auxnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/losses/__pycache__/detection.cpython-310.pyc` & `lacss-0.3.2/lacss/losses/__pycache__/detection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/losses/__pycache__/detection.cpython-38.pyc` & `lacss-0.3.2/lacss/losses/__pycache__/detection.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/losses/__pycache__/instance.cpython-310.pyc` & `lacss-0.3.2/lacss/losses/__pycache__/instance.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/losses/__pycache__/instance.cpython-38.pyc` & `lacss-0.3.2/lacss/losses/__pycache__/instance.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/losses/__pycache__/lacss.cpython-38.pyc` & `lacss-0.3.2/lacss/losses/__pycache__/lacss.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/losses/__pycache__/loss.cpython-38.pyc` & `lacss-0.3.2/lacss/losses/__pycache__/loss.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/losses/auxiliary.py` & `lacss-0.3.2/lacss/losses/auxiliary.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/losses/detection.py` & `lacss-0.3.2/lacss/losses/detection.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/losses/instance.py` & `lacss-0.3.2/lacss/losses/instance.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/metrics/__pycache__/metric.cpython-38.pyc` & `lacss-0.3.2/lacss/metrics/__pycache__/metric.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/metrics/__pycache__/ranked.cpython-310.pyc` & `lacss-0.3.2/lacss/metrics/__pycache__/ranked.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/metrics/__pycache__/ranked.cpython-38.pyc` & `lacss-0.3.2/lacss/metrics/__pycache__/ranked.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/metrics/ranked.py` & `lacss-0.3.2/lacss/metrics/ranked.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/auxiliary.cpython-38.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/auxiliary.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/auxnet.cpython-310.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/auxnet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/auxnet.cpython-38.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/auxnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/common.cpython-38.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/convnext.cpython-310.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/convnext.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/convnext.cpython-38.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/convnext.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/detector.cpython-310.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/detector.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/detector.cpython-38.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/detector.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/lacss.cpython-310.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/lacss.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/lacss.cpython-38.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/lacss.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/lpn.cpython-310.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/lpn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/lpn.cpython-38.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/lpn.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/resnet.cpython-310.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/resnet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/resnet.cpython-38.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/resnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/se_net.cpython-310.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/se_net.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/segmentor.cpython-310.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/segmentor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/segmentor.cpython-38.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/segmentor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/types.cpython-310.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/types.cpython-38.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/types.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/unet.cpython-310.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/unet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/unet.cpython-38.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/unet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/xcit.cpython-310.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/xcit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/__pycache__/xcit.cpython-38.pyc` & `lacss-0.3.2/lacss/modules/__pycache__/xcit.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/auxiliary.py` & `lacss-0.3.2/lacss/modules/auxiliary.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/common.py` & `lacss-0.3.2/lacss/modules/common.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/convnext.py` & `lacss-0.3.2/lacss/modules/convnext.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/detector.py` & `lacss-0.3.2/lacss/modules/detector.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/lacss.py` & `lacss-0.3.2/lacss/modules/lacss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/lpn.py` & `lacss-0.3.2/lacss/modules/lpn.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/resnet.py` & `lacss-0.3.2/lacss/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/segmentor.py` & `lacss-0.3.2/lacss/modules/segmentor.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/modules/unet.py` & `lacss-0.3.2/lacss/modules/unet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/__pycache__/boxes.cpython-310.pyc` & `lacss-0.3.2/lacss/ops/__pycache__/boxes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/__pycache__/boxes.cpython-38.pyc` & `lacss-0.3.2/lacss/ops/__pycache__/boxes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/__pycache__/image.cpython-310.pyc` & `lacss-0.3.2/lacss/ops/__pycache__/image.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/__pycache__/image.cpython-38.pyc` & `lacss-0.3.2/lacss/ops/__pycache__/image.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/__pycache__/locations.cpython-310.pyc` & `lacss-0.3.2/lacss/ops/__pycache__/locations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/__pycache__/locations.cpython-38.pyc` & `lacss-0.3.2/lacss/ops/__pycache__/locations.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/__pycache__/masks.cpython-310.pyc` & `lacss-0.3.2/lacss/ops/__pycache__/masks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/__pycache__/masks.cpython-38.pyc` & `lacss-0.3.2/lacss/ops/__pycache__/masks.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/__pycache__/nms.cpython-310.pyc` & `lacss-0.3.2/lacss/ops/__pycache__/nms.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/__pycache__/nms.cpython-38.pyc` & `lacss-0.3.2/lacss/ops/__pycache__/nms.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/__pycache__/patches.cpython-310.pyc` & `lacss-0.3.2/lacss/ops/__pycache__/patches.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/__pycache__/patches.cpython-38.pyc` & `lacss-0.3.2/lacss/ops/__pycache__/patches.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/boxes.py` & `lacss-0.3.2/lacss/ops/boxes.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/image.py` & `lacss-0.3.2/lacss/ops/image.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/locations.py` & `lacss-0.3.2/lacss/ops/locations.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/masks.py` & `lacss-0.3.2/lacss/ops/masks.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/nms.py` & `lacss-0.3.2/lacss/ops/nms.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/ops/patches.py` & `lacss-0.3.2/lacss/ops/patches.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/tracking/__pycache__/predict.cpython-38.pyc` & `lacss-0.3.2/lacss/tracking/__pycache__/predict.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/tracking/__pycache__/smc.cpython-38.pyc` & `lacss-0.3.2/lacss/tracking/__pycache__/smc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/tracking/__pycache__/utils.cpython-38.pyc` & `lacss-0.3.2/lacss/tracking/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/tracking/predict.py` & `lacss-0.3.2/lacss/tracking/predict.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/tracking/smc.py` & `lacss-0.3.2/lacss/tracking/smc.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/tracking/utils.py` & `lacss-0.3.2/lacss/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/__pycache__/loss.cpython-38.pyc` & `lacss-0.3.2/lacss/train/__pycache__/loss.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/__pycache__/metric.cpython-38.pyc` & `lacss-0.3.2/lacss/train/__pycache__/metric.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/__pycache__/pytree.cpython-38.pyc` & `lacss-0.3.2/lacss/train/__pycache__/pytree.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/__pycache__/strategy.cpython-310.pyc` & `lacss-0.3.2/lacss/train/__pycache__/strategy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/__pycache__/strategy.cpython-38.pyc` & `lacss-0.3.2/lacss/train/__pycache__/strategy.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/__pycache__/trainer.cpython-310.pyc` & `lacss-0.3.2/lacss/train/__pycache__/trainer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/__pycache__/trainer.cpython-38.pyc` & `lacss-0.3.2/lacss/train/__pycache__/trainer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/__pycache__/wrapper.cpython-38.pyc` & `lacss-0.3.2/lacss/train/__pycache__/wrapper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__init__.py` & `lacss-0.3.2/lacss/train/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/__init__.cpython-310.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/__init__.cpython-38.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/array_adapter.cpython-310.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/array_adapter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/array_adapter.cpython-38.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/array_adapter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/data_adapter.cpython-310.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/data_adapter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/data_adapter.cpython-38.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/data_adapter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/data_handler.cpython-310.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/data_handler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/data_handler.cpython-38.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/data_handler.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/dataset.cpython-310.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/dataset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/dataset.cpython-38.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/dataset.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/generator_adapter.cpython-310.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/generator_adapter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/generator_adapter.cpython-38.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/generator_adapter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/list_adapter.cpython-310.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/list_adapter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/list_adapter.cpython-38.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/list_adapter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-310.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-38.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-310.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-38.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/utils.cpython-310.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/__pycache__/utils.cpython-38.pyc` & `lacss-0.3.2/lacss/train/data/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/array_adapter.py` & `lacss-0.3.2/lacss/train/data/array_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/data_adapter.py` & `lacss-0.3.2/lacss/train/data/data_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/data_handler.py` & `lacss-0.3.2/lacss/train/data/data_handler.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/dataset.py` & `lacss-0.3.2/lacss/train/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/generator_adapter.py` & `lacss-0.3.2/lacss/train/data/generator_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/list_adapter.py` & `lacss-0.3.2/lacss/train/data/list_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/tf_dataset_adapter.py` & `lacss-0.3.2/lacss/train/data/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/torch_dataloader_adapter.py` & `lacss-0.3.2/lacss/train/data/torch_dataloader_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/data/utils.py` & `lacss-0.3.2/lacss/train/data/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/loss.py` & `lacss-0.3.2/lacss/train/loss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/strategy.py` & `lacss-0.3.2/lacss/train/strategy.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/train/trainer.py` & `lacss-0.3.2/lacss/train/trainer.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/lacss/utils.py` & `lacss-0.3.2/lacss/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.3.1/pyproject.toml` & `lacss-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacss"
-version = "0.3.1"
+version = "0.3.2"
 description = "Cell segmentation and tracking"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
```

### Comparing `lacss-0.3.1/PKG-INFO` & `lacss-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacss
-Version: 0.3.1
+Version: 0.3.2
 Summary: Cell segmentation and tracking
 License: MIT
 Author: Ji Yu
 Author-email: jyu@uchc.edu
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -26,31 +26,31 @@
 Ref: https://arxiv.org/abs/2304.10671
 
 ### Why LACSS?
 LACSS is designed to utilize point labels for model training. You have three options:
 
 | Method | Data(left) / Label(right)|
 | --- | --- |
-| Point | <img src="https://github.com/jiyuuchc/lacss_jax/blob/main/.github/images/label_scheme_1.png" width="300"> |
-| Point + Mask | <img src="https://github.com/jiyuuchc/lacss_jax/blob/main/.github/images/label_scheme_2.png" width="300"> |
-| Segmentation | <img src="https://github.com/jiyuuchc/lacss_jax/blob/main/.github/images/label_scheme_3.png" width="300"> |
+| Point | <img src="https://github.com/jiyuuchc/lacss_jax/raw/main/.github/images/label_scheme_1.png" width="300"> |
+| Point + Mask | <img src="https://github.com/jiyuuchc/lacss_jax/raw/main/.github/images/label_scheme_2.png" width="300"> |
+| Segmentation | <img src="https://github.com/jiyuuchc/lacss_jax/raw/main/.github/images/label_scheme_3.png" width="300"> |
 
 You can of course also combined these labels in any way you want.
 
 ### What is included?
 
 - A library for training LACSS model and performing inference
 - A few pretrained models as transfer learning starting point
 - SMC-based cell tracking utility for people interested in cell tracking
 
 ### How to generate point label?
 
 If your data include nuclei counter-stain, the easist way to generate point label for your image is to use a [blob detection](https://scikit-image.org/docs/stable/auto_examples/features_detection/plot_blob.html) algorithm on the nuclei images:
 
-![](https://github.com/jiyuuchc/lacss_jax/blob/main/.github/images/blob_detection.png)
+![](https://github.com/jiyuuchc/lacss_jax/raw/main/.github/images/blob_detection.png)
 
 ### Give it a try:
 * Model training
   * [Supervised Training ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jiyuuchc/lacss_jax/blob/main/notebooks/train_with_segmentation_label.ipynb)
   * [With point label + mask ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jiyuuchc/lacss_jax/blob/main/notebooks/train_with_point_and_mask.ipynb)
   * [With point label only ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jiyuuchc/lacss_jax/blob/main/notebooks/train_with_point_label.ipynb)
```

