# Comparing `tmp/onvif-gui-1.1.6.tar.gz` & `tmp/onvif-gui-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-gui-1.1.6.tar", last modified: Wed May 17 23:36:47 2023, max compression
+gzip compressed data, was "onvif-gui-1.1.8.tar", last modified: Thu May 18 20:47:01 2023, max compression
```

## Comparing `onvif-gui-1.1.6.tar` & `onvif-gui-1.1.8.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.641284 onvif-gui-1.1.6/
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11357 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/LICENSE
--rw-r--r--   0 stephen   (1000) stephen   (1000)      217 2023-05-09 00:18:57.000000 onvif-gui-1.1.6/MANIFEST.in
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-17 23:36:47.637284 onvif-gui-1.1.6/PKG-INFO
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8170 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/README.md
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.605284 onvif-gui-1.1.6/detectron2/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       67 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.605284 onvif-gui-1.1.6/detectron2/checkpoint/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/checkpoint/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    17770 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/checkpoint/c2_model_loading.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5685 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/checkpoint/catalog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5258 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/checkpoint/detection_checkpoint.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.609284 onvif-gui-1.1.6/detectron2/config/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      599 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/config/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7890 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/config/compat.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9211 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/config/config.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    29512 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/config/defaults.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3015 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/config/instantiate.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15378 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/config/lazy.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.609284 onvif-gui-1.1.6/detectron2/configs/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1318 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/configs/Base-RCNN-FPN.yaml
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.609284 onvif-gui-1.1.6/detectron2/configs/COCO-InstanceSegmentation/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 23:51:42.000000 onvif-gui-1.1.6/detectron2/configs/COCO-InstanceSegmentation/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      192 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.609284 onvif-gui-1.1.6/detectron2/configs/COCO-Keypoints/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      527 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 23:51:42.000000 onvif-gui-1.1.6/detectron2/configs/COCO-Keypoints/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      182 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/configs/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.609284 onvif-gui-1.1.6/detectron2/data/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      644 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7378 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/benchmark.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    21231 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7224 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/catalog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9162 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/common.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8169 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/dataset_mapper.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.613284 onvif-gui-1.1.6/detectron2/data/datasets/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      523 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/datasets/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10174 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/datasets/builtin.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    21841 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/datasets/builtin_meta.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13167 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/datasets/cityscapes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7821 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/datasets/cityscapes_panoptic.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23465 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/datasets/coco.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8977 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/datasets/coco_panoptic.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9623 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/datasets/lvis.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)   223757 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/datasets/lvis_v0_5_categories.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)   219177 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/datasets/lvis_v1_categories.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    39414 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/datasets/lvis_v1_category_image_count.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3128 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/datasets/pascal_voc.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      169 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/datasets/register_coco.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    22841 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/detection_utils.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.613284 onvif-gui-1.1.6/detectron2/data/samplers/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      412 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/samplers/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11789 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/samplers/distributed_sampler.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1944 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/samplers/grouped_batch_sampler.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.613284 onvif-gui-1.1.6/detectron2/data/transforms/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      466 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/transforms/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14112 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/transforms/augmentation.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23069 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/transforms/augmentation_impl.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12629 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/data/transforms/transform.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.613284 onvif-gui-1.1.6/detectron2/layers/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      874 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/layers/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5764 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/layers/aspp.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12131 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/layers/batch_norm.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3024 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/layers/blocks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    16978 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/layers/deform_conv.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4202 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/layers/losses.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10879 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/layers/mask_ops.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6490 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/layers/nms.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3098 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/layers/roi_align.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3302 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/layers/roi_align_rotated.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      652 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/layers/rotated_boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      537 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/layers/shape_spec.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5123 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/layers/wrappers.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.613284 onvif-gui-1.1.6/detectron2/modeling/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1568 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15439 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/anchor_generator.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.617284 onvif-gui-1.1.6/detectron2/modeling/backbone/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      598 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/backbone/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2512 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/backbone/backbone.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1015 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/backbone/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10360 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/backbone/fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15988 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/backbone/mvit.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    16656 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/backbone/regnet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23658 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/backbone/resnet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25095 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/backbone/swin.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6360 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/backbone/utils.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    19338 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/backbone/vit.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15123 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/box_regression.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6264 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/matcher.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.617284 onvif-gui-1.1.6/detectron2/modeling/meta_arch/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      508 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/meta_arch/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      814 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/meta_arch/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11651 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/meta_arch/dense_detector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13213 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/meta_arch/fcos.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10407 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/meta_arch/panoptic_fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13896 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/meta_arch/rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18265 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/meta_arch/retinanet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9906 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/meta_arch/semantic_seg.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10832 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/mmdet_wrapper.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11316 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/poolers.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4045 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/postprocessing.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.617284 onvif-gui-1.1.6/detectron2/modeling/proposal_generator/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      231 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/proposal_generator/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      836 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/proposal_generator/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8128 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/proposal_generator/proposal_utils.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    23814 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/proposal_generator/rpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8807 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/proposal_generator/rrpn.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.617284 onvif-gui-1.1.6/detectron2/modeling/roi_heads/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      768 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/roi_heads/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4077 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/roi_heads/box_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12990 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/roi_heads/cascade_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25390 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/roi_heads/fast_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11156 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/roi_heads/keypoint_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12169 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/roi_heads/mask_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    37701 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/roi_heads/roi_heads.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11175 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2334 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/sampling.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12416 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/modeling/test_time_augmentation.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1780 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/predictor.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.617284 onvif-gui-1.1.6/detectron2/structures/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      645 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/structures/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14429 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/structures/boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5520 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/structures/image_list.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6613 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/structures/instances.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9030 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/structures/keypoints.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    19802 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/structures/masks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18853 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/structures/rotated_boxes.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2707 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/tracker.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.621284 onvif-gui-1.1.6/detectron2/utils/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       51 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6017 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/analysis.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8391 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/collect_env.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4096 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/colormap.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5608 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/comm.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1852 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/develop.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5644 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/env.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    17022 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/events.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1189 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/file_io.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7807 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/logger.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2583 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/memory.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1874 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/registry.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1064 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/serialize.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    18113 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/testing.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11319 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/video_visualizer.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    51159 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/detectron2/utils/visualizer.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.621284 onvif-gui-1.1.6/gui/
--rw-r--r--   0 stephen   (1000) stephen   (1000)       28 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.621284 onvif-gui-1.1.6/gui/components/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      245 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/components/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1777 2023-05-15 22:24:13.000000 onvif-gui-1.1.6/gui/components/comboselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2397 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/components/directoryselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2118 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/components/fileselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5393 2023-05-15 22:24:13.000000 onvif-gui-1.1.6/gui/components/labelselector.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4077 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/components/progress.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1918 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/components/thresholdslider.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1996 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/glwidget.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14379 2023-05-17 23:36:29.000000 onvif-gui-1.1.6/gui/main.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.621284 onvif-gui-1.1.6/gui/onvif/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      191 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/onvif/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5743 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/onvif/admintab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3959 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/onvif/imagetab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2425 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/onvif/logindialog.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5247 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/onvif/networktab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5118 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/onvif/ptztab.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4527 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/onvif/videotab.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.625284 onvif-gui-1.1.6/gui/panels/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      180 2023-05-03 01:49:37.000000 onvif-gui-1.1.6/gui/panels/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3624 2023-05-03 02:34:01.000000 onvif-gui-1.1.6/gui/panels/audiopanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    13463 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/panels/camerapanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    14483 2023-05-03 15:52:33.000000 onvif-gui-1.1.6/gui/panels/filepanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12913 2023-05-02 23:52:13.000000 onvif-gui-1.1.6/gui/panels/settingspanel.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3627 2023-05-03 02:39:24.000000 onvif-gui-1.1.6/gui/panels/videopanel.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.633284 onvif-gui-1.1.6/gui/resources/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1936 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/LICENSE
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      252 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/apply.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      245 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/apply_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      244 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/apply_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      911 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/audio.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      536 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/audio_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      920 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/audio_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      203 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/branch_closed.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      219 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/branch_closed_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      211 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/branch_closed_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      199 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/branch_open.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      168 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/branch_open_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/branch_open_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      267 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/checked.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      235 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/checked_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      246 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/checked_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12716 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/darkstyle.qss
--rw-r--r--   0 stephen   (1000) stephen   (1000)      910 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/discover.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      849 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/discover_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      937 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/discover_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/fast-forward.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      253 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/fast-forward_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      433 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/fast-forward_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      641 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/mute.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      346 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/mute_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      618 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/mute_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/next.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      225 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/next_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/next_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)    46084 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/onvif-gui.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/pause.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      144 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/pause_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      149 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/pause_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      321 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/play.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      209 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/play_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      316 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/play_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      349 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/previous.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      232 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/previous_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/previous_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/radio-off.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/radio-off_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/radio-off_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      350 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/radio-on.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      263 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/radio-on_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      343 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/radio-on_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      395 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/record.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      394 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/record_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/record_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      408 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/recording.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      435 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/recording_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      532 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/recording_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      454 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/rewind.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/rewind_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      457 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/rewind_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      187 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/small_arrow_left.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      183 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/small_arrow_left_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      189 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/small_arrow_left_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      162 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/small_arrow_up.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      160 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/small_arrow_up_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      161 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/small_arrow_up_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      158 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/stop.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      140 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/stop_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      151 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/stop_lo.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/unchecked.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      142 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/unchecked_hi.png
--rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/gui/resources/unchecked_lo.png
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.633284 onvif-gui-1.1.6/modules/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-03 23:45:47.000000 onvif-gui-1.1.6/modules/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.633284 onvif-gui-1.1.6/modules/audio/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-03 02:36:19.000000 onvif-gui-1.1.6/modules/audio/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3404 2023-05-03 19:20:32.000000 onvif-gui-1.1.6/modules/audio/sample.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.633284 onvif-gui-1.1.6/modules/video/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-04-30 20:27:50.000000 onvif-gui-1.1.6/modules/video/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6913 2023-05-15 22:24:13.000000 onvif-gui-1.1.6/modules/video/keypoint.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4768 2023-05-15 22:24:13.000000 onvif-gui-1.1.6/modules/video/retinanet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3095 2023-05-15 22:24:13.000000 onvif-gui-1.1.6/modules/video/sample.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7423 2023-05-15 22:24:13.000000 onvif-gui-1.1.6/modules/video/segment.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10627 2023-05-17 23:34:06.000000 onvif-gui-1.1.6/modules/video/yolov7.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8833 2023-05-17 23:33:46.000000 onvif-gui-1.1.6/modules/video/yolov8.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    11955 2023-05-17 23:32:41.000000 onvif-gui-1.1.6/modules/video/yolox.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.633284 onvif-gui-1.1.6/onvif_gui.egg-info/
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-17 23:36:47.000000 onvif-gui-1.1.6/onvif_gui.egg-info/PKG-INFO
--rw-r--r--   0 stephen   (1000) stephen   (1000)     8392 2023-05-17 23:36:47.000000 onvif-gui-1.1.6/onvif_gui.egg-info/SOURCES.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)        1 2023-05-17 23:36:47.000000 onvif-gui-1.1.6/onvif_gui.egg-info/dependency_links.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       39 2023-05-17 23:36:47.000000 onvif-gui-1.1.6/onvif_gui.egg-info/entry_points.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       47 2023-05-17 23:36:47.000000 onvif-gui-1.1.6/onvif_gui.egg-info/requires.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)       44 2023-05-17 23:36:47.000000 onvif-gui-1.1.6/onvif_gui.egg-info/top_level.txt
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1659 2023-05-17 23:36:12.000000 onvif-gui-1.1.6/pyproject.toml
--rw-r--r--   0 stephen   (1000) stephen   (1000)       38 2023-05-17 23:36:47.641284 onvif-gui-1.1.6/setup.cfg
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1504 2023-05-17 23:36:04.000000 onvif-gui-1.1.6/setup.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.637284 onvif-gui-1.1.6/tracker/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/tracker/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)      951 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/tracker/basetrack.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    12295 2023-05-16 17:49:10.000000 onvif-gui-1.1.6/tracker/byte_tracker.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9547 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/tracker/kalman_filter.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6127 2023-05-16 16:45:09.000000 onvif-gui-1.1.6/tracker/matching.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.637284 onvif-gui-1.1.6/yolov7/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:08:03.000000 onvif-gui-1.1.6/yolov7/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.637284 onvif-gui-1.1.6/yolov7/models/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        6 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/models/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    84416 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/models/common.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    10905 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/models/experimental.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    40052 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/models/yolo.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.637284 onvif-gui-1.1.6/yolov7/utils/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        6 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/utils/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2248 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/utils/activations.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     5616 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/utils/add_nms.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     7161 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/utils/autoanchor.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    56239 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/utils/datasets.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    36897 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/utils/general.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4873 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/utils/google_utils.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    75044 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/utils/loss.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     9310 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/utils/metrics.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    20935 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/utils/plots.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    15467 2023-05-15 22:33:05.000000 onvif-gui-1.1.6/yolov7/utils/torch_utils.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.637284 onvif-gui-1.1.6/yolox/
--rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/yolox/__init__.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.637284 onvif-gui-1.1.6/yolox/models/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      936 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/yolox/models/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4894 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/yolox/models/build.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6647 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/yolox/models/darknet.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     2305 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/yolox/models/losses.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     6720 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/yolox/models/network_blocks.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     3104 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/yolox/models/yolo_fpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)    25526 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/yolox/models/yolo_head.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     4158 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/yolox/models/yolo_pafpn.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1992 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/yolox/models/yolox.py
-drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-17 23:36:47.637284 onvif-gui-1.1.6/yolox/utils/
--rw-r--r--   0 stephen   (1000) stephen   (1000)      126 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/yolox/utils/__init__.py
--rw-r--r--   0 stephen   (1000) stephen   (1000)     1580 2023-05-08 23:51:04.000000 onvif-gui-1.1.6/yolox/utils/utils.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.710648 onvif-gui-1.1.8/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11357 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      217 2023-05-09 22:10:02.000000 onvif-gui-1.1.8/MANIFEST.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-18 20:47:01.710648 onvif-gui-1.1.8/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8170 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/README.md
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.690648 onvif-gui-1.1.8/detectron2/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       67 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.690648 onvif-gui-1.1.8/detectron2/checkpoint/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      347 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/checkpoint/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17770 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/checkpoint/c2_model_loading.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5685 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/checkpoint/catalog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5258 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/checkpoint/detection_checkpoint.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.690648 onvif-gui-1.1.8/detectron2/config/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      599 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/config/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7890 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/config/compat.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9211 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/config/config.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    29512 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/config/defaults.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3015 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/config/instantiate.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15378 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/config/lazy.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.690648 onvif-gui-1.1.8/detectron2/configs/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1318 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/configs/Base-RCNN-FPN.yaml
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.690648 onvif-gui-1.1.8/detectron2/configs/COCO-InstanceSegmentation/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:40:11.000000 onvif-gui-1.1.8/detectron2/configs/COCO-InstanceSegmentation/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      192 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.690648 onvif-gui-1.1.8/detectron2/configs/COCO-Keypoints/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      527 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:40:01.000000 onvif-gui-1.1.8/detectron2/configs/COCO-Keypoints/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      182 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/configs/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.690648 onvif-gui-1.1.8/detectron2/data/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      644 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7378 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/benchmark.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21231 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7224 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/catalog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9162 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/common.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8169 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/dataset_mapper.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.690648 onvif-gui-1.1.8/detectron2/data/datasets/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      523 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/datasets/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10174 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/datasets/builtin.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21841 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/datasets/builtin_meta.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13167 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/datasets/cityscapes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7821 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/datasets/cityscapes_panoptic.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23465 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/datasets/coco.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8977 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/datasets/coco_panoptic.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9623 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/datasets/lvis.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   223757 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/datasets/lvis_v0_5_categories.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   219177 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/datasets/lvis_v1_categories.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    39414 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3128 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/datasets/pascal_voc.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      169 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/datasets/register_coco.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    22841 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/detection_utils.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.690648 onvif-gui-1.1.8/detectron2/data/samplers/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      412 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/samplers/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11789 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/samplers/distributed_sampler.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1944 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/samplers/grouped_batch_sampler.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.694648 onvif-gui-1.1.8/detectron2/data/transforms/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      466 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/transforms/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14112 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/transforms/augmentation.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23069 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/transforms/augmentation_impl.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12629 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/data/transforms/transform.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.694648 onvif-gui-1.1.8/detectron2/layers/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      874 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/layers/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5764 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/layers/aspp.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12131 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/layers/batch_norm.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3024 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/layers/blocks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16978 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/layers/deform_conv.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4202 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/layers/losses.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10879 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/layers/mask_ops.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6490 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/layers/nms.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3098 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/layers/roi_align.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3302 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/layers/roi_align_rotated.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      652 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/layers/rotated_boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      537 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/layers/shape_spec.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5123 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/layers/wrappers.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.694648 onvif-gui-1.1.8/detectron2/modeling/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1568 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15439 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/anchor_generator.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.694648 onvif-gui-1.1.8/detectron2/modeling/backbone/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      598 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/backbone/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2512 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/backbone/backbone.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1015 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/backbone/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10360 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/backbone/fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15988 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/backbone/mvit.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16656 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/backbone/regnet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23658 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/backbone/resnet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25095 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/backbone/swin.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6360 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/backbone/utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19338 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/backbone/vit.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15123 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/box_regression.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6264 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/matcher.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.694648 onvif-gui-1.1.8/detectron2/modeling/meta_arch/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      508 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/meta_arch/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      814 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/meta_arch/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11651 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/meta_arch/dense_detector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13213 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/meta_arch/fcos.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10407 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13896 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/meta_arch/rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18265 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/meta_arch/retinanet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9906 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/meta_arch/semantic_seg.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10832 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/mmdet_wrapper.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11316 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/poolers.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4045 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/postprocessing.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.694648 onvif-gui-1.1.8/detectron2/modeling/proposal_generator/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      231 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/proposal_generator/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      836 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/proposal_generator/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8128 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/proposal_generator/proposal_utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23814 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/proposal_generator/rpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8807 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/proposal_generator/rrpn.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.698648 onvif-gui-1.1.8/detectron2/modeling/roi_heads/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      768 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/roi_heads/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4077 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/roi_heads/box_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12990 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25390 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/roi_heads/fast_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11156 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/roi_heads/keypoint_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12169 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/roi_heads/mask_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    37701 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/roi_heads/roi_heads.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11175 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2334 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/sampling.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12416 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/modeling/test_time_augmentation.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1780 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/predictor.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.698648 onvif-gui-1.1.8/detectron2/structures/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      645 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/structures/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14429 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/structures/boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5520 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/structures/image_list.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6613 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/structures/instances.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9030 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/structures/keypoints.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19802 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/structures/masks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18853 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/structures/rotated_boxes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2707 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/tracker.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.698648 onvif-gui-1.1.8/detectron2/utils/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       51 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6017 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/analysis.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8391 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/collect_env.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4096 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/colormap.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5608 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/comm.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1852 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/develop.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5644 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/env.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17022 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/events.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1189 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/file_io.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7807 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/logger.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2583 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/memory.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1874 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/registry.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1064 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/serialize.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18113 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/testing.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11319 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/video_visualizer.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    51159 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/detectron2/utils/visualizer.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.698648 onvif-gui-1.1.8/gui/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       28 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.698648 onvif-gui-1.1.8/gui/components/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      245 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/components/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1777 2023-05-13 16:10:05.000000 onvif-gui-1.1.8/gui/components/comboselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2397 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/components/directoryselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2118 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/components/fileselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5393 2023-05-13 16:10:05.000000 onvif-gui-1.1.8/gui/components/labelselector.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4077 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/components/progress.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1918 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/components/thresholdslider.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1996 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/glwidget.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14216 2023-05-18 20:44:33.000000 onvif-gui-1.1.8/gui/main.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.698648 onvif-gui-1.1.8/gui/onvif/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      191 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/onvif/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5743 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/onvif/admintab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3959 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/onvif/imagetab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2425 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/onvif/logindialog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5247 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/onvif/networktab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5118 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/onvif/ptztab.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4527 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/onvif/videotab.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.702648 onvif-gui-1.1.8/gui/panels/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      180 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/panels/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3624 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/panels/audiopanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13463 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/panels/camerapanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14483 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/panels/filepanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13362 2023-05-18 17:30:04.000000 onvif-gui-1.1.8/gui/panels/settingspanel.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3627 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/panels/videopanel.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.706648 onvif-gui-1.1.8/gui/resources/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1936 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      252 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/apply.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      245 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/apply_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      244 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/apply_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      911 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/audio.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      536 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/audio_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      920 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/audio_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      203 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/branch_closed.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      219 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/branch_closed_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      211 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/branch_closed_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      199 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/branch_open.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      168 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/branch_open_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/branch_open_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      267 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/checked.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      235 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/checked_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      246 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/checked_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12716 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/darkstyle.qss
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      910 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/discover.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      849 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/discover_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      937 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/discover_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/fast-forward.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      253 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/fast-forward_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      433 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/fast-forward_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      641 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/mute.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      346 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/mute_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      618 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/mute_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      347 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/next.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      225 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/next_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/next_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    46084 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/onvif-gui.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      172 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/pause.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      144 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/pause_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      149 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/pause_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      321 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/play.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      209 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/play_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      316 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/play_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      349 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/previous.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      232 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/previous_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      348 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/previous_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/radio-off.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/radio-off_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      324 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/radio-off_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      350 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/radio-on.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      263 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/radio-on_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      343 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/radio-on_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      395 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/record.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      394 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/record_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      425 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/record_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      408 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/recording.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      435 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/recording_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      532 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/recording_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      454 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/rewind.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      250 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/rewind_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      457 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/rewind_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      187 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/small_arrow_left.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      183 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/small_arrow_left_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      189 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/small_arrow_left_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      162 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/small_arrow_up.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      160 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/small_arrow_up_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      161 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/small_arrow_up_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      158 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/stop.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      140 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/stop_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      151 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/stop_lo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/unchecked.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      142 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/unchecked_hi.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/gui/resources/unchecked_lo.png
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.706648 onvif-gui-1.1.8/modules/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/modules/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.706648 onvif-gui-1.1.8/modules/audio/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/modules/audio/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3404 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/modules/audio/sample.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.706648 onvif-gui-1.1.8/modules/video/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:13.000000 onvif-gui-1.1.8/modules/video/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6913 2023-05-13 16:10:05.000000 onvif-gui-1.1.8/modules/video/keypoint.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4768 2023-05-13 16:10:05.000000 onvif-gui-1.1.8/modules/video/retinanet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3095 2023-05-13 16:10:05.000000 onvif-gui-1.1.8/modules/video/sample.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7423 2023-05-13 16:10:05.000000 onvif-gui-1.1.8/modules/video/segment.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10650 2023-05-18 17:30:04.000000 onvif-gui-1.1.8/modules/video/yolov7.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8846 2023-05-18 17:30:04.000000 onvif-gui-1.1.8/modules/video/yolov8.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11968 2023-05-18 17:30:04.000000 onvif-gui-1.1.8/modules/video/yolox.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.706648 onvif-gui-1.1.8/onvif_gui.egg-info/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8849 2023-05-18 20:47:01.000000 onvif-gui-1.1.8/onvif_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8392 2023-05-18 20:47:01.000000 onvif-gui-1.1.8/onvif_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-05-18 20:47:01.000000 onvif-gui-1.1.8/onvif_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       39 2023-05-18 20:47:01.000000 onvif-gui-1.1.8/onvif_gui.egg-info/entry_points.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       47 2023-05-18 20:47:01.000000 onvif-gui-1.1.8/onvif_gui.egg-info/requires.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       44 2023-05-18 20:47:01.000000 onvif-gui-1.1.8/onvif_gui.egg-info/top_level.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1659 2023-05-18 20:42:20.000000 onvif-gui-1.1.8/pyproject.toml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-05-18 20:47:01.710648 onvif-gui-1.1.8/setup.cfg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1504 2023-05-18 20:42:15.000000 onvif-gui-1.1.8/setup.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.706648 onvif-gui-1.1.8/tracker/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-16 21:11:27.000000 onvif-gui-1.1.8/tracker/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      951 2023-05-16 21:11:27.000000 onvif-gui-1.1.8/tracker/basetrack.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12295 2023-05-16 21:11:27.000000 onvif-gui-1.1.8/tracker/byte_tracker.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9547 2023-05-16 21:11:27.000000 onvif-gui-1.1.8/tracker/kalman_filter.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6127 2023-05-16 21:11:27.000000 onvif-gui-1.1.8/tracker/matching.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.706648 onvif-gui-1.1.8/yolov7/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-17 15:41:51.000000 onvif-gui-1.1.8/yolov7/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.706648 onvif-gui-1.1.8/yolov7/models/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        6 2023-05-13 21:26:11.000000 onvif-gui-1.1.8/yolov7/models/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    84416 2023-05-15 21:22:28.000000 onvif-gui-1.1.8/yolov7/models/common.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10905 2023-05-15 21:22:28.000000 onvif-gui-1.1.8/yolov7/models/experimental.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    40052 2023-05-15 21:22:28.000000 onvif-gui-1.1.8/yolov7/models/yolo.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.710648 onvif-gui-1.1.8/yolov7/utils/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        6 2023-05-13 21:26:11.000000 onvif-gui-1.1.8/yolov7/utils/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2248 2023-05-13 21:26:11.000000 onvif-gui-1.1.8/yolov7/utils/activations.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5616 2023-05-13 21:26:11.000000 onvif-gui-1.1.8/yolov7/utils/add_nms.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7161 2023-05-15 21:22:28.000000 onvif-gui-1.1.8/yolov7/utils/autoanchor.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    56239 2023-05-15 21:22:28.000000 onvif-gui-1.1.8/yolov7/utils/datasets.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    36897 2023-05-15 21:22:28.000000 onvif-gui-1.1.8/yolov7/utils/general.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4873 2023-05-15 21:22:28.000000 onvif-gui-1.1.8/yolov7/utils/google_utils.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    75044 2023-05-15 21:22:28.000000 onvif-gui-1.1.8/yolov7/utils/loss.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9310 2023-05-13 21:26:11.000000 onvif-gui-1.1.8/yolov7/utils/metrics.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    20935 2023-05-15 21:22:28.000000 onvif-gui-1.1.8/yolov7/utils/plots.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15467 2023-05-13 21:26:11.000000 onvif-gui-1.1.8/yolov7/utils/torch_utils.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.710648 onvif-gui-1.1.8/yolox/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-08 16:34:27.000000 onvif-gui-1.1.8/yolox/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.710648 onvif-gui-1.1.8/yolox/models/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      936 2023-05-08 16:34:27.000000 onvif-gui-1.1.8/yolox/models/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4894 2023-05-08 16:34:27.000000 onvif-gui-1.1.8/yolox/models/build.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6647 2023-05-08 16:34:27.000000 onvif-gui-1.1.8/yolox/models/darknet.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2305 2023-05-08 16:34:27.000000 onvif-gui-1.1.8/yolox/models/losses.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6720 2023-05-08 16:34:27.000000 onvif-gui-1.1.8/yolox/models/network_blocks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3104 2023-05-08 16:34:27.000000 onvif-gui-1.1.8/yolox/models/yolo_fpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25526 2023-05-08 16:34:27.000000 onvif-gui-1.1.8/yolox/models/yolo_head.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4158 2023-05-08 16:34:27.000000 onvif-gui-1.1.8/yolox/models/yolo_pafpn.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1992 2023-05-08 16:34:27.000000 onvif-gui-1.1.8/yolox/models/yolox.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:47:01.710648 onvif-gui-1.1.8/yolox/utils/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      126 2023-05-08 16:34:27.000000 onvif-gui-1.1.8/yolox/utils/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1580 2023-05-08 16:34:27.000000 onvif-gui-1.1.8/yolox/utils/utils.py
```

### Comparing `onvif-gui-1.1.6/LICENSE` & `onvif-gui-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/PKG-INFO` & `onvif-gui-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.1.6
+Version: 1.1.8
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onvif-gui-1.1.6/README.md` & `onvif-gui-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/checkpoint/c2_model_loading.py` & `onvif-gui-1.1.8/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/checkpoint/catalog.py` & `onvif-gui-1.1.8/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/checkpoint/detection_checkpoint.py` & `onvif-gui-1.1.8/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/config/__init__.py` & `onvif-gui-1.1.8/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/config/compat.py` & `onvif-gui-1.1.8/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/config/config.py` & `onvif-gui-1.1.8/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/config/defaults.py` & `onvif-gui-1.1.8/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/config/instantiate.py` & `onvif-gui-1.1.8/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/config/lazy.py` & `onvif-gui-1.1.8/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/configs/Base-RCNN-FPN.yaml` & `onvif-gui-1.1.8/detectron2/configs/Base-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml` & `onvif-gui-1.1.8/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/__init__.py` & `onvif-gui-1.1.8/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/benchmark.py` & `onvif-gui-1.1.8/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/build.py` & `onvif-gui-1.1.8/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/catalog.py` & `onvif-gui-1.1.8/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/common.py` & `onvif-gui-1.1.8/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/dataset_mapper.py` & `onvif-gui-1.1.8/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/datasets/__init__.py` & `onvif-gui-1.1.8/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/datasets/builtin.py` & `onvif-gui-1.1.8/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/datasets/builtin_meta.py` & `onvif-gui-1.1.8/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/datasets/cityscapes.py` & `onvif-gui-1.1.8/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/datasets/cityscapes_panoptic.py` & `onvif-gui-1.1.8/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/datasets/coco.py` & `onvif-gui-1.1.8/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/datasets/coco_panoptic.py` & `onvif-gui-1.1.8/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/datasets/lvis.py` & `onvif-gui-1.1.8/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/datasets/lvis_v0_5_categories.py` & `onvif-gui-1.1.8/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/datasets/lvis_v1_categories.py` & `onvif-gui-1.1.8/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/datasets/lvis_v1_category_image_count.py` & `onvif-gui-1.1.8/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/datasets/pascal_voc.py` & `onvif-gui-1.1.8/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/detection_utils.py` & `onvif-gui-1.1.8/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/samplers/distributed_sampler.py` & `onvif-gui-1.1.8/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/samplers/grouped_batch_sampler.py` & `onvif-gui-1.1.8/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/transforms/augmentation.py` & `onvif-gui-1.1.8/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/transforms/augmentation_impl.py` & `onvif-gui-1.1.8/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/data/transforms/transform.py` & `onvif-gui-1.1.8/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/layers/__init__.py` & `onvif-gui-1.1.8/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/layers/aspp.py` & `onvif-gui-1.1.8/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/layers/batch_norm.py` & `onvif-gui-1.1.8/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/layers/blocks.py` & `onvif-gui-1.1.8/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/layers/deform_conv.py` & `onvif-gui-1.1.8/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/layers/losses.py` & `onvif-gui-1.1.8/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/layers/mask_ops.py` & `onvif-gui-1.1.8/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/layers/nms.py` & `onvif-gui-1.1.8/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/layers/roi_align.py` & `onvif-gui-1.1.8/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/layers/roi_align_rotated.py` & `onvif-gui-1.1.8/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/layers/rotated_boxes.py` & `onvif-gui-1.1.8/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/layers/shape_spec.py` & `onvif-gui-1.1.8/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/layers/wrappers.py` & `onvif-gui-1.1.8/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/__init__.py` & `onvif-gui-1.1.8/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/anchor_generator.py` & `onvif-gui-1.1.8/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/backbone/__init__.py` & `onvif-gui-1.1.8/detectron2/modeling/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/backbone/backbone.py` & `onvif-gui-1.1.8/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/backbone/build.py` & `onvif-gui-1.1.8/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/backbone/fpn.py` & `onvif-gui-1.1.8/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/backbone/mvit.py` & `onvif-gui-1.1.8/detectron2/modeling/backbone/mvit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/backbone/regnet.py` & `onvif-gui-1.1.8/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/backbone/resnet.py` & `onvif-gui-1.1.8/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/backbone/swin.py` & `onvif-gui-1.1.8/detectron2/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/backbone/utils.py` & `onvif-gui-1.1.8/detectron2/modeling/backbone/utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/backbone/vit.py` & `onvif-gui-1.1.8/detectron2/modeling/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/box_regression.py` & `onvif-gui-1.1.8/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/matcher.py` & `onvif-gui-1.1.8/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/meta_arch/build.py` & `onvif-gui-1.1.8/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/meta_arch/dense_detector.py` & `onvif-gui-1.1.8/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/meta_arch/fcos.py` & `onvif-gui-1.1.8/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/meta_arch/panoptic_fpn.py` & `onvif-gui-1.1.8/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/meta_arch/rcnn.py` & `onvif-gui-1.1.8/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/meta_arch/retinanet.py` & `onvif-gui-1.1.8/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/meta_arch/semantic_seg.py` & `onvif-gui-1.1.8/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/mmdet_wrapper.py` & `onvif-gui-1.1.8/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/poolers.py` & `onvif-gui-1.1.8/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/postprocessing.py` & `onvif-gui-1.1.8/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/proposal_generator/build.py` & `onvif-gui-1.1.8/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/proposal_generator/proposal_utils.py` & `onvif-gui-1.1.8/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/proposal_generator/rpn.py` & `onvif-gui-1.1.8/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/proposal_generator/rrpn.py` & `onvif-gui-1.1.8/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/roi_heads/__init__.py` & `onvif-gui-1.1.8/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/roi_heads/box_head.py` & `onvif-gui-1.1.8/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/roi_heads/cascade_rcnn.py` & `onvif-gui-1.1.8/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/roi_heads/fast_rcnn.py` & `onvif-gui-1.1.8/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/roi_heads/keypoint_head.py` & `onvif-gui-1.1.8/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/roi_heads/mask_head.py` & `onvif-gui-1.1.8/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/roi_heads/roi_heads.py` & `onvif-gui-1.1.8/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `onvif-gui-1.1.8/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/sampling.py` & `onvif-gui-1.1.8/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/modeling/test_time_augmentation.py` & `onvif-gui-1.1.8/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/predictor.py` & `onvif-gui-1.1.8/detectron2/predictor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/structures/__init__.py` & `onvif-gui-1.1.8/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/structures/boxes.py` & `onvif-gui-1.1.8/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/structures/image_list.py` & `onvif-gui-1.1.8/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/structures/instances.py` & `onvif-gui-1.1.8/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/structures/keypoints.py` & `onvif-gui-1.1.8/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/structures/masks.py` & `onvif-gui-1.1.8/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/structures/rotated_boxes.py` & `onvif-gui-1.1.8/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/tracker.py` & `onvif-gui-1.1.8/detectron2/tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/analysis.py` & `onvif-gui-1.1.8/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/collect_env.py` & `onvif-gui-1.1.8/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/colormap.py` & `onvif-gui-1.1.8/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/comm.py` & `onvif-gui-1.1.8/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/develop.py` & `onvif-gui-1.1.8/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/env.py` & `onvif-gui-1.1.8/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/events.py` & `onvif-gui-1.1.8/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/file_io.py` & `onvif-gui-1.1.8/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/logger.py` & `onvif-gui-1.1.8/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/memory.py` & `onvif-gui-1.1.8/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/registry.py` & `onvif-gui-1.1.8/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/serialize.py` & `onvif-gui-1.1.8/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/testing.py` & `onvif-gui-1.1.8/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/video_visualizer.py` & `onvif-gui-1.1.8/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/detectron2/utils/visualizer.py` & `onvif-gui-1.1.8/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/components/comboselector.py` & `onvif-gui-1.1.8/gui/components/comboselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/components/directoryselector.py` & `onvif-gui-1.1.8/gui/components/directoryselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/components/fileselector.py` & `onvif-gui-1.1.8/gui/components/fileselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/components/labelselector.py` & `onvif-gui-1.1.8/gui/components/labelselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/components/progress.py` & `onvif-gui-1.1.8/gui/components/progress.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/components/thresholdslider.py` & `onvif-gui-1.1.8/gui/components/thresholdslider.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/glwidget.py` & `onvif-gui-1.1.8/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/main.py` & `onvif-gui-1.1.8/gui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,14 @@
 from gui.glwidget import GLWidget
 from loguru import logger
 
 sys.path.append("../build/libavio")
 sys.path.append("../build/libavio/Release")
 import avio
 
-FORCE_DIRECT_RENDER = False
-
 class MainWindowSignals(QObject):
     started = pyqtSignal(int)
     stopped = pyqtSignal()
     progress = pyqtSignal(float)
     error = pyqtSignal(str)
 
 class ViewLabel(QLabel):
@@ -52,15 +50,15 @@
 
 class MainWindow(QMainWindow):
     def __init__(self, clear_settings=False):
         super().__init__()
         os.environ["QT_FILESYSTEMMODEL_WATCH_FILES"] = "ON"
         QDir.addSearchPath("image", self.getLocation() + "/gui/resources/")
         self.style()
-        self.program_name = "onvif gui version 1.1.6"
+        self.program_name = "onvif gui version 1.1.8"
         self.setWindowTitle(self.program_name)
         self.setWindowIcon(QIcon('image:onvif-gui.png'))
         self.settings = QSettings("onvif", "gui")
         if clear_settings:
             self.settings.clear()
         self.volumeKey = "MainWindow/volume"
         self.muteKey = "MainWindow/mute"
@@ -98,21 +96,18 @@
         self.tab.addTab(self.cameraPanel, "Cameras")
         self.tab.addTab(self.filePanel, "Files")
         self.tab.addTab(self.settingsPanel, "Settings")
         self.tab.addTab(self.videoPanel, "Video")
         self.tab.addTab(self.audioPanel, "Audio")
         self.tab.setCurrentIndex(int(self.settings.value(self.tabIndexKey, 0)))
 
-        if FORCE_DIRECT_RENDER:
-            self.glWidget = ViewLabel()
+        if self.settings.value(self.settingsPanel.renderKey, 0) == 0:
+            self.glWidget = GLWidget()
         else:
-            if self.settings.value(self.settingsPanel.renderKey, 0) == 0:
-                self.glWidget = GLWidget()
-            else:
-                self.glWidget = ViewLabel()
+            self.glWidget = ViewLabel()
 
         self.split = QSplitter()
         self.split.addWidget(self.glWidget)
         self.split.addWidget(self.tab)
         self.split.setStretchFactor(0, 10)
         self.split.splitterMoved.connect(self.splitterMoved)
         splitterState = self.settings.value(self.splitKey)
@@ -227,21 +222,18 @@
         if "fps=" in self.player.video_filter:
             self.filePanel.progress.setEnabled(False)
 
         audio_filter = self.settingsPanel.txtAudioFilter.text()
         if len(audio_filter) > 0:
             self.player.audio_filter = audio_filter
 
-        if FORCE_DIRECT_RENDER:
-            self.player.hWnd = self.glWidget.winId()
+        if self.settings.value(self.settingsPanel.renderKey, 0) == 0:
+            self.player.renderCallback = lambda F : self.glWidget.renderCallback(F)
         else:
-            if self.settings.value(self.settingsPanel.renderKey, 0) == 0:
-                self.player.renderCallback = lambda F : self.glWidget.renderCallback(F)
-            else:
-                self.player.hWnd = self.glWidget.winId()
+            self.player.hWnd = self.glWidget.winId()
 
         self.player.disable_audio = self.settingsPanel.chkDisableAudio.isChecked()
         self.player.disable_video = self.settingsPanel.chkDisableVideo.isChecked()
 
         self.player.pythonCallback = lambda F : self.pyVideoCallback(F)
         self.player.pyAudioCallback = lambda F: self.pyAudioCallback(F)
         self.player.cbMediaPlayingStarted = lambda n : self.mediaPlayingStarted(n)
@@ -250,14 +242,15 @@
         self.player.infoCallback = lambda s : self.infoCallback(s)
         self.player.setVolume(int(self.volume))
         self.player.setMute(self.mute)
         self.player.keyframe_cache_size = self.settingsPanel.spnCacheSize.value()
         self.player.hw_device_type = self.settingsPanel.getDecoder()
         self.player.hw_encoding = self.settingsPanel.chkHardwareEncode.isChecked()
         self.player.post_encode = self.settingsPanel.chkPostEncode.isChecked()
+        self.player.process_pause = self.settingsPanel.chkProcessPause.isChecked()
         self.player.start()
         self.cameraPanel.setEnabled(False)
 
     def stopMedia(self):
         if self.player is not None:
             self.player.running = False
         while self.playing:
```

