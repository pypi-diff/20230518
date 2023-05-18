# Comparing `tmp/tepe-0.6.9.5-py3-none-any.whl.zip` & `tmp/tepe-0.7.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,163 +1,301 @@
-Zip file size: 267288 bytes, number of entries: 161
--rw-rw-r--  2.0 unx      134 b- defN 23-Jan-10 08:16 tepe/__init__.py
--rw-rw-r--  2.0 unx      274 b- defN 22-Dec-21 12:51 tepe/core/__init__.py
--rw-rw-r--  2.0 unx     3820 b- defN 22-Oct-25 02:49 tepe/core/base_evaluator.py
--rw-rw-r--  2.0 unx     6474 b- defN 22-Dec-23 03:42 tepe/core/base_predictor.py
--rw-rw-r--  2.0 unx     8654 b- defN 22-Oct-28 02:33 tepe/core/base_task.py
--rw-rw-r--  2.0 unx    12207 b- defN 22-Oct-25 02:49 tepe/core/base_trainer.py
--rw-rw-r--  2.0 unx     5180 b- defN 22-Oct-25 02:49 tepe/core/exporter.py
--rw-rw-r--  2.0 unx     4331 b- defN 22-Dec-21 12:55 tepe/core/launch.py
--rw-rw-r--  2.0 unx     3437 b- defN 22-Nov-11 04:32 tepe/core/register.py
--rw-rw-r--  2.0 unx       79 b- defN 22-Oct-25 02:49 tepe/core/evaluator/__init__.py
--rw-rw-r--  2.0 unx     1697 b- defN 22-Oct-25 02:49 tepe/core/evaluator/cls_evaluator.py
--rw-rw-r--  2.0 unx     2194 b- defN 22-Oct-25 02:49 tepe/core/evaluator/seg_evaluator.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Oct-25 02:49 tepe/core/evaluator/metrics/__init__.py
--rw-rw-r--  2.0 unx      627 b- defN 22-Oct-25 02:49 tepe/core/evaluator/metrics/cls_metrics.py
--rw-rw-r--  2.0 unx     2117 b- defN 22-Oct-25 02:49 tepe/core/evaluator/metrics/seg_metrics.py
--rw-rw-r--  2.0 unx     5820 b- defN 22-Oct-25 02:49 tepe/core/evaluator/metrics/voc_metrics.py
--rw-rw-r--  2.0 unx      109 b- defN 22-Oct-25 02:49 tepe/core/predictor/__init__.py
--rw-rw-r--  2.0 unx     1409 b- defN 22-Dec-22 09:01 tepe/core/predictor/anomaly_detector.py
--rw-rw-r--  2.0 unx     3258 b- defN 22-Oct-25 02:49 tepe/core/predictor/classifier.py
--rw-rw-r--  2.0 unx     2247 b- defN 22-Oct-25 02:49 tepe/core/predictor/segmentor.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Oct-25 01:29 tepe/core/task_config/__init__.py
--rw-rw-r--  2.0 unx     9176 b- defN 22-Nov-09 02:59 tepe/core/task_config/anomaly_detection_task.py
--rw-rw-r--  2.0 unx       71 b- defN 22-Oct-25 02:49 tepe/core/trainer/__init__.py
--rw-rw-r--  2.0 unx      961 b- defN 22-Oct-25 02:49 tepe/core/trainer/cls_trainer.py
--rw-rw-r--  2.0 unx      740 b- defN 22-Oct-25 02:49 tepe/core/trainer/seg_trainer.py
--rw-rw-r--  2.0 unx       36 b- defN 22-Oct-25 02:49 tepe/data/__init__.py
--rw-rw-r--  2.0 unx    26406 b- defN 22-Oct-25 02:49 tepe/data/augmentations.py
--rw-rw-r--  2.0 unx     1552 b- defN 22-Oct-25 02:49 tepe/data/data_prefetcher.py
--rw-rw-r--  2.0 unx     5767 b- defN 22-Oct-25 02:49 tepe/data/dataloading.py
--rw-rw-r--  2.0 unx    10307 b- defN 22-Oct-28 02:06 tepe/data/infer_datasets.py
--rw-rw-r--  2.0 unx     2194 b- defN 22-Oct-25 02:49 tepe/data/utils.py
--rw-rw-r--  2.0 unx     8082 b- defN 22-Oct-25 02:49 tepe/data/voc_xml.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Nov-11 08:23 tepe/data/augments/__init__.py
--rw-rw-r--  2.0 unx     2229 b- defN 22-Oct-25 02:49 tepe/data/augments/paste_images.py
--rw-rw-r--  2.0 unx    20276 b- defN 22-Oct-25 02:49 tepe/data/augments/seg_augment.py
--rw-rw-r--  2.0 unx      163 b- defN 22-Oct-25 02:49 tepe/data/datasets/__init__.py
--rw-rw-r--  2.0 unx     4630 b- defN 22-Dec-26 11:18 tepe/data/datasets/ad_dataset.py
--rw-rw-r--  2.0 unx     6547 b- defN 22-Oct-25 02:49 tepe/data/datasets/cls_datasets.py
--rw-rw-r--  2.0 unx    14947 b- defN 22-Oct-25 02:49 tepe/data/datasets/keypoint_dataset.py
--rw-rw-r--  2.0 unx     1085 b- defN 22-Oct-25 02:49 tepe/data/datasets/public_class_names.py
--rw-rw-r--  2.0 unx     5399 b- defN 22-Oct-25 02:49 tepe/data/datasets/seg_voc_custom.py
--rw-rw-r--  2.0 unx     4044 b- defN 22-Oct-25 02:49 tepe/data/datasets/ssdrfb_voc.py
--rw-rw-r--  2.0 unx       21 b- defN 22-Oct-25 02:49 tepe/modules/__init__.py
--rw-rw-r--  2.0 unx      370 b- defN 22-Oct-25 02:49 tepe/modules/backbone/__init__.py
--rw-rw-r--  2.0 unx     5074 b- defN 22-Oct-25 02:49 tepe/modules/backbone/mobilenet_rfb.py
--rw-rw-r--  2.0 unx     7527 b- defN 22-Oct-25 02:49 tepe/modules/backbone/mobilenetv2.py
--rw-rw-r--  2.0 unx    15579 b- defN 22-Oct-25 02:49 tepe/modules/backbone/resnet.py
--rw-rw-r--  2.0 unx     5829 b- defN 22-Oct-25 02:49 tepe/modules/backbone/simplenet.py
--rw-rw-r--  2.0 unx     8282 b- defN 22-Oct-25 02:49 tepe/modules/backbone/vgg.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Oct-25 02:49 tepe/modules/neck/__init__.py
--rw-rw-r--  2.0 unx      484 b- defN 22-Oct-25 02:49 tepe/modules/optim/__init__.py
--rw-rw-r--  2.0 unx     9827 b- defN 22-Oct-25 02:49 tepe/modules/optim/adabelief.py
--rw-rw-r--  2.0 unx     7459 b- defN 22-Oct-25 02:49 tepe/modules/optim/adafactor.py
--rw-rw-r--  2.0 unx     6535 b- defN 22-Oct-25 02:49 tepe/modules/optim/adahessian.py
--rw-rw-r--  2.0 unx     3574 b- defN 22-Oct-25 02:49 tepe/modules/optim/adamp.py
--rw-rw-r--  2.0 unx     5147 b- defN 22-Oct-25 02:49 tepe/modules/optim/adamw.py
--rw-rw-r--  2.0 unx     9184 b- defN 22-Oct-25 02:49 tepe/modules/optim/lamb.py
--rw-rw-r--  2.0 unx     5255 b- defN 22-Oct-25 02:49 tepe/modules/optim/lars.py
--rw-rw-r--  2.0 unx     2463 b- defN 22-Oct-25 02:49 tepe/modules/optim/lookahead.py
--rw-rw-r--  2.0 unx     6893 b- defN 22-Oct-25 02:49 tepe/modules/optim/madgrad.py
--rw-rw-r--  2.0 unx     3871 b- defN 22-Oct-25 02:49 tepe/modules/optim/nadam.py
--rw-rw-r--  2.0 unx     4856 b- defN 22-Oct-25 02:49 tepe/modules/optim/nvnovograd.py
--rw-rw-r--  2.0 unx     8422 b- defN 22-Oct-25 02:49 tepe/modules/optim/optim_factory.py
--rw-rw-r--  2.0 unx     3468 b- defN 22-Oct-25 02:49 tepe/modules/optim/radam.py
--rw-rw-r--  2.0 unx     6143 b- defN 22-Oct-25 02:49 tepe/modules/optim/rmsprop_tf.py
--rw-rw-r--  2.0 unx     2296 b- defN 22-Oct-25 02:49 tepe/modules/optim/sgdp.py
--rw-rw-r--  2.0 unx      291 b- defN 22-Oct-25 02:49 tepe/modules/scheduler/__init__.py
--rw-rw-r--  2.0 unx     4161 b- defN 22-Oct-25 02:49 tepe/modules/scheduler/cosine_lr.py
--rw-rw-r--  2.0 unx     2084 b- defN 22-Dec-16 02:56 tepe/modules/scheduler/multistep_lr.py
--rw-rw-r--  2.0 unx     4140 b- defN 22-Oct-25 02:49 tepe/modules/scheduler/plateau_lr.py
--rw-rw-r--  2.0 unx     4003 b- defN 22-Oct-25 02:49 tepe/modules/scheduler/poly_lr.py
--rw-rw-r--  2.0 unx     4750 b- defN 22-Oct-25 02:49 tepe/modules/scheduler/scheduler.py
--rw-rw-r--  2.0 unx     3771 b- defN 22-Dec-23 06:14 tepe/modules/scheduler/scheduler_factory.py
--rw-rw-r--  2.0 unx     1902 b- defN 22-Oct-25 02:49 tepe/modules/scheduler/step_lr.py
--rw-rw-r--  2.0 unx     3936 b- defN 22-Oct-25 02:49 tepe/modules/scheduler/tanh_lr.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Oct-25 02:49 tepe/modules/utils/__init__.py
--rw-rw-r--  2.0 unx     2922 b- defN 22-Oct-25 02:49 tepe/modules/utils/layers.py
--rw-rw-r--  2.0 unx      721 b- defN 22-Oct-25 02:49 tepe/modules/utils/loss.py
--rw-rw-r--  2.0 unx     2616 b- defN 22-Oct-25 02:49 tepe/modules/utils/model_utils.py
--rw-rw-r--  2.0 unx     5052 b- defN 22-Oct-25 02:49 tepe/modules/utils/scheduler.py
--rw-rw-r--  2.0 unx      589 b- defN 22-Oct-25 02:49 tepe/tasks/__init__.py
--rw-rw-r--  2.0 unx      237 b- defN 22-Oct-25 02:49 tepe/tasks/cfa/__init__.py
--rw-rw-r--  2.0 unx     5849 b- defN 22-Oct-25 02:49 tepe/tasks/cfa/auto_encoder.py
--rw-rw-r--  2.0 unx     1358 b- defN 22-Oct-25 02:49 tepe/tasks/cfa/build_encoder.py
--rw-rw-r--  2.0 unx     8366 b- defN 22-Dec-08 07:25 tepe/tasks/cfa/module.py
--rw-rw-r--  2.0 unx     6448 b- defN 22-Oct-25 05:48 tepe/tasks/cfa/predictor.py
--rw-rw-r--  2.0 unx     8426 b- defN 22-Dec-08 07:25 tepe/tasks/cfa/task.py
--rw-rw-r--  2.0 unx     3507 b- defN 22-Oct-25 02:49 tepe/tasks/cfa/utils.py
--rw-rw-r--  2.0 unx       26 b- defN 22-Oct-25 02:49 tepe/tasks/rd/__init__.py
--rw-rw-r--  2.0 unx    16424 b- defN 22-Nov-10 10:24 tepe/tasks/rd/de_resnet.py
--rw-rw-r--  2.0 unx    10599 b- defN 23-Jan-04 08:52 tepe/tasks/rd/evalutor.py
--rw-rw-r--  2.0 unx     2651 b- defN 22-Dec-23 09:13 tepe/tasks/rd/find_thr.py
--rw-rw-r--  2.0 unx     2777 b- defN 22-Dec-22 09:56 tepe/tasks/rd/model.py
--rw-rw-r--  2.0 unx    10713 b- defN 23-Jan-10 07:14 tepe/tasks/rd/predictor.py
--rw-rw-r--  2.0 unx    22705 b- defN 22-Oct-25 02:49 tepe/tasks/rd/resnet.py
--rw-rw-r--  2.0 unx    12266 b- defN 22-Dec-23 03:40 tepe/tasks/rd/task copy.py
--rw-rw-r--  2.0 unx     9990 b- defN 23-Jan-04 08:51 tepe/tasks/rd/task.py
--rw-rw-r--  2.0 unx     2347 b- defN 22-Dec-08 08:18 tepe/tasks/rd/trainer.py
--rw-rw-r--  2.0 unx     3029 b- defN 22-Dec-21 03:50 tepe/tasks/rd/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/__init__.py
--rw-rw-r--  2.0 unx    14894 b- defN 22-Nov-08 10:25 tepe/tasks/yolox/task.py
--rw-rw-r--  2.0 unx     3043 b- defN 22-Nov-17 09:34 tepe/tasks/yolox/yolox_detector.py
--rw-rw-r--  2.0 unx      152 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/core/__init__.py
--rw-rw-r--  2.0 unx     4398 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/core/launch.py
--rw-rw-r--  2.0 unx     6807 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/core/trainer.py
--rw-rw-r--  2.0 unx      397 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/data/__init__.py
--rw-rw-r--  2.0 unx     7399 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/data/data_augment.py
--rw-rw-r--  2.0 unx     1649 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/data/data_prefetcher.py
--rw-rw-r--  2.0 unx     3671 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/data/dataloading.py
--rw-rw-r--  2.0 unx     2854 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/data/samplers.py
--rw-rw-r--  2.0 unx      311 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/data/datasets/__init__.py
--rw-rw-r--  2.0 unx     7415 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/data/datasets/coco.py
--rw-rw-r--  2.0 unx     1296 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/data/datasets/coco_classes.py
--rw-rw-r--  2.0 unx    14060 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/data/datasets/custom_voc.py
--rw-rw-r--  2.0 unx     3752 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/data/datasets/datasets_wrapper.py
--rw-rw-r--  2.0 unx     9569 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/data/datasets/mosaicdetection.py
--rw-rw-r--  2.0 unx    13521 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/data/datasets/voc.py
--rw-rw-r--  2.0 unx      442 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/data/datasets/voc_classes.py
--rw-rw-r--  2.0 unx      178 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/evaluators/__init__.py
--rw-rw-r--  2.0 unx     7237 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/evaluators/coco_evaluator.py
--rw-rw-r--  2.0 unx     5774 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/evaluators/voc_eval.py
--rw-rw-r--  2.0 unx     5661 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/evaluators/voc_evaluator.py
--rw-rw-r--  2.0 unx      151 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/layers/__init__.py
--rw-rw-r--  2.0 unx     5757 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/layers/fast_coco_eval_api.py
--rw-rw-r--  2.0 unx      297 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/models/__init__.py
--rw-rw-r--  2.0 unx     6028 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/models/darknet.py
--rw-rw-r--  2.0 unx     1687 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/models/losses.py
--rw-rw-r--  2.0 unx     6102 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/models/network_blocks.py
--rw-rw-r--  2.0 unx     2486 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/models/yolo_fpn.py
--rw-rw-r--  2.0 unx    23129 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/models/yolo_head.py
--rw-rw-r--  2.0 unx     3540 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/models/yolo_pafpn.py
--rw-rw-r--  2.0 unx     1374 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/models/yolox.py
--rw-rw-r--  2.0 unx      443 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/utils/__init__.py
--rw-rw-r--  2.0 unx     2845 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/utils/allreduce_norm.py
--rw-rw-r--  2.0 unx     4481 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/utils/boxes.py
--rw-rw-r--  2.0 unx     1322 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/utils/checkpoint.py
--rw-rw-r--  2.0 unx     3839 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/utils/demo_utils.py
--rw-rw-r--  2.0 unx     7826 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/utils/dist.py
--rw-rw-r--  2.0 unx     2083 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/utils/ema.py
--rw-rw-r--  2.0 unx     2750 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/utils/logger.py
--rw-rw-r--  2.0 unx     6561 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/utils/lr_scheduler.py
--rw-rw-r--  2.0 unx     3093 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/utils/metric.py
--rw-rw-r--  2.0 unx     3269 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/utils/model_utils.py
--rw-rw-r--  2.0 unx     2685 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/utils/setup_env.py
--rw-rw-r--  2.0 unx     3609 b- defN 22-Nov-08 10:16 tepe/tasks/yolox/utils/visualize.py
--rw-rw-r--  2.0 unx      191 b- defN 22-Oct-25 02:49 tepe/utils/__init__.py
--rw-rw-r--  2.0 unx     3112 b- defN 22-Oct-25 02:49 tepe/utils/autobatch.py
--rw-rw-r--  2.0 unx    10995 b- defN 22-Oct-25 02:49 tepe/utils/box_utils.py
--rw-rw-r--  2.0 unx     1183 b- defN 22-Oct-25 02:49 tepe/utils/coords_utils.py
--rw-rw-r--  2.0 unx    10309 b- defN 22-Dec-21 13:01 tepe/utils/dist.py
--rw-rw-r--  2.0 unx    29582 b- defN 22-Dec-25 02:40 tepe/utils/general.py
--rw-rw-r--  2.0 unx     3267 b- defN 22-Dec-21 06:48 tepe/utils/get_subimg.py
--rw-rw-r--  2.0 unx     2036 b- defN 22-Oct-25 02:49 tepe/utils/meter.py
--rw-rw-r--  2.0 unx    12451 b- defN 22-Oct-25 02:49 tepe/utils/plots.py
--rw-rw-r--  2.0 unx    12725 b- defN 22-Oct-25 02:49 tepe/utils/tensorrt_utils.py
--rw-rw-r--  2.0 unx    10692 b- defN 22-Nov-08 10:27 tepe/utils/torch_utils.py
--rw-rw-r--  2.0 unx     1074 b- defN 23-Jan-10 08:16 tepe-0.6.9.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4600 b- defN 23-Jan-10 08:16 tepe-0.6.9.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-10 08:16 tepe-0.6.9.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jan-10 08:16 tepe-0.6.9.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    14116 b- defN 23-Jan-10 08:16 tepe-0.6.9.5.dist-info/RECORD
-161 files, 812162 bytes uncompressed, 244976 bytes compressed:  69.8%
+Zip file size: 517919 bytes, number of entries: 299
+-rw-rw-r--  2.0 unx      297 b- defN 23-May-18 02:45 tepe/__init__.py
+-rw-rw-r--  2.0 unx      248 b- defN 23-May-18 02:08 tepe/core/__init__.py
+-rw-rw-r--  2.0 unx     4056 b- defN 23-May-18 02:08 tepe/core/base_evaluator.py
+-rw-rw-r--  2.0 unx     6698 b- defN 23-May-18 02:08 tepe/core/base_predictor.py
+-rw-rw-r--  2.0 unx     8882 b- defN 23-May-18 02:08 tepe/core/base_task.py
+-rw-rw-r--  2.0 unx    14810 b- defN 23-May-18 02:08 tepe/core/base_trainer.py
+-rw-rw-r--  2.0 unx    10143 b- defN 23-May-18 02:08 tepe/core/cli.py
+-rw-rw-r--  2.0 unx     5228 b- defN 23-May-18 02:08 tepe/core/exporter.py
+-rw-rw-r--  2.0 unx     4006 b- defN 23-May-18 02:08 tepe/core/register.py
+-rw-rw-r--  2.0 unx       79 b- defN 22-Aug-15 06:40 tepe/core/evaluator/__init__.py
+-rw-rw-r--  2.0 unx     1697 b- defN 22-Aug-15 06:40 tepe/core/evaluator/cls_evaluator.py
+-rw-rw-r--  2.0 unx     2194 b- defN 22-Aug-15 06:40 tepe/core/evaluator/seg_evaluator.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Aug-15 06:40 tepe/core/evaluator/metrics/__init__.py
+-rw-rw-r--  2.0 unx      627 b- defN 22-Aug-15 06:40 tepe/core/evaluator/metrics/cls_metrics.py
+-rw-rw-r--  2.0 unx     2117 b- defN 22-Aug-15 06:40 tepe/core/evaluator/metrics/seg_metrics.py
+-rw-rw-r--  2.0 unx     5820 b- defN 22-Aug-15 06:40 tepe/core/evaluator/metrics/voc_metrics.py
+-rw-rw-r--  2.0 unx      109 b- defN 22-Aug-15 06:46 tepe/core/predictor/__init__.py
+-rw-rw-r--  2.0 unx     1124 b- defN 23-May-18 02:08 tepe/core/predictor/anomaly_detector.py
+-rw-rw-r--  2.0 unx     3258 b- defN 22-Oct-24 09:59 tepe/core/predictor/classifier.py
+-rw-rw-r--  2.0 unx     2653 b- defN 23-May-18 02:08 tepe/core/predictor/segmentor.py
+-rw-rw-r--  2.0 unx       71 b- defN 22-Aug-15 06:40 tepe/core/trainer/__init__.py
+-rw-rw-r--  2.0 unx      961 b- defN 22-Aug-15 06:40 tepe/core/trainer/cls_trainer.py
+-rw-rw-r--  2.0 unx      740 b- defN 22-Aug-15 06:40 tepe/core/trainer/seg_trainer.py
+-rw-rw-r--  2.0 unx       36 b- defN 22-Oct-24 09:59 tepe/data/__init__.py
+-rw-rw-r--  2.0 unx    26406 b- defN 22-Oct-24 09:59 tepe/data/augmentations.py
+-rw-rw-r--  2.0 unx     1552 b- defN 22-Aug-15 06:40 tepe/data/data_prefetcher.py
+-rw-rw-r--  2.0 unx     5767 b- defN 22-Aug-15 06:40 tepe/data/dataloading.py
+-rw-rw-r--  2.0 unx     7569 b- defN 23-May-18 02:08 tepe/data/infer_datasets.py
+-rw-rw-r--  2.0 unx     2194 b- defN 22-Aug-15 06:40 tepe/data/utils.py
+-rw-rw-r--  2.0 unx      220 b- defN 23-May-18 02:08 tepe/data/annotation/__init__.py
+-rw-rw-r--  2.0 unx     4763 b- defN 23-May-18 02:08 tepe/data/annotation/labelme_json.py
+-rw-rw-r--  2.0 unx     8082 b- defN 23-May-18 02:08 tepe/data/annotation/voc_xml.py
+-rw-rw-r--  2.0 unx       36 b- defN 23-May-18 02:08 tepe/data/augments/__init__.py
+-rw-rw-r--  2.0 unx     2229 b- defN 22-Sep-22 12:53 tepe/data/augments/paste_images.py
+-rw-rw-r--  2.0 unx    20305 b- defN 23-May-18 02:08 tepe/data/augments/seg_augment.py
+-rw-rw-r--  2.0 unx      201 b- defN 23-May-18 02:08 tepe/data/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3690 b- defN 23-May-18 02:08 tepe/data/datasets/ad_dataset.py
+-rw-rw-r--  2.0 unx     6547 b- defN 22-Oct-24 09:59 tepe/data/datasets/cls_datasets.py
+-rw-rw-r--  2.0 unx    13485 b- defN 23-May-18 02:08 tepe/data/datasets/keypoint_dataset.py
+-rw-rw-r--  2.0 unx     9086 b- defN 23-May-18 02:08 tepe/data/datasets/line_dataset.py
+-rw-rw-r--  2.0 unx     1085 b- defN 22-Aug-15 06:46 tepe/data/datasets/public_class_names.py
+-rw-rw-r--  2.0 unx     5834 b- defN 23-May-18 02:08 tepe/data/datasets/seg_voc_custom.py
+-rw-rw-r--  2.0 unx     4044 b- defN 22-Aug-15 06:40 tepe/data/datasets/ssdrfb_voc.py
+-rw-rw-r--  2.0 unx       32 b- defN 23-May-18 02:08 tepe/modules/__init__.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-May-18 02:08 tepe/modules/activation.py
+-rw-rw-r--  2.0 unx     1389 b- defN 23-May-18 02:08 tepe/modules/init_weights.py
+-rw-rw-r--  2.0 unx     2939 b- defN 23-May-18 02:08 tepe/modules/layers.py
+-rw-rw-r--  2.0 unx      721 b- defN 23-May-18 02:08 tepe/modules/loss.py
+-rw-rw-r--  2.0 unx     2616 b- defN 23-May-18 02:08 tepe/modules/model_utils.py
+-rw-rw-r--  2.0 unx      410 b- defN 23-May-18 02:08 tepe/modules/model_zoo.py
+-rw-rw-r--  2.0 unx      409 b- defN 23-May-18 02:08 tepe/modules/backbone/__init__.py
+-rw-rw-r--  2.0 unx     5079 b- defN 23-May-18 02:08 tepe/modules/backbone/mobilenet_rfb.py
+-rw-rw-r--  2.0 unx     7527 b- defN 22-Aug-15 06:40 tepe/modules/backbone/mobilenetv2.py
+-rw-rw-r--  2.0 unx    15579 b- defN 22-Sep-22 12:53 tepe/modules/backbone/resnet.py
+-rw-rw-r--  2.0 unx     7123 b- defN 23-May-18 02:08 tepe/modules/backbone/shufflenetv2.py
+-rw-rw-r--  2.0 unx     5829 b- defN 22-Aug-15 06:40 tepe/modules/backbone/simplenet.py
+-rw-rw-r--  2.0 unx     8282 b- defN 22-Sep-22 12:53 tepe/modules/backbone/vgg.py
+-rw-rw-r--  2.0 unx       42 b- defN 23-May-18 02:08 tepe/modules/neck/__init__.py
+-rw-rw-r--  2.0 unx     3046 b- defN 23-May-18 02:08 tepe/modules/neck/fpn.py
+-rw-rw-r--  2.0 unx     3075 b- defN 23-May-18 02:08 tepe/modules/neck/pan.py
+-rw-rw-r--  2.0 unx      484 b- defN 22-Aug-15 06:40 tepe/modules/optim/__init__.py
+-rw-rw-r--  2.0 unx     9827 b- defN 22-Aug-15 06:40 tepe/modules/optim/adabelief.py
+-rw-rw-r--  2.0 unx     7459 b- defN 22-Aug-15 06:40 tepe/modules/optim/adafactor.py
+-rw-rw-r--  2.0 unx     6535 b- defN 22-Aug-15 06:40 tepe/modules/optim/adahessian.py
+-rw-rw-r--  2.0 unx     3574 b- defN 22-Aug-15 06:40 tepe/modules/optim/adamp.py
+-rw-rw-r--  2.0 unx     5147 b- defN 22-Aug-15 06:40 tepe/modules/optim/adamw.py
+-rw-rw-r--  2.0 unx     9184 b- defN 22-Aug-15 06:40 tepe/modules/optim/lamb.py
+-rw-rw-r--  2.0 unx     5255 b- defN 22-Aug-15 06:40 tepe/modules/optim/lars.py
+-rw-rw-r--  2.0 unx     2463 b- defN 22-Aug-15 06:40 tepe/modules/optim/lookahead.py
+-rw-rw-r--  2.0 unx     6893 b- defN 22-Aug-15 06:40 tepe/modules/optim/madgrad.py
+-rw-rw-r--  2.0 unx     3871 b- defN 22-Aug-15 06:40 tepe/modules/optim/nadam.py
+-rw-rw-r--  2.0 unx     4856 b- defN 22-Aug-15 06:40 tepe/modules/optim/nvnovograd.py
+-rw-rw-r--  2.0 unx     8422 b- defN 22-Aug-15 06:40 tepe/modules/optim/optim_factory.py
+-rw-rw-r--  2.0 unx     3468 b- defN 22-Aug-15 06:40 tepe/modules/optim/radam.py
+-rw-rw-r--  2.0 unx     6143 b- defN 22-Aug-15 06:40 tepe/modules/optim/rmsprop_tf.py
+-rw-rw-r--  2.0 unx     2296 b- defN 22-Aug-15 06:40 tepe/modules/optim/sgdp.py
+-rw-rw-r--  2.0 unx      324 b- defN 23-May-18 02:08 tepe/modules/scheduler/__init__.py
+-rw-rw-r--  2.0 unx     3943 b- defN 23-May-18 02:08 tepe/modules/scheduler/cosine_lr.py
+-rw-rw-r--  2.0 unx     1896 b- defN 23-May-18 02:08 tepe/modules/scheduler/multistep_lr.py
+-rw-rw-r--  2.0 unx     3573 b- defN 23-May-18 02:08 tepe/modules/scheduler/plateau_lr.py
+-rw-rw-r--  2.0 unx     3627 b- defN 23-May-18 02:08 tepe/modules/scheduler/poly_lr.py
+-rw-rw-r--  2.0 unx     5408 b- defN 23-May-18 02:08 tepe/modules/scheduler/scheduler.py
+-rw-rw-r--  2.0 unx     3771 b- defN 23-May-18 02:08 tepe/modules/scheduler/scheduler_factory.py
+-rw-rw-r--  2.0 unx     2144 b- defN 23-May-18 02:08 tepe/modules/scheduler/step_lr.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-May-18 02:08 tepe/modules/scheduler/tanh_lr.py
+-rw-rw-r--  2.0 unx      589 b- defN 22-Sep-22 12:53 tepe/tasks/__init__.py
+-rw-rw-r--  2.0 unx      778 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/README.txt
+-rw-rw-r--  2.0 unx       36 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/__init__.py
+-rw-rw-r--  2.0 unx    14051 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/all_config.py
+-rw-rw-r--  2.0 unx     1883 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/builder.py
+-rw-rw-r--  2.0 unx     7610 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/inference.py
+-rw-rw-r--  2.0 unx     2175 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/task.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/__init__.py
+-rw-rw-r--  2.0 unx    17977 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/attention_rpn_detector.py
+-rw-rw-r--  2.0 unx    14711 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/query_support_detector.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/backbone/__init__.py
+-rw-rw-r--  2.0 unx    23764 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/backbone/resnet.py
+-rw-rw-r--  2.0 unx       48 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/dense_heads/__init__.py
+-rw-rw-r--  2.0 unx    13047 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/dense_heads/attention_rpn_head.py
+-rw-rw-r--  2.0 unx      157 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/roi_extractors/__init__.py
+-rw-rw-r--  2.0 unx     3002 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/roi_extractors/base_roi_extractor.py
+-rw-rw-r--  2.0 unx     4790 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/roi_extractors/single_level_roi_extractor.py
+-rw-rw-r--  2.0 unx      152 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/roi_heads/__init__.py
+-rw-rw-r--  2.0 unx     3220 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/roi_heads/base_roi_head.py
+-rw-rw-r--  2.0 unx    15519 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/roi_heads/multi_relation_roi_head.py
+-rw-rw-r--  2.0 unx    17123 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/roi_heads/standard_roi_head.py
+-rw-rw-r--  2.0 unx    13557 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/roi_heads/test_mixins.py
+-rw-rw-r--  2.0 unx      108 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/roi_heads/bbox_heads/__init__.py
+-rw-rw-r--  2.0 unx    11398 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/roi_heads/bbox_heads/multi_relation_bbox_head.py
+-rw-rw-r--  2.0 unx       31 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/roi_heads/shared_head/__init__.py
+-rw-rw-r--  2.0 unx     2509 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/model/roi_heads/shared_head/res_layer.py
+-rw-rw-r--  2.0 unx      599 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/pipelines/__init__.py
+-rw-rw-r--  2.0 unx     1884 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/pipelines/formatting.py
+-rw-rw-r--  2.0 unx    16954 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/pipelines/transforms.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/utils/__init__.py
+-rw-rw-r--  2.0 unx     8459 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/utils/aggregation_layer.py
+-rw-rw-r--  2.0 unx    12778 b- defN 23-May-18 02:08 tepe/tasks/attention_rpn/utils/checkpoint.py
+-rw-rw-r--  2.0 unx      237 b- defN 22-Oct-24 09:59 tepe/tasks/cfa/__init__.py
+-rw-rw-r--  2.0 unx     5849 b- defN 22-Oct-24 09:59 tepe/tasks/cfa/auto_encoder.py
+-rw-rw-r--  2.0 unx     1358 b- defN 22-Oct-24 09:59 tepe/tasks/cfa/build_encoder.py
+-rw-rw-r--  2.0 unx     8361 b- defN 22-Oct-24 09:59 tepe/tasks/cfa/module.py
+-rw-rw-r--  2.0 unx     6448 b- defN 22-Oct-24 09:59 tepe/tasks/cfa/predictor.py
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-18 02:08 tepe/tasks/cfa/requirements.txt
+-rw-rw-r--  2.0 unx     8399 b- defN 23-May-18 02:08 tepe/tasks/cfa/task.py
+-rw-rw-r--  2.0 unx     3507 b- defN 22-Oct-24 09:59 tepe/tasks/cfa/utils.py
+-rw-rw-r--  2.0 unx       33 b- defN 23-May-18 02:08 tepe/tasks/deeplabv3/__init__.py
+-rw-rw-r--  2.0 unx     5827 b- defN 23-May-18 02:08 tepe/tasks/deeplabv3/create_model.py
+-rw-rw-r--  2.0 unx    10816 b- defN 23-May-18 02:08 tepe/tasks/deeplabv3/deeplab.py
+-rw-rw-r--  2.0 unx     8256 b- defN 23-May-18 02:08 tepe/tasks/deeplabv3/task.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-May-18 02:08 tepe/tasks/deeplabv3/utils.py
+-rw-rw-r--  2.0 unx       35 b- defN 23-May-18 02:08 tepe/tasks/mobilenetv2/__init__.py
+-rw-rw-r--  2.0 unx     2270 b- defN 23-May-18 02:08 tepe/tasks/mobilenetv2/task.py
+-rw-rw-r--  2.0 unx       60 b- defN 23-May-18 02:08 tepe/tasks/nanodet/__init__.py
+-rw-rw-r--  2.0 unx     5226 b- defN 23-May-18 02:08 tepe/tasks/nanodet/evaluator.py
+-rw-rw-r--  2.0 unx     2021 b- defN 23-May-18 02:08 tepe/tasks/nanodet/predictor.py
+-rw-rw-r--  2.0 unx       28 b- defN 23-May-18 02:08 tepe/tasks/nanodet/requirements.txt
+-rw-rw-r--  2.0 unx    12481 b- defN 23-May-18 02:08 tepe/tasks/nanodet/task.py
+-rw-rw-r--  2.0 unx    13502 b- defN 23-May-18 02:08 tepe/tasks/nanodet/trainer.py
+-rw-rw-r--  2.0 unx     1129 b- defN 23-May-18 02:08 tepe/tasks/nanodet/util/__init__.py
+-rw-rw-r--  2.0 unx     1670 b- defN 23-May-18 02:08 tepe/tasks/nanodet/util/box_transform.py
+-rw-rw-r--  2.0 unx     3842 b- defN 23-May-18 02:08 tepe/tasks/nanodet/util/check_point.py
+-rw-rw-r--  2.0 unx      900 b- defN 23-May-18 02:08 tepe/tasks/nanodet/util/config.py
+-rw-rw-r--  2.0 unx    20956 b- defN 23-May-18 02:08 tepe/tasks/nanodet/util/flops_counter.py
+-rw-rw-r--  2.0 unx     7168 b- defN 23-May-18 02:08 tepe/tasks/nanodet/util/logger.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-May-18 02:08 tepe/tasks/nanodet/util/misc.py
+-rw-rw-r--  2.0 unx     1062 b- defN 23-May-18 02:08 tepe/tasks/nanodet/util/path.py
+-rw-rw-r--  2.0 unx      774 b- defN 23-May-18 02:08 tepe/tasks/nanodet/util/rank_filter.py
+-rw-rw-r--  2.0 unx     3500 b- defN 23-May-18 02:08 tepe/tasks/nanodet/util/scatter_gather.py
+-rw-rw-r--  2.0 unx     3685 b- defN 23-May-18 02:08 tepe/tasks/nanodet/util/util_mixins.py
+-rw-rw-r--  2.0 unx    21880 b- defN 23-May-18 02:08 tepe/tasks/nanodet/util/visualization.py
+-rw-rw-r--  2.0 unx    19589 b- defN 23-May-18 02:08 tepe/tasks/nanodet/util/yacs.py
+-rw-rw-r--  2.0 unx       26 b- defN 22-Oct-24 09:59 tepe/tasks/rd/__init__.py
+-rw-rw-r--  2.0 unx    16409 b- defN 22-Sep-22 12:53 tepe/tasks/rd/de_resnet.py
+-rw-rw-r--  2.0 unx     2329 b- defN 23-May-18 02:08 tepe/tasks/rd/evalutor.py
+-rw-rw-r--  2.0 unx     1665 b- defN 22-Oct-24 09:59 tepe/tasks/rd/find_thr.py
+-rw-rw-r--  2.0 unx     2353 b- defN 22-Oct-24 09:59 tepe/tasks/rd/model.py
+-rw-rw-r--  2.0 unx     5854 b- defN 23-May-18 02:08 tepe/tasks/rd/predictor.py
+-rw-rw-r--  2.0 unx    22705 b- defN 22-Sep-22 12:53 tepe/tasks/rd/resnet.py
+-rw-rw-r--  2.0 unx     9234 b- defN 23-May-18 02:08 tepe/tasks/rd/task.py
+-rw-rw-r--  2.0 unx       30 b- defN 23-May-18 02:08 tepe/tasks/resnet/__init__.py
+-rw-rw-r--  2.0 unx    10925 b- defN 23-May-18 02:08 tepe/tasks/resnet/task.py
+-rw-rw-r--  2.0 unx       35 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_heatmap/__init__.py
+-rw-rw-r--  2.0 unx     2161 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_heatmap/evaluator.py
+-rw-rw-r--  2.0 unx     5485 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_heatmap/predictor.py
+-rw-rw-r--  2.0 unx     9209 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_heatmap/task.py
+-rw-rw-r--  2.0 unx      379 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_heatmap/trainer.py
+-rw-rw-r--  2.0 unx     3044 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_heatmap/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_heatmap/models/__init__.py
+-rw-rw-r--  2.0 unx     8530 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_heatmap/models/v1.py
+-rw-rw-r--  2.0 unx     6848 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_heatmap/models/v2.py
+-rw-rw-r--  2.0 unx       32 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_line/__init__.py
+-rw-rw-r--  2.0 unx     1981 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_line/evaluator.py
+-rw-rw-r--  2.0 unx     5423 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_line/model.py
+-rw-rw-r--  2.0 unx     5077 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_line/predictor.py
+-rw-rw-r--  2.0 unx     7883 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_line/task.py
+-rw-rw-r--  2.0 unx      262 b- defN 23-May-18 02:08 tepe/tasks/shufflenet_line/trainer.py
+-rw-rw-r--  2.0 unx       33 b- defN 23-May-18 02:08 tepe/tasks/simplenet/__init__.py
+-rw-rw-r--  2.0 unx      759 b- defN 23-May-18 02:08 tepe/tasks/simplenet/classifier.py
+-rw-rw-r--  2.0 unx     5723 b- defN 23-May-18 02:08 tepe/tasks/simplenet/task.py
+-rw-rw-r--  2.0 unx       34 b- defN 23-May-18 02:08 tepe/tasks/ssdlite_rfb/__init__.py
+-rw-rw-r--  2.0 unx    10978 b- defN 23-May-18 02:08 tepe/tasks/ssdlite_rfb/anchor.py
+-rw-rw-r--  2.0 unx    19949 b- defN 23-May-18 02:08 tepe/tasks/ssdlite_rfb/augmentation.py
+-rw-rw-r--  2.0 unx     5248 b- defN 23-May-18 02:08 tepe/tasks/ssdlite_rfb/backbone.py
+-rw-rw-r--  2.0 unx     9941 b- defN 23-May-18 02:08 tepe/tasks/ssdlite_rfb/box_utils.py
+-rw-rw-r--  2.0 unx     2380 b- defN 23-May-18 02:08 tepe/tasks/ssdlite_rfb/creat_model.py
+-rw-rw-r--  2.0 unx     2024 b- defN 23-May-18 02:08 tepe/tasks/ssdlite_rfb/loss.py
+-rw-rw-r--  2.0 unx     6798 b- defN 23-May-18 02:08 tepe/tasks/ssdlite_rfb/ssd.py
+-rw-rw-r--  2.0 unx    14989 b- defN 23-May-18 02:08 tepe/tasks/ssdlite_rfb/task.py
+-rw-rw-r--  2.0 unx      947 b- defN 23-May-18 02:08 tepe/tasks/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     3777 b- defN 23-May-18 02:08 tepe/tasks/yolov5/activations.py
+-rw-rw-r--  2.0 unx    23497 b- defN 23-May-18 02:08 tepe/tasks/yolov5/common.py
+-rw-rw-r--  2.0 unx    46476 b- defN 23-May-18 02:08 tepe/tasks/yolov5/datasets.py
+-rw-rw-r--  2.0 unx     4509 b- defN 23-May-18 02:08 tepe/tasks/yolov5/experimental.py
+-rw-rw-r--  2.0 unx     9772 b- defN 23-May-18 02:08 tepe/tasks/yolov5/loss.py
+-rw-rw-r--  2.0 unx    13622 b- defN 23-May-18 02:08 tepe/tasks/yolov5/task.py
+-rw-rw-r--  2.0 unx    15031 b- defN 23-May-18 02:08 tepe/tasks/yolov5/yolo.py
+-rw-rw-r--  2.0 unx     6740 b- defN 23-May-18 02:08 tepe/tasks/yolov5/yolov5_detector.py
+-rw-rw-r--  2.0 unx     7728 b- defN 23-May-18 02:08 tepe/tasks/yolov5/yolov5_evaluator.py
+-rw-rw-r--  2.0 unx    14574 b- defN 23-May-18 02:08 tepe/tasks/yolov5/yolov5_trainer.py
+-rw-rw-r--  2.0 unx     1401 b- defN 23-May-18 02:08 tepe/tasks/yolov5/yolov5l.yaml
+-rw-rw-r--  2.0 unx     1403 b- defN 23-May-18 02:08 tepe/tasks/yolov5/yolov5m.yaml
+-rw-rw-r--  2.0 unx     1595 b- defN 23-May-18 02:08 tepe/tasks/yolov5/yolov5m2.yaml
+-rw-rw-r--  2.0 unx     1403 b- defN 23-May-18 02:08 tepe/tasks/yolov5/yolov5n.yaml
+-rw-rw-r--  2.0 unx     1403 b- defN 23-May-18 02:08 tepe/tasks/yolov5/yolov5s.yaml
+-rw-rw-r--  2.0 unx     1403 b- defN 23-May-18 02:08 tepe/tasks/yolov5/yolov5x.yaml
+-rw-rw-r--  2.0 unx     3335 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/anchors.yaml
+-rw-rw-r--  2.0 unx     1567 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov3-spp.yaml
+-rw-rw-r--  2.0 unx     1232 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov3-tiny.yaml
+-rw-rw-r--  2.0 unx     1560 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov3.yaml
+-rw-rw-r--  2.0 unx     1423 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov5-bifpn.yaml
+-rw-rw-r--  2.0 unx     1214 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov5-fpn.yaml
+-rw-rw-r--  2.0 unx     1658 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov5-p2.yaml
+-rw-rw-r--  2.0 unx     1704 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov5-p6.yaml
+-rw-rw-r--  2.0 unx     2076 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov5-p7.yaml
+-rw-rw-r--  2.0 unx     1407 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov5-panet.yaml
+-rw-rw-r--  2.0 unx     1820 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov5l6.yaml
+-rw-rw-r--  2.0 unx     1822 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov5m6.yaml
+-rw-rw-r--  2.0 unx     1822 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov5n6.yaml
+-rw-rw-r--  2.0 unx     1483 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov5s-ghost.yaml
+-rw-rw-r--  2.0 unx     1441 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov5s-transformer.yaml
+-rw-rw-r--  2.0 unx     1822 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov5s6.yaml
+-rw-rw-r--  2.0 unx     1822 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hub/yolov5x6.yaml
+-rw-rw-r--  2.0 unx      907 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hyps/hyp.finetune.yaml
+-rw-rw-r--  2.0 unx      460 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hyps/hyp.finetune_objects365.yaml
+-rw-rw-r--  2.0 unx     1683 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hyps/hyp.scratch-high.yaml
+-rw-rw-r--  2.0 unx     1691 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hyps/hyp.scratch-low.yaml
+-rw-rw-r--  2.0 unx     1685 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hyps/hyp.scratch-med.yaml
+-rw-rw-r--  2.0 unx     1663 b- defN 23-May-18 02:08 tepe/tasks/yolov5/hyps/hyp.scratch.yaml
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-18 02:08 tepe/tasks/yolov5/utils/__init__.py
+-rw-rw-r--  2.0 unx    11750 b- defN 23-May-18 02:08 tepe/tasks/yolov5/utils/augmentations.py
+-rw-rw-r--  2.0 unx     7070 b- defN 23-May-18 02:08 tepe/tasks/yolov5/utils/autoanchor.py
+-rw-rw-r--  2.0 unx     2248 b- defN 23-May-18 02:08 tepe/tasks/yolov5/utils/callbacks.py
+-rw-rw-r--  2.0 unx    26752 b- defN 23-May-18 02:08 tepe/tasks/yolov5/utils/general.py
+-rw-rw-r--  2.0 unx    15435 b- defN 23-May-18 02:08 tepe/tasks/yolov5/utils/metrics.py
+-rw-rw-r--  2.0 unx    19253 b- defN 23-May-18 02:08 tepe/tasks/yolov5/utils/plots.py
+-rw-rw-r--  2.0 unx     4595 b- defN 23-May-18 02:08 tepe/tasks/yolov5/utils/torch_utils.py
+-rw-rw-r--  2.0 unx       29 b- defN 23-May-18 02:08 tepe/tasks/yolox/__init__.py
+-rw-rw-r--  2.0 unx    14809 b- defN 23-May-18 02:08 tepe/tasks/yolox/task.py
+-rw-rw-r--  2.0 unx     2971 b- defN 23-May-18 02:08 tepe/tasks/yolox/yolox_detector.py
+-rw-rw-r--  2.0 unx      152 b- defN 23-May-18 02:08 tepe/tasks/yolox/core/__init__.py
+-rw-rw-r--  2.0 unx     4398 b- defN 23-May-18 02:08 tepe/tasks/yolox/core/launch.py
+-rw-rw-r--  2.0 unx     6807 b- defN 23-May-18 02:08 tepe/tasks/yolox/core/trainer.py
+-rw-rw-r--  2.0 unx      397 b- defN 23-May-18 02:08 tepe/tasks/yolox/data/__init__.py
+-rw-rw-r--  2.0 unx     7399 b- defN 23-May-18 02:08 tepe/tasks/yolox/data/data_augment.py
+-rw-rw-r--  2.0 unx     1649 b- defN 23-May-18 02:08 tepe/tasks/yolox/data/data_prefetcher.py
+-rw-rw-r--  2.0 unx     3671 b- defN 23-May-18 02:08 tepe/tasks/yolox/data/dataloading.py
+-rw-rw-r--  2.0 unx     2854 b- defN 23-May-18 02:08 tepe/tasks/yolox/data/samplers.py
+-rw-rw-r--  2.0 unx      311 b- defN 23-May-18 02:08 tepe/tasks/yolox/data/datasets/__init__.py
+-rw-rw-r--  2.0 unx     7415 b- defN 23-May-18 02:08 tepe/tasks/yolox/data/datasets/coco.py
+-rw-rw-r--  2.0 unx     1296 b- defN 23-May-18 02:08 tepe/tasks/yolox/data/datasets/coco_classes.py
+-rw-rw-r--  2.0 unx    14060 b- defN 23-May-18 02:08 tepe/tasks/yolox/data/datasets/custom_voc.py
+-rw-rw-r--  2.0 unx     3752 b- defN 23-May-18 02:08 tepe/tasks/yolox/data/datasets/datasets_wrapper.py
+-rw-rw-r--  2.0 unx     9569 b- defN 23-May-18 02:08 tepe/tasks/yolox/data/datasets/mosaicdetection.py
+-rw-rw-r--  2.0 unx    13521 b- defN 23-May-18 02:08 tepe/tasks/yolox/data/datasets/voc.py
+-rw-rw-r--  2.0 unx      442 b- defN 23-May-18 02:08 tepe/tasks/yolox/data/datasets/voc_classes.py
+-rw-rw-r--  2.0 unx      178 b- defN 23-May-18 02:08 tepe/tasks/yolox/evaluators/__init__.py
+-rw-rw-r--  2.0 unx     7237 b- defN 23-May-18 02:08 tepe/tasks/yolox/evaluators/coco_evaluator.py
+-rw-rw-r--  2.0 unx     5774 b- defN 23-May-18 02:08 tepe/tasks/yolox/evaluators/voc_eval.py
+-rw-rw-r--  2.0 unx     5661 b- defN 23-May-18 02:08 tepe/tasks/yolox/evaluators/voc_evaluator.py
+-rw-rw-r--  2.0 unx      151 b- defN 23-May-18 02:08 tepe/tasks/yolox/layers/__init__.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-May-18 02:08 tepe/tasks/yolox/layers/fast_coco_eval_api.py
+-rw-rw-r--  2.0 unx      297 b- defN 23-May-18 02:08 tepe/tasks/yolox/models/__init__.py
+-rw-rw-r--  2.0 unx     6028 b- defN 23-May-18 02:08 tepe/tasks/yolox/models/darknet.py
+-rw-rw-r--  2.0 unx     1687 b- defN 23-May-18 02:08 tepe/tasks/yolox/models/losses.py
+-rw-rw-r--  2.0 unx     6102 b- defN 23-May-18 02:08 tepe/tasks/yolox/models/network_blocks.py
+-rw-rw-r--  2.0 unx     2486 b- defN 23-May-18 02:08 tepe/tasks/yolox/models/yolo_fpn.py
+-rw-rw-r--  2.0 unx    23129 b- defN 23-May-18 02:08 tepe/tasks/yolox/models/yolo_head.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-May-18 02:08 tepe/tasks/yolox/models/yolo_pafpn.py
+-rw-rw-r--  2.0 unx     1374 b- defN 23-May-18 02:08 tepe/tasks/yolox/models/yolox.py
+-rw-rw-r--  2.0 unx      443 b- defN 23-May-18 02:08 tepe/tasks/yolox/utils/__init__.py
+-rw-rw-r--  2.0 unx     2845 b- defN 23-May-18 02:08 tepe/tasks/yolox/utils/allreduce_norm.py
+-rw-rw-r--  2.0 unx     4481 b- defN 23-May-18 02:08 tepe/tasks/yolox/utils/boxes.py
+-rw-rw-r--  2.0 unx     1322 b- defN 23-May-18 02:08 tepe/tasks/yolox/utils/checkpoint.py
+-rw-rw-r--  2.0 unx     3839 b- defN 23-May-18 02:08 tepe/tasks/yolox/utils/demo_utils.py
+-rw-rw-r--  2.0 unx     7826 b- defN 23-May-18 02:08 tepe/tasks/yolox/utils/dist.py
+-rw-rw-r--  2.0 unx     2083 b- defN 23-May-18 02:08 tepe/tasks/yolox/utils/ema.py
+-rw-rw-r--  2.0 unx     2750 b- defN 23-May-18 02:08 tepe/tasks/yolox/utils/logger.py
+-rw-rw-r--  2.0 unx     6561 b- defN 23-May-18 02:08 tepe/tasks/yolox/utils/lr_scheduler.py
+-rw-rw-r--  2.0 unx     3093 b- defN 23-May-18 02:08 tepe/tasks/yolox/utils/metric.py
+-rw-rw-r--  2.0 unx     3269 b- defN 23-May-18 02:08 tepe/tasks/yolox/utils/model_utils.py
+-rw-rw-r--  2.0 unx     2685 b- defN 23-May-18 02:08 tepe/tasks/yolox/utils/setup_env.py
+-rw-rw-r--  2.0 unx     3609 b- defN 23-May-18 02:08 tepe/tasks/yolox/utils/visualize.py
+-rw-rw-r--  2.0 unx      296 b- defN 23-May-18 02:08 tepe/utils/__init__.py
+-rw-rw-r--  2.0 unx     3112 b- defN 22-Oct-24 09:59 tepe/utils/autobatch.py
+-rw-rw-r--  2.0 unx    10995 b- defN 22-Aug-15 06:40 tepe/utils/box_utils.py
+-rw-rw-r--  2.0 unx     1183 b- defN 22-Aug-15 06:40 tepe/utils/coords_utils.py
+-rw-rw-r--  2.0 unx     7826 b- defN 22-Aug-15 06:40 tepe/utils/dist.py
+-rw-rw-r--  2.0 unx    33202 b- defN 23-May-18 02:08 tepe/utils/general.py
+-rw-rw-r--  2.0 unx     2279 b- defN 23-May-18 02:08 tepe/utils/meter.py
+-rw-rw-r--  2.0 unx     2616 b- defN 23-May-18 02:08 tepe/utils/model_utils.py
+-rw-rw-r--  2.0 unx    12451 b- defN 22-Aug-15 06:40 tepe/utils/plots.py
+-rw-rw-r--  2.0 unx    12725 b- defN 22-Aug-15 06:40 tepe/utils/tensorrt_utils.py
+-rw-rw-r--  2.0 unx    10692 b- defN 23-May-18 02:08 tepe/utils/torch_utils.py
+-rw-rw-r--  2.0 unx     1074 b- defN 23-May-18 02:45 tepe-0.7.5.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4578 b- defN 23-May-18 02:45 tepe-0.7.5.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-18 02:45 tepe-0.7.5.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       45 b- defN 23-May-18 02:45 tepe-0.7.5.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 unx        5 b- defN 23-May-18 02:45 tepe-0.7.5.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    27295 b- defN 23-May-18 02:45 tepe-0.7.5.2.dist-info/RECORD
+299 files, 1596790 bytes uncompressed, 474443 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -12,18 +12,18 @@
 
 Filename: tepe/core/base_task.py
 Comment: 
 
 Filename: tepe/core/base_trainer.py
 Comment: 
 