### Comparing `onvif-gui-1.1.6/gui/onvif/admintab.py` & `onvif-gui-1.1.8/gui/onvif/admintab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/onvif/imagetab.py` & `onvif-gui-1.1.8/gui/onvif/imagetab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/onvif/logindialog.py` & `onvif-gui-1.1.8/gui/onvif/logindialog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/onvif/networktab.py` & `onvif-gui-1.1.8/gui/onvif/networktab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/onvif/ptztab.py` & `onvif-gui-1.1.8/gui/onvif/ptztab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/onvif/videotab.py` & `onvif-gui-1.1.8/gui/onvif/videotab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/panels/audiopanel.py` & `onvif-gui-1.1.8/gui/panels/audiopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/panels/camerapanel.py` & `onvif-gui-1.1.8/gui/panels/camerapanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/panels/filepanel.py` & `onvif-gui-1.1.8/gui/panels/filepanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/panels/settingspanel.py` & `onvif-gui-1.1.8/gui/panels/settingspanel.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         self.renderKey = "settings/render"
         self.convertKey = "settings/convert"
         self.workerKey = "settings/worker"
         self.disableAudioKey = "settings/disableAudio"
         self.disableVideoKey = "settings/disableVideo"
         self.postEncodeKey = "settings/postEncode"
         self.hardwareEncodeKey = "settings/hardwareEncode"
+        self.processPauseKey = "settings/processPause"
         self.processFrameKey = "settings/processFrame"
         self.cacheSizeKey = "settings/cacheSize"
         self.interfaceKey = "settings/interface"
         self.videoFilterKey = "settings/videoFilter"
         self.audioFilterKey = "settings/audioFilter"
 
         decoders = ["NONE", "CUDA", "VAAPI", "VDPAU", "DXVA2", "D3D11VA"]
@@ -108,26 +109,31 @@
         self.chkPostEncode.stateChanged.connect(self.postEncodeChecked)
 
         self.chkHardwareEncode = QCheckBox("Hardware Encode")
         self.chkHardwareEncode.setChecked(int(mw.settings.value(self.hardwareEncodeKey, 0)))
         self.chkHardwareEncode.setEnabled(self.chkPostEncode.isChecked())
         self.chkHardwareEncode.stateChanged.connect(self.hardwareEncodeChecked)
 
+        self.chkProcessPause = QCheckBox("Process Pause")
+        self.chkProcessPause.setChecked(int(mw.settings.value(self.processPauseKey, 0)))
+        self.chkProcessPause.stateChanged.connect(self.processPauseChecked)
+
         self.chkLowLatency = QCheckBox("Low Latency")
         self.chkLowLatency.setChecked(int(mw.settings.value(self.latencyKey, 0)))
         self.chkLowLatency.stateChanged.connect(self.lowLatencyChecked)
 
         pnlChecks = QWidget()
         lytChecks = QGridLayout(pnlChecks)
         lytChecks.addWidget(self.chkDirectRender,   0, 0, 1, 1)
         lytChecks.addWidget(self.chkConvert2RGB,    0, 1, 1, 1)
         lytChecks.addWidget(self.chkDisableAudio,   1, 0, 1, 1)
         lytChecks.addWidget(self.chkDisableVideo,   1, 1, 1, 1)
         lytChecks.addWidget(self.chkPostEncode,     2, 0, 1, 1)
         lytChecks.addWidget(self.chkHardwareEncode, 2, 1, 1, 1)