-Filename: tepe/core/exporter.py
+Filename: tepe/core/cli.py
 Comment: 
 
-Filename: tepe/core/launch.py
+Filename: tepe/core/exporter.py
 Comment: 
 
 Filename: tepe/core/register.py
 Comment: 
 
 Filename: tepe/core/evaluator/__init__.py
 Comment: 
@@ -54,20 +54,14 @@
 
 Filename: tepe/core/predictor/classifier.py
 Comment: 
 
 Filename: tepe/core/predictor/segmentor.py
 Comment: 
 
-Filename: tepe/core/task_config/__init__.py
-Comment: 
-
-Filename: tepe/core/task_config/anomaly_detection_task.py
-Comment: 
-
 Filename: tepe/core/trainer/__init__.py
 Comment: 
 
 Filename: tepe/core/trainer/cls_trainer.py
 Comment: 
 
 Filename: tepe/core/trainer/seg_trainer.py
@@ -87,15 +81,21 @@
 
 Filename: tepe/data/infer_datasets.py
 Comment: 
 
 Filename: tepe/data/utils.py
 Comment: 
 
-Filename: tepe/data/voc_xml.py
+Filename: tepe/data/annotation/__init__.py
+Comment: 
+
+Filename: tepe/data/annotation/labelme_json.py
+Comment: 
+
+Filename: tepe/data/annotation/voc_xml.py
 Comment: 
 
 Filename: tepe/data/augments/__init__.py
 Comment: 
 
 Filename: tepe/data/augments/paste_images.py
 Comment: 
@@ -111,47 +111,77 @@
 
 Filename: tepe/data/datasets/cls_datasets.py
 Comment: 
 
 Filename: tepe/data/datasets/keypoint_dataset.py
 Comment: 
 
+Filename: tepe/data/datasets/line_dataset.py
+Comment: 
+
 Filename: tepe/data/datasets/public_class_names.py
 Comment: 
 
 Filename: tepe/data/datasets/seg_voc_custom.py
 Comment: 
 
 Filename: tepe/data/datasets/ssdrfb_voc.py
 Comment: 
 
 Filename: tepe/modules/__init__.py
 Comment: 
 
+Filename: tepe/modules/activation.py
+Comment: 
+
+Filename: tepe/modules/init_weights.py
+Comment: 
+
+Filename: tepe/modules/layers.py
+Comment: 
+
+Filename: tepe/modules/loss.py
+Comment: 
+
+Filename: tepe/modules/model_utils.py
+Comment: 
+
+Filename: tepe/modules/model_zoo.py
+Comment: 
+
 Filename: tepe/modules/backbone/__init__.py
 Comment: 
 
 Filename: tepe/modules/backbone/mobilenet_rfb.py
 Comment: 
 
 Filename: tepe/modules/backbone/mobilenetv2.py
 Comment: 
 
 Filename: tepe/modules/backbone/resnet.py
 Comment: 
 
+Filename: tepe/modules/backbone/shufflenetv2.py
+Comment: 
+
 Filename: tepe/modules/backbone/simplenet.py
 Comment: 
 
 Filename: tepe/modules/backbone/vgg.py
 Comment: 
 
 Filename: tepe/modules/neck/__init__.py
 Comment: 
 
+Filename: tepe/modules/neck/fpn.py
+Comment: 
+
+Filename: tepe/modules/neck/pan.py
+Comment: 
+
 Filename: tepe/modules/optim/__init__.py
 Comment: 
 
 Filename: tepe/modules/optim/adabelief.py
 Comment: 
 
 Filename: tepe/modules/optim/adafactor.py
@@ -219,30 +249,108 @@
 
 Filename: tepe/modules/scheduler/step_lr.py
 Comment: 
 
 Filename: tepe/modules/scheduler/tanh_lr.py
 Comment: 
 
-Filename: tepe/modules/utils/__init__.py
+Filename: tepe/tasks/__init__.py
 Comment: 
 
-Filename: tepe/modules/utils/layers.py
+Filename: tepe/tasks/attention_rpn/README.txt
 Comment: 
 
-Filename: tepe/modules/utils/loss.py
+Filename: tepe/tasks/attention_rpn/__init__.py
 Comment: 
 
-Filename: tepe/modules/utils/model_utils.py
+Filename: tepe/tasks/attention_rpn/all_config.py
 Comment: 
 
-Filename: tepe/modules/utils/scheduler.py
+Filename: tepe/tasks/attention_rpn/builder.py
 Comment: 
 
-Filename: tepe/tasks/__init__.py
+Filename: tepe/tasks/attention_rpn/inference.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/task.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/__init__.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/attention_rpn_detector.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/query_support_detector.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/backbone/__init__.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/backbone/resnet.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/dense_heads/__init__.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/dense_heads/attention_rpn_head.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/roi_extractors/__init__.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/roi_extractors/base_roi_extractor.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/roi_extractors/single_level_roi_extractor.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/roi_heads/__init__.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/roi_heads/base_roi_head.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/roi_heads/multi_relation_roi_head.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/roi_heads/standard_roi_head.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/roi_heads/test_mixins.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/roi_heads/bbox_heads/__init__.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/roi_heads/bbox_heads/multi_relation_bbox_head.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/roi_heads/shared_head/__init__.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/model/roi_heads/shared_head/res_layer.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/pipelines/__init__.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/pipelines/formatting.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/pipelines/transforms.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/utils/__init__.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/utils/aggregation_layer.py
+Comment: 
+
+Filename: tepe/tasks/attention_rpn/utils/checkpoint.py
 Comment: 
 
 Filename: tepe/tasks/cfa/__init__.py
 Comment: 
 
 Filename: tepe/tasks/cfa/auto_encoder.py
 Comment: 
@@ -252,20 +360,101 @@
 
 Filename: tepe/tasks/cfa/module.py
 Comment: 
 
 Filename: tepe/tasks/cfa/predictor.py
 Comment: 
 
+Filename: tepe/tasks/cfa/requirements.txt
+Comment: 
+
 Filename: tepe/tasks/cfa/task.py
 Comment: 
 
 Filename: tepe/tasks/cfa/utils.py
 Comment: 
 
+Filename: tepe/tasks/deeplabv3/__init__.py
+Comment: 
+
+Filename: tepe/tasks/deeplabv3/create_model.py
+Comment: 
+
+Filename: tepe/tasks/deeplabv3/deeplab.py
+Comment: 
+
+Filename: tepe/tasks/deeplabv3/task.py
+Comment: 
+
+Filename: tepe/tasks/deeplabv3/utils.py
+Comment: 
+
+Filename: tepe/tasks/mobilenetv2/__init__.py
+Comment: 
+
+Filename: tepe/tasks/mobilenetv2/task.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/__init__.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/evaluator.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/predictor.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/requirements.txt
+Comment: 
+
+Filename: tepe/tasks/nanodet/task.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/trainer.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/util/__init__.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/util/box_transform.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/util/check_point.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/util/config.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/util/flops_counter.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/util/logger.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/util/misc.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/util/path.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/util/rank_filter.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/util/scatter_gather.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/util/util_mixins.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/util/visualization.py
+Comment: 
+
+Filename: tepe/tasks/nanodet/util/yacs.py
+Comment: 
+
 Filename: tepe/tasks/rd/__init__.py
 Comment: 
 
 Filename: tepe/tasks/rd/de_resnet.py
 Comment: 
 
 Filename: tepe/tasks/rd/evalutor.py
@@ -279,24 +468,246 @@
 
 Filename: tepe/tasks/rd/predictor.py
 Comment: 
 
 Filename: tepe/tasks/rd/resnet.py
 Comment: 
 
-Filename: tepe/tasks/rd/task copy.py
+Filename: tepe/tasks/rd/task.py
 Comment: 
 
-Filename: tepe/tasks/rd/task.py
+Filename: tepe/tasks/resnet/__init__.py
+Comment: 
+
+Filename: tepe/tasks/resnet/task.py
+Comment: 
+
+Filename: tepe/tasks/shufflenet_heatmap/__init__.py
+Comment: 
+
+Filename: tepe/tasks/shufflenet_heatmap/evaluator.py
 Comment: 
 
-Filename: tepe/tasks/rd/trainer.py
+Filename: tepe/tasks/shufflenet_heatmap/predictor.py
 Comment: 
 
-Filename: tepe/tasks/rd/utils.py
+Filename: tepe/tasks/shufflenet_heatmap/task.py
+Comment: 
+
+Filename: tepe/tasks/shufflenet_heatmap/trainer.py
+Comment: 
+
+Filename: tepe/tasks/shufflenet_heatmap/utils.py
+Comment: 
+
+Filename: tepe/tasks/shufflenet_heatmap/models/__init__.py
+Comment: 
+
+Filename: tepe/tasks/shufflenet_heatmap/models/v1.py
+Comment: 
+
+Filename: tepe/tasks/shufflenet_heatmap/models/v2.py
+Comment: 
+
+Filename: tepe/tasks/shufflenet_line/__init__.py
+Comment: 
+
+Filename: tepe/tasks/shufflenet_line/evaluator.py
+Comment: 
+
+Filename: tepe/tasks/shufflenet_line/model.py
+Comment: 
+
+Filename: tepe/tasks/shufflenet_line/predictor.py
+Comment: 
+
+Filename: tepe/tasks/shufflenet_line/task.py
+Comment: 
+
+Filename: tepe/tasks/shufflenet_line/trainer.py
+Comment: 
+
+Filename: tepe/tasks/simplenet/__init__.py
+Comment: 
+
+Filename: tepe/tasks/simplenet/classifier.py
+Comment: 
+
+Filename: tepe/tasks/simplenet/task.py
+Comment: 
+
+Filename: tepe/tasks/ssdlite_rfb/__init__.py
+Comment: 
+
+Filename: tepe/tasks/ssdlite_rfb/anchor.py
+Comment: 
+
+Filename: tepe/tasks/ssdlite_rfb/augmentation.py
+Comment: 
+
+Filename: tepe/tasks/ssdlite_rfb/backbone.py
+Comment: 
+
+Filename: tepe/tasks/ssdlite_rfb/box_utils.py
+Comment: 
+
+Filename: tepe/tasks/ssdlite_rfb/creat_model.py
+Comment: 
+
+Filename: tepe/tasks/ssdlite_rfb/loss.py
+Comment: 
+
+Filename: tepe/tasks/ssdlite_rfb/ssd.py
+Comment: 
+
+Filename: tepe/tasks/ssdlite_rfb/task.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/__init__.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/activations.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/common.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/datasets.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/experimental.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/loss.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/task.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/yolo.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/yolov5_detector.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/yolov5_evaluator.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/yolov5_trainer.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/yolov5l.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/yolov5m.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/yolov5m2.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/yolov5n.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/yolov5s.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/yolov5x.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/anchors.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov3-spp.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov3-tiny.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov3.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov5-bifpn.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov5-fpn.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov5-p2.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov5-p6.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov5-p7.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov5-panet.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov5l6.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov5m6.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov5n6.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov5s-ghost.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov5s-transformer.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov5s6.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hub/yolov5x6.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hyps/hyp.finetune.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hyps/hyp.finetune_objects365.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hyps/hyp.scratch-high.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hyps/hyp.scratch-low.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hyps/hyp.scratch-med.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/hyps/hyp.scratch.yaml
+Comment: 
+
+Filename: tepe/tasks/yolov5/utils/__init__.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/utils/augmentations.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/utils/autoanchor.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/utils/callbacks.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/utils/general.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/utils/metrics.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/utils/plots.py
+Comment: 
+
+Filename: tepe/tasks/yolov5/utils/torch_utils.py
 Comment: 
 
 Filename: tepe/tasks/yolox/__init__.py
 Comment: 
 
 Filename: tepe/tasks/yolox/task.py
 Comment: 
@@ -447,38 +858,41 @@
 
 Filename: tepe/utils/dist.py
 Comment: 
 
 Filename: tepe/utils/general.py
 Comment: 
 
-Filename: tepe/utils/get_subimg.py
+Filename: tepe/utils/meter.py
 Comment: 
 
-Filename: tepe/utils/meter.py
+Filename: tepe/utils/model_utils.py
 Comment: 
 
 Filename: tepe/utils/plots.py
 Comment: 
 
 Filename: tepe/utils/tensorrt_utils.py
 Comment: 
 
 Filename: tepe/utils/torch_utils.py
 Comment: 
 
-Filename: tepe-0.6.9.5.dist-info/LICENSE
+Filename: tepe-0.7.5.2.dist-info/LICENSE
+Comment: 
+
+Filename: tepe-0.7.5.2.dist-info/METADATA
 Comment: 
 