+        lytChecks.addWidget(self.chkProcessPause,   3, 0, 1, 1)
         lytChecks.addWidget(self.chkLowLatency,     3, 1, 1, 1)
 
         self.spnCacheSize = QSpinBox()
         self.spnCacheSize.setMinimum(1)
         self.spnCacheSize.setMaximum(10)
         self.spnCacheSize.setMaximumWidth(80)
         self.spnCacheSize.setValue(int(self.mw.settings.value(self.cacheSizeKey, 1)))
@@ -246,14 +252,17 @@
         if state == 0:
             self.chkHardwareEncode.setChecked(False)
         self.chkHardwareEncode.setEnabled(state)
 
     def hardwareEncodeChecked(self, state):
         self.mw.settings.setValue(self.hardwareEncodeKey, state)
 
+    def processPauseChecked(self, state):
+        self.mw.settings.setValue(self.processPauseKey, state)
+
     def lowLatencyChecked(self, state):
         self.mw.settings.setValue(self.latencyKey, state)
 
     def radioFilenameChecked(self):
         if self.radGenerateFilename.isChecked():
             self.mw.settings.setValue(self.generateKey, 1)
         else:
```

### Comparing `onvif-gui-1.1.6/gui/panels/videopanel.py` & `onvif-gui-1.1.8/gui/panels/videopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/resources/LICENSE` & `onvif-gui-1.1.8/gui/resources/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/resources/audio.png` & `onvif-gui-1.1.8/gui/resources/audio.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/resources/audio_hi.png` & `onvif-gui-1.1.8/gui/resources/audio_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/resources/audio_lo.png` & `onvif-gui-1.1.8/gui/resources/audio_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/resources/darkstyle.qss` & `onvif-gui-1.1.8/gui/resources/darkstyle.qss`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/resources/discover.png` & `onvif-gui-1.1.8/gui/resources/discover.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/resources/discover_hi.png` & `onvif-gui-1.1.8/gui/resources/discover_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/resources/discover_lo.png` & `onvif-gui-1.1.8/gui/resources/discover_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/resources/mute.png` & `onvif-gui-1.1.8/gui/resources/mute.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/resources/mute_lo.png` & `onvif-gui-1.1.8/gui/resources/mute_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/resources/onvif-gui.png` & `onvif-gui-1.1.8/gui/resources/onvif-gui.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/gui/resources/recording_lo.png` & `onvif-gui-1.1.8/gui/resources/recording_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/modules/audio/sample.py` & `onvif-gui-1.1.8/modules/audio/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/modules/video/keypoint.py` & `onvif-gui-1.1.8/modules/video/keypoint.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/modules/video/retinanet.py` & `onvif-gui-1.1.8/modules/video/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/modules/video/sample.py` & `onvif-gui-1.1.8/modules/video/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/modules/video/segment.py` & `onvif-gui-1.1.8/modules/video/segment.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/modules/video/yolov7.py` & `onvif-gui-1.1.8/modules/video/yolov7.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #*********************************************************************/
 
 IMPORT_ERROR = ""
 try:
     import cv2
     import os
     import sys
+    import gc
     import numpy as np
     from pathlib import Path
     from loguru import logger
 
     from gui.components import ComboSelector, FileSelector, LabelSelector, ThresholdSlider
     from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QCheckBox, QMessageBox
     from PyQt6.QtCore import Qt
@@ -55,26 +56,25 @@
 class VideoConfigure(QWidget):
     def __init__(self, mw):
         try:
             super().__init__()
             self.mw = mw
             self.name = MODULE_NAME
             self.autoKey = "Module/" + MODULE_NAME + "/autoDownload"
-            self.fp16Key = "Module/" + MODULE_NAME + "/fp16"
             self.trackKey = "Module/" + MODULE_NAME + "/track"
 
             self.chkAuto = QCheckBox("Automatically download model")
             self.chkAuto.setChecked(int(self.mw.settings.value(self.autoKey, 1)))
             self.chkAuto.stateChanged.connect(self.chkAutoClicked)
 
             self.txtFilename = FileSelector(mw, MODULE_NAME)
             self.txtFilename.setEnabled(not self.chkAuto.isChecked())
 
-            self.cmbRes = ComboSelector(mw, "Model Size", ("320", "480", "640", "960", "1280", "1440"), "640", MODULE_NAME)
-            self.cmbType = ComboSelector(mw, "Model Name", ("yolov7", "yolov7x", "yolov7-w6", "yolov7-e6", "yolov7-d6", "yolov7-e6e"), "yolov7", MODULE_NAME)
+            self.cmbRes = ComboSelector(mw, "Model Size", ("320", "480", "640", "960", "1280"), "640", MODULE_NAME)
+            self.cmbType = ComboSelector(mw, "Model Name", ("yolov7", "yolov7x"), "yolov7", MODULE_NAME)
 
             self.chkTrack = QCheckBox("Track Objects")
             self.chkTrack.setChecked(int(self.mw.settings.value(self.trackKey, 0)))
             self.chkTrack.stateChanged.connect(self.chkTrackClicked)
 
             self.sldConfThre = ThresholdSlider(mw, MODULE_NAME + "/confidence", "Confidence", 25)
 
@@ -143,14 +143,20 @@
 
             weights = self.ckpt_file
             res = int(self.mw.configure.cmbRes.currentText())
             self.iou_thres = 0.45
 
             self.device = select_device('')
             self.half = self.device.type != 'cpu'
+
+            self.model = None
+            gc.collect()
+            with torch.no_grad():
+                torch.cuda.empty_cache()
+
             self.model = attempt_load(weights, map_location=self.device)
             self.stride = int(self.model.stride.max())
             if self.half:
                 self.model.half()
             self.names = self.model.module.names if hasattr(self.model, 'module') else self.model.names
             with torch.no_grad():
                 self.model(torch.zeros(1, 3, res, res).to(self.device).type_as(next(self.model.parameters())))
@@ -174,22 +180,14 @@
             img = np.ascontiguousarray(img)
             img = torch.from_numpy(img).to(self.device)
             img = img.half() if self.half else img.float()
             img /= 255.0
             if img.ndimension() == 3:
                 img = img.unsqueeze(0)
 
-            tmp = None
-            if self.mw.configure.chkAuto.isChecked():
-                tmp = self.get_auto_ckpt_filename()
-            else:
-                tmp = self.mw.configure.txtFilename.text()
-            if self.ckpt_file != tmp:
-                self.__init__(self.mw)
-
             with torch.no_grad():
                 pred = self.model(img, augment=False)[0]
 
             conf_thres = self.mw.configure.sldConfThre.value()
             if self.mw.configure.chkTrack.isChecked():
                 conf_thres = 0.001
 
@@ -203,15 +201,14 @@
             pred = non_max_suppression(pred, conf_thres, self.iou_thres, classes=label_filter, agnostic=False)
 
             boxes = pred[0]
             if len(boxes):
                 boxes[:, :4] = scale_coords(img.shape[2:], boxes[:, :4], original_img.shape).round()
                 boxes = boxes.cpu().numpy()
 
-
                 if self.mw.configure.chkTrack.isChecked():
                     w = original_img.shape[0]
                     h = original_img.shape[1]
                     if self.track_thresh != self.mw.configure.sldConfThre.value():
                         self.track_thresh = self.mw.configure.sldConfThre.value()
                         self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh)
 
@@ -234,14 +231,22 @@
                         label_counts[cls] += 1
                         color = self.mw.configure.getLabel(cls).color()
                         cv2.rectangle(original_img, (x1, y1), (x2, y2), color, 2)
 
             for lbl in label_filter:
                 self.mw.configure.getLabel(lbl).setCount(label_counts[lbl])
 
+            tmp = None
+            if self.mw.configure.chkAuto.isChecked():
+                tmp = self.get_auto_ckpt_filename()
+            else:
+                tmp = self.mw.configure.txtFilename.text()
+            if self.ckpt_file != tmp:
+                self.__init__(self.mw)
+
         except Exception as ex:
             if self.last_ex != str(ex) and self.mw.configure.name == MODULE_NAME:
                 logger.exception(MODULE_NAME + " runtime error")
             self.last_ex = str(ex)
 
     def get_auto_ckpt_filename(self):
         filename = None
```

### Comparing `onvif-gui-1.1.6/modules/video/yolov8.py` & `onvif-gui-1.1.8/modules/video/yolov8.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,14 @@
     def chkAutoClicked(self, state):
         self.mw.settings.setValue(self.autoKey, state)
         self.cmbModel.setEnabled(self.chkAuto.isChecked())
         self.txtModelFile.setEnabled(not self.chkAuto.isChecked())
 
     def chkTrackClicked(self,state):
         self.mw.settings.setValue(self.trackKey, state)
-        self.sldConfThre.setEnabled(not self.chkTrack.isChecked())
 
     def getModelName(self):
         if self.chkAuto.isChecked():
             return self.model_names[self.cmbModel.currentText()]
         else:
             return self.txtModelFile.text()
         
@@ -149,14 +148,16 @@
 
             confthre = self.mw.configure.sldConfThre.value()
             if self.mw.configure.chkTrack.isChecked():
                 confthre = 0.001
 
             if self.model_name != self.mw.configure.getModelName():
                 self.model_name = self.mw.configure.getModelName()
+                with torch.no_grad():
+                    torch.cuda.empty_cache()
                 self.model = YOLO(self.model_name)
 
             res = int(self.mw.configure.cmbRes.currentText())
                 
             results = self.model.predict(img, stream=True, verbose=False, 
                                          classes=label_filter,
                                          conf=confthre, 
@@ -199,10 +200,7 @@
                 for lbl in label_filter:
                     self.mw.configure.getLabel(lbl).setCount(label_counts[lbl])
             
         except Exception as ex:
             if self.last_ex != str(ex) and self.mw.configure.name == MODULE_NAME:
                 logger.exception(MODULE_NAME + " runtime error")
             self.last_ex = str(ex)
-
-
-
```

### Comparing `onvif-gui-1.1.6/modules/video/yolox.py` & `onvif-gui-1.1.8/modules/video/yolox.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,30 +48,30 @@
 class VideoConfigure(QWidget):
     def __init__(self, mw):
         try:
             super().__init__()
             self.mw = mw
             self.name = MODULE_NAME
             self.autoKey = "Module/" + MODULE_NAME + "/autoDownload"
-            self.fp16Key = "Module/" + MODULE_NAME + "/fp16"
+            #self.fp16Key = "Module/" + MODULE_NAME + "/fp16"
             self.trackKey = "Module/" + MODULE_NAME + "/track"
 
             self.chkAuto = QCheckBox("Automatically download model")
             self.chkAuto.setChecked(int(self.mw.settings.value(self.autoKey, 1)))
             self.chkAuto.stateChanged.connect(self.chkAutoClicked)
 
             self.txtFilename = FileSelector(mw, MODULE_NAME)
             self.txtFilename.setEnabled(not self.chkAuto.isChecked())
 
             self.cmbRes = ComboSelector(mw, "Model Size", ("320", "480", "640", "960", "1280", "1440"), "640", MODULE_NAME)
             self.cmbType = ComboSelector(mw, "Model Name", ("yolox_s", "yolox_m", "yolox_l", "yolox_x"), "yolox_s", MODULE_NAME)
 
-            self.chkFP16 = QCheckBox("Use half precision math")
-            self.chkFP16.setChecked(int(self.mw.settings.value(self.fp16Key, 1)))
-            self.chkFP16.stateChanged.connect(self.chkFP16Clicked)
+            #self.chkFP16 = QCheckBox("Use half precision math")
+            #self.chkFP16.setChecked(int(self.mw.settings.value(self.fp16Key, 1)))
+            #self.chkFP16.stateChanged.connect(self.chkFP16Clicked)
 
             self.chkTrack = QCheckBox("Track Objects")
             self.chkTrack.setChecked(int(self.mw.settings.value(self.trackKey, 0)))
             self.chkTrack.stateChanged.connect(self.chkTrackClicked)
 
             self.sldConfThre = ThresholdSlider(mw, MODULE_NAME + "/confidence", "Confidence", 25)
 
@@ -90,15 +90,15 @@
 
             lytMain = QGridLayout(self)
             lytMain.addWidget(self.chkAuto,      0, 0, 1, 1)
             lytMain.addWidget(self.cmbType,      1, 0, 1, 1)
             lytMain.addWidget(self.txtFilename,  2, 0, 1, 1)
             lytMain.addWidget(self.cmbRes,       3, 0, 1, 1)
             lytMain.addWidget(self.sldConfThre,  4, 0, 1, 1)
-            lytMain.addWidget(self.chkFP16,      5, 0, 1, 1)
+            #lytMain.addWidget(self.chkFP16,      5, 0, 1, 1)
             lytMain.addWidget(self.chkTrack,     6, 0, 1, 1)
             lytMain.addWidget(pnlLabels,         7, 0, 1, 1)
             lytMain.addWidget(QLabel(),          8, 0, 1, 1)
             lytMain.setRowStretch(8, 10)
 
             if len(IMPORT_ERROR) > 0:
                 QMessageBox.critical(None, MODULE_NAME + " Import Error", "Modules required for running this function are missing: " + IMPORT_ERROR)
@@ -106,16 +106,16 @@
         except:
             logger.exception(MODULE_NAME + " configure failed to load")
 
     def chkAutoClicked(self, state):
         self.mw.settings.setValue(self.autoKey, state)
         self.txtFilename.setEnabled(not self.chkAuto.isChecked())
 
-    def chkFP16Clicked(self, state):
-        self.mw.settings.setValue(self.fp16Key, state)
+    #def chkFP16Clicked(self, state):
+    #    self.mw.settings.setValue(self.fp16Key, state)
 
     def chkTrackClicked(self, state):
         self.mw.settings.setValue(self.trackKey, state)
 
 class VideoWorker:
     def __init__(self, mw):
         try:
@@ -124,16 +124,16 @@
             device_name = "cpu"
             if torch.cuda.is_available():
                 device_name = "cuda"
             self.device = torch.device(device_name)
 
             self.num_classes = 80
 
-            self.fp16 = self.mw.configure.chkFP16.isChecked()
-            self.track = self.mw.configure.chkTrack.isChecked()
+            #self.fp16 = self.mw.configure.chkFP16.isChecked()
+            #self.track = self.mw.configure.chkTrack.isChecked()
 
             size = {'yolox_s': [0.33, 0.50], 
                     'yolox_m': [0.67, 0.75],
                     'yolox_l': [1.00, 1.00],
                     'yolox_x': [1.33, 1.25]}[self.mw.configure.cmbType.currentText()]
 
             self.model = None
@@ -151,16 +151,16 @@
                     link = "https://github.com/Megvii-BaseDetection/YOLOX/releases/download/0.1.1rc0/" + model_name + ".pth"
                     torch.hub.download_url_to_file(link, self.ckpt_file)
             else:
                 self.ckpt_file = self.mw.configure.txtFilename.text()
 
             self.model.load_state_dict(torch.load(self.ckpt_file, map_location="cpu")["model"])
 
-            if self.fp16:
-                self.model = self.model.half()
+            #if self.fp16:
+            #    self.model = self.model.half()
 
             self.track_thresh = self.mw.configure.sldConfThre.value()
             self.track_buffer = 30
             self.match_thresh = 0.8
 
             self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh)
 