-Filename: tepe-0.6.9.5.dist-info/METADATA
+Filename: tepe-0.7.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: tepe-0.6.9.5.dist-info/WHEEL
+Filename: tepe-0.7.5.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: tepe-0.6.9.5.dist-info/top_level.txt
+Filename: tepe-0.7.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tepe-0.6.9.5.dist-info/RECORD
+Filename: tepe-0.7.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tepe/__init__.py

```diff
@@ -1,5 +1,13 @@
-__version__ = "0.6.9.5"
+__version__ = "0.7.5.2"
 
-from . import tasks
-from .core import get_task, print_tasks, get_task_cls
-from .core.exporter import Exporter
+from .core import get_task, print_tasks
+from .core.exporter import Exporter
+from .core.cli import main as cli
+from .utils.general import close_logger, show_logger
+
+__all__ = [
+    "get_task", "print_tasks", 
+    "Exporter",
+    "cli",
+    "close_logger", "show_logger",
+]
```

## tepe/core/__init__.py

```diff
@@ -1,7 +1,6 @@
 from .register import register_config, get_task, print_tasks, get_task_cls
 from .base_task import BaseTask
 from .base_trainer import Trainer
 from .base_evaluator import Evaluator
 from .base_predictor import Predictor
 from .exporter import Exporter
-from .launch import launch
```

## tepe/core/base_evaluator.py

```diff
@@ -62,24 +62,26 @@
                 save_dir = 'outputs'
             self.save_dir = increment_path(
                 os.path.join(save_dir, 'eval'), mkdir=True, increment=False
             )
         else:
             self.save_dir = None
         self.metrics = metrics
+        self.result_imgs = {}  # 用于存放eval过程中产生的图片
 
     def evaluate(self, model=None):
         """
         Args:
             model: model to evaluate.
 
         Returns:
             a dict contains:
 
         """
+        self.result_imgs.clear()
         if model is not None:
             self.model = model
         n_samples = max(len(self.dataloader) - 1, 1)
         self.inference_time = 0.0
         eval_meter = MeterBuffer(len(self.dataloader) + 10)
         self.model.eval()
         self.model.to(self.device)
@@ -92,15 +94,18 @@
 
         metrics_dict = {k: v.avg for k, v in eval_meter.get_avg_meter().items()}
 
         a_infer_time = 1000 * self.inference_time / (n_samples * self.dataloader.batch_size)
         info = "Average inference time: {:.2f} ms".format(a_infer_time)
         info += ", " + ", ".join(
             ["{}: {:.3f}".format(k, v) for k, v in metrics_dict.items()])
-        logger.info(colorstr('blue', info))
+        # logger.info(colorstr('blue', info))
+        logger.info(info)
+
+        metrics_dict['eval_result_imgs'] = self.result_imgs  # 将结果图放在输出的字典中
 
         return metrics_dict
 
     def evaluate_one_iter(self, data):
         """
 
         Args:
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## tepe/core/base_predictor.py

```diff
@@ -20,16 +20,15 @@
                  save_result: bool = False,
                  **kwargs) -> None:
 
         self.save_dir = save_dir
         self.save_result = save_result
         self._mkdir_flag = False
         self.view_result = False
-        for flag, value in kwargs.items():
-            setattr(self, flag, value)
+        self.pred2anno = False  # 预测结果保存成训练时的标注文件
 
     @abstractmethod
     def __call__(self, img_meta: Union[np.ndarray, Dict]) -> Optional[Union[np.ndarray, Dict]]:
         """
         Examples:
             result = self.run(img)
             draw_img = self.draw(img, result)
@@ -39,36 +38,36 @@
 
         Returns: destination image or None
         """
         pass
 
     @abstractmethod
     def run(self, img_meta: Union[np.ndarray, Dict]) -> Dict:
-        """
-        run once forward
+        """run once forward
+
         Args:
             img_meta: source image dict, include img, path and other fields
 
         Returns: network inference results
         """
         pass
 
     @abstractmethod
     def draw(self, img: np.ndarray, results: Dict) -> np.ndarray:
-        """
-        visualize the inference results.
+        """visualize the inference results.
+
         Args:
             img: source image
             results: dict of results from self.run function
 
         Returns: destination image
         """
         pass
 