@@ -181,24 +181,16 @@
 
             timg = functional.to_tensor(img.copy()).to(self.device)
             timg *= 255
             timg = functional.resize(timg, inf_shape)
             timg = functional.pad(timg, pad, 114)
             timg = timg.unsqueeze(0)
 
-            if self.fp16:
-                timg = timg.half()  # to FP16
-
-            tmp = None
-            if self.mw.configure.chkAuto.isChecked():
-                tmp = self.get_auto_ckpt_filename()
-            else:
-                tmp = self.mw.configure.txtFilename.text()
-            if self.ckpt_file != tmp:
-                self.__init__(self.mw)
+            #if self.fp16:
+            #    timg = timg.half()  # to FP16
 
             if self.mw.configure.chkTrack.isChecked():
                 confthre = 0.001
             else:
                 confthre = self.mw.configure.sldConfThre.value()
             
             nmsthre = 0.65
@@ -225,14 +217,22 @@
                         self.tracker = BYTETracker(self.track_thresh, self.track_buffer, self.match_thresh)
 
                     online_targets = self.tracker.update(output, [img.shape[0], img.shape[1]], test_size)
                     self.draw_track_boxes(img, online_targets)
                 else:
                     self.draw_plain_boxes(img, output, ratio)
 
+            tmp = None
+            if self.mw.configure.chkAuto.isChecked():
+                tmp = self.get_auto_ckpt_filename()
+            else:
+                tmp = self.mw.configure.txtFilename.text()
+            if self.ckpt_file != tmp:
+                self.__init__(self.mw)
+
         except Exception as ex:
             if self.last_ex != str(ex) and self.mw.configure.name == MODULE_NAME:
                 logger.exception(MODULE_NAME + " runtime error")
             self.last_ex = str(ex)
 
     def draw_plain_boxes(self, img, output, ratio):
         boxes = output[:, 0:4] / ratio
```

### Comparing `onvif-gui-1.1.6/onvif_gui.egg-info/PKG-INFO` & `onvif-gui-1.1.8/onvif_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 1.1.6
+Version: 1.1.8
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `onvif-gui-1.1.6/onvif_gui.egg-info/SOURCES.txt` & `onvif-gui-1.1.8/onvif_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/pyproject.toml` & `onvif-gui-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 [project]
 name = "onvif-gui" 
-version = "1.1.6"  
+version = "1.1.8"  
 description = "A client gui for Onvif"  
 readme = "README.md" 
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]  
 authors = [
   {name = "Stephen Rhodes", email = "sr99622@gmail.com" }
```

### Comparing `onvif-gui-1.1.6/setup.py` & `onvif-gui-1.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from setuptools.command.install import install
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="onvif-gui",
-    version="1.1.6",
+    version="1.1.8",
     author="Stephen Rhodes",
     author_email="sr99622@gmail.com",
     description="GUI program for onvif",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `onvif-gui-1.1.6/tracker/basetrack.py` & `onvif-gui-1.1.8/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/tracker/byte_tracker.py` & `onvif-gui-1.1.8/tracker/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/tracker/kalman_filter.py` & `onvif-gui-1.1.8/tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/tracker/matching.py` & `onvif-gui-1.1.8/tracker/matching.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolov7/models/common.py` & `onvif-gui-1.1.8/yolov7/models/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolov7/models/experimental.py` & `onvif-gui-1.1.8/yolov7/models/experimental.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolov7/models/yolo.py` & `onvif-gui-1.1.8/yolov7/models/yolo.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolov7/utils/activations.py` & `onvif-gui-1.1.8/yolov7/utils/activations.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolov7/utils/add_nms.py` & `onvif-gui-1.1.8/yolov7/utils/add_nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolov7/utils/autoanchor.py` & `onvif-gui-1.1.8/yolov7/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolov7/utils/datasets.py` & `onvif-gui-1.1.8/yolov7/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolov7/utils/general.py` & `onvif-gui-1.1.8/yolov7/utils/general.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolov7/utils/google_utils.py` & `onvif-gui-1.1.8/yolov7/utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolov7/utils/loss.py` & `onvif-gui-1.1.8/yolov7/utils/loss.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolov7/utils/metrics.py` & `onvif-gui-1.1.8/yolov7/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolov7/utils/plots.py` & `onvif-gui-1.1.8/yolov7/utils/plots.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolov7/utils/torch_utils.py` & `onvif-gui-1.1.8/yolov7/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolox/models/__init__.py` & `onvif-gui-1.1.8/yolox/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolox/models/build.py` & `onvif-gui-1.1.8/yolox/models/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolox/models/darknet.py` & `onvif-gui-1.1.8/yolox/models/darknet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolox/models/losses.py` & `onvif-gui-1.1.8/yolox/models/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolox/models/network_blocks.py` & `onvif-gui-1.1.8/yolox/models/network_blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolox/models/yolo_fpn.py` & `onvif-gui-1.1.8/yolox/models/yolo_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolox/models/yolo_head.py` & `onvif-gui-1.1.8/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolox/models/yolo_pafpn.py` & `onvif-gui-1.1.8/yolox/models/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolox/models/yolox.py` & `onvif-gui-1.1.8/yolox/models/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.1.6/yolox/utils/utils.py` & `onvif-gui-1.1.8/yolox/utils/utils.py`

 * *Files identical despite different names*