-    def predict(self, source: str or Path,
+    def predict(self, source: Union[str, Path],
                 view_img: bool = True,
                 save_img: bool = True,
                 **kwargs) -> None:
         """
         source: file/dir/URL/glob, 0 for webcam
         """
         self._check_flag(view_img, save_img, kwargs)
@@ -100,24 +99,18 @@
 
             # Save results (image with detections)
             if self.save_result:
                 basename = os.path.basename(path)
                 name, suffix = os.path.splitext(basename)
                 save_path = os.path.join(self.save_dir, f'{name}_result{suffix}')  # img.jpg
                 if dataset.mode == 'image':
-                    self.save_result_image(result_image, save_path)
+                    cv2.imwrite(save_path, result_image)
                 else:  # 'video' or 'stream'
                     if vid_writer is None:
-                        if vid_cap:  # video
-                            fps = vid_cap.get(cv2.CAP_PROP_FPS)
-                            w = int(vid_cap.get(cv2.CAP_PROP_FRAME_WIDTH))
-                            h = int(vid_cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
-                        else:  # stream
-                            fps, w, h = 30, result_image.shape[1], result_image.shape[0]
-                            save_path += '.mp4'
+                        fps, w, h = 30, result_image.shape[1], result_image.shape[0]
                         vid_writer = cv2.VideoWriter(save_path, cv2.VideoWriter_fourcc(*'mp4v'), fps, (w, h))
                         logger.info(f'Save video...')
                     vid_writer.write(result_image)
 
             # Show results
             if self.view_result:
                 cv2.namedWindow(str(path), cv2.WINDOW_FREERATIO)
@@ -130,52 +123,67 @@
                     key = cv2.waitKey(1)
                 if key & 0xFF == 27:
                     break
             
         if num_img > 0:
             logger.info("Average prediction time: {:.4f}s".format(infer_time / num_img))
         if self.save_result:
-            logger.info(f'Result save in {self.save_dir}')
+            logger.info(f'Result save in {self.save_dir}/')
 
-    @staticmethod
-    def save_result_image(result_image, save_path):
-        if not os.path.exists(os.path.dirname(save_path)):
-            os.makedirs(os.path.dirname(save_path))
-        cv2.imwrite(save_path, result_image)
-    
-    def _check_flag(self, view_img, save_img, kwargs):
+    def annotate(self, 
+                 source: Union[str, Path], 
+                 format: str = "labelme",
+                 target: Optional[Union[str, Path]] = None,) -> None:
+        """将预测结果保存到标注文件
+
+        Args:
+            source (str | Path): 图片/视频路径
+            format (str, optional): 保存标注的格式. Defaults to "labelme".
+            target (Optional[Union[str, Path]], optional): 标注文件保存的路径. 默认保存在output_dir下.
+
+        Raises:
+            NotImplementedError: 基类不实现
         """
-        检查是否绘制结果，是否显示、保存结果图像
+
+        raise NotImplementedError(
+            f'{self.__class__.__name__} does not implement annotate function'
+        )
+
+    def _check_flag(self, view_img, save_img, kwargs):
+        """检查是否绘制结果，是否显示、保存结果图像
         """
         self.view_result |= (view_img and check_imshow())
         self.save_result |= save_img
-        for flag, value in kwargs.items():
-            setattr(self, flag, value)
         if self.save_result and not self._mkdir_flag:
             if self.save_dir is None:
                 logger.warning("Not specified 'save_dir'")
                 self.save_result = False
             else:
                 self.save_dir = increment_path(
                     os.path.join(self.save_dir, 'predict'), mkdir=True,
                     increment=False
                 )
                 self._mkdir_flag = True
 
+        msg = f'save_result: {self.save_result}, view_result: {self.view_result}'
+        for flag, value in kwargs.items():
+            setattr(self, flag, value)
+            msg += f', {flag}: {value}'
+        logger.info(msg)
+
     def _parse_source(self, source):
-        """
-        解析路径的格式: file/dir/URL/glob, 0 for webcam，返回可迭代对象dataset
+        """解析路径的格式: file/dir/URL/glob, 0 for webcam，返回可迭代对象dataset
         """
         source = str(source)
         is_file = Path(source).suffix[1:] in (IMG_FORMATS + VID_FORMATS)
         is_url = source.lower().startswith(('rtsp://', 'rtmp://', 'http://', 'https://'))
         webcam = source.isnumeric() or source.endswith('.txt') or (is_url and not is_file)
         if is_url and is_file:
             source = check_file(source)  # download
 
         # Dataloader
         if webcam:
             cudnn.benchmark = True  # set True to speed up constant image size inference
             dataset = LoadStreams(source)
         else:
             dataset = LoadImages(source)
-        return dataset
+        return dataset
```

## tepe/core/base_task.py

```diff
@@ -5,25 +5,28 @@
 from abc import ABCMeta, abstractmethod
 from typing import List, Dict, Tuple, Any, Optional, Literal, Union, Callable
 
 import addict
 import torch
 from loguru import logger
 from tabulate import tabulate
+from tepe.core.base_trainer import Trainer
+from tepe.core.base_evaluator import Evaluator
+from tepe.core.base_predictor import Predictor
+from tepe.modules.scheduler import Scheduler
 from tepe.utils.general import ROOT, show_runtime_info, init_seeds, setup_logger
 from tepe.utils.torch_utils import load_ckpt
 
 
 class BaseTask(metaclass=ABCMeta):
     """Basic class for any task."""
 
     def __init__(self) -> None:
         super().__init__()
         setup_logger()
-        show_runtime_info()
 
         self.seed: int = 42
         self.data_root: str
         self.input_size: int or tuple or list
         self.cache: bool = False
 
         # train
@@ -37,23 +40,23 @@
         self.basic_lr_per_img = 0.01
         self.__learning_rate = None
         self.fp16 = False
 
         self.device = 0
         self.ema = True
         self.early_stop = True
-        self.print_interval = 10  # iter
+        self.print_interval = 1  # iter [1, max_epoch * len(dataload)]
 
         # eval
+        self.eval_after_epoch = 5
         self.eval_interval = 1  # epoch
 
         # predict
 
         # export
-        self.out_file: str = None
         self.input_name = 'images'
         self.output_name = 'output'
         self.trt_version = ['7']
         self.suffix: str = ''
         self.opset: int = 12
         self.dynamic: bool = False
         self.no_onnxsim: bool = False
@@ -98,46 +101,45 @@
     def learning_rate(self, value):
         self.__learning_rate = value
 
     @abstractmethod
     def get_model(self, train=True):
         pass
 
-    @abstractmethod
     def get_train_loader(self):
         pass
 
     def get_eval_loader(self):
         pass
 
     def get_transform(
             self,
-            mode: Literal['train', 'val', 'test'] = 'train'
+            mode: Literal['train', 'val', 'test'] = 'train',
     ) -> Union[None, Union[Callable, Tuple[Callable, ...]]]:
         return None
 
     def get_optimizer(self, **kwargs):
         pass
 
-    def get_lr_scheduler(self, **kwargs) -> Union[None, Callable]:
+    def get_lr_scheduler(self, **kwargs) -> Union[None, Scheduler, Callable]:
         return None
 
     def get_loss(self):
         return None
 
     def get_metrics(self) -> Union[None, Callable]:
         return None
 
-    def get_trainer(self) -> Union[None, Callable]:
+    def get_trainer(self) -> Union[None, Trainer, Callable]:
         return None
 
-    def get_evaluator(self, train: bool=False) -> Union[None, Callable]:
+    def get_evaluator(self, train: bool=False) -> Union[None, Evaluator, Callable]:
         return None
 
-    def get_predictor(self) -> Union[None, Callable]:
+    def get_predictor(self) -> Union[None, Predictor, Callable]:
         return None
 
     def train(self):
         init_seeds(self.seed)
         trainer = self.get_trainer()
         if trainer is None:
             raise NotImplementedError(f'{self.__class__.__name__} does not'
@@ -243,14 +245,15 @@
                             pass
                         if src_value == v:
                             continue
                         logger.warning(f"default args {k}'s type is {src_type}, "
                                        f"now it will be {arg_type}")
             setattr(self, k, v)
             logger.info(f"set task's attr '{k}' from args, its value is {v}")
+        return self
 
     @staticmethod
     def load_ckpt(model, weights, device=0, is_state_dict=True, load_keys=None):
 
         """
         load ckpt to model
         Args:
@@ -268,8 +271,8 @@
             return
 
         load_ckpt(
             model, weights,
             device=device,
             is_state_dict=is_state_dict,
             load_keys=load_keys
-        )
+        )
```

## tepe/core/base_trainer.py

```diff
@@ -1,107 +1,120 @@
 import os
-import sys
 import shutil
 import time
 import datetime
-import yaml
 from typing import Dict, Iterable
 
 import torch
 from loguru import logger
 from torch.utils.tensorboard import SummaryWriter
 
-from ..modules.utils.model_utils import get_model_info
-from ..utils.dist import get_local_rank, get_rank, get_world_size
-from ..utils.general import get_bar, setup_logger, save_task_attr_to_yaml
-from ..utils.meter import MeterBuffer
-from ..utils.torch_utils import select_device, load_ckpt, ModelEMA, EarlyStopping, is_parallel
+from tepe.modules.scheduler import Scheduler
+from tepe.utils.general import show_runtime_info, setup_logger, save_task_attr_to_yaml, save_task_config_py
+from tepe.utils.dist import get_local_rank, get_rank, get_world_size
+from tepe.utils.model_utils import get_model_info
+from tepe.utils.meter import MeterBuffer
+from tepe.utils.torch_utils import select_device, load_ckpt, ModelEMA, EarlyStopping, is_parallel
 
 
 class Trainer:
     def __init__(self, task):
-        # init function only defines some basic attr, other attrs like model,
-        # optimizer are built in before_train methods.
-        self.task = task
+        """
+        初始化一些训练时用到的基础属性，比如是否滑动平均模型、半精度训练、分布式训练等等
+        Args:
+            task: BaseTask类型的配置任务类
+        """
+        from tepe.core.base_task import BaseTask
+
+        show_runtime_info()
+
+        self.task: BaseTask = task
         
         # training related attr
         self.epoch = 0
         self.amp_training = task.fp16
         self.scaler = torch.cuda.amp.GradScaler(enabled=task.fp16)
         self.is_distributed = get_world_size() > 1
         self.rank = get_rank()
         self.local_rank = get_local_rank()
         self.device = select_device(task.device)
         self.use_model_ema = task.ema if hasattr(task, 'ema') else False
         self.max_epoch = self.task.max_epoch
+        self.eval_after_epoch = self.task.eval_after_epoch
 
         # data/dataloader related attr
         self.data_type = torch.float16 if task.fp16 else torch.float32
         self.input_size = task.input_size
         self.best_eval_value = ['', 0]
 
         # ealy stop
         self.stopper = EarlyStopping(patience=30, early_stop=task.early_stop)
 
         # metric record
         self.meter = MeterBuffer(window_size=task.print_interval)
 
         self.resume = task.resume
-        if self.resume:
+        if self.resume and task.resume_ckpt is not None:
             self.train_result_path = os.path.dirname(task.resume_ckpt)
         else:
             self.train_result_path = task.output_dir
 
         if self.rank == 0:
             os.makedirs(self.train_result_path, exist_ok=True)
 
         # logger
         setup_logger(os.path.join(self.train_result_path, 'train_log.txt'), mode='o')
         # Tensorboard logger
         self.tblogger = SummaryWriter(self.train_result_path)
 
         # save args
         save_task_attr_to_yaml(task, self.train_result_path)
+        save_task_config_py(task, self.train_result_path)
 
         logger.info("task value:\n{}".format(self.task))
 
     def train(self):
         self.before_train()
         try:
             for self.epoch in range(self.start_epoch, self.max_epoch):
-                logger.info("---> Epoch{}/{}".format(self.epoch + 1, self.max_epoch))
+                # logger.info("---> Epoch{}/{}".format(self.epoch + 1, self.max_epoch))
                 self.before_epoch()
 
                 self.train_one_epoch()
 
                 stop = self.after_epoch()
                 # early stop
                 if stop < 0:
                     break
         except Exception:
             raise
         finally:
             self.after_train()
 
     def before_train(self):
+        """
+        初始化训练时所用到的关键组件，比如模型、数据加载器、评估器、损失函数、优化器、学期率下降策略等
+        Returns:
+            None
+        """
 
         # 1. model related init
         torch.cuda.set_device(self.device)
         model = self.task.get_model(train=True)
         model.to(self.device)
-        get_model_info(model, verbose=True, img_size=self.input_size)
+        # get_model_info(model, verbose=True, img_size=self.input_size)
 
         # 2. data related init
         self.train_loader = self.task.get_train_loader()
         # self.prefetcher = DataPrefetcher(self.train_loader)
 
         # max_iter means iters per epoch
         self.max_iter = len(self.train_loader)
 
-        # 3. evaluator init
+        # 3. evaluator init TODO: 可以不需要
         self.evaluator = self.task.get_evaluator(train=True)
 
         # 4. loss
         self.loss_fn = self.task.get_loss()
 
         # 5. solver related init
         self.optimizer = self.task.get_optimizer()
@@ -123,147 +136,200 @@
         logger.info("Training start...")
         # logger.info("\n{}".format(model))
 
     def before_epoch(self):
         pass
 
     def train_one_epoch(self):
-        self.pbar = get_bar(self.train_loader, 'train')
-        for self.iter, data in enumerate(self.pbar):
+        # self.pbar = get_bar(self.train_loader, 'train')
+        for self.iter, data in enumerate(self.train_loader):
             self.before_iter()
-            outputs = self.train_one_iter(data)
-            self.after_iter(outputs)
+            loss_dict = self.train_one_iter(data)
+            self.after_iter(loss_dict)
 
     def before_iter(self):
+        self.optimizer.zero_grad()
         self.iter_start_time = time.time()
 
     def train_one_iter(self, data) -> Dict:
-        inps, targets = data
-        inps = inps.to(self.data_type)
-        targets = targets.to(self.data_type)
-        targets.requires_grad = False
+        """
+        Args:
+            data:
+
+        Returns:
+            loss(Dict)
+        """
+        data = self.preprocess_batch(data)
 
         with torch.cuda.amp.autocast(enabled=self.amp_training):
-            outputs = self.model(inps, targets)
+            outputs = self.model(data['img'])
 
-        loss = outputs['loss']
+        if self.loss_fn is not None:
+            loss = self.loss_fn(outputs, data)
+            loss_dict = loss if isinstance(loss, dict) else {'loss': loss}
+        else:
+            loss_dict = {k: v for k, v in outputs.items() if 'loss' in k} if isinstance(outputs, dict) \
+                else {'loss': outputs}
+
+        assert 'loss' in loss_dict
+        loss = loss_dict['loss']
 
-        self.optimizer.zero_grad()
         self.scaler.scale(loss).backward()
         self.scaler.step(self.optimizer)
         self.scaler.update()
 
-        # update per iter or per epoch?
-        if self.lr_scheduler:
-            lr = self.lr_scheduler.update_lr(self.progress_in_iter + 1)
-            for param_group in self.optimizer.param_groups:
-                param_group["lr"] = lr
-        else:
-            lr = self.init_lr
-
-        outputs['lr'] = lr
-        return outputs
+        return loss_dict
 
     def after_iter(self, outputs):
+        """
+        更新lr_scheduler, optimizer, ema_model, tensorboard, 获得当前lr，打印log
+        Args:
+            outputs(dict):
+        Returns:
+            None
+        """
         self.iter_end_time = time.time()
 
+        # get current lr
+        lrl = [param_group['lr'] for param_group in self.optimizer.param_groups]
+        outputs['lr'] = sum(lrl) / len(lrl)
+
+        # update lr per iter (if have)
+        if self.lr_scheduler is not None:
+            if isinstance(self.lr_scheduler, Scheduler):
+                self.lr_scheduler.step_update(num_updates=self.progress_in_iter + 1)
+
         # update ema model
         if self.use_model_ema:
             self.ema_model.update(self.model)
 
         self.meter.update(
             iter_time=self.iter_end_time - self.iter_start_time,
             **outputs
         )
 
+        # add tensorboard
+        for key in 'loss', 'lr':
+            if key not in self.meter:
+                continue
+            scalar_value = self.meter[key].latest
+            if scalar_value is not None:
+                self.tblogger.add_scalar(
+                    tag=f'train/{key}', scalar_value=scalar_value, global_step=self.epoch + 1
+                )
+
         # log needed information
-        if (self.iter + 1) % self.task.print_interval == 0:
+        if (self.progress_in_iter + 1) % self.task.print_interval == 0:
             # self.pbar.set_description(('%10s' * 2 + '%10.4g' * 5) % (
             #     f'{self.iter + 1}/{self.max_iter}', mem, *mloss, targets.shape[0], imgs.shape[-1]))
+            progress_str = "Epoch: {}/{}, iter: {}/{}".format(
+                self.epoch + 1, self.max_epoch,
+                self.progress_in_iter + 1, self.max_iter * self.max_epoch
+            )
 
             loss_meter = self.meter.get_filtered_meter("loss")
             loss_str = ", ".join(
-                ["{}: {:.5f}".format(k, v.latest) for k, v in loss_meter.items()]
+                ["{}: {:.5f}".format(k, float(v.latest)) for k, v in loss_meter.items()]
             )
-            for k, v in loss_meter.items():
-                self.tblogger.add_scalar(tag=k, scalar_value=v.latest, global_step=self.progress_in_iter)
 
             time_meter = self.meter.get_filtered_meter("time")
             time_str = ", ".join(
                 ["{}: {:.3f}s".format(k, v.avg) for k, v in time_meter.items()]
             )
 
-            postfix_str = "mem: {:.0f}MB, {}".format(
+            msg = "{}, mem: {:.0f}MB, {}".format(
+                progress_str,
                 torch.cuda.max_memory_allocated() / (1024 * 1024),
                 loss_str,
             )
 
             if self.meter["lr"].latest is not None:
                 lr_value = self.meter["lr"].latest
-                postfix_str += ", lr: {:.5f}".format(lr_value)
-                self.tblogger.add_scalar(
-                    tag='lr', scalar_value=lr_value, global_step=self.progress_in_iter)
+                msg += ", lr: {:.5f}".format(lr_value)
+
+            logger.info(msg)
 
-            self.pbar.set_postfix_str(postfix_str)
-            self.meter.clear_meters()
+            # self.pbar.set_postfix_str(postfix_str)
+        self.meter.clear_meters()
 
     def after_epoch(self):
-        self.save_ckpt(ckpt_name="latest")
+        """
+        更新lr_scheduler, 保存模型、评估模型、判断是否触发早停
+        Returns:
+            -1 - 触发早停
+             0 - 继续训练
+        """
+        # update lr per epoch (if have)
+        if self.lr_scheduler is not None:
+            if isinstance(self.lr_scheduler, Scheduler):
+                self.lr_scheduler.step(epoch=self.epoch + 1)
+
+        self.save_ckpt(ckpt_name="last")
+
+        if self.evaluator is None:
+            return 0
+
+        if (self.epoch + 1) % self.task.eval_interval == 0 and self.epoch + 1 >= self.eval_after_epoch:
+            update_ckpt, current_eval_value = self.validate()
 
-        if (self.epoch + 1) % self.task.eval_interval == 0:
-            if self.evaluator is not None:
-                update_ckpt, current_eval_value = self.validate()
-            else:
-                # TODO: =========
-                update_ckpt, current_eval_value = 1, 0
             if update_ckpt:
                 # save a best ckpt file
-                filename = os.path.join(self.train_result_path, "latest_ckpt.pth")
-                best_filename = os.path.join(self.train_result_path, "best_ckpt.pth")
+                filename = os.path.join(self.train_result_path, "last.pth")
+                best_filename = os.path.join(self.train_result_path, "best.pth")
                 shutil.copyfile(filename, best_filename)
 
             if self.stopper(epoch=self.epoch, fitness=current_eval_value):
                 return -1
         return 0
 
     def after_train(self):
         # set best trained model path to task.weights
-        setattr(self.task, 'weights', os.path.join(self.train_result_path, 'best_ckpt.pth'))
+        setattr(self.task, 'weights', os.path.join(self.train_result_path, 'best.pth'))
         
         logger.info(
             "Training task is done in {:.3f} hours and the best {} is {:.2f}".format(
                 (time.time() - self.t0) / 3600, self.best_eval_value[0], self.best_eval_value[1])
         )
         logger.info("Save weights to {}".format(self.train_result_path))
 
     @property
     def progress_in_iter(self):
         return self.epoch * self.max_iter + self.iter
 
+    def preprocess_batch(self, data):
+        data['img'] = data['img'].to(self.data_type).to(self.device)
+        data['target'] = data['target'].to(self.data_type).to(self.device)
+        data['target'].requires_grad = False
+        return data
+
     def resume_train(self, model):
         if self.task.resume:
             logger.info("resume training")
             if self.task.resume_ckpt is None:
                 ckpt_file = os.path.join(self.train_result_path, "latest" + "_ckpt.pth")
             else:
                 ckpt_file = self.task.resume_ckpt
+            assert os.path.exists(ckpt_file), FileNotFoundError("not found ckpt file")
 
             ckpt = torch.load(ckpt_file, map_location=self.device)
+            assert [key in ckpt for key in ("model", "epochs")]
             # resume the model/optimizer state dict
             model.load_state_dict(ckpt["model"])
-            self.optimizer.load_state_dict(ckpt["optimizer"])
+            if "optimizer" in ckpt:
+                self.optimizer.load_state_dict(ckpt["optimizer"])
+
             # resume the training states variables
-            start_epoch = ckpt['epoch'] + 1
+            start_epoch = ckpt['epochs'] + 1
             self.start_epoch = start_epoch
             logger.info( f"loaded checkpoint '{ckpt_file}' (epoch {self.start_epoch})")
             if self.max_epoch < self.start_epoch:
                 logger.info(
-                    f"{ckpt_file} has been trained for {ckpt['epoch']} epochs. "
+                    f"{ckpt_file} has been trained for {ckpt['epochs']} epochs. "
                     f"Training for {self.max_epoch} more epochs.")
-                self.max_epoch += ckpt['epoch']  # finetune additional epochs
+                self.max_epoch += ckpt['epochs']  # finetune additional epochs
             # save last ckpt
             last_ckpt_file = os.path.join(self.train_result_path, f'epoch-{start_epoch}.pth')
             shutil.copyfile(ckpt_file, last_ckpt_file)
         else:
             if self.task.weights is not None and self.task.pretrained:
                 logger.info("loading checkpoint for fine tuning")
                 weights_file = self.task.weights
@@ -293,41 +359,47 @@
                 eval_model = eval_model.module
 
         eval_model.eval()
 
         eval_result = self.evaluator.evaluate(model=eval_model)
         self.model.train()
 
+        for k, v in eval_result.items():
+            if k == 'eval_result_imgs':
+                for n, im in eval_result[k].items():
+                    self.tblogger.add_figure(f'val/{n}', figure=im, global_step=self.epoch + 1)
+            else:
+                try:
+                    self.tblogger.add_scalar(f"val/{k}", scalar_value=v, global_step=self.epoch + 1)
+                except:
+                    pass
+
         eval_res_list = [[k, v] for k, v in eval_result.items() if not isinstance(v, Iterable)]
         eval_key_value = eval_res_list[0]  # first eval value
         self.best_eval_value[0] = eval_key_value[0]
         if 'loss' in eval_key_value[0]:
             if self.epoch == 0:
                 self.best_eval_value[1] = 1000  # adjust initial eval_value
                 self.stopper.best_fitness = 1000
             self.stopper.up_down = False
             update_ckpt = eval_key_value[1] < self.best_eval_value[1]
             self.best_eval_value[1] = min(self.best_eval_value[1], eval_key_value[1])
         else:
             update_ckpt = eval_key_value[1] > self.best_eval_value[1]
             self.best_eval_value[1] = max(self.best_eval_value[1], eval_key_value[1])
 
-        for k, v in eval_res_list:
-            if isinstance(v, str): continue
-            self.tblogger.add_scalar(f"val/{k}", v, self.epoch + 1)
-
         current_eval_value = eval_key_value[1]
 
         return update_ckpt, current_eval_value
 
     def save_ckpt(self, ckpt_name):
         if self.rank == 0:
             save_model = self.ema_model.ema if self.use_model_ema else self.model
             ckpt_state = {
                 "epochs": self.epoch + 1,
                 "model": save_model.state_dict(),
                 "optimizer": self.optimizer.state_dict(),
                 'date': datetime.datetime.now().isoformat()
             }
 
-            filename = os.path.join(self.train_result_path, ckpt_name + "_ckpt.pth")
+            filename = os.path.join(self.train_result_path, ckpt_name + ".pth")
             torch.save(ckpt_state, filename)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## tepe/core/exporter.py

```diff
@@ -20,17 +20,17 @@
         else:
             self.model = model
         assert self.model is not None
         setattr(self.model, 'export', True)
 
         self.input_size = task.input_size
         self.save_dir = task.output_dir
-        out_file = task.out_file
-        assert self.task.weights is not None
         self.save_name, _ = os.path.splitext(os.path.basename(self.task.weights))
+        out_file = getattr(task, 'out_file', None)  # 由命令行参数-o给出
+        assert self.task.weights is not None
         if out_file is not None:
             if os.path.isdir(out_file):  # file_dir
                 self.save_dir = out_file
             elif os.path.isfile(out_file):  # file_path
                 self.save_dir = os.path.abspath(os.path.dirname(out_file))
             else:  # file_name
                 self.save_name = out_file
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## tepe/core/register.py

```diff
@@ -36,35 +36,36 @@
         task_dict[name] = cls
         return cls
 
     return _register
 
 
 def get_task(name: str) -> BaseTask:
-    """
-    Get task instance according to task name or task file.
+    """Get task instance according to task name or task file.
+
     Args:
         name: task name or task file
 
     Returns:
         task config instance
     """
 
     return get_task_cls(name)()
 
 
-def get_task_cls(name: str) -> ClassVar[BaseTask]:
-    """
-    Get task class according to task name or task file.
+def get_task_cls(name: str) -> Callable:
+    """Get task class according to task name or task file.
+
     Args:
         name: task name or task file
 
     Returns:
         task config class
     """
+    assert name is not None or name
     if Path(name).suffix == '.py':
         if not os.path.exists(name):
             raise FileNotFoundError("{} is not found.".format(name))
         task_file = name
     else:
         task_file_list = _get_task_file_list()
         task_file = task_file_list.get(name)
@@ -73,24 +74,23 @@
     task_cls = _find_task_obj(task_file)
     assert task_cls is not None, \
         ImportError(f'Task object is not found in {name}.')
     return task_cls
 
 
 def print_tasks() -> None:
-    """
-    Print tasks list.
+    """Print tasks list.
     """
     task_file_list = _get_task_file_list()
     print('\n'.join(['{:20s} {}'.format(k, v) for k, v in task_file_list.items()]))
 
 
 def _find_task_obj(task_file: str) -> Union[None, Callable]:
-    """
-    Find task class in task file.
+    """Find task class in task file.
+
     Args:
         task_file: Absolute path of task config.
 
     Returns:
         task class
     """
     task_cls = None
@@ -104,28 +104,47 @@
         if not isclass(obj):
             continue
         if obj_name.startswith('_'):
             continue
         if issubclass(obj, BaseTask) and obj_name != 'BaseTask':
             task_cls = obj
     sys.path.remove(task_dir)
+    sys.modules.pop(module_name)
 
     return task_cls
 
 
 def _get_task_file_list() -> Dict:
-    """
-    Get task files list.
+    """Get task files list.
+
     Returns:
         Dict {task_name: task_file}
     """
     task_list = {}
     from tepe import tasks
     tasks_dir = os.path.dirname(tasks.__file__)
     for task_name in os.listdir(tasks_dir):
         if task_name.startswith('_') and not os.path.isdir(os.path.join(tasks_dir, task_name)):
             continue
         task_file = os.path.join(tasks_dir, task_name, 'task.py')
 
         if task_name not in task_list and os.path.exists(task_file):
             task_list[task_name] = task_file
-    return task_list
+    return task_list
+
+
+def get_task_from_output_dir(output_dir: str) -> BaseTask:
+    """从output_dir中直接获得task实例，含有权重路径
+
+    Args:
+        output_dir (str): 含有配置文件和权重文件的文件夹
+
+    Returns:
+        BaseTask: task实例
+    """
+    from tepe.utils.general import find_config, find_weights
+    
+    assert os.path.exists(output_dir) and os.path.isdir(output_dir)
+    config_file = find_config(output_dir)
+    task = get_task(config_file)
+    task.weights = find_weights(output_dir)
+    return task
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## tepe/core/predictor/anomaly_detector.py

```diff
@@ -1,40 +1,30 @@
 import os
 from loguru import logger
-import numpy as np
-import tifffile as tiff
 
 
 class AnomalyDetector(object):
-
-    @staticmethod
-    def save_result_to_xml(image_path, image_shape,
+    def save_result_to_xml(self, image_path, image_shape,
                            anomaly_area, save_dir=None):
         """
         将预测结果以voc格式写入到xml文件中
         Args:
             image_path: 图像路径
             image_shape: 原图大小，[h, w, c]
             anomaly_area: 异物检测的包围框, [[left, top, right, bottom], ...]
 
         Returns:
 
         """
         if save_dir is None:
             save_dir = os.path.abspath(os.path.dirname(image_path))
 
-        from tepe.data.voc_xml import PascalVocWriter
+        from tepe.data.annotation import PascalVocWriter
         img_name = os.path.basename(image_path)
         writer = PascalVocWriter('VOC2007', img_name, image_shape)
         for r in anomaly_area:
             left, top, right, bottom = r
             writer.add_bnd_box(int(left), int(top), int(right), int(bottom), name='abnormal')
         name, suffix = os.path.splitext(img_name)
         save_xml_path = os.path.join(save_dir, name + '.xml')
         writer.save(target_file=save_xml_path)
-        # logger.info(f'Detections save in {save_xml_path}')
-
-    @staticmethod
-    def save_heatmap(heatmap: np.ndarray, save_path: str):
-        if not os.path.exists(os.path.dirname(save_path)):
-            os.makedirs(os.path.dirname(save_path))
-        tiff.imwrite(save_path, heatmap)
+        logger.info(f'Detections save in {save_xml_path}')
```

## tepe/core/predictor/segmentor.py

```diff
@@ -1,39 +1,45 @@
 import cv2
 from loguru import logger
+from matplotlib.pyplot import axes
+import numpy as np
 
 import torch
+from torch import nn
 from torchvision import transforms as T
 from tepe.data.datasets.seg_voc_custom import voc_cmap
 from tepe.utils.torch_utils import select_device, time_synchronized
 from tepe.core.base_predictor import Predictor
 
 
 class SegPredictor(Predictor):
     def __init__(self,
                  input_size,
                  classes,
-                 weights=None,
-                 model=None,
+                 model,
                  device=0,
                  half=False,
                  save_dir=None
                  ):
         super().__init__(save_dir)
         
         self.device = select_device(device)
         self.classes = classes
+        self.pth = isinstance(model, nn.Module)
         self.half = half
-        self.model = model.eval()
         self.input_size = [input_size, input_size] if isinstance(input_size, int) else input_size
+        if self.pth:
+            self.model = model.eval()
 
-        if self.device.type != 'cpu':
-            self.model.cuda()
-            self.model(torch.zeros(1, 3, *self.input_size).to(self.device).type_as(
-                next(self.model.parameters())))  # run once
+            if self.device.type != 'cpu':
+                self.model.cuda()
+                self.model(torch.zeros(1, 3, *self.input_size).to(self.device).type_as(
+                    next(self.model.parameters())))  # run once
+        else:
+            self.model = model
 
         self.preprocess = T.Compose([
                 T.ToTensor(),
                 T.Resize(self.input_size),
                 T.Normalize(mean=[0.485, 0.456, 0.406],
                             std=[0.229, 0.224, 0.225]),
             ])
@@ -41,30 +47,36 @@
 
     def __call__(self, img_meta):
         return self.draw(img_meta['img'], self.run(img_meta))
 
     def run(self, img_meta):
         img0 = img_meta['img']
         img = self.preprocess(img0).unsqueeze(0) # To tensor of NCHW
-        img = img.to(self.device)
-        if self.device.type == "cuda":
-            if self.half:
-                img = img.half()  # to FP16
-        
-        t0 = time_synchronized()
-        with torch.no_grad():
-            pred = self.model(img)
-        pred = pred.max(1)[1].cpu().numpy()[0] # HW
-
-        logger.info("Infer time: {:.4f}s".format(time_synchronized() - t0))
+        if self.pth:
+            img = img.to(self.device)
+            if self.device.type == "cuda":
+                if self.half:
+                    img = img.half()  # to FP16
+            
+            t0 = time_synchronized()
+            with torch.no_grad():
+                pred = self.model(img)
+            pred = pred.max(1)[1].cpu().numpy()[0] # HW
+
+            logger.info("Infer time: {:.4f}s".format(time_synchronized() - t0))
+        else:
+            img = img.numpy()
+            self.model.setInput(img)
+            pred = self.model.forward()
+            pred = np.argmax(pred, axis=1).squeeze()
 
         return pred
 
     def draw(self, img, output):
         label_map = self.color_map[output].astype('uint8')
         label_map = cv2.resize(label_map, (img.shape[1], img.shape[0]))
         label_map = cv2.cvtColor(label_map, cv2.COLOR_RGB2BGR)
-        vis_res = cv2.addWeighted(img, 0.7, label_map, 0.3, 0)
+        vis_res = cv2.addWeighted(img, 1, label_map, 0.3, 0)
 
         return vis_res
```

## tepe/data/infer_datasets.py

```diff
@@ -12,93 +12,14 @@
 import cv2
 import numpy as np
 
 from ..utils.general import check_requirements, clean_str
 from .utils import IMG_FORMATS, VID_FORMATS
 
 
-class LoadImages1:
-    # TEPE image/video inference dataloader, i.e. `python detect.py --source image.jpg/vid.mp4`
-    def __init__(self, path):
-        p = str(Path(path).resolve())  # os-agnostic absolute path
-        if '*' in p:
-            files = sorted(glob.glob(p, recursive=True))  # glob
-        elif os.path.isdir(p):
-            files = sorted(glob.glob(os.path.join(p, '*.*')))  # dir
-        elif os.path.isfile(p):
-            files = [p]  # files
-        else:
-            raise Exception(f'ERROR: {p} does not exist')
-
-        images = [x for x in files if x.split('.')[-1].lower() in IMG_FORMATS]
-        videos = [x for x in files if x.split('.')[-1].lower() in VID_FORMATS]
-        ni, nv = len(images), len(videos)
-
-        # self.img_size = img_size
-        self.files = images + videos
-        self.nf = ni + nv  # number of files
-        self.video_flag = [False] * ni + [True] * nv
-        self.mode = 'image'
-        # self.auto = auto
-        if any(videos):
-            self.new_video(videos[0])  # new video
-        else:
-            self.cap = None
-        assert self.nf > 0, f'No images or videos found in {p}. ' \
-                            f'Supported formats are:\nimages: {IMG_FORMATS}\nvideos: {VID_FORMATS}'
-
-    def __iter__(self):
-        self.count = 0
-        return self
-
-    def __next__(self):
-        if self.count == self.nf:
-            raise StopIteration
-        path = self.files[self.count]
-
-        if self.video_flag[self.count]:
-            # Read video
-            self.mode = 'video'
-            ret_val, img0 = self.cap.read()
-            if not ret_val:
-                self.count += 1
-                self.cap.release()
-                if self.count == self.nf:  # last video
-                    raise StopIteration
-                else:
-                    path = self.files[self.count]
-                    self.new_video(path)
-                    ret_val, img0 = self.cap.read()
-
-            self.frame += 1
-            s = f'video {self.count + 1}/{self.nf} ({self.frame}/{self.frames}) {path}: '
-
-        else:
-            # Read image
-            self.count += 1
-            img0 = cv2.imread(path)  # BGR
-            assert img0 is not None, f'Image Not Found {path}'
-            s = f'image {self.count}/{self.nf} {path}: '
-
-        # Convert
-        # img = img.transpose((2, 0, 1))[::-1]  # HWC to CHW, BGR to RGB
-        # img = np.ascontiguousarray(img)
-
-        img_meta = dict(path=path, img=img0, is_vid=self.cap, idx=self.count)
-        return img_meta
-
-    def new_video(self, path):
-        self.frame = 0
-        self.cap = cv2.VideoCapture(path)
-        self.frames = int(self.cap.get(cv2.CAP_PROP_FRAME_COUNT))
-
-    def __len__(self):
-        return self.nf  # number of files
-
-
 class LoadImages:
     # TEPE image/video inference dataloader, i.e. `python detect.py --source image.jpg/vid.mp4`
     def __init__(self, path):
         p = str(Path(path).resolve())  # os-agnostic absolute path
         if '*' in p:
             files = sorted(glob.glob(p, recursive=True))  # glob
         elif os.path.isdir(p):
@@ -130,15 +51,16 @@
         return self
 
     def __next__(self):
         if self.count == self.nf:
             raise StopIteration
         path = self.files[self.count]
 
-        if self.video_flag[self.count]:
+        is_vid = self.video_flag[self.count]
+        if is_vid:
             # Read video
             self.mode = 'video'
             ret_val, img0 = self.cap.read()
             if not ret_val:
                 self.count += 1
                 self.cap.release()
                 if self.count == self.nf:  # last video
@@ -158,15 +80,15 @@
             assert img0 is not None, f'Image Not Found {path}'
             s = f'image {self.count}/{self.nf} {path}: '
 
         # Convert
         # img = img.transpose((2, 0, 1))[::-1]  # HWC to CHW, BGR to RGB
         # img = np.ascontiguousarray(img)
 
-        return path, img0, self.cap, self.count
+        return path, img0, is_vid, self.count
 
     def new_video(self, path):
         self.frame = 0
         self.cap = cv2.VideoCapture(path)
         self.frames = int(self.cap.get(cv2.CAP_PROP_FRAME_COUNT))
 
     def __len__(self):
```

## tepe/data/augments/__init__.py

```diff
@@ -0,0 +1,3 @@
+00000000: 2320 6672 6f6d 2062 6173 655f 6175 676d  # from base_augm
+00000010: 656e 7473 2069 6d70 6f72 7420 5069 7065  ents import Pipe
+00000020: 6c69 6e65                                line
```

## tepe/data/augments/seg_augment.py

```diff
@@ -369,15 +369,16 @@
     def __call__(self, img, lbl):
         """
         Args:
             img (PIL Image): Image to be scaled.
         Returns:
             PIL Image: Rescaled image.
         """
-        return F.resize(img, self.size, self.interpolation), F.resize(lbl, self.size, Image.NEAREST)
+        return F.resize(img, self.size, self.interpolation), \
+               F.resize(lbl, self.size, InterpolationMode.NEAREST)
 
     def __repr__(self):
         interpolate_str = _pil_interpolation_to_str[self.interpolation]
         return self.__class__.__name__ + '(size={0}, interpolation={1})'.format(self.size, interpolate_str) 
     
 
 class ExtColorJitter(object):
```

## tepe/data/datasets/__init__.py

```diff
@@ -1,4 +1,5 @@
 from .cls_datasets import CustomClsDataset
 from .ssdrfb_voc import VOCDataset
 from .keypoint_dataset import KeyPointsDataset
+from .line_dataset import LineDataset
 from .ad_dataset import AnomalyDataset
```

## tepe/data/datasets/ad_dataset.py

```diff
@@ -1,10 +1,8 @@
 import os
-from loguru import logger
-from tqdm import tqdm
 import cv2
 import numpy as np
 from PIL import Image
 import torch
 from torch.utils.data import Dataset
 from torchvision import transforms as T
 
@@ -14,65 +12,53 @@
 MVTEC_CLASS_NAMES = ['bottle', 'cable', 'capsule', 'carpet', 'grid',
                      'hazelnut', 'leather', 'metal_nut', 'pill', 'screw',
                      'tile', 'toothbrush', 'transistor', 'wood', 'zipper']
 
 class AnomalyDataset(Dataset):
     def __init__(self, dataset_path, class_name='bottle',
                  transform=None, target_transform=None,
-                 resize_fn=None, is_train=True, paste=False,
+                 is_train=True, resize=256, paste=False,
                  is_mvtec=True, cache_img = False):
         # assert class_name in CLASS_NAMES, 'class_name: {}, should be in {}'.format(class_name, CLASS_NAMES)
         self.dataset_path = dataset_path
         self.class_name = class_name
         self.is_train = is_train
-        self.resize_fn = resize_fn
+        resize = [resize, resize] if isinstance(resize, int) else resize
+        self.resize = resize
         self.transform = transform
-        self.mask_transform = target_transform
-        self.is_mvtec = is_mvtec
+        self.target_transform = target_transform
         self.cache_img = cache_img
+        print("cache:",self.cache_img)
         self.imgs, self.img_paths, self.tgt_paths, self.masks = self.load_dataset_folder()
-        phase = 'train' if is_train else 'test'
-        logger.info(f'{phase}: found {len(self.img_paths)} images in scene {self.class_name}')
+        print("self.imgs:",len(self.imgs))
         self.paste = paste
         self.paste_img_paths = []
 
     def __getitem__(self, idx):
         if self.cache_img:
             img, x, y, mask = self.imgs[idx], self.img_paths[idx], self.tgt_paths[idx], self.masks[idx]
         else:
             x, y, mask = self.img_paths[idx], self.tgt_paths[idx], self.masks[idx]
-            img = self.load_resized_image(x)  # resized
+            img = cv2.imread(x)
 
         if self.paste:
             img = paste_images(img, self.paste_img_paths)
 
-        if self.transform:
-            img = self.transform(img)
+        img = self.transform(img)
 
-        if y == 0 or not self.is_mvtec:
-            mask = torch.zeros_like(img)
+        if y == 0:
+            mask = torch.zeros([1, self.resize[0], self.resize[1]])
         else:
             mask = Image.open(mask)
-            mask = self.mask_transform(mask)
-        
-        
-        return dict(img=img, target=y, mask=mask, path=x)
+            mask = self.target_transform(mask)
+
+        return img, y, mask
 
     def __len__(self):
         return len(self.img_paths)
-    
-    def load_resized_image(self, path):
-
-        im = cv2.imread(path)  # BGR
-        assert im is not None, f'Image Not Found {path}'
-
-        if self.resize_fn is not None:  # if sizes are not equal
-            im, ratio, dwh = self.resize_fn(im)
-
-        return im
 
     def load_dataset_folder(self):
         phase = 'train' if self.is_train else 'test'
         imgs, x, y, mask = [], [], [], []
 
         img_dir = os.path.join(self.dataset_path, self.class_name, phase)
         gt_dir = os.path.join(self.dataset_path, self.class_name, 'ground_truth')
@@ -81,40 +67,30 @@
         for img_type in img_types:
 
             img_type_dir = os.path.join(img_dir, img_type)
             if not os.path.isdir(img_type_dir):
                 continue
             img_fpath_list = sorted([os.path.join(img_type_dir, f)
                                     for f in os.listdir(img_type_dir)
-                                    if f.endswith(('.jpg', '.png'))])
+                                    if f.endswith('.jpg')])
 
             x.extend(img_fpath_list)
+            if self.cache_img:
+                img_tmp = []
+                for img_path_list in img_fpath_list:
+                    img_tmp.append(cv2.imread(img_path_list))
+                imgs.extend(img_tmp)
 
             if img_type == 'good':
                 y.extend([0] * len(img_fpath_list))
                 mask.extend([None] * len(img_fpath_list))
             else:
                 y.extend([1] * len(img_fpath_list))
-                if self.is_mvtec:
-                    gt_type_dir = os.path.join(gt_dir, img_type)
-                    img_fname_list = [os.path.splitext(os.path.basename(f))[0] for f in img_fpath_list]
-                    gt_fpath_list = [os.path.join(gt_type_dir, img_fname + '_mask.png')
-                                    for img_fname in img_fname_list]
-                    mask.extend(gt_fpath_list)
-                else:
-                    mask.extend([None] * len(img_fpath_list))
+                gt_type_dir = os.path.join(gt_dir, img_type)
+                img_fname_list = [os.path.splitext(os.path.basename(f))[0] for f in img_fpath_list]
+                gt_fpath_list = [os.path.join(gt_type_dir, img_fname + '_mask.png')
+                                for img_fname in img_fname_list]
+                mask.extend(gt_fpath_list)
 
         assert len(x) == len(y), 'number of x and y should be same'
-        if self.cache_img:
-            for img_path in tqdm(x, desc='cache images'):
-                imgs.append(self.load_resized_image(img_path))
-
-        return list(imgs), list(x), list(y), list(mask)
 
-    def add_hard_samples(self, samples):
-        self.img_paths.extend(list(samples))
-        if self.cache_img:
-            for p in samples:
-                self.imgs.append(self.load_resized_image(p))
-        self.tgt_paths.extend([0] * len(samples))
-        self.masks.extend([None] * len(samples))
-        logger.info(f'add {len(samples)} hard samples to dataset, new dataset size: {len(self.img_paths)}')
+        return list(imgs), list(x), list(y), list(mask)
```

## tepe/data/datasets/keypoint_dataset.py

```diff
@@ -1,155 +1,26 @@
 import copy
 import json
 import math
 import os
 import random
-from loguru import logger
 
-import numpy as np
-import cv2
 import albumentations as A
-from albumentations.pytorch import ToTensorV2
-import torch
+import cv2
 import matplotlib
+import numpy as np
+from loguru import logger
 from matplotlib import pyplot as plt
 from torch.utils.data import Dataset
+
 try:
     matplotlib.use('TkAgg')
 except:
     pass
 
-class NormalizeImage(object):
-    def __init__(self, mean=[103.53,116.28,123.675], 
-                 std=[57.375,57.12,58.395]):
-        self.mean = np.array(mean).astype(np.float32)
-        self.std = np.array(std).astype(np.float32)
-        pass
-
-    def __call__(self, image, labels=None):
-        image = image - self.mean
-        image = image / self.std
-        return image, labels
-
-
-class KPRandomPadCrop(object):
-    def __init__(self, ratio=0.25, pad_value=[128, 128, 128]):
-        assert (ratio > 0 and ratio <= 1)
-        self.ratio = ratio
-        self.pad_value = pad_value
-
-    def __call__(self, image, labels=None):
-        if random.randint(0,1):
-            h, w = image.shape[:2]
-            top_offset = int(h * random.uniform(0, self.ratio))
-            bottom_offset = int(h * random.uniform(0, self.ratio))
-            left_offset = int(w * random.uniform(0, self.ratio))
-            right_offset = int(w * random.uniform(0, self.ratio))
-            # pad
-            if random.randint(0,1):
-                image = cv2.copyMakeBorder(image, top_offset, bottom_offset, left_offset, right_offset, cv2.BORDER_CONSTANT, value=self.pad_value)
-                if labels is not None and len(labels) > 0:
-                    labels[:, 0] = (labels[:, 0] * w + left_offset) / (w + left_offset + right_offset)
-                    labels[:, 1] = (labels[:, 1] * h + top_offset) / (h + top_offset + bottom_offset)
-            # crop
-            else:
-                image = image[top_offset:h - bottom_offset, left_offset:w-right_offset]
-                if labels is not None and len(labels) > 0:
-                    labels[:, 0] = (labels[:, 0] * w - left_offset) / (w - left_offset - right_offset)
-                    labels[:, 1] = (labels[:, 1] * h - top_offset) / (h - top_offset - bottom_offset)
-
-        return image, labels
-
-
-class KPRandomHorizontalFlip(object):
-    def __init__(self):
-        pass
-
-    def __call__(self, image, labels=None):
-        if random.randint(0, 1):
-            image = cv2.flip(image, 1)
-            h, w = image.shape[:2]
-            if labels is not None and len(labels) > 0:
-                labels[:, 0] = 1.0 - labels[:, 0]
-        return image, labels
-
-
-class KPResizeImage(object):
-    def __init__(self, size):
-        self.size = size
-
-    def __call__(self, image, labels=None, resize=None):
-        h, w = image.shape[:2]
-        if resize is None:
-            image = cv2.resize(image, tuple(self.size))
-        else:
-            image = cv2.resize(image, tuple(resize))
-        return image, labels
-
-
-class KPRandomSwapChannels(object):
-    def __init__(self):
-        self.swaps = ((0, 1, 2), (0, 2, 1),
-                      (1, 0, 2), (1, 2, 0),
-                      (2, 0, 1), (2, 1, 0))
-
-    def __call__(self, image, labels=None):
-        if random.randint(0, 1):
-            index = random.randint(0, len(self.swaps) - 1)
-            image = image[:, :, self.swaps[index]]
-        return image, labels
-
-
-class KPRandomContrast(object):
-    def __init__(self, lower=0.8, upper=1.2):
-        self.lower = lower
-        self.upper = upper
-        assert self.upper >= self.lower, "contrast upper must be >= lower."
-        assert self.lower >= 0, "contrast lower must be non-negative."
-
-    # expects float image
-    def __call__(self, image, labels=None):
-        if random.randint(0, 1):
-            alpha = random.uniform(self.lower, self.upper)
-            image = image.astype(np.float32) * alpha
-        return image, labels
-
-
-class KPRandomHSV(object):
-    def __init__(self, hue=0.1, saturation=1.2, value=1.2):
-        self.hue = hue
-        self.saturation = saturation
-        self.value = value
-
-    def __call__(self, image, labels=None):
-        if random.randint(0, 1):
-            dh = random.uniform(-self.hue, self.hue)
-            ds = random.uniform(1, self.saturation)
-            if random.random() < 0.5:
-                ds = 1 / ds
-            dv = random.uniform(1, self.value)
-            if random.random() < 0.5:
-                dv = 1 / dv
-
-            image = image.astype(np.float32) / 255.0
-            image = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)
-
-            def wrap_hue(x):
-                x[x >= 360.0] -= 360.0
-                x[x < 0.0] += 360.0
-                return x
-
-            image[:, :, 0] = wrap_hue(image[:, :, 0] + (360.0 * dh))
-            image[:, :, 1] = np.clip(ds * image[:, :, 1], 0.0, 1.0)
-            image[:, :, 2] = np.clip(dv * image[:, :, 2], 0.0, 1.0)
-
-            image = cv2.cvtColor(image, cv2.COLOR_HSV2BGR)
-            image = (image * 255.0)
-        return image, labels
-
 
 class Albumentations:
     # Albumentations class (optional, only used if package is installed)
     # pip install albumentations
     def __init__(self, transform):
         self.transform = transform
 
@@ -167,61 +38,67 @@
             labels[:, 0] /= im.shape[1]
             labels[:, 1] /= im.shape[0]
 
         return im, labels
 
 
 class KeyPointsDataset(Dataset):
-    def __init__(self, root, transform=None, class_name=None, image_sets=None,
-                 is_train=False, imgsz=224, stride=8,
+    def __init__(self, root, num_keypoint_cls, transform=None, class_name=(), image_sets=None,
+                 is_train=False, imgsz=224, stride=8, body_part_kpt_ids=(),
                  gauss_ratio=1, gauss_sigma=0.5):
         self.root = root
+        class_name = list(range(num_keypoint_cls)) if not class_name else class_name
         self.class_name = {cls: idx for idx, cls in enumerate(class_name)}
-        self.kp_num = len(class_name)
+        if num_keypoint_cls != len(self.class_name):
+            logger.info("override number of keypoint classes")
+        self.kp_num = len(self.class_name)
+
         self.transform = transform
         if isinstance(transform, A.Compose):
             self.transform = Albumentations(transform)
         self.data = []
 
         imgsz = [imgsz, imgsz] if isinstance(imgsz, int) else imgsz
         input_h, input_w = imgsz
-        self.heatmap_h, self.heatmap_w = input_h, input_w
-        self.gauss_ratio = gauss_ratio * stride
+        self.input_size = self.heatmap_h, self.heatmap_w = input_h, input_w
+        self.gauss_ratio = gauss_ratio * stride * (input_w // 224)
         self.gauss_sigma = gauss_sigma * stride
+        self.stride = stride
+        self.body_part_kpt_ids = body_part_kpt_ids
 
         is_dir = True if image_sets is None else False
         if is_dir:
             for name in os.listdir(root):
                 if name.split('.')[-1] not in ['jpg', 'png']:
                     continue
                 path, label = self.get_data(name)
-                if label is None:
+                if label is None or not label:
                     continue
                 self.data.append((path, np.stack(label, axis=0)))
         else:
             if not isinstance(image_sets, list):
                 image_sets = [image_sets]
             is_txt = True
             txt_paths = []
-            for set in image_sets:
-                txt = os.path.join(root, set + '.txt')
+            for dset in image_sets:
+                txt = os.path.join(root, dset + '.txt')
                 txt_paths.append(txt)
                 is_txt &= os.path.exists(txt)
             # split dataset
             if not is_txt:
                 logger.info(f'Not found {image_sets}.txt, generate it.')
                 self.split_train_val(root)
                 txt_name = 'train' if is_train else 'val'
                 txt_paths = [os.path.join(root, txt_name + '.txt')]
             for txt in txt_paths:
                 with open(txt, 'r') as f:
                     for line in f:
                         name = line.strip()
                         path, label = self.get_data(name)
-                        if label is None:
+                        if label is None or not label:
                             continue
                         self.data.append((path, np.stack(label, axis=0)))
 
         logger.info(f'class name: {self.class_name}')
 
         desc = 'train' if is_train else 'val' if not is_dir else 'IMG'
         desc += f': found {len(self.data)} images'
@@ -239,44 +116,56 @@
             return None, None
         return img_path, self.read_label(json_path)
 
     def read_label(self, json_path):
         with open(json_path, 'r') as f:
             json_dict = json.load(f)
         img_width, img_height = json_dict["imageWidth"], json_dict["imageHeight"]
-        # sort shapes from classes 0
-        shapes = [shape for shape in json_dict['shapes'] if shape["shape_type"] == "point"]
+        shapes = [shape for shape in json_dict['shapes'] if shape["shape_type"] != "rectangle"]
+        # sort shapes
         # shapes.sort(key=lambda x: float(x['points'][0][0]) + float(x['points'][0][1]))
-        # for shape in shapes:
-        #     x, y = shape["points"][0]
+
         labels = []
         for shape in shapes:
-            x, y = shape["points"][0]
-            idx = self.class_name[shape["label"]]
+            cls = self.class_name[shape["label"]]
+            points = shape["points"]
+            x, y = points[0][0], points[0][1]
             # normalize
             x /= img_width
             y /= img_height
-            label = np.array([x, y, idx], dtype=np.float32)
+            label = np.array([x, y, cls], dtype=np.float32)
             labels.append(label)
+        # for shape in shapes:
+        #     for cls, (x, y) in enumerate(shape["points"]):
+        #         # normalize
+        #         x /= img_width
+        #         y /= img_height
+        #         label = np.array([x, y, cls], dtype=np.float32)
+        #         labels.append(label)
         return labels
 
     def __getitem__(self, idx):
         img_path, label_ori = self.data[idx]
         labels = copy.deepcopy(label_ori)
         img = cv2.imread(img_path)
         img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
 
         if self.transform is not None:
             img, labels = self.transform(img, labels)
 
         img = img.transpose(2, 0, 1)
 
-        heatmap = self.generate_target(labels)
+        kpt_maps = self.generate_target(labels)
 
-        return img, heatmap
+        if self.body_part_kpt_ids:
+            paf_maps = self._generate_paf_maps(labels)
+            meta_data = dict(img=img, path=img_path, target=kpt_maps, paf_maps=paf_maps, idx=idx)
+        else:
+            meta_data = dict(img=img, path=img_path, target=kpt_maps, idx=idx)
+        return meta_data
 
     def __len__(self):
         return len(self.data)
 
     def generate_target(self, labels):
         """
 
@@ -320,17 +209,79 @@
             g_y = max(0, -ul[1]), min(br[1], self.heatmap_h) - ul[1]
             # Image range
             img_x = max(0, ul[0]), min(br[0], self.heatmap_w)
             img_y = max(0, ul[1]), min(br[1], self.heatmap_h)
 
             heatmap[img_y[0]:img_y[1], img_x[0]:img_x[1]] = g[g_y[0]:g_y[1], g_x[0]:g_x[1]]
 
-        target = cv2.resize(target, (28, 28)).reshape(28, 28, -1).transpose(2, 0, 1)
+        tgt_h, tgt_w = self.heatmap_h // self.stride, self.heatmap_w // self.stride
+        target = cv2.resize(target, (tgt_w, tgt_h)).reshape(tgt_w, tgt_h, -1).transpose(2, 0, 1)
         return target
 
+    def _generate_paf_maps(self, keypoints):
+        n_pafs = len(self.body_part_kpt_ids)
+        assert n_pafs > 0
+        n_rows, n_cols = self.input_size
+
+        paf_maps = np.zeros(shape=(n_pafs * 2, n_rows // self.stride, n_cols // self.stride), dtype=np.float32)
+
+        self._paf_thickness = 2
+        for paf_idx in range(n_pafs):
+            ai, bi = self.body_part_kpt_ids[paf_idx][0], self.body_part_kpt_ids[paf_idx][1]
+            if ai >= len(keypoints) or bi >= len(keypoints): continue
+            keypoint_a, keypoint_b = keypoints[ai], keypoints[bi]
+
+            self._set_paf(paf_maps[paf_idx * 2:paf_idx * 2 + 2],
+                          keypoint_a[0], keypoint_a[1], keypoint_b[0], keypoint_b[1],
+                          self.stride, self._paf_thickness)
+
+        return paf_maps
+
+    def _generate_segment_maps(self, keypoints):
+        n_rows, n_cols = self.input_size
+        seg_maps = np.zeros(shape=(2, n_rows // self.stride, n_cols // self.stride), dtype=np.uint8)
+
+        for keypoint in keypoints:
+            kp = keypoint[:,:2]
+            kp /= self._stride
+            kp = np.array([kp]).reshape(1, -1, 2).round().astype(np.int32)
+            seg_maps[0] = cv2.polylines(seg_maps[0], kp, isClosed=False, color=255, thickness=self._paf_thickness)
+
+        paf_maps = seg_maps / 255
+        paf_maps[-1] = 1 - paf_maps[0]
+
+        return paf_maps
+
+    def _set_paf(self, paf_map, x_a, y_a, x_b, y_b, stride, thickness):
+        x_a /= stride
+        y_a /= stride
+        x_b /= stride
+        y_b /= stride
+        x_ba = x_b - x_a
+        y_ba = y_b - y_a
+        _, h_map, w_map = paf_map.shape
+        x_min = int(max(min(x_a, x_b) - thickness, 0))
+        x_max = int(min(max(x_a, x_b) + thickness, w_map))
+        y_min = int(max(min(y_a, y_b) - thickness, 0))
+        y_max = int(min(max(y_a, y_b) + thickness, h_map))
+        norm_ba = (x_ba * x_ba + y_ba * y_ba) ** 0.5
+        if norm_ba < 1e-7:  # Same points, no paf
+            return
+        x_ba /= norm_ba
+        y_ba /= norm_ba
+
+        for y in range(y_min, y_max):
+            for x in range(x_min, x_max):
+                x_ca = x - x_a
+                y_ca = y - y_a
+                d = math.fabs(x_ca * y_ba - y_ca * x_ba)
+                if d <= thickness:
+                    paf_map[0, y, x] = x_ba
+                    paf_map[1, y, x] = y_ba
+
     @staticmethod
     def split_train_val(root):
         image_list = []
         folder_path = os.path.join(root, 'images')
         if os.path.exists(folder_path) and os.path.isdir(folder_path):
             image_list += [name + '\n' for name in os.listdir(folder_path)
                            if name.split('.')[-1] in ['jpg', 'png']]
@@ -350,21 +301,14 @@
         fval = open(os.path.join(root, 'val.txt'), 'w')
         fval.writelines(val_images)
         fval.close()
 
         logger.info(f'train.txt and val.txt are generated in {root}')
 
     @staticmethod
-    def collate_fn(batch):
-        imgs, labels = list(zip(*batch))
-        imgs = torch.from_numpy(np.stack(imgs, 0))
-        labels = torch.from_numpy(np.stack(labels, 0))
-        return [imgs, labels]
-
-    @staticmethod
     def visual_add_image_with_heatmap(images, labels):
         """
         Args:
             images: (np.ndarray)
             labels:
 
         Returns:
@@ -391,36 +335,33 @@
             plt.imshow(cv2.resize(label0[kp_c], (w, h)), alpha=0.5)
 
         # plt.savefig('./tran_%d.jpg' % epoch)
         plt.show()
 
 
 if __name__ == '__main__':
-
-    RESIZE = (224, 224)
+    RESIZE = (640, 640)
 
     transform = A.Compose([
         A.Resize(RESIZE[0], RESIZE[1], p=1),
         A.RandomBrightnessContrast(brightness_limit=0.2, contrast_limit=0.2, p=0.4),
         A.Rotate(limit=15, border_mode=cv2.BORDER_REPLICATE, p=0.3),
         A.OneOf([
             A.HueSaturationValue(p=0.4),
             A.ChannelShuffle(p=0.5)
         ], p=1),
         A.Normalize(),
         # ToTensorV2()
     ], keypoint_params=A.KeypointParams(format='xy', label_fields=['class_labels']))
 
-    data_path = '/home/zepei/DATA/meter/dataset/special_meter'
-    dataset_train = KeyPointsDataset(data_path, transform=transform,
-                                     class_name=('pointer', 'marker'),
-                                     image_sets='train', is_train=True)
-
-
-    for idx in range(10):
-        images, labels = dataset_train[idx]
-        print(images.shape)
-        print(labels.shape)
-        # dataset_train.visual_add_image_with_heatmap(images, labels)
-        if idx == 0:
-            break
-
+    data_path = '/home/zepei/data/DATA/meter/dataset/samll_meter/yolo_h_1'
+    dataset_train = KeyPointsDataset(data_path, 7, transform=transform,
+                                     image_sets='train', is_train=True,
+                                     body_part_kpt_ids=[[1, 2], [2, 3], [3, 4], [4, 5], [5, 6]])
+
+    print('dataset size:', len(dataset_train))
+    # for idx in range(10):
+    data = dataset_train[2]
+    images, labels, parfs = data['img'], data['target'], data['paf_maps']
+    print(images.shape)
+    print(labels.shape)
+    print(parfs.shape)
```

## tepe/data/datasets/seg_voc_custom.py

```diff
@@ -1,18 +1,21 @@
 import os
 import sys
 import tarfile
 import collections
 import torch.utils.data as data
 import shutil
 import numpy as np
+import cv2
 
 from PIL import Image
 from torchvision.datasets.utils import download_url, check_integrity
 
+from tepe.data.augments.seg_augment import ExtCompose
+
 
 DATASET_YEAR_DICT = {
     '2012': {
         'url': 'http://host.robots.ox.ac.uk/pascal/VOC/voc2012/VOCtrainval_11-May-2012.tar',
         'filename': 'VOCtrainval_11-May-2012.tar',
         'md5': '6cd6e144f989b92b3379bac3b3de84fd',
         'base_dir': 'VOCdevkit/VOC2012'
@@ -125,18 +128,25 @@
     def __getitem__(self, index):
         """
         Args:
             index (int): Index
         Returns:
             tuple: (image, target) where target is the image segmentation.
         """
-        image = Image.open(self.images[index]).convert('RGB')
+        # image = Image.open(self.images[index]).convert('RGB')
+        image = cv2.imread(self.images[index])[:,:,::-1]  # rgb
         mask = Image.open(self.masks[index])
+
         if self.transform is not None:
-            image, mask = self.transform(image, mask)
+            if isinstance(self.transform, ExtCompose):
+                image = Image.fromarray(image, mode='RGB')
+                image, mask = self.transform(image, mask)
+            else:
+                transformed = self.transform(image=image, mask=np.array(mask, dtype='uint8'))
+                image, mask = transformed['image'], transformed['mask']
 
         return image, mask
 
     def __len__(self):
         return len(self.images)
 
     def load_image_label(self, idx):
```

## tepe/modules/__init__.py

```diff
@@ -1 +1 @@
-from ..utils import *
+from .model_zoo import MODEL_ZOO
```

## tepe/modules/backbone/__init__.py

```diff
@@ -1,6 +1,7 @@
 # from .mobilenet_rfb import MobilenetTinyRFB
 from .simplenet import SimpleNet, SimpleNetM, SimpleNetL
 from .mobilenetv2 import MobileNetV2
 from .resnet import resnet18, resnet34, resnet50, resnet101, resnet152, \
     resnext50_32x4d, resnext101_32x8d, wide_resnet101_2, wide_resnet50_2
-from .vgg import vgg11, vgg13, vgg16, vgg19, vgg11_bn, vgg13_bn, vgg16_bn, vgg19_bn
+from .vgg import vgg11, vgg13, vgg16, vgg19, vgg11_bn, vgg13_bn, vgg16_bn, vgg19_bn
+from .shufflenetv2 import ShuffleNetV2
```

## tepe/modules/backbone/mobilenet_rfb.py

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ..utils.layers import conv_bn, conv_dw
+from tepe.modules.layers import conv_bn, conv_dw
 
 
 class BasicConv(nn.Module):
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size,
```

## tepe/modules/neck/__init__.py

```diff
@@ -0,0 +1,3 @@
+00000000: 6672 6f6d 202e 6670 6e20 696d 706f 7274  from .fpn import
+00000010: 2046 504e 0a66 726f 6d20 2e70 616e 2069   FPN.from .pan i
+00000020: 6d70 6f72 7420 5041 4e0a                 mport PAN.
```

## tepe/modules/scheduler/__init__.py

```diff
@@ -1,7 +1,8 @@
+from .scheduler import Scheduler
 from .cosine_lr import CosineLRScheduler
 from .multistep_lr import MultiStepLRScheduler
 from .plateau_lr import PlateauLRScheduler
 from .poly_lr import PolyLRScheduler
 from .step_lr import StepLRScheduler
 from .tanh_lr import TanhLRScheduler
```

## tepe/modules/scheduler/cosine_lr.py

```diff
@@ -1,71 +1,75 @@
 """ Cosine Scheduler
 
 Cosine LR schedule with warmup, cycle/restarts, noise, k-decay.
 
 Hacked together by / Copyright 2021 Ross Wightman
 """
-import logging
+from loguru import logger
 import math
 import numpy as np
 import torch
 
 from .scheduler import Scheduler
 
 
-_logger = logging.getLogger(__name__)
-
-
 class CosineLRScheduler(Scheduler):
     """
     Cosine decay with restarts.
     This is described in the paper https://arxiv.org/abs/1608.03983.
 
     Inspiration from
     https://github.com/allenai/allennlp/blob/master/allennlp/training/learning_rate_schedulers/cosine.py
 
     k-decay option based on `k-decay: A New Method For Learning Rate Schedule` - https://arxiv.org/abs/2004.05909
     """
 
-    def __init__(self,
-                 optimizer: torch.optim.Optimizer,
-                 t_initial: int,
-                 lr_min: float = 0.,
-                 cycle_mul: float = 1.,
-                 cycle_decay: float = 1.,
-                 cycle_limit: int = 1,
-                 warmup_t=0,
-                 warmup_lr_init=0,
-                 warmup_prefix=False,
-                 t_in_epochs=True,
-                 noise_range_t=None,
-                 noise_pct=0.67,
-                 noise_std=1.0,
-                 noise_seed=42,
-                 k_decay=1.0,
-                 initialize=True) -> None:
+    def __init__(
+            self,
+            optimizer: torch.optim.Optimizer,
+            t_initial: int,
+            lr_min: float = 0.,       # lr下界
+            cycle_mul: float = 1.,    # 下次循环长度的乘子
+            cycle_decay: float = 1.,  # 下次循环初始值的乘子
+            cycle_limit: int = 1,     # 循环次数
+            warmup_t=0,
+            warmup_lr_init=0,
+            warmup_prefix=False,
+            t_in_epochs=True,
+            noise_range_t=None,
+            noise_pct=0.67,
+            noise_std=1.0,
+            noise_seed=42,
+            k_decay=1.0,              # 越大越平滑
+            initialize=True
+    ) -> None:
         super().__init__(
-            optimizer, param_group_field="lr",
-            noise_range_t=noise_range_t, noise_pct=noise_pct, noise_std=noise_std, noise_seed=noise_seed,
-            initialize=initialize)
+            optimizer, 
+            param_group_field="lr",
+            t_in_epochs=t_in_epochs,
+            noise_range_t=noise_range_t, 
+            noise_pct=noise_pct, 
+            noise_std=noise_std, 
+            noise_seed=noise_seed,
+            initialize=initialize
+        )
 
         assert t_initial > 0
         assert lr_min >= 0
         if t_initial == 1 and cycle_mul == 1 and cycle_decay == 1:
-            _logger.warning("Cosine annealing scheduler will have no effect on the learning "
+            logger.warning("Cosine annealing scheduler will have no effect on the learning "
                            "rate since t_initial = t_mul = eta_mul = 1.")
         self.t_initial = t_initial
         self.lr_min = lr_min
         self.cycle_mul = cycle_mul
         self.cycle_decay = cycle_decay
         self.cycle_limit = cycle_limit
         self.warmup_t = warmup_t
         self.warmup_lr_init = warmup_lr_init
         self.warmup_prefix = warmup_prefix
-        self.t_in_epochs = t_in_epochs
         self.k_decay = k_decay
         if self.warmup_t:
             self.warmup_steps = [(v - warmup_lr_init) / self.warmup_t for v in self.base_values]
             super().update_groups(self.warmup_lr_init)
         else:
             self.warmup_steps = [1 for _ in self.base_values]
 
@@ -95,25 +99,13 @@
                     for lr_max in lr_max_values
                 ]
             else:
                 lrs = [self.lr_min for _ in self.base_values]
 
         return lrs
 
-    def get_epoch_values(self, epoch: int):
-        if self.t_in_epochs:
-            return self._get_lr(epoch)
-        else:
-            return None
-
-    def get_update_values(self, num_updates: int):
-        if not self.t_in_epochs:
-            return self._get_lr(num_updates)
-        else:
-            return None
-
     def get_cycle_length(self, cycles=0):
         cycles = max(1, cycles or self.cycle_limit)
         if self.cycle_mul == 1.0:
             return self.t_initial * cycles
         else:
             return int(math.floor(-self.t_initial * (self.cycle_mul ** cycles - 1) / (1 - self.cycle_mul)))
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## tepe/modules/scheduler/multistep_lr.py

```diff
@@ -7,37 +7,40 @@
 from .scheduler import Scheduler
 from typing import List
 
 class MultiStepLRScheduler(Scheduler):
     """
     """
 
-    def __init__(self,
-                 optimizer: torch.optim.Optimizer,
-                 decay_t: List[int],
-                 decay_rate: float = 1.,
-                 warmup_t=0,
-                 warmup_lr_init=0,
-                 t_in_epochs=True,
-                 noise_range_t=None,
-                 noise_pct=0.67,
-                 noise_std=1.0,
-                 noise_seed=42,
-                 initialize=True,
-                 ) -> None:
+    def __init__(
+            self,
+            optimizer: torch.optim.Optimizer,
+            decay_t: List[int],
+            decay_rate: float = 1.,
+            warmup_t=0,
+            warmup_lr_init=0,
+            warmup_prefix=True,
+            t_in_epochs=True,
+            noise_range_t=None,
+            noise_pct=0.67,
+            noise_std=1.0,
+            noise_seed=42,
+            initialize=True,
+    ) -> None:
         super().__init__(
-            optimizer, param_group_field="lr",
+            optimizer, param_group_field="lr", t_in_epochs=t_in_epochs,
             noise_range_t=noise_range_t, noise_pct=noise_pct, noise_std=noise_std, noise_seed=noise_seed,
-            initialize=initialize)
+            initialize=initialize
+        )
 
-        self.decay_t = decay_t
+        self.decay_t = decay_t if isinstance(decay_t, list) else [decay_t]
         self.decay_rate = decay_rate
         self.warmup_t = warmup_t
         self.warmup_lr_init = warmup_lr_init
-        self.t_in_epochs = t_in_epochs
+        self.warmup_prefix = warmup_prefix
         if self.warmup_t:
             self.warmup_steps = [(v - warmup_lr_init) / self.warmup_t for v in self.base_values]
             super().update_groups(self.warmup_lr_init)
         else:
             self.warmup_steps = [1 for _ in self.base_values]
 
     def get_curr_decay_steps(self, t):
@@ -45,21 +48,11 @@
         # assumes self.decay_t is sorted
         return bisect.bisect_right(self.decay_t, t+1)
 
     def _get_lr(self, t):
         if t < self.warmup_t:
             lrs = [self.warmup_lr_init + t * s for s in self.warmup_steps]
         else:
+            if self.warmup_prefix:
+                t = t - self.warmup_t
             lrs = [v * (self.decay_rate ** self.get_curr_decay_steps(t)) for v in self.base_values]
-        return lrs
-
-    def get_epoch_values(self, epoch: int):
-        if self.t_in_epochs:
-            return self._get_lr(epoch)
-        else:
-            return None
-
-    def get_update_values(self, num_updates: int):
-        if not self.t_in_epochs:
-            return self._get_lr(num_updates)
-        else:
-            return None
+        return lrs
```

## tepe/modules/scheduler/plateau_lr.py

```diff
@@ -8,50 +8,55 @@
 
 from .scheduler import Scheduler
 
 
 class PlateauLRScheduler(Scheduler):
     """Decay the LR by a factor every time the validation loss plateaus."""
 
-    def __init__(self,
-                 optimizer,
-                 decay_rate=0.1,
-                 patience_t=10,
-                 verbose=True,
-                 threshold=1e-4,
-                 cooldown_t=0,
-                 warmup_t=0,
-                 warmup_lr_init=0,
-                 lr_min=0,
-                 mode='max',
-                 noise_range_t=None,
-                 noise_type='normal',
-                 noise_pct=0.67,
-                 noise_std=1.0,
-                 noise_seed=None,
-                 initialize=True,
-                 ):
-        super().__init__(optimizer, 'lr', initialize=initialize)
+    def __init__(
+            self,
+            optimizer,
+            decay_rate=0.1,
+            patience_t=10,
+            verbose=True,
+            threshold=1e-4,
+            cooldown_t=0,
+            warmup_t=0,
+            warmup_lr_init=0,
+            lr_min=0,
+            mode='max',
+            noise_range_t=None,
+            noise_type='normal',
+            noise_pct=0.67,
+            noise_std=1.0,
+            noise_seed=None,
+            initialize=True,
+    ):
+        super().__init__(
+            optimizer,
+            'lr',
+            noise_range_t=noise_range_t,
+            noise_type=noise_type,
+            noise_pct=noise_pct,
+            noise_std=noise_std,
+            noise_seed=noise_seed,
+            initialize=initialize,
+        )
 
         self.lr_scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(
             self.optimizer,
             patience=patience_t,
             factor=decay_rate,
             verbose=verbose,
             threshold=threshold,
             cooldown=cooldown_t,
             mode=mode,
             min_lr=lr_min
         )
 
-        self.noise_range = noise_range_t
-        self.noise_pct = noise_pct
-        self.noise_type = noise_type
-        self.noise_std = noise_std
-        self.noise_seed = noise_seed if noise_seed is not None else 42
         self.warmup_t = warmup_t
         self.warmup_lr_init = warmup_lr_init
         if self.warmup_t:
             self.warmup_steps = [(v - warmup_lr_init) / self.warmup_t for v in self.base_values]
             super().update_groups(self.warmup_lr_init)
         else:
             self.warmup_steps = [1 for _ in self.base_values]
@@ -78,36 +83,28 @@
                 # restore actual LR from before our last noise perturbation before stepping base
                 for i, param_group in enumerate(self.optimizer.param_groups):
                     param_group['lr'] = self.restore_lr[i]
                 self.restore_lr = None
 
             self.lr_scheduler.step(metric, epoch)  # step the base scheduler
 
-            if self.noise_range is not None:
-                if isinstance(self.noise_range, (list, tuple)):
-                    apply_noise = self.noise_range[0] <= epoch < self.noise_range[1]
-                else:
-                    apply_noise = epoch >= self.noise_range
-                if apply_noise:
-                    self._apply_noise(epoch)
+            if self._is_apply_noise(epoch):
+                self._apply_noise(epoch)
+
+    def step_update(self, num_updates: int, metric: float = None):
+        return None
 
     def _apply_noise(self, epoch):
-        g = torch.Generator()
-        g.manual_seed(self.noise_seed + epoch)
-        if self.noise_type == 'normal':
-            while True:
-                # resample if noise out of percent limit, brute force but shouldn't spin much
-                noise = torch.randn(1, generator=g).item()
-                if abs(noise) < self.noise_pct:
-                    break
-        else:
-            noise = 2 * (torch.rand(1, generator=g).item() - 0.5) * self.noise_pct
+        noise = self._calculate_noise(epoch)
 
         # apply the noise on top of previous LR, cache the old value so we can restore for normal
         # stepping of base scheduler
         restore_lr = []
         for i, param_group in enumerate(self.optimizer.param_groups):
             old_lr = float(param_group['lr'])
             restore_lr.append(old_lr)
             new_lr = old_lr + old_lr * noise
             param_group['lr'] = new_lr
         self.restore_lr = restore_lr
+
+    def _get_lr(self, t: int) -> float:
+        assert False, 'should not be called as step is overridden'
```

## tepe/modules/scheduler/poly_lr.py

```diff
@@ -1,68 +1,67 @@
 """ Polynomial Scheduler
 
 Polynomial LR schedule with warmup, noise.
 
 Hacked together by / Copyright 2021 Ross Wightman
 """
+from loguru import logger
 import math
-import logging
 
 import torch
 
 from .scheduler import Scheduler
 
 
-_logger = logging.getLogger(__name__)
-
-
 class PolyLRScheduler(Scheduler):
     """ Polynomial LR Scheduler w/ warmup, noise, and k-decay
 
     k-decay option based on `k-decay: A New Method For Learning Rate Schedule` - https://arxiv.org/abs/2004.05909
     """
 
-    def __init__(self,
-                 optimizer: torch.optim.Optimizer,
-                 t_initial: int,
-                 power: float = 0.5,
-                 lr_min: float = 0.,
-                 cycle_mul: float = 1.,
-                 cycle_decay: float = 1.,
-                 cycle_limit: int = 1,
-                 warmup_t=0,
-                 warmup_lr_init=0,
-                 warmup_prefix=False,
-                 t_in_epochs=True,
-                 noise_range_t=None,
-                 noise_pct=0.67,
-                 noise_std=1.0,
-                 noise_seed=42,
-                 k_decay=1.0,
-                 initialize=True) -> None:
+    def __init__(
+            self,
+            optimizer: torch.optim.Optimizer,
+            t_initial: int,
+            power: float = 0.5,
+            lr_min: float = 0.,
+            cycle_mul: float = 1.,
+            cycle_decay: float = 1.,
+            cycle_limit: int = 1,
+            warmup_t=0,
+            warmup_lr_init=0,
+            warmup_prefix=False,  # Exclude warmup period from decay schedule.
+            t_in_epochs=True,
+            noise_range_t=None,
+            noise_pct=0.67,
+            noise_std=1.0,
+            noise_seed=42,
+            k_decay=1.0,
+            initialize=True
+    ) -> None:
         super().__init__(
-            optimizer, param_group_field="lr",
+            optimizer, param_group_field="lr", t_in_epochs=t_in_epochs,
             noise_range_t=noise_range_t, noise_pct=noise_pct, noise_std=noise_std, noise_seed=noise_seed,
-            initialize=initialize)
+            initialize=initialize
+        )
 
         assert t_initial > 0
         assert lr_min >= 0
         if t_initial == 1 and cycle_mul == 1 and cycle_decay == 1:
-            _logger.warning("Cosine annealing scheduler will have no effect on the learning "
-                            "rate since t_initial = t_mul = eta_mul = 1.")
+            logger.warning("Cosine annealing scheduler will have no effect on the learning "
+                           "rate since t_initial = t_mul = eta_mul = 1.")
         self.t_initial = t_initial
         self.power = power
         self.lr_min = lr_min
         self.cycle_mul = cycle_mul
         self.cycle_decay = cycle_decay
         self.cycle_limit = cycle_limit
         self.warmup_t = warmup_t
         self.warmup_lr_init = warmup_lr_init
         self.warmup_prefix = warmup_prefix
-        self.t_in_epochs = t_in_epochs
         self.k_decay = k_decay
         if self.warmup_t:
             self.warmup_steps = [(v - warmup_lr_init) / self.warmup_t for v in self.base_values]
             super().update_groups(self.warmup_lr_init)
         else:
             self.warmup_steps = [1 for _ in self.base_values]
 
@@ -92,25 +91,13 @@
                     for lr_max in lr_max_values
                 ]
             else:
                 lrs = [self.lr_min for _ in self.base_values]
 
         return lrs
 
-    def get_epoch_values(self, epoch: int):
-        if self.t_in_epochs:
-            return self._get_lr(epoch)
-        else:
-            return None
-
-    def get_update_values(self, num_updates: int):
-        if not self.t_in_epochs:
-            return self._get_lr(num_updates)
-        else:
-            return None
-
     def get_cycle_length(self, cycles=0):
         cycles = max(1, cycles or self.cycle_limit)
         if self.cycle_mul == 1.0:
             return self.t_initial * cycles
         else:
             return int(math.floor(-self.t_initial * (self.cycle_mul ** cycles - 1) / (1 - self.cycle_mul)))
```

## tepe/modules/scheduler/scheduler.py

```diff
@@ -1,13 +1,15 @@
-from typing import Dict, Any
+import abc
+from abc import ABC
+from typing import Any, Dict, Optional
 
 import torch
 
 
-class Scheduler:
+class Scheduler(ABC):
     """ Parameter Scheduler Base Class
     A scheduler base class that can be used to schedule any optimizer parameter groups.
 
     Unlike the builtin PyTorch schedulers, this is intended to be consistently called
     * At the END of each epoch, before incrementing the epoch count, to calculate next epoch's value
     * At the END of each optimizer update, after incrementing the update count, to calculate next update's value
 
@@ -18,88 +20,108 @@
     code and explicitly passed in to the schedulers on the corresponding step or step_update call.
 
     Based on ideas from:
      * https://github.com/pytorch/fairseq/tree/master/fairseq/optim/lr_scheduler
      * https://github.com/allenai/allennlp/tree/master/allennlp/training/learning_rate_schedulers
     """
 
-    def __init__(self,
-                 optimizer: torch.optim.Optimizer,
-                 param_group_field: str,
-                 noise_range_t=None,
-                 noise_type='normal',
-                 noise_pct=0.67,
-                 noise_std=1.0,
-                 noise_seed=None,
-                 initialize: bool = True) -> None:
+    def __init__(
+            self,
+            optimizer: torch.optim.Optimizer,
+            param_group_field: str,
+            t_in_epochs: bool = True,
+            noise_range_t=None,
+            noise_type='normal',
+            noise_pct=0.67,
+            noise_std=1.0,
+            noise_seed=None,
+            initialize: bool = True,
+    ) -> None:
         self.optimizer = optimizer
         self.param_group_field = param_group_field
         self._initial_param_group_field = f"initial_{param_group_field}"
         if initialize:
             for i, group in enumerate(self.optimizer.param_groups):
                 if param_group_field not in group:
                     raise KeyError(f"{param_group_field} missing from param_groups[{i}]")
                 group.setdefault(self._initial_param_group_field, group[param_group_field])
         else:
             for i, group in enumerate(self.optimizer.param_groups):
                 if self._initial_param_group_field not in group:
                     raise KeyError(f"{self._initial_param_group_field} missing from param_groups[{i}]")
         self.base_values = [group[self._initial_param_group_field] for group in self.optimizer.param_groups]
         self.metric = None  # any point to having this for all?
+        self.t_in_epochs = t_in_epochs
         self.noise_range_t = noise_range_t
         self.noise_pct = noise_pct
         self.noise_type = noise_type
         self.noise_std = noise_std
         self.noise_seed = noise_seed if noise_seed is not None else 42
         self.update_groups(self.base_values)
 
     def state_dict(self) -> Dict[str, Any]:
         return {key: value for key, value in self.__dict__.items() if key != 'optimizer'}
 
     def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
         self.__dict__.update(state_dict)
 
-    def get_epoch_values(self, epoch: int):
-        return None
-
-    def get_update_values(self, num_updates: int):
-        return None
+    @abc.abstractmethod
+    def _get_lr(self, t: int) -> float:
+        pass
+
+    def _get_values(self, t: int, on_epoch: bool = True) -> Optional[float]:
+        proceed = (on_epoch and self.t_in_epochs) or (not on_epoch and not self.t_in_epochs)
+        if not proceed:
+            return None
+        return self._get_lr(t)
 
     def step(self, epoch: int, metric: float = None) -> None:
         self.metric = metric
-        values = self.get_epoch_values(epoch)
+        values = self._get_values(epoch, on_epoch=True)
         if values is not None:
             values = self._add_noise(values, epoch)
             self.update_groups(values)
 
     def step_update(self, num_updates: int, metric: float = None):
         self.metric = metric
-        values = self.get_update_values(num_updates)
+        values = self._get_values(num_updates, on_epoch=False)
         if values is not None:
             values = self._add_noise(values, num_updates)
             self.update_groups(values)
 
     def update_groups(self, values):
         if not isinstance(values, (list, tuple)):
             values = [values] * len(self.optimizer.param_groups)
         for param_group, value in zip(self.optimizer.param_groups, values):
-            param_group[self.param_group_field] = value
+            if 'lr_scale' in param_group:
+                param_group[self.param_group_field] = value * param_group['lr_scale']
+            else:
+                param_group[self.param_group_field] = value
 
     def _add_noise(self, lrs, t):
+        if self._is_apply_noise(t):
+            noise = self._calculate_noise(t)
+            lrs = [v + v * noise for v in lrs]
+        return lrs
+
+    def _is_apply_noise(self, t) -> bool:
+        """Return True if scheduler in noise range."""
+        apply_noise = False
         if self.noise_range_t is not None:
             if isinstance(self.noise_range_t, (list, tuple)):
                 apply_noise = self.noise_range_t[0] <= t < self.noise_range_t[1]
             else:
                 apply_noise = t >= self.noise_range_t
-            if apply_noise:
-                g = torch.Generator()
-                g.manual_seed(self.noise_seed + t)
-                if self.noise_type == 'normal':
-                    while True:
-                        # resample if noise out of percent limit, brute force but shouldn't spin much
-                        noise = torch.randn(1, generator=g).item()
-                        if abs(noise) < self.noise_pct:
-                            break
-                else:
-                    noise = 2 * (torch.rand(1, generator=g).item() - 0.5) * self.noise_pct
-                lrs = [v + v * noise for v in lrs]
-        return lrs
+        return apply_noise
+
+    def _calculate_noise(self, t) -> float:
+        g = torch.Generator()
+        g.manual_seed(self.noise_seed + t)
+        if self.noise_type == 'normal':
+            while True:
+                # resample if noise out of percent limit, brute force but shouldn't spin much
+                noise = torch.randn(1, generator=g).item()
+                if abs(noise) < self.noise_pct:
+                    return noise
+        else:
+            noise = 2 * (torch.rand(1, generator=g).item() - 0.5) * self.noise_pct
+        return noise
```

## tepe/modules/scheduler/step_lr.py

```diff
@@ -10,54 +10,53 @@
 from .scheduler import Scheduler
 
 
 class StepLRScheduler(Scheduler):
     """
     """
 
-    def __init__(self,
-                 optimizer: torch.optim.Optimizer,
-                 decay_t: float,
-                 decay_rate: float = 1.,
-                 warmup_t=0,
-                 warmup_lr_init=0,
-                 t_in_epochs=True,
-                 noise_range_t=None,
-                 noise_pct=0.67,
-                 noise_std=1.0,
-                 noise_seed=42,
-                 initialize=True,
-                 ) -> None:
+    def __init__(
+            self,
+            optimizer: torch.optim.Optimizer,
+            decay_t: float,          # 下降间隔
+            decay_rate: float = 1.,  # 每次下降率
+            warmup_t=0,              # warmup间隔，0说明不进行warmup
+            warmup_lr_init=0,        # warmup初始lr
+            warmup_prefix=True,      # True-第一次更新的间隔中包含warmup阶段
+            t_in_epochs=True,        # 按epoch更新
+            noise_range_t=None,      # 添加噪声开始、结束范围
+            noise_pct=0.67,          # 控制噪声的大小
+            noise_std=1.0,           # 
+            noise_seed=42,
+            initialize=True,         # 在优化器的group_param中加入'initial_lr'字段
+    ) -> None:
         super().__init__(
-            optimizer, param_group_field="lr",
-            noise_range_t=noise_range_t, noise_pct=noise_pct, noise_std=noise_std, noise_seed=noise_seed,
-            initialize=initialize)
+            optimizer, 
+            param_group_field="lr", 
+            t_in_epochs=t_in_epochs,
+            noise_range_t=noise_range_t, 
+            noise_pct=noise_pct, 
+            noise_std=noise_std, 
+            noise_seed=noise_seed,
+            initialize=initialize
+        )
 
         self.decay_t = decay_t
         self.decay_rate = decay_rate
         self.warmup_t = warmup_t
         self.warmup_lr_init = warmup_lr_init
-        self.t_in_epochs = t_in_epochs
+        self.warmup_prefix = warmup_prefix
         if self.warmup_t:
+            # warmup阶段，每次更新时lr增加量
             self.warmup_steps = [(v - warmup_lr_init) / self.warmup_t for v in self.base_values]
             super().update_groups(self.warmup_lr_init)
         else:
             self.warmup_steps = [1 for _ in self.base_values]
 
     def _get_lr(self, t):
         if t < self.warmup_t:
             lrs = [self.warmup_lr_init + t * s for s in self.warmup_steps]
         else:
+            if self.warmup_prefix:
+                t = t - self.warmup_t
             lrs = [v * (self.decay_rate ** (t // self.decay_t)) for v in self.base_values]
-        return lrs
-
-    def get_epoch_values(self, epoch: int):
-        if self.t_in_epochs:
-            return self._get_lr(epoch)
-        else:
-            return None
-
-    def get_update_values(self, num_updates: int):
-        if not self.t_in_epochs:
-            return self._get_lr(num_updates)
-        else:
-            return None
+        return lrs
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## tepe/modules/scheduler/tanh_lr.py

```diff
@@ -1,52 +1,52 @@
 """ TanH Scheduler
 
 TanH schedule with warmup, cycle/restarts, noise.
 
 Hacked together by / Copyright 2021 Ross Wightman
 """
-import logging
+from loguru import logger
 import math
 import numpy as np
 import torch
 
 from .scheduler import Scheduler
 
 
-_logger = logging.getLogger(__name__)
-
-
 class TanhLRScheduler(Scheduler):
     """
     Hyberbolic-Tangent decay with restarts.
     This is described in the paper https://arxiv.org/abs/1806.01593
     """
 
-    def __init__(self,
-                 optimizer: torch.optim.Optimizer,
-                 t_initial: int,
-                 lb: float = -7.,
-                 ub: float = 3.,
-                 lr_min: float = 0.,
-                 cycle_mul: float = 1.,
-                 cycle_decay: float = 1.,
-                 cycle_limit: int = 1,
-                 warmup_t=0,
-                 warmup_lr_init=0,
-                 warmup_prefix=False,
-                 t_in_epochs=True,
-                 noise_range_t=None,
-                 noise_pct=0.67,
-                 noise_std=1.0,
-                 noise_seed=42,
-                 initialize=True) -> None:
+    def __init__(
+            self,
+            optimizer: torch.optim.Optimizer,
+            t_initial: int,
+            lb: float = -7.,
+            ub: float = 3.,
+            lr_min: float = 0.,
+            cycle_mul: float = 1.,
+            cycle_decay: float = 1.,
+            cycle_limit: int = 1,
+            warmup_t=0,
+            warmup_lr_init=0,
+            warmup_prefix=False,
+            t_in_epochs=True,
+            noise_range_t=None,
+            noise_pct=0.67,
+            noise_std=1.0,
+            noise_seed=42,
+            initialize=True
+    ) -> None:
         super().__init__(
-            optimizer, param_group_field="lr",
+            optimizer, param_group_field="lr", t_in_epochs=t_in_epochs,
             noise_range_t=noise_range_t, noise_pct=noise_pct, noise_std=noise_std, noise_seed=noise_seed,
-            initialize=initialize)
+            initialize=initialize
+        )
 
         assert t_initial > 0
         assert lr_min >= 0
         assert lb < ub
         assert cycle_limit >= 0
         assert warmup_t >= 0
         assert warmup_lr_init >= 0
@@ -56,15 +56,14 @@
         self.lr_min = lr_min
         self.cycle_mul = cycle_mul
         self.cycle_decay = cycle_decay
         self.cycle_limit = cycle_limit
         self.warmup_t = warmup_t
         self.warmup_lr_init = warmup_lr_init
         self.warmup_prefix = warmup_prefix
-        self.t_in_epochs = t_in_epochs
         if self.warmup_t:
             t_v = self.base_values if self.warmup_prefix else self._get_lr(self.warmup_t)
             self.warmup_steps = [(v - warmup_lr_init) / self.warmup_t for v in t_v]
             super().update_groups(self.warmup_lr_init)
         else:
             self.warmup_steps = [1 for _ in self.base_values]
 
@@ -93,25 +92,13 @@
                     self.lr_min + 0.5 * (lr_max - self.lr_min) * (1 - math.tanh(self.lb * (1. - tr) + self.ub * tr))
                     for lr_max in lr_max_values
                 ]
             else:
                 lrs = [self.lr_min for _ in self.base_values]
         return lrs
 
-    def get_epoch_values(self, epoch: int):
-        if self.t_in_epochs:
-            return self._get_lr(epoch)
-        else:
-            return None
-
-    def get_update_values(self, num_updates: int):
-        if not self.t_in_epochs:
-            return self._get_lr(num_updates)
-        else:
-            return None
-
     def get_cycle_length(self, cycles=0):
         cycles = max(1, cycles or self.cycle_limit)
         if self.cycle_mul == 1.0:
             return self.t_initial * cycles
         else:
             return int(math.floor(-self.t_initial * (self.cycle_mul ** cycles - 1) / (1 - self.cycle_mul)))
```

## tepe/tasks/cfa/module.py

```diff
@@ -117,16 +117,16 @@
         L_rep  = (1/self.nu) * torch.mean(torch.max(torch.zeros_like(score), score - self.alpha))
         
         loss = L_att + L_rep
 
         return loss 
 
     def init_centroid(self, model, data_loader):
-        for i, data in enumerate(tqdm(data_loader)):
-            x = data['img'].to(self.device)
+        for i, (x, _, _) in enumerate(tqdm(data_loader)):
+            x = x.to(self.device)
             feats = model(x)
             if self.leaky:
                 p = []
                 for v in feats.values():
                     p.append(F.leaky_relu(v))
             else:
                 p = feats
```

## tepe/tasks/cfa/task.py

```diff
@@ -179,18 +179,17 @@
 
         # train loop
         logger.info(f'class: {self.scene}')
         self.weights = f'{save_dir}/{self.encoder_name}_cfa_{self.scene}.pth'
 
         for epoch in range(1, self.max_epoch + 1):
             loss_list = []
-            for data in train_loader:
-                x = data['img'].to(self.device)
+            for (x, _, _) in train_loader:
                 optimizer.zero_grad()
-                loss, _ = model(x)
+                loss, _ = model(x.to(self.device))
 
                 loss.backward()
                 optimizer.step()
                 loss_list.append(loss.item())
             logger.info('epoch [{}/{}], loss:{:.4f}'.format(epoch, self.max_epoch, np.mean(loss_list)))
             # save model
             if epoch % 5 == 0 or epoch == self.max_epoch:
```

## tepe/tasks/rd/de_resnet.py

```diff
@@ -4,17 +4,17 @@
 try:
     from torch.hub import load_state_dict_from_url
 except ImportError:
     from torch.utils.model_zoo import load_url as load_state_dict_from_url
 from typing import Type, Any, Callable, Union, List, Optional
 
 
-__all__ = ['ResNet', 'de_resnet18', 'de_resnet34', 'de_resnet50', 'resnet101',
+__all__ = ['ResNet', 'resnet18', 'resnet34', 'resnet50', 'resnet101',
            'resnet152', 'resnext50_32x4d', 'resnext101_32x8d',
-           'de_wide_resnet50_2', 'de_wide_resnet101_2']
+           'wide_resnet50_2', 'wide_resnet101_2']
 
 
 model_urls = {
     'resnet18': 'https://download.pytorch.org/models/resnet18-f37072fd.pth',
     'resnet34': 'https://download.pytorch.org/models/resnet34-b627a593.pth',
     'resnet50': 'https://download.pytorch.org/models/resnet50-0676ba61.pth',
     'resnet101': 'https://download.pytorch.org/models/resnet101-63fe2227.pth',
```

## tepe/tasks/rd/evalutor.py

```diff
@@ -1,264 +1,22 @@
-import glob
+import numpy as np
 import os
-from statistics import mean
+import glob
 
-import numpy as np
-import pandas as pd
 import torch
-import torch.nn.functional as F
-from numpy import ndarray
-from matplotlib import pyplot as plt
-from scipy.ndimage import gaussian_filter
-from skimage import measure
-from skimage.measure import label, regionprops
-from sklearn.metrics import roc_auc_score, auc, precision_recall_curve, roc_curve
-from torch.utils.data import DataLoader
-from tqdm import tqdm
-
-from tepe.data.datasets import AnomalyDataset
-from tepe.data.voc_xml import PascalVocReader
-
-
-def roc_auc_img(gt, score):
-    img_roc_auc = roc_auc_score(gt, score)
-
-    return img_roc_auc
-
-def roc_auc_pxl(gt, score):
-    per_pixel_roc_auc = roc_auc_score(gt.flatten(), score.flatten())
-
-    return per_pixel_roc_auc
-
-
-def pro_auc_pxl(gt, score):
-    gt = np.squeeze(gt, axis=1)
-
-    gt[gt <= 0.5] = 0
-    gt[gt > 0.5] = 1
-    gt = gt.astype(np.bool)
-
-    max_step = 200
-    expect_fpr = 0.3
-
-    max_th = score.max()
-    min_th = score.min()
-    delta = (max_th - min_th) / max_step
-
-    pros_mean = []
-    pros_std = []
-    threds = []
-    fprs = []
-
-    binary_score_maps = np.zeros_like(score, dtype=np.bool)
-
-    for step in range(max_step):
-        thred = max_th - step * delta
-        binary_score_maps[score <= thred] = 0
-        binary_score_maps[score > thred] = 1
-
-        pro = []
-        for i in range(len(binary_score_maps)):
-            label_map = label(gt[i], connectivity=2)
-            props = regionprops(label_map, binary_score_maps[i])
-
-            for prop in props:
-                pro.append(prop.intensity_image.sum() / prop.area)
-
-        pros_mean.append(np.array(pro).mean())
-        pros_std.append(np.array(pro).std())
-
-        gt_neg = ~gt
-        fpr = np.logical_and(gt_neg, binary_score_maps).sum() / gt_neg.sum()
-        fprs.append(fpr)
-        threds.append(thred)
-
-    threds = np.array(threds)
-    pros_mean = np.array(pros_mean)
-    pros_std = np.array(pros_std)
-    fprs = np.array(fprs)
-
-    idx = fprs <= expect_fpr
-    fprs_selected = fprs[idx]
-    fprs_selected = rescale(fprs_selected)
-    pros_mean_selected = rescale(pros_mean[idx])
-    per_pixel_roc_auc = auc(fprs_selected, pros_mean_selected)
-
-    return per_pixel_roc_auc
-
-
-def rescale(x):
-    return (x - x.min()) / (x.max() - x.min())
-
-
-def get_threshold(gt, score):
-    gt_mask = np.asarray(gt)
-    precision, recall, thresholds = precision_recall_curve(gt_mask.flatten(), score.flatten())
-    a = 2 * precision * recall
-    b = precision + recall
-    f1 = np.divide(a, b, out=np.zeros_like(a), where=b != 0)
-    threshold = thresholds[np.argmax(f1)]
-
-    return threshold
-
-
-def cal_img_roc(scores, gt_list):
-    img_scores = scores.reshape(scores.shape[0], -1).max(axis=1)
-    gt_list = np.asarray(gt_list)
-
-    fpr, tpr, _ = roc_curve(gt_list, img_scores)
-    img_roc_auc = roc_auc_img(gt_list, img_scores)
+from tepe.data.annotation import PascalVocReader
 
-    return fpr, tpr, img_roc_auc
 
-
-def cal_pxl_roc(gt_mask, scores):
-    fpr, tpr, _ = roc_curve(gt_mask.flatten(), scores.flatten())
-    per_pixel_rocauc = roc_auc_pxl(gt_mask.flatten(), scores.flatten())
-
-    return fpr, tpr, per_pixel_rocauc
-
-
-def cal_pxl_pro(gt_mask, scores):
-    per_pixel_proauc = pro_auc_pxl(gt_mask, scores)
-
-    return per_pixel_proauc
-
-
-def mvtec_eval(task):
-    data_transform, target_transform = task.get_transform(mode='val')
-
-    dataset = AnomalyDataset(task.data_root, class_name=task.scene,
-                             transform=data_transform, target_transform=target_transform,
-                             resize=task.input_size, is_train=False, is_mvtec=True,
-                             cache_img=task.cache)
-
-    dataloader = DataLoader(
-        dataset, batch_size=task.batch_size, shuffle=False, num_workers=task.workers
-    )
-
-    model = task.get_model(train=False)
-
-    fig, ax = plt.subplots(1, 2, figsize=(20, 10))
-    fig_img_rocauc = ax[0]
-    fig_pixel_rocauc = ax[1]
-
-
-    gt_list = []
-    gt_mask_list = []
-    anomaly_maps = []
-
-    for data in tqdm(dataloader):
-        img, gt, label = data['img'], data['mask'], data['target']
-        img = img.to(task.device)
-
-        gt_list.extend(label.cpu().detach().numpy())
-        gt_mask_list.extend(gt.cpu().detach().numpy())
-        with torch.no_grad():
-            anomaly_map = model(img)
-        anomaly_maps.append(anomaly_map)
-
-    anomaly_maps = torch.cat(anomaly_maps, dim=0).cpu().detach().numpy()
-    for i in range(anomaly_maps.shape[0]):
-        anomaly_maps[i] = gaussian_filter(anomaly_maps[i], sigma=8)
-
-    gt_mask = np.asarray(gt_mask_list)
-    # rescale
-
-    r'Image-level AUROC'
-    fpr, tpr, img_roc_auc = cal_img_roc(anomaly_maps, gt_list)
-    fig_img_rocauc.plot(fpr, tpr, label='%s img_ROCAUC: %.3f' % (task.scene, img_roc_auc))
-    fig_img_rocauc.set_xlabel('fpr')
-    fig_img_rocauc.set_ylabel('tpr')
-    fig_img_rocauc.title.set_text('image ROCAUC')
-    fig_img_rocauc.legend(loc="lower right")
-
-    r'Pixel-level AUROC'
-    fpr, tpr, per_pixel_rocauc = cal_pxl_roc(gt_mask, anomaly_maps)
-    fig_pixel_rocauc.plot(fpr, tpr, label='%s ROCAUC: %.3f' % (task.scene, per_pixel_rocauc))
-    fig_pixel_rocauc.set_xlabel('fpr')
-    fig_pixel_rocauc.set_ylabel('tpr')
-    fig_pixel_rocauc.title.set_text('pixel ROCAUC')
-    fig_pixel_rocauc.legend(loc="lower right")
-
-    r'Pixel-level AUPRO'
-    per_pixel_proauc = cal_pxl_pro(gt_mask, anomaly_maps)
-
-    # print('image ROCAUC: %.3f'% (img_roc_auc))
-    # print('pixel ROCAUC: %.3f'% (per_pixel_rocauc))
-    # print('pixel PROAUC: %.3f'% (per_pixel_proauc))
-
-    fig.tight_layout()
-    fig.savefig(os.path.join(task.output_dir, task.scene, 'roc_curve.png'), dpi=100)
-
-    return dict(img_rocauc=img_roc_auc, pixel_rocauc=per_pixel_rocauc, pixel_proauc=per_pixel_proauc)
-
-
-def compute_pro(masks: ndarray, amaps: ndarray, num_th: int = 200) -> None:
-
-    """Compute the area under the curve of per-region overlaping (PRO) and 0 to 0.3 FPR
-    Args:
-        category (str): Category of product
-        masks (ndarray): All binary masks in test. masks.shape -> (num_test_data, h, w)
-        amaps (ndarray): All anomaly maps in test. amaps.shape -> (num_test_data, h, w)
-        num_th (int, optional): Number of thresholds
-    """
-
-    assert isinstance(amaps, ndarray), "type(amaps) must be ndarray"
-    assert isinstance(masks, ndarray), "type(masks) must be ndarray"
-    assert amaps.ndim == 3, "amaps.ndim must be 3 (num_test_data, h, w)"
-    assert masks.ndim == 3, "masks.ndim must be 3 (num_test_data, h, w)"
-    assert amaps.shape == masks.shape, "amaps.shape and masks.shape must be same"
-    assert set(masks.flatten()) == {0, 1}, "set(masks.flatten()) must be {0, 1}"
-    assert isinstance(num_th, int), "type(num_th) must be int"
-
-    df = pd.DataFrame([], columns=["pro", "fpr", "threshold"])
-    binary_amaps = np.zeros_like(amaps, dtype=np.bool)
-
-    min_th = amaps.min()
-    max_th = amaps.max()
-    delta = (max_th - min_th) / num_th
-
-    for th in np.arange(min_th, max_th, delta):
-        binary_amaps[amaps <= th] = 0
-        binary_amaps[amaps > th] = 1
-
-        pros = []
-        for binary_amap, mask in zip(binary_amaps, masks):
-            for region in measure.regionprops(measure.label(mask)):
-                axes0_ids = region.coords[:, 0]
-                axes1_ids = region.coords[:, 1]
-                tp_pixels = binary_amap[axes0_ids, axes1_ids].sum()
-                pros.append(tp_pixels / region.area)
-
-        inverse_masks = 1 - masks
-        fp_pixels = np.logical_and(inverse_masks, binary_amaps).sum()
-        fpr = fp_pixels / inverse_masks.sum()
-
-        df = df.append({"pro": mean(pros), "fpr": fpr, "threshold": th}, ignore_index=True)
-
-    # Normalize FPR from 0 ~ 1 to 0 ~ 0.3
-    df = df[df["fpr"] < 0.3]
-    df["fpr"] = df["fpr"] / df["fpr"].max()
-
-    pro_auc = auc(df["fpr"], df["pro"])
-    return pro_auc
-
-
-def read_xml(xml_path, limit_label=()):
+def read_xml(xml_path):
     reader = PascalVocReader(xml_path)
     anno_bboxes = reader.get_bbox()
     bboxes = []
     for anno in anno_bboxes:
         label, box = anno.get('name'), anno.get('bndbox')
-        if limit_label:
-            if label in limit_label:
-                bboxes.append(box)
-        else:
-            bboxes.append(box)
+        bboxes.append(box)
 
     return torch.tensor(bboxes)
 
 
 def box_iou(box1, box2):
     """
     Return intersection-over-union (Jaccard index) of boxes.
@@ -282,49 +40,44 @@
     inter = (torch.min(box1[:, None, 2:], box2[:, 2:]) - torch.max(box1[:, None, :2], box2[:, :2])).clamp(0).prod(2)
     return inter / (area1[:, None] + area2 - inter)  # iou = inter / (area1 + area2 - inter)
 
 
 def cal_true_positive(gt, pred, iou_thr=0.001):
     num_pred = len(pred)
     num_gt = len(gt)
-    p_tp, r_tp = 0, 0
+    tp = 0
     if num_gt > 0 and num_pred > 0:
-        ious = box_iou(gt, pred)  # h: num_gt, w: num_pred
-        for iou in ious:  # 对于每个GT
-            r_tp += int((iou > iou_thr).sum() > 0)  # 只要有重叠即为检出
-
-        ious = ious.T
-        for iou in ious:  # 对于每个Pred
-            p_tp += int((iou > iou_thr).sum() > 0)  # 只要有重叠即为预测正确
+        iou = box_iou(gt, pred)
+        x = torch.where((iou >= iou_thr))
 
-    return p_tp, r_tp
+        if len(x) > 0:
+            x = x[1].numpy()
+            tp = len(np.unique(x))
+
+    tp = num_gt if tp > num_gt else tp
+    return tp
 
 
 if __name__ == '__main__':
-    pred_dir = '/home/zepei/workspace/ad-tepe/outputs/rd_bjguo_101_1110/bjguo/xml_predict'
-    label_idr = '/home/zepei/DATA/lenovo_anomaly/bjguo/ground_truth/bad'
+    pred_dir = '/home/zepei/workspace/tepe/outputs/rd_bguo_221024/bguo/predict'
+    label_idr = '/home/zepei/DATA/lenovo_anomaly/bguo/ground_truth/yiwu3'
 
-    total_pred, total_gt, total_rtp, total_ptp = 0, 0, 0, 0
+    total_pred, total_gt, total_tp = 0, 0, 0
     for pred_xml_path in glob.glob(os.path.join(pred_dir, '*.xml')):
-        if '22273' in pred_xml_path: # or '32428' in pred_xml_path:
-
-            xml_name = os.path.basename(pred_xml_path)
-            label_xml_path = os.path.join(label_idr, xml_name)
+        xml_name = os.path.basename(pred_xml_path)
+        label_xml_path = os.path.join(label_idr, xml_name)
 
-            pred = read_xml(pred_xml_path)
-            gt = read_xml(label_xml_path)
+        pred = read_xml(pred_xml_path)
+        gt = read_xml(label_xml_path)
 
-            num_pred = len(pred)
-            num_gt = len(gt)
-            p_tp, r_tp = cal_true_positive(gt, pred, iou_thr=0.00001)
-
-            total_pred += num_pred
-            total_gt += num_gt
-            total_rtp += r_tp
-            total_ptp += p_tp
-            print(r_tp, p_tp, num_gt, num_pred)
-            print(f'{pred_xml_path}')
+        num_pred = len(pred)
+        num_gt = len(gt)
+        tp = cal_true_positive(gt, pred)
+
+        total_pred += num_pred
+        total_gt += num_gt
+        total_tp += tp
 
-    precision = total_ptp / total_pred
-    recall = total_rtp / total_gt
+    precision = total_tp / total_pred
+    recall = total_tp / total_gt
 
     print('精度， 召回：', precision, recall)
```

## tepe/tasks/rd/find_thr.py

```diff
@@ -1,80 +1,57 @@
-from loguru import logger
 import numpy as np
 import torch
 from scipy.ndimage import gaussian_filter
 from torch.nn import functional as F
 from tqdm import tqdm
 
+'''
+找个阈值
+encoder, bn, decoder:三个模型
+good_loader, bad_loader:训练样本的loader, 训练样本贴图后的loader
+
+thr计算方式: (mean(正常样本的分数)+mean(异常样本分数))/2
+
+return: thr <float>
+'''
+
 
 def find(model, good_loader, bad_loader, device):
-    '''
-    找个阈值, thr计算方式: (mean(正常样本的分数)+mean(异常样本分数))/2
-    model:
-    good_loader, bad_loader:训练样本的loader, 训练样本贴图后的loader
-    return: thr <float>
-    '''
+
     model.eval()
     gt_list_sp = []
     pr_list_sp = []
     #
     most = 40
     i = 0
 
     with torch.no_grad():
-        for data in tqdm(good_loader):
+        for img, _, _ in tqdm(good_loader):
             i = i + 1
             if i > most:
                 break
-            img = data['img'].to(device)
+            img = img.to(device)
             anomaly_map = model(img)
             anomaly_map = anomaly_map.cpu().detach().numpy()
             anomaly_map = gaussian_filter(anomaly_map, sigma=4)  # [256,256]
 
             gt_list_sp.append(0)  # 一个值
             pr_list_sp.append(np.max(anomaly_map))
         i = 0
-        for data in tqdm(bad_loader):
+        for img, _, _ in tqdm(bad_loader):
             i = i + 1
             if i > most:
                 break
-            img = data['img'].to(device)
+            img = img.to(device)
             anomaly_map = model(img)
             anomaly_map = anomaly_map.cpu().detach().numpy()
             anomaly_map = gaussian_filter(anomaly_map, sigma=4)  # [256,256]
 
             gt_list_sp.append(1)  # 一个值
             pr_list_sp.append(np.max(anomaly_map))
 
         gt_list_sp = np.array(gt_list_sp)
         pr_list_sp = np.array(pr_list_sp)
 
         # thr=compare(gt_list_sp=gt_list_sp, pr_list_sp=pr_list_sp)
         thr = (np.mean(pr_list_sp[np.where(gt_list_sp == 0)]) + np.mean(pr_list_sp[np.where(gt_list_sp == 1)])) / 2
-    return thr
-
-
-def find_hard_samples(model, dataloader, device, mining_thr=0.3):
-    model.eval()
-
-    select_paths = []
-    for data in dataloader:
-        img = data['img'].to(device)
-        
-        with torch.no_grad():
-            anomaly_map = model(img)
-            anomaly_values = anomaly_map.view(anomaly_map.shape[0], -1)
-
-            # hard_pixels = (anomaly_values > mining_thr).sum(dim=1)  # 每个样本中大于mining_thr的像素数量
-            # select_indices = torch.where(hard_pixels > 16)  # 寻找大于4x4 pixel的样本索引
-            
-            max_values = anomaly_values.max(dim=1)  # max value and loc index of per sample
-            select_indices = torch.where(max_values[0] > mining_thr)[0].cpu().detach().numpy()
-            
-        paths = np.array(data['path'])
-
-        select_path = paths[select_indices]
-        select_paths.append(select_path)
-
-    select_paths = np.concatenate(select_paths)
-
-    return list(select_paths)
+    return thr
```

## tepe/tasks/rd/model.py

```diff
@@ -1,33 +1,26 @@
 import numpy as np
 import torch
 from torch import nn
 from torch.nn import functional as F
 
-from tepe.tasks.rd.resnet import wide_resnet50_2, wide_resnet101_2
-from tepe.tasks.rd.de_resnet import de_wide_resnet50_2, de_wide_resnet101_2
+from tepe.tasks.rd.resnet import wide_resnet50_2
+from tepe.tasks.rd.de_resnet import de_wide_resnet50_2
 
 
 class Model(nn.Module):
-    def __init__(self, encoder_name, input_size=(256, 256)):
+    def __init__(self):
         super().__init__()
-        if encoder_name == 'wres50':
-            self.encoder, self.bn = wide_resnet50_2(pretrained=True)
-            self.decoder = de_wide_resnet50_2(pretrained=False)
-        elif encoder_name == 'wres101':
-            self.encoder, self.bn = wide_resnet101_2(pretrained=True)
-            self.decoder = de_wide_resnet101_2(pretrained=False)
-        else:
-            raise NotImplementedError
+        self.encoder, self.bn = wide_resnet50_2(pretrained=True)
+        self.decoder = de_wide_resnet50_2(pretrained=False)
 
         # loss
         # self.mse_loss = torch.nn.MSELoss()
         self.cos_loss = nn.CosineSimilarity()
 
-        self.input_size = input_size
         self.export = False
 
     def forward(self, x):
         x1 = self.encoder(x)
         x2 = self.decoder(self.bn(x1))
 
         if self.training:
@@ -41,32 +34,32 @@
             # loss += 0.1*self.mse_loss(a[item], b[item])
             loss += torch.mean(1 - self.cos_loss(a[item].view(a[item].shape[0], -1),
                                                  b[item].view(b[item].shape[0], -1)))
         return loss
 
     def cal_anomaly_map(self, fs_list, ft_list, amap_mode='add'):
         '''
-        fs_list: sdudent model feature
-        ft_list: teacher model feature
+        fs_list：[[1,1024,16,16]]
         '''
         a_map_list = []
-        # max_shape = [64, 64]
+        max_shape = [64, 64]
         for item in range(len(ft_list)):
-            # if item == 0:
-            #     max_shape = [4 * int(fs_list[item].shape[2]), 4 * int(fs_list[item].shape[3])]
+            if item == 0:
+                max_shape = [4 * int(fs_list[item].shape[2]), 4 * int(fs_list[item].shape[3])]
+
             # a_map = 1 - self.cos_loss(fs_list[item], ft_list[item]) # [1,16,16]
             # onnx don't support nn.CosineSimilarity
             a_map = 1 - cosine_similarity(fs_list[item], ft_list[item])
             a_map = torch.unsqueeze(a_map, dim=1)#[1,1,16,16]
-            a_map = F.interpolate(a_map, size=self.input_size, mode='bilinear', align_corners=False)
+            a_map = F.interpolate(a_map, size=max_shape, mode='bilinear', align_corners=False)
+            a_map = a_map[0, 0, :, :]
             a_map_list.append(a_map)
 
-        a_maps = torch.cat(a_map_list, dim=1)  # [B,3,256,256]
-        anomaly_map = torch.sum(a_maps, dim=1)  # [B,256,256]
-
+        a_maps = torch.stack(a_map_list)  # [3, 64, 64]
+        anomaly_map = torch.sum(a_maps, dim=0)
         return anomaly_map
 
 
 def cosine_similarity(a: torch.Tensor, b: torch.Tensor, eps: float = 1e-8) -> torch.Tensor:
     frac1 = torch.sum(torch.mul(a, b), dim=1)
     a_norm = torch.norm(a, p=2, dim=1)
     b_norm = torch.norm(b, p=2, dim=1)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## tepe/tasks/rd/predictor.py

```diff
@@ -3,267 +3,158 @@
 from scipy import ndimage as ndi
 import cv2
 import numpy as np
 import torch
 import torchvision
 from loguru import logger
 from matplotlib import pyplot as plt
-from scipy.ndimage import gaussian_filter
+from scipy.ndimage import gaussian_filter, maximum_filter
 
 from skimage.feature import peak_local_max
-from skimage import data, img_as_float, morphology
+from skimage import data, img_as_float
 
 from tepe.core import Predictor as BasePredictor
 from tepe.core.predictor.anomaly_detector import AnomalyDetector
 from tepe.tasks.cfa.utils import denormalization
-from tepe.tasks.rd.utils import rectMerge_sxf, check_rect_contain_point
 from tepe.utils import increment_path
 
 
 class Predictor(BasePredictor, AnomalyDetector):
     def __init__(
             self,
             model: torch.nn.Module,
             input_size: int or tuple or list,
             resize_fn: Optional[Callable] = None,
             threshold: float = 0.5,
             transform: Optional[torchvision.transforms.Compose] = None,
             save_path: str = None,
             onnx_inf: bool = False,
-            num_slice: int = 1,
-            save_result: bool = False,
-            img_thr: float = 0.4,
-            use_peak: bool = False,
-            peak_min_distance: int = 15,
-            peak_threshold_rel: float = 0.5,
-            **kwargs
+            num_slice: int = 1
     ) -> None:
-        super(Predictor, self).__init__(
-            save_result=save_result, save_dir=save_path, **kwargs
-        )
+        super(Predictor, self).__init__(save_dir=save_path)
         self.model = model
         self.input_size = input_size
         self.resize_fn = resize_fn
-
-        self.img_thr = img_thr
-        self.use_peak = use_peak
-        self.peak_min_distance = peak_min_distance
-        self.peak_threshold_rel = peak_threshold_rel
         self.threshold = threshold
-
         self.transform = transform
         self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
         self.onnx_inf = onnx_inf
         self.num_slice = num_slice
-        detect_people = getattr(self, 'detect_people', False)
-        if detect_people:
-            from configs.yolox_nano_person import PeopleDetectConfig
-            people_config = PeopleDetectConfig()
-            self.people_detector = people_config.get_predictor()
-        else:
-            self.people_detector = None
 
     def __call__(self, img_meta):
         results = self.run(img_meta)
         if not getattr(self, 'no_draw', False):
             results['dst'] = self.draw(img_meta['img'], results)
 
         return results
 
-    def infer(self, img):
+    def run(self, img_meta):
+        img, path, is_vid, idx = img_meta['img'], img_meta['path'], img_meta['is_vid'], img_meta['idx']
         if isinstance(self.input_size, int):
             self.input_size = [self.input_size, self.input_size]
 
         inp = img
         ratio = (1, 1)
         dwh = (0, 0)
         if self.resize_fn:
             inp, ratio, dwh = self.resize_fn(img)
+            assert dwh == (0, 0)
         if self.transform:
             inp = self.transform(inp)
 
         if self.onnx_inf:
             anomaly_map = self.model.run(
                 None,
                 {'images': inp.unsqueeze(0).numpy().astype('float32')}
             )[0]
         else:
             with torch.no_grad():
                 anomaly_map = self.model(inp.unsqueeze(0).to(self.device))
-            anomaly_map = anomaly_map.squeeze(0).cpu().detach().numpy()
-
-        anomaly_map = gaussian_filter(anomaly_map, sigma=4)
+            anomaly_map = anomaly_map.cpu().detach().numpy()
 
-        return anomaly_map
 
-    def postprocess(self, anomaly_map, img_shape,
-                    min_anomaly_value=None, max_anomaly_value=None):
-        if isinstance(self.input_size, int):
-            self.input_size = [self.input_size, self.input_size]
-
-        src_area = self.input_size[1] * self.input_size[0]
-        area_limit = int(src_area * 0.12 * 0.5 * 0.01)
-        length_limit = int(pow(area_limit, 0.5) * 0.5)  # 6
-
-        img_h, img_w = img_shape[:2]
-        if (np.max(anomaly_map) > self.img_thr):
-            anomaly_map = self.min_max_norm(anomaly_map, min_anomaly_value, max_anomaly_value)
-            anomaly_map = gaussian_filter(anomaly_map, sigma=4)
-            anomaly_map = cv2.resize(anomaly_map, self.input_size)
-
-            # image_max = ndi.maximum_filter(im, size=10, mode='constant')
-            # Comparison between image_max and im to find the coordinates of local maxima
-            if (self.use_peak):
-                gray_map = np.uint8(anomaly_map * 255)
-                im = img_as_float(gray_map)
-                coordinates = peak_local_max(im, min_distance=self.peak_min_distance,
-                                             threshold_rel=self.peak_threshold_rel, exclude_border=False)  # 返回[行，列]，即[y, x]
-            # coordinates = coordinates[anomaly_map[coordinates[:, 0], coordinates[:, 1]] > 0.8 * np.max(anomaly_map)]
-            else:
-                coordinates = []
-            mask = anomaly_map.copy()
-            mask[mask > self.threshold] = 1
-            mask[mask <= self.threshold] = 0
-            kernel = morphology.disk(4)
-            mask = morphology.opening(mask, kernel)
-            mask *= 255
-            mask = mask.astype(np.uint8)
-            contours, hierarchy = cv2.findContours(mask, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
-
-            anomaly_area = []
-            for contour in contours:
-                contour = cv2.approxPolyDP(contour, len(contours), True)
-                x, y, w, h = cv2.boundingRect(contour)
-
-                if w < length_limit or h < length_limit or w * h < area_limit:
-                    continue
-
-                x1, y1 = x, y
-                x2, y2 = x + w, y + h
-                # x1, y1 = round((x - dwh[0]) / ratio[0]), round((y - dwh[1]) / ratio[1])
-                # x2, y2 = round(x1 + w / ratio[0]), round(y1 + h / ratio[1])
-                anomaly_area.append([x1, y1, x2, y2])
-        else:
-            anomaly_map = cv2.resize(anomaly_map, self.input_size)
-            anomaly_area = []
-            coordinates = []
-
-        # ------filter-------
-        complete, filter_anomaly_area = rectMerge_sxf(anomaly_area)
-        # print("filter_anomaly_area:", filter_anomaly_area)
-        if len(coordinates) and self.use_peak:
-            filter_anomaly_area = check_rect_contain_point(filter_anomaly_area, coordinates)
-        anomaly_area = filter_anomaly_area
-
-        scale_h, scale_w = float(img_h) / self.input_size[0], float(img_w) / self.input_size[1]
-        bboxes, points = [], []
-        for rect in anomaly_area:
-            x1, y1, x2, y2 = rect
-            x1, y1 = round(x1 * scale_w), round(y1 * scale_h)
-            x2, y2 = round(x2 * scale_w), round(y2 * scale_h)
-            bboxes.append([x1, y1, x2, y2])
-        for point in coordinates:
-            y, x = point
-            x, y = round(x * scale_w), round(y * scale_h)
-            points.append([x, y])
-        del anomaly_area, coordinates
-
-        return dict(
-            anomaly_area=bboxes,
-            anomaly_point=points
-        )
 
-    def min_max_norm(self, image,  min_anomaly_value=None, max_anomaly_value=None):
-        a_min = image.min() if min_anomaly_value is None else min_anomaly_value
-        a_max = image.max() if max_anomaly_value is None else max_anomaly_value
-        return (image - a_min) / (a_max - a_min)
-
-    def run(self, img_meta):
-        img, path, is_vid, idx = img_meta['img'], img_meta['path'], img_meta['is_vid'], img_meta['idx']
-
-        anomaly_map = self.infer(img)
-
-        results = self.postprocess(anomaly_map, img.shape)
+        anomaly_map = gaussian_filter(anomaly_map, sigma=4)
 
-        if self.people_detector is not None:
-            people_results = self.people_detector.run(img_meta)
-            results.update({'people_detection': people_results})
+        anomaly_map = cv2.resize(anomaly_map, self.input_size)
 
-        if getattr(self, 'show_heatmap', True):
-            if is_vid:
-                logger.warning('Source is video, can not plot figure.')
-            else:
-                basename = os.path.basename(path)
-                name, suffix = os.path.splitext(basename)
-                save_path = f'{self.save_dir}/{name}_heatmap{suffix}'
-                self.plot_fig(img, anomaly_map, results['anomaly_area'], results['anomaly_point'], save_path)
+        gray_map = np.uint8(anomaly_map * 255)
+        im = img_as_float(gray_map)
+        image_max = maximum_filter(im, size=10, mode='constant')
+        # Comparison between image_max and im to find the coordinates of local maxima
+        coordinates = peak_local_max(im, min_distance=35)  # 返回[行，列]，即[y, x]
+        coordinates = coordinates[anomaly_map[coordinates[:, 0], coordinates[:, 1]] > 0.8*np.max(anomaly_map)]
+        inp = inp.numpy() if isinstance(inp, torch.Tensor) else inp
+        resized_img = denormalization(inp)
+
+        if getattr(self, 'show_heatmap', False) and not is_vid:
+            self.plot_fig(resized_img, anomaly_map,coordinates, path)
+
+        mask = anomaly_map.copy()
+        mask[mask > self.threshold] = 1
+        mask[mask <= self.threshold] = 0
+
+        mask *= 255
+        mask = mask.astype(np.uint8)
+        contours, hierarchy = cv2.findContours(mask, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+
+        anomaly_area = []
+        for contour in contours:
+            contour = cv2.approxPolyDP(contour, len(contours), True)
+            x, y, w, h = cv2.boundingRect(contour)
+            if w < 17 or h < 17 or w*h<1200:
+                continue
+            x1, y1 = round((x - dwh[0]) / ratio[0]), round((y - dwh[1]) / ratio[1])
+            x2, y2 = round(x1 + w / ratio[0]), round(y1 + h / ratio[1])
+            anomaly_area.append([x1, y1, x2, y2])
 
         if getattr(self, 'save_xml', False):
             if is_vid:
                 logger.warning('Source is video, can not save results to xml.')
-            else:
-                save_xml_dir = os.path.join(self.save_dir, 'xml_predict')
-                self.save_xml_dir = save_xml_dir if save_xml_dir is not None \
-                    else os.path.join(self.save_dir, 'predict')
-                os.makedirs(self.save_xml_dir, exist_ok=True)
-                self.save_result_to_xml(path, img.shape, results['anomaly_area'], self.save_xml_dir)
 
-        return results
+            save_xml_dir = getattr(self, 'save_xml_dir')
+            self.save_xml_dir = save_xml_dir if save_xml_dir is not None \
+                else os.path.join(self.save_dir, 'predict')
+            os.makedirs(self.save_xml_dir, exist_ok=True)
+            self.save_result_to_xml(path, img.shape, anomaly_area, self.save_xml_dir)
+
+        return dict(
+            anomaly_area=anomaly_area
+        )
 
     def draw(self, img: np.ndarray, results) -> np.ndarray:
         for rect in results['anomaly_area']:
             x1, y1, x2, y2 = rect
             cv2.rectangle(img, (x1, y1), (x2, y2), (0, 0, 255), 2)
-        if self.people_detector is not None:
-            img = self.people_detector.draw({'img': img}, results['people_detection'])
         return img
 
-    def plot_fig(self, img, anomaly_map, anomaly_area, anomaly_point, save_path=None):
-
-        r = anomaly_map.shape[1] / img.shape[1], anomaly_map.shape[0] / img.shape[0]
-        resize_img = cv2.resize(img, (anomaly_map.shape[1], anomaly_map.shape[0]))[:, :, ::-1]  # RGB
-
+    def plot_fig(self, resize_img, anomaly_map,coordinates, path):
         fig = plt.figure()
         ax0 = fig.add_subplot(221)
         ax0.axis('off')
         ax0.imshow(resize_img)
         ax0.title.set_text('Image')
 
         ax2 = fig.add_subplot(222)
         ax2.axis('off')
         ax2.imshow(resize_img, cmap='gray', interpolation='none')
         ax2.imshow(anomaly_map, cmap='jet', alpha=0.5, interpolation='none')
-        ax2.title.set_text('Predicted heatmap')
+        ax2.title.set_text('Predicted heat map')
 
         ax3 = fig.add_subplot(223)
         ax3.axis('off')
-        ax3.imshow(resize_img)
-        if len(anomaly_point):
-            anomaly_point = np.array(anomaly_point, dtype=np.float64)
-            anomaly_point[:, 0] *= r[0]
-            anomaly_point[:, 1] *= r[1]
-            anomaly_point.round()
-            ax3.plot(anomaly_point[:, 0], anomaly_point[:, 1], 'r.')
+        ax3.imshow(resize_img, cmap='gray', interpolation='none')
+        ax3.plot(coordinates[:, 1], coordinates[:, 0], 'r.', marker='o')
+        # ax3.imshow(anomaly_map, cmap='jet', alpha=0.5, interpolation='none')
         ax3.title.set_text('Predicted key point')
 
-        ax4 = fig.add_subplot(224)
-        ax4.axis('off')
-        ax4.imshow(resize_img)
-        for rect in anomaly_area:
-            x1, y1, x2, y2 = rect
-            x1, y1 = round(x1 * r[0]), round(y1 * r[1])
-            x2, y2 = round(x2 * r[0]), round(y2 * r[1])
-            ax4.add_patch(plt.Rectangle((x1, y1), x2 - x1, y2 - y1, color='red', fill=False, linewidth=1))
-        ax4.title.set_text('Predicted box')
-
         fig.tight_layout()
 
         if self.view_result:
             plt.show()
 
-        # self.save_result = True
-        if self.save_result and save_path is not None:
-            if not os.path.exists(os.path.dirname(save_path)):
-                os.makedirs(os.path.dirname(save_path))
-            fig.savefig(save_path, dpi=100)
+        if self.save_result:
+            basename = os.path.basename(path)
+            name, suffix = os.path.splitext(basename)
+            fig.savefig(f'{self.save_dir}/{name}_heatmap{suffix}', dpi=100)
 
         plt.close()
```

## tepe/tasks/rd/task.py

```diff
@@ -1,82 +1,55 @@
 import os
-from typing import Union, Callable
-
+from typing import Tuple, Literal, Union, Callable
 import numpy as np
-import torch
-from loguru import logger
 from tabulate import tabulate
-from torch.utils.data import DataLoader
-
+from loguru import logger
+import torch
 from tepe.core import BaseTask
-from tepe.utils.general import check_requirements
 
 
 class RDConfig(BaseTask):
     def __init__(self):
         super(RDConfig, self).__init__()
-
-        # check_requirements(os.path.join(os.path.dirname(__file__), 'requirements.txt'))
         self.task_name = 'rd'
-        
-        # model----------------------------------------------------
-        self.feature_extractor = 'wres50'
-        
-        # data-----------------------------------------------------
         self.data_root = './mvtec/'
-        self.scene = 'bsofa'
         self.is_mvtec = False
+        self.scene = 'bsofa'
+        self.feature_extractor = 'wres50'
+        self.max_epoch = 20
+        self.basic_lr_per_img = 0.005 / 16
         self.batch_size = 16
         self.workers = 4
-        self.cache = False
+
         self.input_size = 256
-        self.num_slice = []
         self.keep_ratio = False
-        
-        # train----------------------------------------------------
-        self.max_epoch = 20
-        self.basic_lr_per_img = 0.01 / 16
         self.device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        self.weight_decay = 0
-        
-        self.hard_sample_mining = True
-        self.mining_thr = 0.3
-        self.mining_epochs = 30
-        
-        self.sched_type = 'cosine'
-        self.warmup_epochs = 0
-        self.min_lr = 1e-5  # 下降到的最小学习率
-        self.lr_noise: float = None  # 从lr_noise*max_epoch时开始添加lr噪声
-        self.lr_noise_pct = 0.2  # 噪声抖动大小
-
-        # predict--------------------------------------------------
-        self.img_thr = 0.4
-        self.use_peak = True
-        self.peak_min_distance = 15
-        self.peak_threshold_rel = 0.5
-        self.threshold = 0.4
-        self.save_result = True
-        self.save_xml = False
-        self.show_heatmap = True
+        self.threshold = 0.5
 
     def get_train_loader(self):
         from tepe.data.datasets import AnomalyDataset
 
-        data_transform, resize_fn, target_transform = self.get_transform()
+        data_transform, target_transform = self.get_transform()
 
-        self.train_data = AnomalyDataset(self.data_root, class_name=self.scene,
-                                         transform=data_transform, target_transform=target_transform,
-                                         resize_fn=resize_fn, is_train=True, is_mvtec=False,
-                                         cache_img=self.cache)
+        train_data = AnomalyDataset(self.data_root, class_name=self.scene,
+                                    transform=data_transform, target_transform=target_transform,
+                                    resize=self.input_size, is_train=True, is_mvtec=False)
+
+        thr_data = AnomalyDataset(self.data_root, class_name=self.scene,
+                                  transform=data_transform, target_transform=target_transform,
+                                  paste=True, is_train=True, is_mvtec=False)
 
-        train_dataloader = DataLoader(
-            self.train_data, batch_size=self.batch_size, shuffle=True, num_workers=self.workers
+        train_dataloader = torch.utils.data.DataLoader(
+            train_data, batch_size=self.batch_size, shuffle=True, num_workers=self.workers
+        )
+        thr_dataloader = torch.utils.data.DataLoader(
+            thr_data, batch_size=self.batch_size, shuffle=True, num_workers=self.workers
         )
 
-        return train_dataloader
+        return train_dataloader, thr_dataloader
 
     def get_transform(self, mode='train'):
         assert mode in ['train', 'val', 'test']
         from functools import partial
         from PIL import Image
         from torchvision import transforms as T
         from tepe.data import letterbox
@@ -84,172 +57,182 @@
         new_shape = [self.input_size, self.input_size] \
             if isinstance(self.input_size, int) else self.input_size
         resize_fn = partial(letterbox, new_shape=new_shape, pad_color=(114, 114, 114),
                             auto=False, stride=None, keep_ratio=self.keep_ratio,
                             scaleup=True, rgb=True, interpolation=3)
 
         if mode == 'train':
-            transform = T.Compose([T.ToTensor(),
+            transform = T.Compose([T.Lambda(lambda x: resize_fn(im=x)[0]),
+                                   T.ToTensor(),
+                                   T.RandomRotation(10),
                                    T.Normalize(mean=[0.485, 0.456, 0.406],
                                                std=[0.229, 0.224, 0.225])])
             transform_mask = T.Compose([T.Resize(self.input_size, Image.NEAREST),
+                                        T.RandomRotation(10),
                                         T.ToTensor()]) if self.is_mvtec else None
-            return transform, resize_fn, transform_mask
+            return transform, transform_mask
         elif mode == 'val':
-            transform = T.Compose([T.ToTensor(),
+            transform = T.Compose([T.Lambda(lambda x: resize_fn(im=x)[0]),
+                                   T.ToTensor(),
                                    T.Normalize(mean=[0.485, 0.456, 0.406],
                                                std=[0.229, 0.224, 0.225])])
 
             transform_mask = T.Compose([T.Resize(self.input_size, Image.NEAREST),
                                         T.ToTensor()]) if self.is_mvtec else None
-            return transform, resize_fn, transform_mask
+            return transform, transform_mask
         else:
             transform = T.Compose([T.ToTensor(),
                                    T.Normalize(mean=[0.485, 0.456, 0.406],
                                                std=[0.229, 0.224, 0.225])])
 
-            return transform, resize_fn, None
+            return transform, resize_fn
 
     def get_model(self, train=True):
         from tepe.tasks.rd.model import Model
 
-        model = Model(self.feature_extractor, self.input_size)
+        model = Model()
         if not train:
             ckpt = torch.load(self.weights, map_location=self.device)
             model.load_state_dict(ckpt['model'])
             model.eval().to(self.device)
             logger.info('Model load done.')
 
         return model
 
     def train(self):
-        from torch.utils.tensorboard import SummaryWriter
         from tepe.utils.general import (
             init_seeds,
+            save_task_attr_to_yaml,
             save_task_config_py,
             setup_logger
         )
-        from tepe.modules.scheduler import create_scheduler
-        from tepe.tasks.rd.find_thr import find_hard_samples
 
-        save_dir = self.output_dir  # + f'/{self.scene}'
-        if not os.path.exists(save_dir):
-            os.makedirs(save_dir, exist_ok=True)
-
-        # save args
-        # save_task_attr_to_yaml(self, save_dir)
-        save_task_config_py(self, save_dir)
-
-        # save log text
-        setup_logger(save_file=os.path.join(save_dir, 'train_log.txt'), mode='a')  # logger
-        tblogger = SummaryWriter(save_dir)  # tensorboard
         init_seeds(self.seed)
 
         model = self.get_model().to(self.device).train()
         model.encoder.eval()
-        
-        # optimier
         optimizer = torch.optim.Adam(
             list(model.decoder.parameters()) + list(model.bn.parameters()),
-            lr=self.learning_rate, betas=(0.5,0.999), weight_decay=self.weight_decay
+            lr=self.learning_rate, betas=(0.5,0.999)
         )
-        
-        # lr schedule
-        if self.hard_sample_mining:  # 更新学习率参数
-            self.lr_cycle_limit = 2    # 循环次数
-            self.lr_cycle_mul = self.mining_epochs / self.max_epoch   # 下次循环长度的乘子
-            self.lr_cycle_decay = 0.1  # 下次循环初始值的乘子
-        lr_scheduler, num_epoch = create_scheduler(self, self.sched_type, optimizer)
 
-        self.train_dataloader = self.get_train_loader()
+        train_dataloader, thr_dataloader = self.get_train_loader()
+
+        save_dir = self.output_dir + f'/{self.scene}'
+        os.makedirs(save_dir, exist_ok=True)
+
+        # save args
+        save_task_attr_to_yaml(self, save_dir)
+        save_task_config_py(self, save_dir)
+
+        # save log text
+        logger.add(os.path.join(save_dir, 'train_log.txt'))
+        setup_logger(save_file=os.path.join(save_dir, 'train_log.txt'))  # logger
 
-        # train loop
         logger.info('Training start...')
-        for epoch in range(1, num_epoch + 1):
+        for epoch in range(1, self.max_epoch + 1):
             loss_list = []
-            for data in self.train_dataloader:
-                img = data['img'].to(self.device)
+            for img, _, _ in train_dataloader:
+                img = img.to(self.device)
                 loss = model(img)
                 optimizer.zero_grad()
                 loss.backward()
                 optimizer.step()
                 loss_list.append(loss.item())
-            
-            # get current lr
-            lrl = [param_group['lr'] for param_group in optimizer.param_groups]
-            lr = sum(lrl) / len(lrl)
-            if lr_scheduler is not None:
-                lr_scheduler.step(epoch + 1)  # update lr
-            
-            # logger
-            logger.info('epoch [{}/{}], loss:{:.4f}, lr:{:.5f}'.format(epoch, num_epoch, np.mean(loss_list), lr))
-            tblogger.add_scalar(tag=f'{self.scene}/loss', scalar_value=np.mean(loss_list), global_step=epoch)
-            tblogger.add_scalar(tag=f'{self.scene}/lr', scalar_value=lr, global_step=epoch)
-            
+            logger.info('epoch [{}/{}], loss:{:.4f}'.format(epoch, self.max_epoch, np.mean(loss_list)))
+
             # save model
-            if epoch % 5 == 0 or epoch == num_epoch:
+            if epoch % 5 == 0 or epoch == self.max_epoch:
                 self.weights = os.path.join(save_dir, f'{self.feature_extractor}_rd_{self.scene}.pth')
                 torch.save({'model': model.state_dict(),
-                            'lr': lr,
                             'epoch': epoch}, self.weights)
                 logger.info(f"model save in {self.weights}")
 
-            # hard sample mining
-            if  self.hard_sample_mining and \
-                    epoch >= (num_epoch-self.mining_epochs) and epoch % 5 == 0 and epoch != num_epoch:
-                
-                select_paths = find_hard_samples(model, self.train_dataloader,
-                                                 self.device, mining_thr=self.mining_thr)
-                if len(select_paths):
-                    dataset = self.train_dataloader.dataset
-                    dataset.add_hard_samples(select_paths)
-                    # update train dataloader
-                    self.train_dataloader = DataLoader(
-                        self.train_data, batch_size=self.batch_size,
-                        shuffle=True, num_workers=self.workers
-                    )
-                else:  # early stop
-                    break
-                model.train()
-                model.encoder.eval()
+        from tepe.tasks.rd.find_thr import find
+        self.threshold = find(model, train_dataloader, thr_dataloader, self.device)
+        logger.info(f"find a appropriate threshold: {self.threshold}")
 
-        self.set_post_info(scene=self.scene, thr=self.threshold)  # post info using http connect
+        self.set_post_info(scene=self.scene, thr=self.threshold)
 
     def eval(self):
-        
-        if self.is_mvtec:
-            from .evalutor import mvtec_eval
-            return mvtec_eval(self)
+        from tepe.data.infer_datasets import LoadImages1
+        from .evalutor import read_xml, cal_true_positive
+
+        predictor = self.get_predictor()
+        eval_data_root = os.path.join(self.data_root, self.scene, 'test')
+
+        all_precision = {}
+        all_recall = {}
+
+        for bad_name in os.listdir(eval_data_root):
+            dataset = LoadImages1(os.path.join(eval_data_root, bad_name))
+            gt_dir = os.path.join(self.data_root, self.scene, 'ground_truth', bad_name)
+
+            total_pred, total_gt, total_tp = 0, 0, 0
+            for data in dataset:
+                # get prediction
+                results = predictor.run(data)
+                pred = torch.Tensor(results['anomaly_area'])
+
+                # get ground-truth
+                img_name = os.path.basename(data['path'])
+                xml_path = os.path.join(
+                    gt_dir, img_name.replace(img_name.rsplit('.', maxsplit=1)[-1], 'xml')
+                )
+                if not os.path.exists(xml_path):
+                    logger.warning(f'not found {xml_path}')
+                    continue
+                gt = read_xml(xml_path)
+
+                tp = cal_true_positive(gt, pred)
+
+                total_pred += len(pred)
+                total_gt += len(gt)
+                total_tp += tp
+
+            all_precision[bad_name] = total_tp / total_pred
+            all_recall[bad_name] = total_tp / total_gt
+            logger.info(f'{bad_name} precision: {all_precision[bad_name]}, '
+                        f'recall: {all_recall[bad_name]}')
+
+        # show eval results
+        all_precision['mean'] = sum(list(all_precision.values())) / len(all_precision)
+        all_recall['mean'] = sum(list(all_recall.values())) / len(all_recall)
+        bad_name = list(all_recall.keys())
+        table_header = [" "] + bad_name
+        each_p = ["precision"] + [all_precision[k] for k in bad_name]
+        each_r = ["recall"] + [all_recall[k] for k in bad_name]
+        result_table = [
+            each_p,
+            each_r
+        ]
+        logger.info('eval result:\n{}'.format(
+            tabulate(result_table, headers=table_header, tablefmt="fancy_grid")
+        ))
+
+        return dict(p=all_precision, r=all_recall)
 
-        else:
-            from tepe.data.infer_datasets import LoadImages1
-            from .evalutor import read_xml, cal_true_positive
-            
-            return
 
     def get_predictor(self) -> Union[None, Callable]:
         from tepe.tasks.rd.predictor import Predictor
 
         onnx_inf = False
         if os.path.splitext(self.weights)[-1] == '.onnx':
             logger.info('use onnxruntime for inference')
             import onnxruntime as ort
             model = ort.InferenceSession(self.weights)
             onnx_inf = True
         else:
             model = self.get_model(train=False)
 
-        transform, resize_fn, _ = self.get_transform(mode='test')
+        transform, resize_fn = self.get_transform(mode='test')
         predictor = Predictor(
             model=model,
             resize_fn=resize_fn,
             input_size=self.input_size,
             transform=transform,
             threshold=self.threshold,
             save_path=self.output_dir,
-            onnx_inf=onnx_inf,
-            save_result=self.save_result,
-            save_xml=self.save_xml,
-            show_heatmap=self.show_heatmap
+            onnx_inf=onnx_inf
         )
 
         return predictor
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## tepe/tasks/yolox/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 6672 6f6d 202e 7461 736b 2069 6d70 6f72  from .task impor
+00000010: 7420 594f 4c4f 5843 6f6e 6669 67         t YOLOXConfig
```

## tepe/tasks/yolox/task.py

```diff
@@ -24,15 +24,15 @@
         # ---------------- model config ---------------- #
         self.model_type = 'l'
         self.CLASS = ('01', '02', )
         self.num_classes = 80
         self.act = 'silu'
 
         # ---------------- dataloader config ---------------- #
-        self.dataset_type = 'coco'  # or voc
+        self.dataset_format = 'coco'  # or voc
         # set worker to 4 for shorter dataloader init time
         self.data_num_workers = 4
         self.input_size = (640, 640)  # (height, width)
         # Actual multiscale ranges: [640-5*32, 640+5*32].
         # To disable multiscale training, set the
         # self.multiscale_range to 0.
         self.multiscale_range = 5
@@ -52,14 +52,15 @@
         self.flip_prob = 0.5
         self.degrees = 10.0
         self.translate = 0.1
         self.mosaic_scale = (0.1, 2)
         self.mixup_scale = (0.5, 1.5)
         self.shear = 2.0
         self.enable_mixup = True
+        self.legacy = False
 
         # --------------  training config --------------------- #
         self.device = 0
         self.is_distributed = False
         self.occupy = False  # occupy GPU memory first for training
         self.fp16 = False
         self.warmup_epochs = 5
@@ -79,15 +80,15 @@
 
         # -----------------  testing config ------------------ #
         self.test_size = (640, 640)
         self.test_conf = 0.01
         self.nmsthre = 0.65
 
     def get_model(self, train=True):
-        from tepe.tasks.yolox.models import YOLOX, YOLOPAFPN, YOLOXHead
+        from .models import YOLOX, YOLOPAFPN, YOLOXHead
         model_dict = {
             'x': [1.33, 1.25],  # depth, width
             'l': [1.0, 1.0],
             'm': [0.67, 0.75],
             's': [0.33, 0.5],
             'tiny': [0.33, 0.375],  # self.input_size = 416
             'nano': [0.33, 0.25]  # self.input_size = 416
@@ -121,15 +122,15 @@
             self.model.cuda()
             if self.fp16:
                 self.model.half()  # to FP16
 
         return self.model
 
     def get_train_loader(self):
-        from tepe.tasks.yolox.data import (
+        from .data import (
             CustomVOC,
             COCODataset,
             TrainTransform,
             YoloBatchSampler,
             DataLoader,
             InfiniteSampler,
             MosaicDetection,
@@ -139,15 +140,15 @@
             wait_for_the_master,
             get_local_rank,
         )
         # from tepe.data.datasets.yolox_voc import YOLOXVOC
 
         local_rank = get_local_rank()
 
-        if self.dataset_type == 'coco':
+        if self.dataset_format == 'coco':
             with wait_for_the_master(local_rank):
                 dataset = COCODataset(
                     data_dir=self.data_root,
                     json_file=self.train_ann,
                     img_size=self.input_size,
                     preproc=TrainTransform(
                         max_labels=50,
@@ -278,32 +279,32 @@
             )  # add pg1 with weight_decay
             optimizer.add_param_group({"params": pg2})
             self.optimizer = optimizer
 
         return self.optimizer
 
     def get_lr_scheduler(self):
-        from tepe.tasks.yolox.utils import LRScheduler
+        from .utils import LRScheduler
 
         scheduler = LRScheduler(
             self.scheduler,
             self.learning_rate,
             len(self.train_loader),
             self.max_epoch,
             warmup_epochs=self.warmup_epochs,
             warmup_lr_start=self.warmup_lr,
             no_aug_epochs=self.no_aug_epochs,
             min_lr_ratio=self.min_lr_ratio,
         )
         return scheduler
 
     def get_eval_loader(self):
-        from tepe.tasks.yolox.data import COCODataset, CustomVOC, ValTransform
+        from .data import COCODataset, CustomVOC, ValTransform
 
-        if self.dataset_type == 'coco':
+        if self.dataset_format == 'coco':
             testdev = False
             valdataset = COCODataset(
                 data_dir=self.data_root,
                 json_file=self.val_ann if not testdev else "image_info_test-dev2017.json",
                 name="val2017" if not testdev else "test2017",
                 img_size=self.input_size,
                 preproc=ValTransform(legacy=False),
@@ -333,19 +334,19 @@
         }
         dataloader_kwargs["batch_size"] = batch_size
         val_loader = torch.utils.data.DataLoader(valdataset, **dataloader_kwargs)
 
         return val_loader
 
     def get_evaluator(self, train=False):
-        from tepe.tasks.yolox.evaluators import COCOEvaluator, VOCEvaluator
+        from .evaluators import COCOEvaluator, VOCEvaluator
 
         model = None if train else self.get_model(train=False)
         val_loader = self.get_eval_loader()
-        if self.dataset_type == 'coco':
+        if self.dataset_format == 'coco':
             testdev = False
             evaluator = COCOEvaluator(
                 dataloader=val_loader,
                 training=train,
                 img_size=self.test_size,
                 num_classes=self.num_classes,
                 model=model,
@@ -370,36 +371,36 @@
                 half=self.fp16,
                 save_dir=self.output_dir,
                 save_result=True
             )
         return evaluator
 
     def get_predictor(self):
-        from tepe.tasks.yolox.data import ValTransform
-        from tepe.tasks.yolox.yolox_detector import YOLOXPredictor
+        from .data import ValTransform
+        from .yolox_detector import YOLOXPredictor
 
         model = self.get_model(train=False)
         predictor = YOLOXPredictor(
             input_size=self.input_size,
             classes=self.CLASS,
             model=model,
-            preprocess=ValTransform(legacy=True),
+            preprocess=ValTransform(legacy=self.legacy),
             conf_thres=self.test_conf,
             iou_thres=self.nmsthre,
             device=self.device,
             save_dir=self.output_dir
         )
         return predictor
 
     def eval(self):
         evaluator = self.get_evaluator(train=False)
         return evaluator.evaluate()
 
     def train(self):
-        from tepe.tasks.yolox.core.trainer import Trainer
+        from .core.trainer import Trainer
 
         if self.seed is not None:
             random.seed(self.seed)
             torch.manual_seed(self.seed)
             cudnn.deterministic = True
             warnings.warn(
                 "You have chosen to seed training. This will turn on the CUDNN deterministic setting, "
```

## tepe/tasks/yolox/yolox_detector.py

```diff
@@ -35,16 +35,16 @@
             self.model(torch.zeros(1, 3, *input_size).to(self.device).type_as(
                 next(self.model.parameters())))  # run once
 
         self.preprocess = preprocess
         self.postprocess = postprecess
 
     def __call__(self, img_meta):
-        results = self.run(img_meta)
-        result_image = self.draw(img_meta, results)
+        outputs, img_info = self.run(img_meta)
+        result_image = self.draw(outputs[0], img_info)
         return result_image
 
     def run(self, img_meta):
         img = img_meta['img']
         img_info = {"id": 0}
 
         height, width = img.shape[:2]
@@ -71,32 +71,29 @@
             outputs = postprocess(
                 outputs, num_classes=len(self.classes),
                 conf_thre=self.conf_thrs, nms_thre=self.iou_thrs
             )
             # if self.postprocess is not None:
                 # outputs = self.postprocess(outputs)
             logger.info("Infer time: {:.4f}s".format(time_synchronized() - t0))
+        return outputs, img_info
+
+    def draw(self, output, img_info):
+        ratio = img_info["ratio"]
+        img = img_info["raw_img"]
+        if output is None:
+            return img
 
         # [x0, y0, x1, y1, obj, conf, cls]
-        output = outputs[0].cpu()
+        output = output.cpu()
         bboxes = output[:, 0:4]
 
         # preprocessing: resize
         bboxes /= ratio
 
         cls = output[:, 6]
         scores = output[:, 4] * output[:, 5]
 
-        return dict(
-            bboxes=bboxes,
-            cls=cls,
-            scores=scores
-        )
-
-    def draw(self, img_meta, results):
-        img = img_meta["img"]
-
-        bboxes, scores, cls = results['bboxes'], results['scores'], results['cls']
-        vis_res = draw_detection(img, bboxes, scores, cls, class_names=self.classes)
+        vis_res = draw_detection(img, bboxes, scores, cls, self.classes)
         return vis_res
```

## tepe/utils/__init__.py

```diff
@@ -1,3 +1,5 @@
-from .general import xyxy2xywh, ROOT, init_seeds, setup_logger, increment_path
+from .general import xyxy2xywh, ROOT, init_seeds, setup_logger, increment_path, setup_logger, save_task_attr_to_yaml, \
+    save_task_config_py
 from .torch_utils import time_synchronized, select_device
-from .dist import gather, is_main_process, synchronize
+from .dist import gather, is_main_process, synchronize
+from .model_utils import get_model_info
```

## tepe/utils/dist.py

```diff
@@ -9,107 +9,39 @@
 This is useful when doing distributed training.
 """
 
 import functools
 import os
 import pickle
 import time
-import subprocess
 from contextlib import contextmanager
 from loguru import logger
 
 import numpy as np
 
-import cv2
 import torch
 from torch import distributed as dist
 
-
 __all__ = [
     "get_num_devices",
     "wait_for_the_master",
     "is_main_process",
     "synchronize",
     "get_world_size",
     "get_rank",
     "get_local_rank",
     "get_local_size",
     "time_synchronized",
     "gather",
     "all_gather",
-    "configure_nccl", "configure_module", "configure_omp"
 ]
 
 _LOCAL_PROCESS_GROUP = None
 
 
-def configure_nccl():
-    """Configure multi-machine environment variables of NCCL."""
-    os.environ["NCCL_LAUNCH_MODE"] = "PARALLEL"
-    os.environ["NCCL_IB_HCA"] = subprocess.getoutput(
-        "pushd /sys/class/infiniband/ > /dev/null; for i in mlx5_*; "
-        "do cat $i/ports/1/gid_attrs/types/* 2>/dev/null "
-        "| grep v >/dev/null && echo $i ; done; popd > /dev/null"
-    )
-    os.environ["NCCL_IB_GID_INDEX"] = "3"
-    os.environ["NCCL_IB_TC"] = "106"
-
-
-def configure_omp(num_threads=1):
-    """
-    If OMP_NUM_THREADS is not configured and world_size is greater than 1,
-    Configure OMP_NUM_THREADS environment variables of NCCL to `num_thread`.
-
-    Args:
-        num_threads (int): value of `OMP_NUM_THREADS` to set.
-    """
-    # We set OMP_NUM_THREADS=1 by default, which achieves the best speed on our machines
-    # feel free to change it for better performance.
-    if "OMP_NUM_THREADS" not in os.environ and get_world_size() > 1:
-        os.environ["OMP_NUM_THREADS"] = str(num_threads)
-        if is_main_process():
-            logger.info(
-                "\n***************************************************************\n"
-                "We set `OMP_NUM_THREADS` for each process to {} to speed up.\n"
-                "please further tune the variable for optimal performance.\n"
-                "***************************************************************".format(
-                    os.environ["OMP_NUM_THREADS"]
-                )
-            )
-
-
-def configure_module(ulimit_value=8192):
-    """
-    Configure pytorch module environment. setting of ulimit and cv2 will be set.
-
-    Args:
-        ulimit_value(int): default open file number on linux. Default value: 8192.
-    """
-    # system setting
-    try:
-        import resource
-
-        rlimit = resource.getrlimit(resource.RLIMIT_NOFILE)
-        resource.setrlimit(resource.RLIMIT_NOFILE, (ulimit_value, rlimit[1]))
-    except Exception:
-        # Exception might be raised in Windows OS or rlimit reaches max limit number.
-        # However, set rlimit value might not be necessary.
-        pass
-
-    # cv2
-    # multiprocess might be harmful on performance of torch dataloader
-    os.environ["OPENCV_OPENCL_RUNTIME"] = "disabled"
-    try:
-        cv2.setNumThreads(0)
-        cv2.ocl.setUseOpenCL(False)
-    except Exception:
-        # cv2 version mismatch might rasie exceptions.
-        pass
-
-
 def get_num_devices():
     gpu_list = os.getenv('CUDA_VISIBLE_DEVICES', None)
     if gpu_list is not None:
         return len(gpu_list.split(','))
     else:
         devices_list_info = os.popen("nvidia-smi -L")
         devices_list_info = devices_list_info.read().strip().split("\n")
```

## tepe/utils/general.py

```diff
@@ -1,9 +1,10 @@
 import contextlib
 import glob
+import inspect
 import datetime
 import sys
 import math
 import os
 import platform
 import random
 import re
@@ -34,14 +35,15 @@
 np.set_printoptions(linewidth=320, formatter={'float_kind': '{:11.5g}'.format})  # format short g, %precision=5
 
 cv2.setNumThreads(0)  # prevent OpenCV from multithreading (incompatible with PyTorch DataLoader)
 os.environ['NUMEXPR_MAX_THREADS'] = str(min(os.cpu_count(), 8))  # NumExpr max threads
 
 FILE = Path(__file__).resolve()
 ROOT = FILE.parents[2]
+PRETRAINED_DIR = ROOT / 'assets/pretrained'
 
 
 def show_runtime_info():
     s = f'TEPE 🚀 {git_describe() or date_modified()} torch {torch.__version__} '  # string
 
     if torch.cuda.is_available():
         device = range(torch.cuda.device_count())  # i.e. 0,1,6,7
@@ -54,17 +56,17 @@
     logger.info(s.encode().decode('ascii', 'ignore') if platform.system() == 'Windows' else s)  # emoji-safe
 
 
 def get_bar(iterable, desc=None):
     from collections import Iterable
     bar_format = '{desc:7s}{percentage:3.0f}%|{bar}|{n_fmt}/{total_fmt}[{elapsed}<{remaining}{postfix}]'
     if isinstance(iterable, int):
-        bar = tqdm(range(iterable), desc=desc, bar_format=bar_format)
+        bar = tqdm(range(iterable), desc=desc, bar_format=bar_format, total=iterable)
     elif isinstance(iterable, Iterable):
-        bar = tqdm(iterable, desc=desc, bar_format=bar_format)
+        bar = tqdm(iterable, desc=desc, bar_format=bar_format, total=len(iterable))
     else:
         raise Exception('iterable is not the required type(int or Iterable)')
     return bar
 
 
 def colorstr(*input):
     # Colors a string https://en.wikipedia.org/wiki/ANSI_escape_code, i.e.  colorstr('blue', 'hello world')
@@ -103,24 +105,27 @@
             n = max(i) + 1 if i else 2  # increment number
             path = Path(f"{path}{sep}{n}{suffix}")  # increment path
     if mkdir:
         path.mkdir(parents=True, exist_ok=True)  # make directory
     return path
 
 
-def init_seeds(seed=0, auto_batch=False):
+def init_seeds(seed=0, deterministic=False):
     # Initialize random number generator (RNG) seeds https://pytorch.org/docs/stable/notes/randomness.html
-    # cudnn seed 0 settings are slower and more reproducible, else faster and less reproducible
-    import torch.backends.cudnn as cudnn
-    if seed is not None:
-        random.seed(seed)
-        np.random.seed(seed)
-        torch.manual_seed(seed)
-        cudnn.deterministic = True if seed == 0 else False
-    cudnn.benchmark = True if not auto_batch else False
+    random.seed(seed)
+    np.random.seed(seed)
+    torch.manual_seed(seed)
+    torch.cuda.manual_seed(seed)
+    torch.cuda.manual_seed_all(seed)  # for Multi-GPU, exception safe
+    # torch.backends.cudnn.benchmark = True  # AutoBatch problem https://github.com/ultralytics/yolov5/issues/9287
+    if deterministic and check_version(torch.__version__, '1.12.0'):  # https://github.com/ultralytics/yolov5/pull/8213
+        torch.use_deterministic_algorithms(True)
+        torch.backends.cudnn.deterministic = True
+        os.environ['CUBLAS_WORKSPACE_CONFIG'] = ':4096:8'
+        os.environ['PYTHONHASHSEED'] = str(seed)
 
 
 def date_modified(path=__file__):
     # return human-readable file modification date, i.e. '2021-3-26'
     t = datetime.datetime.fromtimestamp(Path(path).stat().st_mtime)
     return f'{t.year}-{t.month}-{t.day}'
 
@@ -130,23 +135,32 @@
     s = f'git -C {path} describe --tags --long --always'
     try:
         return subprocess.check_output(s, shell=True, stderr=subprocess.STDOUT).decode()[:-1]
     except subprocess.CalledProcessError as e:
         return ''  # not a git repository
 
 
+def close_logger():
+    logger.disable('tepe')
+
+
+def show_logger():
+    logger.enable('tepe')
+
+
 def setup_logger(save_file=None, mode="o"):
     """setup logger for training and testing.
     Args:
         save_file (string): log save name.
         mode(str): log file write mode, `append` or `override`. default is `a`.
 
     Return:
         logger instance.
     """
+
     loguru_format = (
         "<green>{time:YYYY-MM-DD HH:mm:ss}</green> | "
         "<level>{level: <6}</level> | "
         "<cyan>{name}</cyan>:<cyan>{line: <4}</cyan> - <level>{message}</level>"
     )
 
     logger.remove()
@@ -200,18 +214,16 @@
     Args:
         task: BaskTask类型的任务类
         save_dir: 要保存的文件夹
 
     Returns:
         None
     """
-    if not hasattr(sys.modules[task.__module__], '__file__'):
-        return
 
-    task_file = os.path.abspath(sys.modules[task.__module__].__file__)
+    task_file = inspect.getabsfile(task.__init__)
     if os.path.splitext(task_file)[-1] != '.py':
         return
 
     task_file_r = task_file[len(str(ROOT) + '/'):]
     grade_folder = task_file_r.split(os.path.sep)
     if not task_file_r.startswith('tepe/') or len(grade_folder) <= 2:
         current_module, parent_module, grandparent_module = '', '', ''
@@ -234,43 +246,130 @@
 
             if not in_init_func:
                 f2.write(line)
                 if 'def __init__(' in line.strip():
                     in_init_func = True
                     continue
             else:
-                line_compress = line.strip('\n').strip(' ').replace(' ', '')
-                if line_compress.startswith('super('):
-                    line = line
-                elif line_compress.startswith('self.'):
-                    try:
-                        # attr_name = line_compress.split('=')[0].removeprefix('self.')  # >=python3.9
-                        attr_name = line_compress.split('=')[0][len('self.'):]
-                        line = '        self.' + attr_name + ' = ' + repr(task_args[attr_name]) + '\n'
-                    except Exception:
-                        pass
-                elif line.startswith('    def '):
-                    line = '\n' + line
-                    in_init_func = False
-                else:
-                    line = ''
+                if line:
+                    line_compress = line.strip('\n').strip(' ').replace(' ', '')
+                    if line_compress.startswith('self.'):
+                        try:
+                            # attr_name = line_compress.split('=')[0].removeprefix('self.')  # >=python3.9
+                            attr_name = line_compress.split('=')[0][len('self.'):]
+                            line = '        self.' + attr_name + ' = ' + repr(task_args[attr_name]) + '\n'
+                        except Exception:
+                            pass
+                    elif line.startswith('    def ') or line[0].isalnum():
+                        # line = '\n' + line
+                        in_init_func = False
+
                 f2.write(line)
 
 
+def find_config(output_dir: str):
+    """
+    寻找output_dir下的config.py
+    Args:
+        output_dir (str): 结果文件夹路径
+
+    Returns:
+        config.py文件路径
+    """
+    assert os.path.exists(output_dir)
+
+    config_file = os.path.join(output_dir, 'config.py')
+    if not os.path.exists(config_file):
+        logger.warning(f"make sure contains the 'config.py' file in {output_dir}\n"
+                       f"Or you need to specify '-t/--task-file/--task-name' in the command line")
+        config_file = ''
+    return config_file
+    
+
+def find_weights(output_dir: str):
+    """
+    寻找output_dir下最新的权重文件，权重文件只支持pth/pt
+    Args:
+        output_dir (str): 结果文件夹路径
+
+    Returns:
+        模型文件路径
+    """
+    assert os.path.exists(output_dir)
+
+    weights_list = glob.glob(f'{output_dir}/*.pt*', recursive=True)
+    if weights_list:
+        weights_file = max(weights_list, key=os.path.getctime)
+        logger.info(f"found weights file: {weights_file}")
+    else:
+        logger.warning(f"make sure contains the weights file in {output_dir}\n"
+                       f"you need to specify '-w/--weights' in the command line")
+        weights_file = ''
+    return weights_file
+
+
 def file_size(path):
     # Return file/dir size (MB)
     path = Path(path)
     if path.is_file():
         return path.stat().st_size / 1E6
     elif path.is_dir():
         return sum(f.stat().st_size for f in path.glob('**/*') if f.is_file()) / 1E6
     else:
         return 0.0
 
 
+def download_pretrained_model(url, target=None):
+    target = Path(PRETRAINED_DIR if target is None else target)
+    target.mkdir(exist_ok=True)
+
+    url = str(url).strip().replace("'", '').replace(os.sep, '/')
+
+    # URL specified
+    if str(url).startswith(('http:/', 'https:/')):  # download
+        min_bytes = 1E0
+        file = target / str(url).rsplit('/', 1)[-1]
+        url = str(url).replace('://', ':/')  # Pathlib turns :// -> :/
+
+        if Path(file).is_file():
+            name = str(url).rsplit('/', 1)[-1]
+            logger.info(f'Found {name} locally at {file}')  # file already exists
+        else:
+            try:  # url1
+                logger.info(f'Downloading {url} to {file}...')
+                torch.hub.download_url_to_file(str(url), str(file), progress=logger.level)
+                assert file.exists() and file.stat().st_size > min_bytes # check
+            except Exception as e:  # url2
+                if file.exists():
+                    file.unlink()  # remove partial downloads
+                logger.info(f'ERROR: {e}\nRe-attempting {url} to {file}...')
+                os.system(f"curl -# -L '{url}' -o '{file}' --retry 3 -C -")  # curl download, retry and resume on fail
+            finally:
+                if not file.exists() or file.stat().st_size < min_bytes:  # check
+                    if file.exists():
+                        file.unlink()  # remove partial downloads
+                    logger.error(
+                        f"Get '{url}' failed.\n"
+                        f"Please check url or make sure successful connection 10.106.226.126\n"
+                        f"Or manually copy the model from '10.106.226.126:/mnt/data/datasets/pretrained_models' to "
+                        f"'assets/pretrained'"
+                    )
+                    raise ConnectionError
+
+        return str(file)
+    else:
+        if Path(url).is_file():
+            logger.info(f'Found {url}')  # file already exists
+            file = url
+        else:
+            raise FileNotFoundError
+
+    return str(file)
+
+
 class Profile(contextlib.ContextDecorator):
     # Usage: @Profile() decorator or 'with Profile():' context manager
     def __enter__(self):
         self.start = time.time()
 
     def __exit__(self, type, value, traceback):
         print(f'Profile results: {time.time() - self.start:.5f}s')
```

## tepe/utils/meter.py

```diff
@@ -61,24 +61,33 @@
         super().__init__(factory)
 
     def reset(self):
         for v in self.values():
             v.reset()
 
     def get_filtered_meter(self, filter_key="time"):
-        return {k: v for k, v in self.items() if filter_key in k}
+        if not isinstance(filter_key, list):
+            filter_key = [filter_key]
+
+        keep_key = []
+        for k in self.keys():
+            for fk in filter_key:
+                if fk in k:
+                    keep_key.append(k)
+
+        return {k: v for k, v in self.items() if k in keep_key}
 
     def get_avg_meter(self):
         return {k: v for k, v in self.items()}
 
     def update(self, values=None, **kwargs):
         if values is None:
             values = {}
         values.update(kwargs)
         for k, v in values.items():
             if isinstance(v, torch.Tensor):
-                v = v.cpu().detach()
+                v = float(v.cpu().detach())
             self[k].update(v)
 
     def clear_meters(self):
         for v in self.values():
             v.clear()
```

## Comparing `tepe/data/voc_xml.py` & `tepe/data/annotation/voc_xml.py`

 * *Files identical despite different names*

## Comparing `tepe/modules/utils/layers.py` & `tepe/modules/layers.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,30 +14,30 @@
     return module
 
 
 class BaseConv(nn.Module):
     """A Conv2d -> Batchnorm -> silu/leaky relu block"""
 
     def __init__(
-        self, in_channels, out_channels, ksize, stride, groups=1, bias=False, act="silu"
+        self, in_channels, out_channels, ksize, stride, groups=1, bias=False, act="silu", inplace=True
     ):
         super().__init__()
         # same padding
         pad = (ksize - 1) // 2
         self.conv = nn.Conv2d(
             in_channels,
             out_channels,
             kernel_size=ksize,
             stride=stride,
             padding=pad,
             groups=groups,
             bias=bias,
         )
         self.bn = nn.BatchNorm2d(out_channels)
-        self.act = get_activation(act, inplace=True)
+        self.act = get_activation(act, inplace=inplace)
 
     def forward(self, x):
         return self.act(self.bn(self.conv(x)))
 
     def fuseforward(self, x):
         return self.act(self.conv(x))
```

## Comparing `tepe/modules/utils/loss.py` & `tepe/modules/loss.py`

 * *Files identical despite different names*

## Comparing `tepe/modules/utils/model_utils.py` & `tepe/modules/model_utils.py`

 * *Files identical despite different names*

## Comparing `tepe/tasks/rd/task copy.py` & `tepe/tasks/yolov5/task.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,302 +1,339 @@
 import os
-from typing import Union, Callable
+from pathlib import Path
+from loguru import logger
 
-import numpy as np
 import torch
-from loguru import logger
-from tabulate import tabulate
+import torch.nn as nn
 from torch.utils.data import DataLoader
-from torch.nn.parallel import DistributedDataParallel as DDP
+import numpy as np
+import cv2
 
-from tepe.core import BaseTask
-from tepe.utils.dist import get_world_size, get_rank, get_local_rank, synchronize
-from tepe.utils.general import check_requirements
+from tepe.core import BaseTask, register_config
+from tepe.data.datasets.public_class_names import coco_classes
+from tepe.tasks.yolov5.utils.augmentations import letterbox
+from tepe.utils.general import colorstr
 
 
-class RDConfig(BaseTask):
+@register_config('yolov5')
+class YOLOv5Config(BaseTask):
     def __init__(self):
-        super(RDConfig, self).__init__()
-
-        check_requirements(os.path.join(os.path.dirname(__file__), 'requirements.txt'))
-        self.task_name = 'rd'
-        self.data_root = './mvtec/'
-        self.is_mvtec = False
-        self.scene = 'bsofa'
-        self.feature_extractor = 'wres50'
-        self.batch_size = 16
+        super(YOLOv5Config, self).__init__()
+        self.task_name = 'yolov5'
+        self.CLASS = coco_classes
+        self.num_classes = 80
+        self.include_class_idx = []
+
+        # model config--------------------------------
+        self.yolov5_type = 's'
+        self.model_cfg = None
+        self.input_size = 640
+        self.pretrained = True
+        self.weights = '.pth'
+        self.resume = False
+        self.resume_ckpt = ''
+        self.freeze_layer = 0  # Number of layers to freeze. backbone=10, all=24
+
+        # dataset config-------------------------------
+        self.data_root = ''
+        self.cache = True
         self.workers = 4
-        self.cache = False
-        self.input_size = 256
-        self.num_slice = []
-        self.keep_ratio = False
-        
-        # train----------------------------------------------------        
-        self.max_epoch = 20
-        self.basic_lr_per_img = 0.01 / 16
-        self.device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        self.weight_decay = 0
-        self.sched_type = 'cosine'
-        self.warmup_epochs = 0
-        self.min_lr = 1e-5  # 下降到的最小学习率
-        self.lr_noise = 0.6  # 从0.6*max_epoch时开始添加lr噪声
-        self.lr_noise_pct = 0.2  # 噪声抖动大小
-        self.is_distributed = get_world_size() > 1
-
-        # predict--------------------------------------------------
-        self.threshold = 0.4
-        self.save_result = True
-        self.save_xml = False
-        self.show_heatmap = True
+        self.multi_scale = False
+        self.dataset_format = 'yolo'
+        self.single_cls = False  # 所有类别视为一类训练
+
+        # training config------------------------------
+        self.seed = 0
+        self.device = 0
+        self.max_epoch = 80
+        self.no_aug_epochs = 0
+        self.fp16 = False
+        self.ema = True
+        self.early_stop_patience = 100
+
+        self.linear_lr = False
+        self.warmup_lr = 0.1  # warmup initial bias lr
+        self.warmup_epochs = 3  # warmup epochs (fractions ok)
+        self.basic_lr_per_img = 0.01 / 64.0  # initial learning rate (SGD=1E-2, Adam=1E-3)
+        self.adam = False  # True for Adam, False for SGD
+        self.scheduler = "yoloxwarmcos"
+        self.min_lr_ratio = 0.05
+        self.weight_decay = 5e-4
+        self.momentum = 0.937
+        self.label_smoothing = 0.0
+        self.lrf = 0.1
+
+        self.hyp_file = 'hyp.scratch.yaml'
+        # custom hyp
+        self.hyp_update = {
+            'warmup_epochs': 3.0
+        }
+        self.transform_hyp = {}
+
+        # test config---------------------------------
+        self.conf_thre = 0.3
+        self.nms_thre = 0.5
 
-    def get_train_loader(self):
-        from tepe.data.datasets import AnomalyDataset
-        from tepe.utils.dist import wait_for_the_master, get_local_rank
-        
-        with wait_for_the_master(get_local_rank()):
-            data_transform, target_transform = self.get_transform()
-            self.train_data = AnomalyDataset(self.data_root, class_name=self.scene,
-                                            transform=data_transform, target_transform=target_transform,
-                                            resize=self.input_size, is_train=True, is_mvtec=False,
-                                            cache_img=self.cache)
+        # export config-------------------------------
+        self.nodecode = False  # easy to ncnn deploy
 
-        train_dataloader = DataLoader(
-            self.train_data, batch_size=self.batch_size, shuffle=True, num_workers=self.workers
-        )
+    def get_model(self, train=True):
+        from tepe.tasks.yolov5.yolo import Model, Detect, Conv
 
-        return train_dataloader
+        if train:
+            self.model = Model(self.yolov5_type, ch=3, nc=self.num_classes, model_cfg=self.model_cfg)  # create
+            return self.model
 
-    def get_transform(self, mode='train'):
-        assert mode in ['train', 'val', 'test']
-        from functools import partial
-        from PIL import Image
-        from torchvision import transforms as T
-        from tepe.data import letterbox
-
-        new_shape = [self.input_size, self.input_size] \
-            if isinstance(self.input_size, int) else self.input_size
-        resize_fn = partial(letterbox, new_shape=new_shape, pad_color=(114, 114, 114),
-                            auto=False, stride=None, keep_ratio=self.keep_ratio,
-                            scaleup=True, rgb=True, interpolation=3)
-
-        if mode == 'train':
-            transform = T.Compose([T.Lambda(lambda x: resize_fn(im=x)[0]),
-                                   T.ToTensor(),
-                                   T.Normalize(mean=[0.485, 0.456, 0.406],
-                                               std=[0.229, 0.224, 0.225])])
-            transform_mask = T.Compose([T.Resize(self.input_size, Image.NEAREST),
-                                        T.ToTensor()]) if self.is_mvtec else None
-            return transform, transform_mask
-        elif mode == 'val':
-            transform = T.Compose([T.Lambda(lambda x: resize_fn(im=x)[0]),
-                                   T.ToTensor(),
-                                   T.Normalize(mean=[0.485, 0.456, 0.406],
-                                               std=[0.229, 0.224, 0.225])])
-
-            transform_mask = T.Compose([T.Resize(self.input_size, Image.NEAREST),
-                                        T.ToTensor()]) if self.is_mvtec else None
-            return transform, transform_mask
         else:
-            transform = T.Compose([T.ToTensor(),
-                                   T.Normalize(mean=[0.485, 0.456, 0.406],
-                                               std=[0.229, 0.224, 0.225])])
-
-            return transform, resize_fn
-
-    def get_model(self, train=True):
-        from tepe.tasks.rd.model import Model
-
-        model = Model(self.feature_extractor, self.input_size)
-        if not train:
-            ckpt = torch.load(self.weights, map_location=self.device)
-            model.load_state_dict(ckpt['model'])
-            model.eval().to(self.device)
-            logger.info('Model load done.')
+            if Path(self.weights).suffix == '.pt':            
+                ckpt = torch.load(self.weights)  # load
+                model = ckpt['ema' if ckpt.get('ema') else 'model'].float().fuse().eval()  # FP32 model
+            else:
+                if not Path(self.weights).exists() and self.weights == '.pth':
+                    # use coco pretrained weights
+                    model = Model(self.yolov5_type, ch=3, nc=80, model_cfg=None)  # create
+                    # logger.info(f"Load COCO pretrained yolov5{self.yolov5_type} model")
+                    from tepe.tasks.yolov5 import YOLOv5Trainer
+                    model = YOLOv5Trainer.load_pretrained_weights(
+                        model, self.yolov5_type, self.device, exclude=()
+                    )
+                else:
+                    model = Model(self.yolov5_type, ch=3, nc=self.num_classes, model_cfg=self.model_cfg)  # create
+                    self.load_ckpt(model, self.weights, self.device, load_keys='model')
+                model = model.float().fuse().eval()
+            # Compatibility updates
+            for m in model.modules():
+                if type(m) in [nn.Hardswish, nn.LeakyReLU, nn.ReLU, nn.ReLU6, nn.SiLU, Detect, Model]:
+                    m.inplace = True  # pytorch 1.7.0 compatibility
+                    if type(m) is Detect:
+                        if not isinstance(m.anchor_grid, list):  # new Detect Layer compatibility
+                            delattr(m, 'anchor_grid')
+                            setattr(m, 'anchor_grid', [torch.zeros(1)] * m.nl)
+                elif type(m) is Conv:
+                    m._non_persistent_buffers_set = set()  # pytorch 1.6.0 compatibility
+
+        self.model = model
+        return self.model
+
+    def _get_data_loader(self,
+                         data_path,
+                         batch_size,
+                         augment=False,
+                         workers=8,
+                         rect=False,
+                         pad=0.0,
+                         image_weights=False,
+                         is_train=True):
+        from .datasets import LoadImagesAndLabels
+        from .datasets import InfiniteDataLoader
+
+        stride = max(int(self.model.stride.max()), 32)
+        transform_hyp = {
+            'hsv_h': 0.015,  # image HSV-Hue augmentation (fraction)
+            'hsv_s': 0.7,  # image HSV-Saturation augmentation (fraction)
+            'hsv_v': 0.4,  # image HSV-Value augmentation (fraction)
+            'degrees': 0.0,  # image rotation (+/- deg)
+            'translate': 0.1,  # image translation (+/- fraction)
+            'scale': 0.5,  # image scale (+/- gain)
+            'shear': 0.0,  # image shear (+/- deg)
+            'perspective': 0.0,  # image perspective (+/- fraction), range 0-0.001
+            'flipud': 0.0,  # image flip up-down (probability)
+            'fliplr': 0.5,  # image flip left-right (probability)
+            'mosaic': 1.0,  # image mosaic (probability)
+            'mixup': 0.0,  # image mixup (probability)
+            'copy_paste': 0.0,  # segment copy-paste (probability)
+        }
+        transform_hyp.update(self.transform_hyp)
+        dataset = LoadImagesAndLabels(
+            data_path,
+            classes=self.CLASS,
+            img_size=self.input_size[0] if isinstance(self.input_size, tuple) else self.input_size,
+            batch_size=batch_size,
+            augment=augment,  # 使用Albumentations进行辅助增强
+            hyp=transform_hyp,  # augmentation hyper-parameters
+            rect=rect,  # 对输入大小进行排序，使一个batch内的图像大小尽可能相似
+            cache_images=self.cache,  # 将所有图像缓存到内存中，加速训练
+            single_cls=self.single_cls,  # 所有类别视为一类训练
+            stride=int(stride),
+            pad=pad,
+            image_weights=image_weights,  # use weighted image selection for training
+            include_class=self.include_class_idx,
+            is_train=is_train,
+            dataset_format=self.dataset_format
+        )
 
-        return model
+        batch_size = min(batch_size, len(dataset))
+        num_workers = min([
+            os.cpu_count(), batch_size if batch_size > 1 else 0, workers])  # number of workers
+        sampler = None
+        loader = DataLoader if image_weights else InfiniteDataLoader
+
+        dataloader = loader(dataset,
+                            batch_size=batch_size,
+                            num_workers=num_workers,
+                            sampler=sampler,
+                            pin_memory=True,
+                            collate_fn=LoadImagesAndLabels.collate_fn)
+        return dataloader, dataset
 
-    def train(self):
-        from torch.utils.tensorboard import SummaryWriter
-        from tepe.utils.general import (
-            init_seeds,
-            save_task_config_py,
-            setup_logger
+    def get_train_loader(self):
+        kwargs = dict(
+            augment=True,
+            workers=self.workers,
+            rect=False,
+            pad=0.0,
+            image_weights=False,
+            is_train=True
         )
-        from tepe.modules.scheduler import create_scheduler
-        from tepe.tasks.rd.find_thr import find_hard_samples
-        
-        init_seeds(self.seed)
-        
-        # dist info
-        rank = get_rank()
-        local_rank = get_local_rank()
-        device = "cuda:{}".format(self.local_rank)
-
-        save_dir = self.output_dir + f'/{self.scene}'
-        if rank == 0:
-            os.makedirs(save_dir, exist_ok=True)
-
-        # save args
-        # save_task_attr_to_yaml(self, save_dir)
-        save_task_config_py(self, save_dir)
-
-        # save log text
-        setup_logger(save_file=os.path.join(save_dir, 'train_log.txt'))  # logger
-        if rank == 0:
-            tblogger = SummaryWriter(save_dir)  # tensorboard
-
-        torch.cuda.set_device(local_rank)
-        model = self.get_model()  #.to(self.device).train()
-        if self.is_distributed:
-            model = DDP(model, device_ids=[local_rank], broadcast_buffers=False)
-        model.train()
-        model.encoder.eval()
-        
-        optimizer = torch.optim.Adam(
-            list(model.decoder.parameters()) + list(model.bn.parameters()),
-            lr=self.learning_rate, betas=(0.5,0.999), weight_decay=self.weight_decay
+
+        self.train_loader, self.train_dataset = self._get_data_loader(
+            self.data_root, self.batch_size, **kwargs)
+        return self.train_loader, self.train_dataset
+
+    def get_eval_loader(self):
+        kwargs = dict(
+            augment=False,
+            workers=self.workers // 2,
+            rect=True,
+            pad=0.5,
+            image_weights=False,
+            is_train=False
         )
-        lr_scheduler, num_epoch = create_scheduler(self, self.sched_type, optimizer)
 
-        self.train_dataloader = self.get_train_loader()
+        val_loader, val_dataset = self._get_data_loader(self.data_root, self.batch_size, **kwargs)
+        return val_loader
 
-        logger.info('Training start...')
-        for epoch in range(1, num_epoch + 1):
-            loss_list = []
-            for data in self.train_dataloader:
-                img = data['img'].to(self.device)
-                loss = model(img)
-                optimizer.zero_grad()
-                loss.backward()
-                optimizer.step()
-                loss_list.append(loss.item())
-            
-            # get current lr
-            lrl = [param_group['lr'] for param_group in optimizer.param_groups]
-            lr = sum(lrl) / len(lrl)
-            if lr_scheduler is not None:
-                lr_scheduler.step(epoch + 1)  # update lr
-            
-            # logger
-            logger.info('epoch [{}/{}], loss:{:.4f}, lr:{:.5f}'.format(epoch, num_epoch, np.mean(loss_list), lr))
-            if rank == 0:
-                tblogger.add_scalar(tag=f'{self.scene}/loss', scalar_value=np.mean(loss_list), global_step=epoch)
-                tblogger.add_scalar(tag=f'{self.scene}/lr', scalar_value=lr, global_step=epoch)
-                
-            # save model
-            if epoch % 5 == 0 or epoch == num_epoch:
-                synchronize()
-                self.weights = os.path.join(save_dir, f'{self.feature_extractor}_rd_{self.scene}.pth')
-                torch.save({'model': model.state_dict(),
-                            'epoch': epoch}, self.weights)
-                logger.info(f"model save in {self.weights}")
-
-            # hard sample mining
-            if epoch > num_epoch - 30 and epoch % 5 == 0 and epoch != num_epoch:
-                select_paths = find_hard_samples(model, self.train_dataloader,
-                                                 self.device, mining_thr=self.threshold * 0.75)
-                model.train()
-                model.encoder.eval()
-                if len(select_paths):
-                    dataset = self.train_dataloader.dataset
-                    dataset.add_hard_samples(select_paths)
-                    # update train dataloader
-                    self.train_dataloader = DataLoader(
-                        self.train_data, batch_size=self.batch_size,
-                        shuffle=True, num_workers=self.workers
-                    )
+    def get_optimizer(self):
 
-        # from tepe.tasks.rd.find_thr import find
-        # self.threshold = find(model, self.train_dataloader, thr_dataloader, self.device)
-        # logger.info(f"find a appropriate threshold: {self.threshold}")
+        self.nbs = 64  # nominal batch size
+        self.accumulate = max(round(self.nbs / self.batch_size), 1)  # accumulate loss before optimizing
+        self.weight_decay *= self.batch_size * self.accumulate / self.nbs  # scale weight_decay
+        logger.info(f"Scaled weight_decay = {self.weight_decay}")
+
+        pg0, pg1, pg2 = [], [], []  # optimizer parameter groups
+
+        for k, v in self.model.named_modules():
+            if hasattr(v, "bias") and isinstance(v.bias, nn.Parameter):
+                pg2.append(v.bias)  # biases
+            if isinstance(v, nn.BatchNorm2d) or "bn" in k:
+                pg0.append(v.weight)  # no decay
+            elif hasattr(v, "weight") and isinstance(v.weight, nn.Parameter):
+                pg1.append(v.weight)  # apply decay
+
+        if self.adam:
+            optimizer = torch.optim.Adam(
+                pg0, lr=self.learning_rate, betas=(self.momentum, 0.999))  # adjust beta1 to momentum
+        else:
+            optimizer = torch.optim.SGD(
+                pg0, lr=self.learning_rate, momentum=self.momentum, nesterov=True
+            )
+        optimizer.add_param_group(
+            {"params": pg1, "weight_decay": self.weight_decay}
+        )  # add pg1 with weight_decay
+        optimizer.add_param_group({"params": pg2})
+        logger.info(f"{colorstr('optimizer:')} {type(optimizer).__name__} with parameter groups "
+                    f"{len(pg0)} weight, {len(pg1)} weight (no decay), {len(pg2)} bias")
+        self.optimizer = optimizer
+
+        del pg0, pg1, pg2
+
+        return self.optimizer
+
+    def get_evaluator(self, train=False):
+        from .yolov5_evaluator import YOLOv5Evaluator
+
+        dataloader = self.get_eval_loader()
+        evaluator = YOLOv5Evaluator(dataloader=dataloader,
+                                    img_size=self.input_size,
+                                    num_classes=self.num_classes,
+                                    save_result=True,
+                                    save_dir=self.output_dir,
+                                    conf_thre=self.conf_thre,
+                                    nms_thre=self.nms_thre,
+                                    single_cls=False,
+                                    device=self.device,
+                                    training=train
+                                    )
+        return evaluator
 
-        self.set_post_info(scene=self.scene, thr=self.threshold)
+    def train(self):
+        from .yolov5_trainer import Trainer
+        trainer = Trainer(self)
+        trainer.train()
 
     def eval(self):
-        from tepe.data.infer_datasets import LoadImages1
-        from .evalutor import read_xml, cal_true_positive
-
-        predictor = self.get_predictor()
-        eval_data_root = os.path.join(self.data_root, self.scene, 'test')
+        model = self.get_model(train=False)
+        evaluator = self.get_evaluator(train=False)
+        evaluator.evaluate(model)
+
+    def get_predictor(self):
+        from tepe.tasks.yolov5 import YOLOv5Predictor
+
+        model = self.get_model(train=False) if Path(self.weights).suffix in '.pth' else None
+        self.predictor = YOLOv5Predictor(
+            weights=self.weights, model=model,
+            imgsz=self.input_size, classes=self.CLASS,
+            conf_thres=self.conf_thre, iou_thres=self.nms_thre,
+            device=self.device, save_dir=self.output_dir,
+            half=self.fp16, 
+        )
+        return self.predictor
 
-        all_precision = {}
-        all_recall = {}
+    def predict(self, source, view_img=False, save_img=True):
+        if "predictor" not in self.__dict__:
+            self.predictor = self.get_predictor()
+        
+        self.predictor.predict(source, view_img, save_img)
 
-        for bad_name in os.listdir(eval_data_root):
-            dataset = LoadImages1(os.path.join(eval_data_root, bad_name))
-            gt_dir = os.path.join(self.data_root, self.scene, 'ground_truth', bad_name)
-
-            total_pred, total_gt, total_rtp, total_ptp = 0, 0, 0, 0
-            for idx, data in enumerate(dataset):
-                img_path = data['path']
-                # get prediction
-                results = predictor.run(data)
-                pred = torch.Tensor(results['anomaly_area'])
-
-                # get ground-truth
-                img_name = os.path.basename(data['path'])
-                xml_path = os.path.join(
-                    gt_dir, img_name.replace(img_name.rsplit('.', maxsplit=1)[-1], 'xml')
-                )
-                if not os.path.exists(xml_path):
-                    logger.warning(f'not found {xml_path}')
-                    continue
-                gt = read_xml(xml_path)
-
-                p_tp, r_tp = cal_true_positive(gt, pred)
-
-                total_pred += len(pred)
-                total_gt += len(gt)
-                total_rtp += r_tp
-                total_ptp += p_tp
-                logger.info(f'[{idx + 1}/{len(dataset)}] {img_path} tp={r_tp}')
-
-            all_precision[bad_name] = total_ptp / total_pred if total_pred > 0 else 1
-            all_recall[bad_name] = total_rtp / total_gt if total_gt > 0 else 1
-
-            logger.info(f'{bad_name} precision: {all_precision[bad_name]}, '
-                        f'recall: {all_recall[bad_name]}')
-
-        # show eval results
-        all_precision['mean'] = sum(list(all_precision.values())) / len(all_precision)
-        all_recall['mean'] = sum(list(all_recall.values())) / len(all_recall)
-        bad_name = list(all_recall.keys())
-        table_header = [" "] + bad_name
-        each_p = ["precision"] + [all_precision[k] for k in bad_name]
-        each_r = ["recall"] + [all_recall[k] for k in bad_name]
-        result_table = [
-            each_p,
-            each_r
-        ]
-        logger.info('eval result:\n{}'.format(
-            tabulate(result_table, headers=table_header, tablefmt="fancy_grid")
-        ))
-
-        return dict(p=all_precision, r=all_recall)
-
-    def get_predictor(self) -> Union[None, Callable]:
-        from tepe.tasks.rd.predictor import Predictor
-
-        onnx_inf = False
-        if os.path.splitext(self.weights)[-1] == '.onnx':
-            logger.info('use onnxruntime for inference')
-            import onnxruntime as ort
-            model = ort.InferenceSession(self.weights)
-            onnx_inf = True
+    def export(self):
+        from tepe.core.exporter import Exporter
+        from tepe.tasks.yolov5.yolo import Conv, Detect
+        from tepe.tasks.yolov5.activations import SiLU
+
+        model = self.get_model(train=False)
+        # Update model
+        if self.fp16:
+            model = model.half()  # to FP16
+        for k, m in model.named_modules():
+            if isinstance(m, Conv):  # assign export-friendly activations
+                if isinstance(m.act, nn.SiLU):
+                    m.act = SiLU()
+            elif isinstance(m, Detect):
+                m.inplace = False
+                m.onnx_dynamic = self.dynamic
+                m.decoding = not self.nodecode
+
+        if self.export_nms:
+            from .common import End2End
+            model = End2End(model, iou_thres=self.nms_thre, score_thres=self.conf_thre, max_obj=100).eval()
+
+        self.batch_size = 1
+        model.to('cpu')
+        exporter = Exporter(self, model=model)
+
+        if 'tensorrt' in self.include:
+            if '7' in self.trt_version:  # TensorRT 7 handling https://github.com/ultralytics/yolov5/issues/6012
+                grid = model.model[-1].anchor_grid
+                model.model[-1].anchor_grid = [a[..., :1, :1, :] for a in grid]
+                exporter.task.opset = 12 # opset 12
+                exporter.task.suffix = '.trt7'
+                exporter.model = model
+                exporter.export(YOLOv5Config.preprocess)
+                model.model[-1].anchor_grid = grid
+            if '8' in self.trt_version:  # TensorRT >= 8
+                exporter.task.opset = 13 # opset 13
+                exporter.task.suffix = '.trt8'
+                exporter.export(YOLOv5Config.preprocess)
         else:
-            model = self.get_model(train=False)
+            exporter.export()
 
-        transform, resize_fn = self.get_transform(mode='test')
-        predictor = Predictor(
-            model=model,
-            resize_fn=resize_fn,
-            input_size=self.input_size,
-            transform=transform,
-            threshold=self.threshold,
-            save_path=self.output_dir,
-            onnx_inf=onnx_inf,
-            save_result=self.save_result,
-            save_xml=self.save_xml,
-            show_heatmap=self.show_heatmap
-        )
 
-        return predictor
+    @staticmethod
+    def preprocess(im, img_size):
+        img = cv2.imread(im)
+        img = letterbox(img, img_size, auto=False, stride=32)[0]
+        img = img.transpose((2, 0, 1))[::-1]  # HWC to CHW, BGR to RGB
+        img = np.ascontiguousarray(img)
+        img = img.astype(np.float32)
+        img /= 255  # 0 - 255 to 0.0 - 1.0
+
+        return img
```

## Comparing `tepe-0.6.9.5.dist-info/LICENSE` & `tepe-0.7.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

